# Comparing `tmp/spida-0.3.tar.gz` & `tmp/spida-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spida-0.3.tar", last modified: Mon May 29 07:09:27 2023, max compression
+gzip compressed data, was "spida-0.3.1.tar", last modified: Tue May 30 17:57:31 2023, max compression
```

## Comparing `spida-0.3.tar` & `spida-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:09:27.667983 spida-0.3/
--rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.3/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6146 2023-05-29 07:09:27.667983 spida-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 07:09:27.669022 spida-0.3/setup.cfg
--rw-rw-rw-   0        0        0      777 2023-05-29 07:07:22.000000 spida-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:09:27.607968 spida-0.3/spida/
--rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.3/spida/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:09:27.640609 spida-0.3/spida/data/
--rw-rw-rw-   0        0        0        2 2023-05-28 23:00:43.000000 spida-0.3/spida/data/config.json
--rw-rw-rw-   0        0        0    17478 2023-05-29 07:05:45.000000 spida-0.3/spida/stable_diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:09:27.665726 spida-0.3/spida/utils/
--rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.3/spida/utils/__init__.py
--rw-rw-rw-   0        0        0     5913 2023-05-26 19:58:34.000000 spida-0.3/spida/utils/img.py
--rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.3/spida/utils/misc.py
--rw-rw-rw-   0        0        0     1087 2023-05-28 22:57:32.000000 spida-0.3/spida/utils/net.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:09:27.638508 spida-0.3/spida.egg-info/
--rw-rw-rw-   0        0        0     6146 2023-05-29 07:09:27.000000 spida-0.3/spida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-29 07:09:27.000000 spida-0.3/spida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:09:27.000000 spida-0.3/spida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-05-29 07:09:27.000000 spida-0.3/spida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-29 07:09:27.000000 spida-0.3/spida.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 17:57:31.917253 spida-0.3.1/
+-rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6148 2023-05-30 17:57:31.916252 spida-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 17:57:31.917253 spida-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-05-30 17:55:37.000000 spida-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:57:31.870144 spida-0.3.1/spida/
+-rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.3.1/spida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:57:31.900244 spida-0.3.1/spida/data/
+-rw-rw-rw-   0        0        0        2 2023-05-30 16:55:04.000000 spida-0.3.1/spida/data/config.json
+-rw-rw-rw-   0        0        0    18000 2023-05-30 17:54:06.000000 spida-0.3.1/spida/stable_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:57:31.914252 spida-0.3.1/spida/utils/
+-rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.3.1/spida/utils/__init__.py
+-rw-rw-rw-   0        0        0     5913 2023-05-26 19:58:34.000000 spida-0.3.1/spida/utils/img.py
+-rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.3.1/spida/utils/misc.py
+-rw-rw-rw-   0        0        0     1087 2023-05-28 22:57:32.000000 spida-0.3.1/spida/utils/net.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:57:31.898241 spida-0.3.1/spida.egg-info/
+-rw-rw-rw-   0        0        0     6148 2023-05-30 17:57:31.000000 spida-0.3.1/spida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-30 17:57:31.000000 spida-0.3.1/spida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 17:57:31.000000 spida-0.3.1/spida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-30 17:57:31.000000 spida-0.3.1/spida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 17:57:31.000000 spida-0.3.1/spida.egg-info/top_level.txt
```

### Comparing `spida-0.3/LICENSE` & `spida-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spida-0.3/PKG-INFO` & `spida-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.3
+Version: 0.3.1
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `spida-0.3/README.md` & `spida-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `spida-0.3/setup.py` & `spida-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="spida",
-    version="0.3",
+    version="0.3.1",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description="A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="h2see",
```

### Comparing `spida-0.3/spida/stable_diffusion.py` & `spida-0.3.1/spida/stable_diffusion.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,23 @@
         config["webui_startfile"] = (
             webui_startfile if webui_startfile else "webui-user.bat"
         )
         url = input(
             "\nPlease input API url\n(if ENTER defaults to http://127.0.0.1:7860)\n"
         )
         config["url"] = url if url else "http://127.0.0.1:7860"
+        use_subprocess = input(
+            "\nWould you like to start the Stable Diffusion WebUI using subprocess? [y/n]\n(if possible, ENTER defaults to n)\n"
+        )
+        config["use_subprocess"] = (
+            False
+            if (use_subprocess.lower() if use_subprocess else "n") is "n"
+            and sys.platform is "win32"
+            else True
+        )
         print()
     else:
         config.update(config_dict)
     with open(config_path, "w") as f:
         json.dump(config, f)
 
 
@@ -67,56 +76,59 @@
 # PRIMARY FUNCTIONS
 
 
 def start():
     """
     Starts the local API by running the specified start file from the configuration.
 
-    Changes the current working directory to the path specified in the configuration,
+    If not using subprocess: Changes the current working directory to the path specified in the configuration,
     starts the file specified in the configuration, and then changes back to the original directory.
 
     Returns
     -------
     None
         This function does not return a value; it initiates the local API.
     """
-    cwd = os.getcwd()
-    os.chdir(config["webui_path"])
-    if sys.platform == "win32":
-        os.startfile(config["webui_startfile"])
-    else:
+    if config["use_subprocess"]:
         global webui_process
-        webui_process = subprocess.Popen(config["webui_startfile"])
-    os.chdir(cwd)
+        webui_process = subprocess.Popen(
+            config["webui_path"] + "/" + config["webui_startfile"],
+            cwd=config["webui_path"],
+        )
+    else:
+        cwd = os.getcwd()
+        os.chdir(config["webui_path"])
+        os.startfile(config["webui_startfile"])
+        os.chdir(cwd)
 
 
 def stop(shell=False):
     """
-    Stops the local API. On Windows, kills all cmd or powershell terminals.
+    Stops the local API. If not a subprocess, kills all cmd or powershell terminals.
 
     Parameters
     ----------
     shell : bool, optional
         Whether to kill powershell terminals instead of cmd terminals, by default False.
 
     Returns
     -------
     None
         This function does not return a value; it stops the local API.
     """
-    if sys.platform == "win32":
-        if shell:
-            os.system("taskkill /f /im powershell.exe")
-        else:
-            os.system("taskkill /f /im cmd.exe")
-    else:
+    if config["use_subprocess"]:
         if webui_process is None:
             raise Exception("Could not find process id.")
         else:
             webui_process.terminate()
+    else:
+        if shell:
+            os.system("taskkill /f /im powershell.exe")
+        else:
+            os.system("taskkill /f /im cmd.exe")
 
 
 def model(name: str, search: bool = True):
     """
     Sets the Stable Diffusion (SD) model to be used.
 
     Parameters
```

### Comparing `spida-0.3/spida/utils/img.py` & `spida-0.3.1/spida/utils/img.py`

 * *Files identical despite different names*

### Comparing `spida-0.3/spida/utils/misc.py` & `spida-0.3.1/spida/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spida-0.3/spida/utils/net.py` & `spida-0.3.1/spida/utils/net.py`

 * *Files identical despite different names*

### Comparing `spida-0.3/spida.egg-info/PKG-INFO` & `spida-0.3.1/spida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.3
+Version: 0.3.1
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

