# Comparing `tmp/streamlit_chatbox-0.1.1-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3924 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     7601 b- defN 23-May-28 14:21 streamlit_chatbox/__init__.py
--rw-rw-rw-  2.0 fat     1252 b- defN 23-May-28 14:25 streamlit_chatbox-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 14:25 streamlit_chatbox-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-28 14:25 streamlit_chatbox-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      424 b- defN 23-May-28 14:25 streamlit_chatbox-0.1.1.dist-info/RECORD
-5 files, 9387 bytes uncompressed, 3128 bytes compressed:  66.7%
+Zip file size: 3996 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     7876 b- defN 23-May-30 10:02 streamlit_chatbox/__init__.py
+-rw-rw-rw-  2.0 fat     1305 b- defN 23-May-30 10:11 streamlit_chatbox-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 10:11 streamlit_chatbox-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-30 10:11 streamlit_chatbox-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      424 b- defN 23-May-30 10:11 streamlit_chatbox-0.1.2.dist-info/RECORD
+5 files, 9715 bytes uncompressed, 3200 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: streamlit_chatbox/__init__.py
 Comment: 
 
-Filename: streamlit_chatbox-0.1.1.dist-info/METADATA
+Filename: streamlit_chatbox-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-0.1.1.dist-info/WHEEL
+Filename: streamlit_chatbox-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-0.1.1.dist-info/top_level.txt
+Filename: streamlit_chatbox-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-0.1.1.dist-info/RECORD
+Filename: streamlit_chatbox-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/__init__.py

```diff
@@ -12,22 +12,24 @@
 class StChatBox:
     def __init__(
         self,
         chat_box,
         session_var='chat_box',
         greetings=[],
         box_margin='10%',
+        box_border='1px solid',
         user_bg_color='#77ff77',
         user_icon='',
         robot_bg_color='#ccccee',
         robot_icon='',
     ):
         self.session_var = session_var
         self.greetings = greetings
         self.box_margin = box_margin
+        self.box_border = box_border
         self.user_bg_color = user_bg_color
         self.user_icon = user_icon
         self.robot_bg_color = robot_bg_color
         self.robot_icon = robot_icon
         self.last_response = None
         self.chat_box = chat_box
         self.init_session()
@@ -45,36 +47,39 @@
     def welcomed(self):
         return st.session_state.get(self.session_var, {}).get('welcomed', False)
 
     @welcomed.setter
     def welcomed(self, val):
         st.session_state[self.session_var]['welcomed'] = bool(val)
 
-    def format_md(self, msg, is_user=False, bg_color=None, margin=None):
+    def format_md(self, msg, is_user=False, bg_color=None, margin=None, border=None):
         '''
         将文本消息格式化为markdown文本
         '''
         margin = margin or self.box_margin
+        border = border or self.box_border
         if is_user:
             bg_color = bg_color or self.user_bg_color
             text = f'''
                     <div style="background:{bg_color};
                             margin-left:{margin};
+                            border: {border};
                             word-break:break-all;
                             float:right;
                             padding:2%;
                             border-radius:0 20px 0 0;">
                     {msg}
                     </div>
                     '''
         else:
             bg_color = bg_color or self.robot_bg_color
             text = f'''
                     <div style="background:{bg_color};
                             margin-right:{margin};
+                            border: {border};
                             word-break:break-all;
                             padding:2%;
                             border-radius:20px 0 0 0;">
                     {msg}
                     </div>
                     '''
         return text
@@ -160,33 +165,33 @@
         if self.last_response is not None:
             self.history[-1]['content'] = msg
             self.last_response.markdown(
                 self.format_md(msg, False),
                 unsafe_allow_html=True
             )
 
-    def robot_stream(self, msg, words_per_sec=10, max_seconds=10):
+    def robot_stream(self, msg, init_msg='', words_per_sec=10, max_seconds=10):
         step = max(words_per_sec, len(msg) // max_seconds + 1) // 5 + 1
-        self.robot_say('')
+        self.robot_say(init_msg)
         self.output_messages()
         for i in range(step, len(msg) + step * 2, step):
-            print(i, msg[:i])
             time.sleep(0.2)
             self.update_last_box_text(msg[:i])
 
     def clear_history(self, welcome_again=False):
         self.history = []
         if welcome_again:
             self.show_welcome()
 
 
 def st_chatbox(
         session_var='chat_box',
         greetings=[],
         box_margin='10%',
+        box_border='1px solid',
         user_bg_color='#77ff77',
         user_icon='https://tse2-mm.cn.bing.net/th/id/OIP-C.LTTKrxNWDr_k74wz6jKqBgHaHa?w=203&h=203&c=7&r=0&o=5&pid=1.7',
         robot_bg_color='#ccccee',
         robot_icon='https://ts1.cn.mm.bing.net/th/id/R-C.5302e2cc6f5c7c4933ebb3394e0c41bc?rik=z4u%2b7efba5Mgxw&riu=http%3a%2f%2fcomic-cons.xyz%2fwp-content%2fuploads%2fStar-Wars-avatar-icon-C3PO.png&ehk=kBBvCvpJMHPVpdfpw1GaH%2brbOaIoHjY5Ua9PKcIs%2bAc%3d&risl=&pid=ImgRaw&r=0',
 ):
     '''
     :param session_var: variable name used to store chat history in session_state
@@ -200,12 +205,13 @@
     '''
     empty = st.empty()
     return StChatBox(
         chat_box=empty,
         session_var=session_var,
         greetings=greetings,
         box_margin=box_margin,
+        box_border=box_border,
         user_bg_color=user_bg_color,
         user_icon=user_icon,
         robot_bg_color=robot_bg_color,
         robot_icon=robot_icon
     )
```

## Comparing `streamlit_chatbox-0.1.1.dist-info/METADATA` & `streamlit_chatbox-0.1.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: A chat box used in streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -48,9 +48,13 @@
     if streaming:
         chat_box.robot_stream(text)
     else:
         chat_box.robot_say(text)
 
 chat_box.output_messages()
 ```
+
+use `help(st_chatbox)` to see more custom params.
+
+
 ![demo](https://github.com/liunux4odoo/streamlit-chatbox/blob/master/demo.gif)
```

