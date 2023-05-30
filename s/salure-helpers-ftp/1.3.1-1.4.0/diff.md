# Comparing `tmp/salure_helpers_ftp-1.3.1.tar.gz` & `tmp/salure_helpers_ftp-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_ftp-1.3.1.tar", last modified: Wed May 24 09:28:00 2023, max compression
+gzip compressed data, was "dist/salure_helpers_ftp-1.4.0.tar", last modified: Tue May 30 11:08:59 2023, max compression
```

## Comparing `salure_helpers_ftp-1.3.1.tar` & `salure_helpers_ftp-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/salure_helpers/ftp/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-24 09:27:45.000000 salure_helpers_ftp-1.3.1/salure_helpers/ftp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9010 2023-05-24 09:27:45.000000 salure_helpers_ftp-1.3.1/salure_helpers/ftp/ftps.py
--rw-rw-rw-   0 root         (0) root         (0)     6231 2023-05-24 09:27:45.000000 salure_helpers_ftp-1.3.1/salure_helpers/ftp/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/salure_helpers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/salure_helpers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/salure_helpers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/salure_helpers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/salure_helpers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/salure_helpers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/salure_helpers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 09:28:00.000000 salure_helpers_ftp-1.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-05-24 09:27:45.000000 salure_helpers_ftp-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/salure_helpers/ftp/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-30 11:08:44.000000 salure_helpers_ftp-1.4.0/salure_helpers/ftp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-05-30 11:08:44.000000 salure_helpers_ftp-1.4.0/salure_helpers/ftp/ftps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6231 2023-05-30 11:08:44.000000 salure_helpers_ftp-1.4.0/salure_helpers/ftp/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/salure_helpers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/salure_helpers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/salure_helpers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/salure_helpers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/salure_helpers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/salure_helpers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/salure_helpers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 11:08:58.000000 salure_helpers_ftp-1.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-05-30 11:08:44.000000 salure_helpers_ftp-1.4.0/setup.py
```

### Comparing `salure_helpers_ftp-1.3.1/salure_helpers/ftp/ftps.py` & `salure_helpers_ftp-1.4.0/salure_helpers/ftp/ftps.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,7 +177,26 @@
     def remove_file(self, remote_filepath):
         """
         Remove a file on a remote location
         :param remote_file: the full path of the file that needs to be removed
         """
         with FTP(host=self.host, user=self.username, passwd=self.password) as ftp:
             ftp.delete(remote_filepath)
+
+    def remove_directory(self, remote_directory):
+        """
+        Remove a file on a remote location
+        :param remote_directory: the directory you want to remove
+        """
+        with FTP(host=self.host, user=self.username, passwd=self.password) as ftp:
+            ftp.rmd(remote_directory)
+
+    def send_command(self, command):
+        """
+        Send a command to the ftp server
+        :param command: the command that needs to be send
+        :return: the response of the server
+        """
+        with FTP(host=self.host, user=self.username, passwd=self.password) as ftp:
+            response = ftp.sendcmd(command)
+            return response
+
```

### Comparing `salure_helpers_ftp-1.3.1/salure_helpers/ftp/sftp.py` & `salure_helpers_ftp-1.4.0/salure_helpers/ftp/sftp.py`

 * *Files identical despite different names*

