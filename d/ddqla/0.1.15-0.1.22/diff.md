# Comparing `tmp/ddqla-0.1.15.tar.gz` & `tmp/ddqla-0.1.22.tar.gz`

## Comparing `ddqla-0.1.15.tar` & `ddqla-0.1.22.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqla-0.1.15/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ddqla-0.1.15/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ddqla-0.1.15/src/ddqla/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ddqla-0.1.15/src/ddqla/agents/__init__.py
--rw-r--r--   0        0        0     8404 2020-02-02 00:00:00.000000 ddqla-0.1.15/src/ddqla/agents/base_agent.py
--rw-r--r--   0        0        0    14676 2020-02-02 00:00:00.000000 ddqla-0.1.15/test/pacchi.ipynb
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ddqla-0.1.15/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ddqla-0.1.15/LICENSE
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 ddqla-0.1.15/README.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ddqla-0.1.15/pyproject.toml
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 ddqla-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqla-0.1.22/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ddqla-0.1.22/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ddqla-0.1.22/src/ddqla/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ddqla-0.1.22/src/ddqla/agents/__init__.py
+-rw-r--r--   0        0        0     8680 2020-02-02 00:00:00.000000 ddqla-0.1.22/src/ddqla/agents/base_agent.py
+-rw-r--r--   0        0        0    79308 2020-02-02 00:00:00.000000 ddqla-0.1.22/test/pacchi.ipynb
+-rw-r--r--   0        0        0    58255 2020-02-02 00:00:00.000000 ddqla-0.1.22/test/pacchi.jpg
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ddqla-0.1.22/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ddqla-0.1.22/LICENSE
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 ddqla-0.1.22/README.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ddqla-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 ddqla-0.1.22/PKG-INFO
```

### Comparing `ddqla-0.1.15/.github/workflows/python-publish.yml` & `ddqla-0.1.22/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ddqla-0.1.15/src/ddqla/agents/base_agent.py` & `ddqla-0.1.22/src/ddqla/agents/base_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         self.__memory_index = 0
         self._memory_ready = False
         self._memory_batch_size = memory_batch_size
         self.__allow_episode_tracking = allow_episode_tracking
         self.__episodes = []
         self.__actual_episode = BaseAgent.__get_empty_episode()
         self._steps = 0
+        self._tests = 0
+        self.__test_running = False
 
     def start_episode(self, flush=False):
         if self.__allow_episode_tracking and flush:
             self.stop_episode()
         self.__actual_episode = BaseAgent.__get_empty_episode()
 
     def stop_episode(self):
@@ -89,44 +91,48 @@
         x = self._memory_buffer_x
         y = self._memory_buffer_y
         h1 = self._model_1.fit(x, y, verbose=0, batch_size=batch_size)
         h2 = self._model_2.fit(x, y, verbose=0, batch_size=batch_size)
         return h1, h2
 
     def test(self, steps):
+        self._tests += 1
+        self.__test_running = True
         self.reset_state()
         test_rewards = 0
         self.environment_test_log.append(self._state)
         for _ in range(steps):
             pt1 = self._model_1(np.expand_dims(self._state, axis=0), training=False)[0]
             pt2 = self._model_2(np.expand_dims(self._state, axis=0), training=False)[0]
             next_action = np.argmax(pt1 + pt2)
-            test_rewards += self._get_reward(next_action, self._state)
+            test_rewards += self._get_reward(next_action)
             self.environment_test_log.append(self._state)
         self.tests_log.append(test_rewards)
+        self.__test_running = False
         return test_rewards
 
     def step(self):
         rnd = np.random.random()
         action = np.argmax(self.__q) if rnd > self._exploration_rate else np.random.randint(self._num_actions)
-        reward = self._get_reward(action, self._state)
+        reward = self._get_reward(action)
         self._cum_rewards.append(reward)
         if len(self._cum_rewards) > self._cum_rewards_length: self._cum_rewards = self._cum_rewards[1:]
         self.cum_rewards_log.append(np.sum(self._cum_rewards))
         p1 = self._model_1(np.expand_dims(self._state, axis=0), training=False)[0]
         p2 = self._model_2(np.expand_dims(self._state, axis=0), training=False)[0]
         q2 = BaseAgent._max_min(p1, p2)
         self.__q[action] = self.__q[action] * .1 + (reward + np.max(q2) * self._gamma) * .9
         self.__memory_add(self._state, self.__q)
         self.__q = q2
         self._steps += 1
         if self._exploration_rate > 0.05:
             self._exploration_rate -= self._exploration_rate_decay
         if self._steps % self._fit_each_n_steps == 0 and self._memory_ready:
             self._fit(self._memory_batch_size)
+        test_string = "T" + str(self._tests)
         simulation_step = [self._steps]
         for i in range(0, len(self._state)):
             simulation_step.append(self._state[i])
         for i in range(0, self._num_actions):
             simulation_step.append(p1[i].numpy().item())
         for i in range(0, self._num_actions):
             simulation_step.append(p2[i].numpy().item())
@@ -134,14 +140,15 @@
             simulation_step.append(self.__q[i])
         simulation_step.append(rnd)
         simulation_step.append(self._exploration_rate)
         simulation_step.append(1 if rnd > self._exploration_rate else 0)
         simulation_step.append(action)
         simulation_step.append(reward)
         simulation_step.append(np.sum(self._cum_rewards))
+        simulation_step.append(test_string if self.__test_running is True else "")
         self.simulation_log.append(simulation_step)
 
     def get_last_cumulative_rewards(self):
         return np.sum(self._cum_rewards)
 
     def get_simulation_log_headers(self):
         headers = ["step"]
@@ -155,14 +162,15 @@
             headers.append("q_" + str(i))
         headers.append("rnd")
         headers.append("er")
         headers.append("net")
         headers.append("action")
         headers.append("reward")
         headers.append("cum_reward")
+        headers.append("test")
         return headers
 
     def save_simulation_log(self, append_ts=True):
         now = datetime.datetime.now()
         filename = 'simulation_log'
         if append_ts:
             filename += now.strftime("%Y%m%d%H%M%S")
@@ -194,15 +202,15 @@
         plt.show()
 
     @abstractmethod
     def reset_state(self):
         pass
 
     @abstractmethod
-    def _get_reward(self, action, environment):
+    def _get_reward(self, action):
         pass
 
     @abstractmethod
     def _get_model(self, state_features):
         pass
 
     @staticmethod
```

### Comparing `ddqla-0.1.15/LICENSE` & `ddqla-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `ddqla-0.1.15/README.md` & `ddqla-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `ddqla-0.1.15/pyproject.toml` & `ddqla-0.1.22/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ddqla"
-version = "0.1.15"
+version = "0.1.22"
 authors = [{ name="Marco Sarti", email="info@marcosarti.com" }]
 description = "A smart way to create a ddql agent"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `ddqla-0.1.15/PKG-INFO` & `ddqla-0.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddqla
-Version: 0.1.15
+Version: 0.1.22
 Summary: A smart way to create a ddql agent
 Project-URL: Homepage, https://github.com/marco-sarti/ddqla
 Project-URL: Bug Tracker, https://github.com/marco-sarti/ddqla/issues
 Author-email: Marco Sarti <info@marcosarti.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

