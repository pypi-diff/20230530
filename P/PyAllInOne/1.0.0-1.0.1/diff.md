# Comparing `tmp/PyAllInOne-1.0.0.tar.gz` & `tmp/PyAllInOne-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAllInOne-1.0.0.tar", last modified: Tue May 30 10:37:48 2023, max compression
+gzip compressed data, was "PyAllInOne-1.0.1.tar", last modified: Tue May 30 11:08:06 2023, max compression
```

## Comparing `PyAllInOne-1.0.0.tar` & `PyAllInOne-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 10:37:48.751037 PyAllInOne-1.0.0/
--rw-rw-rw-   0        0        0      613 2023-05-30 10:33:05.000000 PyAllInOne-1.0.0/CREDITS.md
--rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyAllInOne-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       94 2023-05-30 10:31:51.000000 PyAllInOne-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2874 2023-05-30 10:37:48.750040 PyAllInOne-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 10:37:48.708152 PyAllInOne-1.0.0/PyAllInOne/
-drwxrwxrwx   0        0        0        0 2023-05-30 10:37:48.738072 PyAllInOne-1.0.0/PyAllInOne/Computer/
--rw-rw-rw-   0        0        0     1194 2023-05-30 10:28:22.000000 PyAllInOne-1.0.0/PyAllInOne/Computer/Brightness.py
--rw-rw-rw-   0        0        0      462 2023-05-30 10:12:33.000000 PyAllInOne-1.0.0/PyAllInOne/Computer/System.py
--rw-rw-rw-   0        0        0     2684 2023-05-30 10:26:47.000000 PyAllInOne-1.0.0/PyAllInOne/Computer/Volume.py
--rw-rw-rw-   0        0        0       71 2023-05-30 09:49:19.000000 PyAllInOne-1.0.0/PyAllInOne/Computer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 10:37:48.741063 PyAllInOne-1.0.0/PyAllInOne/Computer/assets/
--rwxrwxrwx   0        0        0   899784 2023-05-23 02:05:42.000000 PyAllInOne-1.0.0/PyAllInOne/Computer/assets/SetVol.exe
--rw-rw-rw-   0        0        0       60 2023-05-30 09:49:01.000000 PyAllInOne-1.0.0/PyAllInOne/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 10:37:48.726103 PyAllInOne-1.0.0/PyAllInOne.egg-info/
--rw-rw-rw-   0        0        0     2874 2023-05-30 10:37:47.000000 PyAllInOne-1.0.0/PyAllInOne.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-05-30 10:37:47.000000 PyAllInOne-1.0.0/PyAllInOne.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 10:37:47.000000 PyAllInOne-1.0.0/PyAllInOne.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-30 10:37:47.000000 PyAllInOne-1.0.0/PyAllInOne.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 10:37:47.000000 PyAllInOne-1.0.0/PyAllInOne.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2027 2023-05-30 09:46:26.000000 PyAllInOne-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 10:37:48.752036 PyAllInOne-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1335 2023-05-30 09:43:50.000000 PyAllInOne-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:08:06.881664 PyAllInOne-1.0.1/
+-rw-rw-rw-   0        0        0      613 2023-05-30 10:33:05.000000 PyAllInOne-1.0.1/CREDITS.md
+-rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyAllInOne-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      127 2023-05-30 11:02:15.000000 PyAllInOne-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2874 2023-05-30 11:08:06.879665 PyAllInOne-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 11:08:06.754998 PyAllInOne-1.0.1/PyAllInOne/
+drwxrwxrwx   0        0        0        0 2023-05-30 11:08:06.791909 PyAllInOne-1.0.1/PyAllInOne/Computer/
+-rw-rw-rw-   0        0        0     1232 2023-05-30 10:57:53.000000 PyAllInOne-1.0.1/PyAllInOne/Computer/Brightness.py
+-rw-rw-rw-   0        0        0      462 2023-05-30 10:12:33.000000 PyAllInOne-1.0.1/PyAllInOne/Computer/System.py
+-rw-rw-rw-   0        0        0     2798 2023-05-30 10:58:42.000000 PyAllInOne-1.0.1/PyAllInOne/Computer/Volume.py
+-rw-rw-rw-   0        0        0       71 2023-05-30 09:49:19.000000 PyAllInOne-1.0.1/PyAllInOne/Computer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:08:06.794891 PyAllInOne-1.0.1/PyAllInOne/Computer/assets/
+-rwxrwxrwx   0        0        0   899784 2023-05-23 02:05:42.000000 PyAllInOne-1.0.1/PyAllInOne/Computer/assets/SetVol.exe
+drwxrwxrwx   0        0        0        0 2023-05-30 11:08:06.813841 PyAllInOne-1.0.1/PyAllInOne/English/
+-rw-rw-rw-   0        0        0      477 2023-05-30 11:00:13.000000 PyAllInOne-1.0.1/PyAllInOne/English/Grammar.py
+-rw-rw-rw-   0        0        0     1496 2023-05-30 11:05:49.000000 PyAllInOne-1.0.1/PyAllInOne/English/Words.py
+-rw-rw-rw-   0        0        0       70 2023-05-30 10:54:16.000000 PyAllInOne-1.0.1/PyAllInOne/English/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:08:06.817831 PyAllInOne-1.0.1/PyAllInOne/English/assets/
+-rw-rw-rw-   0        0        0 22970019 2023-05-20 13:53:02.000000 PyAllInOne-1.0.1/PyAllInOne/English/assets/dictionary.json
+-rw-rw-rw-   0        0        0       60 2023-05-30 09:49:01.000000 PyAllInOne-1.0.1/PyAllInOne/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:08:06.771954 PyAllInOne-1.0.1/PyAllInOne.egg-info/
+-rw-rw-rw-   0        0        0     2874 2023-05-30 11:08:06.000000 PyAllInOne-1.0.1/PyAllInOne.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-05-30 11:08:06.000000 PyAllInOne-1.0.1/PyAllInOne.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 11:08:06.000000 PyAllInOne-1.0.1/PyAllInOne.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-30 11:08:06.000000 PyAllInOne-1.0.1/PyAllInOne.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 11:08:06.000000 PyAllInOne-1.0.1/PyAllInOne.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2027 2023-05-30 11:06:56.000000 PyAllInOne-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 11:08:06.882664 PyAllInOne-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1335 2023-05-30 11:07:02.000000 PyAllInOne-1.0.1/setup.py
```

### Comparing `PyAllInOne-1.0.0/CREDITS.md` & `PyAllInOne-1.0.1/CREDITS.md`

 * *Files identical despite different names*

### Comparing `PyAllInOne-1.0.0/LICENSE.txt` & `PyAllInOne-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyAllInOne-1.0.0/PKG-INFO` & `PyAllInOne-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAllInOne
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyAllInOne is an advanced multi-purpose Python package.
 Home-page: https://github.com/Anikethc/PyAllInOne
 Download-URL: https://pypi.org/project/PyAllInOne
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,15 +26,15 @@
 PyAllInOne is an advanced multi-purpose Python package.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyallinone-docs).
 
 ## Package Information
 
 **Name** - PyAllInOne</br>
-**Version** - 1.0.0</br>
+**Version** - 1.0.1</br>
 **Description** - PyAllInOne is an advanced multi-purpose Python package.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyAllInOne](https://github.com/Anikethc/PyAllInOne)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyAllInOne](https://pypi.org/project/PyAllInOne)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyallinone-docs](https://aniketh-chavare.gitbook.io/pyallinone-docs)
 
 ## License
```

### Comparing `PyAllInOne-1.0.0/PyAllInOne/Computer/Brightness.py` & `PyAllInOne-1.0.1/PyAllInOne/Computer/Brightness.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     else:
         raise Exception("This function only works on Windows and Linux.")
 
 # Function 3 - Set
 def set(value):
     # Checking the OS
     if (platform.uname().system == "Windows" or platform.uname().system == "Linux"):
-        # Setting the Brightness
+        # Checking the Data Type
         if (isinstance(value, (int, float))):
+            # Setting the Brightness
             sbc.set_brightness(value)
         else:
             raise Exception("The 'value' argument must be an integer or a float.")
     else:
         raise Exception("This function only works on Windows and Linux.")
```

### Comparing `PyAllInOne-1.0.0/PyAllInOne/Computer/Volume.py` & `PyAllInOne-1.0.1/PyAllInOne/Computer/Volume.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,29 +29,31 @@
     else:
         raise Exception("This function only works on Windows.")
 
 # Function 3 - Increase
 def increase(value):
     # Checking the OS
     if (platform.uname().system == "Windows"):
-        # Setting the Volume
+        # Checking the Data Type
         if (isinstance(value, int)):
+            # Setting the Volume
             os.chdir(directory + "/assets")
             os.system("setvol +" + str(value))
         else:
             raise Exception("The 'value' argument must be an integer.")
     else:
         raise Exception("This function only works on Windows.")
 
 # Function 4 - Decrease
 def decrease(value):
     # Checking the OS
     if (platform.uname().system == "Windows"):
-        # Setting the Volume
+        # Checking the Data Type
         if (isinstance(value, int)):
+            # Setting the Volume
             os.chdir(directory + "/assets")
             os.system("setvol -" + str(value))
         else:
             raise Exception("The 'value' argument must be an integer.")
     else:
         raise Exception("This function only works on Windows.")
 
@@ -75,15 +77,16 @@
     else:
         raise Exception("This function only works on Windows.")
 
 # Function 7 - Set
 def set(value):
     # Checking the OS
     if (platform.uname().system == "Windows"):
-        # Setting the Volume
+        # Checking the Data Type
         if (isinstance(value, int)):
+            # Setting the Volume
             os.chdir(directory + "/assets")
             os.system("setvol " + str(value))
         else:
             raise Exception("The 'value' argument must be an integer.")
     else:
         raise Exception("This function only works on Windows.")
```

### Comparing `PyAllInOne-1.0.0/PyAllInOne/Computer/assets/SetVol.exe` & `PyAllInOne-1.0.1/PyAllInOne/Computer/assets/SetVol.exe`

 * *Files identical despite different names*

### Comparing `PyAllInOne-1.0.0/PyAllInOne.egg-info/PKG-INFO` & `PyAllInOne-1.0.1/PyAllInOne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAllInOne
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyAllInOne is an advanced multi-purpose Python package.
 Home-page: https://github.com/Anikethc/PyAllInOne
 Download-URL: https://pypi.org/project/PyAllInOne
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,15 +26,15 @@
 PyAllInOne is an advanced multi-purpose Python package.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyallinone-docs).
 
 ## Package Information
 
 **Name** - PyAllInOne</br>
-**Version** - 1.0.0</br>
+**Version** - 1.0.1</br>
 **Description** - PyAllInOne is an advanced multi-purpose Python package.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyAllInOne](https://github.com/Anikethc/PyAllInOne)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyAllInOne](https://pypi.org/project/PyAllInOne)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyallinone-docs](https://aniketh-chavare.gitbook.io/pyallinone-docs)
 
 ## License
```

### Comparing `PyAllInOne-1.0.0/README.md` & `PyAllInOne-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PyAllInOne is an advanced multi-purpose Python package.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyallinone-docs).
 
 ## Package Information
 
 **Name** - PyAllInOne</br>
-**Version** - 1.0.0</br>
+**Version** - 1.0.1</br>
 **Description** - PyAllInOne is an advanced multi-purpose Python package.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyAllInOne](https://github.com/Anikethc/PyAllInOne)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyAllInOne](https://pypi.org/project/PyAllInOne)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyallinone-docs](https://aniketh-chavare.gitbook.io/pyallinone-docs)
 
 ## License
```

### Comparing `PyAllInOne-1.0.0/setup.py` & `PyAllInOne-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguments
 setup_args = dict (
     name = "PyAllInOne",
-    version = "1.0.0",
+    version = "1.0.1",
     description = "PyAllInOne is an advanced multi-purpose Python package.",
     long_description = README,
     long_description_content_type = "text/markdown",
     license = "MIT",
     packages = find_packages(),
     include_package_data = True,
     author = "Aniketh Chavare",
```

