# Comparing `tmp/thumbor-piliptc-engine-7.4.7.3.tar.gz` & `tmp/thumbor-piliptc-engine-7.4.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thumbor-piliptc-engine-7.4.7.3.tar", last modified: Mon Mar 13 18:46:11 2023, max compression
+gzip compressed data, was "thumbor-piliptc-engine-7.4.7.4.tar", last modified: Tue May 30 09:55:53 2023, max compression
```

## Comparing `thumbor-piliptc-engine-7.4.7.3.tar` & `thumbor-piliptc-engine-7.4.7.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-03-13 18:46:11.086081 thumbor-piliptc-engine-7.4.7.3/
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)     1075 2023-03-13 18:26:10.000000 thumbor-piliptc-engine-7.4.7.3/LICENSE
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    20470 2023-03-13 18:46:11.090081 thumbor-piliptc-engine-7.4.7.3/PKG-INFO
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    19205 2023-03-13 18:25:18.000000 thumbor-piliptc-engine-7.4.7.3/README.md
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      382 2023-03-13 17:39:34.000000 thumbor-piliptc-engine-7.4.7.3/pyproject.toml
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      314 2023-03-13 18:46:11.090081 thumbor-piliptc-engine-7.4.7.3/setup.cfg
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)     2507 2023-03-13 18:38:23.000000 thumbor-piliptc-engine-7.4.7.3/setup.py
-drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-03-13 18:46:11.086081 thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine/
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      331 2023-03-09 17:55:07.000000 thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine/__init__.py
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    20803 2023-03-13 18:45:58.000000 thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine/engine.py
-drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-03-13 18:46:11.086081 thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine.egg-info/
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    20470 2023-03-13 18:46:11.000000 thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine.egg-info/PKG-INFO
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      348 2023-03-13 18:46:11.000000 thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine.egg-info/SOURCES.txt
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)        1 2023-03-13 18:46:11.000000 thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine.egg-info/dependency_links.txt
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      120 2023-03-13 18:46:11.000000 thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine.egg-info/requires.txt
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)       23 2023-03-13 18:46:11.000000 thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine.egg-info/top_level.txt
+drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-05-30 09:55:53.681309 thumbor-piliptc-engine-7.4.7.4/
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)     1075 2023-03-13 18:53:30.000000 thumbor-piliptc-engine-7.4.7.4/LICENSE
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    19105 2023-05-30 09:55:53.681309 thumbor-piliptc-engine-7.4.7.4/PKG-INFO
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    17840 2023-05-30 09:52:58.000000 thumbor-piliptc-engine-7.4.7.4/README.md
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      382 2023-03-13 18:53:30.000000 thumbor-piliptc-engine-7.4.7.4/pyproject.toml
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      314 2023-05-30 09:55:53.685309 thumbor-piliptc-engine-7.4.7.4/setup.cfg
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)     2507 2023-03-13 18:53:30.000000 thumbor-piliptc-engine-7.4.7.4/setup.py
+drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-05-30 09:55:53.681309 thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine/
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      331 2023-03-09 17:55:07.000000 thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine/__init__.py
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    20803 2023-05-30 09:55:37.000000 thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine/engine.py
+drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-05-30 09:55:53.681309 thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine.egg-info/
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    19105 2023-05-30 09:55:53.000000 thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine.egg-info/PKG-INFO
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      348 2023-05-30 09:55:53.000000 thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine.egg-info/SOURCES.txt
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)        1 2023-05-30 09:55:53.000000 thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine.egg-info/dependency_links.txt
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      120 2023-05-30 09:55:53.000000 thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine.egg-info/requires.txt
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)       23 2023-05-30 09:55:53.000000 thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine.egg-info/top_level.txt
```

### Comparing `thumbor-piliptc-engine-7.4.7.3/LICENSE` & `thumbor-piliptc-engine-7.4.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thumbor-piliptc-engine-7.4.7.3/PKG-INFO` & `thumbor-piliptc-engine-7.4.7.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbor-piliptc-engine
-Version: 7.4.7.3
+Version: 7.4.7.4
 Summary: Pil imaging engine for Thumbor with IPTC data passthrough
 Home-page: https://github.com/gdegoulet/thumbor-piliptc-engine
 Author: Guillaume Degoulet
 Author-email: piliptc@degoulet.net
 License: MIT
 Keywords: thumbor imaging pillow iptc copyright tags
 Classifier: Development Status :: 3 - Alpha
@@ -29,14 +29,16 @@
 Provides-Extra: tests
 License-File: LICENSE
 
 # thumbor-piliptc-engine
 
 thumbor-piliptc-engine is a patched version from the legacy Pil imaging engine for [thumbor](https://github.com/thumbor/thumbor).
 
+Warning : Since [Thumbor release 7.5.0](https://github.com/thumbor/thumbor/releases) , "piliptc" feature is integrated to official thumbor : this project will no more be maintained.
+
 ![](/thumbor-piliptc-engine.png?raw=true)
 
 ## IPTC tags :
 JPEG IPTC (International Press Telecommunications Council) tags are a set of metadata that can be embedded into JPEG image files to provide information about the image content, including ownership and copyright information. These tags can be used by photographers, artists, and publishers to identify their work and protect their intellectual property rights. By including IPTC tags in their JPEG images, creators can ensure that their ownership and copyright information is attached to their work and remains with it as it is shared and distributed across the internet. This can be particularly important for photographers and other creators who rely on their work to generate income, as it can help deter unauthorized use and ensure that they are properly credited for their work. In this way, JPEG IPTC tags can play an essential role in protecting the intellectual property of creators and maintaining the integrity of their work.
 
 
 In Europe, image copyright is protected by various laws and regulations, such as the Berne Convention for the Protection of Literary and Artistic Works and the Directive on the harmonization of certain aspects of copyright and related rights in the information society. These laws provide creators with exclusive rights over their works, including photographs and images, and require that any use of these works by others be authorized or licensed by the creator.
@@ -84,15 +86,15 @@
 
 ```
 docker run --rm -it gdegoulet/thumbor_piliptc_engine:latest      pip list | egrep -i "(thumbor|iptc|jpeg|pillow)"
 JpegIPTC               1.1
 libthumbor             2.0.2
 Pillow                 9.4.0
 thumbor                7.4.7
-thumbor-piliptc-engine 7.4.7
+thumbor-piliptc-engine 7.4.7.3
 thumbor-plugins        0.2.4
 thumbor-plugins-gifv   0.1.2
 thumbor-wand-engine    0.1.1
 
 docker run --rm -it -p8902:8000 \
   -e LOG_LEVEL=DEBUG \
   -e ENGINE=thumbor_piliptc_engine \
@@ -120,64 +122,47 @@
  1:070    Date Sent            Date         8  20230311
 ```
 
 ## Installation
 
 You can install the package from this repository with `pip`:
 
-    $ pip install git+https://github.com/gdegoulet/thumbor-piliptc-engine@v7.4.7.1
+    $ pip install git+https://github.com/gdegoulet/thumbor-piliptc-engine@v7.4.7.3
 
     or
 
-    pip install thumbor-piliptc-engine==7.4.7.1
+    pip install thumbor-piliptc-engine==7.4.7.*
 
 ### Requirements
 -   Python 3.7 or higher
 -   Thumbor (same version than thumbor-piliptc-engine )
 -   git (for now, you can only install from github repository )
--   iptcinfo3 (configured as dependance)
+-   JpegIPTC (configured as dependance)
 
 ```
-root@44171bd2df65:/src# pip install     --no-cache-dir     --prefix="${PYTHONUSERBASE}" git+https://github.com/gdegoulet/thumbor-piliptc-engine
+root@44171bd2df65:/# pip install --no-cache-dir thumbor-piliptc-engine==7.4.7.*
 
-Processing ./thumbor-piliptc-engine
-  Installing build dependencies ... done
-  Getting requirements to build wheel ... done
-  Preparing metadata (pyproject.toml) ... done
-Collecting JpegIPTC@ git+https://github.com/gdegoulet/JpegIPTC@v1.2
-  Cloning https://github.com/gdegoulet/JpegIPTC (to revision v1.2) to /tmp/pip-install-q_46r3la/jpegiptc_ef90d167450740b397ed6774fca992e2
-  Running command git clone --filter=blob:none --quiet https://github.com/gdegoulet/JpegIPTC /tmp/pip-install-q_46r3la/jpegiptc_ef90d167450740b397ed6774fca992e2
-  Resolved https://github.com/gdegoulet/JpegIPTC to commit 88d2433d1eb1e27d3dbe8267cb595d06fb36e092
-  Preparing metadata (setup.py) ... done
-Requirement already satisfied: thumbor>=7.1 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==1.1.0) (7.4.7)
-Requirement already satisfied: pillow>=9.0 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==1.1.0) (9.4.0)
-Requirement already satisfied: colorama==0.*,>=0.4.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (0.4.6)
-Requirement already satisfied: derpconf==0.*,>=0.8.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (0.8.3)
-Requirement already satisfied: libthumbor==2.*,>=2.0.2 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (2.0.2)
-Requirement already satisfied: piexif==1.*,>=1.1.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (1.1.3)
-Requirement already satisfied: pytz>=2019.3.0 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (2022.7.1)
-Requirement already satisfied: statsd==3.*,>=3.3.0 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (3.3.0)
-Requirement already satisfied: tornado==6.*,>=6.0.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (6.2)
-Requirement already satisfied: thumbor-plugins-gifv==0.*,>=0.1.2 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (0.1.2)
-Requirement already satisfied: webcolors==1.*,>=1.10.0 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (1.11.1)
-Requirement already satisfied: six in /app/lib/python3.11/site-packages (from derpconf==0.*,>=0.8.3->thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (1.16.0)
-Building wheels for collected packages: thumbor-piliptc-engine, JpegIPTC
-  Building wheel for thumbor-piliptc-engine (pyproject.toml) ... done
-  Created wheel for thumbor-piliptc-engine: filename=thumbor_piliptc_engine-1.1.0-py3-none-any.whl size=16750 sha256=94a8fc46f363d22a3bd2c1f15989952bcbbde53ec116dc5db9c9a9e262112a57
-  Stored in directory: /tmp/pip-ephem-wheel-cache-tjp9zvzc/wheels/f0/21/40/0e8f20f4be68abb8d80c9cf2fe548f6f3cfd352df72825930c
-  Building wheel for JpegIPTC (setup.py) ... done
-  Created wheel for JpegIPTC: filename=JpegIPTC-1.1-py3-none-any.whl size=7268 sha256=37a3edbbe2c6ab462aa7c65a83ed0e6be7b67f26c09a05c75d591283fb51dbaa
-  Stored in directory: /tmp/pip-ephem-wheel-cache-tjp9zvzc/wheels/c3/f2/e5/05cf3aa7051cf5d7db96fa57f2b7bd453d867f448b016c70c3
-Successfully built thumbor-piliptc-engine JpegIPTC
+Collecting thumbor-piliptc-engine==7.4.7.*
+  Downloading thumbor_piliptc_engine-7.4.7.3-py3-none-any.whl (14 kB)
+Requirement already satisfied: thumbor==7.4.7 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==7.4.7.*) (7.4.7)
+Requirement already satisfied: pillow>=9.0 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==7.4.7.*) (9.4.0)
+Collecting JpegIPTC>=1.4
+  Downloading JpegIPTC-1.4-py3-none-any.whl (9.7 kB)
+Requirement already satisfied: colorama==0.*,>=0.4.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (0.4.6)
+Requirement already satisfied: derpconf==0.*,>=0.8.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (0.8.3)
+Requirement already satisfied: libthumbor==2.*,>=2.0.2 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (2.0.2)
+Requirement already satisfied: piexif==1.*,>=1.1.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (1.1.3)
+Requirement already satisfied: pytz>=2019.3.0 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (2022.7.1)
+Requirement already satisfied: statsd==3.*,>=3.3.0 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (3.3.0)
+Requirement already satisfied: tornado==6.*,>=6.0.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (6.2)
+Requirement already satisfied: thumbor-plugins-gifv==0.*,>=0.1.2 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (0.1.2)
+Requirement already satisfied: webcolors==1.*,>=1.10.0 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (1.11.1)
+Requirement already satisfied: six in /app/lib/python3.11/site-packages (from derpconf==0.*,>=0.8.3->thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (1.16.0)
 Installing collected packages: JpegIPTC, thumbor-piliptc-engine
-  Attempting uninstall: thumbor-piliptc-engine
-    Found existing installation: thumbor-piliptc-engine 0.3.0
-    Uninstalling thumbor-piliptc-engine-0.3.0:
-      Successfully uninstalled thumbor-piliptc-engine-0.3.0
-Successfully installed JpegIPTC-1.1 thumbor-piliptc-engine-1.1.0
+Successfully installed JpegIPTC-1.4 thumbor-piliptc-engine-7.4.7.3
 ```
 
 
 ## Usage
 
 To use this engine with thumbor, define `thumbor_piliptc_engine` as the imaging
 engine in `thumbor.conf`:
```

### Comparing `thumbor-piliptc-engine-7.4.7.3/README.md` & `thumbor-piliptc-engine-7.4.7.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # thumbor-piliptc-engine
 
 thumbor-piliptc-engine is a patched version from the legacy Pil imaging engine for [thumbor](https://github.com/thumbor/thumbor).
 
+Warning : Since [Thumbor release 7.5.0](https://github.com/thumbor/thumbor/releases) , "piliptc" feature is integrated to official thumbor : this project will no more be maintained.
+
 ![](/thumbor-piliptc-engine.png?raw=true)
 
 ## IPTC tags :
 JPEG IPTC (International Press Telecommunications Council) tags are a set of metadata that can be embedded into JPEG image files to provide information about the image content, including ownership and copyright information. These tags can be used by photographers, artists, and publishers to identify their work and protect their intellectual property rights. By including IPTC tags in their JPEG images, creators can ensure that their ownership and copyright information is attached to their work and remains with it as it is shared and distributed across the internet. This can be particularly important for photographers and other creators who rely on their work to generate income, as it can help deter unauthorized use and ensure that they are properly credited for their work. In this way, JPEG IPTC tags can play an essential role in protecting the intellectual property of creators and maintaining the integrity of their work.
 
 
 In Europe, image copyright is protected by various laws and regulations, such as the Berne Convention for the Protection of Literary and Artistic Works and the Directive on the harmonization of certain aspects of copyright and related rights in the information society. These laws provide creators with exclusive rights over their works, including photographs and images, and require that any use of these works by others be authorized or licensed by the creator.
@@ -53,15 +55,15 @@
 
 ```
 docker run --rm -it gdegoulet/thumbor_piliptc_engine:latest      pip list | egrep -i "(thumbor|iptc|jpeg|pillow)"
 JpegIPTC               1.1
 libthumbor             2.0.2
 Pillow                 9.4.0
 thumbor                7.4.7
-thumbor-piliptc-engine 7.4.7
+thumbor-piliptc-engine 7.4.7.3
 thumbor-plugins        0.2.4
 thumbor-plugins-gifv   0.1.2
 thumbor-wand-engine    0.1.1
 
 docker run --rm -it -p8902:8000 \
   -e LOG_LEVEL=DEBUG \
   -e ENGINE=thumbor_piliptc_engine \
@@ -89,64 +91,47 @@
  1:070    Date Sent            Date         8  20230311
 ```
 
 ## Installation
 
 You can install the package from this repository with `pip`:
 
-    $ pip install git+https://github.com/gdegoulet/thumbor-piliptc-engine@v7.4.7.1
+    $ pip install git+https://github.com/gdegoulet/thumbor-piliptc-engine@v7.4.7.3
 
     or
 
-    pip install thumbor-piliptc-engine==7.4.7.1
+    pip install thumbor-piliptc-engine==7.4.7.*
 
 ### Requirements
 -   Python 3.7 or higher
 -   Thumbor (same version than thumbor-piliptc-engine )
 -   git (for now, you can only install from github repository )
--   iptcinfo3 (configured as dependance)
+-   JpegIPTC (configured as dependance)
 
 ```
-root@44171bd2df65:/src# pip install     --no-cache-dir     --prefix="${PYTHONUSERBASE}" git+https://github.com/gdegoulet/thumbor-piliptc-engine
+root@44171bd2df65:/# pip install --no-cache-dir thumbor-piliptc-engine==7.4.7.*
 
-Processing ./thumbor-piliptc-engine
-  Installing build dependencies ... done
-  Getting requirements to build wheel ... done
-  Preparing metadata (pyproject.toml) ... done
-Collecting JpegIPTC@ git+https://github.com/gdegoulet/JpegIPTC@v1.2
-  Cloning https://github.com/gdegoulet/JpegIPTC (to revision v1.2) to /tmp/pip-install-q_46r3la/jpegiptc_ef90d167450740b397ed6774fca992e2
-  Running command git clone --filter=blob:none --quiet https://github.com/gdegoulet/JpegIPTC /tmp/pip-install-q_46r3la/jpegiptc_ef90d167450740b397ed6774fca992e2
-  Resolved https://github.com/gdegoulet/JpegIPTC to commit 88d2433d1eb1e27d3dbe8267cb595d06fb36e092
-  Preparing metadata (setup.py) ... done
-Requirement already satisfied: thumbor>=7.1 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==1.1.0) (7.4.7)
-Requirement already satisfied: pillow>=9.0 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==1.1.0) (9.4.0)
-Requirement already satisfied: colorama==0.*,>=0.4.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (0.4.6)
-Requirement already satisfied: derpconf==0.*,>=0.8.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (0.8.3)
-Requirement already satisfied: libthumbor==2.*,>=2.0.2 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (2.0.2)
-Requirement already satisfied: piexif==1.*,>=1.1.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (1.1.3)
-Requirement already satisfied: pytz>=2019.3.0 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (2022.7.1)
-Requirement already satisfied: statsd==3.*,>=3.3.0 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (3.3.0)
-Requirement already satisfied: tornado==6.*,>=6.0.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (6.2)
-Requirement already satisfied: thumbor-plugins-gifv==0.*,>=0.1.2 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (0.1.2)
-Requirement already satisfied: webcolors==1.*,>=1.10.0 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (1.11.1)
-Requirement already satisfied: six in /app/lib/python3.11/site-packages (from derpconf==0.*,>=0.8.3->thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (1.16.0)
-Building wheels for collected packages: thumbor-piliptc-engine, JpegIPTC
-  Building wheel for thumbor-piliptc-engine (pyproject.toml) ... done
-  Created wheel for thumbor-piliptc-engine: filename=thumbor_piliptc_engine-1.1.0-py3-none-any.whl size=16750 sha256=94a8fc46f363d22a3bd2c1f15989952bcbbde53ec116dc5db9c9a9e262112a57
-  Stored in directory: /tmp/pip-ephem-wheel-cache-tjp9zvzc/wheels/f0/21/40/0e8f20f4be68abb8d80c9cf2fe548f6f3cfd352df72825930c
-  Building wheel for JpegIPTC (setup.py) ... done
-  Created wheel for JpegIPTC: filename=JpegIPTC-1.1-py3-none-any.whl size=7268 sha256=37a3edbbe2c6ab462aa7c65a83ed0e6be7b67f26c09a05c75d591283fb51dbaa
-  Stored in directory: /tmp/pip-ephem-wheel-cache-tjp9zvzc/wheels/c3/f2/e5/05cf3aa7051cf5d7db96fa57f2b7bd453d867f448b016c70c3
-Successfully built thumbor-piliptc-engine JpegIPTC
+Collecting thumbor-piliptc-engine==7.4.7.*
+  Downloading thumbor_piliptc_engine-7.4.7.3-py3-none-any.whl (14 kB)
+Requirement already satisfied: thumbor==7.4.7 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==7.4.7.*) (7.4.7)
+Requirement already satisfied: pillow>=9.0 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==7.4.7.*) (9.4.0)
+Collecting JpegIPTC>=1.4
+  Downloading JpegIPTC-1.4-py3-none-any.whl (9.7 kB)
+Requirement already satisfied: colorama==0.*,>=0.4.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (0.4.6)
+Requirement already satisfied: derpconf==0.*,>=0.8.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (0.8.3)
+Requirement already satisfied: libthumbor==2.*,>=2.0.2 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (2.0.2)
+Requirement already satisfied: piexif==1.*,>=1.1.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (1.1.3)
+Requirement already satisfied: pytz>=2019.3.0 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (2022.7.1)
+Requirement already satisfied: statsd==3.*,>=3.3.0 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (3.3.0)
+Requirement already satisfied: tornado==6.*,>=6.0.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (6.2)
+Requirement already satisfied: thumbor-plugins-gifv==0.*,>=0.1.2 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (0.1.2)
+Requirement already satisfied: webcolors==1.*,>=1.10.0 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (1.11.1)
+Requirement already satisfied: six in /app/lib/python3.11/site-packages (from derpconf==0.*,>=0.8.3->thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (1.16.0)
 Installing collected packages: JpegIPTC, thumbor-piliptc-engine
-  Attempting uninstall: thumbor-piliptc-engine
-    Found existing installation: thumbor-piliptc-engine 0.3.0
-    Uninstalling thumbor-piliptc-engine-0.3.0:
-      Successfully uninstalled thumbor-piliptc-engine-0.3.0
-Successfully installed JpegIPTC-1.1 thumbor-piliptc-engine-1.1.0
+Successfully installed JpegIPTC-1.4 thumbor-piliptc-engine-7.4.7.3
 ```
 
 
 ## Usage
 
 To use this engine with thumbor, define `thumbor_piliptc_engine` as the imaging
 engine in `thumbor.conf`:
```

### Comparing `thumbor-piliptc-engine-7.4.7.3/setup.py` & `thumbor-piliptc-engine-7.4.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine/engine.py` & `thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from thumbor.engines import BaseEngine
 from thumbor.engines.extensions.pil import GifWriter
 from thumbor.filters.fill import Filter
 from thumbor.utils import deprecated, ensure_srgb, get_color_space, logger
 from JpegIPTC import JpegIPTC
 
-__version__ = '7.4.7.3'
+__version__ = '7.4.7.4'
 
 try:
     from thumbor.ext.filters import _composite
 
     FILTERS_AVAILABLE = True
 except ImportError:
     FILTERS_AVAILABLE = False
```

### Comparing `thumbor-piliptc-engine-7.4.7.3/thumbor_piliptc_engine.egg-info/PKG-INFO` & `thumbor-piliptc-engine-7.4.7.4/thumbor_piliptc_engine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbor-piliptc-engine
-Version: 7.4.7.3
+Version: 7.4.7.4
 Summary: Pil imaging engine for Thumbor with IPTC data passthrough
 Home-page: https://github.com/gdegoulet/thumbor-piliptc-engine
 Author: Guillaume Degoulet
 Author-email: piliptc@degoulet.net
 License: MIT
 Keywords: thumbor imaging pillow iptc copyright tags
 Classifier: Development Status :: 3 - Alpha
@@ -29,14 +29,16 @@
 Provides-Extra: tests
 License-File: LICENSE
 
 # thumbor-piliptc-engine
 
 thumbor-piliptc-engine is a patched version from the legacy Pil imaging engine for [thumbor](https://github.com/thumbor/thumbor).
 
+Warning : Since [Thumbor release 7.5.0](https://github.com/thumbor/thumbor/releases) , "piliptc" feature is integrated to official thumbor : this project will no more be maintained.
+
 ![](/thumbor-piliptc-engine.png?raw=true)
 
 ## IPTC tags :
 JPEG IPTC (International Press Telecommunications Council) tags are a set of metadata that can be embedded into JPEG image files to provide information about the image content, including ownership and copyright information. These tags can be used by photographers, artists, and publishers to identify their work and protect their intellectual property rights. By including IPTC tags in their JPEG images, creators can ensure that their ownership and copyright information is attached to their work and remains with it as it is shared and distributed across the internet. This can be particularly important for photographers and other creators who rely on their work to generate income, as it can help deter unauthorized use and ensure that they are properly credited for their work. In this way, JPEG IPTC tags can play an essential role in protecting the intellectual property of creators and maintaining the integrity of their work.
 
 
 In Europe, image copyright is protected by various laws and regulations, such as the Berne Convention for the Protection of Literary and Artistic Works and the Directive on the harmonization of certain aspects of copyright and related rights in the information society. These laws provide creators with exclusive rights over their works, including photographs and images, and require that any use of these works by others be authorized or licensed by the creator.
@@ -84,15 +86,15 @@
 
 ```
 docker run --rm -it gdegoulet/thumbor_piliptc_engine:latest      pip list | egrep -i "(thumbor|iptc|jpeg|pillow)"
 JpegIPTC               1.1
 libthumbor             2.0.2
 Pillow                 9.4.0
 thumbor                7.4.7
-thumbor-piliptc-engine 7.4.7
+thumbor-piliptc-engine 7.4.7.3
 thumbor-plugins        0.2.4
 thumbor-plugins-gifv   0.1.2
 thumbor-wand-engine    0.1.1
 
 docker run --rm -it -p8902:8000 \
   -e LOG_LEVEL=DEBUG \
   -e ENGINE=thumbor_piliptc_engine \
@@ -120,64 +122,47 @@
  1:070    Date Sent            Date         8  20230311
 ```
 
 ## Installation
 
 You can install the package from this repository with `pip`:
 
-    $ pip install git+https://github.com/gdegoulet/thumbor-piliptc-engine@v7.4.7.1
+    $ pip install git+https://github.com/gdegoulet/thumbor-piliptc-engine@v7.4.7.3
 
     or
 
-    pip install thumbor-piliptc-engine==7.4.7.1
+    pip install thumbor-piliptc-engine==7.4.7.*
 
 ### Requirements
 -   Python 3.7 or higher
 -   Thumbor (same version than thumbor-piliptc-engine )
 -   git (for now, you can only install from github repository )
--   iptcinfo3 (configured as dependance)
+-   JpegIPTC (configured as dependance)
 
 ```
-root@44171bd2df65:/src# pip install     --no-cache-dir     --prefix="${PYTHONUSERBASE}" git+https://github.com/gdegoulet/thumbor-piliptc-engine
+root@44171bd2df65:/# pip install --no-cache-dir thumbor-piliptc-engine==7.4.7.*
 
-Processing ./thumbor-piliptc-engine
-  Installing build dependencies ... done
-  Getting requirements to build wheel ... done
-  Preparing metadata (pyproject.toml) ... done
-Collecting JpegIPTC@ git+https://github.com/gdegoulet/JpegIPTC@v1.2
-  Cloning https://github.com/gdegoulet/JpegIPTC (to revision v1.2) to /tmp/pip-install-q_46r3la/jpegiptc_ef90d167450740b397ed6774fca992e2
-  Running command git clone --filter=blob:none --quiet https://github.com/gdegoulet/JpegIPTC /tmp/pip-install-q_46r3la/jpegiptc_ef90d167450740b397ed6774fca992e2
-  Resolved https://github.com/gdegoulet/JpegIPTC to commit 88d2433d1eb1e27d3dbe8267cb595d06fb36e092
-  Preparing metadata (setup.py) ... done
-Requirement already satisfied: thumbor>=7.1 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==1.1.0) (7.4.7)
-Requirement already satisfied: pillow>=9.0 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==1.1.0) (9.4.0)
-Requirement already satisfied: colorama==0.*,>=0.4.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (0.4.6)
-Requirement already satisfied: derpconf==0.*,>=0.8.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (0.8.3)
-Requirement already satisfied: libthumbor==2.*,>=2.0.2 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (2.0.2)
-Requirement already satisfied: piexif==1.*,>=1.1.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (1.1.3)
-Requirement already satisfied: pytz>=2019.3.0 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (2022.7.1)
-Requirement already satisfied: statsd==3.*,>=3.3.0 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (3.3.0)
-Requirement already satisfied: tornado==6.*,>=6.0.3 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (6.2)
-Requirement already satisfied: thumbor-plugins-gifv==0.*,>=0.1.2 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (0.1.2)
-Requirement already satisfied: webcolors==1.*,>=1.10.0 in /app/lib/python3.11/site-packages (from thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (1.11.1)
-Requirement already satisfied: six in /app/lib/python3.11/site-packages (from derpconf==0.*,>=0.8.3->thumbor>=7.1->thumbor-piliptc-engine==1.1.0) (1.16.0)
-Building wheels for collected packages: thumbor-piliptc-engine, JpegIPTC
-  Building wheel for thumbor-piliptc-engine (pyproject.toml) ... done
-  Created wheel for thumbor-piliptc-engine: filename=thumbor_piliptc_engine-1.1.0-py3-none-any.whl size=16750 sha256=94a8fc46f363d22a3bd2c1f15989952bcbbde53ec116dc5db9c9a9e262112a57
-  Stored in directory: /tmp/pip-ephem-wheel-cache-tjp9zvzc/wheels/f0/21/40/0e8f20f4be68abb8d80c9cf2fe548f6f3cfd352df72825930c
-  Building wheel for JpegIPTC (setup.py) ... done
-  Created wheel for JpegIPTC: filename=JpegIPTC-1.1-py3-none-any.whl size=7268 sha256=37a3edbbe2c6ab462aa7c65a83ed0e6be7b67f26c09a05c75d591283fb51dbaa
-  Stored in directory: /tmp/pip-ephem-wheel-cache-tjp9zvzc/wheels/c3/f2/e5/05cf3aa7051cf5d7db96fa57f2b7bd453d867f448b016c70c3
-Successfully built thumbor-piliptc-engine JpegIPTC
+Collecting thumbor-piliptc-engine==7.4.7.*
+  Downloading thumbor_piliptc_engine-7.4.7.3-py3-none-any.whl (14 kB)
+Requirement already satisfied: thumbor==7.4.7 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==7.4.7.*) (7.4.7)
+Requirement already satisfied: pillow>=9.0 in /app/lib/python3.11/site-packages (from thumbor-piliptc-engine==7.4.7.*) (9.4.0)
+Collecting JpegIPTC>=1.4
+  Downloading JpegIPTC-1.4-py3-none-any.whl (9.7 kB)
+Requirement already satisfied: colorama==0.*,>=0.4.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (0.4.6)
+Requirement already satisfied: derpconf==0.*,>=0.8.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (0.8.3)
+Requirement already satisfied: libthumbor==2.*,>=2.0.2 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (2.0.2)
+Requirement already satisfied: piexif==1.*,>=1.1.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (1.1.3)
+Requirement already satisfied: pytz>=2019.3.0 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (2022.7.1)
+Requirement already satisfied: statsd==3.*,>=3.3.0 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (3.3.0)
+Requirement already satisfied: tornado==6.*,>=6.0.3 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (6.2)
+Requirement already satisfied: thumbor-plugins-gifv==0.*,>=0.1.2 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (0.1.2)
+Requirement already satisfied: webcolors==1.*,>=1.10.0 in /app/lib/python3.11/site-packages (from thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (1.11.1)
+Requirement already satisfied: six in /app/lib/python3.11/site-packages (from derpconf==0.*,>=0.8.3->thumbor==7.4.7->thumbor-piliptc-engine==7.4.7.*) (1.16.0)
 Installing collected packages: JpegIPTC, thumbor-piliptc-engine
-  Attempting uninstall: thumbor-piliptc-engine
-    Found existing installation: thumbor-piliptc-engine 0.3.0
-    Uninstalling thumbor-piliptc-engine-0.3.0:
-      Successfully uninstalled thumbor-piliptc-engine-0.3.0
-Successfully installed JpegIPTC-1.1 thumbor-piliptc-engine-1.1.0
+Successfully installed JpegIPTC-1.4 thumbor-piliptc-engine-7.4.7.3
 ```
 
 
 ## Usage
 
 To use this engine with thumbor, define `thumbor_piliptc_engine` as the imaging
 engine in `thumbor.conf`:
```

