# Comparing `tmp/chai-guanaco-1.0.8.tar.gz` & `tmp/chai-guanaco-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chai-guanaco-1.0.8.tar", last modified: Tue Aug  1 22:48:43 2023, max compression
+gzip compressed data, was "dist/chai-guanaco-1.1.0.tar", last modified: Fri Aug  4 21:40:10 2023, max compression
```

## Comparing `chai-guanaco-1.0.8.tar` & `chai-guanaco-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/
--rw-rw-r--   0 tom       (1002) tom       (1002)       47 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/MANIFEST.in
--rw-rw-r--   0 tom       (1002) tom       (1002)    11187 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     9477 2023-08-01 17:28:11.000000 chai-guanaco-1.0.8/README.md
--rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/requirements.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/setup.cfg
--rw-rw-r--   0 tom       (1002) tom       (1002)      988 2023-08-01 22:48:25.000000 chai-guanaco-1.0.8/setup.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco/
--rw-rw-r--   0 tom       (1002) tom       (1002)      270 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/__init__.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     4841 2023-07-23 22:36:42.000000 chai-guanaco-1.0.8/src/chai_guanaco/chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3259 2023-07-23 20:07:04.000000 chai-guanaco-1.0.8/src/chai_guanaco/feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/formatters.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/login_cli.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     6036 2023-08-01 17:28:11.000000 chai-guanaco-1.0.8/src/chai_guanaco/metrics.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/
--rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/blade.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/captain_wyatt.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/filbert.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/leo.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/levi.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/mr_wilson.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/nerd_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/scaramouche.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/story_teller.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/vampire_queen.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/wednesday_addams.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     5474 2023-08-01 17:28:11.000000 chai-guanaco-1.0.8/src/chai_guanaco/submit.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1945 2023-07-23 20:07:04.000000 chai-guanaco-1.0.8/src/chai_guanaco/utils.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco.egg-info/
--rw-rw-r--   0 tom       (1002) tom       (1002)    11187 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     1430 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco.egg-info/not-zip-safe
--rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco.egg-info/requires.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/src/chai_guanaco.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/tests/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-01 22:48:43.000000 chai-guanaco-1.0.8/tests/resources/
--rw-rw-r--   0 tom       (1002) tom       (1002)  2224538 2023-08-01 17:28:11.000000 chai-guanaco-1.0.8/tests/resources/test_get_leaderboard.yaml
--rw-rw-r--   0 tom       (1002) tom       (1002)  9300316 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/tests/resources/test_get_submission_metrics.yaml
--rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/tests/test_chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-07-23 20:07:04.000000 chai-guanaco-1.0.8/tests/test_feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     2062 2023-07-23 16:39:07.000000 chai-guanaco-1.0.8/tests/test_guanaco_python_utils.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/tests/test_login.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     6282 2023-08-01 17:28:11.000000 chai-guanaco-1.0.8/tests/test_metrics.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     5607 2023-07-23 16:39:02.000000 chai-guanaco-1.0.8/tests/test_submit.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/
+-rw-rw-r--   0 tom       (1002) tom       (1002)       47 2023-08-04 21:39:07.000000 chai-guanaco-1.1.0/MANIFEST.in
+-rw-rw-r--   0 tom       (1002) tom       (1002)    11463 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     9713 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/README.md
+-rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/requirements.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/setup.cfg
+-rw-rw-r--   0 tom       (1002) tom       (1002)      978 2023-08-04 21:40:05.000000 chai-guanaco-1.1.0/setup.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/src/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/src/chai_guanaco/
+-rw-rw-r--   0 tom       (1002) tom       (1002)      270 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/__init__.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     4841 2023-07-23 22:36:42.000000 chai-guanaco-1.1.0/src/chai_guanaco/chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3259 2023-07-23 20:07:04.000000 chai-guanaco-1.1.0/src/chai_guanaco/feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/formatters.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/login_cli.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     7397 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/src/chai_guanaco/metrics.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/blade.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/captain_wyatt.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/filbert.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/leo.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/levi.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/mr_wilson.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/nerd_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/scaramouche.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/story_teller.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/vampire_queen.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-23 16:39:02.000000 chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/wednesday_addams.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     5474 2023-08-04 14:52:41.000000 chai-guanaco-1.1.0/src/chai_guanaco/submit.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1945 2023-07-23 20:07:04.000000 chai-guanaco-1.1.0/src/chai_guanaco/utils.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/src/chai_guanaco.egg-info/
+-rw-rw-r--   0 tom       (1002) tom       (1002)    11463 2023-08-04 21:40:09.000000 chai-guanaco-1.1.0/src/chai_guanaco.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1705 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/src/chai_guanaco.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-08-04 21:40:09.000000 chai-guanaco-1.1.0/src/chai_guanaco.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-08-04 21:40:09.000000 chai-guanaco-1.1.0/src/chai_guanaco.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-08-04 21:40:09.000000 chai-guanaco-1.1.0/src/chai_guanaco.egg-info/not-zip-safe
+-rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-08-04 21:40:09.000000 chai-guanaco-1.1.0/src/chai_guanaco.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-08-04 21:40:09.000000 chai-guanaco-1.1.0/src/chai_guanaco.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/src/chai_guanaco_private/
+-rw-rw-r--   0 tom       (1002) tom       (1002)        0 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/src/chai_guanaco_private/__init__.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)      603 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/src/chai_guanaco_private/submit_blend.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/tests/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/resources/
+-rw-rw-r--   0 tom       (1002) tom       (1002)  2224538 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/resources/test_get_leaderboard.yaml
+-rw-rw-r--   0 tom       (1002) tom       (1002)  9300316 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/resources/test_get_submission_metrics.yaml
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/test_chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/test_feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2062 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/test_guanaco_python_utils.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/test_login.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6863 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/test_metrics.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     5607 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco/test_submit.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 21:40:10.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco_private/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1875 2023-08-04 19:49:20.000000 chai-guanaco-1.1.0/tests/test_chai_guanaco_private/test_submit_blend.py
```

### Comparing `chai-guanaco-1.0.8/PKG-INFO` & `chai-guanaco-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.8
+Version: 1.1.0
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -64,25 +64,25 @@
         chai-guanaco login
         ```
         
         And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
         
         **Model Submission**
         
-        Upload any GPT-J 6B based language model *with a tokenizer* to huggingface, i.e. [EleutherAI/gpt-j-6b](https://huggingface.co/EleutherAI/gpt-j-6b). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "EleutherAI/gpt-j-6b")
+        Upload any Llama based language model *with a tokenizer* to huggingface, i.e. [NousResearch/Llama-2-7b-chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "NousResearch/Llama-2-7b-chat-hf")
         
         To submit model simply run:
         
         ```python
         import chai_guanaco as chai
         
-        model_url = "EleutherAI/gpt-j-6b" # Your model URL
+        model_url = "NousResearch/Llama-2-7b-chat-hf" # Your model URL
         
         generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0.2, "top_k": 40, "stopping_words": ['\n']}
-        submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-gptj-6b'}
+        submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-llama'}
         
         submitter = chai.ModelSubmitter()
         submission_id = submitter.submit(submission_parameters)
         ```
         
         This will display an animation while your model is being deployed, a typical
         deployment takes approximately 10 minutes. Note the `model_name` parameter is used for show-casing your model on the leaderboard and it should help you with identifying your model
@@ -129,17 +129,22 @@
         print(df)
         ```
         
         This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
         
         **Getting Live Leaderboard**
         
+        To view the public leaderboard used to determine prizes (which only shows the best model submitted by each developer):
+        ```python
+        df = chai.display_leaderboard(detailed=False)
+        ```
+        
         To see how your model performs against other models, run:
         ```python
-        df = chai.display_leaderboard()
+        df = chai.display_leaderboard(detailed=True)
         ```
         which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
         
         **Re-Submitting Models**
         
         Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
```

### Comparing `chai-guanaco-1.0.8/README.md` & `chai-guanaco-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,25 +56,25 @@
 chai-guanaco login
 ```
 
 And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
 
 **Model Submission**
 
-Upload any GPT-J 6B based language model *with a tokenizer* to huggingface, i.e. [EleutherAI/gpt-j-6b](https://huggingface.co/EleutherAI/gpt-j-6b). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "EleutherAI/gpt-j-6b")
+Upload any Llama based language model *with a tokenizer* to huggingface, i.e. [NousResearch/Llama-2-7b-chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "NousResearch/Llama-2-7b-chat-hf")
 
 To submit model simply run:
 
 ```python
 import chai_guanaco as chai
 
-model_url = "EleutherAI/gpt-j-6b" # Your model URL
+model_url = "NousResearch/Llama-2-7b-chat-hf" # Your model URL
 
 generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0.2, "top_k": 40, "stopping_words": ['\n']}
-submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-gptj-6b'}
+submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-llama'}
 
 submitter = chai.ModelSubmitter()
 submission_id = submitter.submit(submission_parameters)
 ```
 
 This will display an animation while your model is being deployed, a typical
 deployment takes approximately 10 minutes. Note the `model_name` parameter is used for show-casing your model on the leaderboard and it should help you with identifying your model
@@ -121,17 +121,22 @@
 print(df)
 ```
 
 This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
 
 **Getting Live Leaderboard**
 
+To view the public leaderboard used to determine prizes (which only shows the best model submitted by each developer):
+```python
+df = chai.display_leaderboard(detailed=False)
+```
+
 To see how your model performs against other models, run:
 ```python
-df = chai.display_leaderboard()
+df = chai.display_leaderboard(detailed=True)
 ```
 which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
 
 **Re-Submitting Models**
 
 Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
```

### Comparing `chai-guanaco-1.0.8/setup.py` & `chai-guanaco-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 if os.environ.get('CI_COMMIT_TAG', None):
     version = os.environ['CI_COMMIT_TAG']
 else:
-    version = "1.0.8"
+    version = "1.1.0"
 
 setup(
     name='chai-guanaco',
     version=version,
     description='Chai Guanaco',
     author='Chai Research Corp.',
     author_email='hello@chai-research.com',
     license='MIT',
-    packages=find_packages(where='src'),
+    packages=['chai_guanaco'],
     package_dir={"": "src"},
     package_data={"chai_guanaco": ["resources/*"]},
     url='https://www.chai-research.com',
     zip_safe=False,
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=requirements,
```

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/chat.py` & `chai-guanaco-1.1.0/src/chai_guanaco/chat.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/feedback.py` & `chai-guanaco-1.1.0/src/chai_guanaco/feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/formatters.py` & `chai-guanaco-1.1.0/src/chai_guanaco/formatters.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/login_cli.py` & `chai-guanaco-1.1.0/src/chai_guanaco/login_cli.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/metrics.py` & `chai-guanaco-1.1.0/src/chai_guanaco/metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from chai_guanaco.login_cli import auto_authenticate
 from chai_guanaco.submit import get_url
 from chai_guanaco.utils import print_color, cache
 
 
 LEADERBOARD_ENDPOINT = "/leaderboard"
 FEEDBACK_CUTOFF_DAYS = 7
-MINIMUM_FEEDBACK_NUMBER_TO_DISPLAY = 50
+MINIMUM_FEEDBACK_NUMBER_TO_DISPLAY = 120
 LEADERBOARD_DISPLAY_COLS = [
     'developer_uid',
     'model_name',
     'thumbs_up_ratio',
-    'user_response_length',
+    'user_engagement',
+    'retry_score',
     'overall_rank',
 ]
 
 
 @auto_authenticate
 def display_leaderboard(developer_key=None, regenerate=False, detailed=False):
     df = cache(get_leaderboard, regenerate)(developer_key)
@@ -43,18 +44,21 @@
 
 @auto_authenticate
 def get_submission_metrics(submission_id, developer_key):
     feedback = get_feedback(submission_id, developer_key)
     feedback_metrics = FeedbackMetrics(feedback.raw_data)
 
     metrics = {
-        'thumbs_up_ratio': feedback_metrics.thumbs_up_ratio,
         'mcl': feedback_metrics.mcl,
-        'user_response_length': feedback_metrics.user_response_length,
-        'total_feedback_count': feedback_metrics.total_feedback_count
+        'thumbs_up_ratio': feedback_metrics.thumbs_up_ratio,
+        'thumbs_up_ratio_se': feedback_metrics.thumbs_up_ratio_se,
+        'retry_score': feedback_metrics.retry_score,
+        'user_engagement': feedback_metrics.mean_user_engagement,
+        'user_engagement_se': feedback_metrics.user_engagement_se,
+        'total_feedback_count': feedback_metrics.total_feedback_count,
     }
     return metrics
 
 
 def get_all_historical_submissions(developer_key):
     headers = {
         "developer_key": developer_key,
@@ -74,55 +78,87 @@
     def convo_metrics(self):
         return [ConversationMetrics(feedback['messages']) for feedback in self.feedbacks]
 
     @property
     def thumbs_up_ratio(self):
         is_thumbs_up = [feedback['thumbs_up'] for feedback in self.feedbacks]
         thumbs_up = sum(is_thumbs_up)
-        thumbs_up_ratio = 0 if not thumbs_up else thumbs_up / len(is_thumbs_up)
+        thumbs_up_ratio = np.nan if not thumbs_up else thumbs_up / len(is_thumbs_up)
         return thumbs_up_ratio
 
     @property
+    def thumbs_up_ratio_se(self):
+        num = self.thumbs_up_ratio * (1 - self.thumbs_up_ratio)
+        denom = self.total_feedback_count**0.5
+        se = np.nan if self.total_feedback_count < 2 else num / denom
+        return se
+
+    @property
     def total_feedback_count(self):
         return len(self.feedbacks)
 
     @property
     def mcl(self):
         return np.mean([m.mcl for m in self.convo_metrics])
 
     @property
-    def user_response_length(self):
-        return np.median([m.user_response_length for m in self.convo_metrics])
+    def mean_user_engagement(self):
+        # taking geometric mean over user response length
+        log_engagement = [np.log(m.user_engagement+1) for m in self.convo_metrics]
+        geometric_mean = np.exp(np.mean(log_engagement))
+        return geometric_mean
+
+    @property
+    def user_engagement_se(self):
+        log_engagement = [np.log(m.user_engagement+1) for m in self.convo_metrics]
+        log_mean = np.mean(log_engagement)
+        log_se = np.std(log_engagement) / len(log_engagement)**0.5
+        mean = np.exp(log_mean)
+        se = mean * log_se
+        return se
+
+    @property
+    def retry_score(self):
+        total_retries = sum([m.num_retries for m in self.convo_metrics])
+        total_bot_responses = sum([m.num_model_responses for m in self.convo_metrics])
+        return 0 if (total_bot_responses) == 0 else total_retries / total_bot_responses
 
 
 class ConversationMetrics():
     def __init__(self, messages):
         self.messages = messages
 
     @property
     def mcl(self):
         return len([m for m in self.messages if not m['deleted']])
 
     @property
-    def user_response_length(self):
+    def num_retries(self):
+        return len([m for m in self.messages if m['deleted']])
+
+    @property
+    def num_model_responses(self):
+        user_messages = [m for m in self.messages if self._is_from_user(m)]
+        return len(self.messages) - len(user_messages)
+
+    @property
+    def user_engagement(self):
         response_length = [len(m['content']) for m in self.messages if self._is_from_user(m)]
         return np.sum(response_length)
 
     def _is_from_user(self, message):
         return '_bot' not in message['sender']['uid']
 
 
 def _print_formatted_leaderboard(raw_df, detailed):
     df = _get_processed_leaderboard(raw_df)
     if not detailed:
         df = _get_df_with_unique_hf_repo(df)
         df = df[LEADERBOARD_DISPLAY_COLS].copy()
-    _pprint_leaderboard(df, '💎 Grand Prize Contenders:', 'overall_rank', detailed, ascending=True)
-    _pprint_leaderboard(df, '😎 Engagement Prize Contenders:', 'user_response_length', detailed, ascending=False)
-    _pprint_leaderboard(df, '👍 Thumbs Up Prize Contenders:', 'thumbs_up_ratio', detailed, ascending=False)
+    _pprint_leaderboard(df, '💎 Leaderboard:', 'overall_rank', detailed, ascending=True)
     return df
 
 
 def _get_processed_leaderboard(df):
     # maintain backwards compatibility with model_name field
     df['model_name'] = df['model_name'].fillna(df['submission_id'])
     df = _format_leaderboard_date(df)
@@ -145,33 +181,36 @@
 
 def _filter_submissions_with_few_feedback(df):
     filtered_df = df[df.total_feedback_count > MINIMUM_FEEDBACK_NUMBER_TO_DISPLAY]
     return filtered_df
 
 
 def _add_overall_rank(df):
-    response_len, thumbs_up = df['user_response_length'], df['thumbs_up_ratio']
+    response_len = df['user_engagement']
+    thumbs_up = df['thumbs_up_ratio']
+    retry_score = df['retry_score']
     response_len_rank = response_len.rank(ascending=False)
     thumbs_up_rank = thumbs_up.rank(ascending=False)
-    overall_score = (response_len_rank + thumbs_up_rank) / 2
+    retry_rate_rank = retry_score.rank(ascending=True)
+    overall_score = (response_len_rank + thumbs_up_rank + retry_rate_rank) / 3
     df['overall_rank'] = overall_score.rank().astype(int)
     df = df.sort_values('overall_rank').reset_index(drop=True)
     return df
 
 
 def _get_df_with_unique_dev_id(df):
     out = df.drop_duplicates('developer_uid', keep='first').reset_index(drop=True)
     return out
 
 
 def _pprint_leaderboard(df, title, sort_by, detailed=False, ascending=True):
     print_color(f'\n{title}', 'red')
     df = df.sort_values(sort_by, ascending=ascending).reset_index(drop=True)
     df = df if detailed else _get_df_with_unique_dev_id(df)
-    print(df.round(3).head(15))
+    print(df.round(3).head(30))
 
 
 def _filter_feedbacks(feedbacks):
     out = {k: v for k, v in feedbacks.items() if _is_n_days_within_current_date(k)}
     return out
```

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/blade.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/blade.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/captain_wyatt.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/captain_wyatt.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/filbert.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/filbert.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/leo.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/leo.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/levi.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/levi.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/mr_wilson.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/mr_wilson.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/nerd_girl.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/nerd_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/scaramouche.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/scaramouche.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/story_teller.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/story_teller.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/vampire_queen.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/vampire_queen.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/resources/bot_config/wednesday_addams.json` & `chai-guanaco-1.1.0/src/chai_guanaco/resources/bot_config/wednesday_addams.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/submit.py` & `chai-guanaco-1.1.0/src/chai_guanaco/submit.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco/utils.py` & `chai-guanaco-1.1.0/src/chai_guanaco/utils.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco.egg-info/PKG-INFO` & `chai-guanaco-1.1.0/src/chai_guanaco.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.8
+Version: 1.1.0
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -64,25 +64,25 @@
         chai-guanaco login
         ```
         
         And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
         
         **Model Submission**
         
-        Upload any GPT-J 6B based language model *with a tokenizer* to huggingface, i.e. [EleutherAI/gpt-j-6b](https://huggingface.co/EleutherAI/gpt-j-6b). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "EleutherAI/gpt-j-6b")
+        Upload any Llama based language model *with a tokenizer* to huggingface, i.e. [NousResearch/Llama-2-7b-chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "NousResearch/Llama-2-7b-chat-hf")
         
         To submit model simply run:
         
         ```python
         import chai_guanaco as chai
         
-        model_url = "EleutherAI/gpt-j-6b" # Your model URL
+        model_url = "NousResearch/Llama-2-7b-chat-hf" # Your model URL
         
         generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0.2, "top_k": 40, "stopping_words": ['\n']}
-        submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-gptj-6b'}
+        submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-llama'}
         
         submitter = chai.ModelSubmitter()
         submission_id = submitter.submit(submission_parameters)
         ```
         
         This will display an animation while your model is being deployed, a typical
         deployment takes approximately 10 minutes. Note the `model_name` parameter is used for show-casing your model on the leaderboard and it should help you with identifying your model
@@ -129,17 +129,22 @@
         print(df)
         ```
         
         This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
         
         **Getting Live Leaderboard**
         
+        To view the public leaderboard used to determine prizes (which only shows the best model submitted by each developer):
+        ```python
+        df = chai.display_leaderboard(detailed=False)
+        ```
+        
         To see how your model performs against other models, run:
         ```python
-        df = chai.display_leaderboard()
+        df = chai.display_leaderboard(detailed=True)
         ```
         which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
         
         **Re-Submitting Models**
         
         Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
```

### Comparing `chai-guanaco-1.0.8/src/chai_guanaco.egg-info/SOURCES.txt` & `chai-guanaco-1.1.0/src/chai_guanaco.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 src/chai_guanaco/resources/bot_config/levi.json
 src/chai_guanaco/resources/bot_config/mr_wilson.json
 src/chai_guanaco/resources/bot_config/nerd_girl.json
 src/chai_guanaco/resources/bot_config/scaramouche.json
 src/chai_guanaco/resources/bot_config/story_teller.json
 src/chai_guanaco/resources/bot_config/vampire_queen.json
 src/chai_guanaco/resources/bot_config/wednesday_addams.json
-tests/test_chat.py
-tests/test_feedback.py
-tests/test_guanaco_python_utils.py
-tests/test_login.py
-tests/test_metrics.py
-tests/test_submit.py
-tests/resources/test_get_leaderboard.yaml
-tests/resources/test_get_submission_metrics.yaml
+src/chai_guanaco_private/__init__.py
+src/chai_guanaco_private/submit_blend.py
+tests/test_chai_guanaco/test_chat.py
+tests/test_chai_guanaco/test_feedback.py
+tests/test_chai_guanaco/test_guanaco_python_utils.py
+tests/test_chai_guanaco/test_login.py
+tests/test_chai_guanaco/test_metrics.py
+tests/test_chai_guanaco/test_submit.py
+tests/test_chai_guanaco/resources/test_get_leaderboard.yaml
+tests/test_chai_guanaco/resources/test_get_submission_metrics.yaml
+tests/test_chai_guanaco_private/test_submit_blend.py
```

### Comparing `chai-guanaco-1.0.8/tests/resources/test_get_leaderboard.yaml` & `chai-guanaco-1.1.0/tests/test_chai_guanaco/resources/test_get_leaderboard.yaml`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/tests/resources/test_get_submission_metrics.yaml` & `chai-guanaco-1.1.0/tests/test_chai_guanaco/resources/test_get_submission_metrics.yaml`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/tests/test_chat.py` & `chai-guanaco-1.1.0/tests/test_chai_guanaco/test_chat.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/tests/test_feedback.py` & `chai-guanaco-1.1.0/tests/test_chai_guanaco/test_feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/tests/test_guanaco_python_utils.py` & `chai-guanaco-1.1.0/tests/test_chai_guanaco/test_guanaco_python_utils.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/tests/test_login.py` & `chai-guanaco-1.1.0/tests/test_chai_guanaco/test_login.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.8/tests/test_metrics.py` & `chai-guanaco-1.1.0/tests/test_chai_guanaco/test_metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,76 +18,89 @@
 def test_get_leaderboard(data_dir_mock, get_ids_mock, tmpdir):
     data_dir_mock.return_value = str(tmpdir)
     get_ids_mock.return_value = historical_submisions()
     df = chai.get_leaderboard()
     expected_cols = [
         'submission_id',
         'thumbs_up_ratio',
-        'mcl',
-        'user_response_length'
+        'retry_score',
+        'total_feedback_count',
+        'user_engagement'
         ]
     for col in expected_cols:
         assert col in df.columns, f'{col} not found in leaderboard'
     expected_data = [
-            {
-                'submission_id': 'alekseykorshuk-exp-sy_1690222960',
-                'timestamp': '2023-07-24 18:22:40+00:00',
-                'status': 'inactive',
-                'model_repo': 'AlekseyKorshuk/exp-syn-friendly-cp475',
-                'developer_uid': 'aleksey',
-                'model_name': 'None',
-                'thumbs_down': 42,
-                'thumbs_up': 33,
-                'thumbs_up_ratio': 0.45454545454545453,
-                'mcl': 12.0,
-                'user_response_length': 75.0,
-                'total_feedback_count': 33
-                },
-            {
-                'submission_id': 'psiilu-funny-bunny-1-_1689922219',
-                'timestamp': '2023-07-21 06:50:19+00:00',
-                'status': 'inactive',
-                'model_repo': 'psiilu/funny-bunny-1-1-1-1-1',
-                'developer_uid': 'philipp',
-                'model_name': 'None',
-                'thumbs_down': 306,
-                'thumbs_up': 187,
-                'thumbs_up_ratio': 0.41148325358851673,
-                'mcl': 9.191387559808613,
-                'user_response_length': 84.0,
-                'total_feedback_count': 209
-                },
-            {
-                'submission_id': 'tehvenom-dolly-shygma_1690135695',
-                'timestamp': '2023-07-23 18:08:15+00:00',
-                'status': 'inactive',
-                'model_repo': 'TehVenom/Dolly_Shygmalion-6b-Dev_V8P2',
-                'developer_uid': 'tehvenom',
-                'model_name': 'None',
-                'thumbs_down': 76,
-                'thumbs_up': 79,
-                'thumbs_up_ratio': 0.48214285714285715,
-                'mcl': 13.053571428571429,
-                'user_response_length': 98.5,
-                'total_feedback_count': 56
-                }
-            ]
+        {
+            'submission_id': 'alekseykorshuk-exp-sy_1690222960',
+            'timestamp': '2023-07-24 18:22:40+00:00',
+            'status': 'inactive',
+            'model_repo': 'AlekseyKorshuk/exp-syn-friendly-cp475',
+            'developer_uid': 'aleksey',
+            'model_name': 'None',
+            'thumbs_down': 42,
+            'thumbs_up': 33,
+            'mcl': 12.0,
+            'thumbs_up_ratio': 0.45454545454545453,
+            'thumbs_up_ratio_se': 0.043159749410503594,
+            'retry_score': 0.14741035856573706,
+            'user_engagement': 67.34005746050721,
+            'user_engagement_se': 18.57789825723364,
+            'total_feedback_count': 33
+            },
+        {
+            'submission_id': 'psiilu-funny-bunny-1-_1689922219',
+            'timestamp': '2023-07-21 06:50:19+00:00',
+            'status': 'inactive',
+            'model_repo': 'psiilu/funny-bunny-1-1-1-1-1',
+            'developer_uid': 'philipp',
+            'model_name': 'None',
+            'thumbs_down': 306,
+            'thumbs_up': 187,
+            'mcl': 9.191387559808613,
+            'thumbs_up_ratio': 0.41148325358851673,
+            'thumbs_up_ratio_se': 0.016750888484181537,
+            'retry_score': 0.22954380883417813,
+            'user_engagement': 75.09995515460673,
+            'user_engagement_se': 6.7271173705601095,
+            'total_feedback_count': 209
+            },
+        {
+            'submission_id': 'tehvenom-dolly-shygma_1690135695',
+            'timestamp': '2023-07-23 18:08:15+00:00',
+            'status': 'inactive',
+            'model_repo': 'TehVenom/Dolly_Shygmalion-6b-Dev_V8P2',
+            'developer_uid': 'tehvenom',
+            'model_name': 'None',
+            'thumbs_down': 76,
+            'thumbs_up': 79,
+            'mcl': 13.053571428571429,
+            'thumbs_up_ratio': 0.48214285714285715,
+            'thumbs_up_ratio_se': 0.03336504343390119,
+            'retry_score': 0.20647773279352227,
+            'user_engagement': 86.49293170787536,
+            'user_engagement_se': 15.430467887932489,
+            'total_feedback_count': 56
+            }
+    ]
     pd.testing.assert_frame_equal(df, pd.DataFrame(expected_data))
 
 
 @vcr.use_cassette(os.path.join(RESOURCE_DIR, 'test_get_submission_metrics.yaml'))
 @freeze_time('2023-07-14 19:00:00')
 def test_get_submission_metrics():
     results = metrics.get_submission_metrics('wizard-vicuna-13b-bo4')
     expected_metrics = {
-            'thumbs_up_ratio': 0.7464788732394366,
             'mcl': 31.507042253521128,
-            'user_response_length': 354.,
+            'thumbs_up_ratio': 0.7464788732394366,
+            'thumbs_up_ratio_se': 0.022459625112416903,
+            'retry_score': 0.08716323296354993,
+            'user_engagement': 328.08592882430924,
+            'user_engagement_se': 31.498130560129095,
             'total_feedback_count': 71
-        }
+            }
     assert results == expected_metrics
 
 
 def test_conversation_metrics():
     bot_sender_data = {'uid': '_bot_123'}
     user_sender_data = {'uid': 'XLQR6'}
     messages = [
@@ -98,23 +111,24 @@
         {'deleted': False, 'content': 'dont go!', 'sender': bot_sender_data},
         {'deleted': False, 'content': '123456', 'sender': user_sender_data},
         {'deleted': False, 'content': 'bye', 'sender': bot_sender_data},
 
     ]
     convo_metrics = metrics.ConversationMetrics(messages)
     assert convo_metrics.mcl == 5
-    assert convo_metrics.user_response_length == 9
+    assert convo_metrics.user_engagement == 9
 
 
 def test_print_formatted_leaderboard():
     data = {
         'submission_id': ['tom_1689542168', 'tom_1689404889', 'val_1689051887', 'zl_1689542168'],
-        'total_feedback_count': [10, 60, 100, 51],
+        'total_feedback_count': [130, 160, 140, 51],
         'mcl': [1.0, 2.0, 3.0, 4.0],
-        'user_response_length': [500, 600, 700, 800],
+        'user_engagement': [500, 600, 700, 800],
+        'retry_score': [.5, .6, .7, .8],
         'thumbs_up_ratio': [0.1, 0.5, 0.8, 0.2],
         'model_name': ['psutil', 'htop', 'watch', 'gunzip'],
         'developer_uid': ['tom', 'tom', 'val', 'zl'],
         'timestamp': ['2023-07-24 18:22:40+00:00'] * 4,
         'model_repo': ['psutil', 'psutil', 'watch', 'gunzip']
     }
     all_metrics_df = pd.DataFrame(data)
@@ -122,15 +136,16 @@
     df = metrics._print_formatted_leaderboard(all_metrics_df, detailed=True)
 
     assert len(df) == 3
     expected_columns = [
             'submission_id',
             'total_feedback_count',
             'mcl',
-            'user_response_length',
+            'user_engagement',
+            'retry_score',
             'thumbs_up_ratio',
             'model_name',
             'developer_uid',
             'model_repo',
             'date',
             'overall_rank'
         ]
```

### Comparing `chai-guanaco-1.0.8/tests/test_submit.py` & `chai-guanaco-1.1.0/tests/test_chai_guanaco/test_submit.py`

 * *Files identical despite different names*

