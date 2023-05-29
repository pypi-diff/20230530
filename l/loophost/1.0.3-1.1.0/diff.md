# Comparing `tmp/loophost-1.0.3.tar.gz` & `tmp/loophost-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loophost-1.0.3.tar", max compression
+gzip compressed data, was "loophost-1.1.0.tar", max compression
```

## Comparing `loophost-1.0.3.tar` & `loophost-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,30 @@
--rw-r--r--   0        0        0       68 2023-05-29 22:11:50.211357 loophost-1.0.3/README.md
--rw-r--r--   0        0        0        5 2023-05-29 22:11:50.211357 loophost-1.0.3/VERSION
--rw-r--r--   0        0        0      670 2023-05-29 22:11:50.211357 loophost-1.0.3/build.py
--rw-r--r--   0        0        0      925 2023-05-29 22:11:50.211357 loophost-1.0.3/loophost/__init__.py
--rw-r--r--   0        0        0     4401 2023-05-29 22:11:50.211357 loophost-1.0.3/loophost/flingroute.py
--rw-r--r--   0        0        0     3452 2023-05-29 22:11:50.211357 loophost-1.0.3/loophost/installer.py
--rw-r--r--   0        0        0     1353 2023-05-29 22:11:50.211357 loophost-1.0.3/loophost/launchd_plist.py
--rwxr-xr-x   0        0        0  8045762 2023-05-29 22:11:50.263357 loophost-1.0.3/loophost/loopproxy
--rw-r--r--   0        0        0  8751616 2023-05-29 22:11:50.319356 loophost-1.0.3/loophost/loopproxy.exe
--rw-r--r--   0        0        0      783 2023-05-29 22:11:50.319356 loophost-1.0.3/loophost/plist/hub.plist.template
--rw-r--r--   0        0        0      771 2023-05-29 22:11:50.319356 loophost-1.0.3/loophost/plist/loophost.plist.template
--rw-r--r--   0        0        0     1150 2023-05-29 22:11:50.319356 loophost-1.0.3/loophost/plist/ssh.plist.template
--rw-r--r--   0        0        0      100 2023-05-29 22:11:50.319356 loophost-1.0.3/loophost/postinstall.py
--rw-r--r--   0        0        0    95159 2023-05-29 22:11:50.319356 loophost-1.0.3/loophost/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/static/fling-logo-light.png
--rw-r--r--   0        0        0     6393 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/static/github-mark.png
--rw-r--r--   0        0        0     3834 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/static/logo-hc.txt
--rw-r--r--   0        0        0    34153 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/static/logo-square.png
--rw-r--r--   0        0        0      457 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/step_two.py
--rw-r--r--   0        0        0      828 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/templates/admin.html
--rw-r--r--   0        0        0     1657 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/templates/base.html
--rw-r--r--   0        0        0     2921 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/templates/local.html
--rw-r--r--   0        0        0     1478 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/templates/partials/apptable.html
--rw-r--r--   0        0        0      289 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1730 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/templates/start/base.html
--rw-r--r--   0        0        0     1656 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/uninstall.py
--rw-r--r--   0        0        0      517 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/win/build.txt
--rw-r--r--   0        0        0     2431 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/win_hub.py
--rw-r--r--   0        0        0     2579 2023-05-29 22:11:50.323356 loophost-1.0.3/loophost/win_lp.py
--rw-r--r--   0        0        0     1274 2023-05-29 22:11:50.323356 loophost-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-29 22:11:50.323356 loophost-1.0.3/setup.py
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 loophost-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-05-29 23:50:14.168206 loophost-1.1.0/README.md
+-rw-r--r--   0        0        0        5 2023-05-29 23:50:14.168206 loophost-1.1.0/VERSION
+-rw-r--r--   0        0        0      670 2023-05-29 23:50:14.168206 loophost-1.1.0/build.py
+-rw-r--r--   0        0        0      925 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/__init__.py
+-rw-r--r--   0        0        0     4401 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/flingroute.py
+-rw-r--r--   0        0        0     3452 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/installer.py
+-rw-r--r--   0        0        0     1353 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/launchd_plist.py
+-rw-r--r--   0        0        0      787 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/plist/hub.plist.template
+-rw-r--r--   0        0        0      771 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/plist/loophost.plist.template
+-rw-r--r--   0        0        0     1150 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/plist/ssh.plist.template
+-rw-r--r--   0        0        0      100 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-05-29 23:50:14.168206 loophost-1.1.0/loophost/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/static/fling-logo-light.png
+-rw-r--r--   0        0        0     6393 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/static/github-mark.png
+-rw-r--r--   0        0        0     3834 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/static/logo-hc.txt
+-rw-r--r--   0        0        0    34153 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/static/logo-square.png
+-rw-r--r--   0        0        0      457 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/step_two.py
+-rw-r--r--   0        0        0      828 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/admin.html
+-rw-r--r--   0        0        0     1657 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/base.html
+-rw-r--r--   0        0        0     2921 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/local.html
+-rw-r--r--   0        0        0     1478 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/partials/apptable.html
+-rw-r--r--   0        0        0      289 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1730 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/templates/start/base.html
+-rw-r--r--   0        0        0     1656 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/uninstall.py
+-rw-r--r--   0        0        0      517 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/win/build.txt
+-rw-r--r--   0        0        0     2431 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/win_hub.py
+-rw-r--r--   0        0        0     2584 2023-05-29 23:50:14.172206 loophost-1.1.0/loophost/win_lp.py
+-rw-r--r--   0        0        0     1181 2023-05-29 23:50:14.176206 loophost-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-29 23:50:14.176206 loophost-1.1.0/setup.py
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 loophost-1.1.0/PKG-INFO
```

### Comparing `loophost-1.0.3/build.py` & `loophost-1.1.0/build.py`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/__init__.py` & `loophost-1.1.0/loophost/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.3"
+__version__ = "1.1.0"
 
 import os
 import pathlib
 import platform
 import sys
```

### Comparing `loophost-1.0.3/loophost/flingroute.py` & `loophost-1.1.0/loophost/flingroute.py`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/installer.py` & `loophost-1.1.0/loophost/installer.py`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/launchd_plist.py` & `loophost-1.1.0/loophost/launchd_plist.py`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/plist/hub.plist.template` & `loophost-1.1.0/loophost/plist/hub.plist.template`

 * *Files 12% similar despite different names*

#### Comparing `loophost-1.0.3/loophost/plist/hub.plist.template` & `loophost-1.1.0/loophost/plist/hub.plist.template`

```diff
@@ -4,15 +4,15 @@
   'http://www.apple.com/DTDs/PropertyList-1.0.dtd'>
 <plist version="1.0">
   <dict>
     <key>Label</key>
     <string>dev.fling.hub</string>
     <key>ProgramArguments</key>
     <array>
-      <string>${HUBDIR}/loopproxy</string>
+      <string>${HUBDIR}/bin/loopproxy</string>
       <string>${CWD}</string>
     </array>
     <key>RunAtLoad</key>
     <true/>
     <key>KeepAlive</key>
     <true/>
     <key>WorkingDirectory</key>
```

### Comparing `loophost-1.0.3/loophost/plist/loophost.plist.template` & `loophost-1.1.0/loophost/plist/loophost.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/plist/ssh.plist.template` & `loophost-1.1.0/loophost/plist/ssh.plist.template`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/static/fling-logo-dark.png` & `loophost-1.1.0/loophost/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/static/fling-logo-light.png` & `loophost-1.1.0/loophost/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/static/github-mark.png` & `loophost-1.1.0/loophost/static/github-mark.png`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/static/logo-hc.txt` & `loophost-1.1.0/loophost/static/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/static/logo-square.png` & `loophost-1.1.0/loophost/static/logo-square.png`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/templates/admin.html` & `loophost-1.1.0/loophost/templates/admin.html`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/templates/base.html` & `loophost-1.1.0/loophost/templates/base.html`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/templates/local.html` & `loophost-1.1.0/loophost/templates/local.html`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
           For example, /tmp/myapp.soc.</p><br/>
   </div>     
 <div>
 
 {% if project in apps %} 
 <div class="row">
   <div class="col col-lg-7">
-<a class="btn btn-primary"  onclick="action_submit('share')" href="#">{% if project in share %}Disable public sharing{% else %}Enable public shaing{% endif %}</a>
+<a class="btn btn-primary" onclick="action_submit('share')" href="#">{% if project in share %}Disable public sharing{% else %}Enable public sharing{% endif %}</a>
 </div>
   <div class="col">
     <p>Public sharing will open up a remote tunnel that allows other people in the world to visit your application, at a dedicated address.</p>
   </div>
 </div>
 
 <div class="row pb-3">
```

#### html2text {}

```diff
@@ -14,16 +14,16 @@
 Your application can run on a local network port, or a unix domain socket.
 If it's running on a network port, make sure the address above starts with the
 full http://localhost, for example http://localhost:8000.
 If you're using a unix socket (which is much faster), use the full path to the
 socket (including a starting /). For example, /tmp/myapp.soc.
 
 {% if project in apps %}
-{%_if_project_in_share_%}Disable_public_sharing{%_else_%}Enable_public_shaing{%
-endif_%}
+{%_if_project_in_share_%}Disable_public_sharing{%_else_%}Enable_public_sharing
+{%_endif_%}
 Public sharing will open up a remote tunnel that allows other people in the
 world to visit your application, at a dedicated address.
 Unbind_this_project
 This will remove this app from loophost entirely, and disconnect any shared
 tunnels as well.
 *** <-_Back_to_application_list ***
 {% endif %}
```

### Comparing `loophost-1.0.3/loophost/templates/partials/apptable.html` & `loophost-1.1.0/loophost/templates/partials/apptable.html`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/templates/start/base.html` & `loophost-1.1.0/loophost/templates/start/base.html`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/uninstall.py` & `loophost-1.1.0/loophost/uninstall.py`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/win/build.txt` & `loophost-1.1.0/loophost/win/build.txt`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/win_hub.py` & `loophost-1.1.0/loophost/win_hub.py`

 * *Files identical despite different names*

### Comparing `loophost-1.0.3/loophost/win_lp.py` & `loophost-1.1.0/loophost/win_lp.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         # Following Lines are written so that, the program doesn't get quit
         # Will Run a Endless While Loop till Stop signal is not received from Windows Service API
         while not self.quitEvent.isSet():  # If stop signal is triggered, exit
             time.sleep(1)
 
     def start_flask(self):
-        cmd = "loopproxy.exe /Users/Public/.loophost"
+        cmd = "bin\\loopproxy.exe /Users/Public/.loophost"
         run(
             cmd,
             shell=True,
             # stdout=subprocess.PIPE,
             # stderr=subprocess.PIPE,
             # stdin=subprocess.PIPE,
             cwd=HUBDIR,
```

### Comparing `loophost-1.0.3/pyproject.toml` & `loophost-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [build-system]
-requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel", "setuptools-cpp", "setuptools-golang"]
+requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "loophost"
-version = "1.0.3"
+version = "1.1.0"
 description = "Loophost: for a better local dev"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 include = [{ path = "VERSION" }, 
             { path = "README.md" }, 
             { path = "setup.py" }, 
             { path = "build.py" }, 
+            { path = "loophost/bin" }, 
             { path = "loophost/templates" }, 
             { path = "loophost/static" }, 
-            { path = "loophost/loopproxy"}, 
-            { path = "loophost/loopproxy.exe"}, 
             { path = "loophost/plist/*.plist.template"}] 
 packages = [
     { include = "loophost", format = ["wheel"] },
 ]
 build = "build.py"
 
 [tool.poetry.urls]
```

### Comparing `loophost-1.0.3/PKG-INFO` & `loophost-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loophost
-Version: 1.0.3
+Version: 1.1.0
 Summary: Loophost: for a better local dev
 License: Apache-2.0
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

