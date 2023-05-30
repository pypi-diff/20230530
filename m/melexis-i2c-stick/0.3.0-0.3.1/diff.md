# Comparing `tmp/melexis-i2c-stick-0.3.0.tar.gz` & `tmp/melexis-i2c-stick-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melexis-i2c-stick-0.3.0.tar", last modified: Wed May 24 20:25:48 2023, max compression
+gzip compressed data, was "melexis-i2c-stick-0.3.1.tar", last modified: Tue May 30 21:52:44 2023, max compression
```

## Comparing `melexis-i2c-stick-0.3.0.tar` & `melexis-i2c-stick-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:48.948268 melexis-i2c-stick-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-24 20:25:48.944268 melexis-i2c-stick-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:48.940268 melexis-i2c-stick-0.3.0/melexis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:48.944268 melexis-i2c-stick-0.3.0/melexis/i2c_stick/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/melexis/i2c_stick/I2CStick.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/melexis/i2c_stick/MemoryFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/melexis/i2c_stick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/melexis/i2c_stick/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:48.944268 melexis-i2c-stick-0.3.0/melexis_i2c_stick.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-24 20:25:48.000000 melexis-i2c-stick-0.3.0/melexis_i2c_stick.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-24 20:25:48.000000 melexis-i2c-stick-0.3.0/melexis_i2c_stick.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:25:48.000000 melexis-i2c-stick-0.3.0/melexis_i2c_stick.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 20:25:48.000000 melexis-i2c-stick-0.3.0/melexis_i2c_stick.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:25:48.000000 melexis-i2c-stick-0.3.0/melexis_i2c_stick.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 20:25:48.000000 melexis-i2c-stick-0.3.0/melexis_i2c_stick.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-24 20:25:33.000000 melexis-i2c-stick-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:25:48.948268 melexis-i2c-stick-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/melexis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/melexis/i2c_stick/
+-rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/melexis/i2c_stick/I2CStick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/melexis/i2c_stick/MemoryFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/melexis/i2c_stick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/melexis/i2c_stick/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 21:52:44.000000 melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-30 21:52:24.000000 melexis-i2c-stick-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:52:44.315754 melexis-i2c-stick-0.3.1/setup.cfg
```

### Comparing `melexis-i2c-stick-0.3.0/CONTRIBUTING.md` & `melexis-i2c-stick-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.3.0/LICENSE` & `melexis-i2c-stick-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.3.0/PKG-INFO` & `melexis-i2c-stick-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.3.0
+Version: 0.3.1
 Summary: Melexis I2C Stick, python interface
 Author-email: Karel Vanroye <kva@melexis.com>
 License:    Copyright 2023 Melexis
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
```

### Comparing `melexis-i2c-stick-0.3.0/melexis/i2c_stick/I2CStick.py` & `melexis-i2c-stick-0.3.1/melexis/i2c_stick/I2CStick.py`

 * *Files 15% similar despite different names*

```diff
@@ -258,32 +258,80 @@
             if a[0] != "cs":
                 self.ser.timeout = timeout_old
                 return None
             if a[1] != "{:02X}".format(sa):
                 self.ser.timeout = timeout_old
                 return None
             if a[2] == "RO":
-                if 'RO' not in result.keys():
+                if 'read_only' not in result.keys():
                     result['read_only'] = {}
                 a = a[3].split("=")
-                result['read_only'][a[0]] = a[1]
+                value = a[1].split(",")
+                for i, v in enumerate(value):
+                    regex = r"(?P<value>[^\s\(\)]+)(?:\((?P<description>\S+)\))?"
+                    new_value = re.match(regex, v).groupdict()
+                    if (new_value['value'][:1].isdigit() or new_value['value'][:1] == '-') & (a[0] != 'SA'):
+                        try:
+                            new_value['value'] = int(new_value['value'])
+                        except:
+                            try:
+                                new_value['value'] = float(new_value['value'])
+                            except:
+                                None
+                            None
+                    if new_value['description'] is not None:
+                        value[i] = new_value
+                    else:
+                        value[i] = new_value['value']
+                if (len(value) == 1):
+                    value = value[0]
+                result['read_only'][a[0]] = value
             else:
                 a = a[2].split("=")
-                result[a[0]] = a[1]
+                value = a[1].split(",")
+                for i, v in enumerate(value):
+                    regex = r"(?P<value>[^\s\(\)]+)(?:\((?P<description>\S+)\))?"
+                    new_value = re.match(regex, v).groupdict()
+                    if (new_value['value'][:1].isdigit() or new_value['value'][:1] == '-') & (a[0] != 'SA'):
+                        try:
+                            new_value['value'] = int(new_value['value'])
+                        except:
+                            try:
+                                new_value['value'] = float(new_value['value'])
+                            except:
+                                None
+                            None
+                    if new_value['description'] is not None:
+                        value[i] = new_value
+                    else:
+                        value[i] = new_value['value']
+                if (len(value) == 1):
+                    value = value[0]
+                result[a[0]] = value
             start = time.time()
             a = self.ser.readline().decode('utf-8').rstrip()   # read a '\n' terminated line
             t = time.time() - start
 
         self.ser.timeout = timeout_old
 
         return result
 
 
-    def cs_write(self, sa):
-        return None
+    def cs_write(self, sa, item, value):
+        a = self.run_cmd("+cs:{:02X}:{}={}".format(sa, item, value))
+        a = a.split(":")
+        # +cs:3A:MEAS_SELECT=OK [host&mlx-register]'
+        # '+cs:3A:FAIL; unknown variable'
+        if a[0] != "+cs":
+            return None
+        if a[1] != "{:02X}".format(sa):
+            return None
+        if a[2].startswith("FAIL"):
+            return a[2]
+        return a[2]
 
 
     def nd(self, sa):
         a = self.run_cmd("nd:{:02X}".format(sa))
         a = a.split(":")
         if a[0] != "nd":
             return None
@@ -356,15 +404,17 @@
         if a[0] != "raw":
             return None
         if a[1] != "{:02X}".format(sa):
             return None
         if a[2] == "FAIL":
             return "FAIL:" + a[3]
         result = {}
-        result['values'] = [int(x, 16) for x in a[2].split(',')]
+        result = {}
+        result['time_ms'] = int(a[2])
+        result['values'] = [int(x, 16) for x in a[3].split(',')]
         return result
 
 
     def pwm(self, pin, pwm):
         a = self.run_cmd("pwm:{}:{}".format(pin, pwm))
         return a
```

### Comparing `melexis-i2c-stick-0.3.0/melexis/i2c_stick/MemoryFile.py` & `melexis-i2c-stick-0.3.1/melexis/i2c_stick/MemoryFile.py`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.3.0/melexis_i2c_stick.egg-info/PKG-INFO` & `melexis-i2c-stick-0.3.1/melexis_i2c_stick.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.3.0
+Version: 0.3.1
 Summary: Melexis I2C Stick, python interface
 Author-email: Karel Vanroye <kva@melexis.com>
 License:    Copyright 2023 Melexis
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
```

### Comparing `melexis-i2c-stick-0.3.0/pyproject.toml` & `melexis-i2c-stick-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=63.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "melexis-i2c-stick"
-version = "0.3.0"
+version = "0.3.1"
 description = "Melexis I2C Stick, python interface"
 readme = "README.md"
 authors = [{ name = "Karel Vanroye", email = "kva@melexis.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -32,15 +32,15 @@
 Homepage = "https://github.com/melexis/i2c-stick"
 
 [project.scripts]
 melexis_i2c_stick = "melexis.i2c_stick.__main__:main"
 
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

