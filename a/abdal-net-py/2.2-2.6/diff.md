# Comparing `tmp/abdal_net_py-2.2.tar.gz` & `tmp/abdal_net_py-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abdal_net_py-2.2.tar", last modified: Sat Feb 19 15:43:47 2022, max compression
+gzip compressed data, was "abdal_net_py-2.6.tar", last modified: Mon May 29 22:47:19 2023, max compression
```

## Comparing `abdal_net_py-2.2.tar` & `abdal_net_py-2.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-02-19 15:43:47.248377 abdal_net_py-2.2/
--rw-rw-rw-   0        0        0     1098 2022-02-19 05:32:22.000000 abdal_net_py-2.2/LICENSE
--rw-rw-rw-   0        0        0     2510 2022-02-19 15:43:47.248377 abdal_net_py-2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1485 2022-02-19 15:43:02.000000 abdal_net_py-2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-02-19 15:43:47.221378 abdal_net_py-2.2/abdal_net_py/
--rw-rw-rw-   0        0        0      145 2022-02-19 14:51:02.000000 abdal_net_py-2.2/abdal_net_py/__init__.py
--rw-rw-rw-   0        0        0      531 2022-02-19 14:47:23.000000 abdal_net_py-2.2/abdal_net_py/abdal_net_py_about.py
--rw-rw-rw-   0        0        0      951 2022-02-19 15:10:13.000000 abdal_net_py-2.2/abdal_net_py/abdal_net_py_generator.py
--rw-rw-rw-   0        0        0     1340 2022-02-19 15:41:57.000000 abdal_net_py-2.2/abdal_net_py/abdal_net_py_loger.py
--rw-rw-rw-   0        0        0     1150 2022-02-19 14:28:17.000000 abdal_net_py-2.2/abdal_net_py/abdal_net_py_unit.py
-drwxrwxrwx   0        0        0        0 2022-02-19 15:43:47.245378 abdal_net_py-2.2/abdal_net_py.egg-info/
--rw-rw-rw-   0        0        0     2510 2022-02-19 15:43:46.000000 abdal_net_py-2.2/abdal_net_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2022-02-19 15:43:47.000000 abdal_net_py-2.2/abdal_net_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-19 15:43:46.000000 abdal_net_py-2.2/abdal_net_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-02-19 15:43:47.000000 abdal_net_py-2.2/abdal_net_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-02-19 15:43:47.000000 abdal_net_py-2.2/abdal_net_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2022-02-18 21:33:53.000000 abdal_net_py-2.2/pyproject.toml
--rw-rw-rw-   0        0        0      140 2022-02-19 15:43:47.252378 abdal_net_py-2.2/setup.cfg
--rw-rw-rw-   0        0        0     1469 2022-02-19 15:42:33.000000 abdal_net_py-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 22:47:19.728202 abdal_net_py-2.6/
+-rw-rw-rw-   0        0        0     1098 2023-05-29 20:51:23.000000 abdal_net_py-2.6/LICENSE
+-rw-rw-rw-   0        0        0     2572 2023-05-29 22:47:19.728202 abdal_net_py-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-05-29 22:02:04.000000 abdal_net_py-2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 22:47:19.711191 abdal_net_py-2.6/abdal_net_py/
+-rw-rw-rw-   0        0        0      145 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/__init__.py
+-rw-rw-rw-   0        0        0      531 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_about.py
+-rw-rw-rw-   0        0        0      661 2023-05-29 21:39:00.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_admin.py
+-rw-rw-rw-   0        0        0      951 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_generator.py
+-rw-rw-rw-   0        0        0     1340 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_loger.py
+-rw-rw-rw-   0        0        0     1150 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_unit.py
+drwxrwxrwx   0        0        0        0 2023-05-29 22:47:19.725199 abdal_net_py-2.6/abdal_net_py.egg-info/
+-rw-rw-rw-   0        0        0     2572 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-05-29 20:51:23.000000 abdal_net_py-2.6/pyproject.toml
+-rw-rw-rw-   0        0        0      140 2023-05-29 22:47:19.730191 abdal_net_py-2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1469 2023-05-29 22:06:17.000000 abdal_net_py-2.6/setup.py
```

### Comparing `abdal_net_py-2.2/LICENSE` & `abdal_net_py-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.2/PKG-INFO` & `abdal_net_py-2.6/abdal_net_py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abdal_net_py
-Version: 2.2
+Name: abdal-net-py
+Version: 2.6
 Summary: Powerful security network package
 Home-page: https://github.com/abdal-security-group/abdal-net-py
 Author: Ebrahim Shafiei (EbraSha)
 Author-email: Prof.Shafiei@Gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/abdal-security-group/abdal-net-py/issues
 Keywords: python,security,hack,network,camera stream,sockets
@@ -18,80 +18,86 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# Abdal Net Py
-
-
-## Made For
-
-
-
-Powerful security network package for hackers and all security experts
-
-
-
-**Requires Lib**
-> hurry.filesize - psutil
-
-
-**Requires python**
-> Python >= 3.9
-
-
-
-## Features
-
-
-- calculate internet speed with unit
-- calculate byte to other unit (show in xbit vs xbyte )
-- Convert byte to other unit by select unit
-- multi password generator 
-- log writer + logging ram and cpu usage
-- iranian mobile phone generate
-- 
-
-**How To install**
-
-```py
-pip install abdal-net-py
-```
-
-**How To use**
-
-```py
-import abdal_net_py
-```
-
-
-## ❤️ Donation
-> Donate link: https://donate.abdalagency.ir/
-
-
-## Reporting Issues 
-
-If you are facing a configuration issue or something is not working as you expected to be, please use the **Abdal.Group@Gmail.Com** or **Prof.Shafiei@Gmail.com** . Issues on GitLab are also welcomed.
-
-
-
-
-### About Programmer
-Ebrahim Shafiei (EbraSha) (Ready to cooperate with international projects)
-- Email : Prof.Shafiei@Gmail.com
-
-
-## License
-Abdal Net Py is open-source software licensed under the [MIT license.](https://choosealicense.com/licenses/mit/)
-
-
-## ⚠️ Legal disclaimer ⚠️
-
-Usage of Abdal Net Py for Spying targets without prior mutual consent is illegal. It's the end user's responsibility to obey all applicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program.
-
-
-
-
+# Abdal Net Py
+
+
+## Made For
+
+
+
+Powerful security network package for hackers and all security experts
+
+
+
+**Requires Lib**
+> hurry.filesize - psutil
+
+
+**Requires python**
+> Python >= 3.9
+
+
+
+## Features
+
+
+- calculate internet speed with unit
+- calculate byte to other unit (show in xbit vs xbyte )
+- Convert byte to other unit by select unit
+- multi password generator 
+- log writer + logging ram and cpu usage
+- iranian mobile phone generate
+- 
+
+**How To install**
+
+```py
+pip install abdal-net-py
+```
+
+**How To use**
+
+```py
+import abdal_net_py
+```
+
+
+## ❤️ Donation
+
+> USDT:      TXLasexoQTjKMoWarikkfYRYWWXtbaVadB
+
+> BTC :   bc1q9w9ymgz2wluax60rsuza4q0at7gpy82g8el6zj
+
+> ETH :   0x402b9f67091Af07224286F16d7377bc50268Db94
+
+> For Iranian People -> MellatBank : 6104-3378-5301-4247
+
+## 🤵 Programmer
+Ebrahim Shafiei (EbraSha)
+
+E-Mail = Prof.Shafiei@Gmail.com
+
+Telegram: https://t.me/ProfShafiei
+
+
+## License
+Abdal Net Py is open-source software licensed under the [MIT license.](https://choosealicense.com/licenses/mit/)
+
+
+## ☠️ Reporting Issues
+
+If you are facing a configuration issue or something is not working as you expected to be, please use the **Prof.Shafiei@Gmail.com** . Issues on GitLab are also welcomed.
+
+## ⚠️ Legal disclaimer ⚠️
+
+Usage of Abdal Net Py for Spying targets without prior mutual consent is illegal. It's the end user's responsibility to obey all applicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program.
+
+
+
+
```

### Comparing `abdal_net_py-2.2/README.md` & `abdal_net_py-2.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: abdal_net_py
+Version: 2.6
+Summary: Powerful security network package
+Home-page: https://github.com/abdal-security-group/abdal-net-py
+Author: Ebrahim Shafiei (EbraSha)
+Author-email: Prof.Shafiei@Gmail.com
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/abdal-security-group/abdal-net-py/issues
+Keywords: python,security,hack,network,camera stream,sockets
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # Abdal Net Py
 
 
 ## Made For
 
 
 
@@ -39,33 +63,41 @@
 
 ```py
 import abdal_net_py
 ```
 
 
 ## ❤️ Donation
-> Donate link: https://donate.abdalagency.ir/
 
+> USDT:      TXLasexoQTjKMoWarikkfYRYWWXtbaVadB
 
-## Reporting Issues 
+> BTC :   bc1q9w9ymgz2wluax60rsuza4q0at7gpy82g8el6zj
 
-If you are facing a configuration issue or something is not working as you expected to be, please use the **Abdal.Group@Gmail.Com** or **Prof.Shafiei@Gmail.com** . Issues on GitLab are also welcomed.
+> ETH :   0x402b9f67091Af07224286F16d7377bc50268Db94
 
+> For Iranian People -> MellatBank : 6104-3378-5301-4247
 
+## 🤵 Programmer
+Ebrahim Shafiei (EbraSha)
 
+E-Mail = Prof.Shafiei@Gmail.com
 
-### About Programmer
-Ebrahim Shafiei (EbraSha) (Ready to cooperate with international projects)
-- Email : Prof.Shafiei@Gmail.com
+Telegram: https://t.me/ProfShafiei
 
 
 ## License
 Abdal Net Py is open-source software licensed under the [MIT license.](https://choosealicense.com/licenses/mit/)
 
 
+## ☠️ Reporting Issues
+
+If you are facing a configuration issue or something is not working as you expected to be, please use the **Prof.Shafiei@Gmail.com** . Issues on GitLab are also welcomed.
+
 ## ⚠️ Legal disclaimer ⚠️
 
 Usage of Abdal Net Py for Spying targets without prior mutual consent is illegal. It's the end user's responsibility to obey all applicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program.
 
 
 
 
+
+
```

### Comparing `abdal_net_py-2.2/abdal_net_py/abdal_net_py_about.py` & `abdal_net_py-2.6/abdal_net_py/abdal_net_py_about.py`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.2/abdal_net_py/abdal_net_py_generator.py` & `abdal_net_py-2.6/abdal_net_py/abdal_net_py_generator.py`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.2/abdal_net_py/abdal_net_py_loger.py` & `abdal_net_py-2.6/abdal_net_py/abdal_net_py_loger.py`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.2/abdal_net_py/abdal_net_py_unit.py` & `abdal_net_py-2.6/abdal_net_py/abdal_net_py_unit.py`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.2/setup.py` & `abdal_net_py-2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "2.2"
+VERSION = "2.6"
 DESCRIPTION = 'Powerful security network package'
 LONG_DESCRIPTION = 'Powerful security network package for hackers and all security experts'
 
 # Setting up
 setup(
     name="abdal_net_py",
     version=VERSION,
```

