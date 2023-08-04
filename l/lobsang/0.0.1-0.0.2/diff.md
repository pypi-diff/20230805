# Comparing `tmp/lobsang-0.0.1.tar.gz` & `tmp/lobsang-0.0.2.tar.gz`

## Comparing `lobsang-0.0.1.tar` & `lobsang-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,21 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lobsang-0.0.1/.todo
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 lobsang-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lobsang-0.0.1/docs/GETTING_STARTED.md
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 lobsang-0.0.1/examples/simple.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 lobsang-0.0.1/examples/utilize_directives.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/__init__.py
--rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/chat.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/messages.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/directives/__init__.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/directives/base.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/directives/json.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/directives/text.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/llms/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/llms/base.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/llms/fake.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/prompts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/prompts/vicuna/__init__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/subroutines/__init__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 lobsang-0.0.1/lobsang/subroutines/base.py
--rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 lobsang-0.0.1/tests/test_chat.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 lobsang-0.0.1/tests/test_directives.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 lobsang-0.0.1/tests/test_messages.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 lobsang-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 lobsang-0.0.1/LICENSE
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 lobsang-0.0.1/README.md
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 lobsang-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 lobsang-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lobsang-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 lobsang-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 lobsang-0.0.2/examples/.env
+-rw-r--r--   0        0        0    31185 2020-02-02 00:00:00.000000 lobsang-0.0.2/examples/1_basics.ipynb
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/__init__.py
+-rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/chat.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/messages.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/directives/__init__.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/directives/base.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/directives/text.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/llms/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/llms/base.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/llms/fake.py
+-rw-r--r--   0        0        0    18340 2020-02-02 00:00:00.000000 lobsang-0.0.2/tests/test_chat.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 lobsang-0.0.2/tests/test_directives.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 lobsang-0.0.2/tests/test_messages.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 lobsang-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 lobsang-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 lobsang-0.0.2/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 lobsang-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 lobsang-0.0.2/PKG-INFO
```

### Comparing `lobsang-0.0.1/lobsang/chat.py` & `lobsang-0.0.2/lobsang/chat.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,287 +9,328 @@
 from lobsang.directives import Directive, TextDirective
 from lobsang.llms.base import LLM
 from lobsang.messages import Message, SystemMessage, UserMessage, AssistantMessage
 
 
 class Chat(list[Message]):
     """
-    A chat (subclass of list) holds a conversation between a user and an assistant. Each subsequent call of a chat
-    instance with a message, i.e. `chat(message)`, will
-        1. append the message,
-        2. send it and the chat history (the message context) to the LLM and
-        3. append the response to the chat as well
-
-    >>> # It's a list everyone! 🎉
-    >>> chat = Chat("You are a helpful assistant.")
-    >>> len(chat)
-    1
-    >>> message = chat[0]
-    >>> isinstance(message, SystemMessage)
-    True
-    >>> message.text
-    'You are a helpful assistant.'
+    A chat (subclass of list) holds a conversation between a user and an assistant which can be called with one or
+    more messages, i.e. `chat(message)` or `chat([message1, message2, ...])`.
+
+    **Disclaimer:** Not all methods of list were re-implemented, so some might not work as expected. If you need a
+    specific method, please open an issue or make a pull request on GitHub. Thanks! 🙏
     """
 
-    def __init__(self, data: str | Message | Sequence[Message] = (), llm: LLM = None):
+    def __init__(self, seq: Sequence[Message] = (),
+                 system_message: str | SystemMessage = "You are a helpful assistant.", llm: LLM = None) -> None:
         """
         Creates a new chat instance.
 
-        **Note**: The message(s) you provide won't be sent to the LLM until you call the chat using the `__call__`
-        method with a message. This setup allows you to define initial messages such as instructions and examples
-        before starting the actual conversation.
-
-        >>> # 1. Option: No parameters -> empty chat
-        >>> chat = Chat()
-        >>> len(chat)
-        0
-        >>>
-        >>> # 2. Option: A string -> chat with a SystemMessage
-        >>> chat = Chat("Hello World")
-        >>> isinstance(chat[0], SystemMessage)
-        True
-        >>> chat[0].text
-        'Hello World'
-        >>>
-        >>> # 3. Option: A Message -> chat with a Message (usually a SystemMessage to instruct the LLM)
-        >>> chat = Chat(SystemMessage("Hello World"))
-        >>> isinstance(chat[0], SystemMessage)
-        True
-        >>> chat[0].text
-        'Hello World'
-        >>>
-        >>> # 4. Option: A list of messages -> chat with the provided messages
-        >>> chat = Chat([SystemMessage("You are a helpful assistant."), UserMessage("My name is Bark Twain"),
-        ... AssistantMessage("Nice to meet you, Bark Twain!")])
-        >>> len(chat)
-        3
-
-        :param data: The message(s) to initialize the chat.
-        :param llm: The language model to use. Currently, only OpenAI's API is supported.
-        :raises TypeError: If data is not of type str, Message or Sequence[Message].
-        """
-        if isinstance(data, (str, Message)):
-            data = [SystemMessage(data)] if isinstance(data, str) else [data]
-        elif isinstance(data, Sequence):
-            self._assert_all_messages(data)
-        else:
-            raise TypeError(f"Expected str, Message or Sequence[Message], got {type(data)} instead.")
-
-        super().__init__(data)
-        # If debug log level warn if llm is not set
+        :param seq: A sequence of messages to initialize the chat with.
+        :param llm: The language model to use.
+        """
+        assert isinstance(seq, Sequence), f"Expected 'Sequence' but got {type(seq)} for 'seq'."
+        assert all(isinstance(m, Message) for m in seq), f"Found non-Message element in 'seq'."
+        assert isinstance(system_message, (str, SystemMessage)), \
+            f"Expected 'str' or 'SystemMessage' but got {type(system_message)}."
+
+        # Convert system_message to SystemMessage if necessary
+        if isinstance(system_message, str):
+            system_message = SystemMessage(system_message)
+
+        # Set attributes
+        super().__init__(seq)
+        self.system_message = system_message
         self.llm = llm
 
-    def __call__(self, data: str | Message | Sequence[str | Message | Directive]) -> list[Message]:
+    def __call__(self, msg: str | UserMessage, append: bool = True,
+                 system_message: str | SystemMessage = None) -> AssistantMessage:
         """
-        Calls the chat with a message or a list of message(s) and returns the response(s) from the LLM.
-        All messages (more accurately all directives) are sent to the LLM one by one in the order they are provided.
+        Convenience wrapper for `Chat.run()` to be able to call chat with a single message, i.e. `chat(message)`.
+        Returns the response from the LLM. Internally simply calls `chat.run([message])`. See `Chat.run()` for more
+        information.
 
         >>> from lobsang.llms import FakeLLM
-        >>> chat = Chat("You are a helpful assistant.", llm=FakeLLM())
-        >>> len(chat)
-        1
-        >>> res = chat("My name is Bark Twain")
-        >>> res[1].text
-        "DUMMY RESPONSE for 'My name is Bark Twain'"
-        >>> len(chat)
-        3
-        >>> res = chat(["What is 1+1?", "What is 2+2?"])
-        >>> res[1].text
-        "DUMMY RESPONSE for 'What is 1+1?'"
-        >>> res[3].text
-        "DUMMY RESPONSE for 'What is 2+2?'"
-
-        :param data: The message(s) to send to the LLM.
-        :return: The corresponding chat snippet, i.e. the message(s) you provided and the response(s) from the LLM.
-        :raises ValueError: If no LLM set.
-        :raises TypeError: If data is not of type str, Message or Sequence[Message | Directive].
-        """
-        # Ensure that an LLM is set
-        if not isinstance(self.llm, LLM):
-            raise ValueError("No LLM set. Please set self.llm to an instance of an LLM (e.g. 'Chat(llm=OpenAI())')")
-
-        # If data is a string or a Message, convert it to a list of messages
-        if isinstance(data, (str, Message)):
-            data = [data]
-
-        # Convert all strings to UserMessages
-        data = [UserMessage(item) if isinstance(item, str) else item for item in data]
-        self._assert_all_messages(data, allowed_types=(Message, Directive))
-
-        # Insert default directive (TextDirective) after all messages, which are not followed by a directive. This
-        # is necessary as the LLM is called on directives and not on messages. So we need a corresponding directive for
-        # each message. For example the list [user_msg, user_msg, directive, user_msg] would be converted to
-        # [user_msg, TextDirective, user_msg, directive, user_msg, TextDirective] (i.e. 2 TextDirectives are inserted).
-        *rest, last = data
-        for i, item in enumerate(rest):
-            if isinstance(item, UserMessage) and not isinstance(data[i + 1], (AssistantMessage, Directive)):
-                data.insert(i + 1, TextDirective())
-        else:
-            # Handle last message, which would raise an IndexError if handled in the loop
-            if isinstance(last, UserMessage):
-                data.append(TextDirective())
-
-        # Loop through data, add non-directives to chat and send directives to LLM
-        for item in data:
-            if isinstance(item, Message):
-                self.append(item)
-            elif isinstance(item, Directive):
-                self._invoke_with_directive(item)
+        >>> chat = Chat(llm=FakeLLM())
+        >>> res = chat("My name is Bark Twain")  # 👈 Internally converted to UserMessage for convenience
+        >>> chat == res
+        True
+        >>> str(chat[-1])
+        "ASSISTANT: DUMMY RESPONSE for 'My name is Bark Twain'"
+
+        :param msg: The message to send to the LLM.
+        :param append: Whether to append the conversation to the chat history.
+        :param system_message: The system message to use. If None, the chat's system message is used.
+        :return: The response from the LLM.
+        """
+        assert isinstance(msg, (str, UserMessage)), f"Expected 'str' or 'UserMessage' but got {type(msg)} for 'msg'."
+
+        res = self.run([msg], append=append, system_message=system_message)[-1]
+        assert isinstance(res, AssistantMessage), f"Expected 'AssistantMessage' but got {type(res)} for 'res'."
+
+        return res
+
+    def run(self, seq: Sequence[str | Message | Directive], append: bool = True,
+            system_message: str | SystemMessage = None) -> list[Message]:
+        """
+        Calls the chat with a seq of messages and directives, i.e. `chat([user_msg, directive, ...])`.
+        Returns the conversation with all messages and corresponding responses from the LLM.
+
+        **Note:** All messages of type `str` will be implicitly converted to `UserMessage` for convenience.
+
+        :param seq: The messages and directives to send to the LLM.
+        :param append: Whether to append the conversation to the chat history.
+        :param system_message: The system message to use. If None, the chat's system message is used.
+        :return: The conversation with all messages and corresponding responses from the LLM.
+        :raises TypeError: If data is not of correct type (see note above).
+        """
+        assert isinstance(seq, Sequence), f"Expected 'Sequence' but got {type(seq)} for 'seq'."
+        assert len(seq) > 0, "Expected non-empty sequence for 'seq'."
+        assert all(isinstance(m, (str, Message, Directive)) for m in seq), \
+            "Expected only 'str', 'Message' or 'Directive' as elements of 'seq'."
+        assert isinstance(self.llm, LLM), "Expected 'LLM' but got {type(self.llm)} for 'self.llm'."
+
+        # Check if system_message is set and convert to SystemMessage if necessary
+        system_message = system_message or self.system_message
+        system_message = SystemMessage(system_message) if isinstance(system_message, str) else system_message
+        assert isinstance(system_message, SystemMessage), \
+            f"Expected 'str' or 'SystemMessage' but got {type(system_message)} for 'system_message'."
+
+        # Convert strings to UserMessages
+        seq = [UserMessage(m) if isinstance(m, str) else m for m in seq]
+
+        # Interpolate messages (add default directives [TextDirective] after messages if necessary)
+        seq = self._interpolate(seq)
+
+        # Loop through data and invoke LLM
+        conversation = []
+        for elem in seq:
+            if isinstance(elem, Message):
+                conversation.append(elem)
+            elif isinstance(elem, Directive):
+                assistant_message = self._invoke_with_directive(directive=elem, context=[*self, *conversation],
+                                                                system_message=system_message)
+                conversation.append(assistant_message)
             else:
-                raise TypeError(f"Expected Message or Directive, got {type(item)} instead.")
+                raise NotImplementedError(f"Cannot handle {type(elem)}. "
+                                          f"Only Message and Directive are supported for now.")
 
-        # Return response(s)
-        return self[-len(data):]
+        # If flag is set, append conversation to chat
+        if append:
+            self.extend(conversation)
 
-    def _invoke_with_directive(self, directive: Directive) -> AssistantMessage:
+        return conversation
+
+    @staticmethod
+    def _interpolate(seq: Sequence[Message | Directive], default_directive=TextDirective()) -> list[Message]:
         """
-        Invokes the LLM with a directive.
+        Interpolates the provided sequence with default directives (TextDirective) if necessary.
 
-        The provided directive is applied to the last message in the chat. The LLM then processes the chat history
-        including the last message (the query). The response is parsed using the directive and appended to the chat.
-        **Caution:** This method is not idempotent, i.e. it will change the chat history.
+        **Details:** For convenience, we do not require a directive after each unanswered message, i.e. this is fine:
+        `[user_msg, user_msg, directive, user_msg]`. However, the LLM is called on directives and not on messages. So we
+        need a corresponding directive for each message. This is done by inserting the provided default directive after
+        each user message if it is directly followed by another user message.
+
+        **Example:** `[user_msg, user_msg, directive, user_msg]` is interpolated to `[user_msg, TextDirective, user_msg,
+        directive, user_msg, TextDirective]`, i.e. 2 TextDirectives are inserted.
+
+        :param seq: The sequence to interpolate.
+        :param default_directive: The default directive to interpolate with.
+        :return: The interpolated sequence.
+        """
+        assert isinstance(seq, Sequence), f"Expected 'Sequence' but got {type(seq)} for 'seq'."
+        assert len(seq) > 0, "Expected non-empty sequence for 'seq'."
+        assert all(isinstance(item, (Message, Directive)) for item in seq), \
+            "Expected only 'Message' or 'Directive' as elements of 'seq'."
+        assert isinstance(default_directive, Directive), \
+            f"Expected 'Directive' but got {type(default_directive)} for 'default_directive'."
+
+        # Split sequence into head and last item to avoid IndexError
+        *head, last = seq
+        interpolated = []
+
+        # Loop through head and add items to interpolated if necessary
+        for idx, elem in enumerate(head):
+            interpolated.append(elem)
+
+            # When two user messages directly follow each other, add a TextDirective
+            if isinstance(elem, UserMessage) and isinstance(seq[idx + 1], UserMessage):
+                interpolated.append(default_directive)
+
+        # Append last item and, if necessary, a TextDirective
+        interpolated.append(last)
+        if isinstance(last, UserMessage):
+            interpolated.append(default_directive)
 
-        :param directive: The directive to invoke the LLM with.
-        :return: The response from the LLM as an AssistantMessage (also appended to the chat) for convenience.
-        :raises TypeError: If the last message in the chat is not a UserMessage.
+        return interpolated
+
+    def _invoke_with_directive(self, directive: Directive, context: Sequence[Message],
+                               system_message: str | SystemMessage = None) -> AssistantMessage:
         """
-        query = self[-1]
+        Invokes the LLM with a directive.
+
+        **Details:** The directive is applied to the last message in the context (embeds the directive's instructions
+        into the message). The LLM then processes all together (system message, context, directive) and returns the
+        response which is parsed using the directive and returned as an AssistantMessage.
 
-        if not isinstance(query, UserMessage):
-            raise TypeError(f"Expected UserMessage, got {type(query)} instead.")
+        :param directive: The directive to invoke the LLM with.
+        :param context: The context to invoke the LLM with, i.e. a sequence of messages
+        :param system_message: The system message to use. If None, the chat's system message is used.
+        :return: The response from the LLM as an AssistantMessage.
+        """
+        assert isinstance(directive, Directive), f"Expected 'Directive' but got {type(directive)} for 'directive'."
+        assert isinstance(context, Sequence), f"Expected 'Sequence' but got {type(context)} for 'context'."
+        assert len(context) > 0, "Expected non-empty sequence for 'context'."
+        assert all(isinstance(m, Message) for m in context), "Expected only 'Message' as elements of 'context'."
+
+        # Check if system_message is set and convert to SystemMessage if necessary
+        system_message = system_message or self.system_message
+        system_message = SystemMessage(system_message) if isinstance(system_message, str) else system_message
+        assert isinstance(system_message, SystemMessage), \
+            f"Expected 'str' or 'SystemMessage' but got {type(system_message)} for 'system_message'."
 
-        # Update query with directive (embed instructions into text, update info)
+        # Embed directive's instructions into query (i.e. last message in context)
+        query = context[-1]
         query.text, directive_info = directive.embed(query.text)
         query.info.update(directive_info)
 
-        # Invoke LLM with chat as context
-        response, llm_info = self.llm.chat(self)
+        # Invoke LLM with system message and context
+        system_message = system_message or self.system_message
+        response, llm_info = self.llm.chat([system_message, *context])
 
         # Parse response
         parsed_response, directive_info = directive.parse(response)
 
-        # Create AssistantMessage
+        # Create and return assistant message
         assistant_info = llm_info | directive_info | {'directive': directive, 'query': query}
         assistant_message = AssistantMessage(parsed_response, info=assistant_info)
-
-        self.append(assistant_message)
         return assistant_message
 
-    def __setitem__(self, __i: SupportsIndex, __o: Message) -> None:
+    def __setitem__(self, idx: SupportsIndex, item) -> None:
         """
         Sets an item at a given index in the chat.
 
-        :param __i: The index to set the message at.
-        :param __o: The message to set.
-        :raises IndexError: If __i is out of range.
-        :raises TypeError: If __o is not of type Message.
+        :param idx: The index to set the message at.
+        :param item: The message to set.
         """
-        if not isinstance(__o, Message):
-            raise TypeError(f"Expected Message, got {type(__o)} instead.")
+        # If item is a slice, check if all items are messages
+        if isinstance(idx, slice):
+            assert all(isinstance(msg, Message) for msg in item), \
+                "Expected only 'Message' as elements of slice 'item'."
+        else:
+            assert isinstance(item, Message), f"Expected 'Message' but got {type(item)} for 'item'."
 
-        super().__setitem__(__i, __o)
+        super().__setitem__(idx, item)
 
-    def __add__(self, other: Sequence[Message]):
+    def __getitem__(self, item):
         """
-        Concatenates two chats using the + operator.
+        Gets an item from the chat.
 
-        >>> chat = Chat("You are a helpful assistant.")
-        >>> messages = [UserMessage("My name is Bark Twain"), AssistantMessage("Nice to meet you, Bark Twain!")]
-        >>> chat + messages == chat.__add__(messages) == Chat([*chat, *messages])
-        True
+        :param item: The item to get.
+        :return: The item.
+        """
+        # If item is a slice, return a new chat with the sliced messages
+        if isinstance(item, slice):
+            return Chat(super().__getitem__(item), self.system_message, self.llm)
+        else:
+            return super().__getitem__(item)
+
+    def __add__(self, other):
+        # Not supported bc how to handle the system message and the LLM? 🤔
+        raise NotImplementedError("Not supported. Use extend() instead.")
 
-        :param other: A sequence of messages to concatenate with the chat.
-        :return: A new chat containing the messages of both chats.
-        :raises TypeError:  If other is not of type Sequence[Message].
+    def __radd__(self, other):
+        # Not supported bc how to handle the system message and the LLM? 🤔
+        raise NotImplementedError("Not supported. Use extend() instead.")
+
+    def copy(self) -> "Chat":
         """
-        return Chat([*self, *other])
+        Returns a shallow copy of the chat.
 
-    def append(self, __object: Message) -> None:
+        :return: The shallow copy.
         """
-        Appends a message to the chat.
+        return Chat(self, self.system_message, self.llm)
 
-        :param __object: The message to append.
-        :raises TypeError: If __object is not of type Message.
+    def append(self, msg: Message) -> None:
         """
-        if not isinstance(__object, Message):
-            raise TypeError(f"Expected Message, got {type(__object)} instead.")
+        Appends a message to the chat.
 
-        super().append(__object)
+        :param msg: The message to append.
+        """
+        assert isinstance(msg, Message), f"Expected 'Message' but got {type(msg)} for 'msg'."
+        super().append(msg)
 
-    def extend(self, sequence: Sequence[Message]) -> None:
+    def extend(self, seq: Sequence[Message]) -> None:
         """
-        Extends the list by appending all items from the sequence.
-        :param sequence: The messages to extend the chat with.
-        :raises TypeError: If sequence is not of type sequence[Message].
+        Extends the list by the given sequence of messages.
+
+        :param seq: The sequence of messages to extend the list with.
         """
-        if not isinstance(sequence, Sequence):
-            raise TypeError(f"Expected a sequence of Messages, but got {type(sequence)} instead.")
+        assert isinstance(seq, Sequence), f"Expected 'Sequence' but got {type(seq)} for 'seq'."
+        assert all(isinstance(m, Message) for m in seq), "Expected only 'Message' as elements of 'seq'."
 
-        self._assert_all_messages(sequence)
-        super().extend(sequence)
+        super().extend(seq)
 
-    def insert(self, __index: SupportsIndex, __object: Message) -> None:
+    def insert(self, idx: SupportsIndex, msg: Message) -> None:
         """
         Inserts a message at a given index into the chat history.
 
-        :param __index: The index to insert the message at.
-        :param __object: The message to insert.
-        :raises TypeError: If __object is not of type Message.
+        :param idx: The index to insert the message at.
+        :param msg: The message to insert.
         """
-        if not isinstance(__object, Message):
-            raise TypeError(f"Expected Message, got {type(__object)} instead.")
-
-        super().insert(__index, __object)
+        assert isinstance(msg, Message), f"Expected 'Message' but got {type(msg)} for 'msg'."
+        super().insert(idx, msg)
 
     def sort(self, *args, **kwargs):
-        raise NotImplementedError("Alas, the mystical art of sorting remains a secret yet to be unlocked "
-                                  "in this enchanted realm of code. 🧙‍♂️")
+        # Not supported bc why the hell would you want to sort a chat? By what criterion? 🤔
+        # If you try this, a magic wizard will appear and cast a spell on you to turn you into a frog
+        raise NotImplementedError("🧙‍♂️ Thou shalt not sort a chat! Ribbit ribbit. 🐸")
 
     def validate(self):
         """
-        Validates the chat according to the following rules:
-        1. The chat must start with a SystemMessage
-        2. Messages after the first message must alternate between UserMessage and AssistantMessage,
-        starting with a UserMessage.
+        Validates the chat, by checking if it is a sequence of alternating user and assistant messages, starting with a
+        user message.
+
+        **Examples:**
+        - `[user_msg, assistant_msg, user_msg, assistant_msg]` would be valid.
+        - `[user_msg, assistant_msg, user_msg]` would be invalid. (odd number of messages, missing assistant message)
+        - `[assistant_msg, user_msg, assistant_msg, user_msg]` would be invalid. (not starting with user message)
+        - `[user_msg, user_msg, assistant_msg, user_msg]` would be invalid. (two user messages in a row)
 
         :return: True if the chat is valid, otherwise raises a ValueError.
         :raises ValueError: If the chat is not valid.
         """
-        if not self:
+        if len(self) == 0:
             return True
 
-        if not isinstance(self[0], SystemMessage):
-            raise ValueError(f"Expected the first message to be a SystemMessage, but got {type(self[0])} instead.")
-
-        for i, message in enumerate(self[1:], start=0):
+        for i, message in enumerate(self):
             if i % 2 == 0 and not isinstance(message, UserMessage):
                 raise ValueError(f"Expected a UserMessage at index {i}, but got {type(message)} instead.")
             elif i % 2 == 1 and not isinstance(message, AssistantMessage):
-                raise ValueError(f"Expected a AssistantMessage at index {i}, "
-                                 f"but got {type(message)} instead.")
+                raise ValueError(f"Expected a AssistantMessage at index {i}, but got {type(message)} instead.")
 
+        # Check if the chat ends with an assistant message.
+        if not isinstance(self[-1], AssistantMessage):
+            raise ValueError("Chat is missing an assistant message at the end.")
+
+        # If we got here, the chat is valid 🎉 Passing the loop above implies that the chat starts with a user message
+        # and alternates between user and assistant messages. Finally, we checked that the chat ends with an assistant
+        # message. Therefore, each user message is followed by an assistant message, and the chat is valid. QED.
         return True
 
-    @staticmethod
-    def _assert_all_messages(sequence: Sequence, allowed_types=(Message,)):
+    def __str__(self, sep='\n'):
         """
-        Asserts that all items in the sequence are of one of the allowed types.
+        Returns a string representation of the chat HISTORY.
 
-        :param sequence: The sequence to assert.
-        :param allowed_types: The allowed types.
-        :raises TypeError: If sequence contains items that are not of one of the allowed types.
-        """
-        invalid_items = [(i, item, type(item)) for i, item in enumerate(sequence) if
-                         not isinstance(item, allowed_types)]
-        if invalid_items:
-            raise TypeError(
-                f"Expected items of type Message, but got {len(invalid_items)} invalid items:\n{invalid_items}")
-
-    def __str__(self):
-        return str([*map(str, self)])
+        :param sep: The separator to use between messages.
+        """
+        return sep.join(map(str, self))
 
     def __repr__(self):
-        # Show only the first and last two messages if the chat is longer than 4 messages
-        excerpt = [*map(str, self[:2]), "...", *map(str, self[-2:])] if len(self) > 4 else [*map(str, self)]
+        """
+        Returns a string representation of the chat OBJECT.
+        """
+        # Show only the first and last message if the chat is longer than 4 messages
+        excerpt = f"[{self[0]}, ..., {self[-1]}]" if len(self) > 4 else list(map(str, self))
 
         return f"Chat(llm={self.llm.__class__.__name__ if isinstance(self.llm, LLM) else self.llm}, " \
-               f"total_messages={len(self)}), messages={excerpt}"
+               f"system_message='{self.system_message}', total_messages={len(self)}, messages={excerpt}"
```

### Comparing `lobsang-0.0.1/lobsang/messages.py` & `lobsang-0.0.2/lobsang/messages.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.1/lobsang/directives/__init__.py` & `lobsang-0.0.2/lobsang/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.1/lobsang/directives/base.py` & `lobsang-0.0.2/lobsang/directives/base.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.1/lobsang/directives/text.py` & `lobsang-0.0.2/lobsang/directives/text.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.1/lobsang/llms/base.py` & `lobsang-0.0.2/lobsang/llms/base.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.1/lobsang/llms/fake.py` & `lobsang-0.0.2/lobsang/llms/fake.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.1/LICENSE` & `lobsang-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.1/README.md` & `lobsang-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-[//]: # (TODO: replace heading with text mask on blimp image)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/lobsang)
+![GitHub](https://img.shields.io/github/license/cereisen/lobsang)
+![GitHub issues](https://img.shields.io/github/issues/cereisen/lobsang)
+[![Discord](https://img.shields.io/discord/1137030158323294331)](https://discord.gg/wMHVAaqh)
+[![Twitter Follow](https://img.shields.io/twitter/follow/lobsang_ai)](https://twitter.com/lobsang_ai)
+
+
 # Lobsang
 
 > **Welcome to Lobsang** 🧘‍♂️
 > 
 > Lobsang is a framework to interact with conversational LLMs in the simplest way possible. \
 > It's easy to get started, yet designed to scale up to complex use cases. Enjoy the ride! 🚀
 
@@ -23,15 +29,15 @@
     It is the main entry point to the framework and stores the chat history for a single conversation. 
     After creating a `Chat` instance, you can interact with it by calling itself with one
     or more messages:
     ```python
     from lobsang import Chat
     from lobsang.llms import FakeLLM
     chat = Chat(llm=FakeLLM()) 
-    #                 👆 FakeLLL returns dummy responses
+    #                 👆 FakeLLM returns dummy responses
     # Call the chat with one message
     chat("Hello!")
     chat("How are you?")
     print("Chat history:")  
     print(chat)
     
     # Call the chat with multiple messages
@@ -41,17 +47,12 @@
     print("Full chat history:")
     print(chat)
     ```
   - **Directives**: Directives are used to guide the LLM to generate a specific response by embedding instructions
       in a corresponding message. For example, you can use the JSON directive to instruct the LLM to generate a JSON
       response (see [examples/utilize_directives.py](./examples/utilize_directives.py) for more details).
 
-## Documentation
-For a detailed documentation, check out the [docs](./docs) folder.
-
-[//]: # (TODO: add link to documentation website)
-
 ## Examples
 We provide a few examples to get you started. You can find them in the [examples](./examples) folder.
 The examples use the openai package, make sure to install it before running the examples (`pip install openai`).
 You will also need an OpenAI API key, which you can get here: https://platform.openai.com/account/api-keys.
```

