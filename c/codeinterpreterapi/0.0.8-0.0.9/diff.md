# Comparing `tmp/codeinterpreterapi-0.0.8.tar.gz` & `tmp/codeinterpreterapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeinterpreterapi-0.0.8.tar", max compression
+gzip compressed data, was "codeinterpreterapi-0.0.9.tar", max compression
```

## Comparing `codeinterpreterapi-0.0.8.tar` & `codeinterpreterapi-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.8/LICENSE
--rw-r--r--   0        0        0     4364 2023-07-29 19:51:57.281872 codeinterpreterapi-0.0.8/README.md
--rw-r--r--   0        0        0      104 2023-07-29 19:51:57.279068 codeinterpreterapi-0.0.8/codeinterpreterapi/__init__.py
--rw-r--r--   0        0        0      929 2023-07-29 19:51:57.279769 codeinterpreterapi-0.0.8/codeinterpreterapi/callbacks.py
--rw-r--r--   0        0        0        0 2023-07-29 19:51:57.277704 codeinterpreterapi-0.0.8/codeinterpreterapi/chains/__init__.py
--rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.8/codeinterpreterapi/chains/functions_agent.py
--rw-r--r--   0        0        0     1578 2023-07-29 19:51:57.279319 codeinterpreterapi-0.0.8/codeinterpreterapi/chains/modifications_check.py
--rw-r--r--   0        0        0      977 2023-07-29 19:51:57.279378 codeinterpreterapi-0.0.8/codeinterpreterapi/chains/remove_download_link.py
--rw-r--r--   0        0        0      390 2023-07-17 19:38:21.218647 codeinterpreterapi-0.0.8/codeinterpreterapi/config.py
--rw-r--r--   0        0        0      225 2023-07-29 19:51:57.279480 codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/__init__.py
--rw-r--r--   0        0        0     1379 2023-07-29 19:51:57.279579 codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/modifications_check.py
--rw-r--r--   0        0        0      959 2023-07-17 11:26:26.313924 codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/remove_dl_link.py
--rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/system_message.py
--rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.8/codeinterpreterapi/schema/__init__.py
--rw-r--r--   0        0        0     2385 2023-07-27 12:56:18.814797 codeinterpreterapi-0.0.8/codeinterpreterapi/schema/file.py
--rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.8/codeinterpreterapi/schema/input.py
--rw-r--r--   0        0        0      629 2023-07-29 19:51:57.279665 codeinterpreterapi-0.0.8/codeinterpreterapi/schema/response.py
--rw-r--r--   0        0        0     8266 2023-07-29 19:51:57.279122 codeinterpreterapi-0.0.8/codeinterpreterapi/session.py
--rw-r--r--   0        0        0      681 2023-07-29 19:58:48.997254 codeinterpreterapi-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4556 2023-08-02 14:07:01.207752 codeinterpreterapi-0.0.9/README.md
+-rw-r--r--   0        0        0      105 2023-08-02 14:07:01.204437 codeinterpreterapi-0.0.9/codeinterpreterapi/__init__.py
+-rw-r--r--   0        0        0       50 2023-08-02 14:07:01.205302 codeinterpreterapi-0.0.9/codeinterpreterapi/agents/__init__.py
+-rw-r--r--   0        0        0      101 2023-08-02 14:07:01.204800 codeinterpreterapi-0.0.9/codeinterpreterapi/agents/custom_agent.py
+-rw-r--r--   0        0        0     9989 2023-08-02 14:07:01.204928 codeinterpreterapi-0.0.9/codeinterpreterapi/agents/functions_agent.py
+-rw-r--r--   0        0        0      147 2023-08-02 14:07:01.205032 codeinterpreterapi-0.0.9/codeinterpreterapi/chains/__init__.py
+-rw-r--r--   0        0        0     1016 2023-08-02 14:07:01.205191 codeinterpreterapi-0.0.9/codeinterpreterapi/chains/extract_code.py
+-rw-r--r--   0        0        0     1477 2023-08-02 14:07:01.204585 codeinterpreterapi-0.0.9/codeinterpreterapi/chains/modifications_check.py
+-rw-r--r--   0        0        0      977 2023-08-02 14:07:01.204675 codeinterpreterapi-0.0.9/codeinterpreterapi/chains/rm_dl_link.py
+-rw-r--r--   0        0        0      390 2023-07-17 19:38:21.218647 codeinterpreterapi-0.0.9/codeinterpreterapi/config.py
+-rw-r--r--   0        0        0      191 2023-08-02 14:07:01.205717 codeinterpreterapi-0.0.9/codeinterpreterapi/prompts/__init__.py
+-rw-r--r--   0        0        0     1869 2023-08-02 14:07:01.206067 codeinterpreterapi-0.0.9/codeinterpreterapi/prompts/modifications_check.py
+-rw-r--r--   0        0        0      959 2023-07-17 11:26:26.313924 codeinterpreterapi-0.0.9/codeinterpreterapi/prompts/remove_dl_link.py
+-rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.9/codeinterpreterapi/prompts/system_message.py
+-rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.9/codeinterpreterapi/schema/__init__.py
+-rw-r--r--   0        0        0     2401 2023-08-02 14:07:01.206307 codeinterpreterapi-0.0.9/codeinterpreterapi/schema/file.py
+-rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.9/codeinterpreterapi/schema/input.py
+-rw-r--r--   0        0        0      752 2023-08-02 14:07:01.206398 codeinterpreterapi-0.0.9/codeinterpreterapi/schema/response.py
+-rw-r--r--   0        0        0    10522 2023-08-02 15:05:49.897925 codeinterpreterapi-0.0.9/codeinterpreterapi/session.py
+-rw-r--r--   0        0        0      112 2023-08-02 14:07:01.206534 codeinterpreterapi-0.0.9/codeinterpreterapi/utils/__init__.py
+-rw-r--r--   0        0        0      929 2023-08-02 14:07:01.207126 codeinterpreterapi-0.0.9/codeinterpreterapi/utils/callbacks.py
+-rw-r--r--   0        0        0     2499 2023-08-02 14:07:01.207327 codeinterpreterapi-0.0.9/codeinterpreterapi/utils/parser.py
+-rw-r--r--   0        0        0      764 2023-08-02 14:39:59.592869 codeinterpreterapi-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.9/PKG-INFO
```

### Comparing `codeinterpreterapi-0.0.8/LICENSE` & `codeinterpreterapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.8/README.md` & `codeinterpreterapi-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 - Use CodeBox API for easy scaling in production (coming soon)
 
 ## Installation
 
 Get your OpenAI API Key [here](https://platform.openai.com/account/api-keys) and install the package.
 
 ```bash
-pip install codeinterpreterapi
+pip install "codeinterpreterapi[all]"
 ```
 
+Everything for local experiments are installed with the `all` extra.
+For deployments, you can use `pip install codeinterpreterapi` instead which does not install the additional dependencies.
+
 ## Usage
 
 Make sure to set the `OPENAI_API_KEY` environment variable (or use a `.env` file)
 
 ```python
 from codeinterpreterapi import CodeInterpreterSession
 
@@ -123,15 +126,15 @@
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Contact
 
 You can contact me at [contact@shroominic.com](mailto:contact@shroominic.com).
-But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://gptassistant.app/community) DMs.
+But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://discord.gg/QYzBtq37) DMs.
 
 ## Support this project
 
 If you would like to help this project with a donation, you can [click here](https://ko-fi.com/shroominic).
 Thanks, this helps a lot! ❤️
 
 ## Star History
```

### Comparing `codeinterpreterapi-0.0.8/codeinterpreterapi/callbacks.py` & `codeinterpreterapi-0.0.9/codeinterpreterapi/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.8/codeinterpreterapi/chains/functions_agent.py` & `codeinterpreterapi-0.0.9/codeinterpreterapi/agents/functions_agent.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.8/codeinterpreterapi/chains/remove_download_link.py` & `codeinterpreterapi-0.0.9/codeinterpreterapi/chains/rm_dl_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/remove_dl_link.py` & `codeinterpreterapi-0.0.9/codeinterpreterapi/prompts/remove_dl_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/system_message.py` & `codeinterpreterapi-0.0.9/codeinterpreterapi/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.8/codeinterpreterapi/schema/file.py` & `codeinterpreterapi-0.0.9/codeinterpreterapi/schema/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         # Display the image
         try:
             # Try to get the IPython shell if available.
             shell = get_ipython().__class__.__name__  # type: ignore
 
             # If the shell is ZMQInteractiveShell, it means we're in a Jupyter notebook or similar.
             if shell == 'ZMQInteractiveShell':
-                from IPython.display import display
+                from IPython.display import display  # type: ignore
                 display(img)
             else:
                 # We're not in a Jupyter notebook.
                 img.show()
         except NameError:
             # We're probably not in an IPython environment, use PIL's show.
             img.show()
```

### Comparing `codeinterpreterapi-0.0.8/codeinterpreterapi/schema/response.py` & `codeinterpreterapi-0.0.9/codeinterpreterapi/schema/response.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,12 +13,17 @@
 
 
 class CodeInterpreterResponse(AIMessage):
     files: list[File] = []
     # final_code: str = ""  TODO: implement
     # final_output: str = ""  TODO: implement
 
+    def show(self):
+        print("AI: ", self.content)
+        for file in self.files:
+            file.show_image()
+    
     def __str__(self):
         return self.content
 
     def __repr__(self):
         return f"CodeInterpreterResponse(content={self.content}, files={self.files})"
```

### Comparing `codeinterpreterapi-0.0.8/codeinterpreterapi/session.py` & `codeinterpreterapi-0.0.9/codeinterpreterapi/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,154 @@
-import uuid, base64, re
+import uuid, base64, re, traceback
 from io import BytesIO
+from os import getenv
 from typing import Optional
 from codeboxapi import CodeBox  # type: ignore
 from codeboxapi.schema import CodeBoxOutput  # type: ignore
 from langchain.tools import StructuredTool, BaseTool
-from langchain.chat_models import ChatOpenAI
+from langchain.chat_models import ChatOpenAI, ChatAnthropic
 from langchain.chat_models.base import BaseChatModel
+from langchain.schema.language_model import BaseLanguageModel
 from langchain.prompts.chat import MessagesPlaceholder
-from langchain.agents import AgentExecutor, BaseSingleActionAgent
+from langchain.agents import AgentExecutor, BaseSingleActionAgent, ConversationalChatAgent, ConversationalAgent
 from langchain.memory import ConversationBufferMemory
 
-from codeinterpreterapi.schema import CodeInterpreterResponse, CodeInput, File, UserRequest
 from codeinterpreterapi.config import settings
-from codeinterpreterapi.chains.functions_agent import OpenAIFunctionsAgent
+from codeinterpreterapi.agents import OpenAIFunctionsAgent
 from codeinterpreterapi.prompts import code_interpreter_system_message
-from codeinterpreterapi.callbacks import CodeCallbackHandler
-from codeinterpreterapi.chains.modifications_check import get_file_modifications
-from codeinterpreterapi.chains.remove_download_link import remove_download_link
+from codeinterpreterapi.chains import get_file_modifications, remove_download_link
+from codeinterpreterapi.utils import CodeCallbackHandler, CodeAgentOutputParser, CodeChatAgentOutputParser
+from codeinterpreterapi.schema import CodeInterpreterResponse, CodeInput, File, UserRequest
 
 
 class CodeInterpreterSession:
     def __init__(
-        self,
-        model="gpt-4",
-        openai_api_key=settings.OPENAI_API_KEY,
-        verbose=settings.VERBOSE,
-        tools: list[BaseTool] = [],
+        self, 
+        llm: Optional[BaseLanguageModel] = None, 
+        additional_tools: list[BaseTool] = [], 
+        **kwargs
     ) -> None:
         self.codebox = CodeBox()
-        self.verbose = verbose
-        self.tools: list[BaseTool] = self._tools(tools)
-        self.llm: BaseChatModel = self._llm(model, openai_api_key)
+        self.verbose = kwargs.get("verbose", settings.VERBOSE)
+        self.tools: list[BaseTool] = self._tools(additional_tools)
+        self.llm: BaseLanguageModel = llm or self._choose_llm(**kwargs)
         self.agent_executor: AgentExecutor = self._agent_executor()
         self.input_files: list[File] = []
         self.output_files: list[File] = []
 
+    def start(self) -> None:
+        self.codebox.start()
+    
     async def astart(self) -> None:
+        if type(self.codebox) != CodeBox:
+            # check if jupyter-kernel-gateway is installed
+            import pkg_resources  # type: ignore
+            try:
+                pkg_resources.get_distribution("jupyter-kernel-gateway")
+            except pkg_resources.DistributionNotFound:
+                print(
+                    "Make sure 'jupyter-kernel-gateway' is installed when using without a CODEBOX_API_KEY.\n"
+                    "You can install it with 'pip install jupyter-kernel-gateway'."
+                )
+                exit(1)
         await self.codebox.astart()
 
     def _tools(
         self, 
         additional_tools: list[BaseTool]
     ) -> list[BaseTool]:
         return additional_tools + [
             StructuredTool(
                 name="python",
                 description=
                 # TODO: variables as context to the agent
                 # TODO: current files as context to the agent
                 "Input a string of code to a python interpreter (jupyter kernel). "
+                "Write the entire code in a single string. This string can "
+                "be really long, so you can use the `;` character to split lines. "
                 "Variables are preserved between runs. ",
-                func=self.run_handler,
-                coroutine=self.arun_handler,
+                func=self._run_handler,
+                coroutine=self._arun_handler,
                 args_schema=CodeInput,
             ),
         ]
 
-    def _llm(
-        self, 
-        model: str, 
-        openai_api_key: Optional[str] = None
+    def _choose_llm(
+        self,
+        model: str = "gpt-4",
+        openai_api_key: Optional[str] = None,
+        **kwargs
     ) -> BaseChatModel:
-        if openai_api_key is None:
-            raise ValueError(
-                "OpenAI API key missing. Set OPENAI_API_KEY env variable or pass `openai_api_key` to session."
+        if "gpt" in model:
+            openai_api_key = (
+                openai_api_key 
+                or settings.OPENAI_API_KEY 
+                or getenv("OPENAI_API_KEY", None)
+            )
+            if openai_api_key is None:
+                raise ValueError(
+                    "OpenAI API key missing. Set OPENAI_API_KEY env variable or pass `openai_api_key` to session."
+                )
+            return ChatOpenAI(
+                temperature=0.03,
+                model=model,
+                openai_api_key=openai_api_key,
+                max_retries=3,
+                request_timeout=60 * 3,
+            )  # type: ignore
+        elif "claude" in model:
+            return ChatAnthropic(model=model)
+        else:
+            raise ValueError(f"Unknown model: {model} (expected gpt or claude model)")
+
+    def _choose_agent(self) -> BaseSingleActionAgent:
+        return (
+            OpenAIFunctionsAgent.from_llm_and_tools(
+                llm=self.llm,
+                tools=self.tools,
+                system_message=code_interpreter_system_message,
+                extra_prompt_messages=[MessagesPlaceholder(variable_name="chat_history")],
+            )
+            if isinstance(self.llm, ChatOpenAI)
+            else ConversationalChatAgent.from_llm_and_tools(
+                llm=self.llm,
+                tools=self.tools,
+                system_message=code_interpreter_system_message.content,
+                output_parser=CodeChatAgentOutputParser(),
+            )
+            if isinstance(self.llm, BaseChatModel)
+            else ConversationalAgent.from_llm_and_tools(
+                llm=self.llm,
+                tools=self.tools,
+                prefix=code_interpreter_system_message.content,
+                output_parser=CodeAgentOutputParser(),
             )
-
-        return ChatOpenAI(
-            temperature=0.03,
-            model=model,
-            openai_api_key=openai_api_key,
-            max_retries=3,
-            request_timeout=60 * 3,
-        )  # type: ignore
-
-    def _agent(self) -> BaseSingleActionAgent:
-        return OpenAIFunctionsAgent.from_llm_and_tools(
-            llm=self.llm,
-            tools=self.tools,
-            system_message=code_interpreter_system_message,
-            extra_prompt_messages=[MessagesPlaceholder(variable_name="memory")],
         )
 
     def _agent_executor(self) -> AgentExecutor:
         return AgentExecutor.from_agent_and_tools(
-            agent=self._agent(),
+            agent=self._choose_agent(),
             callbacks=[CodeCallbackHandler(self)],
             max_iterations=9,
             tools=self.tools,
             verbose=self.verbose,
-            memory=ConversationBufferMemory(memory_key="memory", return_messages=True),
+            memory=ConversationBufferMemory(memory_key="chat_history", return_messages=True),
         )
 
     async def show_code(self, code: str) -> None:
         """Callback function to show code to the user."""
         if self.verbose:
             print(code)
 
-    def run_handler(self, code: str):
+    def _run_handler(self, code: str):
         raise NotImplementedError("Use arun_handler for now.")
 
-    async def arun_handler(self, code: str):
+    async def _arun_handler(self, code: str):
         """Run code in container and send the output to the user"""
+        print("Running code in container...", code)
         output: CodeBoxOutput = await self.codebox.arun(code)
 
         if not isinstance(output.content, str):
             raise TypeError("Expected output.content to be a string.")
 
         if output.type == "image/png":
             filename = f"image-{uuid.uuid4()}.png"
@@ -117,16 +160,17 @@
         elif output.type == "error":
             if "ModuleNotFoundError" in output.content:
                 if package := re.search(
                     r"ModuleNotFoundError: No module named '(.*)'", output.content
                 ):
                     await self.codebox.ainstall(package.group(1))
                     return f"{package.group(1)} was missing but got installed now. Please try again."
-            else: pass
+            else: 
                 # TODO: preanalyze error to optimize next code generation
+                pass
             if self.verbose:
                 print("Error:", output.content)
 
         elif modifications := await get_file_modifications(code, self.llm):
             for filename in modifications:
                 if filename in [file.name for file in self.input_files]:
                     continue
@@ -137,56 +181,58 @@
                 file_buffer.name = filename
                 self.output_files.append(
                     File(name=filename, content=file_buffer.read())
                 )
 
         return output.content
 
-    async def input_handler(self, request: UserRequest):
+    async def _input_handler(self, request: UserRequest):
         if not request.files:
             return
         if not request.content:
             request.content = (
                 "I uploaded, just text me back and confirm that you got the file(s)."
             )
         request.content += "\n**The user uploaded the following files: **\n"
         for file in request.files:
             self.input_files.append(file)
             request.content += f"[Attachment: {file.name}]\n"
             await self.codebox.aupload(file.name, file.content)
         request.content += "**File(s) are now available in the cwd. **\n"
 
-    async def output_handler(self, final_response: str) -> CodeInterpreterResponse:
+    async def _output_handler(self, final_response: str) -> CodeInterpreterResponse:
         """Embed images in the response"""
         for file in self.output_files:
             if str(file.name) in final_response:
                 # rm ![Any](file.name) from the response
                 final_response = re.sub(rf"\n\n!\[.*\]\(.*\)", "", final_response)
 
         if self.output_files and re.search(rf"\n\[.*\]\(.*\)", final_response):
-            final_response = await remove_download_link(final_response, self.llm)
+            try:
+                final_response = await remove_download_link(final_response, self.llm)
+            except Exception as e:
+                if self.verbose:
+                    print("Error while removing download links:", e)
 
         return CodeInterpreterResponse(content=final_response, files=self.output_files)
 
     async def generate_response(
         self,
         user_msg: str,
         files: list[File] = [],
         detailed_error: bool = False,
     ) -> CodeInterpreterResponse:
         """Generate a Code Interpreter response based on the user's input."""
         user_request = UserRequest(content=user_msg, files=files)
         try:
-            await self.input_handler(user_request)
+            await self._input_handler(user_request)
             response = await self.agent_executor.arun(input=user_request.content)
-            return await self.output_handler(response)
+            return await self._output_handler(response)
         except Exception as e:
             if self.verbose:
-                import traceback
-
                 traceback.print_exc()
             if detailed_error:
                 return CodeInterpreterResponse(
                     content=f"Error in CodeInterpreterSession: {e.__class__.__name__}  - {e}"
                 )
             else:
                 return CodeInterpreterResponse(
```

### Comparing `codeinterpreterapi-0.0.8/PKG-INFO` & `codeinterpreterapi-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: codeinterpreterapi
-Version: 0.0.8
-Summary: CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter.
+Version: 0.0.9
+Summary: CodeInterpreterAPI is an (unofficial) open source python interface for the ChatGPT CodeInterpreter.
 License: MIT
 Author: Shroominic
 Author-email: contact@shroominic.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: frontend
 Provides-Extra: image-support
-Provides-Extra: streamlit-support
-Requires-Dist: codeboxapi (>=0.0.11,<0.0.12)
-Requires-Dist: langchain (>=0.0.232,<0.0.233)
+Provides-Extra: localbox
+Requires-Dist: codeboxapi (>=0.0.14,<0.0.15)
+Requires-Dist: langchain (>=0.0.242,<0.0.243)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Code Interpreter API
 
 A LangChain implementation of the ChatGPT Code Interpreter.
@@ -36,17 +38,20 @@
 - Use CodeBox API for easy scaling in production (coming soon)
 
 ## Installation
 
 Get your OpenAI API Key [here](https://platform.openai.com/account/api-keys) and install the package.
 
 ```bash
-pip install codeinterpreterapi
+pip install "codeinterpreterapi[all]"
 ```
 
+Everything for local experiments are installed with the `all` extra.
+For deployments, you can use `pip install codeinterpreterapi` instead which does not install the additional dependencies.
+
 ## Usage
 
 Make sure to set the `OPENAI_API_KEY` environment variable (or use a `.env` file)
 
 ```python
 from codeinterpreterapi import CodeInterpreterSession
 
@@ -144,15 +149,15 @@
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Contact
 
 You can contact me at [contact@shroominic.com](mailto:contact@shroominic.com).
-But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://gptassistant.app/community) DMs.
+But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://discord.gg/QYzBtq37) DMs.
 
 ## Support this project
 
 If you would like to help this project with a donation, you can [click here](https://ko-fi.com/shroominic).
 Thanks, this helps a lot! ❤️
 
 ## Star History
```

