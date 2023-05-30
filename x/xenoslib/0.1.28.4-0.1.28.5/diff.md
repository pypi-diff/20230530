# Comparing `tmp/xenoslib-0.1.28.4.tar.gz` & `tmp/xenoslib-0.1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.28.4.tar", last modified: Tue May 30 06:14:29 2023, max compression
+gzip compressed data, was "xenoslib-0.1.28.5.tar", last modified: Tue May 30 06:47:28 2023, max compression
```

## Comparing `xenoslib-0.1.28.4.tar` & `xenoslib-0.1.28.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:29.028062 xenoslib-0.1.28.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 06:14:29.028062 xenoslib-0.1.28.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:14:29.028062 xenoslib-0.1.28.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:29.024062 xenoslib-0.1.28.4/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-30 06:14:07.000000 xenoslib-0.1.28.4/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:29.024062 xenoslib-0.1.28.4/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 06:14:29.000000 xenoslib-0.1.28.4/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-30 06:14:29.000000 xenoslib-0.1.28.4/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:14:29.000000 xenoslib-0.1.28.4/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-30 06:14:29.000000 xenoslib-0.1.28.4/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 06:14:29.000000 xenoslib-0.1.28.4/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 06:47:27.000000 xenoslib-0.1.28.5/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-30 06:47:28.000000 xenoslib-0.1.28.5/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:47:27.000000 xenoslib-0.1.28.5/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-30 06:47:28.000000 xenoslib-0.1.28.5/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 06:47:28.000000 xenoslib-0.1.28.5/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.28.4/LICENSE` & `xenoslib-0.1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/README.md` & `xenoslib-0.1.28.5/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/setup.py` & `xenoslib-0.1.28.5/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/xenoslib/base.py` & `xenoslib-0.1.28.5/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/xenoslib/dev.py` & `xenoslib-0.1.28.5/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/xenoslib/extend.py` & `xenoslib-0.1.28.5/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/xenoslib/linux.py` & `xenoslib-0.1.28.5/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/xenoslib/mail.py` & `xenoslib-0.1.28.5/xenoslib/mail.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,36 +35,42 @@
 
 
 class MailFetcher:
     """
     Fetch emails from mail inbox using IMAP protocol.
     """
 
-    def __new__(cls, imap_server, mail_addr, mail_pwd, interval=30, days=1, skip_current=True):
+    def __new__(
+        cls, imap_server, mail_addr, mail_pwd, interval=30, days=1, skip_current=True, endless=True
+    ):
         self = super().__new__(cls)
         self.imap_server = imap_server
         self.mail_addr = mail_addr
         self.mail_pwd = mail_pwd
         self.days = days
 
         self.msg_ids = deque(maxlen=999)
+        if not endless:
+            skip_current = False
         if skip_current:  # mark and skip current mails
             logger.debug("Skipping existing emails...")
             mails = self.fetch_emails()
             self.msg_ids.extend(mails.keys())
-        return self.fetching(interval=interval)
+        return self.fetching(interval=interval, endless=endless)
 
-    def fetching(self, interval=30):
+    def fetching(self, interval=30, endless=True):
         """Continuously fetch emails at the specified interval."""
         logger.debug("Start checking emails...")
         while True:
             try:
                 yield from self.parse_emails(self.fetch_emails())
             except Exception as exc:
                 logger.warning(exc)
+            if not endless:
+                break
             sleep(interval)
 
     def parse_emails(self, emails):
         for msg_id, msg in emails.items():
             if msg_id in self.msg_ids:
                 continue
             body = email.message_from_bytes(msg[b"BODY[]"])
```

### Comparing `xenoslib-0.1.28.4/xenoslib/mock.py` & `xenoslib-0.1.28.5/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/xenoslib/onedrive.py` & `xenoslib-0.1.28.5/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/xenoslib/win_trayicon.py` & `xenoslib-0.1.28.5/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.4/xenoslib/windows.py` & `xenoslib-0.1.28.5/xenoslib/windows.py`

 * *Files identical despite different names*

