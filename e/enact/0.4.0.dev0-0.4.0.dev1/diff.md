# Comparing `tmp/enact-0.4.0.dev0.tar.gz` & `tmp/enact-0.4.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enact-0.4.0.dev0.tar", last modified: Wed Jul 26 00:41:03 2023, max compression
+gzip compressed data, was "enact-0.4.0.dev1.tar", last modified: Sat Aug  5 03:31:58 2023, max compression
```

## Comparing `enact-0.4.0.dev0.tar` & `enact-0.4.0.dev1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-07-26 00:41:03.369570 enact-0.4.0.dev0/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    11357 2023-06-16 23:48:09.000000 enact-0.4.0.dev0/LICENSE
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6858 2023-07-26 00:41:03.369570 enact-0.4.0.dev0/PKG-INFO
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6514 2023-07-25 22:49:47.000000 enact-0.4.0.dev0/README.md
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      451 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/pyproject.toml
--rw-rw-r--   0 leo      (824781618) leo      (824781618)       38 2023-07-26 00:41:03.369570 enact-0.4.0.dev0/setup.cfg
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-07-26 00:41:03.369570 enact-0.4.0.dev0/src/
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-07-26 00:41:03.369570 enact-0.4.0.dev0/src/enact/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2476 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     4889 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/contexts.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3719 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/digests.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    24333 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/guis.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6521 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/interfaces.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    19653 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/invocations.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5913 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/pretty_print.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     9296 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/references.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2565 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/resource_registry.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     4405 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/resource_types.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2367 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/resources.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5755 2023-07-26 00:40:10.000000 enact-0.4.0.dev0/src/enact/serialization.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-07-26 00:41:03.369570 enact-0.4.0.dev0/src/enact.egg-info/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6858 2023-07-26 00:41:03.000000 enact-0.4.0.dev0/src/enact.egg-info/PKG-INFO
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      691 2023-07-26 00:41:03.000000 enact-0.4.0.dev0/src/enact.egg-info/SOURCES.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        1 2023-07-26 00:41:03.000000 enact-0.4.0.dev0/src/enact.egg-info/dependency_links.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)       20 2023-07-26 00:41:03.000000 enact-0.4.0.dev0/src/enact.egg-info/requires.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        6 2023-07-26 00:41:03.000000 enact-0.4.0.dev0/src/enact.egg-info/top_level.txt
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-07-26 00:41:03.369570 enact-0.4.0.dev0/tests/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3427 2023-06-21 14:43:54.000000 enact-0.4.0.dev0/tests/test_contexts.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1392 2023-06-17 00:48:14.000000 enact-0.4.0.dev0/tests/test_digest.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    15113 2023-07-25 22:49:47.000000 enact-0.4.0.dev0/tests/test_invocations.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5055 2023-06-17 00:48:14.000000 enact-0.4.0.dev0/tests/test_references.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1832 2023-06-17 00:48:14.000000 enact-0.4.0.dev0/tests/test_resource_registry.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1611 2023-06-17 00:48:14.000000 enact-0.4.0.dev0/tests/test_resource_types.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     4525 2023-06-21 19:59:29.000000 enact-0.4.0.dev0/tests/test_resources.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2199 2023-06-22 15:27:01.000000 enact-0.4.0.dev0/tests/test_serialize.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-08-05 03:31:58.525300 enact-0.4.0.dev1/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    11357 2023-06-16 23:48:09.000000 enact-0.4.0.dev1/LICENSE
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    10917 2023-08-05 03:31:58.525300 enact-0.4.0.dev1/PKG-INFO
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    10573 2023-08-05 03:19:25.000000 enact-0.4.0.dev1/README.md
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      451 2023-08-05 03:30:40.000000 enact-0.4.0.dev1/pyproject.toml
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)       38 2023-08-05 03:31:58.525300 enact-0.4.0.dev1/setup.cfg
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-08-05 03:31:58.525300 enact-0.4.0.dev1/src/
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-08-05 03:31:58.525300 enact-0.4.0.dev1/src/enact/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2774 2023-08-03 21:52:57.000000 enact-0.4.0.dev1/src/enact/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4946 2023-08-04 22:53:27.000000 enact-0.4.0.dev1/src/enact/contexts.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3990 2023-08-05 03:13:20.000000 enact-0.4.0.dev1/src/enact/digests.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-08-05 03:31:58.525300 enact-0.4.0.dev1/src/enact/gradio/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      668 2023-08-03 22:43:25.000000 enact-0.4.0.dev1/src/enact/gradio/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    24850 2023-08-04 22:53:27.000000 enact-0.4.0.dev1/src/enact/gradio/gradio.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     6849 2023-08-05 03:13:20.000000 enact-0.4.0.dev1/src/enact/interfaces.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    26270 2023-08-05 03:13:20.000000 enact-0.4.0.dev1/src/enact/invocations.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5909 2023-08-05 01:28:09.000000 enact-0.4.0.dev1/src/enact/pretty_print.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     9595 2023-08-04 21:26:57.000000 enact-0.4.0.dev1/src/enact/references.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2607 2023-08-04 22:53:27.000000 enact-0.4.0.dev1/src/enact/resource_registry.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4405 2023-07-26 00:40:10.000000 enact-0.4.0.dev1/src/enact/resource_types.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2367 2023-07-31 21:56:15.000000 enact-0.4.0.dev1/src/enact/resources.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5755 2023-07-26 00:40:10.000000 enact-0.4.0.dev1/src/enact/serialization.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-08-05 03:31:58.525300 enact-0.4.0.dev1/src/enact.egg-info/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    10917 2023-08-05 03:31:58.000000 enact-0.4.0.dev1/src/enact.egg-info/PKG-INFO
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      729 2023-08-05 03:31:58.000000 enact-0.4.0.dev1/src/enact.egg-info/SOURCES.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        1 2023-08-05 03:31:58.000000 enact-0.4.0.dev1/src/enact.egg-info/dependency_links.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)       20 2023-08-05 03:31:58.000000 enact-0.4.0.dev1/src/enact.egg-info/requires.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        6 2023-08-05 03:31:58.000000 enact-0.4.0.dev1/src/enact.egg-info/top_level.txt
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2023-08-05 03:31:58.525300 enact-0.4.0.dev1/tests/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3427 2023-06-21 14:43:54.000000 enact-0.4.0.dev1/tests/test_contexts.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1392 2023-06-17 00:48:14.000000 enact-0.4.0.dev1/tests/test_digest.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    19133 2023-08-04 22:53:27.000000 enact-0.4.0.dev1/tests/test_invocations.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5122 2023-08-03 21:07:34.000000 enact-0.4.0.dev1/tests/test_references.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1832 2023-06-17 00:48:14.000000 enact-0.4.0.dev1/tests/test_resource_registry.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1621 2023-08-03 21:07:34.000000 enact-0.4.0.dev1/tests/test_resource_types.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4526 2023-08-04 22:53:27.000000 enact-0.4.0.dev1/tests/test_resources.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2199 2023-06-22 15:27:01.000000 enact-0.4.0.dev1/tests/test_serialize.py
```

### Comparing `enact-0.4.0.dev0/LICENSE` & `enact-0.4.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `enact-0.4.0.dev0/PKG-INFO` & `enact-0.4.0.dev1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,209 @@
-Metadata-Version: 2.1
-Name: enact
-Version: 0.4.0.dev0
-Summary: A framework for generative software.
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # enact - A Framework for Generative Software.
 
-## Introduction
-
-TODO: Intro, core features.
+Enact is a python framework for building generative software, specifically
+software that integrates with machine learning models or APIs that generate
+distributions of outputs.
+
+The advent of generative AI is driving changes in the way software is built.
+The unique challenges of implementing, maintaining and improving generative
+systems indicate a need to rethink the software stack from a first-principles
+perspective. See [why-enact](#why-enact) for a more in-depth discussion.
+
+The design philosophy of enact is to provide an easy-to-use python framework
+that addresses the needs of emerging AI-based systems in a fundamental manner.
+Enact is designed as a core framework that provides low-level primitives
+required by generative software systems.
+
+To this end, enact provides support for the following features:
+* The ability to commit data, generative components and executions to
+  persistent storage in a versioned manner.
+* Journaled executions of generative python components.
+* The ability to rewind and replay past executions.
+* Easy interchangeability of human and AI-driven subsystems.
+* Support for all of the above features in higher-order generative flows, i.e.,
+  generative programs that generate and execute other generative flows.
+* A simple hash-based storage model that simplifies distributed and
+  asynchronous generative flows.
+
+## Installation and overview
+
+Enact is available as a [pypi package](https://pypi.org/project/enact/) and can
+be installed via:
+
+```bash
+pip install enact
+```
+
+Enact defines generative components as python classes with annotated input and
+output types:
+
+```python
+import enact
+
+import dataclasses
+import random
+
+@enact.typed_invokable(
+  input_type=enact.NoneResource,
+  output_type=enact.Int)
+@dataclasses.dataclass
+class RollDie(enact.Invokable):
+  """An enact invokable that rolls a die."""
+  sides: int
+
+  def call(self):
+    return enact.Int(random.randint(1, self.sides))
+
+
+@enact.typed_invokable(
+  input_type=enact.Int,
+  output_type=enact.Int)
+@dataclasses.dataclass
+class RollDice(enact.Invokable):
+  """An enact invokable that rolls a specified number of dice."""
+  roll: enact.Invokable
+  def call(self, num_dice: enact.Int):
+    return enact.Int(sum(self.roll() for _ in range(num_dice)))
+
+roll_dice = RollDice(RollDie(6))
+print(roll_dice(enact.Int(3)))   # Print sum of 3 rolls.
+```
+
+Executions can be journaled and committed to persistent storage. A journaled
+execution supports rewinding and replaying.
+
+```python
+with enact.FileStore('/tmp/my_store') as store:
+  num_rolls = enact.commit(enact.Int(3))  # commit input to store.
+  invocation = roll_dice.invoke(num_rolls)  # create journaled execution.
+
+  print(invocation.get_output())  # Print sum of 3 rolls
+  for i in range(3):
+    print(invocation.get_child(i).get_output())  # Print each die roll.
+
+  invocation = invocation.rewind()  # Rewind by one dice roll.
+  invocation = invocation.replay()  # Replay dice roll 1 & 2, resample roll 3.
+  print(invocation.get_output())
+```
+
+Human input can be flexibly swapped in for generative components:
+
+```python
+@enact.typed_invokable(enact.NoneResource, enact.Int)
+class HumanRollsDie(enact.Invokable):
+  def call(self):
+    return enact.request_input(
+      enact.Int, context='Please roll a six-sided die')
+
+with store:
+  roll_dice = RollDice(HumanRollsDie())
+  inv_gen = enact.InvocationGenerator(roll_dice, num_rolls)
+  for input_request in inv_gen:
+    inv_gen.set_input(enact.Int(6))  # Provide a roll of 6.
+
+print(inv_gen.invocation.get_output())  # Prints '18'.
+```
+
+## Documentation
+
+Full documentation is work in progress. A quickstart tutorial, explanation of
+enact concepts and examples can be found in the
+[examples directory](https://github.com/agentic-ai/enact/tree/main/examples).
 
 ## Why enact?
 
-With the rise of generative AI models, we are witnessing a significant shift in
-how software systems are conceptualized and built.
+The rise of generative AI models is transforming the software development
+process.
 
-Traditional software relies on functional buildings blocks in which inputs and
-system state directly determine outputs. In contrast, modern AI-powered software
-utilizes generative elements, in which each input is associated with a range of
-possible outputs.
-
-This seemingly small change - from functions to conditional distributions -
-implies a shift in focus across multiple dimensions of the engineering process,
-summarized in the table below.
+Traditional software relies primarily on functional buildings blocks in which
+inputs and system state directly determine outputs. In contrast, modern software
+increasingly utilizes generative AI elements, in which each input is associated
+with a range of possible outputs.
+
+This seemingly small change in emphasis - from functions to conditional
+distributions - implies a shift across multiple dimensions of the engineering
+process, summarized in the table below.
 
 |        |  Traditional  |  Generative  |
 | :----: | :-----------: | :----------: |
 | Building block | Deterministic functions | Conditional distributions |
-| Engineers | Add features, debug errors | Improve output distributions |
+| Engineering | Add features, debug errors | Improve output distributions |
 | Subsystems | Interchangeable | Unique |
 | Code sharing | Frameworks | Components |
 | Executions | Logged for metrics/debugging | Training data |
 | Interactivity | At system boundaries | Within system components |
 | Code vs data | Distinct | Overlapping |
 
 ### Building generative software means fitting distributions
 
 In traditional software, a large part of engineering effort revolves around
 implementing features and debugging errors. In contrast, a generative software
-system may be feature complete and bug-free, but still not suitable for
+system may be feature-complete and bug-free, but still not suitable for
 deployment. Consider the following examples:
 
-* A search chatbot that is feature complete, but becomes rude and unhelpful.
-* An autonomous agent that recursively accomplishes tasks, but has a tendency to
-drift off into behavioral loops.
+* A search chatbot that is sometimes rude and unhelpful
+* An autonomous agent that recursively sets itself goals and accomplishes tasks,
+  but has a tendency to drift off into behavioral loops.
 * An AI avatar generator that produces accurate but unattractive portrait
-images.
+  images.
 
 System correctness is no longer merely a question of specific inputs leading
-to correct outputs, but of the _distribution of outputs_ satisfying some
-quality target when the system is deployed.
+to outputs that are either correct or incorrect, but of the _distribution of
+outputs_ satisfying some implicitly or explicitly defined quality target.
 
 In cases where generativity is localized, e.g., when the software is a thin
 wrapper around a large language model (LLM) or image generator, machine-learning
 tools and techniques can directly be used to improve the system, but in cases
-where multiple generative-components work together to produce an output, or a
-single generative model is called repeatedly, the system must be fitted as a whole
-to the target distributions.
+where multiple generative components work together to produce an output the
+system must be fitted to the target distribution as a whole.
 
 ### Generative software requires recursively swapping subsystems
 
 In traditional software engineering, the choice between two API-identical
 implementations primarily revolves around practicalities such as performance or
 maintainability. However, in generative software, individual components produce
 distributions that may be more or less well-fitted to the system's overall goal,
 for example:
 
-* A foundation text-to-image ML model may perform well on a wide range of
+* A foundation text-to-image model may perform well on a wide range of
 prompts, whereas an API-identical fine-tuned version may be less general but
-produce better results for images in a particular style.
+produce better results for images of a particular style.
 * An instruction-tuned LLM and an LLM trained as a chatbot both autoregressively
-extend token sequences, but one will tend to be better suited towards data
-processing applications, while the other will make a better math tutor.
-
-Generative system outputs are fitted distributions, and their target is only
-implicitly specified. Data selection, training parameters, model composition,
-sampling of feedback and self-improvement flows produce systems whose
-conditional output distributions represent a unique, opinionated take on the
-problem they were trained to solve. Therefore the development of generative
-systems involves recursively swapping out and comparing subsystems.
+extend token sequences, but one may be better suited towards data processing
+applications, while another will make a better math tutor.
+* Different components may have vastly different execution costs.
+
+Generative system outputs are distributions that optimized towards some - often
+implicitly specified - target. Data selection, training parameters, model
+composition, sampling of feedback and self-improvement flows produce systems
+whose conditional output distributions represent a unique, opinionated take on
+the problem they were trained to solve. Therefore the development of generative
+systems motivates ongoing reevaluation, tuning and replacement of subsystems,
+more so than in traditional engineering applications.
 
 ### Generative software should be shareable
 
 There are large numbers of generative AI components that are mutually
 API-compatible (e.g., text-to-image generation, LLMs) but cannot be directly
 ranked in terms of quality since they represent a unique take on the problem
 domain. The combination of API compatibility and variation lends itself to a
 more evolutionary collaborative style than traditional software, where
 shared effort tends to centralize into fewer, lower-level frameworks.
 
-This new collaborative approach is evidenced by:
-* Prompt sharing in image generators and LLMs.
-* Public databases of fine-tuned models.
+This new collaborative approach is already evidenced by widespread sharing of
+prompt templates and the existence of public databases of fine-tuned models.
 
 ### Generative software reflects on its executions.
 
 In conventional software, executions are typically tracked at a low level
 of resolution, since their primary use is to track metrics and debug errors.
 A generative system represents an implicitly specified distribution, and
 its execution history provides valuable information that may be used for
-training.
+analysis or training.
 
 * System outputs can be corrected, scored or critiqued by humans or AI
 models to produce data for fine-tuning.
 * Data from one generative model can be distilled into another.
 * Complex orchestrations of different ML models can be replaced by end-to-end
 trained models once sufficient data is available.
 * Failed executions are potential input data for generative systems, e.g., in
@@ -134,19 +229,15 @@
 Traditional software systems tend to allow a clear distinction between code
 (written by developers) and data (generated by the user and the system). In
 generative systems this distinction breaks down: Approaches such as AutoGPT or
 Voyager use generative AI to generate programs (specified in code or plain
 text), which in turn may be interpreted by generative AI systems; prompts for
 chat-based generative AI could equally be considered code or data.
 
-## Installation
-
-## Quick start
-
-## Usage / Examples
-
-## API Reference
-
-## Contributing
-
+## Development and Contributing
 
+Enact is currently in alpha release. The framework is open source and Apache
+licensed. We are actively looking for contributors that are excited about the
+vision.
 
+You can download the source code, report issues and create pull requests at
+https://github.com/agentic-ai/enact.
```

### Comparing `enact-0.4.0.dev0/src/enact/__init__.py` & `enact-0.4.0.dev1/src/enact/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,24 +22,25 @@
 from enact.interfaces import ResourceDict
 
 from enact.invocations import ExceptionResource
 from enact.invocations import InputChanged
 from enact.invocations import InputRequest
 from enact.invocations import InputRequestOutsideInvocation
 from enact.invocations import RequestedTypeUndetermined
+from enact.invocations import InvocationGenerator
 from enact.invocations import Invokable
 from enact.invocations import InvokableBase
 from enact.invocations import InvokableBase
 from enact.invocations import Invocation
 from enact.invocations import ReplayContext
 from enact.invocations import ReplayError
 from enact.invocations import Request
 from enact.invocations import Response
-from enact.invocations import request_input
 from enact.invocations import RequestInput
+from enact.invocations import request_input
 from enact.invocations import typed_invokable
 from enact.invocations import WrappedException
 
 from enact.pretty_print import pformat
 from enact.pretty_print import pprint
 from enact.pretty_print import PPrinter
 from enact.pretty_print import PPValue
@@ -47,24 +48,28 @@
 from enact.references import commit
 from enact.references import get
 from enact.references import FileBackend
 from enact.references import InMemoryBackend
 from enact.references import Ref
 from enact.references import RefError
 from enact.references import Store
+from enact.references import InMemoryStore
+from enact.references import FileStore
 
 from enact.resources import Resource
 
 from enact.resource_registry import register
 from enact.resource_registry import Registry
 
 from enact.resource_types import Image
 from enact.resource_types import Int
 from enact.resource_types import Float
 from enact.resource_types import Str
 from enact.resource_types import Bytes
 from enact.resource_types import NPArray
 
-
-from enact.guis import GUI
+from enact.serialization import Serializer
+from enact.serialization import JsonSerializer
+from enact.serialization import SerializationError
+from enact.serialization import DeserializationError
 
 from enact import contexts
```

### Comparing `enact-0.4.0.dev0/src/enact/contexts.py` & `enact-0.4.0.dev1/src/enact/contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,18 @@
 
 _context_vars: Dict[Type['Context'],
                     contextvars.ContextVar[Optional['Context']]] = {}
 
 
 class ContextError(Exception):
   """Error raised when there is a problem with the context."""
-  pass
 
 
 class NoActiveContext(ContextError):
   """Raised when there is no active context."""
-  pass
 
 C = TypeVar('C', bound='Context')
 
 
 class Context:
   """A thread-aware context superclass."""
 
@@ -43,18 +41,18 @@
     self._token: Optional[contextvars.Token[Optional[C]]] = None
 
   @classmethod
   def _get_context_var(cls: Type[C]) -> contextvars.ContextVar[Optional[C]]:
     """Returns the context var for this type."""
     try:
       return cast(contextvars.ContextVar[Optional[C]], _context_vars[cls])
-    except KeyError:
+    except KeyError as key_error:
       raise ContextError(
         f'Context {cls} not registered. A context class must be registered '
-        f'with the "@register" decorator.')
+        f'with the "@register" decorator.') from key_error
 
   @classmethod
   @contextlib.contextmanager
   def top_level(cls: Type[C]):
     """Returns a context manager to execute code in a top-level context."""
     context_var = cls._get_context_var()
     token = context_var.set(None)
@@ -65,19 +63,20 @@
 
   @classmethod
   def get_current(cls: Type[C]) -> Optional[C]:
     """Returns the current context of this type or None."""
     context_var = cls._get_context_var()
     try:
       current_context = context_var.get()
-    except LookupError:
+    except LookupError as lookup_error:
       raise ContextError(
         f'Context {cls} not initialized. If running inside a thread, make sure '
         f'to annotate the thread function with either the '
-        f'"@with_current_contexts" or "@with_new_contexts" decorator.')
+        f'"@with_current_contexts" or "@with_new_contexts" decorator.'
+        ) from lookup_error
     return current_context
 
   @classmethod
   def current(cls: Type[C]) -> C:
     """Returns the current context of this type or raises an error."""
     context = cls.get_current()
     if context is None:
```

### Comparing `enact-0.4.0.dev0/src/enact/digests.py` & `enact-0.4.0.dev1/src/enact/digests.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 Value = Union[
   interfaces.FieldValue,
   interfaces.ResourceDictValue]
 
 
 def type_digest(cls: Type[interfaces.ResourceBase]) -> str:
   """Return a digest of the type of resource."""
-  hash = hashlib.sha256()
-  hash.update(cls.__module__.encode('utf-8'))
-  hash.update(b'.')
-  hash.update(cls.__qualname__.encode('utf-8'))
-  for field in cls.field_names():
-    hash.update(repr(field).encode('utf-8'))
-  return hash.hexdigest()
+  hash_obj = hashlib.sha256()
+  hash_obj.update(cls.__module__.encode('utf-8'))
+  hash_obj.update(b'.')
+  hash_obj.update(cls.__qualname__.encode('utf-8'))
+  for field in sorted(cls.field_names()):
+    hash_obj.update(repr(field).encode('utf-8'))
+  return hash_obj.hexdigest()
 
 
 def _digest(
     value: Value,
-    hash: Any,
+    hash_obj: Any,
     stack: List[int]):
   """Recursively compute digest over a field value.
 
   Args:
     value: The value to digest.
     hash: A hash object with an update method, e.g., hashlib.sha256().
   """
@@ -50,68 +50,69 @@
     raise interfaces.FieldTypeError(
       'Cyclic references are not allowed in field values.')
   stack.append(id(value))
   if isinstance(value, (interfaces.ResourceBase,
                         interfaces.ResourceDict)):
     if isinstance(value, interfaces.ResourceBase):
       res_type = type(value)
-      items = value.field_items()
+      # Use alphabetical ordering.
+      items = sorted(value.field_items(), key=lambda x: x[0])
     else:
       assert isinstance(value, interfaces.ResourceDict)
       res_type = value.type
-      items = value.items()
-    hash.update(b'res[')
-    hash.update(res_type.type_id().encode('utf-8'))
+      items = sorted(value.items(), key=lambda x: x[0])
+    hash_obj.update(b'res[')
+    hash_obj.update(res_type.type_id().encode('utf-8'))
     for k, v in items:
-      hash.update(repr(k).encode('utf-8'))
-      _digest(v, hash, stack)
-    hash.update(b']')
+      hash_obj.update(repr(k).encode('utf-8'))
+      _digest(v, hash_obj, stack)
+    hash_obj.update(b']')
   elif isinstance(value, int):
-    hash.update(b'i')
-    hash.update(repr(int(value)).encode('utf-8'))
+    hash_obj.update(b'i')
+    hash_obj.update(repr(int(value)).encode('utf-8'))
   elif isinstance(value, float):
-    hash.update(b'f')
-    hash.update(repr(value).encode('utf-8'))
+    hash_obj.update(b'f')
+    hash_obj.update(repr(value).encode('utf-8'))
   elif isinstance(value, str):
-    hash.update(b's')
-    hash.update(repr(value).encode('utf-8'))
+    hash_obj.update(b's')
+    hash_obj.update(repr(value).encode('utf-8'))
   elif isinstance(value, bytes):
-    hash.update(b'b')
-    hash.update(value)
+    hash_obj.update(b'b')
+    hash_obj.update(value)
   elif value is True:
-    hash.update(b'1')
+    hash_obj.update(b'1')
   elif value is False:
-    hash.update(b'0')
+    hash_obj.update(b'0')
   elif value is None:
-    hash.update(b'n')
+    hash_obj.update(b'n')
   elif isinstance(value, Sequence):
-    hash.update(b'seq[')
+    hash_obj.update(b'seq[')
     for item in value:
-      _digest(item, hash, stack)
-    hash.update(b']')
+      _digest(item, hash_obj, stack)
+    hash_obj.update(b']')
   elif isinstance(value, Mapping):
-    hash.update(b'map[')
-    for k, v in value.items():
+    hash_obj.update(b'map[')
+    for k, v in sorted(value.items(), key=lambda x: x[0]):
       if not isinstance(k, str):
         raise interfaces.FieldTypeError('Map keys must be strings')
-      hash.update(repr(k).encode('utf-8'))
-      _digest(v, hash, stack)
-    hash.update(b']')
+      hash_obj.update(repr(k).encode('utf-8'))
+      _digest(v, hash_obj, stack)
+    hash_obj.update(b']')
   elif issubclass(value, interfaces.ResourceBase):
     # Type of resource.
-    hash.update(b'type[')
-    hash.update(value.type_id().encode('utf-8'))
-    hash.update(b']')
+    hash_obj.update(b'type[')
+    hash_obj.update(value.type_id().encode('utf-8'))
+    hash_obj.update(b']')
   else:
     raise interfaces.FieldTypeError(
       f'Got unexpected field type: {type(value)}. '
       f'Allowed fields types are: int, float, str, bytes, bool, None and '
       f'Ref, and nested maps from strings or sequences of these types.')
   stack.pop()
 
 
 def digest(resource: Union[interfaces.ResourceDict,
                            interfaces.ResourceBase]) -> str:
   """Compute a digest of a resource or a dict representation."""
-  hash = hashlib.sha256()
-  _digest(resource, hash, [])
-  return hash.hexdigest()
+  hash_obj = hashlib.sha256()
+  _digest(resource, hash_obj, [])
+  return hash_obj.hexdigest()
```

### Comparing `enact-0.4.0.dev0/src/enact/guis.py` & `enact-0.4.0.dev1/src/enact/gradio/gradio.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,15 @@
     """Set from an event."""
     def _set(*args):
       resource = fun(*args)
       updates = self.set(resource, **kwargs)
       if len(updates) == 1:
         # Gradio needs unpacking for singleton lists.
         return updates[0]
-      else:
-        return updates
+      return updates
     return event(
       contexts.with_current_contexts(_set),
       inputs=inputs,
       outputs=self.components)
 
 
 RW = TypeVar('RW', bound='RefWidget')
@@ -120,15 +119,15 @@
     def changed_ref_id(ref_id: str) -> Dict:
       """Performs necessary updates when ref id changes."""
       try:
         ref: references.Ref = references.Ref.from_id(ref_id)
       except json.JSONDecodeError:
         return self.ref_details.update(value='Invalid reference id.')
       try:
-        resource = ref.get()
+        resource = ref()
       except references.NotFound:
         return self.ref_details.update(value='Reference not found.')
       return self.ref_details.update(
         value=f'```\n{pretty_print.pformat(resource)}\n```')
 
     self.change(contexts.with_current_contexts(changed_ref_id),
                 inputs=[self.digest_box],
@@ -297,20 +296,20 @@
     self._input_required_inputs = input_required_inputs or [
       resource_types.Str
     ]
     self._input_required_outputs = input_required_outputs or [
       resource_types.Str
     ]
 
-    input_type = self._invokable.get().get_input_type()
+    input_type = self._invokable().get_input_type()
     if not input_type:
       raise ValueError('Input type must be specified.')
     self._input_type: Type[interfaces.ResourceBase] = input_type
 
-    output_type = self._invokable.get().get_output_type()
+    output_type = self._invokable().get_output_type()
     if not output_type:
       raise ValueError('Output type must be specified.')
     self._output_type: Type[interfaces.ResourceBase] = output_type
 
     self._blocks: Optional[gr.Blocks] = None
     self._input_widget: Optional[ResourceWidget] = None
     self._output_widget: Optional[ResourceWidget] = None
@@ -324,32 +323,37 @@
     self.register(JsonFieldWidget)
     self.register(RefWidget)
     self.register(StrWidget)
     self.register(ImageWidget)
 
   @property
   def input_widget(self) -> ResourceWidget:
+    """Input widget of GUI."""
     assert self._input_widget, 'Blocks not generated yet.'
     return self._input_widget
 
   @property
   def output_widget(self) -> ResourceWidget:
+    """Output widget of GUI."""
     assert self._output_widget, 'Blocks not generated yet.'
     return self._output_widget
 
   @property
   def invocation_widget(self) -> RefWidget:
+    """Invocation widget of GUI."""
     assert self._invocation_widget, 'Blocks not generated yet.'
     return self._invocation_widget
 
   def register(self, resource_widget: Type[ResourceWidget]):
+    """Register a resource widget."""
     self._widget_types.append(resource_widget)
 
   @property
   def blocks(self) -> gr.Blocks:
+    """Blocks object representing the UI."""
     if not self._blocks:
       self._blocks = self._create_blocks()
     return self._blocks
 
   def _create_widget_by_resource_type(
       self, resource_type: Type[interfaces.ResourceBase], **kwargs) -> (
         ResourceWidget):
@@ -373,16 +377,16 @@
     if not input_resource:
       return None
     last_invocation = self.invocation_widget.get(*args[len(
       self.input_widget.components):])
     invokable = self._invokable
     if last_invocation:
       assert isinstance(last_invocation, references.Ref)
-      invokable = last_invocation.get().response.get().invokable
-    invocation = invokable.get().invoke(references.commit(input_resource))
+      invokable = last_invocation().response().invokable
+    invocation = invokable().invoke(references.commit(input_resource))
     return references.commit(invocation)
 
   def _continue(self, *args) -> Optional[references.Ref[invocations.Invocation]]:
     """Invoke the object."""
     component_values = list(args)
     invocation_ref = self.invocation_widget.consume(component_values)
     assert isinstance(invocation_ref, references.Ref)
@@ -401,24 +405,24 @@
 
     if user_input is None:
       return None
     continued = raised.continue_invocation(invocation, user_input)
     return references.commit(continued)
 
   def _title(self, ref: references.Ref) -> str:
-    return f'### *{type(ref.get()).__name__}* `{ref.digest[:6]}`'
+    return f'### *{type(ref()).__name__}* `{ref.digest[:6]}`'
 
   def _create_blocks(self) -> gr.Blocks:
     """Return the gradio Blocks object representing the UI."""
     with gr.Blocks() as blocks:
       with gr.Group():
         title = gr.Markdown(value=self._title(self._invokable))
-        with gr.Accordion(label='Resource details', open=False) as details:
+        with gr.Accordion(label='Resource details', open=False):
           invokable_details = gr.Markdown(
-            value=f'```{pretty_print.pformat(self._invokable.get())}```')
+            value=f'```{pretty_print.pformat(self._invokable())}```')
 
       with gr.Group():
         gr.Markdown(value='Input:')
         self._input_widget = self._create_widget_by_resource_type(
           self._input_type)
 
       # Row is a workaround https://github.com/gradio-app/gradio/issues/4505.
@@ -456,15 +460,15 @@
       run_button = gr.Button('Run')
       def get_invocation(*args):
         """Grab the current invocation."""
         ref = self.invocation_widget.get(*args)
         if not ref:
           return None
         assert isinstance(ref, references.Ref)
-        invocation = ref.get()
+        invocation = ref()
         assert isinstance(invocation, invocations.Invocation)
         return invocation
 
       def invocation_input(*args):
         """Return the input of the current invocation."""
         return get_invocation(*args).request().input()
 
@@ -625,10 +629,22 @@
       self._invocation_widget.change(
         contexts.with_current_contexts(update_title),
         inputs=self._invocation_widget.components,
         outputs=[title, invokable_details])
 
       return blocks
 
-  def launch(self, *args, **kwargs) -> Tuple[Any, str, str]:
-      """Launch the gradio UI, passing arguments to Blocks.launch."""
-      return self.blocks.launch(*args, **kwargs)
+  def launch(self, *args, use_queue: bool=True, **kwargs) -> (
+      Tuple[Any, str, Optional[str]]):
+    """Launch the gradio UI, passing arguments to Blocks.launch.
+
+    Args:
+      use_queue: Specify whether queue should be used. The queue is required
+        for executions exceeding 60 seconds.
+
+    Returns:
+      Tuple containing the FastAPI app object running the demo, local URL, and
+      optional public URL if called with share=True.
+    """
+    if use_queue:
+      return self.blocks.queue().launch(*args, **kwargs)
+    return self.blocks.launch(*args, **kwargs)
```

### Comparing `enact-0.4.0.dev0/src/enact/interfaces.py` & `enact-0.4.0.dev1/src/enact/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,33 +76,35 @@
   def type_id(cls) -> str:
     """Returns a string descriptor of the type."""
     return json.dumps(cls.type_descr(), sort_keys=True)
 
   @classmethod
   def field_names(cls) -> Iterable[str]:
     """Returns the names of the fields of the resource."""
-    raise NotImplementedError()
+    raise NotImplementedError(f'{cls} does not implement field_names')
 
   def field_values(self) -> Iterable[FieldValue]:
     """Return a list of field values, aligned with field_names."""
-    raise NotImplementedError()
+    raise NotImplementedError(f'{type(self)} does not implement field_values')
 
   def field_items(self) -> Iterable[Tuple[str, FieldValue]]:
     """Iterate through the field names and values."""
     return zip(self.field_names(), self.field_values())
 
   @classmethod
   def from_fields(cls: Type[C],
                   field_dict: Mapping[str, FieldValue]) -> C:
     """Constructs the resource from a field dictionary."""
     raise NotImplementedError()
 
   @staticmethod
   def _to_dict_value(v: FieldValue) -> ResourceDictValue:
     """Transforms a field value to a resource dict value."""
+    if isinstance(v, ResourceBase):
+      return v.to_resource_dict()
     if isinstance(v, PRIMITIVES):
       return v
     if isinstance(v, type) and issubclass(v, ResourceBase):
       return v
     if isinstance(v, Sequence):
       return [ResourceBase._to_dict_value(x) for x in v]
     if isinstance(v, Mapping):
@@ -110,16 +112,14 @@
         if not isinstance(s, str):
           raise FieldTypeError(
             f'Expected string key, got {type(s)}')
         return s
       return {
         _assert_str(k): ResourceBase._to_dict_value(v)
         for k, v in v.items()}
-    if isinstance(v, ResourceBase):
-      return v.to_resource_dict()
     raise FieldTypeError(
       f'Encountered unsupported field type {type(v)}: {v}')
 
   @staticmethod
   def _from_dict_value(v: ResourceDictValue) -> FieldValue:
     """Transforms a resource dict value to a field value."""
     if isinstance(v, PRIMITIVES):
@@ -178,17 +178,17 @@
       f'Setting fields from another resource is not '
       f'supported by type {type(self)}.')
 
 
 class ResourceDict(Generic[C], dict, Mapping[str, ResourceDictValue]):
   """A dictionary representing a resource with attached type info."""
 
-  def __init__(self, type: Type[C], *args, **kwargs):
+  def __init__(self, resource_type: Type[C], *args, **kwargs):
     super().__init__(*args, **kwargs)
-    self.type = type
+    self.type = resource_type
 
   def to_resource(self) -> C:
     """Constructs the resource from the dictionary."""
     return self.type.from_resource_dict(self)
 
 
 class NoneResource(ResourceBase):
@@ -202,12 +202,17 @@
   def field_values(self) -> Iterable[FieldValue]:
     """Return a list of field values, aligned with field_names."""
     return ()
 
   @classmethod
   def from_fields(
       cls: Type[C],
-      field_values: Mapping[str, FieldValue]) -> C:
+      field_dict: Mapping[str, FieldValue]) -> C:
     """Constructs the resource from a value dictionary."""
-    assert not field_values
+    assert not field_dict
     return cls()
 
+  def set_from(self: C, other: C):
+    """Sets the fields of this resource from another resource."""
+    raise NotImplementedError(
+      f'Setting fields from another resource is not '
+      f'supported by type {type(self)}.')
```

### Comparing `enact-0.4.0.dev0/src/enact/invocations.py` & `enact-0.4.0.dev1/src/enact/invocations.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Functionality for invokable resources."""
+
 import abc
+import collections
 import contextlib
 import dataclasses
 import inspect
-import time
 import traceback
-from typing import Callable, Generic, Iterable, List, Mapping, Optional, Tuple, Type, TypeVar, cast
+from typing import Callable, Generic, Iterable, List, Mapping, Optional, Tuple, Type, TypeVar, Union, cast
 
 
 from enact import contexts
 from enact import interfaces
 from enact import references
 from enact import resources
 from enact import resource_registry
@@ -61,25 +63,25 @@
 
 I_contra = TypeVar('I_contra', contravariant=True, bound=interfaces.ResourceBase)
 O_co = TypeVar('O_co', covariant=True, bound=interfaces.ResourceBase)
 
 
 @resource_registry.register
 class InputRequest(ExceptionResource):
-  """An exception indicating that external input is required.."""
+  """An exception indicating that external input is required."""
 
   def __init__(
       self,
       invokable: references.Ref['InvokableBase'],
       input: references.Ref,
       requested_output: Type[interfaces.ResourceBase],
       context: interfaces.FieldValue):
     if not references.Store.get_current():
       raise contexts.NoActiveContext(
-        'InputRequired must be created within a Store context.')
+        'InputRequest must be created within a Store context.')
     super().__init__(
       invokable,
       input,
       requested_output,
       context)
 
   @property
@@ -135,20 +137,22 @@
 
 
 @resource_registry.register
 class RequestedTypeUndetermined(InvocationError):
   """Raised when the requested type cannot be determined."""
 
 
-def request_input(
-    requested_type: Optional[Type[interfaces.ResourceBase]]=None,
+def _request_input(
+    for_resource: Optional[interfaces.ResourceBase],
+    requested_type: Optional[Type[interfaces.ResourceBase]],
     context: interfaces.FieldValue=None):
   """Requests an input from a user or external system.
 
   Args:
+    for_resource: The resource for which input is requested.
     requested_type: The type of input requested. If not specified, the type will
       be inferred to be the output type of the current invocation.
     context: Anything that provides context for the request.
   Raises:
     InputRequest: The input request exception.
     InputRequestOutsideInvocation: If the request was made outside an invocation.
   """
@@ -157,15 +161,15 @@
     raise InputRequestOutsideInvocation(context, requested_type)
   requested_type = requested_type or builder.invokable.get_output_type()
   if not requested_type:
     raise RequestedTypeUndetermined(
       'Requested type must be specified when output type is undetermined.')
   raise InputRequest(
     references.commit(builder.invokable),
-    builder.input_ref,
+    references.commit(for_resource),
     requested_type,
     context)
 
 
 @resource_registry.register
 @dataclasses.dataclass
 class Request(Generic[I_contra, O_co], resources.Resource):
@@ -199,20 +203,14 @@
 
 @resource_registry.register
 @dataclasses.dataclass
 class Invocation(Generic[I_contra, O_co], resources.Resource):
   """An invocation."""
   request: references.Ref[Request[I_contra, O_co]]
   response: references.Ref[Response[I_contra, O_co]]
-  timestamp_ns: int = dataclasses.field(default_factory=lambda: Invocation.now())
-
-  @classmethod
-  def now(cls) -> int:
-    """Returns the current timestamp."""
-    return time.time_ns()
 
   def successful(self) -> bool:
     """Returns true if the invocation completed successfully."""
     if not self.response:
       return False
     return self.response().output is not None
 
@@ -231,19 +229,34 @@
   def get_raised_here(self) -> bool:
     """Whether the exception was originally raised here or in a child."""
     response = self.response()
     assert response.raised, 'No exception was raised.'
     return response.raised_here
 
   def get_children(self) -> Iterable['Invocation']:
-    """Yields the child invocations or raises assertion error."""
+    """Yields the child invocations."""
     children = self.response().children
     for child in children:
       yield child()
 
+  def get_child(self, index: int) -> 'Invocation':
+    """Returns the child invocation corresponding to the index."""
+    children = self.response().children
+    return children[index]()
+
+  def rewind(self, num_calls=1) -> 'Invocation[I_contra, O_co]':
+    """Rewinds the invocation by the specified number of calls."""
+    invocation = self.deep_copy_resource()
+    with invocation.response.modify() as response:
+      response.output = None
+      for _ in range(num_calls):
+        if response.children:
+          response.children.pop(-1)
+    return invocation
+
   def replay(
       self,
       exception_override: ExceptionOverride=lambda x: None,
       strict: bool=True) -> (
         'Invocation[I_contra, O_co]'):
     """Replay the invocation, retrying exceptions or overiding them."""
     return self.request().invokable().invoke(
@@ -314,16 +327,16 @@
       if (child.request().invokable == references.commit(invokable) and
           child.request().input == references.commit(input)):
         break
       elif self._strict:
         raise ReplayError(
           f'Expected invocation {invokable}({input}) but got '
           f'{child.request().invokable()}({child.request().input()}).\n'
-          f'Ensure that all non-deterministic functions are wrapped in '
-          f'invokables or use strict=False.')
+          f'Ensure that calls to subinvokable are deterministic '
+          f'or use strict=False.')
     else:
       # No matching replay found.
       return None, ReplayContext([], self._exception_override)
 
     # Consume child invocation
     self._available_children.pop(i)
     response = child.response()
@@ -336,28 +349,30 @@
         self._exception_override,
         self._strict)
 
     # Check for exception override
     if response.raised and response.raised_here:
       # Only override exceptions raised in the current frame.
       override = self._exception_override(response.raised)
+      invokable.set_from(response.invokable())
       if override is not None:
         # Typecheck the override.
         output_type = invokable.get_output_type()
         if output_type and not isinstance(override, output_type):
           raise InvokableTypeError(
             f'Exception override {override} is not of required type '
             f'{invokable.get_input_type()}.')
         # Set invokable from response.
-        invokable.set_from(response.invokable())
         return (
           cast(O_co, override),
           ReplayContext(child.get_children(),
                         self._exception_override,
                         self._strict))
+      # No override found.
+      raise response.raised()
 
     # Trigger reexecution of the invocation.
     return None, ReplayContext(
       child.get_children(), self._exception_override, self._strict)
 
 
 @contexts.register
@@ -409,15 +424,19 @@
           self.invokable, input_resource)
         if references.commit(input_resource) != self.input_ref:
           raise InputChanged(
             f'Input changed during invocation of {self.invokable} on input '
             f'{input_resource}. Only the invokable may change.')
         if output_resource is None:
           output_resource = interfaces.NoneResource()
-        output = references.commit(output_resource)
+        if not isinstance(output_resource, interfaces.ResourceBase):
+          raise InvokableTypeError(
+            f'Invokable {self.invokable} returned {output_resource} '
+            f'which is not a resource.')
+        output = cast(references.Ref[O_co], references.commit(output_resource))
       except ExceptionResource as e:
         python_exc = e
         exception = references.commit(e)
         raise
       except Exception as e:
         python_exc = e
         exception = references.commit(WrappedException(traceback.format_exc()))
@@ -432,15 +451,15 @@
           references.commit(self.invokable), output,
           exception, raised_here, self.children)
         self._invocation = Invocation(
           references.commit(self._request),
           references.commit(response))
         if parent:
           parent.record_child(self._invocation)
-      return output_resource
+      return cast(O_co, output_resource)
 
 
 class InvokableBase(Generic[I_contra, O_co], interfaces.ResourceBase):
   """Base class for invokable resources."""
 
   _input_type: Optional[Type[I_contra]] = None
   _output_type: Optional[Type[I_contra]] = None
@@ -496,31 +515,35 @@
 
   def invoke(
       self,
       arg: Optional[references.Ref[I_contra]]=None,
       replay_from: Optional[Invocation[I_contra, O_co]]=None,
       exception_override: ExceptionOverride=lambda _: None,
       raise_on_invocation_error:bool=True,
-      strict: bool=True) -> Invocation[I_contra, O_co]:
+      strict: bool=True,
+      commit: bool=True) -> Invocation[I_contra, O_co]:
     """Invoke the invokable, tracking invocation metadata.
 
     Args:
       arg: The input resource.
       replay_from: An optional invocation to replay form.
       exception_override: If replaying, an optional override for replayed
         exceptions.
       raise_on_invocation_error: Whether invocation errors should be reraised.
       strict: Whether replay should fail if the replayed invocation
         does not match the current invocation.
+      commit: Whether to commit the new invocation object.
     Returns:
       The invocation generated.
     """
     if arg is None:
       arg = cast(references.Ref[I_contra],
                  references.commit(interfaces.NoneResource()))
+    if not isinstance(arg, references.Ref):
+      raise InvokableTypeError('Input must be a reference.')
 
     exit_stack = contextlib.ExitStack()
     # Execute in a top-level context to ensure that there are no parents.
     exit_stack.enter_context(Builder.top_level())
     if replay_from:
       exit_stack.enter_context(ReplayContext.top_level())
       exit_stack.enter_context(ReplayContext(
@@ -532,14 +555,16 @@
         builder.call()
       except InvocationError:
         if raise_on_invocation_error:
           raise
       except Exception:
         pass  # Do nothing
       invocation = builder.invocation
+    if commit:
+      references.commit(invocation)
     return invocation
 
 
 @dataclasses.dataclass
 class Invokable(InvokableBase[I_contra, O_co], resources.Resource):
   """Base class for dataclass-based invokable resources."""
 
@@ -569,9 +594,162 @@
 @dataclasses.dataclass
 class RequestInput(Invokable):
   """An invokable that raises an InputRequest."""
   requested_type: Type[interfaces.ResourceBase]
   context: Optional[interfaces.FieldValue] = None
 
   def call(self, resource: interfaces.ResourceBase) -> interfaces.ResourceBase:
-    request_input(self.requested_type, self.context)
+    _request_input(resource, self.requested_type, self.context)
     assert False
+
+def request_input(
+    requested_type: Type[C],
+    for_resource: Optional[interfaces.ResourceBase]=None,
+    context: Optional[interfaces.FieldValue]=None) -> C:
+  """Request an input from an external system / user.
+
+  Args:
+    requested_type: The type of input to request.
+    for_resource: The resource to request input for. If unset, defaults to None.
+    context: An optional context to provide to the input request, e.g., instructions
+      to a user.
+  Returns:
+    The requested input. Note that this function will not return a value
+    during normal execution, but will raise an InputRequest exception,
+    which can be used to resume the execution with an injected value.
+  Raises:
+    InputRequest: Raised to halt execution in order to await input.
+  """
+  if for_resource is None:
+    for_resource = interfaces.NoneResource()
+  return RequestInput(requested_type, context)(for_resource)
+
+
+class InvocationGenerator(
+    collections.Generator,
+    Generic[I_contra, O_co]):
+  """A generator that yields InputRequests from an invocation."""
+
+  def __init__(
+      self,
+      invokable: Optional[InvokableBase[I_contra, O_co]]=None,
+      input: Optional[references.Ref[I_contra]]=None,
+      from_invocation: Optional[Invocation[I_contra, O_co]]=None):
+    """Initializes an interactive invocation."""
+    if from_invocation is not None and invokable is not None:
+      raise ValueError(
+        'Cannot specify both an invokable and an invocation.')
+    if from_invocation is not None and input is not None:
+      raise ValueError(
+        'Cannot specify both an input and an invocation.')
+    self._invocation: Optional[Invocation[I_contra, O_co]] = None
+    self._from_invocation = from_invocation
+    self._invokable = invokable
+    self._input = input
+    self._request_input: Optional[interfaces.ResourceBase] = None
+
+  @property
+  def complete(self) -> bool:
+    """Whether the invocation is complete."""
+    if not self._invocation:
+      return False
+    if self._invocation.successful():
+      return True
+    if not self._invocation.response().raised:
+      return False
+    return not isinstance(self._invocation.get_raised(), InputRequest)
+
+  @property
+  def invocation(self) -> Invocation[I_contra, O_co]:
+    """The invocation."""
+    if not self._invocation:
+      raise InvocationError(
+        'Invocation not started, please call next.')
+    return self._invocation
+
+  @property
+  def input_request(self) -> InputRequest:
+    """The current input request."""
+    if self.complete:
+      raise InvocationError('Invocation is complete.')
+    input_request = self.invocation.get_raised()
+    assert isinstance(input_request, InputRequest)
+    return input_request
+
+  def set_input(self, resource: interfaces.ResourceBase):
+    """Set input for the next call to __next__.
+
+    This allows using the generator in iterator-style, e.g.,
+
+      for input_request in invocation_generator:
+        input_request.set_input(...)
+
+    Which can be more convenient than using send():
+
+      input_request = next(invocation_generator)
+      while True:
+        try:
+          input_request.send(...)
+        except StopIteration:
+          break
+
+    Args:
+      resource: The resource to set as input.
+    """
+    self._request_input = resource.deep_copy_resource()
+
+  def __next__(self) -> InputRequest:
+    """Continues the invocation until the next input request or completion."""
+    if self.complete:
+      raise StopIteration()
+
+    if not self._invocation:
+      if self._from_invocation:
+        self._invocation = self._from_invocation.replay()
+      else:
+        assert self._invokable
+        if not self._input:
+          if interfaces.NoneResource != self._invokable._input_type:
+            raise InvocationError(
+              'Invokable does not have input type NoneResource. '
+              'Please provide an explicit input reference on generator '
+              'construction')
+          self._input = cast(references.Ref[I_contra],
+                             references.commit(interfaces.NoneResource()))
+        self._invocation = self._invokable.invoke(self._input)
+      if self.complete:
+        raise StopIteration()
+      return self.input_request
+    else:
+      if self._request_input is None:
+        if not issubclass(interfaces.NoneResource,
+                          self.input_request.requested_type):
+          raise InvocationError(
+            'Invocation requests non-None input. Please use \'send(...)\' '
+            'instead or set the input using \'set_input(...)\'.')
+        self._request_input = interfaces.NoneResource()
+      self._invocation = self.input_request.continue_invocation(
+        self._invocation, self._request_input)
+      self._request_input = None
+      if self.complete:
+        raise StopIteration()
+      return self.input_request
+
+  def send(self, value) -> InputRequest:
+    if not self._invocation:
+      if value is not None:
+        raise TypeError('Can\'t send non-None value to a just-started generator.')
+      return self.__next__()
+    if self.complete:
+      raise StopIteration()
+    if not isinstance(value, self.input_request.requested_type):
+      raise InvokableTypeError(
+        f'Input type {type(value)} does not match requested type: '
+        f'{self.input_request.requested_type}.')
+    self._invocation = self.input_request.continue_invocation(
+      self.invocation, value)
+    if self.complete:
+      raise StopIteration()
+    return self.input_request
+
+  def throw(self, *args, **kwargs):
+    super().throw(*args, **kwargs)
```

### Comparing `enact-0.4.0.dev0/src/enact/pretty_print.py` & `enact-0.4.0.dev1/src/enact/pretty_print.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         for field_name, field_value in v.field_items()],
       open=':',
       close='')
     return result
 
   def from_ref(self, v: interfaces.FieldValue, depth: int) -> PPValue:
     assert isinstance(v, references.Ref)
-    resource: interfaces.ResourceBase = v.get()
+    resource: interfaces.ResourceBase = v()
     if ((self.max_ref_depth and depth > self.max_ref_depth) or
         (self.skip_repeated_refs and v.digest in self._seen_refs)):
       return PPValue(f'-> {type(resource).__name__}#{v.digest[0:6]}', [])
     result = self.pvalue(resource, depth + 1)
     result.value = f'-> {result.value}#{v.digest[0:6]}'
     self._seen_refs.add(v.digest)
     return result
```

### Comparing `enact-0.4.0.dev0/src/enact/references.py` & `enact-0.4.0.dev1/src/enact/references.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 P = TypeVar('P', bound='Ref')
 R = TypeVar('R', bound=interfaces.ResourceBase)
 
 
 def get(ref: Optional['Ref[R]']) -> R:
   """Gets the reference or asserts false if None."""
   assert ref
-  return ref.get()
+  return ref.checkout()
 
 
 def commit(resource: R) -> 'Ref[R]':
   """Commits a resource to the store and returns a reference."""
   return Store.current().commit(resource)
 
 
@@ -92,27 +92,28 @@
     """Returns a string version of this reference."""
     return cls.from_resource_dict(
       interfaces.ResourceDict(cls, **json.loads(id)))
 
   @contextlib.contextmanager
   def modify(self) -> Iterator[R]:
     """Context manager for modifying the resource."""
-    resource = self.get()
+    resource = self.checkout()
     yield resource
+    commit(resource)
     self.set(resource)
 
-  def get(self) -> R:
+  def checkout(self) -> R:
     """Fetches the resource from the cache or active store."""
     if self._cached is None or self.from_resource(self._cached) != self:
-      self._cached = Store.current().get(self)
+      self._cached = Store.current().checkout(self)
     return self._cached
 
   def __call__(self) -> R:
     """Alias for get."""
-    return self.get()
+    return self.checkout()
 
   def set(self, resource: R):
     """Sets the reference to point to the given resource."""
     self._cached = resource
     self._digest = digests.digest(resource)
 
   @classmethod
@@ -121,15 +122,15 @@
     return cls(digest=digests.digest(resource), resource=resource)
 
   def __eq__(self, other: Any):
     """Returns true if the referenced object is the same."""
     if not isinstance(other, Ref):
       return False
     if type(self) != type(other):
-      other = self.from_resource(other.get())
+      other = self.from_resource(other.checkout())
     return self.digest == other.digest
 
   @classmethod
   def verify(cls, packed_resource: PackedResource):
     """Check the integrity of a packed resource.
 
     Args:
@@ -188,15 +189,15 @@
     """Stores a packed resource."""
 
   @abc.abstractmethod
   def has(self, ref: Ref) -> bool:
     """Returns whether the storage backend has the resource."""
 
   @abc.abstractmethod
-  def get(self, ref: Ref) -> Optional[interfaces.ResourceDict]:
+  def checkout(self, ref: Ref) -> Optional[interfaces.ResourceDict]:
     """Returns the packed resource or None if not available."""
 
 
 class NotFound(Exception):
   """Raised when a resource is not found."""
 
 
@@ -212,15 +213,15 @@
     packed_resource.ref.verify(packed_resource)
     self._resources[packed_resource.ref.id] = packed_resource.data
 
   def has(self, ref: Ref) -> bool:
     """Returns whether the backend has the referenced resource."""
     return ref.id in self._resources
 
-  def get(self, ref: Ref) -> Optional[interfaces.ResourceDict]:
+  def checkout(self, ref: Ref) -> Optional[interfaces.ResourceDict]:
     """Returns the packed resource or None if not available."""
     return self._resources.get(ref.id)
 
   def __len__(self) -> int:
     """Returns the number of resources in the backend."""
     return len(self._resources)
 
@@ -243,15 +244,15 @@
       f.write(self._serializer.serialize(
         packed_resource.data))
 
   def has(self, ref: Ref) -> bool:
     """Returns whether the backend has the referenced resource."""
     return os.path.exists(os.path.join(self._root_dir, ref.id))
 
-  def get(self, ref: Ref) -> Optional[interfaces.ResourceDict]:
+  def checkout(self, ref: Ref) -> Optional[interfaces.ResourceDict]:
     """Returns the packed resource or None if not available."""
     with open(os.path.join(self._root_dir, ref.id), 'rb') as f:
       return self._serializer.deserialize(f.read())
 
 
 @contexts.register
 class Store(contexts.Context):
@@ -273,14 +274,24 @@
     self._backend.commit(packed_resource)
     return packed_resource.ref
 
   def has(self, ref: Ref) -> bool:
     """Returns whether the store has a resource."""
     return self._backend.has(ref)
 
-  def get(self, ref: Ref[R]) -> R:
+  def checkout(self, ref: Ref[R]) -> R:
     """Retrieves a resource from the store."""
-    resource_data = self._backend.get(ref)
+    resource_data = self._backend.checkout(ref)
     if resource_data is None:
       raise NotFound(ref.id)
     packed_resource = PackedResource(resource_data, ref=ref)
     return ref.unpack(packed_resource)
+
+
+def InMemoryStore() -> Store:
+  """Returns an in-memory store."""
+  return Store(backend=InMemoryBackend())
+
+
+def FileStore(root_dir: str):
+  """Returns a file-based store."""
+  return Store(backend=FileBackend(root_dir))
```

### Comparing `enact-0.4.0.dev0/src/enact/resource_registry.py` & `enact-0.4.0.dev1/src/enact/resource_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 class Registry:
   """Registers resource types for deserialization."""
 
   _singleton: Optional['Registry'] = None
 
   def __init__(self):
     """Initializes a registry."""
-    self.allow_reregistration = False
+    self.allow_reregistration = True
     self._type_map: Dict[str, Type[interfaces.ResourceBase]] = {}
+    self.register(interfaces.NoneResource)
 
   def register(self, resource: Type[interfaces.ResourceBase]):
     """Registers the resource or reference type."""
     if not issubclass(resource, interfaces.ResourceBase):
       raise RegistryError(
         f'Cannot register non-resource type: {resource}')
     import traceback as tb
```

### Comparing `enact-0.4.0.dev0/src/enact/resource_types.py` & `enact-0.4.0.dev1/src/enact/resource_types.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.0.dev0/src/enact/resources.py` & `enact-0.4.0.dev1/src/enact/resources.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.0.dev0/src/enact/serialization.py` & `enact-0.4.0.dev1/src/enact/serialization.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.0.dev0/src/enact.egg-info/PKG-INFO` & `enact-0.4.0.dev1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,114 +1,220 @@
 Metadata-Version: 2.1
 Name: enact
-Version: 0.4.0.dev0
+Version: 0.4.0.dev1
 Summary: A framework for generative software.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enact - A Framework for Generative Software.
 
-## Introduction
-
-TODO: Intro, core features.
+Enact is a python framework for building generative software, specifically
+software that integrates with machine learning models or APIs that generate
+distributions of outputs.
+
+The advent of generative AI is driving changes in the way software is built.
+The unique challenges of implementing, maintaining and improving generative
+systems indicate a need to rethink the software stack from a first-principles
+perspective. See [why-enact](#why-enact) for a more in-depth discussion.
+
+The design philosophy of enact is to provide an easy-to-use python framework
+that addresses the needs of emerging AI-based systems in a fundamental manner.
+Enact is designed as a core framework that provides low-level primitives
+required by generative software systems.
+
+To this end, enact provides support for the following features:
+* The ability to commit data, generative components and executions to
+  persistent storage in a versioned manner.
+* Journaled executions of generative python components.
+* The ability to rewind and replay past executions.
+* Easy interchangeability of human and AI-driven subsystems.
+* Support for all of the above features in higher-order generative flows, i.e.,
+  generative programs that generate and execute other generative flows.
+* A simple hash-based storage model that simplifies distributed and
+  asynchronous generative flows.
+
+## Installation and overview
+
+Enact is available as a [pypi package](https://pypi.org/project/enact/) and can
+be installed via:
+
+```bash
+pip install enact
+```
+
+Enact defines generative components as python classes with annotated input and
+output types:
+
+```python
+import enact
+
+import dataclasses
+import random
+
+@enact.typed_invokable(
+  input_type=enact.NoneResource,
+  output_type=enact.Int)
+@dataclasses.dataclass
+class RollDie(enact.Invokable):
+  """An enact invokable that rolls a die."""
+  sides: int
+
+  def call(self):
+    return enact.Int(random.randint(1, self.sides))
+
+
+@enact.typed_invokable(
+  input_type=enact.Int,
+  output_type=enact.Int)
+@dataclasses.dataclass
+class RollDice(enact.Invokable):
+  """An enact invokable that rolls a specified number of dice."""
+  roll: enact.Invokable
+  def call(self, num_dice: enact.Int):
+    return enact.Int(sum(self.roll() for _ in range(num_dice)))
+
+roll_dice = RollDice(RollDie(6))
+print(roll_dice(enact.Int(3)))   # Print sum of 3 rolls.
+```
+
+Executions can be journaled and committed to persistent storage. A journaled
+execution supports rewinding and replaying.
+
+```python
+with enact.FileStore('/tmp/my_store') as store:
+  num_rolls = enact.commit(enact.Int(3))  # commit input to store.
+  invocation = roll_dice.invoke(num_rolls)  # create journaled execution.
+
+  print(invocation.get_output())  # Print sum of 3 rolls
+  for i in range(3):
+    print(invocation.get_child(i).get_output())  # Print each die roll.
+
+  invocation = invocation.rewind()  # Rewind by one dice roll.
+  invocation = invocation.replay()  # Replay dice roll 1 & 2, resample roll 3.
+  print(invocation.get_output())
+```
+
+Human input can be flexibly swapped in for generative components:
+
+```python
+@enact.typed_invokable(enact.NoneResource, enact.Int)
+class HumanRollsDie(enact.Invokable):
+  def call(self):
+    return enact.request_input(
+      enact.Int, context='Please roll a six-sided die')
+
+with store:
+  roll_dice = RollDice(HumanRollsDie())
+  inv_gen = enact.InvocationGenerator(roll_dice, num_rolls)
+  for input_request in inv_gen:
+    inv_gen.set_input(enact.Int(6))  # Provide a roll of 6.
+
+print(inv_gen.invocation.get_output())  # Prints '18'.
+```
+
+## Documentation
+
+Full documentation is work in progress. A quickstart tutorial, explanation of
+enact concepts and examples can be found in the
+[examples directory](https://github.com/agentic-ai/enact/tree/main/examples).
 
 ## Why enact?
 
-With the rise of generative AI models, we are witnessing a significant shift in
-how software systems are conceptualized and built.
+The rise of generative AI models is transforming the software development
+process.
 
-Traditional software relies on functional buildings blocks in which inputs and
-system state directly determine outputs. In contrast, modern AI-powered software
-utilizes generative elements, in which each input is associated with a range of
-possible outputs.
-
-This seemingly small change - from functions to conditional distributions -
-implies a shift in focus across multiple dimensions of the engineering process,
-summarized in the table below.
+Traditional software relies primarily on functional buildings blocks in which
+inputs and system state directly determine outputs. In contrast, modern software
+increasingly utilizes generative AI elements, in which each input is associated
+with a range of possible outputs.
+
+This seemingly small change in emphasis - from functions to conditional
+distributions - implies a shift across multiple dimensions of the engineering
+process, summarized in the table below.
 
 |        |  Traditional  |  Generative  |
 | :----: | :-----------: | :----------: |
 | Building block | Deterministic functions | Conditional distributions |
-| Engineers | Add features, debug errors | Improve output distributions |
+| Engineering | Add features, debug errors | Improve output distributions |
 | Subsystems | Interchangeable | Unique |
 | Code sharing | Frameworks | Components |
 | Executions | Logged for metrics/debugging | Training data |
 | Interactivity | At system boundaries | Within system components |
 | Code vs data | Distinct | Overlapping |
 
 ### Building generative software means fitting distributions
 
 In traditional software, a large part of engineering effort revolves around
 implementing features and debugging errors. In contrast, a generative software
-system may be feature complete and bug-free, but still not suitable for
+system may be feature-complete and bug-free, but still not suitable for
 deployment. Consider the following examples:
 
-* A search chatbot that is feature complete, but becomes rude and unhelpful.
-* An autonomous agent that recursively accomplishes tasks, but has a tendency to
-drift off into behavioral loops.
+* A search chatbot that is sometimes rude and unhelpful
+* An autonomous agent that recursively sets itself goals and accomplishes tasks,
+  but has a tendency to drift off into behavioral loops.
 * An AI avatar generator that produces accurate but unattractive portrait
-images.
+  images.
 
 System correctness is no longer merely a question of specific inputs leading
-to correct outputs, but of the _distribution of outputs_ satisfying some
-quality target when the system is deployed.
+to outputs that are either correct or incorrect, but of the _distribution of
+outputs_ satisfying some implicitly or explicitly defined quality target.
 
 In cases where generativity is localized, e.g., when the software is a thin
 wrapper around a large language model (LLM) or image generator, machine-learning
 tools and techniques can directly be used to improve the system, but in cases
-where multiple generative-components work together to produce an output, or a
-single generative model is called repeatedly, the system must be fitted as a whole
-to the target distributions.
+where multiple generative components work together to produce an output the
+system must be fitted to the target distribution as a whole.
 
 ### Generative software requires recursively swapping subsystems
 
 In traditional software engineering, the choice between two API-identical
 implementations primarily revolves around practicalities such as performance or
 maintainability. However, in generative software, individual components produce
 distributions that may be more or less well-fitted to the system's overall goal,
 for example:
 
-* A foundation text-to-image ML model may perform well on a wide range of
+* A foundation text-to-image model may perform well on a wide range of
 prompts, whereas an API-identical fine-tuned version may be less general but
-produce better results for images in a particular style.
+produce better results for images of a particular style.
 * An instruction-tuned LLM and an LLM trained as a chatbot both autoregressively
-extend token sequences, but one will tend to be better suited towards data
-processing applications, while the other will make a better math tutor.
-
-Generative system outputs are fitted distributions, and their target is only
-implicitly specified. Data selection, training parameters, model composition,
-sampling of feedback and self-improvement flows produce systems whose
-conditional output distributions represent a unique, opinionated take on the
-problem they were trained to solve. Therefore the development of generative
-systems involves recursively swapping out and comparing subsystems.
+extend token sequences, but one may be better suited towards data processing
+applications, while another will make a better math tutor.
+* Different components may have vastly different execution costs.
+
+Generative system outputs are distributions that optimized towards some - often
+implicitly specified - target. Data selection, training parameters, model
+composition, sampling of feedback and self-improvement flows produce systems
+whose conditional output distributions represent a unique, opinionated take on
+the problem they were trained to solve. Therefore the development of generative
+systems motivates ongoing reevaluation, tuning and replacement of subsystems,
+more so than in traditional engineering applications.
 
 ### Generative software should be shareable
 
 There are large numbers of generative AI components that are mutually
 API-compatible (e.g., text-to-image generation, LLMs) but cannot be directly
 ranked in terms of quality since they represent a unique take on the problem
 domain. The combination of API compatibility and variation lends itself to a
 more evolutionary collaborative style than traditional software, where
 shared effort tends to centralize into fewer, lower-level frameworks.
 
-This new collaborative approach is evidenced by:
-* Prompt sharing in image generators and LLMs.
-* Public databases of fine-tuned models.
+This new collaborative approach is already evidenced by widespread sharing of
+prompt templates and the existence of public databases of fine-tuned models.
 
 ### Generative software reflects on its executions.
 
 In conventional software, executions are typically tracked at a low level
 of resolution, since their primary use is to track metrics and debug errors.
 A generative system represents an implicitly specified distribution, and
 its execution history provides valuable information that may be used for
-training.
+analysis or training.
 
 * System outputs can be corrected, scored or critiqued by humans or AI
 models to produce data for fine-tuning.
 * Data from one generative model can be distilled into another.
 * Complex orchestrations of different ML models can be replaced by end-to-end
 trained models once sufficient data is available.
 * Failed executions are potential input data for generative systems, e.g., in
@@ -134,19 +240,15 @@
 Traditional software systems tend to allow a clear distinction between code
 (written by developers) and data (generated by the user and the system). In
 generative systems this distinction breaks down: Approaches such as AutoGPT or
 Voyager use generative AI to generate programs (specified in code or plain
 text), which in turn may be interpreted by generative AI systems; prompts for
 chat-based generative AI could equally be considered code or data.
 
-## Installation
-
-## Quick start
-
-## Usage / Examples
-
-## API Reference
-
-## Contributing
-
+## Development and Contributing
 
+Enact is currently in alpha release. The framework is open source and Apache
+licensed. We are actively looking for contributors that are excited about the
+vision.
 
+You can download the source code, report issues and create pull requests at
+https://github.com/agentic-ai/enact.
```

### Comparing `enact-0.4.0.dev0/src/enact.egg-info/SOURCES.txt` & `enact-0.4.0.dev1/src/enact.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
 src/enact/__init__.py
 src/enact/contexts.py
 src/enact/digests.py
-src/enact/guis.py
 src/enact/interfaces.py
 src/enact/invocations.py
 src/enact/pretty_print.py
 src/enact/references.py
 src/enact/resource_registry.py
 src/enact/resource_types.py
 src/enact/resources.py
 src/enact/serialization.py
 src/enact.egg-info/PKG-INFO
 src/enact.egg-info/SOURCES.txt
 src/enact.egg-info/dependency_links.txt
 src/enact.egg-info/requires.txt
 src/enact.egg-info/top_level.txt
+src/enact/gradio/__init__.py
+src/enact/gradio/gradio.py
 tests/test_contexts.py
 tests/test_digest.py
 tests/test_invocations.py
 tests/test_references.py
 tests/test_resource_registry.py
 tests/test_resource_types.py
 tests/test_resources.py
```

### Comparing `enact-0.4.0.dev0/tests/test_contexts.py` & `enact-0.4.0.dev1/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.0.dev0/tests/test_digest.py` & `enact-0.4.0.dev1/tests/test_digest.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.0.dev0/tests/test_invocations.py` & `enact-0.4.0.dev1/tests/test_invocations.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,209 +11,210 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for invocations."""
 
 import dataclasses
+import tempfile
 import time
 from typing import Optional, cast
 import unittest
 from unittest import mock
 
 import enact
 from enact import invocations
 
 
-@dataclasses.dataclass
-class Int(enact.Resource):
-  """An int resource."""
-  v: int
-
-
-@dataclasses.dataclass
-class Str(enact.Resource):
-  """A string resource."""
-  v: str
-
-
-@enact.typed_invokable(Int, Str)
+@enact.typed_invokable(enact.Int, enact.Str)
 @dataclasses.dataclass
 class IntToStr(enact.Invokable):
   """An invokable that converts an int to a string."""
   salt: str = ''
 
-  def call(self, input: Int) -> Str:
-    return Str(v=str(input.v) + self.salt)
+  def call(self, input: enact.Int) -> enact.Str:
+    return enact.Str(str(input) + self.salt)
 
 
-@enact.typed_invokable(Int, Str)
+@enact.typed_invokable(enact.Int, enact.Str)
 class WrongOutputType(enact.Invokable):
 
-  def call(self, input: Int) -> Int:
+  def call(self, input: enact.Int) -> enact.Int:
     return input
 
 
 @dataclasses.dataclass
-@enact.typed_invokable(Int, Int)
+@enact.typed_invokable(enact.Int, enact.Int)
 class AddOne(enact.Invokable):
   fail: bool = False
-  def call(self, input: Int) -> Int:
+  def call(self, input: enact.Int) -> enact.Int:
     if self.fail:
       raise ValueError('fail')
-    return Int(v=input.v + 1)
+    return enact.Int(input + 1)
 
 
 @dataclasses.dataclass
 class Fail(enact.Invokable):
-  def call(self, arg: enact.ResourceBase) -> Int:
+  def call(self, arg: enact.ResourceBase) -> enact.Int:
     raise ValueError('fail')
 
 
-@enact.typed_invokable(Int, Int)
+@enact.typed_invokable(enact.Int, enact.Int)
 @dataclasses.dataclass
 class NestedFunction(enact.Invokable):
   fun: enact.InvokableBase = AddOne()
   iter: int = 10
   fail_on: Optional[int] = None
 
-  def call(self, input: Int) -> Int:
+  def call(self, input: enact.Int) -> enact.Int:
     for i in range(self.iter):
       if i == self.fail_on:
         input = Fail()(input)
       else:
         input = self.fun(input)
     return input
 
 
 class InvocationsTest(unittest.TestCase):
   """Tests invocations."""
 
   def setUp(self):
-    self.backend = enact.InMemoryBackend()
+    self.dir = tempfile.TemporaryDirectory()
+    self.backend = enact.FileBackend(self.dir.name)
     self.store = enact.Store(self.backend)
 
+  def tearDown(self):
+    self.dir.cleanup()
+
   def test_typed_invokable(self):
     """"Test that the decorator works as expected."""
     fun = IntToStr('salt')
-    self.assertEqual(fun.get_input_type(), Int)
-    self.assertEqual(fun.get_output_type(), Str)
-    output = fun.call(Int(v=1))
+    self.assertEqual(fun.get_input_type(), enact.Int)
+    self.assertEqual(fun.get_output_type(), enact.Str)
+    output = fun.call(enact.Int(1))
     # Input and output types should not show up as fields.
     self.assertEqual(list(fun.field_names()), ['salt'])
     # The following line should typecheck correctly.
-    self.assertEqual(output.v, '1salt')
+    self.assertEqual(output, '1salt')
 
   def test_typecheck_input(self):
     fun = IntToStr('salt')
     with self.assertRaises(TypeError):
-      fun(Str(v='1'))
+      fun(enact.Str('1'))
 
   def test_typecheck_output(self):
     fun = WrongOutputType()
     with self.assertRaises(TypeError):
-      fun(Str(v='1'))
+      fun(enact.Str('1'))
 
   def test_auto_input_args(self):
     self.assertEqual(
-      IntToStr()(1).v, '1')
+      IntToStr()(1), '1')
 
   def test_auto_input_kwargs(self):
     self.assertEqual(
-      IntToStr()(v=1).v, '1')
+      IntToStr()(1), '1')
 
   def test_invoke_simple(self):
     with self.store:
       fun = IntToStr('salt')
       invocation = fun.invoke(
-        enact.commit(Int(v=1)))
+        enact.commit(enact.Int(1)))
       want: enact.Invocation = enact.Invocation(
         request=enact.commit(
           enact.Request(enact.commit(fun),
-                        enact.commit(Int(v=1)))),
+                        enact.commit(enact.Int(1)))),
         response=enact.commit(
           enact.Response(
             invokable=enact.commit(fun),
-            output=enact.commit(Str(v='1salt')),
+            output=enact.commit(enact.Str('1salt')),
             raised=None,
             raised_here=False,
-            children=[])),
-        timestamp_ns=invocation.timestamp_ns)
+            children=[])))
     self.assertEqual(
       invocation,
       want)
 
   def test_call_nested(self):
     """Test calling a nested function."""
-    self.assertEqual(NestedFunction()(1).v, 11)
+    self.assertEqual(NestedFunction()(1), 11)
 
   def test_invoke_nested(self):
     """Test invoking a nested function."""
     with self.store:
       invocation = NestedFunction().invoke(
-        enact.commit(Int(v=1)))
+        enact.commit(enact.Int(1)))
       output = invocation.get_output()
-      self.assertEqual(output.v, 11)
+      self.assertEqual(output, 11)
       self.assertEqual(len(list(invocation.get_children())), 10)
       for i, child in enumerate(invocation.get_children()):
-        self.assertEqual(child.request.get().input.get().v, i + 1)
+        self.assertEqual(child.request().input(), i + 1)
         output = child.get_output()
-        self.assertEqual(output.v, i + 2)
+        self.assertEqual(output, i + 2)
+
+  def test_invoke_output_error(self):
+    """Test that error is raised if a non-resource object is returned."""
+    class BadInvokable(enact.Invokable):
+      def call(self, input: enact.Int) -> int:
+        return 1
+    with self.store:
+      with self.assertRaises(TypeError):
+        BadInvokable().invoke(enact.commit(enact.Int(1)))
 
   def test_invoke_fail(self):
     with self.store:
       invocation = NestedFunction(fail_on=3).invoke(
-        enact.commit(Int(v=1)))
+        enact.commit(enact.Int(1)))
       self.assertFalse(invocation.successful())
       exception = invocation.get_raised()
       self.assertIsInstance(
         exception,
         enact.ExceptionResource)
       assert invocation.response().children
       self.assertEqual(len(invocation.response().children), 4)
       for i, child in enumerate(invocation.get_children()):
         if i < 3:
-          self.assertEqual(child.request().input().v, i + 1)
+          self.assertEqual(child.request().input(), i + 1)
           output = child.get_output()
-          self.assertEqual(output.v, i + 2)
+          self.assertEqual(output, i + 2)
         else:
-          self.assertEqual(child.request().input().v, 4)
+          self.assertEqual(child.request().input(), 4)
           self.assertFalse(child.successful())
           exception = child.get_raised()
           self.assertIsInstance(
             exception,
             enact.ExceptionResource)
 
   def test_no_parent_on_invoke(self):
     """Tests that invocations are tracked in a fresh context."""
     with mock.patch.object(time, 'time_ns', return_value=0):
       with self.store as store:
         fun = IntToStr()
-        with invocations.Builder(fun, store.commit(Int(v=1))) as builder:
+        with invocations.Builder(fun, store.commit(enact.Int(1))) as builder:
           # Enter an unrelated context.
           nested = NestedFunction()
-          inner_invocation = nested.invoke(store.commit(Int(1)))
+          inner_invocation = nested.invoke(store.commit(enact.Int(1)))
           # The invocation should not be tracked in the builder.
           self.assertEqual(builder.children, [])
         # Redo the invocation outside the builder.
-        outer_invocation = nested.invoke(store.commit(Int(1)))
+        outer_invocation = nested.invoke(store.commit(enact.Int(1)))
         # Ensure that executing in the misleading context made no difference.
         self.assertEqual(outer_invocation, inner_invocation)
 
   def test_meta_invoke(self):
     """Tests that meta-invocations are tracked correctly."""
     @dataclasses.dataclass
     class MetaInvoke(enact.Invokable):
       invokable: enact.InvokableBase
       def call(self, input: enact.ResourceBase):
         return self.invokable.invoke(enact.commit(input))
 
     with self.store as store:
       fun = NestedFunction()
-      meta_invocation = MetaInvoke(fun).invoke(store.commit(Int(v=1)))
+      meta_invocation = MetaInvoke(fun).invoke(store.commit(enact.Int(1)))
       self.assertEqual(
         len(list(meta_invocation.get_children())), 0)
       invocation = meta_invocation.get_output()
       assert isinstance(invocation, enact.Invocation)
       self.assertEqual(
         len(list(invocation.get_children())), 10)
 
@@ -255,28 +256,55 @@
       def call(self, input: enact.ResourceBase):
         raise ValueError('foo')
 
     @dataclasses.dataclass
     class SubCall(enact.Invokable):
       invokable: enact.Ref[enact.InvokableBase]
       def call(self, input: enact.ResourceBase):
-        self.invokable.get()(input)
+        self.invokable.checkout()(input)
 
     with self.store as store:
       error_fun = PythonErrorOnInvoke()
       subcall_1 = SubCall(store.commit(error_fun))
       subcall_2 = SubCall(store.commit(subcall_1))
 
       invocation = subcall_2.invoke(store.commit(enact.Int(5)))
       self.assertFalse(invocation.get_raised_here())
       (subinvocation,) = invocation.get_children()
       self.assertFalse(subinvocation.get_raised_here())
       (subsubinvocation,) = subinvocation.get_children()
       self.assertTrue(subsubinvocation.get_raised_here())
 
+  def test_reraise_in_replay(self):
+    """Tests that exceptions are replayed."""
+    native_errors_raised = 0
+    class PythonErrorOnInvoke(enact.Invokable):
+      def call(self, input: enact.ResourceBase):
+        nonlocal native_errors_raised
+        native_errors_raised += 1
+        raise ValueError('foo')
+
+    @dataclasses.dataclass
+    class SubCall(enact.Invokable):
+      invokable: enact.Ref[enact.InvokableBase]
+      def call(self, input: enact.ResourceBase):
+        self.invokable.checkout()(input)
+
+    with self.store as store:
+      error_fun = PythonErrorOnInvoke()
+      subcall_1 = SubCall(store.commit(error_fun))
+      subcall_2 = SubCall(store.commit(subcall_1))
+      invocation = subcall_2.invoke(store.commit(enact.Int(5)))
+      self.assertEqual(native_errors_raised, 1)
+      with self.assertRaises(enact.WrappedException):
+        with invocations.ReplayContext(subinvocations=[invocation]):
+          subcall_2(enact.Int(5))
+      self.assertEqual(native_errors_raised, 1)
+
+
   def test_input_changed_error(self):
     @dataclasses.dataclass
     class Changeable(enact.Resource):
       x: int = 0
 
     class ChangesInput(enact.Invokable):
       def call(self, input: Changeable):
@@ -288,165 +316,236 @@
         ChangesInput().invoke(store.commit(Changeable()))
 
   def test_replay_call(self):
     """Test replaying a call."""
     fun = NestedFunction(fail_on=3)
     with self.store:
       invocation = fun.invoke(
-        enact.commit(Int(v=0)))
+        enact.commit(enact.Int(0)))
       with enact.ReplayContext(
           subinvocations=[invocation],
-          exception_override=lambda x: Int(v=100)):
-        result = fun(Int(v=0))
-      self.assertEqual(result.v, 106)
+          exception_override=lambda x: enact.Int(100)):
+        result = fun(enact.Int(0))
+      self.assertEqual(result, 106)
+
+  def test_rewind_call(self):
+    """Test rewinding a call."""
+    leaf_calls = 0
+
+    @enact.typed_invokable(enact.NoneResource, enact.Int)
+    class Leaf(enact.Invokable):
+      def call(self):
+        nonlocal leaf_calls
+        leaf_calls += 1
+        return enact.Int(1)
+
+    @enact.typed_invokable(enact.NoneResource, enact.Int)
+    class Nested(enact.Invokable):
+      def call(self):
+        leaf = Leaf()
+        return enact.Int(leaf() + leaf() + leaf())
+
+    fun = Nested()
+    with self.store:
+      invocation = fun.invoke()
+      self.assertEqual(leaf_calls, 3)
+      invocation.replay()
+      self.assertEqual(leaf_calls, 3)
+      invocation = invocation.rewind(2)
+      invocation.replay()
+      self.assertEqual(leaf_calls, 5)
 
   def test_replay_modifies_invokable(self):
+    @enact.register
     @dataclasses.dataclass
     class Counter(enact.Invokable):
       call_count: int = 0
       def call(self, input: enact.ResourceBase):
         self.call_count += 1
         return input
 
     with self.store:
       counter = Counter()
       fun = NestedFunction(counter, iter=10)
       invocation = fun.invoke(
-        enact.commit(Int(v=0)))
+        enact.commit(enact.Int(0)))
       self.assertEqual(counter.call_count, 10)
 
       # Modify output to ensure we got a replay and
       # not a reexecution.
       with invocation.response.modify() as response:
-        response.output = enact.commit(Int(v=100))
+        response.output = enact.commit(enact.Int(100))
 
       fun.fun = Counter()
       result = invocation.replay()
-      self.assertEqual(result.get_output().v, 100)
+      self.assertEqual(result.get_output(), 100)
       self.assertEqual(counter.call_count, 10)
 
   def test_replay_partial(self):
     """Test replaying a partial invocation."""
     fun = NestedFunction(fail_on=3)
     with self.store:
       invocation = fun.invoke(
-        enact.commit(Int(v=0)))
+        enact.commit(enact.Int(0)))
       with invocation.response.modify() as response:
         del response.children[4:]
         with response.children[-1].modify() as child:
           with child.response.modify() as child_response:
             assert child_response.raised
             child_response.raised = None
-            child_response.output = enact.commit(Int(v=100))
+            child_response.output = enact.commit(enact.Int(100))
       with enact.ReplayContext(
           subinvocations=[invocation]):
-        result = fun(Int(v=0))
-      self.assertEqual(result.v, 106)
+        result = fun(enact.Int(0))
+      self.assertEqual(result, 106)
 
   def test_replay_call_on_mismatch_nonstrict(self):
     """Test non-strict replays are ignored if arguments don't match."""
     fun = NestedFunction(fail_on=3)
     with self.store:
       invocation = fun.invoke(
-        enact.commit(Int(v=0)))
+        enact.commit(enact.Int(0)))
       with enact.ReplayContext(
           subinvocations=[invocation],
-          exception_override=lambda x: Int(v=100), strict=False):
+          exception_override=lambda x: enact.Int(100), strict=False):
         with self.assertRaises(ValueError):
           # Exception override is not active since we're ignoring the
           # replay.
-          fun(Int(v=1))
+          fun(enact.Int(1))
 
   def test_replay_call_on_mismatch_strict(self):
     """Test strict replays raise."""
     fun = NestedFunction(fail_on=3)
     with self.store:
       invocation = fun.invoke(
-        enact.commit(Int(v=0)))
+        enact.commit(enact.Int(0)))
       with enact.ReplayContext(
           subinvocations=[invocation],
-          exception_override=lambda x: Int(v=100), strict=True):
+          exception_override=lambda x: enact.Int(100), strict=True):
         with self.assertRaises(enact.ReplayError):
-          fun(Int(v=1))
+          fun(enact.Int(1))
 
   def test_invoke_with_replay(self):
     """Test replays are ignored if arguments don't match."""
     fun = NestedFunction(fail_on=3)
     with self.store:
       invocation = fun.invoke(
-        enact.commit(Int(v=0)))
+        enact.commit(enact.Int(0)))
       invocation = fun.invoke(
-        enact.commit(Int(v=0)),
+        enact.commit(enact.Int(0)),
         replay_from=invocation,
-        exception_override=lambda x: Int(v=100))
-      self.assertEqual(invocation.get_output().v, 106)
+        exception_override=lambda x: enact.Int(100))
+      self.assertEqual(invocation.get_output(), 106)
 
   def test_request_input(self):
-    class TextInput(enact.Invokable):
-      def call(self, resource: enact.ResourceBase):
-        raise enact.request_input(Str)
-
-    fun = NestedFunction(fun=TextInput(), iter=2)
+    """Tests the RequestInput invokable."""
+    fun = NestedFunction(fun=enact.RequestInput(enact.Str), iter=2)
     with self.store:
       inputs = ['foo', 'bar', 'bish']
-      invocation = fun.invoke(enact.commit(Str(v=inputs[0])))
+      invocation = fun.invoke(enact.commit(enact.Str(inputs[0])))
       for cur_input, next_input in zip(inputs[:-1], inputs[1:]):
         raised = invocation.get_raised()
         assert isinstance(raised, enact.InputRequest)
         self.assertEqual(
-          cast(Str, raised.input.get()).v, cur_input)
+          cast(enact.Str, raised.input.checkout()), cur_input)
         invocation = raised.continue_invocation(
-          invocation, Str(v=next_input))
-      self.assertEqual(invocation.get_output().v, 'bish')
+          invocation, enact.Str(next_input))
+      self.assertEqual(invocation.get_output(), 'bish')
       child_outputs = [
-        c.get_output().v for c in invocation.get_children()]
+        c.get_output() for c in invocation.get_children()]
       self.assertEqual(child_outputs, inputs[1:])
 
-  def test_input_requested_outside_invocation(self):
-    class TextInput(enact.Invokable):
-      def call(self, resource: enact.ResourceBase):
-        raise enact.request_input(Str)
-    with self.assertRaises(enact.InputRequestOutsideInvocation):
-      TextInput()(Str(v='foo'))
-
-  def test_request_input_infer_type(self):
-    @enact.typed_invokable(Str, Str)
-    class TextInput(enact.Invokable):
-      def call(self, resource: enact.ResourceBase):
-        raise enact.request_input(Str)
+  def test_request_input_fun(self):
+    """Tests the request_input function."""
+    class MyInvokable(enact.Invokable):
+      def call(self, value: enact.Int):
+        return enact.Int(enact.request_input(enact.Int) + value)
     with self.store:
-      fun = TextInput()
-      invocation = fun.invoke(enact.commit(Str(v='foo')))
+      invocation = MyInvokable().invoke(enact.commit(enact.Int(3)))
       raised = invocation.get_raised()
       assert isinstance(raised, enact.InputRequest)
-      self.assertEqual(raised.requested_type, Str)
+      invocation = raised.continue_invocation(invocation, enact.Int(5))
+      self.assertEqual(invocation.get_output(), 8)
 
-  def test_request_inference_fails(self):
-    class TextInput(enact.Invokable):
-      def call(self, resource: enact.ResourceBase):
-        raise enact.request_input()
-    with self.store:
-      fun = TextInput()
-      with self.assertRaises(enact.RequestedTypeUndetermined):
-        fun.invoke(enact.commit(Str(v='foo')))
+  def test_input_requested_outside_invocation(self):
+    with self.assertRaises(enact.InputRequestOutsideInvocation):
+      enact.RequestInput(enact.Str)(enact.Str('foo'))
 
   def test_request_input_class(self):
     with self.store:
       fun = enact.RequestInput(enact.Str, enact.Str('Context'))
       invocation = fun.invoke(enact.commit(enact.Str('foo')))
       raised = invocation.get_raised()
       assert isinstance(raised, enact.InputRequest)
       assert raised.context == 'Context'
       self.assertEqual(raised.requested_type, enact.Str)
 
   def test_empty_call_args(self):
     """Tests that empty call args are ok for NoneResource inputs."""
-    @enact.typed_invokable(enact.NoneResource, Str)
+    @enact.typed_invokable(enact.NoneResource, enact.Str)
     class TextInput(enact.Invokable):
       def call(self):
         return enact.Str('Foo')
 
     with self.store:
       fun = TextInput()
       invocation = fun.invoke()
       self.assertEqual(invocation.get_output(), 'Foo')
 
+  def test_invokable_generator_send_without_next(self):
+    """Tests that send without next fails on invokable generator."""
+    with self.store:
+      inv_gen = enact.InvocationGenerator(
+        IntToStr(), enact.commit(enact.Int(3)))
+      with self.assertRaisesRegex(TypeError, '.*non-None.*'):
+        inv_gen.send(enact.Int(3))
+
+  def test_invokable_generator_send_none_without_next(self):
+    """Tests that send None without next works."""
+    with self.store:
+      inv_gen = enact.InvocationGenerator(
+        IntToStr(), enact.commit(enact.Int(3)))
+      with self.assertRaises(StopIteration):
+        inv_gen.send(None)
+
+  def test_invokable_generator_send_flow(self):
+    """Test an invokable generator in a send-based flow."""
+    @enact.typed_invokable(enact.NoneResource, enact.Int)
+    class SumUserRequests(enact.Invokable):
+      def call(self):
+        return enact.Int(
+          enact.request_input(enact.Int) +
+          enact.request_input(enact.Int) +
+          enact.request_input(enact.Int))
+
+    with self.store:
+      inv_gen = enact.InvocationGenerator(
+        SumUserRequests(), enact.commit(enact.NoneResource()))
+      input_request = next(inv_gen)
+      for i in range(5):
+        assert isinstance(input_request, enact.InputRequest)
+        self.assertFalse(inv_gen.complete)
+        try:
+          input_request = inv_gen.send(enact.Int(i))
+        except StopIteration:
+          break
+      self.assertEqual(
+        inv_gen.invocation.get_output(), 0 + 1 + 2)
+
+  def test_invokable_generator_set_input_flow(self):
+    """Test an invokable generator in a send-based flow."""
+    @enact.typed_invokable(enact.NoneResource, enact.Int)
+    class SumUserRequests(enact.Invokable):
+      def call(self):
+        return enact.Int(
+          enact.request_input(enact.Int) +
+          enact.request_input(enact.Int) +
+          enact.request_input(enact.Int))
+
+    with self.store:
+      inv_gen = enact.InvocationGenerator(
+        SumUserRequests(), enact.commit(enact.NoneResource()))
+      for i, _ in enumerate(inv_gen):
+        self.assertFalse(inv_gen.complete)
+        inv_gen.set_input(enact.Int(i))
+      self.assertEqual(
+        inv_gen.invocation.get_output(), 0 + 1 + 2)
```

### Comparing `enact-0.4.0.dev0/tests/test_references.py` & `enact-0.4.0.dev1/tests/test_references.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,54 +97,55 @@
 
   def test_commit_has_get(self):
     """Create a store and test that commit, has, and get work."""
     store = enact.Store()
     resource = SimpleResource(x=1, y=2.0)
     ref = store.commit(resource)
     self.assertTrue(store.has(ref))
-    self.assertEqual(store.get(ref), resource)
-    self.assertNotEqual(id(store.get(ref)), id(resource))
+    self.assertEqual(store.checkout(ref), resource)
+    self.assertNotEqual(id(store.checkout(ref)), id(resource))
 
   def test_custom_ref(self):
     """Test stores with custom ref types."""
     store = enact.Store(ref_type=JsonPackedRef)
     resource = SimpleResource(x=1, y=2.0)
     ref = store.commit(resource)
     self.assertIsInstance(ref, JsonPackedRef)
     self.assertTrue(store.has(ref))
-    self.assertEqual(store.get(ref), resource)
-    self.assertNotEqual(id(store.get(ref)), id(resource))
+    self.assertEqual(store.checkout(ref), resource)
+    self.assertNotEqual(id(store.checkout(ref)), id(resource))
 
   def test_caching(self):
     """Test that caching works correctly."""
     store = enact.Store()
     resource = SimpleResource(x=1, y=2.0)
     ref = store.commit(resource)
 
     # get() works because cached reference is correct.
-    ref.get().x = 10
+    ref.checkout().x = 10
 
     # get() fails because cached reference is incorrect.
     with self.assertRaises(contexts.NoActiveContext):
-      ref.get()
+      ref.checkout()
 
     with store:
       # Refetches the correct resource from the store.
-      self.assertEqual(ref.get().x, 1)
+      self.assertEqual(ref.checkout().x, 1)
 
   def test_modify(self):
     """Tests the modify context."""
     store = enact.Store()
     resource = SimpleResource(x=1, y=2.0)
     ref = store.commit(resource)
     old_digest = ref.digest
 
-    with ref.modify() as resource:
-      resource.x = 10
-    self.assertEqual(ref.get().x, 10)
+    with store:
+      with ref.modify() as resource:
+        resource.x = 10
+      self.assertEqual(ref.checkout().x, 10)
     self.assertNotEqual(ref.digest, old_digest)
 
   def test_pack_none(self):
     """Tests packing the none resource."""
     store = enact.Store()
     resource = interfaces.NoneResource()
     ref = store.commit(resource)
@@ -154,8 +155,8 @@
   def test_file_backend(self):
     """Tests the file backend."""
     with tempfile.TemporaryDirectory() as tmpdir:
       store = enact.Store(backend=enact.FileBackend(tmpdir))
       resource = SimpleResource(x=1, y=2.0)
       ref = store.commit(resource)
       self.assertTrue(store.has(ref))
-      self.assertEqual(store.get(ref), resource)
+      self.assertEqual(store.checkout(ref), resource)
```

### Comparing `enact-0.4.0.dev0/tests/test_resource_registry.py` & `enact-0.4.0.dev1/tests/test_resource_registry.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.0.dev0/tests/test_resource_types.py` & `enact-0.4.0.dev1/tests/test_resource_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,12 +41,12 @@
 
   def test_ref_deref(self):
     """Test storing and dereferencing a resource from a store."""
     for resource_type, value in self.TYPES:
       with self.subTest(resource_type=resource_type):
         resource = cast(enact.ResourceBase, resource_type(value))
         ref = self.store.commit(resource)
-        ref2 = self.store.commit(ref.get())
+        ref2 = self.store.commit(ref.checkout())
         self.assertEqual(ref, ref2)
 
-        for v1, v2 in zip(resource.field_values(), ref2.get().field_values()):
+        for v1, v2 in zip(resource.field_values(), ref2.checkout().field_values()):
           self.assertEqual(v1, v2)
```

### Comparing `enact-0.4.0.dev0/tests/test_resources.py` & `enact-0.4.0.dev1/tests/test_resources.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -150,8 +150,8 @@
     """Tests that set-from works as expected."""
     x = SimpleResource(SimpleResource(1, 2, 3), [4, None],
                        {'a': 0.0, 'b': [True, False]})
     y = SimpleResource(None, None, None)
     y.set_from(x)
     self.assertEqual(y, x)
     x.a.a = 5
-    self.assertNotEqual(y, x)
+    self.assertNotEqual(y, x)
```

### Comparing `enact-0.4.0.dev0/tests/test_serialize.py` & `enact-0.4.0.dev1/tests/test_serialize.py`

 * *Files identical despite different names*

