# Comparing `tmp/guanine-crystal-analysis-0.0.1.tar.gz` & `tmp/guanine-crystal-analysis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guanine-crystal-analysis-0.0.1.tar", last modified: Tue Jul 26 15:14:07 2022, max compression
+gzip compressed data, was "guanine-crystal-analysis-0.0.2.tar", last modified: Tue May 30 13:54:27 2023, max compression
```

## Comparing `guanine-crystal-analysis-0.0.1.tar` & `guanine-crystal-analysis-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 mara       (501) staff       (20)        0 2022-07-26 15:14:07.100365 guanine-crystal-analysis-0.0.1/
--rw-r--r--   0 mara       (501) staff       (20)     1495 2022-07-19 13:24:00.000000 guanine-crystal-analysis-0.0.1/LICENSE
--rw-r--r--   0 mara       (501) staff       (20)       96 2022-07-19 13:24:00.000000 guanine-crystal-analysis-0.0.1/MANIFEST.in
--rw-r--r--   0 mara       (501) staff       (20)     4202 2022-07-26 15:14:07.100634 guanine-crystal-analysis-0.0.1/PKG-INFO
--rw-r--r--   0 mara       (501) staff       (20)     2830 2022-07-19 13:30:56.000000 guanine-crystal-analysis-0.0.1/README.md
--rw-r--r--   0 mara       (501) staff       (20)      180 2022-07-19 13:24:00.000000 guanine-crystal-analysis-0.0.1/pyproject.toml
--rw-r--r--   0 mara       (501) staff       (20)     1967 2022-07-26 15:14:07.102005 guanine-crystal-analysis-0.0.1/setup.cfg
--rw-r--r--   0 mara       (501) staff       (20)       83 2022-07-26 15:09:22.000000 guanine-crystal-analysis-0.0.1/setup.py
-drwxr-xr-x   0 mara       (501) staff       (20)        0 2022-07-26 15:14:07.079768 guanine-crystal-analysis-0.0.1/src/
-drwxr-xr-x   0 mara       (501) staff       (20)        0 2022-07-26 15:14:07.086959 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/
--rw-r--r--   0 mara       (501) staff       (20)      103 2022-07-19 13:38:43.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/__init__.py
--rw-r--r--   0 mara       (501) staff       (20)      630 2022-07-19 13:24:00.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/_sample_data.py
-drwxr-xr-x   0 mara       (501) staff       (20)        0 2022-07-26 15:14:07.092054 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/_tests/
--rw-r--r--   0 mara       (501) staff       (20)        0 2022-07-19 13:24:00.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/_tests/__init__.py
--rw-r--r--   0 mara       (501) staff       (20)      115 2022-07-19 13:24:00.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/_tests/test_sample_data.py
--rw-r--r--   0 mara       (501) staff       (20)     1257 2022-07-19 13:24:00.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/_tests/test_widget.py
--rw-r--r--   0 mara       (501) staff       (20)     8288 2022-07-26 14:31:01.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/_widget.py
-drwxr-xr-x   0 mara       (501) staff       (20)        0 2022-07-26 15:14:07.098038 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_classifier/
--rw-r--r--   0 mara       (501) staff       (20)        0 2022-07-26 15:12:50.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_classifier/__init__.py
--rw-r--r--   0 mara       (501) staff       (20)     2832 2022-07-25 13:45:42.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_intensity.cl
--rw-r--r--   0 mara       (501) staff       (20)     3957 2022-07-25 13:46:04.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_shape.cl
--rw-r--r--   0 mara       (501) staff       (20)     3957 2022-07-25 13:46:18.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_shape_intensity.cl
--rw-r--r--   0 mara       (501) staff       (20)     2236 2022-07-25 13:46:00.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_size.cl
--rw-r--r--   0 mara       (501) staff       (20)     2942 2022-07-25 13:46:09.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_size_intensity.cl
--rw-r--r--   0 mara       (501) staff       (20)     3540 2022-07-25 13:46:14.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_size_shape.cl
--rw-r--r--   0 mara       (501) staff       (20)     4145 2022-07-25 13:46:23.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_size_shape_intensity.cl
-drwxr-xr-x   0 mara       (501) staff       (20)        0 2022-07-26 15:14:07.099244 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_segmenter/
--rw-r--r--   0 mara       (501) staff       (20)        0 2022-07-26 15:13:58.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_segmenter/__init__.py
--rw-r--r--   0 mara       (501) staff       (20)    29714 2022-07-19 13:52:26.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/cl_segmenter/object_segmenter_20220523_sorted.cl
--rw-r--r--   0 mara       (501) staff       (20)     1823 2022-07-26 14:27:55.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/napari.yaml
-drwxr-xr-x   0 mara       (501) staff       (20)        0 2022-07-26 15:14:07.090475 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis.egg-info/
--rw-r--r--   0 mara       (501) staff       (20)     4202 2022-07-26 15:14:06.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis.egg-info/PKG-INFO
--rw-r--r--   0 mara       (501) staff       (20)     1481 2022-07-26 15:14:07.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 mara       (501) staff       (20)        1 2022-07-26 15:14:06.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 mara       (501) staff       (20)       82 2022-07-26 15:14:06.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis.egg-info/entry_points.txt
--rw-r--r--   0 mara       (501) staff       (20)      216 2022-07-26 15:14:06.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis.egg-info/requires.txt
--rw-r--r--   0 mara       (501) staff       (20)       25 2022-07-26 15:14:06.000000 guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 13:54:27.734406 guanine-crystal-analysis-0.0.2/
+-rw-rw-rw-   0        0        0     1523 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9511 2023-05-30 13:54:27.734406 guanine-crystal-analysis-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8110 2023-05-30 13:48:40.000000 guanine-crystal-analysis-0.0.2/README.md
+-rw-rw-rw-   0        0        0      192 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     2039 2023-05-30 13:54:27.744352 guanine-crystal-analysis-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       87 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:54:27.447596 guanine-crystal-analysis-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 13:54:27.628588 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/
+-rw-rw-rw-   0        0        0      386 2023-05-30 13:51:21.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/_sample_data.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:54:27.673930 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/_tests/
+-rw-rw-rw-   0        0        0        0 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/_tests/__init__.py
+-rw-rw-rw-   0        0        0      122 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/_tests/test_sample_data.py
+-rw-rw-rw-   0        0        0     1293 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     8683 2023-02-15 12:57:21.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/_widget.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:54:27.724404 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_classifier/
+-rw-rw-rw-   0        0        0        0 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_classifier/__init__.py
+-rw-rw-rw-   0        0        0     2996 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_intensity.cl
+-rw-rw-rw-   0        0        0     4134 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_shape.cl
+-rw-rw-rw-   0        0        0     4134 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_shape_intensity.cl
+-rw-rw-rw-   0        0        0     2414 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_size.cl
+-rw-rw-rw-   0        0        0     3112 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_size_intensity.cl
+-rw-rw-rw-   0        0        0     3723 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_size_shape.cl
+-rw-rw-rw-   0        0        0     4330 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_classifier/object_classifier_20220523_size_shape_intensity.cl
+drwxrwxrwx   0        0        0        0 2023-05-30 13:54:27.733408 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_segmenter/
+-rw-rw-rw-   0        0        0        0 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_segmenter/__init__.py
+-rw-rw-rw-   0        0        0    31850 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/cl_segmenter/object_segmenter_20220523_sorted.cl
+-rw-rw-rw-   0        0        0     1867 2023-01-18 15:12:04.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/napari.yaml
+drwxrwxrwx   0        0        0        0 2023-05-30 13:54:27.656971 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis.egg-info/
+-rw-rw-rw-   0        0        0     9511 2023-05-30 13:54:27.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2023-05-30 13:54:27.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:54:27.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-05-30 13:54:27.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      216 2023-05-30 13:54:27.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-30 13:54:27.000000 guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis.egg-info/top_level.txt
```

### Comparing `guanine-crystal-analysis-0.0.1/LICENSE` & `guanine-crystal-analysis-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-
-Copyright (c) 2022, Mara Lampert
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of guanine-crystal-analysis nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+Copyright (c) 2022, Mara Lampert
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of guanine-crystal-analysis nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `guanine-crystal-analysis-0.0.1/setup.cfg` & `guanine-crystal-analysis-0.0.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,128 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6775 616e 696e 652d 6372 7973 7461  = guanine-crysta
-00000020: 6c2d 616e 616c 7973 6973 0a76 6572 7369  l-analysis.versi
-00000030: 6f6e 203d 2030 2e30 2e31 0a64 6573 6372  on = 0.0.1.descr
-00000040: 6970 7469 6f6e 203d 2041 2070 6c75 6769  iption = A plugi
-00000050: 6e20 666f 7220 7468 6520 6775 616e 696e  n for the guanin
-00000060: 6520 6372 7973 7461 6c20 7365 676d 656e  e crystal segmen
-00000070: 7461 7469 6f6e 2c20 636c 6173 7369 6669  tation, classifi
-00000080: 6361 7469 6f6e 2061 6e64 2063 6861 7261  cation and chara
-00000090: 6374 6572 697a 6174 696f 6e20 696e 2074  cterization in t
-000000a0: 6865 207a 6562 7261 6669 7368 2065 7965  he zebrafish eye
-000000b0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000c0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-000000d0: 2e6d 640a 6c6f 6e67 5f64 6573 6372 6970  .md.long_descrip
-000000e0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-000000f0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000100: 6e0a 7572 6c20 3d20 6874 7470 733a 2f2f  n.url = https://
-00000110: 6769 7468 7562 2e63 6f6d 2f62 6961 706f  github.com/biapo
-00000120: 6c2f 6775 616e 696e 652d 6372 7973 7461  l/guanine-crysta
-00000130: 6c2d 616e 616c 7973 6973 0a61 7574 686f  l-analysis.autho
-00000140: 7220 3d20 4d61 7261 204c 616d 7065 7274  r = Mara Lampert
-00000150: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-00000160: 6d61 7261 5f68 6172 7269 6574 2e6c 616d  mara_harriet.lam
-00000170: 7065 7274 406d 6169 6c62 6f78 2e74 752d  pert@mailbox.tu-
-00000180: 6472 6573 6465 6e2e 6465 0a6c 6963 656e  dresden.de.licen
-00000190: 7365 203d 2042 5344 2d33 2d43 6c61 7573  se = BSD-3-Claus
-000001a0: 650a 6c69 6365 6e73 655f 6669 6c65 7320  e.license_files 
-000001b0: 3d20 4c49 4345 4e53 450a 636c 6173 7369  = LICENSE.classi
-000001c0: 6669 6572 7320 3d20 0a09 4465 7665 6c6f  fiers = ..Develo
-000001d0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-000001e0: 3220 2d20 5072 652d 416c 7068 610a 0946  2 - Pre-Alpha..F
-000001f0: 7261 6d65 776f 726b 203a 3a20 6e61 7061  ramework :: napa
-00000200: 7269 0a09 496e 7465 6e64 6564 2041 7564  ri..Intended Aud
-00000210: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000220: 6572 730a 094c 6963 656e 7365 203a 3a20  ers..License :: 
-00000230: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000240: 4253 4420 4c69 6365 6e73 650a 094f 7065  BSD License..Ope
-00000250: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000260: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
-00000270: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000280: 6775 6167 6520 3a3a 2050 7974 686f 6e0a  guage :: Python.
-00000290: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002b0: 3a3a 2033 0a09 5072 6f67 7261 6d6d 696e  :: 3..Programmin
-000002c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002d0: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-000002e0: 790a 0950 726f 6772 616d 6d69 6e67 204c  y..Programming L
-000002f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000300: 6e20 3a3a 2033 2e38 0a09 5072 6f67 7261  n :: 3.8..Progra
-00000310: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
-00000330: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000340: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000350: 3a3a 2033 2e31 300a 0954 6f70 6963 203a  :: 3.10..Topic :
-00000360: 3a20 5363 6965 6e74 6966 6963 2f45 6e67  : Scientific/Eng
-00000370: 696e 6565 7269 6e67 203a 3a20 496d 6167  ineering :: Imag
-00000380: 6520 5072 6f63 6573 7369 6e67 0a70 726f  e Processing.pro
-00000390: 6a65 6374 5f75 726c 7320 3d20 0a09 4275  ject_urls = ..Bu
-000003a0: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
-000003b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-000003c0: 6961 706f 6c2f 6775 616e 696e 652d 6372  iapol/guanine-cr
-000003d0: 7973 7461 6c2d 616e 616c 7973 6973 2f69  ystal-analysis/i
-000003e0: 7373 7565 730a 0944 6f63 756d 656e 7461  ssues..Documenta
-000003f0: 7469 6f6e 203d 2068 7474 7073 3a2f 2f67  tion = https://g
-00000400: 6974 6875 622e 636f 6d2f 6269 6170 6f6c  ithub.com/biapol
-00000410: 2f67 7561 6e69 6e65 2d63 7279 7374 616c  /guanine-crystal
-00000420: 2d61 6e61 6c79 7369 7323 5245 4144 4d45  -analysis#README
-00000430: 2e6d 640a 0953 6f75 7263 6520 436f 6465  .md..Source Code
-00000440: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000450: 622e 636f 6d2f 6269 6170 6f6c 2f67 7561  b.com/biapol/gua
-00000460: 6e69 6e65 2d63 7279 7374 616c 2d61 6e61  nine-crystal-ana
-00000470: 6c79 7369 730a 0955 7365 7220 5375 7070  lysis..User Supp
-00000480: 6f72 7420 3d20 6874 7470 733a 2f2f 6769  ort = https://gi
-00000490: 7468 7562 2e63 6f6d 2f62 6961 706f 6c2f  thub.com/biapol/
-000004a0: 6775 616e 696e 652d 6372 7973 7461 6c2d  guanine-crystal-
-000004b0: 616e 616c 7973 6973 2f69 7373 7565 730a  analysis/issues.
-000004c0: 0a5b 6f70 7469 6f6e 735d 0a70 6163 6b61  .[options].packa
-000004d0: 6765 7320 3d20 6669 6e64 3a0a 696e 7374  ges = find:.inst
-000004e0: 616c 6c5f 7265 7175 6972 6573 203d 200a  all_requires = .
-000004f0: 096e 756d 7079 0a09 6d61 6769 6367 7569  .numpy..magicgui
-00000500: 0a09 7174 7079 0a09 6170 6f63 0a09 7363  ..qtpy..apoc..sc
-00000510: 696b 6974 2d69 6d61 6765 0a09 7061 6e64  ikit-image..pand
-00000520: 6173 0a09 6e61 7061 7269 2d73 696d 706c  as..napari-simpl
-00000530: 6569 746b 2d69 6d61 6765 2d70 726f 6365  eitk-image-proce
-00000540: 7373 696e 670a 096e 6170 6172 692d 736b  ssing..napari-sk
-00000550: 696d 6167 652d 7265 6769 6f6e 7072 6f70  image-regionprop
-00000560: 730a 0970 7963 6c65 7370 6572 616e 746f  s..pyclesperanto
-00000570: 2d70 726f 746f 7479 7065 0a09 7363 696b  -prototype..scik
-00000580: 6974 2d6c 6561 726e 0a09 6e61 7061 7269  it-learn..napari
-00000590: 2d77 6f72 6b66 6c6f 7773 0a70 7974 686f  -workflows.pytho
-000005a0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000005b0: 2e38 0a69 6e63 6c75 6465 5f70 6163 6b61  .8.include_packa
-000005c0: 6765 5f64 6174 6120 3d20 5472 7565 0a70  ge_data = True.p
-000005d0: 6163 6b61 6765 5f64 6972 203d 200a 093d  ackage_dir = ..=
-000005e0: 7372 630a 0a5b 6f70 7469 6f6e 732e 7061  src..[options.pa
-000005f0: 636b 6167 6573 2e66 696e 645d 0a77 6865  ckages.find].whe
-00000600: 7265 203d 2073 7263 0a0a 5b6f 7074 696f  re = src..[optio
-00000610: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000620: 0a6e 6170 6172 692e 6d61 6e69 6665 7374  .napari.manifest
-00000630: 203d 200a 0967 7561 6e69 6e65 2d63 7279   = ..guanine-cry
-00000640: 7374 616c 2d61 6e61 6c79 7369 7320 3d20  stal-analysis = 
-00000650: 6775 616e 696e 655f 6372 7973 7461 6c5f  guanine_crystal_
-00000660: 616e 616c 7973 6973 3a6e 6170 6172 692e  analysis:napari.
-00000670: 7961 6d6c 0a0a 5b6f 7074 696f 6e73 2e65  yaml..[options.e
-00000680: 7874 7261 735f 7265 7175 6972 655d 0a74  xtras_require].t
-00000690: 6573 7469 6e67 203d 200a 0974 6f78 0a09  esting = ..tox..
-000006a0: 7079 7465 7374 2020 2320 6874 7470 733a  pytest  # https:
-000006b0: 2f2f 646f 6373 2e70 7974 6573 742e 6f72  //docs.pytest.or
-000006c0: 672f 656e 2f6c 6174 6573 742f 636f 6e74  g/en/latest/cont
-000006d0: 656e 7473 2e68 746d 6c0a 0970 7974 6573  ents.html..pytes
-000006e0: 742d 636f 7620 2023 2068 7474 7073 3a2f  t-cov  # https:/
-000006f0: 2f70 7974 6573 742d 636f 762e 7265 6164  /pytest-cov.read
-00000700: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000710: 7465 7374 2f0a 0970 7974 6573 742d 7174  test/..pytest-qt
-00000720: 2020 2320 6874 7470 733a 2f2f 7079 7465    # https://pyte
-00000730: 7374 2d71 742e 7265 6164 7468 6564 6f63  st-qt.readthedoc
-00000740: 732e 696f 2f65 6e2f 6c61 7465 7374 2f0a  s.io/en/latest/.
-00000750: 096e 6170 6172 690a 0970 7971 7435 0a0a  .napari..pyqt5..
-00000760: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000770: 5f64 6174 615d 0a2a 203d 202a 2e79 616d  _data].* = *.yam
-00000780: 6c2c 202a 2e63 6c0a 0a5b 6567 675f 696e  l, *.cl..[egg_in
-00000790: 666f 5d0a 7461 675f 6275 696c 6420 3d20  fo].tag_build = 
-000007a0: 0a74 6167 5f64 6174 6520 3d20 300a 0a    .tag_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2067 7561 6e69 6e65 2d63 7279 7374   = guanine-cryst
+00000020: 616c 2d61 6e61 6c79 7369 730d 0a76 6572  al-analysis..ver
+00000030: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6465  sion = 0.0.2..de
+00000040: 7363 7269 7074 696f 6e20 3d20 4120 706c  scription = A pl
+00000050: 7567 696e 2066 6f72 2074 6865 2067 7561  ugin for the gua
+00000060: 6e69 6e65 2063 7279 7374 616c 2073 6567  nine crystal seg
+00000070: 6d65 6e74 6174 696f 6e2c 2063 6c61 7373  mentation, class
+00000080: 6966 6963 6174 696f 6e20 616e 6420 6368  ification and ch
+00000090: 6172 6163 7465 7269 7a61 7469 6f6e 2069  aracterization i
+000000a0: 6e20 7468 6520 7a65 6272 6166 6973 6820  n the zebrafish 
+000000b0: 6579 650d 0a6c 6f6e 675f 6465 7363 7269  eye..long_descri
+000000c0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
+000000d0: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
+000000e0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
+000000f0: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
+00000100: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
+00000110: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000120: 2f62 6961 706f 6c2f 6775 616e 696e 652d  /biapol/guanine-
+00000130: 6372 7973 7461 6c2d 616e 616c 7973 6973  crystal-analysis
+00000140: 0d0a 6175 7468 6f72 203d 204d 6172 6120  ..author = Mara 
+00000150: 4c61 6d70 6572 740d 0a61 7574 686f 725f  Lampert..author_
+00000160: 656d 6169 6c20 3d20 6d61 7261 5f68 6172  email = mara_har
+00000170: 7269 6574 2e6c 616d 7065 7274 406d 6169  riet.lampert@mai
+00000180: 6c62 6f78 2e74 752d 6472 6573 6465 6e2e  lbox.tu-dresden.
+00000190: 6465 0d0a 6c69 6365 6e73 6520 3d20 4253  de..license = BS
+000001a0: 442d 332d 436c 6175 7365 0d0a 6c69 6365  D-3-Clause..lice
+000001b0: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
+000001c0: 4e53 450d 0a63 6c61 7373 6966 6965 7273  NSE..classifiers
+000001d0: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
+000001e0: 7420 5374 6174 7573 203a 3a20 3220 2d20  t Status :: 2 - 
+000001f0: 5072 652d 416c 7068 610d 0a09 4672 616d  Pre-Alpha...Fram
+00000200: 6577 6f72 6b20 3a3a 206e 6170 6172 690d  ework :: napari.
+00000210: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+00000220: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+00000230: 730d 0a09 4c69 6365 6e73 6520 3a3a 204f  s...License :: O
+00000240: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
+00000250: 5344 204c 6963 656e 7365 0d0a 094f 7065  SD License...Ope
+00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000270: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000280: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002a0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002c0: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
+000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002e0: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
+000002f0: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
+00000300: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000310: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
+00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000340: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
+00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000360: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+00000370: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
+00000380: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
+00000390: 3a3a 2049 6d61 6765 2050 726f 6365 7373  :: Image Process
+000003a0: 696e 670d 0a70 726f 6a65 6374 5f75 726c  ing..project_url
+000003b0: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
+000003c0: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
+000003d0: 6875 622e 636f 6d2f 6269 6170 6f6c 2f67  hub.com/biapol/g
+000003e0: 7561 6e69 6e65 2d63 7279 7374 616c 2d61  uanine-crystal-a
+000003f0: 6e61 6c79 7369 732f 6973 7375 6573 0d0a  nalysis/issues..
+00000400: 0944 6f63 756d 656e 7461 7469 6f6e 203d  .Documentation =
+00000410: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000420: 636f 6d2f 6269 6170 6f6c 2f67 7561 6e69  com/biapol/guani
+00000430: 6e65 2d63 7279 7374 616c 2d61 6e61 6c79  ne-crystal-analy
+00000440: 7369 7323 5245 4144 4d45 2e6d 640d 0a09  sis#README.md...
+00000450: 536f 7572 6365 2043 6f64 6520 3d20 6874  Source Code = ht
+00000460: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000470: 2f62 6961 706f 6c2f 6775 616e 696e 652d  /biapol/guanine-
+00000480: 6372 7973 7461 6c2d 616e 616c 7973 6973  crystal-analysis
+00000490: 0d0a 0955 7365 7220 5375 7070 6f72 7420  ...User Support 
+000004a0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000004b0: 2e63 6f6d 2f62 6961 706f 6c2f 6775 616e  .com/biapol/guan
+000004c0: 696e 652d 6372 7973 7461 6c2d 616e 616c  ine-crystal-anal
+000004d0: 7973 6973 2f69 7373 7565 730d 0a0d 0a5b  ysis/issues....[
+000004e0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+000004f0: 6573 203d 2066 696e 643a 0d0a 696e 7374  es = find:..inst
+00000500: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000510: 0a09 6e75 6d70 790d 0a09 6d61 6769 6367  ..numpy...magicg
+00000520: 7569 0d0a 0971 7470 790d 0a09 6170 6f63  ui...qtpy...apoc
+00000530: 0d0a 0973 6369 6b69 742d 696d 6167 650d  ...scikit-image.
+00000540: 0a09 7061 6e64 6173 0d0a 096e 6170 6172  ..pandas...napar
+00000550: 692d 7369 6d70 6c65 6974 6b2d 696d 6167  i-simpleitk-imag
+00000560: 652d 7072 6f63 6573 7369 6e67 0d0a 096e  e-processing...n
+00000570: 6170 6172 692d 736b 696d 6167 652d 7265  apari-skimage-re
+00000580: 6769 6f6e 7072 6f70 730d 0a09 7079 636c  gionprops...pycl
+00000590: 6573 7065 7261 6e74 6f2d 7072 6f74 6f74  esperanto-protot
+000005a0: 7970 650d 0a09 7363 696b 6974 2d6c 6561  ype...scikit-lea
+000005b0: 726e 0d0a 096e 6170 6172 692d 776f 726b  rn...napari-work
+000005c0: 666c 6f77 730d 0a70 7974 686f 6e5f 7265  flows..python_re
+000005d0: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
+000005e0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+000005f0: 6461 7461 203d 2054 7275 650d 0a70 6163  data = True..pac
+00000600: 6b61 6765 5f64 6972 203d 200d 0a09 3d73  kage_dir = ...=s
+00000610: 7263 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  rc....[options.p
+00000620: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000630: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
+00000640: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
+00000650: 6e74 735d 0d0a 6e61 7061 7269 2e6d 616e  nts]..napari.man
+00000660: 6966 6573 7420 3d20 0d0a 0967 7561 6e69  ifest = ...guani
+00000670: 6e65 2d63 7279 7374 616c 2d61 6e61 6c79  ne-crystal-analy
+00000680: 7369 7320 3d20 6775 616e 696e 655f 6372  sis = guanine_cr
+00000690: 7973 7461 6c5f 616e 616c 7973 6973 3a6e  ystal_analysis:n
+000006a0: 6170 6172 692e 7961 6d6c 0d0a 0d0a 5b6f  apari.yaml....[o
+000006b0: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
+000006c0: 7175 6972 655d 0d0a 7465 7374 696e 6720  quire]..testing 
+000006d0: 3d20 0d0a 0974 6f78 0d0a 0970 7974 6573  = ...tox...pytes
+000006e0: 7420 2023 2068 7474 7073 3a2f 2f64 6f63  t  # https://doc
+000006f0: 732e 7079 7465 7374 2e6f 7267 2f65 6e2f  s.pytest.org/en/
+00000700: 6c61 7465 7374 2f63 6f6e 7465 6e74 732e  latest/contents.
+00000710: 6874 6d6c 0d0a 0970 7974 6573 742d 636f  html...pytest-co
+00000720: 7620 2023 2068 7474 7073 3a2f 2f70 7974  v  # https://pyt
+00000730: 6573 742d 636f 762e 7265 6164 7468 6564  est-cov.readthed
+00000740: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000750: 2f0d 0a09 7079 7465 7374 2d71 7420 2023  /...pytest-qt  #
+00000760: 2068 7474 7073 3a2f 2f70 7974 6573 742d   https://pytest-
+00000770: 7174 2e72 6561 6474 6865 646f 6373 2e69  qt.readthedocs.i
+00000780: 6f2f 656e 2f6c 6174 6573 742f 0d0a 096e  o/en/latest/...n
+00000790: 6170 6172 690d 0a09 7079 7174 350d 0a0d  apari...pyqt5...
+000007a0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+000007b0: 655f 6461 7461 5d0d 0a2a 203d 202a 2e79  e_data]..* = *.y
+000007c0: 616d 6c2c 202a 2e63 6c0d 0a0d 0a5b 6567  aml, *.cl....[eg
+000007d0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000007e0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000007f0: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/_sample_data.py` & `guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/_sample_data.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""
-This module is an example of a barebones sample data provider for napari.
-
-It implements the "sample data" specification.
-see: https://napari.org/plugins/guides.html?#sample-data
-
-Replace code below according to your needs.
-"""
-from __future__ import annotations
-
-import numpy
-
-
-def make_sample_data():
-    """Generates an image"""
-    # Return list of tuples
-    # [(data1, add_image_kwargs1), (data2, add_image_kwargs2)]
-    # Check the documentation for more information about the
-    # add_image_kwargs
-    # https://napari.org/api/napari.Viewer.html#napari.Viewer.add_image
-    return [(numpy.random.rand(512, 512), {})]
+"""
+This module is an example of a barebones sample data provider for napari.
+
+It implements the "sample data" specification.
+see: https://napari.org/plugins/guides.html?#sample-data
+
+Replace code below according to your needs.
+"""
+from __future__ import annotations
+
+import numpy
+
+
+def make_sample_data():
+    """Generates an image"""
+    # Return list of tuples
+    # [(data1, add_image_kwargs1), (data2, add_image_kwargs2)]
+    # Check the documentation for more information about the
+    # add_image_kwargs
+    # https://napari.org/api/napari.Viewer.html#napari.Viewer.add_image
+    return [(numpy.random.rand(512, 512), {})]
```

### Comparing `guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/_tests/test_widget.py` & `guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/_tests/test_widget.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import numpy as np
-
-from guanine_crystal_analysis import ExampleQWidget, example_magic_widget
-
-
-# make_napari_viewer is a pytest fixture that returns a napari viewer object
-# capsys is a pytest fixture that captures stdout and stderr output streams
-def test_example_q_widget(make_napari_viewer, capsys):
-    # make viewer and add an image layer using our fixture
-    viewer = make_napari_viewer()
-    viewer.add_image(np.random.random((100, 100)))
-
-    # create our widget, passing in the viewer
-    my_widget = ExampleQWidget(viewer)
-
-    # call our widget method
-    my_widget._on_click()
-
-    # read captured output and check that it's as we expected
-    captured = capsys.readouterr()
-    assert captured.out == "napari has 1 layers\n"
-
-
-def test_example_magic_widget(make_napari_viewer, capsys):
-    viewer = make_napari_viewer()
-    layer = viewer.add_image(np.random.random((100, 100)))
-
-    # this time, our widget will be a MagicFactory or FunctionGui instance
-    my_widget = example_magic_widget()
-
-    # if we "call" this object, it'll execute our function
-    my_widget(viewer.layers[0])
-
-    # read captured output and check that it's as we expected
-    captured = capsys.readouterr()
-    assert captured.out == f"you have selected {layer}\n"
+import numpy as np
+
+from guanine_crystal_analysis import ExampleQWidget, example_magic_widget
+
+
+# make_napari_viewer is a pytest fixture that returns a napari viewer object
+# capsys is a pytest fixture that captures stdout and stderr output streams
+def test_example_q_widget(make_napari_viewer, capsys):
+    # make viewer and add an image layer using our fixture
+    viewer = make_napari_viewer()
+    viewer.add_image(np.random.random((100, 100)))
+
+    # create our widget, passing in the viewer
+    my_widget = ExampleQWidget(viewer)
+
+    # call our widget method
+    my_widget._on_click()
+
+    # read captured output and check that it's as we expected
+    captured = capsys.readouterr()
+    assert captured.out == "napari has 1 layers\n"
+
+
+def test_example_magic_widget(make_napari_viewer, capsys):
+    viewer = make_napari_viewer()
+    layer = viewer.add_image(np.random.random((100, 100)))
+
+    # this time, our widget will be a MagicFactory or FunctionGui instance
+    my_widget = example_magic_widget()
+
+    # if we "call" this object, it'll execute our function
+    my_widget(viewer.layers[0])
+
+    # read captured output and check that it's as we expected
+    captured = capsys.readouterr()
+    assert captured.out == f"you have selected {layer}\n"
```

### Comparing `guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/_widget.py` & `guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/_widget.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,205 +1,211 @@
-"""
-This module is an example of a barebones QWidget plugin for napari
-
-It implements the Widget specification.
-see: https://napari.org/plugins/guides.html?#widgets
-
-Replace code below according to your needs.
-"""
-
-# Uses the `autogenerate: true` flag in the plugin manifest
-# to indicate it should be wrapped as a magicgui to autogenerate
-# a widget.
-def normalization(input_image: "napari.types.ImageData")->"napari.types.ImageData":
-    import numpy as np
-    
-    normalized_image = input_image/np.percentile(input_image,99)
-    return normalized_image
-
-def segmentation(normalized_image: "napari.types.ImageData", 
-                 segmenter: str="object_segmenter_20220523_sorted.cl",
-                 minimum_pixel_count:int=50)->"napari.types.LabelsData":
-    from pathlib import Path
-    import apoc
-    import pyclesperanto_prototype as cle
-    
-    segmenter_filename = Path(__file__).parent/"cl_segmenter"/segmenter
-    print(segmenter_filename)
-    
-    segmenter = apoc.ObjectSegmenter(opencl_filename=segmenter_filename)
-     #show result of object segmenter
-    labels = segmenter.predict(normalized_image)
-    
-    #show result of object segmenter with labels in range
-    labels_in_range = cle.exclude_small_labels(source = labels, maximum_size = minimum_pixel_count)
-    return labels_in_range
-
-def analyze_image(image: "napari.types.ImageData", 
-                  label: "napari.types.LabelsData", 
-                  napari_viewer: "napari.Viewer" = None) -> "pandas.DataFrame":
-
-    import pandas as pd
-    from napari_skimage_regionprops import regionprops_table
-    from napari_simpleitk_image_processing import label_statistics
-
-    # measure in normalized image
-    df_skimage = pd.DataFrame(regionprops_table(image , label, size = True, intensity = True, perimeter = True, shape = True))
-    df_skimage["aspect_ratio"] = df_skimage["major_axis_length"]/df_skimage["minor_axis_length"]
-    df_simpleitk = pd.DataFrame(label_statistics(image, label, size = True, intensity = True, perimeter = True, shape = True))
-    results = pd.merge(df_skimage, df_simpleitk, on = "label", suffixes = ('_skimage', '_simpleitk'))
-    to_drop = ["extent", "local_centroid-0", "local_centroid-1","orientation"]
-    results = results.drop(to_drop, axis=1)
-    
-    #visualize table in napari
-    if napari_viewer is not None:
-        from napari_workflows._workflow import _get_layer_from_data
-        labels_layer = _get_layer_from_data(napari_viewer, label)
-        # Store results in the properties dictionary:
-        labels_layer.properties = results
-
-        # turn table into a widget
-        from napari_skimage_regionprops import add_table
-        add_table(labels_layer, napari_viewer)
-    else:
-        import pandas
-        return pandas.DataFrame(results)
-
-def classify_objects(label: "napari.types.LabelsData",
-                    intensity: bool = False,
-                     shape: bool = True, 
-                     size: bool = True,
-                    classifier_filename:str = "object_classifier_20220523_",
-                    napari_viewer: "napari.Viewer" = None)-> "napari.types.LabelsData":
-    from napari_workflows._workflow import _get_layer_from_data
-    import pandas as pd
-    labels_layer = _get_layer_from_data(napari_viewer, label)
-    table = pd.DataFrame(labels_layer.properties)
-    print("alle keys:", table.keys())
-    print(type(table))
-    keep = table[['label', 'aspect_ratio', 'max_intensity', 'min_intensity', 'perimeter_skimage', 'area', 'mean_intensity', 'major_axis_length', 'minor_axis_length', 'circularity', 'solidity', 'eccentricity', 'roundness_skimage', 'median', 'sum', 'variance', 'perimeter_on_border','perimeter_on_border_ratio']]
-    
-    #intensity table
-    df_intensity = keep[['label','max_intensity', 'mean_intensity', 'min_intensity','median', 'sum', 'variance']]
-    
-    #size table
-    df_size = keep[['label','area']]
-    
-    #shape table
-    df_shape = keep[['label', 'aspect_ratio','perimeter_skimage', 'major_axis_length',
-       'minor_axis_length', 'circularity', 'solidity', 'eccentricity',
-       'roundness_skimage', 'perimeter_on_border',
-       'perimeter_on_border_ratio']]
-    
-    selected_table = None 
-    
-    if size:
-        classifier_filename = classifier_filename + "size_"
-        if selected_table is not None:
-            selected_table = pd.merge(df_size, selected_table, on=('label'))
-        else:
-            selected_table = df_size
-            
-    if shape:
-        classifier_filename = classifier_filename + "shape_"
-        if selected_table is not None:
-            selected_table = pd.merge(df_shape, selected_table, on=('label'))
-        else:
-            selected_table = df_shape
-
-    if intensity:
-        classifier_filename = classifier_filename + "intensity_"
-        if selected_table is not None:
-            selected_table = pd.merge(df_intensity, selected_table, on=('label'))
-        else:
-            selected_table = df_intensity
-    
-    classifier_filename = classifier_filename[:-1]+".cl"
-    print("selected keys:", selected_table.keys())
-    print(classifier_filename)
-    return classifier(selected_table, label, classifier_filename)
-
-def classifier(table, label, tabrowcl_filename):
-    '''
-    this function applies the classifier to the testing data.
-    it creates:
-    - an output image
-    - writes the good crystal labels to a new table
-    '''
-    
-    #import statements
-    from pyclesperanto_prototype import imshow, replace_intensities
-    import numpy as np
-    import pandas as pd
-    import apoc
-    import os
-    import pyclesperanto_prototype as cle
-    from skimage.segmentation import relabel_sequential
-    from pathlib import Path
-    
-    #prediction
-    classifier_filename = Path(__file__).parent/"cl_classifier"/tabrowcl_filename
-    print(classifier_filename)
-    
-    classifier = apoc.TableRowClassifier(opencl_filename= classifier_filename)
-    prediction = classifier.predict(table)
-
-    #append predicted classes as columns to the table
-    table['predicted_class'] = prediction
-    
-    #add background to the prediction
-    predicted_class_with_background = [0] + prediction.tolist()
-    
-    # connect prediction to label image
-    class_image = replace_intensities(label, predicted_class_with_background).astype(int)
-    return class_image
-
-
-def bad_label_exclusion(label: "napari.types.LabelsData",
-                        class_image: "napari.types.LabelsData")-> "napari.types.LabelsData":
-    import os
-    import numpy as np
-    from pyclesperanto_prototype import relabel_sequential
-    
-    #change class of bad crystals (1) to background (0)
-    class_image = np.asarray(class_image)
-    class_image[class_image == 1]=0
-    class_image_mask = class_image.astype(bool)
-    
-    #exclude bad labels from label image
-    label_image_filtered=np.copy(label)
-    label_image_filtered[class_image_mask==False]=0
-    return relabel_sequential(label_image_filtered)
-
-def analyze_deluxe(input_image: "napari.types.ImageData",
-                   normalize: bool = True,
-                   segmenter: str="object_segmenter_20220523_sorted.cl",
-                   minimum_pixel_count:int=50,
-                   intensity: bool = False,
-                    shape: bool = True, 
-                    size: bool = True,
-                    classifier_filename:str = "object_classifier_20220523_",
-                   napari_viewer: "napari.Viewer" = None):
-    if normalize:
-        image_maybe_normalized = normalization(input_image)
-        napari_viewer.add_image(image_maybe_normalized,name="normalized")
-    else:
-        image_maybe_normalized = input_image
-        
-    segmentation_result = segmentation(image_maybe_normalized, segmenter, minimum_pixel_count)
-    napari_viewer.add_labels(segmentation_result)
-    
-    analyze_image(image_maybe_normalized, segmentation_result, napari_viewer)
-    classification_result = classify_objects(segmentation_result, intensity, shape, size, classifier_filename, napari_viewer)
-    napari_viewer.add_labels(classification_result)
-    
-    exclusion_result = bad_label_exclusion(segmentation_result, classification_result)
-    napari_viewer.add_labels(exclusion_result)
-    
-    analyze_image(image_maybe_normalized, exclusion_result, napari_viewer)
-    
-    
-    
-
-    
-    
-    
+"""
+This module is an example of a barebones QWidget plugin for napari
+
+It implements the Widget specification.
+see: https://napari.org/plugins/guides.html?#widgets
+
+Replace code below according to your needs.
+"""
+
+# Uses the `autogenerate: true` flag in the plugin manifest
+# to indicate it should be wrapped as a magicgui to autogenerate
+# a widget.
+def normalization(input_image: "napari.types.ImageData")->"napari.types.ImageData":
+    import numpy as np
+    
+    normalized_image = input_image/np.percentile(input_image,99)
+    return normalized_image
+
+def segmentation(normalized_image: "napari.types.ImageData", 
+                 segmenter: str="object_segmenter_20220523_sorted.cl",
+                 minimum_pixel_count:int=50)->"napari.types.LabelsData":
+    from pathlib import Path
+    import apoc
+    import pyclesperanto_prototype as cle
+    
+    segmenter_filename = Path(__file__).parent/"cl_segmenter"/segmenter
+    print(segmenter_filename)
+    
+    segmenter = apoc.ObjectSegmenter(opencl_filename=segmenter_filename)
+     #show result of object segmenter
+    labels = segmenter.predict(normalized_image)
+    
+    #show result of object segmenter with labels in range
+    labels_in_range = cle.exclude_small_labels(source = labels, maximum_size = minimum_pixel_count)
+    return labels_in_range
+
+def analyze_image(image: "napari.types.ImageData", 
+                  label: "napari.types.LabelsData", 
+                  napari_viewer: "napari.Viewer" = None) -> "pandas.DataFrame":
+
+    import pandas as pd
+    from napari_skimage_regionprops import regionprops_table
+    from napari_simpleitk_image_processing import label_statistics
+
+    # measure in normalized image
+    df_skimage = pd.DataFrame(regionprops_table(image , label, size = True, intensity = True, perimeter = True, shape = True))
+    df_skimage["aspect_ratio"] = df_skimage["major_axis_length"]/df_skimage["minor_axis_length"]
+    df_simpleitk = pd.DataFrame(label_statistics(image, label, size = True, intensity = True, perimeter = True, shape = True))
+    results = pd.merge(df_skimage, df_simpleitk, on = "label", suffixes = ('_skimage', '_simpleitk'))
+    to_drop = ["extent", "local_centroid-0", "local_centroid-1","orientation"]
+    results = results.drop(to_drop, axis=1)
+    
+    #visualize table in napari
+    if napari_viewer is not None:
+        from napari_workflows._workflow import _get_layer_from_data
+        labels_layer = _get_layer_from_data(napari_viewer, label)
+        # Store results in the properties dictionary:
+        labels_layer.properties = results
+
+        # turn table into a widget
+        from napari_skimage_regionprops import add_table
+        add_table(labels_layer, napari_viewer)
+    else:
+        import pandas
+        return pandas.DataFrame(results)
+
+def classify_objects(label: "napari.types.LabelsData",
+                    intensity: bool = False,
+                     shape: bool = True, 
+                     size: bool = True,
+                    classifier_filename:str = "object_classifier_20220523_",
+                     table: "pandas.DataFrame" = None,
+                    napari_viewer: "napari.Viewer" = None)-> "napari.types.LabelsData":
+    from napari_workflows._workflow import _get_layer_from_data
+    import pandas as pd
+    
+    if napari_viewer is not None:
+        labels_layer = _get_layer_from_data(napari_viewer, label)
+        table = pd.DataFrame(labels_layer.properties)
+        
+            
+    print("alle keys:", table.keys())
+    print(type(table))
+    keep = table[['label', 'aspect_ratio', 'max_intensity', 'min_intensity', 'perimeter_skimage', 'area', 'mean_intensity', 'major_axis_length', 'minor_axis_length', 'circularity', 'solidity', 'eccentricity', 'roundness_skimage', 'median', 'sum', 'variance', 'perimeter_on_border','perimeter_on_border_ratio']]
+    
+    #intensity table
+    df_intensity = keep[['label','max_intensity', 'mean_intensity', 'min_intensity','median', 'sum', 'variance']]
+    
+    #size table
+    df_size = keep[['label','area']]
+    
+    #shape table
+    df_shape = keep[['label', 'aspect_ratio','perimeter_skimage', 'major_axis_length',
+       'minor_axis_length', 'circularity', 'solidity', 'eccentricity',
+       'roundness_skimage', 'perimeter_on_border',
+       'perimeter_on_border_ratio']]
+    
+    selected_table = None 
+    
+    if size:
+        classifier_filename = classifier_filename + "size_"
+        if selected_table is not None:
+            selected_table = pd.merge(df_size, selected_table, on=('label'))
+        else:
+            selected_table = df_size
+            
+    if shape:
+        classifier_filename = classifier_filename + "shape_"
+        if selected_table is not None:
+            selected_table = pd.merge(df_shape, selected_table, on=('label'))
+        else:
+            selected_table = df_shape
+
+    if intensity:
+        classifier_filename = classifier_filename + "intensity_"
+        if selected_table is not None:
+            selected_table = pd.merge(df_intensity, selected_table, on=('label'))
+        else:
+            selected_table = df_intensity
+    
+    classifier_filename = classifier_filename[:-1]+".cl"
+    print("selected keys:", selected_table.keys())
+    print(classifier_filename)
+    return classifier(selected_table, label, classifier_filename)
+
+def classifier(table, label, tabrowcl_filename):
+    '''
+    this function applies the classifier to the testing data.
+    it creates:
+    - an output image
+    - writes the good crystal labels to a new table
+    '''
+    
+    #import statements
+    from pyclesperanto_prototype import imshow, replace_intensities
+    import numpy as np
+    import pandas as pd
+    import apoc
+    import os
+    import pyclesperanto_prototype as cle
+    from skimage.segmentation import relabel_sequential
+    from pathlib import Path
+    
+    #prediction
+    classifier_filename = Path(__file__).parent/"cl_classifier"/tabrowcl_filename
+    print(classifier_filename)
+    
+    classifier = apoc.TableRowClassifier(opencl_filename= classifier_filename)
+    prediction = classifier.predict(table)
+
+    #append predicted classes as columns to the table
+    table['predicted_class'] = prediction
+    
+    #add background to the prediction
+    predicted_class_with_background = [0] + prediction.tolist()
+    
+    # connect prediction to label image
+    class_image = replace_intensities(label, predicted_class_with_background).astype(int)
+    return class_image
+
+
+def bad_label_exclusion(label: "napari.types.LabelsData",
+                        class_image: "napari.types.LabelsData")-> "napari.types.LabelsData":
+    import os
+    import numpy as np
+    from pyclesperanto_prototype import relabel_sequential
+    
+    #change class of bad crystals (1) to background (0)
+    class_image = np.asarray(class_image)
+    class_image[class_image == 1]=0
+    class_image_mask = class_image.astype(bool)
+    
+    #exclude bad labels from label image
+    label_image_filtered=np.copy(label)
+    label_image_filtered[class_image_mask==False]=0
+    return relabel_sequential(label_image_filtered)
+
+def analyze_deluxe(input_image: "napari.types.ImageData",
+                   normalize: bool = True,
+                   segmenter: str="object_segmenter_20220523_sorted.cl",
+                   minimum_pixel_count:int=50,
+                   intensity: bool = False,
+                    shape: bool = True, 
+                    size: bool = True,
+                    classifier_filename:str = "object_classifier_20220523_",
+                   table: "pandas.DataFrame" = None,
+                   napari_viewer: "napari.Viewer" = None):
+    if normalize:
+        image_maybe_normalized = normalization(input_image)
+        napari_viewer.add_image(image_maybe_normalized,name="normalized")
+    else:
+        image_maybe_normalized = input_image
+        
+    segmentation_result = segmentation(image_maybe_normalized, segmenter, minimum_pixel_count)
+    napari_viewer.add_labels(segmentation_result)
+    
+    analyze_image(image_maybe_normalized, segmentation_result, napari_viewer)
+    classification_result = classify_objects(segmentation_result, intensity, shape, size, classifier_filename, table, napari_viewer)
+    napari_viewer.add_labels(classification_result)
+    
+    exclusion_result = bad_label_exclusion(segmentation_result, classification_result)
+    napari_viewer.add_labels(exclusion_result)
+    
+    analyze_image(image_maybe_normalized, exclusion_result, napari_viewer)
+    
+    
+    
+
+    
+    
+
```

### Comparing `guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis/napari.yaml` & `guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis/napari.yaml`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-name: guanine-crystal-analysis
-display_name: Guanine Crystal Analysis
-contributions:
-  commands:
-    - id: guanine-crystal-analysis.normalization
-      python_name: guanine_crystal_analysis._widget:normalization
-      title: normalization
-    - id: guanine-crystal-analysis.segmentation
-      python_name: guanine_crystal_analysis._widget:segmentation
-      title: segmentation
-    - id: guanine-crystal-analysis.analyze_image
-      python_name: guanine_crystal_analysis._widget:analyze_image
-      title: analyze_image
-    - id: guanine-crystal-analysis.classify_objects
-      python_name: guanine_crystal_analysis._widget:classify_objects
-      title: classify_objects
-    - id: guanine-crystal-analysis.bad_label_exclusion
-      python_name: guanine_crystal_analysis._widget:bad_label_exclusion
-      title: bad_label_exclusion
-    - id: guanine-crystal-analysis.analyze_deluxe
-      python_name: guanine_crystal_analysis._widget:analyze_deluxe
-      title: analyze_deluxe
-  sample_data:
-    - command: guanine-crystal-analysis.make_sample_data
-      display_name: Guanine Crystal Analysis
-      key: unique_id.1
-  widgets:
-    - command: guanine-crystal-analysis.normalization
-      autogenerate: true
-      display_name: Normalization 
-    - command: guanine-crystal-analysis.segmentation
-      autogenerate: true
-      display_name: Segmentation
-    - command: guanine-crystal-analysis.analyze_image
-      autogenerate: true
-      display_name: Analyze Image
-    - command: guanine-crystal-analysis.classify_objects
-      autogenerate: true
-      display_name: Classify Objects
-    - command: guanine-crystal-analysis.bad_label_exclusion
-      autogenerate: true
-      display_name: Bad Label Exclusion
-    - command: guanine-crystal-analysis.analyze_deluxe
-      autogenerate: true
+name: guanine-crystal-analysis
+display_name: Guanine Crystal Analysis
+contributions:
+  commands:
+    - id: guanine-crystal-analysis.normalization
+      python_name: guanine_crystal_analysis._widget:normalization
+      title: normalization
+    - id: guanine-crystal-analysis.segmentation
+      python_name: guanine_crystal_analysis._widget:segmentation
+      title: segmentation
+    - id: guanine-crystal-analysis.analyze_image
+      python_name: guanine_crystal_analysis._widget:analyze_image
+      title: analyze_image
+    - id: guanine-crystal-analysis.classify_objects
+      python_name: guanine_crystal_analysis._widget:classify_objects
+      title: classify_objects
+    - id: guanine-crystal-analysis.bad_label_exclusion
+      python_name: guanine_crystal_analysis._widget:bad_label_exclusion
+      title: bad_label_exclusion
+    - id: guanine-crystal-analysis.analyze_deluxe
+      python_name: guanine_crystal_analysis._widget:analyze_deluxe
+      title: analyze_deluxe
+  sample_data:
+    - command: guanine-crystal-analysis.make_sample_data
+      display_name: Guanine Crystal Analysis
+      key: unique_id.1
+  widgets:
+    - command: guanine-crystal-analysis.normalization
+      autogenerate: true
+      display_name: Normalization 
+    - command: guanine-crystal-analysis.segmentation
+      autogenerate: true
+      display_name: Segmentation
+    - command: guanine-crystal-analysis.analyze_image
+      autogenerate: true
+      display_name: Analyze Image
+    - command: guanine-crystal-analysis.classify_objects
+      autogenerate: true
+      display_name: Classify Objects
+    - command: guanine-crystal-analysis.bad_label_exclusion
+      autogenerate: true
+      display_name: Bad Label Exclusion
+    - command: guanine-crystal-analysis.analyze_deluxe
+      autogenerate: true
       display_name: Analyze Deluxe
```

### Comparing `guanine-crystal-analysis-0.0.1/src/guanine_crystal_analysis.egg-info/SOURCES.txt` & `guanine-crystal-analysis-0.0.2/src/guanine_crystal_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

