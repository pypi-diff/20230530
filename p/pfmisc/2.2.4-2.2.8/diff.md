# Comparing `tmp/pfmisc-2.2.4.tar.gz` & `tmp/pfmisc-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfmisc-2.2.4.tar", last modified: Mon Mar 22 23:26:33 2021, max compression
+gzip compressed data, was "pfmisc-2.2.8.tar", last modified: Thu Jul 29 19:24:17 2021, max compression
```

## Comparing `pfmisc-2.2.4.tar` & `pfmisc-2.2.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2021-03-22 23:26:33.081215 pfmisc-2.2.4/
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)       20 2017-10-09 14:05:32.000000 pfmisc-2.2.4/MANIFEST.in
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1998 2021-03-22 23:26:33.081215 pfmisc-2.2.4/PKG-INFO
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1235 2021-03-22 23:22:58.000000 pfmisc-2.2.4/README.rst
-drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2021-03-22 23:26:33.077881 pfmisc-2.2.4/bin/
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     2059 2021-03-22 23:22:47.000000 pfmisc-2.2.4/bin/pfmisc
-drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2021-03-22 23:26:33.081215 pfmisc-2.2.4/pfmisc/
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     5519 2018-10-09 03:04:43.000000 pfmisc-2.2.4/pfmisc/Auth.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    65234 2021-03-22 23:22:32.000000 pfmisc-2.2.4/pfmisc/C_snode.py
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     3550 2021-01-05 22:36:03.000000 pfmisc-2.2.4/pfmisc/C_stringCore.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)      219 2021-01-05 22:36:03.000000 pfmisc-2.2.4/pfmisc/__init__.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1374 2021-01-05 22:36:03.000000 pfmisc-2.2.4/pfmisc/_colors.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     6126 2021-01-05 22:36:03.000000 pfmisc-2.2.4/pfmisc/debug.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     3028 2021-03-22 23:25:26.000000 pfmisc-2.2.4/pfmisc/dgmsocket.py
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     5094 2021-01-05 22:36:03.000000 pfmisc-2.2.4/pfmisc/error.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1635 2021-01-05 22:36:03.000000 pfmisc-2.2.4/pfmisc/local_ip.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    14818 2021-01-05 23:05:49.000000 pfmisc-2.2.4/pfmisc/message.py
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    41948 2021-01-05 23:24:38.000000 pfmisc-2.2.4/pfmisc/other.py
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     3658 2021-01-05 23:30:25.000000 pfmisc-2.2.4/pfmisc/pfmisc.py
--rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     3761 2021-01-05 23:06:20.000000 pfmisc-2.2.4/pfmisc/pfmisc2.py
-drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2021-03-22 23:26:33.081215 pfmisc-2.2.4/pfmisc.egg-info/
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1998 2021-03-22 23:26:32.000000 pfmisc-2.2.4/pfmisc.egg-info/PKG-INFO
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)      463 2021-03-22 23:26:32.000000 pfmisc-2.2.4/pfmisc.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        1 2021-03-22 23:26:32.000000 pfmisc-2.2.4/pfmisc.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        1 2017-10-17 22:42:30.000000 pfmisc-2.2.4/pfmisc.egg-info/not-zip-safe
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        5 2021-03-22 23:26:32.000000 pfmisc-2.2.4/pfmisc.egg-info/requires.txt
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        7 2021-03-22 23:26:32.000000 pfmisc-2.2.4/pfmisc.egg-info/top_level.txt
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)       65 2021-03-22 23:26:33.084548 pfmisc-2.2.4/setup.cfg
--rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)      891 2021-03-22 23:22:53.000000 pfmisc-2.2.4/setup.py
+drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2021-07-29 19:24:17.680345 pfmisc-2.2.8/
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)       20 2017-10-09 14:05:32.000000 pfmisc-2.2.8/MANIFEST.in
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     2199 2021-07-29 19:24:17.680345 pfmisc-2.2.8/PKG-INFO
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1380 2021-07-29 18:53:56.000000 pfmisc-2.2.8/README.rst
+drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2021-07-29 19:24:17.667012 pfmisc-2.2.8/bin/
+-rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     2136 2021-07-29 18:42:32.000000 pfmisc-2.2.8/bin/pfmisc
+drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2021-07-29 19:24:17.677012 pfmisc-2.2.8/pfmisc/
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     5519 2018-10-09 03:04:43.000000 pfmisc-2.2.8/pfmisc/Auth.py
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    65234 2021-03-22 23:22:32.000000 pfmisc-2.2.8/pfmisc/C_snode.py
+-rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     3550 2021-01-05 22:36:03.000000 pfmisc-2.2.8/pfmisc/C_stringCore.py
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)      219 2021-01-05 22:36:03.000000 pfmisc-2.2.8/pfmisc/__init__.py
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1374 2021-01-05 22:36:03.000000 pfmisc-2.2.8/pfmisc/_colors.py
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     6309 2021-07-29 17:05:34.000000 pfmisc-2.2.8/pfmisc/debug.py
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     3028 2021-03-22 23:25:26.000000 pfmisc-2.2.8/pfmisc/dgmsocket.py
+-rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     5094 2021-01-05 22:36:03.000000 pfmisc-2.2.8/pfmisc/error.py
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     1635 2021-01-05 22:36:03.000000 pfmisc-2.2.8/pfmisc/local_ip.py
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    14818 2021-01-05 23:05:49.000000 pfmisc-2.2.8/pfmisc/message.py
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)    41948 2021-01-05 23:24:38.000000 pfmisc-2.2.8/pfmisc/other.py
+-rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     4373 2021-07-29 18:53:19.000000 pfmisc-2.2.8/pfmisc/pfmisc.py
+-rwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)     3847 2021-07-29 17:15:36.000000 pfmisc-2.2.8/pfmisc/pfmisc2.py
+drwxrwxr-x   0 rudolphpienaar (2090878) rudolphpienaar   (977)        0 2021-07-29 19:24:17.677012 pfmisc-2.2.8/pfmisc.egg-info/
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)     2199 2021-07-29 19:24:17.000000 pfmisc-2.2.8/pfmisc.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)      463 2021-07-29 19:24:17.000000 pfmisc-2.2.8/pfmisc.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        1 2021-07-29 19:24:17.000000 pfmisc-2.2.8/pfmisc.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        1 2017-10-17 22:42:30.000000 pfmisc-2.2.8/pfmisc.egg-info/not-zip-safe
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        5 2021-07-29 19:24:17.000000 pfmisc-2.2.8/pfmisc.egg-info/requires.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)        7 2021-07-29 19:24:17.000000 pfmisc-2.2.8/pfmisc.egg-info/top_level.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)       65 2021-07-29 19:24:17.680345 pfmisc-2.2.8/setup.cfg
+-rw-rw-r--   0 rudolphpienaar (2090878) rudolphpienaar   (977)      891 2021-07-29 18:56:52.000000 pfmisc-2.2.8/setup.py
```

### Comparing `pfmisc-2.2.4/PKG-INFO` & `pfmisc-2.2.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.0
 Name: pfmisc
-Version: 2.2.4
+Version: 2.2.8
 Summary: Misc utilities for FNNDSC python repos
 Home-page: https://github.com/FNNDSC/pfmisc
 Author: Rudolph Pienaar
 Author-email: rudolph.pienaar@gmail.com
 License: MIT
 Description: ################
-        pfmisc  v2.2.4
+        pfmisc  v2.2.8
         ################
         
         .. image:: https://badge.fury.io/py/pfmisc.svg
             :target: https://badge.fury.io/py/pfmisc
         
         .. image:: https://travis-ci.org/FNNDSC/pfdcm.svg?branch=master
             :target: https://travis-ci.org/FNNDSC/pfmisc
@@ -42,15 +42,22 @@
             class MyClass():
         
                 def __init__(self, *args, **kwargs):
                     self.debug  = pfmisc.debug()
         
                     self.debug.qprint('hello there!')
         
-        which will result in some decent debugging in stdout.
+        which will result in some decent debugging in ``stdout``. Sometimes, it is useful to create a shortcut
+        
+        .. code-block:: python
+        
+            self.debug  = pfmisc.debug()
+            self.log    = self.debug.qprint
+        
+        
         
         ************
         Installation
         ************
         
         Installation is relatively straightforward, and best done with ``pip``:
```

### Comparing `pfmisc-2.2.4/README.rst` & `pfmisc-2.2.8/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ################
-pfmisc  v2.2.4
+pfmisc  v2.2.8
 ################
 
 .. image:: https://badge.fury.io/py/pfmisc.svg
     :target: https://badge.fury.io/py/pfmisc
 
 .. image:: https://travis-ci.org/FNNDSC/pfdcm.svg?branch=master
     :target: https://travis-ci.org/FNNDSC/pfmisc
@@ -34,15 +34,22 @@
     class MyClass():
 
         def __init__(self, *args, **kwargs):
             self.debug  = pfmisc.debug()
 
             self.debug.qprint('hello there!')
 
-which will result in some decent debugging in stdout.
+which will result in some decent debugging in ``stdout``. Sometimes, it is useful to create a shortcut
+
+.. code-block:: python
+
+    self.debug  = pfmisc.debug()
+    self.log    = self.debug.qprint
+
+
 
 ************
 Installation
 ************
 
 Installation is relatively straightforward, and best done with ``pip``:
```

### Comparing `pfmisc-2.2.4/bin/pfmisc` & `pfmisc-2.2.8/bin/pfmisc`

 * *Files 5% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 # (c) 2017-2020 Fetal-Neonatal Neuroimaging & Developmental Science Center
 #                     Boston Children's Hospital
 #
 #                http://childrenshospital.org/FNNDSC/
 #                         dev@babyMRI.org
 #
 
-import sys, os
+import  sys, os
+sys.path.insert(1, os.path.join(os.path.dirname(__file__), '..'))
 
 import  socket
 from    argparse                import RawTextHelpFormatter
 from    argparse                import ArgumentParser
 
 import  pudb
-
-from pfmisc import Colors, pfmisc, pfmisc2, local_ip_address
+from    pfmisc import Colors, pfmisc, pfmisc2, local_ip_address
 
 
 str_defIP = local_ip_address()
-str_version = "2.2.4"
-str_desc = Colors.CYAN + """
+str_version = "2.2.8"
+str_desc = Colors.CYAN + r"""
 
 
         __           _          
        / _|         (_)         
  _ __ | |_ _ __ ___  _ ___  ___ 
 | '_ \|  _| '_ ` _ \| / __|/ __|
 | |_) | | | | | | | | \__ \ (__ 
 | .__/|_| |_| |_| |_|_|___/\___|
 | |                             
 |_|                             
 
 
-                            Path-File-misc
+                              Path-File-misc
 
-           Miscellaneous utilities for the pf* family.
+                Miscellaneous utilities for the pf* family.
 
                               -- version """ + \
              Colors.YELLOW + str_version + Colors.CYAN + """ --
 
     'pfmisc' is a simple example script of how to use the various family
     of miscellaneous help utilties (typically the debug utility) in misc
     settings.
```

### Comparing `pfmisc-2.2.4/pfmisc/Auth.py` & `pfmisc-2.2.8/pfmisc/Auth.py`

 * *Files identical despite different names*

### Comparing `pfmisc-2.2.4/pfmisc/C_snode.py` & `pfmisc-2.2.8/pfmisc/C_snode.py`

 * *Files identical despite different names*

### Comparing `pfmisc-2.2.4/pfmisc/C_stringCore.py` & `pfmisc-2.2.8/pfmisc/C_stringCore.py`

 * *Files identical despite different names*

### Comparing `pfmisc-2.2.4/pfmisc/_colors.py` & `pfmisc-2.2.8/pfmisc/_colors.py`

 * *Files identical despite different names*

### Comparing `pfmisc-2.2.4/pfmisc/debug.py` & `pfmisc-2.2.8/pfmisc/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,25 +50,25 @@
 
         self.verbosity              = 1
         self.level                  = 1
 
         self.b_colorize             = True
         self.b_useDebug             = False
         self.str_debugDirFile       = '/tmp'
-        self.__name__               = 'debug'
+        self.within                 = 'debug'
         self.hostnamecol            = 15
         self.methodcol              = 45
         self.b_syslog               = True
 
         for k, v in kwargs.items():
             if k == 'verbosity':    self.verbosity          = v
             if k == 'level':        self.level              = v
             if k == 'debugToFile':  self.b_useDebug         = v
             if k == 'debugFile':    self.str_debugDirFile   = v
-            if k == 'within':       self.__name__           = v
+            if k == 'within':       self.within             = v
             if k == 'colorize':     self.b_colorize         = v
             if k == 'hostnamecol':  self.hostnamecol        = int(v)
             if k == 'methodcol':    self.methodcol          = int(v)
             if k == 'syslog':       self.b_syslog           = bool(v)
 
         if self.b_useDebug:
             str_debugDir                = os.path.dirname(self.str_debugDirFile)
@@ -97,26 +97,28 @@
         str_comms   = "normal"
         self.level  = 1
         self.msg    = ""
         stackDepth  = 1
 
         b_syslog    = self.b_syslog
         b_end       = False
-
+        b_colorize  = self.b_colorize
         methodcol   = self.methodcol
+        end         = ""
 
         for k, v in kwargs.items():
             if k == 'level'     :   self.level  = v
             if k == 'msg'       :   self.msg    = v
             if k == 'comms'     :   str_comms   = v
             if k == 'teeFile'   :   str_teeFile = v
             if k == 'teeMode'   :   str_teeMode = v
             if k == 'stackDepth':   stackDepth  = v
             if k == 'methodcol' :   methodcol   = int(v)
             if k == 'syslog'    :   b_syslog    = bool(v)
+            if k == 'colorize'  :   b_colorize  = bool(v)
             if k == 'end'       :
                 b_end       = True
                 end         = v
 
         if msg != None:
             self.msg = msg
 
@@ -130,41 +132,47 @@
 
         stack = inspect.stack()
         str_callerFile      = os.path.split(stack[1][1])[1]
         str_callerMethod    = inspect.stack()[stackDepth][3]
 
         if self.level <= self.verbosity:
             if b_syslog:
-                if self.b_colorize: write(Colors.CYAN,                                  end="")
-                write('%s' % datetime.datetime.now().replace(microsecond=0) + "  | ",   end="")
-                if self.b_colorize: write(Colors.LIGHT_CYAN,                            end="")
-                write('%*s | ' % (self.hostnamecol, self.str_hostname),                 end="")
-                if self.b_colorize: write(Colors.LIGHT_BLUE,                            end="")
-                write('%*s' % ( methodcol, str_callerFile + ':' +
-                                self.__name__ + "." + str_callerMethod + '()') + ' | ', end="")
-            if self.b_colorize:
-                if str_comms == 'normal':   write(Colors.WHITE,                     end="")
-                if str_comms == 'status':   write(Colors.PURPLE,                    end="")
-                if str_comms == 'error':    write(Colors.RED,                       end="")
-                if str_comms == "tx":       write(Colors.YELLOW,                    end="")
-                if str_comms == "rx":       write(Colors.GREEN,                     end="")
+                if b_colorize: write(Colors.CYAN,                   end="")
+                write('%s' %
+                    datetime.datetime.now().replace(microsecond=0)
+                    + "  | ",                                       end="")
+                if b_colorize: write(Colors.LIGHT_CYAN,             end="")
+                write('%*s | ' % (
+                        self.hostnamecol, self.str_hostname
+                    ),                                              end="")
+                if b_colorize: write(Colors.LIGHT_BLUE,             end="")
+                write('%*s' % (
+                        methodcol, str_callerFile + ':'                 +
+                        self.within + "." + str_callerMethod + '()')    +
+                        ' | ',                                      end="")
+            if b_colorize:
+                if str_comms == 'normal':   write(Colors.WHITE,     end="")
+                if str_comms == 'status':   write(Colors.PURPLE,    end="")
+                if str_comms == 'error':    write(Colors.RED,       end="")
+                if str_comms == "tx":       write(Colors.YELLOW,    end="")
+                if str_comms == "rx":       write(Colors.GREEN,     end="")
             if str_comms == "tx":           write("\n---->")
             if str_comms == "rx":           write("\n<----")
 
             if b_end:
                 write(msg, end = end )
             else:
                 write(msg)
 
             if len(str_teeFile):
                 tf.write(msg)
                 tf.close()
 
             if not self.b_colorize:
-                if str_comms == "tx":       write(Colors.YELLOW,                    end="")
-                if str_comms == "rx":       write(Colors.GREEN,                     end="")
+                if str_comms == "tx":       write(Colors.YELLOW,    end="")
+                if str_comms == "rx":       write(Colors.GREEN,     end="")
 
             if str_comms == "tx":           write("---->")
             if str_comms == "rx":           write("<----")
 
-            if self.b_colorize:         write(Colors.NO_COLOUR, end="")
+            if b_colorize:         write(Colors.NO_COLOUR, end="")
```

### Comparing `pfmisc-2.2.4/pfmisc/dgmsocket.py` & `pfmisc-2.2.8/pfmisc/dgmsocket.py`

 * *Files identical despite different names*

### Comparing `pfmisc-2.2.4/pfmisc/error.py` & `pfmisc-2.2.8/pfmisc/error.py`

 * *Files identical despite different names*

### Comparing `pfmisc-2.2.4/pfmisc/local_ip.py` & `pfmisc-2.2.8/pfmisc/local_ip.py`

 * *Files identical despite different names*

### Comparing `pfmisc-2.2.4/pfmisc/message.py` & `pfmisc-2.2.8/pfmisc/message.py`

 * *Files identical despite different names*

### Comparing `pfmisc-2.2.4/pfmisc/other.py` & `pfmisc-2.2.8/pfmisc/other.py`

 * *Files identical despite different names*

### Comparing `pfmisc-2.2.4/pfmisc/pfmisc.py` & `pfmisc-2.2.8/pfmisc/pfmisc2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#!/usr/bin/env python3.5
+import sys
+import os
+import json
+import pudb
+sys.path.insert(1, os.path.join(os.path.dirname(__file__), '..'))
+
+from    pfmisc._colors  import Colors
+from    pfmisc.debug    import debug
+from    pfmisc.C_snode  import *
+from    pfmisc.error    import *
 
-import  sys
-import  os
-import  json
-import  pudb
-
-from pfmisc._colors import Colors
-from pfmisc.debug   import debug
-from pfmisc.C_snode import *
-from pfmisc.error   import *
 
-class someOtherClass():
+class someOtherClass2():
     """
     Some other class
     """
 
     def __init__(self, *args, **kwargs):
         """
         """
 
-        self.dp             = debug(verbosity=0, level=-1, within = "someOtherClass")
+        self.dp             = debug(verbosity=0, level=-1, within = "someOtherClass2")
 
     def say(self, msg):
         print('\n* Now we are in a different class in this module...')
         print('* Note the different class and method in the debug output.')
         print('* calling: self.dp.qprint(msg):')
         self.dp.qprint(msg)
 
-class pfmisc():
+class pfmisc2():
     """
     Example of how to use the local misc dependencies
     """
 
     # An error declaration block
     _dictErr = {
         'someError1'   : {
@@ -63,46 +63,50 @@
         self.RC             = 40
         self.args           = None
         self.str_desc       = 'pfmisc'
         self.str_name       = self.str_desc
         self.str_version    = ''
 
         self.dp             = debug(verbosity   = 1,
-                                    within      = 'pfmisc',
-                                    hostnamecol = 7,
-                                    methodcol   = 10)
+                                    within      = 'pfmisc2')
 
         self.dp2            = debug(verbosity   = 1,
-                                    within      = 'pfmisc',
+                                    within      = 'pfmisc2',
                                     debugToFile = True,
-                                    debugFile   = '/tmp/pfmisc.txt')
-
+                                    debugFile   = '/tmp/pfmisc2.txt')
     def demo(self, *args, **kwargs):
         """
         Simple run method
         """
 
         print('* calling: self.dp.qprint("Why hello there, world!"):')
         self.dp.qprint("Why hello there, world!")
 
         print('* calling: self.dp2.qprint("Why hello there, world! In a debugging file!"):')
         self.dp2.qprint("Why hello there, world! In a debugging file!")
-        print('* Check on /tmp/pfmisc.txt')
-
-        print('* calling: self.dp.qprint("Why hello there, world! With teeFile!", teeFile="/tmp/pfmisc-teefile.txt", teeMode = "w+"):')
-        self.dp.qprint("Why hello there, world! With teeFile!", teeFile="/tmp/pfmisc-teefile.txt", teeMode = "w+")
-        print('* Check on /tmp/pfmisc-teefile.txt')
+        print('* Check on /tmp/pfmisc2.txt')
 
-        other = someOtherClass()
+        other = someOtherClass2()
         other.say("And this is from a different class")
 
+        print('* now with no syslog...')
+        print('* calling: self.dp.qprint("Hello there, world w/o syslog!", syslog = False):')
+        self.dp.qprint("Hello there, world w/o syslog!", syslog = False)
+
+        print('\n* end and no end...')
+        print('* calling: self.dp.qprint("This is the end... ", end=''):')
+        print('* calling: self.dp.qprint("My only friend the end", syslog = False):')
+        self.dp.qprint("This is the end... ", end='')
+        self.dp.qprint("My only friend the end", syslog = False)
+
         for str_comms in ['status', 'error', 'tx', 'rx']:
             print('\n* calling: self.dp.qprint("This string is tagged with %s" % str_comms, ', end='')
             print("comms = '%s')" % str_comms)
             self.dp.qprint("This string is tagged with '%s'" % str_comms, comms = str_comms)
 
-        print("And here is warning...")
-        warn(
-            self, 'someError1',
-            header  = 'This is only a warning!',
+        print("Followed by an error...")
+        fatal(
+            self, 'someError2',
+            header  = 'This is an unrecoverable error!',
             drawBox = True
         )
+
```

### Comparing `pfmisc-2.2.4/pfmisc/pfmisc2.py` & `pfmisc-2.2.8/pfmisc/pfmisc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,43 @@
-import sys
-import os
-import json
-import pudb
-
-from pfmisc._colors import Colors
-from pfmisc.debug import debug
-from pfmisc.C_snode import *
-from pfmisc.error import *
+#!/usr/bin/env python3.5
 
+import  sys
+import  os
+import  json
+import  pudb
+sys.path.insert(1, os.path.join(os.path.dirname(__file__), '..'))
+
+from    pfmisc._colors import Colors
+from    pfmisc.debug   import debug
+from    pfmisc.C_snode import *
+from    pfmisc.error   import *
 
-class someOtherClass2():
+class someOtherClass():
     """
     Some other class
     """
 
     def __init__(self, *args, **kwargs):
         """
         """
 
-        self.dp             = debug(verbosity=0, level=-1, within = "someOtherClass2")
+        self.dp             = debug(
+                                verbosity   = 0,
+                                level       = -1,
+                                within      = "someOtherClass"
+                            )
+        self.log            = self.dp.qprint
 
     def say(self, msg):
         print('\n* Now we are in a different class in this module...')
         print('* Note the different class and method in the debug output.')
         print('* calling: self.dp.qprint(msg):')
-        self.dp.qprint(msg)
+        self.log(msg, level = -1)
 
-class pfmisc2():
+class pfmisc():
     """
     Example of how to use the local misc dependencies
     """
 
     # An error declaration block
     _dictErr = {
         'someError1'   : {
@@ -62,50 +69,54 @@
         self.RC             = 40
         self.args           = None
         self.str_desc       = 'pfmisc'
         self.str_name       = self.str_desc
         self.str_version    = ''
 
         self.dp             = debug(verbosity   = 1,
-                                    within      = 'pfmisc2')
+                                    within      = 'pfmisc',
+                                    hostnamecol = 7,
+                                    methodcol   = 10)
+        self.log            = self.dp.qprint
 
         self.dp2            = debug(verbosity   = 1,
-                                    within      = 'pfmisc2',
+                                    within      = 'pfmisc',
                                     debugToFile = True,
-                                    debugFile   = '/tmp/pfmisc2.txt')
+                                    debugFile   = '/tmp/pfmisc.txt')
+        self.log2           = self.dp2.qprint
+
     def demo(self, *args, **kwargs):
         """
         Simple run method
         """
+        # pudb.set_trace()
+        print('\n* calling: self.dp.qprint("Why hello there, world!"):')
+        self.log("Why hello there, world!")
 
-        print('* calling: self.dp.qprint("Why hello there, world!"):')
-        self.dp.qprint("Why hello there, world!")
+        print('\n* calling: self.dp.qprint("Why hello there, world!", colorize = False):')
+        self.log("Why hello there, world!", colorize = False)
 
-        print('* calling: self.dp2.qprint("Why hello there, world! In a debugging file!"):')
-        self.dp2.qprint("Why hello there, world! In a debugging file!")
-        print('* Check on /tmp/pfmisc2.txt')
+        print('\n* calling: self.dp.qprint("Why hello there, world!", colorize = False, syslog = False):')
+        self.log("Why hello there, world!", colorize = False, syslog = False)
 
-        other = someOtherClass2()
-        other.say("And this is from a different class")
+        print('\n* calling: self.dp2.qprint("Why hello there, world! In a debugging file!"):')
+        self.log2("Why hello there, world! In a debugging file!")
+        print('\n* Check on /tmp/pfmisc.txt')
 
-        print('* now with no syslog...')
-        print('* calling: self.dp.qprint("Hello there, world w/o syslog!", syslog = False):')
-        self.dp.qprint("Hello there, world w/o syslog!", syslog = False)
-
-        print('\n* end and no end...')
-        print('* calling: self.dp.qprint("This is the end... ", end=''):')
-        print('* calling: self.dp.qprint("My only friend the end", syslog = False):')
-        self.dp.qprint("This is the end... ", end='')
-        self.dp.qprint("My only friend the end", syslog = False)
+        print('\n* calling: self.dp.qprint("Why hello there, world! With teeFile!", teeFile="/tmp/pfmisc-teefile.txt", teeMode = "w+"):')
+        self.log("Why hello there, world! With teeFile!", teeFile="/tmp/pfmisc-teefile.txt", teeMode = "w+")
+        print('\n* Check on /tmp/pfmisc-teefile.txt')
+
+        other = someOtherClass()
+        other.say("And this is from a different class")
 
         for str_comms in ['status', 'error', 'tx', 'rx']:
             print('\n* calling: self.dp.qprint("This string is tagged with %s" % str_comms, ', end='')
             print("comms = '%s')" % str_comms)
-            self.dp.qprint("This string is tagged with '%s'" % str_comms, comms = str_comms)
+            self.log("This string is tagged with '%s'" % str_comms, comms = str_comms)
 
-        print("Followed by an error...")
-        fatal(
-            self, 'someError2',
-            header  = 'This is an unrecoverable error!',
+        print("And here is warning...")
+        warn(
+            self, 'someError1',
+            header  = 'This is only a warning!',
             drawBox = True
         )
-
```

### Comparing `pfmisc-2.2.4/pfmisc.egg-info/PKG-INFO` & `pfmisc-2.2.8/pfmisc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.0
 Name: pfmisc
-Version: 2.2.4
+Version: 2.2.8
 Summary: Misc utilities for FNNDSC python repos
 Home-page: https://github.com/FNNDSC/pfmisc
 Author: Rudolph Pienaar
 Author-email: rudolph.pienaar@gmail.com
 License: MIT
 Description: ################
-        pfmisc  v2.2.4
+        pfmisc  v2.2.8
         ################
         
         .. image:: https://badge.fury.io/py/pfmisc.svg
             :target: https://badge.fury.io/py/pfmisc
         
         .. image:: https://travis-ci.org/FNNDSC/pfdcm.svg?branch=master
             :target: https://travis-ci.org/FNNDSC/pfmisc
@@ -42,15 +42,22 @@
             class MyClass():
         
                 def __init__(self, *args, **kwargs):
                     self.debug  = pfmisc.debug()
         
                     self.debug.qprint('hello there!')
         
-        which will result in some decent debugging in stdout.
+        which will result in some decent debugging in ``stdout``. Sometimes, it is useful to create a shortcut
+        
+        .. code-block:: python
+        
+            self.debug  = pfmisc.debug()
+            self.log    = self.debug.qprint
+        
+        
         
         ************
         Installation
         ************
         
         Installation is relatively straightforward, and best done with ``pip``:
```

### Comparing `pfmisc-2.2.4/setup.py` & `pfmisc-2.2.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
       name             =   'pfmisc',
-      version          =   '2.2.4',
+      version          =   '2.2.8',
       description      =   'Misc utilities for FNNDSC python repos',
       long_description =   readme(),
       author           =   'Rudolph Pienaar',
       author_email     =   'rudolph.pienaar@gmail.com',
       url              =   'https://github.com/FNNDSC/pfmisc',
       packages         =   ['pfmisc'],
       install_requires =   ['pudb'],
```

