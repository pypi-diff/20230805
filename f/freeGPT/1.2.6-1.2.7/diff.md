# Comparing `tmp/freeGPT-1.2.6.tar.gz` & `tmp/freeGPT-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.2.6.tar", last modified: Sat Jul 29 09:16:31 2023, max compression
+gzip compressed data, was "freeGPT-1.2.7.tar", last modified: Sat Aug  5 09:22:21 2023, max compression
```

## Comparing `freeGPT-1.2.6.tar` & `freeGPT-1.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 09:16:31.424970 freeGPT-1.2.6/
--rw-rw-rw-   0        0        0    18092 2023-07-29 09:15:34.000000 freeGPT-1.2.6/LICENSE
--rw-rw-rw-   0        0        0     4387 2023-07-29 09:16:31.424970 freeGPT-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3078 2023-07-29 09:15:34.000000 freeGPT-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 09:16:31.408969 freeGPT-1.2.6/freeGPT/
--rw-rw-rw-   0        0        0      164 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/alpaca_7b.py
--rw-rw-rw-   0        0        0     2697 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/gpt3.py
--rw-rw-rw-   0        0        0     2495 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/gpt4.py
--rw-rw-rw-   0        0        0      738 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/pollinations.py
--rw-rw-rw-   0        0        0     3530 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/prodia.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:16:31.424970 freeGPT-1.2.6/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     4387 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 09:16:31.424970 freeGPT-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1663 2023-07-29 09:15:34.000000 freeGPT-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:22:21.610381 freeGPT-1.2.7/
+-rw-rw-rw-   0        0        0    18092 2023-08-05 09:21:17.000000 freeGPT-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     4575 2023-08-05 09:22:21.610381 freeGPT-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3243 2023-08-05 09:21:17.000000 freeGPT-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 09:22:21.602376 freeGPT-1.2.7/freeGPT/
+-rw-rw-rw-   0        0        0      164 2023-08-05 09:21:17.000000 freeGPT-1.2.7/freeGPT/__init__.py
+-rw-rw-rw-   0        0        0     2000 2023-08-05 09:21:17.000000 freeGPT-1.2.7/freeGPT/alpaca_7b.py
+-rw-rw-rw-   0        0        0     2669 2023-08-05 09:21:17.000000 freeGPT-1.2.7/freeGPT/gpt3.py
+-rw-rw-rw-   0        0        0     2430 2023-08-05 09:21:17.000000 freeGPT-1.2.7/freeGPT/gpt4.py
+-rw-rw-rw-   0        0        0      759 2023-08-05 09:21:17.000000 freeGPT-1.2.7/freeGPT/pollinations.py
+-rw-rw-rw-   0        0        0     3551 2023-08-05 09:21:17.000000 freeGPT-1.2.7/freeGPT/prodia.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:22:21.608380 freeGPT-1.2.7/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     4575 2023-08-05 09:22:21.000000 freeGPT-1.2.7/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-08-05 09:22:21.000000 freeGPT-1.2.7/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 09:22:21.000000 freeGPT-1.2.7/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-05 09:22:21.000000 freeGPT-1.2.7/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 09:22:21.000000 freeGPT-1.2.7/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 09:22:21.611380 freeGPT-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1685 2023-08-05 09:21:17.000000 freeGPT-1.2.7/setup.py
```

### Comparing `freeGPT-1.2.6/LICENSE` & `freeGPT-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.6/PKG-INFO` & `freeGPT-1.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.6
-Summary: freeGPT provides free access to GPT3, GPT4 and more models.
+Version: 1.2.7
+Summary: freeGPT provides free access to text and image generation models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
-Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
+Keywords: natural-language-processing,artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,freegpt,chatgpt,python,llama,llm,nlp,gpt,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,50 +20,51 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-##### The freeGPT bot has been verified, invite it [here](https://dsc.gg/freegpt)!
-
 [![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
 [![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
 [![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
 
 # freeGPT
 
-freeGPT provides free access to GPT3, GPT4 and more models.
+freeGPT provides free access to GPT3, GPT4, and more models.
 
 ## Get started:
 
 ```
 python -m pip install -U freeGPT
 ```
 
 **Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
-| Models       | Websites                                                |
-| ------------ | ------------------------------------------------------- |
-| gpt3         | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
-| gpt4         | [<you.com>](https://you.com/)                           |
-| alpaca_7b    | [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
-| prodia       | [<prodia.com>](https://prodia.com/)                     |
-| pollinations | [<pollinations.ai>](https://pollinations.ai/)           |
+### Text Generation:
+| Model     | Website                                               |
+| --------- | ----------------------------------------------------- |
+| gpt3      | [ava-ai-ef611.web.app](https://ava-ai-ef611.web.app/) |
+| gpt4      | [you.com](https://you.com/)                           |
+| alpaca_7b | [chatllama.baseten.co](https://chatllama.baseten.co/) |
+
+### Image Generation:
+| Model        | Website                                     |
+| ------------ | ------------------------------------------- |
+| prodia       | [prodia.com](https://prodia.com/)           |
+| pollinations | [pollinations.ai](https://pollinations.ai/) |
 
 
 ## Support this repository:
-
-- Star this repository :D
-- Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
-- Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
+- ⭐ **Star the project:** Star this and the [freeGPT-discord-bot repository](https://github.com/Ruu3f/freeGPT-discord-bot). It means a lot to me! 💕
+- 🎉 **Join my Discord Server:** Try the bot and chat with others. [Join here](https://discord.gg/XH6pUGkwRr):
 
 [![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## TODO List:
 
 - [x] Make the library well-documented.
 - [x] Make the overall library easier to use.
@@ -88,15 +89,15 @@
 from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
-            resp = await getattr(freeGPT, "MODEL NAME").Completion.create(prompt)
+            resp = await getattr(freeGPT, "MODEL NAME").Completion().create(prompt)
             print(f"🤖: {resp}")
         except Exception as e:
             print(f"🤖: {e}")
 
 
 run(main())
 ```
@@ -109,15 +110,15 @@
 from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
-            resp = await getattr(freeGPT, "MODEL NAME").Generation.create(prompt)
+            resp = await getattr(freeGPT, "MODEL NAME").Generation().create(prompt)
             Image.open(BytesIO(resp)).show()
             print(f"🤖: Image shown.")
         except Exception as e:
             print(f"🤖: {e}")
 
 
 run(main())
```

### Comparing `freeGPT-1.2.6/README.md` & `freeGPT-1.2.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-##### The freeGPT bot has been verified, invite it [here](https://dsc.gg/freegpt)!
-
 [![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
 [![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
 [![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
 
 # freeGPT
 
-freeGPT provides free access to GPT3, GPT4 and more models.
+freeGPT provides free access to GPT3, GPT4, and more models.
 
 ## Get started:
 
 ```
 python -m pip install -U freeGPT
 ```
 
 **Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
-| Models       | Websites                                                |
-| ------------ | ------------------------------------------------------- |
-| gpt3         | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
-| gpt4         | [<you.com>](https://you.com/)                           |
-| alpaca_7b    | [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
-| prodia       | [<prodia.com>](https://prodia.com/)                     |
-| pollinations | [<pollinations.ai>](https://pollinations.ai/)           |
+### Text Generation:
+| Model     | Website                                               |
+| --------- | ----------------------------------------------------- |
+| gpt3      | [ava-ai-ef611.web.app](https://ava-ai-ef611.web.app/) |
+| gpt4      | [you.com](https://you.com/)                           |
+| alpaca_7b | [chatllama.baseten.co](https://chatllama.baseten.co/) |
+
+### Image Generation:
+| Model        | Website                                     |
+| ------------ | ------------------------------------------- |
+| prodia       | [prodia.com](https://prodia.com/)           |
+| pollinations | [pollinations.ai](https://pollinations.ai/) |
 
 
 ## Support this repository:
-
-- Star this repository :D
-- Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
-- Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
+- ⭐ **Star the project:** Star this and the [freeGPT-discord-bot repository](https://github.com/Ruu3f/freeGPT-discord-bot). It means a lot to me! 💕
+- 🎉 **Join my Discord Server:** Try the bot and chat with others. [Join here](https://discord.gg/XH6pUGkwRr):
 
 [![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## TODO List:
 
 - [x] Make the library well-documented.
 - [x] Make the overall library easier to use.
@@ -62,15 +63,15 @@
 from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
-            resp = await getattr(freeGPT, "MODEL NAME").Completion.create(prompt)
+            resp = await getattr(freeGPT, "MODEL NAME").Completion().create(prompt)
             print(f"🤖: {resp}")
         except Exception as e:
             print(f"🤖: {e}")
 
 
 run(main())
 ```
@@ -83,15 +84,15 @@
 from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
-            resp = await getattr(freeGPT, "MODEL NAME").Generation.create(prompt)
+            resp = await getattr(freeGPT, "MODEL NAME").Generation().create(prompt)
             Image.open(BytesIO(resp)).show()
             print(f"🤖: Image shown.")
         except Exception as e:
             print(f"🤖: {e}")
 
 
 run(main())
```

### Comparing `freeGPT-1.2.6/freeGPT/alpaca_7b.py` & `freeGPT-1.2.7/freeGPT/alpaca_7b.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from requests import post, exceptions
+from requests import post
+from requests.exceptions import RequestException
 
 
 class Completion:
     """
     A class for generating text completions using an API.
 
     Attributes:
         None
 
     Methods:
         create(prompt): Generates a text completion for the given prompt using an API.
     """
 
-    async def create(prompt):
+    async def create(self, prompt):
         """
         Generates a text completion for the given prompt using an API.
 
         Args:
             prompt (str): The prompt for which to generate a text completion.
 
         Returns:
@@ -43,11 +44,11 @@
                     "Sec-Fetch-Mode": "cors",
                     "Sec-Fetch-Site": "cross-site",
                     "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.79 Safari/537.36",
                 },
                 json={"prompt": prompt},
                 timeout=30,
             ).json()
-        except exceptions.RequestException:
+        except RequestException:
             raise Exception("Unable to fetch the response.")
 
         return resp["completion"]
```

### Comparing `freeGPT-1.2.6/freeGPT/gpt3.py` & `freeGPT-1.2.7/freeGPT/gpt3.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 
 class Completion:
     """
     This class provides methods for generating completions based on prompts.
     """
 
-    @classmethod
-    async def create(cls, prompt):
+    async def create(self, prompt):
         """
         Create a new completion based on the given prompt.
 
         Args:
             prompt (str): The prompt to generate a completion for.
 
         Returns:
@@ -59,9 +58,9 @@
                                             "delta" in choice
                                             and "content" in choice["delta"]
                                         ):
                                             resp += choice["delta"]["content"]
                             except JSONDecodeError:
                                 pass
                     return resp
-        except ClientError:
+        except:
             raise Exception("Unable to fetch the response.")
```

### Comparing `freeGPT-1.2.6/freeGPT/gpt4.py` & `freeGPT-1.2.7/freeGPT/gpt4.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from uuid import uuid4
 from re import findall
-from typing import Optional
 from subprocess import check_call
 
 try:
     import tls_client
-except Exception:
+except ModuleNotFoundError:
     check_call(["pip", "install", "tls_client", "--no-cache-dir"])
 
 
 class Completion:
-    async def create(
-        prompt: str,
-        proxy: Optional[str] = None,
-    ) -> str:
+    async def create(self, prompt):
         """
         Create a completion for the given prompt using the you.com API.
 
         Args:
             prompt (str): The prompt for which completion is requested.
             proxy (str, optional): The proxy to be used for the API request. Defaults to None.
 
@@ -39,28 +35,29 @@
             "sec-ch-ua-platform": '"Windows"',
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin",
             "cookie": f"safesearch_guest=Off; uuid_guest={str(uuid4())}",
             "user-agent": "Mozilla/5.0 (Windows NT 5.1; U;  ; rv:1.8.1) Gecko/20061208 Firefox/2.0.0 Opera 9.52",
         }
-        client.proxies = proxy
         params = {
             "q": prompt,
             "page": 1,
             "count": 10,
             "safeSearch": "Off",
             "onShoppingPage": False,
             "mkt": "",
             "responseFilter": "WebPages,Translations,TimeZone,Computation,RelatedSearches",
             "domain": "youchat",
             "queryTraceId": str(uuid4()),
             "chat": [],
         }
-        resp = client.get("https://you.com/api/streamingSearch", params=params)
+        resp = client.get(
+            "https://you.com/api/streamingSearch", params=params, timeout_seconds=30
+        )
         if "youChatToken" not in resp.text:
             raise Exception("Unable to fetch response.")
         return (
             "".join(findall(r"{\"youChatToken\": \"(.*?)\"}", resp.text))
             .replace("\\n", "\n")
             .replace("\\\\", "\\")
             .replace('\\"', '"')
```

### Comparing `freeGPT-1.2.6/freeGPT/pollinations.py` & `freeGPT-1.2.7/freeGPT/pollinations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from random import randint
-from aiohttp import ClientSession
+from aiohttp import ClientSession, ClientError
 
 
 class Generation:
-    async def create(prompt):
+    async def create(self, prompt):
         """
         Create a new image generation based on the given prompt.
 
         Args:
             prompt (str): The prompt for generating the image.
 
         Returns:
             resp: The generated image content
         """
         try:
             async with ClientSession() as session:
                 async with session.get(
                     url=f"https://image.pollinations.ai/prompt/{prompt}{randint(1, 10000)}",
-                    timeout=45,
+                    timeout=30,
                 ) as resp:
                     return await resp.content.read()
-        except Exception:
+        except ClientError:
             raise Exception("Unable to fetch the response.")
```

### Comparing `freeGPT-1.2.6/freeGPT/prodia.py` & `freeGPT-1.2.7/freeGPT/prodia.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from random import randint
-from aiohttp import ClientSession
+from aiohttp import ClientSession, ClientError
 
 
 class Generation:
-    async def create(prompt):
+    async def create(self, prompt):
         """
         Create a new image generation based on the given prompt.
 
         Args:
             prompt (str): The prompt for generating the image.
 
         Returns:
@@ -42,24 +42,24 @@
         }
         try:
             async with ClientSession() as session:
                 async with session.get(
                     "https://api.prodia.com/generate",
                     params=params,
                     headers=headers,
-                    timeout=45,
+                    timeout=30,
                 ) as resp:
                     data = await resp.json()
                     job_id = data["job"]
                     while True:
                         async with session.get(
                             f"https://api.prodia.com/job/{job_id}", headers=headers
                         ) as resp:
                             json = await resp.json()
                             if json["status"] == "succeeded":
                                 async with session.get(
                                     f"https://images.prodia.xyz/{job_id}.png?download=1",
                                     headers=headers,
                                 ) as resp:
                                     return await resp.content.read()
-        except Exception:
+        except ClientError:
             raise Exception("Unable to fetch the response.")
```

### Comparing `freeGPT-1.2.6/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.2.7/freeGPT.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.6
-Summary: freeGPT provides free access to GPT3, GPT4 and more models.
+Version: 1.2.7
+Summary: freeGPT provides free access to text and image generation models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
-Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
+Keywords: natural-language-processing,artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,freegpt,chatgpt,python,llama,llm,nlp,gpt,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,50 +20,51 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-##### The freeGPT bot has been verified, invite it [here](https://dsc.gg/freegpt)!
-
 [![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
 [![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
 [![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
 
 # freeGPT
 
-freeGPT provides free access to GPT3, GPT4 and more models.
+freeGPT provides free access to GPT3, GPT4, and more models.
 
 ## Get started:
 
 ```
 python -m pip install -U freeGPT
 ```
 
 **Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
-| Models       | Websites                                                |
-| ------------ | ------------------------------------------------------- |
-| gpt3         | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
-| gpt4         | [<you.com>](https://you.com/)                           |
-| alpaca_7b    | [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
-| prodia       | [<prodia.com>](https://prodia.com/)                     |
-| pollinations | [<pollinations.ai>](https://pollinations.ai/)           |
+### Text Generation:
+| Model     | Website                                               |
+| --------- | ----------------------------------------------------- |
+| gpt3      | [ava-ai-ef611.web.app](https://ava-ai-ef611.web.app/) |
+| gpt4      | [you.com](https://you.com/)                           |
+| alpaca_7b | [chatllama.baseten.co](https://chatllama.baseten.co/) |
+
+### Image Generation:
+| Model        | Website                                     |
+| ------------ | ------------------------------------------- |
+| prodia       | [prodia.com](https://prodia.com/)           |
+| pollinations | [pollinations.ai](https://pollinations.ai/) |
 
 
 ## Support this repository:
-
-- Star this repository :D
-- Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
-- Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
+- ⭐ **Star the project:** Star this and the [freeGPT-discord-bot repository](https://github.com/Ruu3f/freeGPT-discord-bot). It means a lot to me! 💕
+- 🎉 **Join my Discord Server:** Try the bot and chat with others. [Join here](https://discord.gg/XH6pUGkwRr):
 
 [![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## TODO List:
 
 - [x] Make the library well-documented.
 - [x] Make the overall library easier to use.
@@ -88,15 +89,15 @@
 from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
-            resp = await getattr(freeGPT, "MODEL NAME").Completion.create(prompt)
+            resp = await getattr(freeGPT, "MODEL NAME").Completion().create(prompt)
             print(f"🤖: {resp}")
         except Exception as e:
             print(f"🤖: {e}")
 
 
 run(main())
 ```
@@ -109,15 +110,15 @@
 from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
-            resp = await getattr(freeGPT, "MODEL NAME").Generation.create(prompt)
+            resp = await getattr(freeGPT, "MODEL NAME").Generation().create(prompt)
             Image.open(BytesIO(resp)).show()
             print(f"🤖: Image shown.")
         except Exception as e:
             print(f"🤖: {e}")
 
 
 run(main())
```

### Comparing `freeGPT-1.2.6/setup.py` & `freeGPT-1.2.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.2.6",
-    description="freeGPT provides free access to GPT3, GPT4 and more models.",
+    version="1.2.7",
+    description="freeGPT provides free access to text and image generation models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv2",
     keywords=[
+        "natural-language-processing",
         "artificial-intelligence",
         "machine-learning",
         "deep-learning",
         "gpt4free",
         "gpt4all",
-        "chatbot",
         "freegpt",
         "chatgpt",
         "python",
-        "openai",
         "llama",
-        "free",
+        "llm",
+        "nlp",
         "gpt",
         "ai",
     ],
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

