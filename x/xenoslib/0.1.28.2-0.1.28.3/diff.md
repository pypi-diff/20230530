# Comparing `tmp/xenoslib-0.1.28.2.tar.gz` & `tmp/xenoslib-0.1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.28.2.tar", last modified: Mon May 29 02:29:50 2023, max compression
+gzip compressed data, was "xenoslib-0.1.28.3.tar", last modified: Tue May 30 05:57:25 2023, max compression
```

## Comparing `xenoslib-0.1.28.2.tar` & `xenoslib-0.1.28.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:29:50.380768 xenoslib-0.1.28.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-29 02:29:50.380768 xenoslib-0.1.28.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:29:50.380768 xenoslib-0.1.28.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:29:50.376768 xenoslib-0.1.28.2/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:29:50.380768 xenoslib-0.1.28.2/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:57:25.391021 xenoslib-0.1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 05:57:25.387021 xenoslib-0.1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 05:57:25.391021 xenoslib-0.1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:57:25.387021 xenoslib-0.1.28.3/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-30 05:57:14.000000 xenoslib-0.1.28.3/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:57:25.387021 xenoslib-0.1.28.3/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 05:57:25.000000 xenoslib-0.1.28.3/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-30 05:57:25.000000 xenoslib-0.1.28.3/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:57:25.000000 xenoslib-0.1.28.3/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-30 05:57:25.000000 xenoslib-0.1.28.3/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 05:57:25.000000 xenoslib-0.1.28.3/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.28.2/LICENSE` & `xenoslib-0.1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/README.md` & `xenoslib-0.1.28.3/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/setup.py` & `xenoslib-0.1.28.3/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/xenoslib/base.py` & `xenoslib-0.1.28.3/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/xenoslib/dev.py` & `xenoslib-0.1.28.3/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/xenoslib/extend.py` & `xenoslib-0.1.28.3/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/xenoslib/linux.py` & `xenoslib-0.1.28.3/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/xenoslib/mail.py` & `xenoslib-0.1.28.3/xenoslib/mail.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,29 +65,24 @@
 
     def parse_emails(self, emails):
         for msg_id, msg in emails.items():
             if msg_id in self.msg_ids:
                 continue
             body = email.message_from_bytes(msg[b"BODY[]"])
             subject = str(email.header.make_header(email.header.decode_header(body["Subject"])))
-            sender = body["From"]
-            date = body["Date"]
+
             payload = body.get_payload(decode=True)
             if payload:
                 payload = payload.decode()
             internal_date = msg[b"INTERNALDATE"]
-            email_data = {
-                "body": body,
-                "subject": subject,
-                "payload": payload,
-                "date": date,
-                "sender": sender,
-                "internal_date": internal_date,
-            }
-            yield email_data
+            
+            body['subject'] = subject
+            body['payload'] = payload
+            body['internal_date'] = internal_date
+            yield body
             self.msg_ids.append(msg_id)
 
     def fetch_emails(self):
         """Login and fetch emails."""
         logger.debug(f"Fetching emails from the past {self.days} day(s)...")
         date_str = datetime.datetime.today() - datetime.timedelta(days=self.days)
         with IMAPClient(self.imap_server, timeout=30) as client:
```

### Comparing `xenoslib-0.1.28.2/xenoslib/mock.py` & `xenoslib-0.1.28.3/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/xenoslib/onedrive.py` & `xenoslib-0.1.28.3/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/xenoslib/win_trayicon.py` & `xenoslib-0.1.28.3/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.2/xenoslib/windows.py` & `xenoslib-0.1.28.3/xenoslib/windows.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
 
     def update(self, environs):
         for key, value in environs.items():
             self.set(key, value)
         self.refresh()
 
 
-
 def add_windows_path_env(new_path):
     """Add directory to Windows path environment variable"""
     env = Environment()
     path_str = env.get("Path")
     path_list = path_str.split(";")
     if new_path in path_list:
         print(f"{new_path} already exists in the path, skip.")
```

