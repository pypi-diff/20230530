# Comparing `tmp/aistudio-scheduler-lock-1.0.5b1.tar.gz` & `tmp/aistudio-scheduler-lock-1.0.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistudio-scheduler-lock-1.0.5b1.tar", max compression
+gzip compressed data, was "aistudio-scheduler-lock-1.0.6a1.tar", max compression
```

## Comparing `aistudio-scheduler-lock-1.0.5b1.tar` & `aistudio-scheduler-lock-1.0.6a1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0        0 2022-09-02 06:46:57.612688 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/__init__.py
--rw-r--r--   0        0        0       63 2022-09-02 06:46:57.614636 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/admin.py
--rw-r--r--   0        0        0     2020 2023-02-08 14:36:29.540645 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/apps.py
--rw-r--r--   0        0        0      645 2023-02-21 08:25:38.221902 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/base_lock.py
--rw-r--r--   0        0        0     1078 2022-09-05 07:32:43.545338 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/database_advisory_lock.py
--rw-r--r--   0        0        0     4853 2023-02-21 08:25:47.196802 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/database_lock.py
--rw-r--r--   0        0        0     5727 2023-02-21 08:28:17.705028 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/file_lock.py
--rw-r--r--   0        0        0     1104 2023-02-09 08:31:51.309540 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/utils.py
--rw-r--r--   0        0        0      773 2022-09-02 06:46:57.623569 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-09-02 06:46:57.623676 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/migrations/__init__.py
--rw-r--r--   0        0        0     6015 2022-09-05 08:49:04.799827 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/models.py
--rw-r--r--   0        0        0    11387 2023-02-23 14:09:57.164172 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/schedules/scheduler_lock_job.py
--rw-r--r--   0        0        0     1019 2023-02-22 13:15:08.418959 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/schedules/schedules_master_base.py
--rw-r--r--   0        0        0       60 2022-09-02 06:46:57.624105 aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/tests.py
--rw-r--r--   0        0        0      435 2023-02-23 14:11:05.280937 aistudio-scheduler-lock-1.0.5b1/pyproject.toml
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 aistudio-scheduler-lock-1.0.5b1/setup.py
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 aistudio-scheduler-lock-1.0.5b1/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2022-09-02 06:46:57.612688 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/__init__.py
+-rwxr-xr-x   0        0        0       63 2022-09-02 06:46:57.614636 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/admin.py
+-rwxr-xr-x   0        0        0     2020 2023-04-10 05:49:04.342584 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/apps.py
+-rwxr-xr-x   0        0        0      645 2023-04-10 05:49:04.342910 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/base_lock.py
+-rwxr-xr-x   0        0        0     1078 2022-09-05 07:32:43.545338 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/database_advisory_lock.py
+-rwxr-xr-x   0        0        0     4853 2023-04-10 05:49:04.343353 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/database_lock.py
+-rwxr-xr-x   0        0        0     5732 2023-04-10 05:49:04.345163 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/file_lock.py
+-rwxr-xr-x   0        0        0     1104 2023-04-10 05:49:04.345653 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/utils.py
+-rwxr-xr-x   0        0        0      773 2022-09-02 06:46:57.623569 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2022-09-02 06:46:57.623676 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/migrations/__init__.py
+-rwxr-xr-x   0        0        0     6015 2022-09-05 08:49:04.799827 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/models.py
+-rwxr-xr-x   0        0        0       92 2023-04-10 05:49:04.345892 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/schedules/enums.py
+-rwxr-xr-x   0        0        0     8932 2023-04-10 05:50:54.414395 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/schedules/scheduler_lock_job.py
+-rwxr-xr-x   0        0        0     1658 2023-04-10 05:49:04.346624 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/schedules/schedules_master_base.py
+-rwxr-xr-x   0        0        0       60 2022-09-02 06:46:57.624105 aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/tests.py
+-rwxr-xr-x   0        0        0      457 2023-05-30 11:07:21.899173 aistudio-scheduler-lock-1.0.6a1/pyproject.toml
+-rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 aistudio-scheduler-lock-1.0.6a1/setup.py
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 aistudio-scheduler-lock-1.0.6a1/PKG-INFO
```

### Comparing `aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/apps.py` & `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/apps.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/base_lock.py` & `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/base_lock.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/database_advisory_lock.py` & `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/database_advisory_lock.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/database_lock.py` & `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/database_lock.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/file_lock.py` & `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/file_lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import os
 import sys
-from os.path import exists
 
 from .base_lock import DistributedLock
 from .utils import LockUtils
 
 logger = logging.getLogger(__name__)
 
 
@@ -59,15 +58,15 @@
         self.fcntl = fcntl
         self.lock_file = lock_file
         self.lock_file_fd = None
 
     def try_acquire_lock(self) -> True:
         fd = None
         try:
-            f_exists = exists(self.lock_file)
+            f_exists = os.path.exists(self.lock_file)
             open_mode = os.O_RDWR if f_exists else os.O_RDWR | os.O_CREAT
             fd = os.open(self.lock_file, open_mode, 0o600)
 
             # LOCK_EX: Place an exclusive lock. Only one process may hold an
             # exclusive lock for a given file at a given time.
             # LOCK_NB: A call to flock() may block if an incompatible lock is
             # held by another process. To make a nonblocking request, include LOCK_NB.
@@ -90,15 +89,15 @@
 
     # This method actually never gets called.
     # Lock is released only when lock owner dies, shuts down etc.
     # Also, following code is most probably buggy
     def release(self) -> None:
 
         if not self.lock_file_fd:
-            f_exists = exists(self.lock_file)
+            f_exists = os.path.exists(self.lock_file)
             open_mode = os.O_RDWR if f_exists else os.O_RDWR | os.O_CREAT
             fd = os.open(self.lock_file, open_mode, 0o600)
         else:
             fd = self.lock_file_fd
         # Do not remove the lockfile:
         #
         #   https://github.com/benediktschmitt/py-filelock/issues/31
@@ -106,15 +105,15 @@
         self.fcntl.flock(fd, self.fcntl.LOCK_UN | self.fcntl.LOCK_NB)
         os.close(fd)
 
     def renew_lease(self) -> bool:
         # We can possibly use the concept of lease here, by maintaining the
         # validity of the lock in the file. But for now, we don't.
         # We just return true if the lock file is present, else false.
-        return bool(exists(self.lock_file))
+        return bool(os.path.exists(self.lock_file))
 
     def get_current_owner(self) -> str:
-        if exists(self.lock_file):
+        if os.path.exists(self.lock_file):
             with open(self.lock_file) as f:
                 return f.read().strip()
         else:
             return "Lock file does not exist. Unable to fetch lock owner."
```

### Comparing `aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/locks/utils.py` & `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/locks/utils.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/migrations/0001_initial.py` & `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.5b1/aistudio_scheduler_lock/models.py` & `aistudio-scheduler-lock-1.0.6a1/aistudio_scheduler_lock/models.py`

 * *Files identical despite different names*

### Comparing `aistudio-scheduler-lock-1.0.5b1/setup.py` & `aistudio-scheduler-lock-1.0.6a1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,19 @@
  'aistudio_scheduler_lock.migrations',
  'aistudio_scheduler_lock.schedules']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Django==3.2.6', 'django-apscheduler==0.6.2']
+['Django==3.2.19', 'django-apscheduler==0.6.2', 'setuptools==65.5.1']
 
 setup_kwargs = {
     'name': 'aistudio-scheduler-lock',
-    'version': '1.0.5b1',
+    'version': '1.0.6a1',
     'description': 'Implements a distributed locking scheme for schedulers running on HA mode.',
     'long_description': 'None',
     'author': 'Yogesh Ketkar',
     'author_email': 'yogesh.ketkar@automationedge.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

