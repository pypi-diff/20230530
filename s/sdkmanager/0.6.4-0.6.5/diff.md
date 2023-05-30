# Comparing `tmp/sdkmanager-0.6.4.tar.gz` & `tmp/sdkmanager-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkmanager-0.6.4.tar", last modified: Fri Mar 24 12:14:11 2023, max compression
+gzip compressed data, was "sdkmanager-0.6.5.tar", last modified: Tue May 30 11:24:45 2023, max compression
```

## Comparing `sdkmanager-0.6.4.tar` & `sdkmanager-0.6.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2023-03-24 12:14:11.008251 sdkmanager-0.6.4/
--rw-r--r--   0 hans      (1000) hans      (1000)    34520 2021-06-18 10:09:13.000000 sdkmanager-0.6.4/LICENSE
--rw-r--r--   0 hans      (1000) hans      (1000)     1922 2023-03-24 12:14:11.008251 sdkmanager-0.6.4/PKG-INFO
--rw-r--r--   0 hans      (1000) hans      (1000)      639 2021-06-18 10:09:13.000000 sdkmanager-0.6.4/README.md
--rw-r--r--   0 hans      (1000) hans      (1000)       46 2021-06-18 10:09:13.000000 sdkmanager-0.6.4/pyproject.toml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2023-03-24 12:14:11.008251 sdkmanager-0.6.4/sdkmanager.egg-info/
--rw-r--r--   0 hans      (1000) hans      (1000)     1922 2023-03-24 12:14:10.000000 sdkmanager-0.6.4/sdkmanager.egg-info/PKG-INFO
--rw-r--r--   0 hans      (1000) hans      (1000)      271 2023-03-24 12:14:10.000000 sdkmanager-0.6.4/sdkmanager.egg-info/SOURCES.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        1 2023-03-24 12:14:10.000000 sdkmanager-0.6.4/sdkmanager.egg-info/dependency_links.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       47 2023-03-24 12:14:10.000000 sdkmanager-0.6.4/sdkmanager.egg-info/entry_points.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       71 2023-03-24 12:14:10.000000 sdkmanager-0.6.4/sdkmanager.egg-info/requires.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       11 2023-03-24 12:14:10.000000 sdkmanager-0.6.4/sdkmanager.egg-info/top_level.txt
--rwxr-xr-x   0 hans      (1000) hans      (1000)    66169 2023-03-24 12:13:28.000000 sdkmanager-0.6.4/sdkmanager.py
--rw-r--r--   0 hans      (1000) hans      (1000)      113 2023-03-24 12:14:11.008251 sdkmanager-0.6.4/setup.cfg
--rwxr-xr-x   0 hans      (1000) hans      (1000)     2641 2023-03-24 12:13:11.000000 sdkmanager-0.6.4/setup.py
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2023-05-30 11:24:45.129865 sdkmanager-0.6.5/
+-rw-r--r--   0 hans      (1000) hans      (1000)    34520 2021-06-18 10:09:13.000000 sdkmanager-0.6.5/LICENSE
+-rw-r--r--   0 hans      (1000) hans      (1000)     1922 2023-05-30 11:24:45.129865 sdkmanager-0.6.5/PKG-INFO
+-rw-r--r--   0 hans      (1000) hans      (1000)      639 2021-06-18 10:09:13.000000 sdkmanager-0.6.5/README.md
+-rw-r--r--   0 hans      (1000) hans      (1000)       46 2021-06-18 10:09:13.000000 sdkmanager-0.6.5/pyproject.toml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2023-05-30 11:24:45.129865 sdkmanager-0.6.5/sdkmanager.egg-info/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1922 2023-05-30 11:24:45.000000 sdkmanager-0.6.5/sdkmanager.egg-info/PKG-INFO
+-rw-r--r--   0 hans      (1000) hans      (1000)      271 2023-05-30 11:24:45.000000 sdkmanager-0.6.5/sdkmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        1 2023-05-30 11:24:45.000000 sdkmanager-0.6.5/sdkmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       47 2023-05-30 11:24:45.000000 sdkmanager-0.6.5/sdkmanager.egg-info/entry_points.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       81 2023-05-30 11:24:45.000000 sdkmanager-0.6.5/sdkmanager.egg-info/requires.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       11 2023-05-30 11:24:45.000000 sdkmanager-0.6.5/sdkmanager.egg-info/top_level.txt
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    66628 2023-05-11 14:49:52.000000 sdkmanager-0.6.5/sdkmanager.py
+-rw-r--r--   0 hans      (1000) hans      (1000)      113 2023-05-30 11:24:45.129865 sdkmanager-0.6.5/setup.cfg
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     2654 2023-05-30 10:52:56.000000 sdkmanager-0.6.5/setup.py
```

### Comparing `sdkmanager-0.6.4/LICENSE` & `sdkmanager-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkmanager-0.6.4/PKG-INFO` & `sdkmanager-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkmanager
-Version: 0.6.4
+Version: 0.6.5
 Summary: Android SDK Manager
 Home-page: https://gitlab.com/fdroid/sdkmanager
 Author: The F-Droid Project
 Author-email: team@f-droid.org
 License: AGPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `sdkmanager-0.6.4/README.md` & `sdkmanager-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `sdkmanager-0.6.4/sdkmanager.egg-info/PKG-INFO` & `sdkmanager-0.6.5/sdkmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkmanager
-Version: 0.6.4
+Version: 0.6.5
 Summary: Android SDK Manager
 Home-page: https://gitlab.com/fdroid/sdkmanager
 Author: The F-Droid Project
 Author-email: team@f-droid.org
 License: AGPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `sdkmanager-0.6.4/sdkmanager.py` & `sdkmanager-0.6.5/sdkmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,17 @@
     'platforms': 'platforms/{revision}',
     'platform-tools': 'platform-tools',
     'skiaparser': 'skiaparser/{revision}',
     'tools': 'tools',
     'extras;android;m2repository': 'extras/android/m2repository',
 }
 
+# NDK releases are like r25b, revisions are like 25.1.8937393. Dir names use revisions.
+NDK_REVISIONS = {}
+
 # xsi:type="ns3:genericDetailsType
 GENERIC_PACKAGE_XML_TEMPLATE = textwrap.dedent(
     """
     <?xml version="1.0" encoding="UTF-8" standalone="yes"?>
     <ns2:repository
         xmlns:ns2="http://schemas.android.com/repository/android/common/01"
         xmlns:ns3="http://schemas.android.com/repository/android/generic/01"
@@ -634,22 +637,25 @@
     if 'source.properties' in d:
         source_properties = get_properties_dict(d['source.properties'])
         _add_to_revisions(url, source_properties)
         key = tuple(source_properties['pkg.path'].split(';'))
         if key not in packages:
             packages[key] = url
 
-    highest = '0'
+    v = re.compile(r'^[0-9.]+$')
+    highest = None
     for key, url in packages.items():
         if key[0] != 'cmdline-tools' or len(key) < 2:
             continue
         version = key[-1]
         if version == 'latest':
             continue
-        if LooseVersion(version) > LooseVersion(highest):
+        if highest is None:
+            highest = version
+        elif v.match(version) and LooseVersion(version) > LooseVersion(highest):
             highest = version
     # TODO choose version for 'latest' based on --channel
     # https://developer.android.com/studio/releases/cmdline-tools
     packages[('cmdline-tools', 'latest')] = packages[('cmdline-tools', highest)]
 
 
 def parse_emulator(url, d):
@@ -681,25 +687,28 @@
                 packages[versioned] = url
             noleading0 = key + tuple([revision.lstrip('0')])
             if noleading0 not in packages:
                 packages[noleading0] = url
 
 
 def parse_ndk(url, d):
+    revision = None
     if 'source.properties' in d:
         source_properties = get_properties_dict(d['source.properties'])
         _add_to_revisions(url, source_properties)
         revision = source_properties['pkg.revision']
         for k in ('ndk', 'ndk-bundle'):
             key = (k, revision)
             if key not in packages:
                 packages[key] = url
     m = NDK_RELEASE_REGEX.search(url)
     if m:
         release = m.group()
+        if revision:
+            NDK_REVISIONS[release] = revision
         packages[('ndk', release)] = url
         packages[('ndk-bundle', release)] = url
         # add fake revision for NDKs without source.properties
         if url not in revisions:
             revisions[url] = (1,)
             vstring = re.search(r"android-ndk-r(\d*)([a-z])-linux", url)
             if vstring:
@@ -1000,15 +1009,19 @@
 
         if key[0] == 'extras' and len(key) in (3, 4):
             name = ';'.join(key[:3])
         else:
             name = key[0]
 
         if len(key) > 1:
-            install_dir = android_home / INSTALL_DIRS[name].format(revision=key[-1])
+            if key[0] == 'ndk':
+                revision = NDK_REVISIONS.get(key[-1], key[-1])
+            else:
+                revision = key[-1]
+            install_dir = android_home / INSTALL_DIRS[name].format(revision=revision)
         else:
             install_dir = android_home / INSTALL_DIRS[name]
         if install_dir.exists():
             continue
 
         zipball = get_cachedir() / os.path.basename(url)
         if not zipball.exists():
```

### Comparing `sdkmanager-0.6.4/setup.py` & `sdkmanager-0.6.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,27 +33,27 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='sdkmanager',
-    version='0.6.4',
+    version='0.6.5',
     description='Android SDK Manager',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='The F-Droid Project',
     author_email='team@f-droid.org',
     url='https://gitlab.com/fdroid/sdkmanager',
     license='AGPL-3.0',
     py_modules=['sdkmanager'],
     entry_points={'console_scripts': ['sdkmanager=sdkmanager:main']},
     python_requires='>=3.5',
     cmdclass={'versioncheck': VersionCheckCommand},
-    install_requires=['argcomplete', 'requests > 2.12.2, != 2.18.0'],
+    install_requires=['argcomplete', 'requests > 2.12.2, != 2.18.0', 'urllib3<2'],
     extras_require={'test': ['defusedxml', 'requests-cache']},
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: System Administrators',
         'Intended Audience :: Telecommunications Industry',
```

