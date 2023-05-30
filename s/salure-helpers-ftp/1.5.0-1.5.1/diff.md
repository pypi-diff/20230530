# Comparing `tmp/salure_helpers_ftp-1.5.0.tar.gz` & `tmp/salure_helpers_ftp-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_ftp-1.5.0.tar", last modified: Tue May 30 12:06:42 2023, max compression
+gzip compressed data, was "dist/salure_helpers_ftp-1.5.1.tar", last modified: Tue May 30 13:05:06 2023, max compression
```

## Comparing `salure_helpers_ftp-1.5.0.tar` & `salure_helpers_ftp-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/salure_helpers/ftp/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-30 12:06:29.000000 salure_helpers_ftp-1.5.0/salure_helpers/ftp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10703 2023-05-30 12:06:29.000000 salure_helpers_ftp-1.5.0/salure_helpers/ftp/ftps.py
--rw-rw-rw-   0 root         (0) root         (0)     6231 2023-05-30 12:06:29.000000 salure_helpers_ftp-1.5.0/salure_helpers/ftp/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/salure_helpers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/salure_helpers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/salure_helpers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/salure_helpers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/salure_helpers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/salure_helpers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/salure_helpers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 12:06:42.000000 salure_helpers_ftp-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-05-30 12:06:29.000000 salure_helpers_ftp-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers/ftp/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-30 13:04:43.000000 salure_helpers_ftp-1.5.1/salure_helpers/ftp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2023-05-30 13:04:43.000000 salure_helpers_ftp-1.5.1/salure_helpers/ftp/ftps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6231 2023-05-30 13:04:43.000000 salure_helpers_ftp-1.5.1/salure_helpers/ftp/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/salure_helpers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 13:05:06.000000 salure_helpers_ftp-1.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-05-30 13:04:43.000000 salure_helpers_ftp-1.5.1/setup.py
```

### Comparing `salure_helpers_ftp-1.5.0/salure_helpers/ftp/ftps.py` & `salure_helpers_ftp-1.5.1/salure_helpers/ftp/ftps.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                 if file_name in ('.', '..'):
                     continue
                 try:
                     ftp.delete(file_name)  # Delete file
                 except:
                     self.remove_directory(f"{remote_directory}/{file_name}", recursive=True)  # Recursive call for subdirectories
             ftp.cwd('..')  # Move back to the parent directory
-            ftp.rmd(remote_directory)  # Remove the empty directory
+            ftp.rmd(remote_directory.split('/')[-1])  # Remove the empty directory
         else:
             ftp.rmd(remote_directory)
 
 
     @retry(stop=stop_after_attempt(5), wait=wait_exponential_jitter(initial=60, max=900), retry=retry_if_exception(is_ftp_exception), reraise=True)
     def send_command(self, command):
         """
```

### Comparing `salure_helpers_ftp-1.5.0/salure_helpers/ftp/sftp.py` & `salure_helpers_ftp-1.5.1/salure_helpers/ftp/sftp.py`

 * *Files identical despite different names*

