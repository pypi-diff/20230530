# Comparing `tmp/pulumi_select-0.1.5.tar.gz` & `tmp/pulumi_select-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_select-0.1.5.tar", last modified: Tue May 30 07:35:13 2023, max compression
+gzip compressed data, was "pulumi_select-0.1.6.tar", last modified: Tue May 30 07:40:01 2023, max compression
```

## Comparing `pulumi_select-0.1.5.tar` & `pulumi_select-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 romainrbr   (501) staff       (20)        0 2023-05-30 07:35:13.016727 pulumi_select-0.1.5/
--rw-r--r--   0 romainrbr   (501) staff       (20)      476 2023-03-31 12:27:08.000000 pulumi_select-0.1.5/LICENCE.txt
--rw-r--r--   0 romainrbr   (501) staff       (20)      763 2023-05-30 07:35:13.016818 pulumi_select-0.1.5/PKG-INFO
--rw-r--r--   0 romainrbr   (501) staff       (20)       71 2023-03-31 12:15:46.000000 pulumi_select-0.1.5/README.md
-drwxr-xr-x   0 romainrbr   (501) staff       (20)        0 2023-05-30 07:35:13.015593 pulumi_select-0.1.5/pulumi_select/
--rw-r--r--   0 romainrbr   (501) staff       (20)     1843 2023-03-31 12:40:03.000000 pulumi_select-0.1.5/pulumi_select/__main__.py
-drwxr-xr-x   0 romainrbr   (501) staff       (20)        0 2023-05-30 07:35:13.016548 pulumi_select-0.1.5/pulumi_select.egg-info/
--rw-r--r--   0 romainrbr   (501) staff       (20)      763 2023-05-30 07:35:12.000000 pulumi_select-0.1.5/pulumi_select.egg-info/PKG-INFO
--rw-r--r--   0 romainrbr   (501) staff       (20)      290 2023-05-30 07:35:12.000000 pulumi_select-0.1.5/pulumi_select.egg-info/SOURCES.txt
--rw-r--r--   0 romainrbr   (501) staff       (20)        1 2023-05-30 07:35:12.000000 pulumi_select-0.1.5/pulumi_select.egg-info/dependency_links.txt
--rw-r--r--   0 romainrbr   (501) staff       (20)       62 2023-05-30 07:35:12.000000 pulumi_select-0.1.5/pulumi_select.egg-info/entry_points.txt
--rw-r--r--   0 romainrbr   (501) staff       (20)       72 2023-05-30 07:35:12.000000 pulumi_select-0.1.5/pulumi_select.egg-info/requires.txt
--rw-r--r--   0 romainrbr   (501) staff       (20)       14 2023-05-30 07:35:12.000000 pulumi_select-0.1.5/pulumi_select.egg-info/top_level.txt
--rw-r--r--   0 romainrbr   (501) staff       (20)       50 2023-05-30 07:35:13.017038 pulumi_select-0.1.5/setup.cfg
--rw-r--r--   0 romainrbr   (501) staff       (20)     1179 2023-05-30 07:35:08.000000 pulumi_select-0.1.5/setup.py
+drwxr-xr-x   0 romainrbr   (501) staff       (20)        0 2023-05-30 07:40:01.159924 pulumi_select-0.1.6/
+-rw-r--r--   0 romainrbr   (501) staff       (20)      476 2023-03-31 12:27:08.000000 pulumi_select-0.1.6/LICENCE.txt
+-rw-r--r--   0 romainrbr   (501) staff       (20)      763 2023-05-30 07:40:01.159988 pulumi_select-0.1.6/PKG-INFO
+-rw-r--r--   0 romainrbr   (501) staff       (20)       71 2023-03-31 12:15:46.000000 pulumi_select-0.1.6/README.md
+drwxr-xr-x   0 romainrbr   (501) staff       (20)        0 2023-05-30 07:40:01.158914 pulumi_select-0.1.6/pulumi_select/
+-rw-r--r--   0 romainrbr   (501) staff       (20)     1440 2023-05-30 07:39:33.000000 pulumi_select-0.1.6/pulumi_select/__main__.py
+drwxr-xr-x   0 romainrbr   (501) staff       (20)        0 2023-05-30 07:40:01.159765 pulumi_select-0.1.6/pulumi_select.egg-info/
+-rw-r--r--   0 romainrbr   (501) staff       (20)      763 2023-05-30 07:40:01.000000 pulumi_select-0.1.6/pulumi_select.egg-info/PKG-INFO
+-rw-r--r--   0 romainrbr   (501) staff       (20)      290 2023-05-30 07:40:01.000000 pulumi_select-0.1.6/pulumi_select.egg-info/SOURCES.txt
+-rw-r--r--   0 romainrbr   (501) staff       (20)        1 2023-05-30 07:40:01.000000 pulumi_select-0.1.6/pulumi_select.egg-info/dependency_links.txt
+-rw-r--r--   0 romainrbr   (501) staff       (20)       62 2023-05-30 07:40:01.000000 pulumi_select-0.1.6/pulumi_select.egg-info/entry_points.txt
+-rw-r--r--   0 romainrbr   (501) staff       (20)       72 2023-05-30 07:40:01.000000 pulumi_select-0.1.6/pulumi_select.egg-info/requires.txt
+-rw-r--r--   0 romainrbr   (501) staff       (20)       14 2023-05-30 07:40:01.000000 pulumi_select-0.1.6/pulumi_select.egg-info/top_level.txt
+-rw-r--r--   0 romainrbr   (501) staff       (20)       50 2023-05-30 07:40:01.160178 pulumi_select-0.1.6/setup.cfg
+-rw-r--r--   0 romainrbr   (501) staff       (20)     1179 2023-05-30 07:39:55.000000 pulumi_select-0.1.6/setup.py
```

### Comparing `pulumi_select-0.1.5/PKG-INFO` & `pulumi_select-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_select
-Version: 0.1.5
+Version: 0.1.6
 Summary: dynamically select urns to apply from a pulumi preview
 Home-page: https://github.com/romainrbr/pulumi-select
 Download-URL: https://github.com/romainrbr/pulumi-select/archive/v_01.tar.gz
 Author: romainrbr
 Author-email: contact@romain.tech
 License: WTFPL
 Keywords: pulumi,select
```

### Comparing `pulumi_select-0.1.5/pulumi_select/__main__.py` & `pulumi_select-0.1.6/pulumi_select/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 import inquirer
 import subprocess
 import re
 
 def main(args=None):
     click.secho('Pulumi preview in progress ...', fg='green')
     with click_spinner.spinner():
-        # Hack for zsh & atuin
-        if os.environ.get('ATUIN_SESSION') is not None and os.environ.get('SHELL') == "/bin/zsh":
-            subprocess.call('echoti rmkx',shell=True,executable='/bin/zsh')
         subprocess.call('pulumi preview -j > /tmp/preview.json',shell=True,executable='/bin/zsh')
 
     create = []
     update = []
     delete = []
     with open('/tmp/preview.json') as f:
         data = json.load(f)
@@ -38,15 +35,11 @@
     # remove ascii color code from answers
     answers['pulumiup'] = [re.sub(r'\x1b[^m]*m', '', x) for x in answers['pulumiup']]
 
     pulumi_command = "pulumi up "
     for answer in answers['pulumiup']:
         pulumi_command += "-t "+ answer + " "
 
-    # Hack for zsh & atuin
-    if os.environ.get('ATUIN_SESSION') is not None and os.environ.get('SHELL') == "/bin/zsh":
-            subprocess.call('echoti smkx',shell=True,executable='/bin/zsh')
-
     click.secho(pulumi_command, fg='green')
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pulumi_select-0.1.5/pulumi_select.egg-info/PKG-INFO` & `pulumi_select-0.1.6/pulumi_select.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-select
-Version: 0.1.5
+Version: 0.1.6
 Summary: dynamically select urns to apply from a pulumi preview
 Home-page: https://github.com/romainrbr/pulumi-select
 Download-URL: https://github.com/romainrbr/pulumi-select/archive/v_01.tar.gz
 Author: romainrbr
 Author-email: contact@romain.tech
 License: WTFPL
 Keywords: pulumi,select
```

### Comparing `pulumi_select-0.1.5/setup.py` & `pulumi_select-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'pulumi_select',
   packages = ['pulumi_select'],
-  version = '0.1.5', 
+  version = '0.1.6', 
   license='WTFPL',
   description = 'dynamically select urns to apply from a pulumi preview',
   author = 'romainrbr',
   author_email = 'contact@romain.tech',
   url = 'https://github.com/romainrbr/pulumi-select',
   download_url = 'https://github.com/romainrbr/pulumi-select/archive/v_01.tar.gz',
   keywords = ['pulumi', 'select'],
```

