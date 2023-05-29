# Comparing `tmp/simple_chatgpt_cli-0.1.8.tar.gz` & `tmp/simple_chatgpt_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_chatgpt_cli-0.1.8.tar", max compression
+gzip compressed data, was "simple_chatgpt_cli-0.1.9.tar", max compression
```

## Comparing `simple_chatgpt_cli-0.1.8.tar` & `simple_chatgpt_cli-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1431 2023-05-13 20:16:11.168124 simple_chatgpt_cli-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.8/chatgpt_cli/__init__.py
--rw-r--r--   0        0        0     6998 2023-05-23 13:20:50.908136 simple_chatgpt_cli-0.1.8/chatgpt_cli/main.py
--rw-r--r--   0        0        0      701 2023-05-24 02:08:23.182621 simple_chatgpt_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1431 2023-05-13 20:16:11.168124 simple_chatgpt_cli-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.9/chatgpt_cli/__init__.py
+-rw-r--r--   0        0        0     7629 2023-05-24 14:07:54.932799 simple_chatgpt_cli-0.1.9/chatgpt_cli/main.py
+-rw-r--r--   0        0        0      701 2023-05-24 14:25:27.070273 simple_chatgpt_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.9/PKG-INFO
```

### Comparing `simple_chatgpt_cli-0.1.8/README.md` & `simple_chatgpt_cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `simple_chatgpt_cli-0.1.8/chatgpt_cli/main.py` & `simple_chatgpt_cli-0.1.9/chatgpt_cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,14 +115,42 @@
                 user_input += input() + "\n"
         except EOFError:
             pass
 
     return user_input
 
 
+def request_ai_response(
+    messages: list[Message], model: str, count_tries: int = 0
+) -> tuple[str, bool]:
+    try:
+        response = openai.ChatCompletion.create(  # type: ignore
+            model=model,
+            temperature=TEMPERATURE,
+            messages=[
+                {"role": message.role.value, "content": message.content}
+                for message in messages
+            ],
+        )
+        assert response.choices[0]["message"]["role"] == Role.ASSISTANT.value
+        return (
+            response.choices[0]["message"]["content"],
+            response.choices[0]["finish_reason"] == "length",
+        )
+    except Exception as e:
+        if count_tries < 3:
+            print(f"{WARNING_PREFIX} {e}")
+            print(f"{WARNING_PREFIX} Retrying...")
+            return request_ai_response(messages, model, count_tries + 1)
+        else:
+            print(f"{WARNING_PREFIX} {e}")
+            print(f"{WARNING_PREFIX} Failed to get response from OpenAI API.")
+            exit(1)
+
+
 def chat(
     model: str, has_previous_chat: bool, rollover_message: Message | None = None
 ) -> tuple[ChatExitReason, Message | None]:
     # welcome console message
     if not has_previous_chat:
         print(
             f"{INFO_PREFIX} You can now start chatting with the bot. \n"
@@ -165,34 +193,22 @@
                         timestamp=user_input_timestamp,
                     )
             messages.append(
                 Message(
                     role=Role.USER, content=user_input, timestamp=user_input_timestamp
                 )
             )
-
-        response = openai.ChatCompletion.create(  # type: ignore
-            model=model,
-            temperature=TEMPERATURE,
-            messages=[
-                {"role": message.role.value, "content": message.content}
-                for message in messages
-            ],
-        )
-        assert response.choices[0]["message"]["role"] == Role.ASSISTANT.value
-
-        bot_response = response.choices[0]["message"]["content"]
+        bot_response, is_max_token_exceeded = request_ai_response(messages, model)
         print(f"{BOT_DISPLAY_NAME}:", bot_response)
         messages.append(
             Message(
                 role=Role.ASSISTANT, content=bot_response, timestamp=int(time.time())
             )
         )
-
-        if response.choices[0]["finish_reason"] == "length":
+        if is_max_token_exceeded:
             Prompt.ask(
                 f"{WARNING_PREFIX} The total token count exceeds the maximum. You must start a new conversation. Press Enter to continue",
             )
             return ChatExitReason.START_OVER, None
 
 
 def run() -> None:
```

### Comparing `simple_chatgpt_cli-0.1.8/pyproject.toml` & `simple_chatgpt_cli-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 wrap-descriptions = 88
 
 [tool.poetry.scripts]
 chatgpt = 'chatgpt_cli.main:run'
 
 [tool.poetry]
 name = "simple-chatgpt-cli"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["tailaiw <29800495+tailaiw@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "chatgpt_cli" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `simple_chatgpt_cli-0.1.8/PKG-INFO` & `simple_chatgpt_cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-chatgpt-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: tailaiw
 Author-email: 29800495+tailaiw@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

