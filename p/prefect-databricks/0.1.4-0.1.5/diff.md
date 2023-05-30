# Comparing `tmp/prefect-databricks-0.1.4.tar.gz` & `tmp/prefect-databricks-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-databricks/prefect-databricks/dist/.tmp-fmno64hg/prefect-databricks-0.1.4.tar", last modified: Wed Jan  4 17:08:49 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-databricks/prefect-databricks/dist/.tmp-4s35le7u/prefect-databricks-0.1.5.tar", last modified: Tue May 30 17:50:05 2023, max compression
```

## Comparing `prefect-databricks-0.1.4.tar` & `prefect-databricks-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/prefect_databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/prefect_databricks/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    18358 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/prefect_databricks/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    81198 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/prefect_databricks/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/prefect_databricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   168201 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/prefect_databricks/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/prefect_databricks/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/prefect_databricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/scripts/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-01-04 17:08:49.000000 prefect-databricks-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-01-04 17:07:30.000000 prefect-databricks-0.1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81381 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168820 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/prefect_databricks/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/prefect_databricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/scripts/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:05.000000 prefect-databricks-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-30 17:48:44.000000 prefect-databricks-0.1.5/versioneer.py
```

### Comparing `prefect-databricks-0.1.4/LICENSE` & `prefect-databricks-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.4/PKG-INFO` & `prefect-databricks-0.1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,475 +1,597 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7072 6566  : 2.1.Name: pref
-00000020: 6563 742d 6461 7461 6272 6963 6b73 0a56  ect-databricks.V
-00000030: 6572 7369 6f6e 3a20 302e 312e 340a 5375  ersion: 0.1.4.Su
-00000040: 6d6d 6172 793a 2050 7265 6665 6374 2069  mmary: Prefect i
-00000050: 6e74 6567 7261 7469 6f6e 7320 696e 7465  ntegrations inte
-00000060: 7261 6374 696e 6720 7769 7468 2044 6174  racting with Dat
-00000070: 6162 7269 636b 730a 486f 6d65 2d70 6167  abricks.Home-pag
-00000080: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-00000090: 622e 636f 6d2f 5072 6566 6563 7448 512f  b.com/PrefectHQ/
-000000a0: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-000000b0: 6b73 0a41 7574 686f 723a 2050 7265 6665  ks.Author: Prefe
-000000c0: 6374 2054 6563 686e 6f6c 6f67 6965 732c  ct Technologies,
-000000d0: 2049 6e63 2e0a 4175 7468 6f72 2d65 6d61   Inc..Author-ema
-000000e0: 696c 3a20 6865 6c70 4070 7265 6665 6374  il: help@prefect
-000000f0: 2e69 6f0a 4c69 6365 6e73 653a 2041 7061  .io.License: Apa
-00000100: 6368 6520 4c69 6365 6e73 6520 322e 300a  che License 2.0.
-00000110: 4b65 7977 6f72 6473 3a20 7072 6566 6563  Keywords: prefec
-00000120: 740a 436c 6173 7369 6669 6572 3a20 4e61  t.Classifier: Na
-00000130: 7475 7261 6c20 4c61 6e67 7561 6765 203a  tural Language :
-00000140: 3a20 456e 676c 6973 680a 436c 6173 7369  : English.Classi
-00000150: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000160: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-00000170: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
-00000180: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-00000190: 6e63 6520 3a3a 2053 7973 7465 6d20 4164  nce :: System Ad
-000001a0: 6d69 6e69 7374 7261 746f 7273 0a43 6c61  ministrators.Cla
-000001b0: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-000001c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000001d0: 203a 3a20 4170 6163 6865 2053 6f66 7477   :: Apache Softw
-000001e0: 6172 6520 4c69 6365 6e73 650a 436c 6173  are License.Clas
-000001f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000210: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
-00000220: 6e6c 790a 436c 6173 7369 6669 6572 3a20  nly.Classifier: 
-00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000250: 3a20 332e 370a 436c 6173 7369 6669 6572  : 3.7.Classifier
-00000260: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000270: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000280: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
-00000290: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000002a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002b0: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
-000002c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000002d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002e0: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
-000002f0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000300: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000310: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
-00000320: 6965 730a 5265 7175 6972 6573 2d50 7974  ies.Requires-Pyt
-00000330: 686f 6e3a 203e 3d33 2e37 0a44 6573 6372  hon: >=3.7.Descr
-00000340: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-00000350: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-00000360: 776e 0a50 726f 7669 6465 732d 4578 7472  wn.Provides-Extr
-00000370: 613a 2064 6576 0a4c 6963 656e 7365 2d46  a: dev.License-F
-00000380: 696c 653a 204c 4943 454e 5345 0a0a 2320  ile: LICENSE..# 
-00000390: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-000003a0: 6b73 0a0a 5669 7369 7420 7468 6520 6675  ks..Visit the fu
-000003b0: 6c6c 2064 6f63 7320 5b68 6572 655d 2868  ll docs [here](h
-000003c0: 7474 7073 3a2f 2f50 7265 6665 6374 4851  ttps://PrefectHQ
-000003d0: 2e67 6974 6875 622e 696f 2f70 7265 6665  .github.io/prefe
-000003e0: 6374 2d64 6174 6162 7269 636b 7329 2074  ct-databricks) t
-000003f0: 6f20 7365 6520 6164 6469 7469 6f6e 616c  o see additional
-00000400: 2065 7861 6d70 6c65 7320 616e 6420 7468   examples and th
-00000410: 6520 4150 4920 7265 6665 7265 6e63 652e  e API reference.
-00000420: 0a20 0a3c 7020 616c 6967 6e3d 2263 656e  . .<p align="cen
-00000430: 7465 7222 3e0a 2020 2020 3c61 2068 7265  ter">.    <a hre
-00000440: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
-00000450: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
-00000460: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00000470: 6b73 2f22 2061 6c74 3d22 5079 5049 2076  ks/" alt="PyPI v
-00000480: 6572 7369 6f6e 223e 0a20 2020 2020 2020  ersion">.       
-00000490: 203c 696d 6720 616c 743d 2250 7950 4922   <img alt="PyPI"
-000004a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-000004b0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000004c0: 692f 762f 7072 6566 6563 742d 6461 7461  i/v/prefect-data
-000004d0: 6272 6963 6b73 3f63 6f6c 6f72 3d30 3035  bricks?color=005
-000004e0: 3246 4626 6c61 6265 6c43 6f6c 6f72 3d30  2FF&labelColor=0
-000004f0: 3930 3432 3222 3e3c 2f61 3e0a 2020 2020  90422"></a>.    
-00000500: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000510: 2f67 6974 6875 622e 636f 6d2f 5072 6566  /github.com/Pref
-00000520: 6563 7448 512f 7072 6566 6563 742d 6461  ectHQ/prefect-da
-00000530: 7461 6272 6963 6b73 2f22 2061 6c74 3d22  tabricks/" alt="
-00000540: 5374 6172 7322 3e0a 2020 2020 2020 2020  Stars">.        
-00000550: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000560: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000570: 2f67 6974 6875 622f 7374 6172 732f 5072  /github/stars/Pr
-00000580: 6566 6563 7448 512f 7072 6566 6563 742d  efectHQ/prefect-
-00000590: 6461 7461 6272 6963 6b73 3f63 6f6c 6f72  databricks?color
-000005a0: 3d30 3035 3246 4626 6c61 6265 6c43 6f6c  =0052FF&labelCol
-000005b0: 6f72 3d30 3930 3432 3222 202f 3e3c 2f61  or=090422" /></a
-000005c0: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-000005d0: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-000005e0: 2f62 6164 6765 2f70 7265 6665 6374 2d64  /badge/prefect-d
-000005f0: 6174 6162 7269 636b 732f 2220 616c 743d  atabricks/" alt=
-00000600: 2244 6f77 6e6c 6f61 6473 223e 0a20 2020  "Downloads">.   
-00000610: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
-00000620: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000630: 6473 2e69 6f2f 7079 7069 2f64 6d2f 7072  ds.io/pypi/dm/pr
-00000640: 6566 6563 742d 6461 7461 6272 6963 6b73  efect-databricks
-00000650: 3f63 6f6c 6f72 3d30 3035 3246 4626 6c61  ?color=0052FF&la
-00000660: 6265 6c43 6f6c 6f72 3d30 3930 3432 3222  belColor=090422"
-00000670: 202f 3e3c 2f61 3e0a 2020 2020 3c61 2068   /></a>.    <a h
-00000680: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000690: 6875 622e 636f 6d2f 5072 6566 6563 7448  hub.com/PrefectH
-000006a0: 512f 7072 6566 6563 742d 6461 7461 6272  Q/prefect-databr
-000006b0: 6963 6b73 2f70 756c 7365 2220 616c 743d  icks/pulse" alt=
-000006c0: 2241 6374 6976 6974 7922 3e0a 2020 2020  "Activity">.    
-000006d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-000006e0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000006f0: 732e 696f 2f67 6974 6875 622f 636f 6d6d  s.io/github/comm
-00000700: 6974 2d61 6374 6976 6974 792f 6d2f 5072  it-activity/m/Pr
-00000710: 6566 6563 7448 512f 7072 6566 6563 742d  efectHQ/prefect-
-00000720: 6461 7461 6272 6963 6b73 3f63 6f6c 6f72  databricks?color
-00000730: 3d30 3035 3246 4626 6c61 6265 6c43 6f6c  =0052FF&labelCol
-00000740: 6f72 3d30 3930 3432 3222 202f 3e3c 2f61  or=090422" /></a
-00000750: 3e0a 2020 2020 3c62 723e 0a20 2020 203c  >.    <br>.    <
-00000760: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000770: 7072 6566 6563 742d 636f 6d6d 756e 6974  prefect-communit
-00000780: 792e 736c 6163 6b2e 636f 6d22 2061 6c74  y.slack.com" alt
-00000790: 3d22 536c 6163 6b22 3e0a 2020 2020 2020  ="Slack">.      
-000007a0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-000007b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000007c0: 696f 2f62 6164 6765 2f73 6c61 636b 2d6a  io/badge/slack-j
-000007d0: 6f69 6e5f 636f 6d6d 756e 6974 792d 7265  oin_community-re
-000007e0: 642e 7376 673f 636f 6c6f 723d 3030 3532  d.svg?color=0052
-000007f0: 4646 266c 6162 656c 436f 6c6f 723d 3039  FF&labelColor=09
-00000800: 3034 3232 266c 6f67 6f3d 736c 6163 6b22  0422&logo=slack"
-00000810: 202f 3e3c 2f61 3e0a 2020 2020 3c61 2068   /></a>.    <a h
-00000820: 7265 663d 2268 7474 7073 3a2f 2f64 6973  ref="https://dis
-00000830: 636f 7572 7365 2e70 7265 6665 6374 2e69  course.prefect.i
-00000840: 6f2f 2220 616c 743d 2244 6973 636f 7572  o/" alt="Discour
-00000850: 7365 223e 0a20 2020 2020 2020 203c 696d  se">.        <im
-00000860: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000870: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000880: 6467 652f 6469 7363 6f75 7273 652d 6272  dge/discourse-br
-00000890: 6f77 7365 5f66 6f72 756d 2d72 6564 2e73  owse_forum-red.s
-000008a0: 7667 3f63 6f6c 6f72 3d30 3035 3246 4626  vg?color=0052FF&
-000008b0: 6c61 6265 6c43 6f6c 6f72 3d30 3930 3432  labelColor=09042
-000008c0: 3226 6c6f 676f 3d64 6973 636f 7572 7365  2&logo=discourse
-000008d0: 2220 2f3e 3c2f 613e 0a3c 2f70 3e0a 0a23  " /></a>.</p>..#
-000008e0: 2320 5765 6c63 6f6d 6521 0a0a 5072 6566  # Welcome!..Pref
-000008f0: 6563 7420 696e 7465 6772 6174 696f 6e73  ect integrations
-00000900: 2066 6f72 2069 6e74 6572 6163 7469 6e67   for interacting
-00000910: 2077 6974 6820 4461 7461 6272 6963 6b73   with Databricks
-00000920: 0a0a 5468 6520 7461 736b 7320 7769 7468  ..The tasks with
-00000930: 696e 2074 6869 7320 636f 6c6c 6563 7469  in this collecti
-00000940: 6f6e 2077 6572 6520 6372 6561 7465 6420  on were created 
-00000950: 6279 2061 2063 6f64 6520 6765 6e65 7261  by a code genera
-00000960: 746f 7220 7573 696e 6720 7468 6520 7365  tor using the se
-00000970: 7276 6963 6527 7320 4f70 656e 4150 4920  rvice's OpenAPI 
-00000980: 7370 6563 2e0a 0a54 6865 2073 6572 7669  spec...The servi
-00000990: 6365 2773 2052 4553 5420 4150 4920 646f  ce's REST API do
-000009a0: 6375 6d65 6e74 6174 696f 6e20 6361 6e20  cumentation can 
-000009b0: 6265 2066 6f75 6e64 205b 6865 7265 5d28  be found [here](
-000009c0: 6874 7470 733a 2f2f 646f 6373 2e64 6174  https://docs.dat
-000009d0: 6162 7269 636b 732e 636f 6d2f 6465 762d  abricks.com/dev-
-000009e0: 746f 6f6c 732f 6170 692f 6c61 7465 7374  tools/api/latest
-000009f0: 2f69 6e64 6578 2e68 746d 6c29 2e0a 0a23  /index.html)...#
-00000a00: 2320 4765 7474 696e 6720 5374 6172 7465  # Getting Starte
-00000a10: 640a 0a23 2323 2050 7974 686f 6e20 7365  d..### Python se
-00000a20: 7475 700a 0a52 6571 7569 7265 7320 616e  tup..Requires an
-00000a30: 2069 6e73 7461 6c6c 6174 696f 6e20 6f66   installation of
-00000a40: 2050 7974 686f 6e20 332e 372b 2e0a 0a57   Python 3.7+...W
-00000a50: 6520 7265 636f 6d6d 656e 6420 7573 696e  e recommend usin
-00000a60: 6720 6120 5079 7468 6f6e 2076 6972 7475  g a Python virtu
-00000a70: 616c 2065 6e76 6972 6f6e 6d65 6e74 206d  al environment m
-00000a80: 616e 6167 6572 2073 7563 6820 6173 2070  anager such as p
-00000a90: 6970 656e 762c 2063 6f6e 6461 206f 7220  ipenv, conda or 
-00000aa0: 7669 7274 7561 6c65 6e76 2e0a 0a54 6865  virtualenv...The
-00000ab0: 7365 2074 6173 6b73 2061 7265 2064 6573  se tasks are des
-00000ac0: 6967 6e65 6420 746f 2077 6f72 6b20 7769  igned to work wi
-00000ad0: 7468 2050 7265 6665 6374 2032 2e20 466f  th Prefect 2. Fo
-00000ae0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-00000af0: 6f6e 2061 626f 7574 2068 6f77 2074 6f20  on about how to 
-00000b00: 7573 6520 5072 6566 6563 742c 2070 6c65  use Prefect, ple
-00000b10: 6173 6520 7265 6665 7220 746f 2074 6865  ase refer to the
-00000b20: 205b 5072 6566 6563 7420 646f 6375 6d65   [Prefect docume
-00000b30: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-00000b40: 2f6f 7269 6f6e 2d64 6f63 732e 7072 6566  /orion-docs.pref
-00000b50: 6563 742e 696f 2f29 2e0a 0a23 2323 2049  ect.io/)...### I
-00000b60: 6e73 7461 6c6c 6174 696f 6e0a 0a49 6e73  nstallation..Ins
-00000b70: 7461 6c6c 2060 7072 6566 6563 742d 6461  tall `prefect-da
-00000b80: 7461 6272 6963 6b73 6020 7769 7468 2060  tabricks` with `
-00000b90: 7069 7060 3a0a 0a60 6060 6261 7368 0a70  pip`:..```bash.p
-00000ba0: 6970 2069 6e73 7461 6c6c 2070 7265 6665  ip install prefe
-00000bb0: 6374 2d64 6174 6162 7269 636b 730a 6060  ct-databricks.``
-00000bc0: 600a 0a41 206c 6973 7420 6f66 2061 7661  `..A list of ava
-00000bd0: 696c 6162 6c65 2062 6c6f 636b 7320 696e  ilable blocks in
-00000be0: 2060 7072 6566 6563 742d 6461 7461 6272   `prefect-databr
-00000bf0: 6963 6b73 6020 616e 6420 7468 6569 7220  icks` and their 
-00000c00: 7365 7475 7020 696e 7374 7275 6374 696f  setup instructio
-00000c10: 6e73 2063 616e 2062 6520 666f 756e 6420  ns can be found 
-00000c20: 5b68 6572 655d 2868 7474 7073 3a2f 2f50  [here](https://P
-00000c30: 7265 6665 6374 4851 2e67 6974 6875 622e  refectHQ.github.
-00000c40: 696f 2f70 7265 6665 6374 2d64 6174 6162  io/prefect-datab
-00000c50: 7269 636b 732f 2362 6c6f 636b 732d 6361  ricks/#blocks-ca
-00000c60: 7461 6c6f 6729 2e0a 0a23 2323 204c 6973  talog)...### Lis
-00000c70: 7473 206a 6f62 7320 6f6e 2074 6865 2044  ts jobs on the D
-00000c80: 6174 6162 7269 636b 7320 696e 7374 616e  atabricks instan
-00000c90: 6365 0a0a 6060 6070 7974 686f 6e0a 6672  ce..```python.fr
-00000ca0: 6f6d 2070 7265 6665 6374 2069 6d70 6f72  om prefect impor
-00000cb0: 7420 666c 6f77 0a66 726f 6d20 7072 6566  t flow.from pref
-00000cc0: 6563 745f 6461 7461 6272 6963 6b73 2069  ect_databricks i
-00000cd0: 6d70 6f72 7420 4461 7461 6272 6963 6b73  mport Databricks
-00000ce0: 4372 6564 656e 7469 616c 730a 6672 6f6d  Credentials.from
-00000cf0: 2070 7265 6665 6374 5f64 6174 6162 7269   prefect_databri
-00000d00: 636b 732e 6a6f 6273 2069 6d70 6f72 7420  cks.jobs import 
-00000d10: 6a6f 6273 5f6c 6973 740a 0a0a 4066 6c6f  jobs_list...@flo
-00000d20: 770a 6465 6620 6578 616d 706c 655f 6578  w.def example_ex
-00000d30: 6563 7574 655f 656e 6470 6f69 6e74 5f66  ecute_endpoint_f
-00000d40: 6c6f 7728 293a 0a20 2020 2064 6174 6162  low():.    datab
-00000d50: 7269 636b 735f 6372 6564 656e 7469 616c  ricks_credential
-00000d60: 7320 3d20 4461 7461 6272 6963 6b73 4372  s = DatabricksCr
-00000d70: 6564 656e 7469 616c 732e 6c6f 6164 2822  edentials.load("
-00000d80: 6d79 2d62 6c6f 636b 2229 0a20 2020 206a  my-block").    j
-00000d90: 6f62 7320 3d20 6a6f 6273 5f6c 6973 7428  obs = jobs_list(
-00000da0: 0a20 2020 2020 2020 2064 6174 6162 7269  .        databri
-00000db0: 636b 735f 6372 6564 656e 7469 616c 732c  cks_credentials,
-00000dc0: 0a20 2020 2020 2020 206c 696d 6974 3d35  .        limit=5
-00000dd0: 0a20 2020 2029 0a20 2020 2072 6574 7572  .    ).    retur
-00000de0: 6e20 6a6f 6273 0a0a 6578 616d 706c 655f  n jobs..example_
-00000df0: 6578 6563 7574 655f 656e 6470 6f69 6e74  execute_endpoint
-00000e00: 5f66 6c6f 7728 290a 6060 600a 0a23 2323  _flow().```..###
-00000e10: 2055 7365 2060 7769 7468 5f6f 7074 696f   Use `with_optio
-00000e20: 6e73 6020 746f 2063 7573 746f 6d69 7a65  ns` to customize
-00000e30: 206f 7074 696f 6e73 206f 6e20 616e 7920   options on any 
-00000e40: 6578 6973 7469 6e67 2074 6173 6b20 6f72  existing task or
-00000e50: 2066 6c6f 770a 0a60 6060 7079 7468 6f6e   flow..```python
-00000e60: 0a63 7573 746f 6d5f 6578 616d 706c 655f  .custom_example_
-00000e70: 6578 6563 7574 655f 656e 6470 6f69 6e74  execute_endpoint
-00000e80: 5f66 6c6f 7720 3d20 6578 616d 706c 655f  _flow = example_
-00000e90: 6578 6563 7574 655f 656e 6470 6f69 6e74  execute_endpoint
-00000ea0: 5f66 6c6f 772e 7769 7468 5f6f 7074 696f  _flow.with_optio
-00000eb0: 6e73 280a 2020 2020 6e61 6d65 3d22 4d79  ns(.    name="My
-00000ec0: 2063 7573 746f 6d20 666c 6f77 206e 616d   custom flow nam
-00000ed0: 6522 2c0a 2020 2020 7265 7472 6965 733d  e",.    retries=
-00000ee0: 322c 0a20 2020 2072 6574 7279 5f64 656c  2,.    retry_del
-00000ef0: 6179 5f73 6563 6f6e 6473 3d31 302c 0a29  ay_seconds=10,.)
-00000f00: 0a60 6060 0a0a 2323 2320 4c61 756e 6368  .```..### Launch
-00000f10: 2061 206e 6577 2063 6c75 7374 6572 2061   a new cluster a
-00000f20: 6e64 2072 756e 2061 2044 6174 6162 7269  nd run a Databri
-00000f30: 636b 7320 6e6f 7465 626f 6f6b 0a0a 4e6f  cks notebook..No
-00000f40: 7465 626f 6f6b 206e 616d 6564 2060 6578  tebook named `ex
-00000f50: 616d 706c 652e 6970 796e 6260 206f 6e20  ample.ipynb` on 
-00000f60: 4461 7461 6272 6963 6b73 2077 6869 6368  Databricks which
-00000f70: 2061 6363 6570 7473 2061 206e 616d 6520   accepts a name 
-00000f80: 7061 7261 6d65 7465 723a 0a0a 6060 6070  parameter:..```p
-00000f90: 7974 686f 6e0a 6e61 6d65 203d 2064 6275  ython.name = dbu
-00000fa0: 7469 6c73 2e77 6964 6765 7473 2e67 6574  tils.widgets.get
-00000fb0: 2822 6e61 6d65 2229 0a6d 6573 7361 6765  ("name").message
-00000fc0: 203d 2066 2244 6f6e 2774 2077 6f72 7279   = f"Don't worry
-00000fd0: 207b 6e61 6d65 7d2c 2049 2067 6f74 2079   {name}, I got y
-00000fe0: 6f75 7220 7265 7175 6573 7421 2057 656c  our request! Wel
-00000ff0: 636f 6d65 2074 6f20 7072 6566 6563 742d  come to prefect-
-00001000: 6461 7461 6272 6963 6b73 2122 0a70 7269  databricks!".pri
-00001010: 6e74 286d 6573 7361 6765 290a 6060 600a  nt(message).```.
-00001020: 0a50 7265 6665 6374 2066 6c6f 7720 7468  .Prefect flow th
-00001030: 6174 206c 6175 6e63 6865 7320 6120 6e65  at launches a ne
-00001040: 7720 636c 7573 7465 7220 746f 2072 756e  w cluster to run
-00001050: 2060 6578 616d 706c 652e 6970 796e 6260   `example.ipynb`
-00001060: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
-00001070: 6d20 7072 6566 6563 7420 696d 706f 7274  m prefect import
-00001080: 2066 6c6f 770a 6672 6f6d 2070 7265 6665   flow.from prefe
-00001090: 6374 5f64 6174 6162 7269 636b 7320 696d  ct_databricks im
-000010a0: 706f 7274 2044 6174 6162 7269 636b 7343  port DatabricksC
-000010b0: 7265 6465 6e74 6961 6c73 0a66 726f 6d20  redentials.from 
-000010c0: 7072 6566 6563 745f 6461 7461 6272 6963  prefect_databric
-000010d0: 6b73 2e6a 6f62 7320 696d 706f 7274 206a  ks.jobs import j
-000010e0: 6f62 735f 7275 6e73 5f73 7562 6d69 740a  obs_runs_submit.
-000010f0: 6672 6f6d 2070 7265 6665 6374 5f64 6174  from prefect_dat
-00001100: 6162 7269 636b 732e 6d6f 6465 6c73 2e6a  abricks.models.j
-00001110: 6f62 7320 696d 706f 7274 2028 0a20 2020  obs import (.   
-00001120: 2041 7574 6f53 6361 6c65 2c0a 2020 2020   AutoScale,.    
-00001130: 4177 7341 7474 7269 6275 7465 732c 0a20  AwsAttributes,. 
-00001140: 2020 204a 6f62 5461 736b 5365 7474 696e     JobTaskSettin
-00001150: 6773 2c0a 2020 2020 4e6f 7465 626f 6f6b  gs,.    Notebook
-00001160: 5461 736b 2c0a 2020 2020 4e65 7743 6c75  Task,.    NewClu
-00001170: 7374 6572 2c0a 290a 0a0a 4066 6c6f 770a  ster,.)...@flow.
-00001180: 6465 6620 6a6f 6273 5f72 756e 735f 7375  def jobs_runs_su
-00001190: 626d 6974 5f66 6c6f 7728 6e6f 7465 626f  bmit_flow(notebo
-000011a0: 6f6b 5f70 6174 682c 202a 2a62 6173 655f  ok_path, **base_
-000011b0: 7061 7261 6d65 7465 7273 293a 0a20 2020  parameters):.   
-000011c0: 2064 6174 6162 7269 636b 735f 6372 6564   databricks_cred
-000011d0: 656e 7469 616c 7320 3d20 4461 7461 6272  entials = Databr
-000011e0: 6963 6b73 4372 6564 656e 7469 616c 732e  icksCredentials.
-000011f0: 6c6f 6164 2822 6d79 2d62 6c6f 636b 2229  load("my-block")
-00001200: 0a0a 2020 2020 2320 7370 6563 6966 7920  ..    # specify 
-00001210: 6e65 7720 636c 7573 7465 7220 7365 7474  new cluster sett
-00001220: 696e 6773 0a20 2020 2061 7773 5f61 7474  ings.    aws_att
-00001230: 7269 6275 7465 7320 3d20 4177 7341 7474  ributes = AwsAtt
-00001240: 7269 6275 7465 7328 0a20 2020 2020 2020  ributes(.       
-00001250: 2061 7661 696c 6162 696c 6974 793d 2253   availability="S
-00001260: 504f 5422 2c0a 2020 2020 2020 2020 7a6f  POT",.        zo
-00001270: 6e65 5f69 643d 2275 732d 7765 7374 2d32  ne_id="us-west-2
-00001280: 6122 2c0a 2020 2020 2020 2020 6562 735f  a",.        ebs_
-00001290: 766f 6c75 6d65 5f74 7970 653d 2247 454e  volume_type="GEN
-000012a0: 4552 414c 5f50 5552 504f 5345 5f53 5344  ERAL_PURPOSE_SSD
-000012b0: 222c 0a20 2020 2020 2020 2065 6273 5f76  ",.        ebs_v
-000012c0: 6f6c 756d 655f 636f 756e 743d 332c 0a20  olume_count=3,. 
-000012d0: 2020 2020 2020 2065 6273 5f76 6f6c 756d         ebs_volum
-000012e0: 655f 7369 7a65 3d31 3030 2c0a 2020 2020  e_size=100,.    
-000012f0: 290a 2020 2020 6175 746f 5f73 6361 6c65  ).    auto_scale
-00001300: 203d 2041 7574 6f53 6361 6c65 286d 696e   = AutoScale(min
-00001310: 5f77 6f72 6b65 7273 3d31 2c20 6d61 785f  _workers=1, max_
-00001320: 776f 726b 6572 733d 3229 0a20 2020 206e  workers=2).    n
-00001330: 6577 5f63 6c75 7374 6572 203d 204e 6577  ew_cluster = New
-00001340: 436c 7573 7465 7228 0a20 2020 2020 2020  Cluster(.       
-00001350: 2061 7773 5f61 7474 7269 6275 7465 733d   aws_attributes=
-00001360: 6177 735f 6174 7472 6962 7574 6573 2c0a  aws_attributes,.
-00001370: 2020 2020 2020 2020 6175 746f 7363 616c          autoscal
-00001380: 653d 6175 746f 5f73 6361 6c65 2c0a 2020  e=auto_scale,.  
-00001390: 2020 2020 2020 6e6f 6465 5f74 7970 655f        node_type_
-000013a0: 6964 3d22 6d34 2e6c 6172 6765 222c 0a20  id="m4.large",. 
-000013b0: 2020 2020 2020 2073 7061 726b 5f76 6572         spark_ver
-000013c0: 7369 6f6e 3d22 3130 2e34 2e78 2d73 6361  sion="10.4.x-sca
-000013d0: 6c61 322e 3132 222c 0a20 2020 2020 2020  la2.12",.       
-000013e0: 2073 7061 726b 5f63 6f6e 663d 7b22 7370   spark_conf={"sp
-000013f0: 6172 6b2e 7370 6563 756c 6174 696f 6e22  ark.speculation"
-00001400: 3a20 5472 7565 7d2c 0a20 2020 2029 0a0a  : True},.    )..
-00001410: 2020 2020 2320 7370 6563 6966 7920 6e6f      # specify no
-00001420: 7465 626f 6f6b 2074 6f20 7573 6520 616e  tebook to use an
-00001430: 6420 7061 7261 6d65 7465 7273 2074 6f20  d parameters to 
-00001440: 7061 7373 0a20 2020 206e 6f74 6562 6f6f  pass.    noteboo
-00001450: 6b5f 7461 736b 203d 204e 6f74 6562 6f6f  k_task = Noteboo
-00001460: 6b54 6173 6b28 0a20 2020 2020 2020 206e  kTask(.        n
-00001470: 6f74 6562 6f6f 6b5f 7061 7468 3d6e 6f74  otebook_path=not
-00001480: 6562 6f6f 6b5f 7061 7468 2c0a 2020 2020  ebook_path,.    
-00001490: 2020 2020 6261 7365 5f70 6172 616d 6574      base_paramet
-000014a0: 6572 733d 6261 7365 5f70 6172 616d 6574  ers=base_paramet
-000014b0: 6572 732c 0a20 2020 2029 0a0a 2020 2020  ers,.    )..    
-000014c0: 2320 636f 6d70 696c 6520 6a6f 6220 7461  # compile job ta
-000014d0: 736b 2073 6574 7469 6e67 730a 2020 2020  sk settings.    
-000014e0: 6a6f 625f 7461 736b 5f73 6574 7469 6e67  job_task_setting
-000014f0: 7320 3d20 4a6f 6254 6173 6b53 6574 7469  s = JobTaskSetti
-00001500: 6e67 7328 0a20 2020 2020 2020 206e 6577  ngs(.        new
-00001510: 5f63 6c75 7374 6572 3d6e 6577 5f63 6c75  _cluster=new_clu
-00001520: 7374 6572 2c0a 2020 2020 2020 2020 6e6f  ster,.        no
-00001530: 7465 626f 6f6b 5f74 6173 6b3d 6e6f 7465  tebook_task=note
-00001540: 626f 6f6b 5f74 6173 6b2c 0a20 2020 2020  book_task,.     
-00001550: 2020 2074 6173 6b5f 6b65 793d 2270 7265     task_key="pre
-00001560: 6665 6374 2d74 6173 6b22 0a20 2020 2029  fect-task".    )
-00001570: 0a0a 2020 2020 7275 6e20 3d20 6a6f 6273  ..    run = jobs
-00001580: 5f72 756e 735f 7375 626d 6974 280a 2020  _runs_submit(.  
-00001590: 2020 2020 2020 6461 7461 6272 6963 6b73        databricks
-000015a0: 5f63 7265 6465 6e74 6961 6c73 3d64 6174  _credentials=dat
-000015b0: 6162 7269 636b 735f 6372 6564 656e 7469  abricks_credenti
-000015c0: 616c 732c 0a20 2020 2020 2020 2072 756e  als,.        run
-000015d0: 5f6e 616d 653d 2270 7265 6665 6374 2d6a  _name="prefect-j
-000015e0: 6f62 222c 0a20 2020 2020 2020 2074 6173  ob",.        tas
-000015f0: 6b73 3d5b 6a6f 625f 7461 736b 5f73 6574  ks=[job_task_set
-00001600: 7469 6e67 735d 0a20 2020 2029 0a0a 2020  tings].    )..  
-00001610: 2020 7265 7475 726e 2072 756e 0a0a 0a6a    return run...j
-00001620: 6f62 735f 7275 6e73 5f73 7562 6d69 745f  obs_runs_submit_
-00001630: 666c 6f77 2822 2f55 7365 7273 2f75 7365  flow("/Users/use
-00001640: 726e 616d 6540 676d 6169 6c2e 636f 6d2f  rname@gmail.com/
-00001650: 6578 616d 706c 652e 6970 796e 6222 2c20  example.ipynb", 
-00001660: 6e61 6d65 3d22 4d61 7276 696e 2229 0a60  name="Marvin").`
-00001670: 6060 0a0a 4e6f 7465 2c20 696e 7374 6561  ``..Note, instea
-00001680: 6420 6f66 2075 7369 6e67 2074 6865 2062  d of using the b
-00001690: 7569 6c74 2d69 6e20 6d6f 6465 6c73 2c20  uilt-in models, 
-000016a0: 796f 7520 6d61 7920 616c 736f 2069 6e70  you may also inp
-000016b0: 7574 2076 616c 6964 204a 534f 4e2e 2046  ut valid JSON. F
-000016c0: 6f72 2065 7861 6d70 6c65 2c20 6041 7574  or example, `Aut
-000016d0: 6f53 6361 6c65 286d 696e 5f77 6f72 6b65  oScale(min_worke
-000016e0: 7273 3d31 2c20 6d61 785f 776f 726b 6572  rs=1, max_worker
-000016f0: 733d 3229 6020 6973 2065 7175 6976 616c  s=2)` is equival
-00001700: 656e 7420 746f 2060 7b22 6d69 6e5f 776f  ent to `{"min_wo
-00001710: 726b 6572 7322 3a20 312c 2022 6d61 785f  rkers": 1, "max_
-00001720: 776f 726b 6572 7322 3a20 327d 602e 0a0a  workers": 2}`...
-00001730: 466f 7220 6d6f 7265 2074 6970 7320 6f6e  For more tips on
-00001740: 2068 6f77 2074 6f20 7573 6520 7461 736b   how to use task
-00001750: 7320 616e 6420 666c 6f77 7320 696e 2061  s and flows in a
-00001760: 2043 6f6c 6c65 6374 696f 6e2c 2063 6865   Collection, che
-00001770: 636b 206f 7574 205b 5573 696e 6720 436f  ck out [Using Co
-00001780: 6c6c 6563 7469 6f6e 735d 2868 7474 7073  llections](https
-00001790: 3a2f 2f6f 7269 6f6e 2d64 6f63 732e 7072  ://orion-docs.pr
-000017a0: 6566 6563 742e 696f 2f63 6f6c 6c65 6374  efect.io/collect
-000017b0: 696f 6e73 2f75 7361 6765 2f29 210a 0a23  ions/usage/)!..#
-000017c0: 2320 5265 736f 7572 6365 730a 0a49 6620  # Resources..If 
-000017d0: 796f 7520 656e 636f 756e 7465 7220 616e  you encounter an
-000017e0: 7920 6275 6773 2077 6869 6c65 2075 7369  y bugs while usi
-000017f0: 6e67 2060 7072 6566 6563 742d 6461 7461  ng `prefect-data
-00001800: 6272 6963 6b73 602c 2066 6565 6c20 6672  bricks`, feel fr
-00001810: 6565 2074 6f20 6f70 656e 2061 6e20 6973  ee to open an is
-00001820: 7375 6520 696e 2074 6865 205b 7072 6566  sue in the [pref
-00001830: 6563 742d 6461 7461 6272 6963 6b73 5d28  ect-databricks](
-00001840: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001850: 6f6d 2f50 7265 6665 6374 4851 2f70 7265  om/PrefectHQ/pre
-00001860: 6665 6374 2d64 6174 6162 7269 636b 7329  fect-databricks)
-00001870: 2072 6570 6f73 6974 6f72 792e 0a0a 4966   repository...If
-00001880: 2079 6f75 2068 6176 6520 616e 7920 7175   you have any qu
-00001890: 6573 7469 6f6e 7320 6f72 2069 7373 7565  estions or issue
-000018a0: 7320 7768 696c 6520 7573 696e 6720 6070  s while using `p
-000018b0: 7265 6665 6374 2d64 6174 6162 7269 636b  refect-databrick
-000018c0: 7360 2c20 796f 7520 6361 6e20 6669 6e64  s`, you can find
-000018d0: 2068 656c 7020 696e 2065 6974 6865 7220   help in either 
-000018e0: 7468 6520 5b50 7265 6665 6374 2044 6973  the [Prefect Dis
-000018f0: 636f 7572 7365 2066 6f72 756d 5d28 6874  course forum](ht
-00001900: 7470 733a 2f2f 6469 7363 6f75 7273 652e  tps://discourse.
-00001910: 7072 6566 6563 742e 696f 2f29 206f 7220  prefect.io/) or 
-00001920: 7468 6520 5b50 7265 6665 6374 2053 6c61  the [Prefect Sla
-00001930: 636b 2063 6f6d 6d75 6e69 7479 5d28 6874  ck community](ht
-00001940: 7470 733a 2f2f 7072 6566 6563 742e 696f  tps://prefect.io
-00001950: 2f73 6c61 636b 292e 0a0a 4665 656c 2066  /slack)...Feel f
-00001960: 7265 6520 746f 2073 7461 7220 6f72 2077  ree to star or w
-00001970: 6174 6368 205b 6070 7265 6665 6374 2d64  atch [`prefect-d
-00001980: 6174 6162 7269 636b 7360 5d28 6874 7470  atabricks`](http
-00001990: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f50  s://github.com/P
-000019a0: 7265 6665 6374 4851 2f70 7265 6665 6374  refectHQ/prefect
-000019b0: 2d64 6174 6162 7269 636b 7329 2066 6f72  -databricks) for
-000019c0: 2075 7064 6174 6573 2074 6f6f 210a 0a23   updates too!..#
-000019d0: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
-000019e0: 4966 2079 6f75 2764 206c 696b 6520 746f  If you'd like to
-000019f0: 2068 656c 7020 636f 6e74 7269 6275 7465   help contribute
-00001a00: 2074 6f20 6669 7820 616e 2069 7373 7565   to fix an issue
-00001a10: 206f 7220 6164 6420 6120 6665 6174 7572   or add a featur
-00001a20: 6520 746f 2060 7072 6566 6563 742d 6461  e to `prefect-da
-00001a30: 7461 6272 6963 6b73 602c 2070 6c65 6173  tabricks`, pleas
-00001a40: 6520 5b70 726f 706f 7365 2063 6861 6e67  e [propose chang
-00001a50: 6573 2074 6872 6f75 6768 2061 2070 756c  es through a pul
-00001a60: 6c20 7265 7175 6573 7420 6672 6f6d 2061  l request from a
-00001a70: 2066 6f72 6b20 6f66 2074 6865 2072 6570   fork of the rep
-00001a80: 6f73 6974 6f72 795d 2868 7474 7073 3a2f  ository](https:/
-00001a90: 2f64 6f63 732e 6769 7468 7562 2e63 6f6d  /docs.github.com
-00001aa0: 2f65 6e2f 7075 6c6c 2d72 6571 7565 7374  /en/pull-request
-00001ab0: 732f 636f 6c6c 6162 6f72 6174 696e 672d  s/collaborating-
-00001ac0: 7769 7468 2d70 756c 6c2d 7265 7175 6573  with-pull-reques
-00001ad0: 7473 2f70 726f 706f 7369 6e67 2d63 6861  ts/proposing-cha
-00001ae0: 6e67 6573 2d74 6f2d 796f 7572 2d77 6f72  nges-to-your-wor
-00001af0: 6b2d 7769 7468 2d70 756c 6c2d 7265 7175  k-with-pull-requ
-00001b00: 6573 7473 2f63 7265 6174 696e 672d 612d  ests/creating-a-
-00001b10: 7075 6c6c 2d72 6571 7565 7374 2d66 726f  pull-request-fro
-00001b20: 6d2d 612d 666f 726b 292e 0a0a 4865 7265  m-a-fork)...Here
-00001b30: 2061 7265 2074 6865 2073 7465 7073 3a0a   are the steps:.
-00001b40: 312e 205b 466f 726b 2074 6865 2072 6570  1. [Fork the rep
-00001b50: 6f73 6974 6f72 795d 2868 7474 7073 3a2f  ository](https:/
-00001b60: 2f64 6f63 732e 6769 7468 7562 2e63 6f6d  /docs.github.com
-00001b70: 2f65 6e2f 6765 742d 7374 6172 7465 642f  /en/get-started/
-00001b80: 7175 6963 6b73 7461 7274 2f66 6f72 6b2d  quickstart/fork-
-00001b90: 612d 7265 706f 2366 6f72 6b69 6e67 2d61  a-repo#forking-a
-00001ba0: 2d72 6570 6f73 6974 6f72 7929 0a32 2e20  -repository).2. 
-00001bb0: 5b43 6c6f 6e65 2074 6865 2066 6f72 6b65  [Clone the forke
-00001bc0: 6420 7265 706f 7369 746f 7279 5d28 6874  d repository](ht
-00001bd0: 7470 733a 2f2f 646f 6373 2e67 6974 6875  tps://docs.githu
-00001be0: 622e 636f 6d2f 656e 2f67 6574 2d73 7461  b.com/en/get-sta
-00001bf0: 7274 6564 2f71 7569 636b 7374 6172 742f  rted/quickstart/
-00001c00: 666f 726b 2d61 2d72 6570 6f23 636c 6f6e  fork-a-repo#clon
-00001c10: 696e 672d 796f 7572 2d66 6f72 6b65 642d  ing-your-forked-
-00001c20: 7265 706f 7369 746f 7279 290a 332e 2049  repository).3. I
-00001c30: 6e73 7461 6c6c 2074 6865 2072 6570 6f73  nstall the repos
-00001c40: 6974 6f72 7920 616e 6420 6974 7320 6465  itory and its de
-00001c50: 7065 6e64 656e 6369 6573 3a0a 6060 600a  pendencies:.```.
-00001c60: 7069 7020 696e 7374 616c 6c20 2d65 2022  pip install -e "
-00001c70: 2e5b 6465 765d 220a 6060 600a 342e 204d  .[dev]".```.4. M
-00001c80: 616b 6520 6465 7369 7265 6420 6368 616e  ake desired chan
-00001c90: 6765 730a 352e 2041 6464 2074 6573 7473  ges.5. Add tests
-00001ca0: 0a36 2e20 496e 7365 7274 2061 6e20 656e  .6. Insert an en
-00001cb0: 7472 7920 746f 205b 4348 414e 4745 4c4f  try to [CHANGELO
-00001cc0: 472e 6d64 5d28 6874 7470 733a 2f2f 6769  G.md](https://gi
-00001cd0: 7468 7562 2e63 6f6d 2f50 7265 6665 6374  thub.com/Prefect
-00001ce0: 4851 2f70 7265 6665 6374 2d64 6174 6162  HQ/prefect-datab
-00001cf0: 7269 636b 732f 626c 6f62 2f6d 6169 6e2f  ricks/blob/main/
-00001d00: 4348 414e 4745 4c4f 472e 6d64 290a 372e  CHANGELOG.md).7.
-00001d10: 2049 6e73 7461 6c6c 2060 7072 652d 636f   Install `pre-co
-00001d20: 6d6d 6974 6020 746f 2070 6572 666f 726d  mmit` to perform
-00001d30: 2071 7561 6c69 7479 2063 6865 636b 7320   quality checks 
-00001d40: 7072 696f 7220 746f 2063 6f6d 6d69 743a  prior to commit:
-00001d50: 0a60 6060 0a70 7265 2d63 6f6d 6d69 7420  .```.pre-commit 
-00001d60: 696e 7374 616c 6c0a 6060 600a 382e 2060  install.```.8. `
-00001d70: 6769 7420 636f 6d6d 6974 602c 2060 6769  git commit`, `gi
-00001d80: 7420 7075 7368 602c 2061 6e64 2063 7265  t push`, and cre
-00001d90: 6174 6520 6120 7075 6c6c 2072 6571 7565  ate a pull reque
-00001da0: 7374 0a                                  st.
+00000000: 2320 496e 7465 6772 6174 6520 4461 7461  # Integrate Data
+00000010: 6272 6963 6b73 206a 6f62 7320 696e 746f  bricks jobs into
+00000020: 2079 6f75 7220 6461 7461 666c 6f77 2077   your dataflow w
+00000030: 6974 6820 7072 6566 6563 742d 6461 7461  ith prefect-data
+00000040: 6272 6963 6b73 0a20 0a3c 7020 616c 6967  bricks. .<p alig
+00000050: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+00000060: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000070: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
+00000080: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000090: 636f 6d2f 3135 3333 3139 3930 2f32 3139  com/15331990/219
+000000a0: 3832 3234 3339 2d37 3065 6338 3266 622d  822439-70ec82fb-
+000000b0: 6539 3361 2d34 3938 332d 6265 6337 2d38  e93a-4983-bec7-8
+000000c0: 6338 3235 3066 6262 3761 632e 706e 6722  c8250fbb7ac.png"
+000000d0: 3e0a 2020 2020 3c62 723e 0a20 2020 203c  >.    <br>.    <
+000000e0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000000f0: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
+00000100: 7079 7069 2f70 7265 6665 6374 2d64 6174  pypi/prefect-dat
+00000110: 6162 7269 636b 732f 2220 616c 743d 2250  abricks/" alt="P
+00000120: 7950 4920 7665 7273 696f 6e22 3e0a 2020  yPI version">.  
+00000130: 2020 2020 2020 3c69 6d67 2061 6c74 3d22        <img alt="
+00000140: 5079 5049 2220 7372 633d 2268 7474 7073  PyPI" src="https
+00000150: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000160: 6f2f 7079 7069 2f76 2f70 7265 6665 6374  o/pypi/v/prefect
+00000170: 2d64 6174 6162 7269 636b 733f 636f 6c6f  -databricks?colo
+00000180: 723d 3030 3532 4646 266c 6162 656c 436f  r=0052FF&labelCo
+00000190: 6c6f 723d 3039 3034 3232 223e 3c2f 613e  lor=090422"></a>
+000001a0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+000001b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001c0: 2f50 7265 6665 6374 4851 2f70 7265 6665  /PrefectHQ/prefe
+000001d0: 6374 2d64 6174 6162 7269 636b 732f 2220  ct-databricks/" 
+000001e0: 616c 743d 2253 7461 7273 223e 0a20 2020  alt="Stars">.   
+000001f0: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+00000200: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000210: 6473 2e69 6f2f 6769 7468 7562 2f73 7461  ds.io/github/sta
+00000220: 7273 2f50 7265 6665 6374 4851 2f70 7265  rs/PrefectHQ/pre
+00000230: 6665 6374 2d64 6174 6162 7269 636b 733f  fect-databricks?
+00000240: 636f 6c6f 723d 3030 3532 4646 266c 6162  color=0052FF&lab
+00000250: 656c 436f 6c6f 723d 3039 3034 3232 2220  elColor=090422" 
+00000260: 2f3e 3c2f 613e 0a20 2020 203c 6120 6872  /></a>.    <a hr
+00000270: 6566 3d22 6874 7470 733a 2f2f 7065 7079  ef="https://pepy
+00000280: 2e74 6563 682f 6261 6467 652f 7072 6566  .tech/badge/pref
+00000290: 6563 742d 6461 7461 6272 6963 6b73 2f22  ect-databricks/"
+000002a0: 2061 6c74 3d22 446f 776e 6c6f 6164 7322   alt="Downloads"
+000002b0: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
+000002c0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000002d0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000002e0: 646d 2f70 7265 6665 6374 2d64 6174 6162  dm/prefect-datab
+000002f0: 7269 636b 733f 636f 6c6f 723d 3030 3532  ricks?color=0052
+00000300: 4646 266c 6162 656c 436f 6c6f 723d 3039  FF&labelColor=09
+00000310: 3034 3232 2220 2f3e 3c2f 613e 0a20 2020  0422" /></a>.   
+00000320: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000330: 2f2f 6769 7468 7562 2e63 6f6d 2f50 7265  //github.com/Pre
+00000340: 6665 6374 4851 2f70 7265 6665 6374 2d64  fectHQ/prefect-d
+00000350: 6174 6162 7269 636b 732f 7075 6c73 6522  atabricks/pulse"
+00000360: 2061 6c74 3d22 4163 7469 7669 7479 223e   alt="Activity">
+00000370: 0a20 2020 2020 2020 203c 696d 6720 7372  .        <img sr
+00000380: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000390: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+000003a0: 2f63 6f6d 6d69 742d 6163 7469 7669 7479  /commit-activity
+000003b0: 2f6d 2f50 7265 6665 6374 4851 2f70 7265  /m/PrefectHQ/pre
+000003c0: 6665 6374 2d64 6174 6162 7269 636b 733f  fect-databricks?
+000003d0: 636f 6c6f 723d 3030 3532 4646 266c 6162  color=0052FF&lab
+000003e0: 656c 436f 6c6f 723d 3039 3034 3232 2220  elColor=090422" 
+000003f0: 2f3e 3c2f 613e 0a20 2020 203c 6272 3e0a  /></a>.    <br>.
+00000400: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000410: 7073 3a2f 2f70 7265 6665 6374 2d63 6f6d  ps://prefect-com
+00000420: 6d75 6e69 7479 2e73 6c61 636b 2e63 6f6d  munity.slack.com
+00000430: 2220 616c 743d 2253 6c61 636b 223e 0a20  " alt="Slack">. 
+00000440: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+00000450: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000460: 656c 6473 2e69 6f2f 6261 6467 652f 736c  elds.io/badge/sl
+00000470: 6163 6b2d 6a6f 696e 5f63 6f6d 6d75 6e69  ack-join_communi
+00000480: 7479 2d72 6564 2e73 7667 3f63 6f6c 6f72  ty-red.svg?color
+00000490: 3d30 3035 3246 4626 6c61 6265 6c43 6f6c  =0052FF&labelCol
+000004a0: 6f72 3d30 3930 3432 3226 6c6f 676f 3d73  or=090422&logo=s
+000004b0: 6c61 636b 2220 2f3e 3c2f 613e 0a20 2020  lack" /></a>.   
+000004c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000004d0: 2f2f 6469 7363 6f75 7273 652e 7072 6566  //discourse.pref
+000004e0: 6563 742e 696f 2f22 2061 6c74 3d22 4469  ect.io/" alt="Di
+000004f0: 7363 6f75 7273 6522 3e0a 2020 2020 2020  scourse">.      
+00000500: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000510: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000520: 696f 2f62 6164 6765 2f64 6973 636f 7572  io/badge/discour
+00000530: 7365 2d62 726f 7773 655f 666f 7275 6d2d  se-browse_forum-
+00000540: 7265 642e 7376 673f 636f 6c6f 723d 3030  red.svg?color=00
+00000550: 3532 4646 266c 6162 656c 436f 6c6f 723d  52FF&labelColor=
+00000560: 3039 3034 3232 266c 6f67 6f3d 6469 7363  090422&logo=disc
+00000570: 6f75 7273 6522 202f 3e3c 2f61 3e0a 3c2f  ourse" /></a>.</
+00000580: 703e 0a0a 5669 7369 7420 7468 6520 6675  p>..Visit the fu
+00000590: 6c6c 2064 6f63 7320 5b68 6572 655d 2868  ll docs [here](h
+000005a0: 7474 7073 3a2f 2f50 7265 6665 6374 4851  ttps://PrefectHQ
+000005b0: 2e67 6974 6875 622e 696f 2f70 7265 6665  .github.io/prefe
+000005c0: 6374 2d64 6174 6162 7269 636b 7329 2074  ct-databricks) t
+000005d0: 6f20 7365 6520 6164 6469 7469 6f6e 616c  o see additional
+000005e0: 2065 7861 6d70 6c65 7320 616e 6420 7468   examples and th
+000005f0: 6520 4150 4920 7265 6665 7265 6e63 652e  e API reference.
+00000600: 0a0a 5468 6520 7072 6566 6563 742d 6461  ..The prefect-da
+00000610: 7461 6272 6963 6b73 2063 6f6c 6c65 6374  tabricks collect
+00000620: 696f 6e20 6d61 6b65 7320 6974 2065 6173  ion makes it eas
+00000630: 7920 746f 2063 6f6f 7264 6961 6e74 6520  y to coordiante 
+00000640: 4461 7461 6272 6963 6b73 206a 6f62 7320  Databricks jobs 
+00000650: 7769 7468 206f 7468 6572 2074 6f6f 6c73  with other tools
+00000660: 2069 6e20 796f 7572 2064 6174 6120 7374   in your data st
+00000670: 6163 6b20 7573 696e 6720 5072 6566 6563  ack using Prefec
+00000680: 742e 2043 6865 636b 206f 7574 2074 6865  t. Check out the
+00000690: 2065 7861 6d70 6c65 7320 6265 6c6f 7720   examples below 
+000006a0: 746f 2067 6574 2073 7461 7274 6564 210a  to get started!.
+000006b0: 0a23 2320 4765 7474 696e 6720 5374 6172  .## Getting Star
+000006c0: 7465 640a 0a23 2323 2049 6e74 6567 7261  ted..### Integra
+000006d0: 7465 2077 6974 6820 5072 6566 6563 7420  te with Prefect 
+000006e0: 666c 6f77 730a 0a55 7369 6e67 2050 7265  flows..Using Pre
+000006f0: 6665 6374 2077 6974 6820 4461 7461 6272  fect with Databr
+00000700: 6963 6b73 2061 6c6c 6f77 7320 796f 7520  icks allows you 
+00000710: 746f 2064 6566 696e 6520 616e 6420 6f72  to define and or
+00000720: 6368 6573 7472 6174 6520 636f 6d70 6c65  chestrate comple
+00000730: 7820 6461 7461 2077 6f72 6b66 6c6f 7773  x data workflows
+00000740: 2074 6861 7420 7461 6b65 2061 6476 616e   that take advan
+00000750: 7461 6765 206f 6620 7468 6520 7363 616c  tage of the scal
+00000760: 6162 696c 6974 7920 616e 6420 7065 7266  ability and perf
+00000770: 6f72 6d61 6e63 6520 6f66 2044 6174 6162  ormance of Datab
+00000780: 7269 636b 732e 0a0a 5468 6973 2063 616e  ricks...This can
+00000790: 2062 6520 6573 7065 6369 616c 6c79 2075   be especially u
+000007a0: 7365 6675 6c20 666f 7220 6461 7461 2d69  seful for data-i
+000007b0: 6e74 656e 7369 7665 2074 6173 6b73 2073  ntensive tasks s
+000007c0: 7563 6820 6173 2045 544c 2028 6578 7472  uch as ETL (extr
+000007d0: 6163 742c 2074 7261 6e73 666f 726d 2c20  act, transform, 
+000007e0: 6c6f 6164 2920 7069 7065 6c69 6e65 732c  load) pipelines,
+000007f0: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
+00000800: 6720 7472 6169 6e69 6e67 2061 6e64 2069  g training and i
+00000810: 6e66 6572 656e 6365 2c20 616e 6420 7265  nference, and re
+00000820: 616c 2d74 696d 6520 6461 7461 2070 726f  al-time data pro
+00000830: 6365 7373 696e 672e 0a0a 4265 6c6f 7720  cessing...Below 
+00000840: 6973 2061 6e20 6578 616d 706c 6520 6f66  is an example of
+00000850: 2068 6f77 2079 6f75 2063 616e 2069 6e63   how you can inc
+00000860: 6f72 706f 7261 7465 2044 6174 6162 7269  orporate Databri
+00000870: 636b 7320 6e6f 7465 626f 6f6b 7320 7769  cks notebooks wi
+00000880: 7468 696e 2079 6f75 7220 5072 6566 6563  thin your Prefec
+00000890: 7420 666c 6f77 732e 0a0a 4265 2073 7572  t flows...Be sur
+000008a0: 6520 746f 2069 6e73 7461 6c6c 205b 7072  e to install [pr
+000008b0: 6566 6563 742d 6461 7461 6272 6963 6b73  efect-databricks
+000008c0: 5d28 2369 6e73 7461 6c6c 6174 696f 6e29  ](#installation)
+000008d0: 2061 6e64 205b 7361 7665 2061 2063 7265   and [save a cre
+000008e0: 6465 6e74 6961 6c73 2062 6c6f 636b 5d28  dentials block](
+000008f0: 2373 6176 696e 672d 6372 6564 656e 7469  #saving-credenti
+00000900: 616c 732d 746f 2d62 6c6f 636b 2920 746f  als-to-block) to
+00000910: 2072 756e 2074 6865 2065 7861 6d70 6c65   run the example
+00000920: 7320 6265 6c6f 7721 0a0a 4966 2079 6f75  s below!..If you
+00000930: 2064 6f6e 2774 2068 6176 6520 616e 2065   don't have an e
+00000940: 7869 7374 696e 6720 6e6f 7465 626f 6f6b  xisting notebook
+00000950: 2072 6561 6479 206f 6e20 4461 7461 6272   ready on Databr
+00000960: 6963 6b73 2c20 796f 7520 6361 6e20 636f  icks, you can co
+00000970: 7079 2074 6865 2066 6f6c 6c6f 7769 6e67  py the following
+00000980: 2c20 616e 6420 6e61 6d65 2069 7420 6065  , and name it `e
+00000990: 7861 6d70 6c65 2e69 7079 6e62 602e 2054  xample.ipynb`. T
+000009a0: 6869 7320 6e6f 7465 626f 6f6b 2c20 6163  his notebook, ac
+000009b0: 6365 7074 7320 6120 6e61 6d65 2070 6172  cepts a name par
+000009c0: 616d 6574 6572 2066 726f 6d20 7468 6520  ameter from the 
+000009d0: 666c 6f77 2061 6e64 2073 696d 706c 7920  flow and simply 
+000009e0: 7072 696e 7473 2061 206d 6573 7361 6765  prints a message
+000009f0: 2e0a 0a60 6060 7079 7468 6f6e 0a6e 616d  ...```python.nam
+00000a00: 6520 3d20 6462 7574 696c 732e 7769 6467  e = dbutils.widg
+00000a10: 6574 732e 6765 7428 226e 616d 6522 290a  ets.get("name").
+00000a20: 6d65 7373 6167 6520 3d20 6622 446f 6e27  message = f"Don'
+00000a30: 7420 776f 7272 7920 7b6e 616d 657d 2c20  t worry {name}, 
+00000a40: 4920 676f 7420 796f 7572 2072 6571 7565  I got your reque
+00000a50: 7374 2120 5765 6c63 6f6d 6520 746f 2070  st! Welcome to p
+00000a60: 7265 6665 6374 2d64 6174 6162 7269 636b  refect-databrick
+00000a70: 7321 220a 7072 696e 7428 6d65 7373 6167  s!".print(messag
+00000a80: 6529 0a60 6060 0a0a 4865 7265 2c20 7468  e).```..Here, th
+00000a90: 6520 666c 6f77 206c 6175 6e63 6865 7320  e flow launches 
+00000aa0: 6120 6e65 7720 636c 7573 7465 7220 746f  a new cluster to
+00000ab0: 2072 756e 2060 6578 616d 706c 652e 6970   run `example.ip
+00000ac0: 796e 6260 2061 6e64 2077 6169 7473 2066  ynb` and waits f
+00000ad0: 6f72 2074 6865 2063 6f6d 706c 6574 696f  or the completio
+00000ae0: 6e20 6f66 2074 6865 206e 6f74 6562 6f6f  n of the noteboo
+00000af0: 6b20 7275 6e2e 2052 6570 6c61 6365 2074  k run. Replace t
+00000b00: 6865 2070 6c61 6365 686f 6c64 6572 7320  he placeholders 
+00000b10: 616e 6420 7275 6e2e 0a0a 6060 6070 7974  and run...```pyt
+00000b20: 686f 6e0a 6672 6f6d 2070 7265 6665 6374  hon.from prefect
+00000b30: 2069 6d70 6f72 7420 666c 6f77 0a66 726f   import flow.fro
+00000b40: 6d20 7072 6566 6563 745f 6461 7461 6272  m prefect_databr
+00000b50: 6963 6b73 2069 6d70 6f72 7420 4461 7461  icks import Data
+00000b60: 6272 6963 6b73 4372 6564 656e 7469 616c  bricksCredential
+00000b70: 730a 6672 6f6d 2070 7265 6665 6374 5f64  s.from prefect_d
+00000b80: 6174 6162 7269 636b 732e 666c 6f77 7320  atabricks.flows 
+00000b90: 696d 706f 7274 206a 6f62 735f 7275 6e73  import jobs_runs
+00000ba0: 5f73 7562 6d69 745f 616e 645f 7761 6974  _submit_and_wait
+00000bb0: 5f66 6f72 5f63 6f6d 706c 6574 696f 6e0a  _for_completion.
+00000bc0: 6672 6f6d 2070 7265 6665 6374 5f64 6174  from prefect_dat
+00000bd0: 6162 7269 636b 732e 6d6f 6465 6c73 2e6a  abricks.models.j
+00000be0: 6f62 7320 696d 706f 7274 2028 0a20 2020  obs import (.   
+00000bf0: 2041 7574 6f53 6361 6c65 2c0a 2020 2020   AutoScale,.    
+00000c00: 4177 7341 7474 7269 6275 7465 732c 0a20  AwsAttributes,. 
+00000c10: 2020 204a 6f62 5461 736b 5365 7474 696e     JobTaskSettin
+00000c20: 6773 2c0a 2020 2020 4e6f 7465 626f 6f6b  gs,.    Notebook
+00000c30: 5461 736b 2c0a 2020 2020 4e65 7743 6c75  Task,.    NewClu
+00000c40: 7374 6572 2c0a 290a 0a0a 4066 6c6f 770a  ster,.)...@flow.
+00000c50: 6465 6620 6a6f 6273 5f72 756e 735f 7375  def jobs_runs_su
+00000c60: 626d 6974 5f66 6c6f 7728 626c 6f63 6b5f  bmit_flow(block_
+00000c70: 6e61 6d65 3a20 7374 722c 206e 6f74 6562  name: str, noteb
+00000c80: 6f6f 6b5f 7061 7468 3a20 7374 722c 202a  ook_path: str, *
+00000c90: 2a62 6173 655f 7061 7261 6d65 7465 7273  *base_parameters
+00000ca0: 293a 0a20 2020 2064 6174 6162 7269 636b  ):.    databrick
+00000cb0: 735f 6372 6564 656e 7469 616c 7320 3d20  s_credentials = 
+00000cc0: 4461 7461 6272 6963 6b73 4372 6564 656e  DatabricksCreden
+00000cd0: 7469 616c 732e 6c6f 6164 2862 6c6f 636b  tials.load(block
+00000ce0: 5f6e 616d 6529 0a0a 2020 2020 2320 7370  _name)..    # sp
+00000cf0: 6563 6966 7920 6e65 7720 636c 7573 7465  ecify new cluste
+00000d00: 7220 7365 7474 696e 6773 0a20 2020 2061  r settings.    a
+00000d10: 7773 5f61 7474 7269 6275 7465 7320 3d20  ws_attributes = 
+00000d20: 4177 7341 7474 7269 6275 7465 7328 0a20  AwsAttributes(. 
+00000d30: 2020 2020 2020 2061 7661 696c 6162 696c         availabil
+00000d40: 6974 793d 2253 504f 5422 2c0a 2020 2020  ity="SPOT",.    
+00000d50: 2020 2020 7a6f 6e65 5f69 643d 2275 732d      zone_id="us-
+00000d60: 7765 7374 2d32 6122 2c0a 2020 2020 2020  west-2a",.      
+00000d70: 2020 6562 735f 766f 6c75 6d65 5f74 7970    ebs_volume_typ
+00000d80: 653d 2247 454e 4552 414c 5f50 5552 504f  e="GENERAL_PURPO
+00000d90: 5345 5f53 5344 222c 0a20 2020 2020 2020  SE_SSD",.       
+00000da0: 2065 6273 5f76 6f6c 756d 655f 636f 756e   ebs_volume_coun
+00000db0: 743d 332c 0a20 2020 2020 2020 2065 6273  t=3,.        ebs
+00000dc0: 5f76 6f6c 756d 655f 7369 7a65 3d31 3030  _volume_size=100
+00000dd0: 2c0a 2020 2020 290a 2020 2020 6175 746f  ,.    ).    auto
+00000de0: 5f73 6361 6c65 203d 2041 7574 6f53 6361  _scale = AutoSca
+00000df0: 6c65 286d 696e 5f77 6f72 6b65 7273 3d31  le(min_workers=1
+00000e00: 2c20 6d61 785f 776f 726b 6572 733d 3229  , max_workers=2)
+00000e10: 0a20 2020 206e 6577 5f63 6c75 7374 6572  .    new_cluster
+00000e20: 203d 204e 6577 436c 7573 7465 7228 0a20   = NewCluster(. 
+00000e30: 2020 2020 2020 2061 7773 5f61 7474 7269         aws_attri
+00000e40: 6275 7465 733d 6177 735f 6174 7472 6962  butes=aws_attrib
+00000e50: 7574 6573 2c0a 2020 2020 2020 2020 6175  utes,.        au
+00000e60: 746f 7363 616c 653d 6175 746f 5f73 6361  toscale=auto_sca
+00000e70: 6c65 2c0a 2020 2020 2020 2020 6e6f 6465  le,.        node
+00000e80: 5f74 7970 655f 6964 3d22 6d34 2e6c 6172  _type_id="m4.lar
+00000e90: 6765 222c 0a20 2020 2020 2020 2073 7061  ge",.        spa
+00000ea0: 726b 5f76 6572 7369 6f6e 3d22 3130 2e34  rk_version="10.4
+00000eb0: 2e78 2d73 6361 6c61 322e 3132 222c 0a20  .x-scala2.12",. 
+00000ec0: 2020 2020 2020 2073 7061 726b 5f63 6f6e         spark_con
+00000ed0: 663d 7b22 7370 6172 6b2e 7370 6563 756c  f={"spark.specul
+00000ee0: 6174 696f 6e22 3a20 5472 7565 7d2c 0a20  ation": True},. 
+00000ef0: 2020 2029 0a0a 2020 2020 2320 7370 6563     )..    # spec
+00000f00: 6966 7920 6e6f 7465 626f 6f6b 2074 6f20  ify notebook to 
+00000f10: 7573 6520 616e 6420 7061 7261 6d65 7465  use and paramete
+00000f20: 7273 2074 6f20 7061 7373 0a20 2020 206e  rs to pass.    n
+00000f30: 6f74 6562 6f6f 6b5f 7461 736b 203d 204e  otebook_task = N
+00000f40: 6f74 6562 6f6f 6b54 6173 6b28 0a20 2020  otebookTask(.   
+00000f50: 2020 2020 206e 6f74 6562 6f6f 6b5f 7061       notebook_pa
+00000f60: 7468 3d6e 6f74 6562 6f6f 6b5f 7061 7468  th=notebook_path
+00000f70: 2c0a 2020 2020 2020 2020 6261 7365 5f70  ,.        base_p
+00000f80: 6172 616d 6574 6572 733d 6261 7365 5f70  arameters=base_p
+00000f90: 6172 616d 6574 6572 732c 0a20 2020 2029  arameters,.    )
+00000fa0: 0a0a 2020 2020 2320 636f 6d70 696c 6520  ..    # compile 
+00000fb0: 6a6f 6220 7461 736b 2073 6574 7469 6e67  job task setting
+00000fc0: 730a 2020 2020 6a6f 625f 7461 736b 5f73  s.    job_task_s
+00000fd0: 6574 7469 6e67 7320 3d20 4a6f 6254 6173  ettings = JobTas
+00000fe0: 6b53 6574 7469 6e67 7328 0a20 2020 2020  kSettings(.     
+00000ff0: 2020 206e 6577 5f63 6c75 7374 6572 3d6e     new_cluster=n
+00001000: 6577 5f63 6c75 7374 6572 2c0a 2020 2020  ew_cluster,.    
+00001010: 2020 2020 6e6f 7465 626f 6f6b 5f74 6173      notebook_tas
+00001020: 6b3d 6e6f 7465 626f 6f6b 5f74 6173 6b2c  k=notebook_task,
+00001030: 0a20 2020 2020 2020 2074 6173 6b5f 6b65  .        task_ke
+00001040: 793d 2270 7265 6665 6374 2d74 6173 6b22  y="prefect-task"
+00001050: 0a20 2020 2029 0a0a 2020 2020 7275 6e20  .    )..    run 
+00001060: 3d20 6a6f 6273 5f72 756e 735f 7375 626d  = jobs_runs_subm
+00001070: 6974 5f61 6e64 5f77 6169 745f 666f 725f  it_and_wait_for_
+00001080: 636f 6d70 6c65 7469 6f6e 280a 2020 2020  completion(.    
+00001090: 2020 2020 6461 7461 6272 6963 6b73 5f63      databricks_c
+000010a0: 7265 6465 6e74 6961 6c73 3d64 6174 6162  redentials=datab
+000010b0: 7269 636b 735f 6372 6564 656e 7469 616c  ricks_credential
+000010c0: 732c 0a20 2020 2020 2020 2072 756e 5f6e  s,.        run_n
+000010d0: 616d 653d 2270 7265 6665 6374 2d6a 6f62  ame="prefect-job
+000010e0: 222c 0a20 2020 2020 2020 2074 6173 6b73  ",.        tasks
+000010f0: 3d5b 6a6f 625f 7461 736b 5f73 6574 7469  =[job_task_setti
+00001100: 6e67 735d 0a20 2020 2029 0a0a 2020 2020  ngs].    )..    
+00001110: 7265 7475 726e 2072 756e 0a0a 0a6a 6f62  return run...job
+00001120: 735f 7275 6e73 5f73 7562 6d69 745f 666c  s_runs_submit_fl
+00001130: 6f77 280a 2020 2020 626c 6f63 6b5f 6e61  ow(.    block_na
+00001140: 6d65 3d22 424c 4f43 4b2d 4e41 4d45 2d50  me="BLOCK-NAME-P
+00001150: 4c41 4345 484f 4c44 4552 220a 2020 2020  LACEHOLDER".    
+00001160: 6e6f 7465 626f 6f6b 5f70 6174 683d 222f  notebook_path="/
+00001170: 5573 6572 732f 3c45 4d41 494c 5f41 4444  Users/<EMAIL_ADD
+00001180: 5245 5353 5f50 4c41 4345 484f 4c44 4552  RESS_PLACEHOLDER
+00001190: 3e2f 6578 616d 706c 652e 6970 796e 6222  >/example.ipynb"
+000011a0: 2c0a 2020 2020 6e61 6d65 3d22 4d61 7276  ,.    name="Marv
+000011b0: 696e 220a 290a 6060 600a 0a55 706f 6e20  in".).```..Upon 
+000011c0: 6578 6563 7574 696f 6e2c 2074 6865 206e  execution, the n
+000011d0: 6f74 6562 6f6f 6b20 7275 6e20 7368 6f75  otebook run shou
+000011e0: 6c64 206f 7574 7075 743a 0a0a 6060 600a  ld output:..```.
+000011f0: 446f 6e27 7420 776f 7272 7920 4d61 7276  Don't worry Marv
+00001200: 696e 2c20 4920 676f 7420 796f 7572 2072  in, I got your r
+00001210: 6571 7565 7374 2120 5765 6c63 6f6d 6520  equest! Welcome 
+00001220: 746f 2070 7265 6665 6374 2d64 6174 6162  to prefect-datab
+00001230: 7269 636b 7321 0a60 6060 0a0a 2121 2120  ricks!.```..!!! 
+00001240: 696e 666f 2022 496e 7075 7420 6469 6374  info "Input dict
+00001250: 696f 6e61 7269 6573 2069 6e20 7468 6520  ionaries in the 
+00001260: 706c 6163 6520 6f66 206d 6f64 656c 7322  place of models"
+00001270: 0a20 2020 200a 2020 2020 496e 7374 6561  .    .    Instea
+00001280: 6420 6f66 2075 7369 6e67 2074 6865 2062  d of using the b
+00001290: 7569 6c74 2d69 6e20 6d6f 6465 6c73 2c20  uilt-in models, 
+000012a0: 796f 7520 6d61 7920 616c 736f 2069 6e70  you may also inp
+000012b0: 7574 2061 2076 616c 6964 2064 6963 7469  ut a valid dicti
+000012c0: 6f6e 6172 792e 0a20 2020 200a 2020 2020  onary..    .    
+000012d0: 466f 7220 6578 616d 706c 652c 2074 6865  For example, the
+000012e0: 2066 6f6c 6c6f 7769 6e67 2061 7265 2065   following are e
+000012f0: 7175 6976 616c 656e 743a 0a0a 2020 2020  quivalent:..    
+00001300: 6060 6070 7974 686f 6e0a 2020 2020 6175  ```python.    au
+00001310: 746f 5f73 6361 6c65 3d41 7574 6f53 6361  to_scale=AutoSca
+00001320: 6c65 286d 696e 5f77 6f72 6b65 7273 3d31  le(min_workers=1
+00001330: 2c20 6d61 785f 776f 726b 6572 733d 3229  , max_workers=2)
+00001340: 0a20 2020 2060 6060 0a0a 2020 2020 6060  .    ```..    ``
+00001350: 6070 7974 686f 6e0a 2020 2020 6175 746f  `python.    auto
+00001360: 5f73 6361 6c65 3d7b 226d 696e 5f77 6f72  _scale={"min_wor
+00001370: 6b65 7273 223a 2031 2c20 226d 6178 5f77  kers": 1, "max_w
+00001380: 6f72 6b65 7273 223a 2032 7d0a 2020 2020  orkers": 2}.    
+00001390: 6060 600a 0a49 6620 796f 7520 6861 7665  ```..If you have
+000013a0: 2061 6e20 6578 6973 7469 6e67 2044 6174   an existing Dat
+000013b0: 6162 7269 636b 7320 6a6f 622c 2079 6f75  abricks job, you
+000013c0: 2063 616e 2072 756e 2069 7420 7573 696e   can run it usin
+000013d0: 6720 606a 6f62 735f 7275 6e73 5f73 7562  g `jobs_runs_sub
+000013e0: 6d69 745f 6279 5f69 645f 616e 645f 7761  mit_by_id_and_wa
+000013f0: 6974 5f66 6f72 5f63 6f6d 706c 6574 696f  it_for_completio
+00001400: 6e60 3a0a 0a60 6060 7079 7468 6f6e 0a66  n`:..```python.f
+00001410: 726f 6d20 7072 6566 6563 7420 696d 706f  rom prefect impo
+00001420: 7274 2066 6c6f 770a 0a66 726f 6d20 7072  rt flow..from pr
+00001430: 6566 6563 745f 6461 7461 6272 6963 6b73  efect_databricks
+00001440: 2069 6d70 6f72 7420 4461 7461 6272 6963   import Databric
+00001450: 6b73 4372 6564 656e 7469 616c 730a 6672  ksCredentials.fr
+00001460: 6f6d 2070 7265 6665 6374 5f64 6174 6162  om prefect_datab
+00001470: 7269 636b 732e 666c 6f77 7320 696d 706f  ricks.flows impo
+00001480: 7274 2028 0a20 2020 206a 6f62 735f 7275  rt (.    jobs_ru
+00001490: 6e73 5f73 7562 6d69 745f 6279 5f69 645f  ns_submit_by_id_
+000014a0: 616e 645f 7761 6974 5f66 6f72 5f63 6f6d  and_wait_for_com
+000014b0: 706c 6574 696f 6e2c 0a29 0a0a 0a40 666c  pletion,.)...@fl
+000014c0: 6f77 0a64 6566 2065 7869 7374 696e 675f  ow.def existing_
+000014d0: 6a6f 625f 7375 626d 6974 2864 6174 6162  job_submit(datab
+000014e0: 7269 636b 735f 6372 6564 656e 7469 616c  ricks_credential
+000014f0: 735f 626c 6f63 6b5f 6e61 6d65 3a20 7374  s_block_name: st
+00001500: 722c 206a 6f62 5f69 6429 3a0a 2020 2020  r, job_id):.    
+00001510: 6461 7461 6272 6963 6b73 5f63 7265 6465  databricks_crede
+00001520: 6e74 6961 6c73 203d 2044 6174 6162 7269  ntials = Databri
+00001530: 636b 7343 7265 6465 6e74 6961 6c73 2e6c  cksCredentials.l
+00001540: 6f61 6428 6e61 6d65 3d62 6c6f 636b 5f6e  oad(name=block_n
+00001550: 616d 6529 0a0a 2020 2020 7275 6e20 3d20  ame)..    run = 
+00001560: 6a6f 6273 5f72 756e 735f 7375 626d 6974  jobs_runs_submit
+00001570: 5f62 795f 6964 5f61 6e64 5f77 6169 745f  _by_id_and_wait_
+00001580: 666f 725f 636f 6d70 6c65 7469 6f6e 280a  for_completion(.
+00001590: 2020 2020 2020 2020 6461 7461 6272 6963          databric
+000015a0: 6b73 5f63 7265 6465 6e74 6961 6c73 3d64  ks_credentials=d
+000015b0: 6174 6162 7269 636b 735f 6372 6564 656e  atabricks_creden
+000015c0: 7469 616c 732c 206a 6f62 5f69 643d 6a6f  tials, job_id=jo
+000015d0: 625f 6964 0a20 2020 2029 0a0a 2020 2020  b_id.    )..    
+000015e0: 7265 7475 726e 2072 756e 0a0a 6578 6973  return run..exis
+000015f0: 7469 6e67 5f6a 6f62 5f73 7562 6d69 7428  ting_job_submit(
+00001600: 6461 7461 6272 6963 6b73 5f63 7265 6465  databricks_crede
+00001610: 6e74 6961 6c73 5f62 6c6f 636b 5f6e 616d  ntials_block_nam
+00001620: 653d 2264 622d 6372 6564 7322 2c20 6a6f  e="db-creds", jo
+00001630: 625f 6964 3d22 594f 5552 2d4a 4f42 2d4e  b_id="YOUR-JOB-N
+00001640: 414d 4522 290a 6060 600a 0a23 2320 5265  AME").```..## Re
+00001650: 736f 7572 6365 730a 0a46 6f72 206d 6f72  sources..For mor
+00001660: 6520 7469 7073 206f 6e20 686f 7720 746f  e tips on how to
+00001670: 2075 7365 2074 6173 6b73 2061 6e64 2066   use tasks and f
+00001680: 6c6f 7773 2069 6e20 6120 436f 6c6c 6563  lows in a Collec
+00001690: 7469 6f6e 2c20 6368 6563 6b20 6f75 7420  tion, check out 
+000016a0: 5b55 7369 6e67 2043 6f6c 6c65 6374 696f  [Using Collectio
+000016b0: 6e73 5d28 6874 7470 733a 2f2f 6f72 696f  ns](https://orio
+000016c0: 6e2d 646f 6373 2e70 7265 6665 6374 2e69  n-docs.prefect.i
+000016d0: 6f2f 636f 6c6c 6563 7469 6f6e 732f 7573  o/collections/us
+000016e0: 6167 652f 2921 0a0a 4e6f 7465 2c20 7468  age/)!..Note, th
+000016f0: 6520 7461 736b 7320 7769 7468 696e 2074  e tasks within t
+00001700: 6869 7320 636f 6c6c 6563 7469 6f6e 2077  his collection w
+00001710: 6572 6520 6372 6561 7465 6420 6279 2061  ere created by a
+00001720: 2063 6f64 6520 6765 6e65 7261 746f 7220   code generator 
+00001730: 7573 696e 6720 7468 6520 7365 7276 6963  using the servic
+00001740: 6527 7320 4f70 656e 4150 4920 7370 6563  e's OpenAPI spec
+00001750: 2e0a 0a54 6865 2073 6572 7669 6365 2773  ...The service's
+00001760: 2052 4553 5420 4150 4920 646f 6375 6d65   REST API docume
+00001770: 6e74 6174 696f 6e20 6361 6e20 6265 2066  ntation can be f
+00001780: 6f75 6e64 205b 6865 7265 5d28 6874 7470  ound [here](http
+00001790: 733a 2f2f 646f 6373 2e64 6174 6162 7269  s://docs.databri
+000017a0: 636b 732e 636f 6d2f 6465 762d 746f 6f6c  cks.com/dev-tool
+000017b0: 732f 6170 692f 6c61 7465 7374 2f69 6e64  s/api/latest/ind
+000017c0: 6578 2e68 746d 6c29 2e0a 0a23 2323 2049  ex.html)...### I
+000017d0: 6e73 7461 6c6c 6174 696f 6e0a 0a49 6e73  nstallation..Ins
+000017e0: 7461 6c6c 2060 7072 6566 6563 742d 6461  tall `prefect-da
+000017f0: 7461 6272 6963 6b73 6020 7769 7468 2060  tabricks` with `
+00001800: 7069 7060 3a0a 0a60 6060 6261 7368 0a70  pip`:..```bash.p
+00001810: 6970 2069 6e73 7461 6c6c 2070 7265 6665  ip install prefe
+00001820: 6374 2d64 6174 6162 7269 636b 730a 6060  ct-databricks.``
+00001830: 600a 0a52 6571 7569 7265 7320 616e 2069  `..Requires an i
+00001840: 6e73 7461 6c6c 6174 696f 6e20 6f66 2050  nstallation of P
+00001850: 7974 686f 6e20 332e 372b 2e0a 0a57 6520  ython 3.7+...We 
+00001860: 7265 636f 6d6d 656e 6420 7573 696e 6720  recommend using 
+00001870: 6120 5079 7468 6f6e 2076 6972 7475 616c  a Python virtual
+00001880: 2065 6e76 6972 6f6e 6d65 6e74 206d 616e   environment man
+00001890: 6167 6572 2073 7563 6820 6173 2070 6970  ager such as pip
+000018a0: 656e 762c 2063 6f6e 6461 206f 7220 7669  env, conda or vi
+000018b0: 7274 7561 6c65 6e76 2e0a 0a54 6865 7365  rtualenv...These
+000018c0: 2074 6173 6b73 2061 7265 2064 6573 6967   tasks are desig
+000018d0: 6e65 6420 746f 2077 6f72 6b20 7769 7468  ned to work with
+000018e0: 2050 7265 6665 6374 2032 2e20 466f 7220   Prefect 2. For 
+000018f0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00001900: 2061 626f 7574 2068 6f77 2074 6f20 7573   about how to us
+00001910: 6520 5072 6566 6563 742c 2070 6c65 6173  e Prefect, pleas
+00001920: 6520 7265 6665 7220 746f 2074 6865 205b  e refer to the [
+00001930: 5072 6566 6563 7420 646f 6375 6d65 6e74  Prefect document
+00001940: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6f  ation](https://o
+00001950: 7269 6f6e 2d64 6f63 732e 7072 6566 6563  rion-docs.prefec
+00001960: 742e 696f 2f29 2e0a 0a23 2323 2053 6176  t.io/)...### Sav
+00001970: 696e 6720 4372 6564 656e 7469 616c 7320  ing Credentials 
+00001980: 746f 2042 6c6f 636b 0a0a 546f 2075 7365  to Block..To use
+00001990: 2074 6865 2060 6c6f 6164 6020 6d65 7468   the `load` meth
+000019a0: 6f64 206f 6e20 426c 6f63 6b73 2c20 796f  od on Blocks, yo
+000019b0: 7520 6d75 7374 2061 6c72 6561 6479 2068  u must already h
+000019c0: 6176 6520 6120 626c 6f63 6b20 646f 6375  ave a block docu
+000019d0: 6d65 6e74 205b 7361 7665 6420 7468 726f  ment [saved thro
+000019e0: 7567 6820 636f 6465 5d28 6874 7470 733a  ugh code](https:
+000019f0: 2f2f 6f72 696f 6e2d 646f 6373 2e70 7265  //orion-docs.pre
+00001a00: 6665 6374 2e69 6f2f 636f 6e63 6570 7473  fect.io/concepts
+00001a10: 2f62 6c6f 636b 732f 2373 6176 696e 672d  /blocks/#saving-
+00001a20: 626c 6f63 6b73 2920 6f72 205b 7361 7665  blocks) or [save
+00001a30: 6420 7468 726f 7567 6820 7468 6520 5549  d through the UI
+00001a40: 5d28 6874 7470 733a 2f2f 6f72 696f 6e2d  ](https://orion-
+00001a50: 646f 6373 2e70 7265 6665 6374 2e69 6f2f  docs.prefect.io/
+00001a60: 7569 2f62 6c6f 636b 732f 292e 0a0a 4265  ui/blocks/)...Be
+00001a70: 6c6f 7720 6973 2061 2077 616c 6b74 6872  low is a walkthr
+00001a80: 6f75 6768 206f 6e20 7361 7669 6e67 2062  ough on saving b
+00001a90: 6c6f 636b 2064 6f63 756d 656e 7473 2074  lock documents t
+00001aa0: 6872 6f75 6768 2063 6f64 653b 2073 696d  hrough code; sim
+00001ab0: 706c 7920 6372 6561 7465 2061 2073 686f  ply create a sho
+00001ac0: 7274 2073 6372 6970 742c 2072 6570 6c61  rt script, repla
+00001ad0: 6369 6e67 2074 6865 2070 6c61 6365 686f  cing the placeho
+00001ae0: 6c64 6572 732e 200a 0a31 2e20 4865 6164  lders. ..1. Head
+00001af0: 206f 7665 7220 746f 205b 4461 7461 6272   over to [Databr
+00001b00: 6963 6b73 5d28 6874 7470 733a 2f2f 6163  icks](https://ac
+00001b10: 636f 756e 7473 2e63 6c6f 7564 2e64 6174  counts.cloud.dat
+00001b20: 6162 7269 636b 732e 636f 6d2f 292e 0a32  abricks.com/)..2
+00001b30: 2e20 4c6f 6769 6e20 746f 2079 6f75 7220  . Login to your 
+00001b40: 4461 7461 6272 6963 6b73 2061 6363 6f75  Databricks accou
+00001b50: 6e74 2061 6e64 2073 656c 6563 7420 6120  nt and select a 
+00001b60: 776f 726b 7370 6163 652e 0a33 2e20 4f6e  workspace..3. On
+00001b70: 2074 6865 2074 6f70 2072 6967 6874 2073   the top right s
+00001b80: 6964 6520 6f66 2074 6865 206e 6176 2062  ide of the nav b
+00001b90: 6172 2c20 636c 6963 6b20 6f6e 2079 6f75  ar, click on you
+00001ba0: 7220 6163 636f 756e 7420 6e61 6d65 202d  r account name -
+00001bb0: 3e20 5573 6572 2053 6574 7469 6e67 732e  > User Settings.
+00001bc0: 0a34 2e20 436c 6963 6b20 4163 6365 7373  .4. Click Access
+00001bd0: 2074 6f6b 656e 7320 2d3e 2047 656e 6572   tokens -> Gener
+00001be0: 6174 6520 6e65 7720 746f 6b65 6e20 2d3e  ate new token ->
+00001bf0: 2047 656e 6572 6174 6520 616e 6420 636f   Generate and co
+00001c00: 7079 2074 6865 2074 6f6b 656e 2e0a 352e  py the token..5.
+00001c10: 204e 6f74 6520 646f 776e 2079 6f75 7220   Note down your 
+00001c20: 4461 7461 6272 6963 6b73 2069 6e73 7461  Databricks insta
+00001c30: 6e63 6520 6672 6f6d 2074 6865 2062 726f  nce from the bro
+00001c40: 7773 6572 2055 524c 2c20 666f 726d 6174  wser URL, format
+00001c50: 7465 6420 6c69 6b65 2060 6874 7470 733a  ted like `https:
+00001c60: 2f2f 3c44 4154 4142 5249 434b 532d 494e  //<DATABRICKS-IN
+00001c70: 5354 414e 4345 3e2e 636c 6f75 642e 6461  STANCE>.cloud.da
+00001c80: 7461 6272 6963 6b73 2e63 6f6d 2f60 0a36  tabricks.com/`.6
+00001c90: 2e20 4372 6561 7465 2061 2073 686f 7274  . Create a short
+00001ca0: 2073 6372 6970 742c 2072 6570 6c61 6369   script, replaci
+00001cb0: 6e67 2074 6865 2070 6c61 6365 686f 6c64  ng the placehold
+00001cc0: 6572 732e 0a0a 6060 6070 7974 686f 6e0a  ers...```python.
+00001cd0: 6672 6f6d 2070 7265 6665 6374 5f64 6174  from prefect_dat
+00001ce0: 6162 7269 636b 7320 696d 706f 7274 2044  abricks import D
+00001cf0: 6174 6162 7269 636b 7343 7265 6465 6e74  atabricksCredent
+00001d00: 6961 6c73 0a0a 6372 6564 656e 7469 616c  ials..credential
+00001d10: 7320 3d20 4461 7461 6272 6963 6b73 4372  s = DatabricksCr
+00001d20: 6564 656e 7469 616c 7328 0a20 2020 2064  edentials(.    d
+00001d30: 6174 6162 7269 636b 735f 696e 7374 616e  atabricks_instan
+00001d40: 6365 3d22 4441 5441 4252 4943 4b53 2d49  ce="DATABRICKS-I
+00001d50: 4e53 5441 4e43 452d 504c 4143 4548 4f4c  NSTANCE-PLACEHOL
+00001d60: 4445 5222 0a20 2020 2074 6f6b 656e 3d22  DER".    token="
+00001d70: 544f 4b45 4e2d 504c 4143 4548 4f4c 4445  TOKEN-PLACEHOLDE
+00001d80: 5222 0a29 0a0a 636f 6e6e 6563 746f 722e  R".)..connector.
+00001d90: 7361 7665 2822 424c 4f43 4b5f 4e41 4d45  save("BLOCK_NAME
+00001da0: 2d50 4c41 4345 484f 4c44 4552 2229 0a60  -PLACEHOLDER").`
+00001db0: 6060 0a0a 436f 6e67 7261 7473 2120 596f  ``..Congrats! Yo
+00001dc0: 7520 6361 6e20 6e6f 7720 6561 7369 6c79  u can now easily
+00001dd0: 206c 6f61 6420 7468 6520 7361 7665 6420   load the saved 
+00001de0: 626c 6f63 6b2c 2077 6869 6368 2068 6f6c  block, which hol
+00001df0: 6473 2079 6f75 7220 6372 6564 656e 7469  ds your credenti
+00001e00: 616c 733a 0a0a 6060 6070 7974 686f 6e0a  als:..```python.
+00001e10: 6672 6f6d 2070 7265 6665 6374 5f64 6174  from prefect_dat
+00001e20: 6162 7269 636b 7320 696d 706f 7274 2044  abricks import D
+00001e30: 6174 6162 7269 636b 7343 7265 6465 6e74  atabricksCredent
+00001e40: 6961 6c73 0a0a 4461 7461 6272 6963 6b73  ials..Databricks
+00001e50: 4372 6564 656e 7469 616c 732e 6c6f 6164  Credentials.load
+00001e60: 2822 424c 4f43 4b5f 4e41 4d45 2d50 4c41  ("BLOCK_NAME-PLA
+00001e70: 4345 484f 4c44 4552 2229 0a60 6060 0a0a  CEHOLDER").```..
+00001e80: 2121 2120 696e 666f 2022 5265 6769 7374  !!! info "Regist
+00001e90: 6572 696e 6720 626c 6f63 6b73 220a 0a20  ering blocks".. 
+00001ea0: 2020 2052 6567 6973 7465 7220 626c 6f63     Register bloc
+00001eb0: 6b73 2069 6e20 7468 6973 206d 6f64 756c  ks in this modul
+00001ec0: 6520 746f 0a20 2020 205b 7669 6577 2061  e to.    [view a
+00001ed0: 6e64 2065 6469 7420 7468 656d 5d28 6874  nd edit them](ht
+00001ee0: 7470 733a 2f2f 6f72 696f 6e2d 646f 6373  tps://orion-docs
+00001ef0: 2e70 7265 6665 6374 2e69 6f2f 7569 2f62  .prefect.io/ui/b
+00001f00: 6c6f 636b 732f 290a 2020 2020 6f6e 2050  locks/).    on P
+00001f10: 7265 6665 6374 2043 6c6f 7564 3a0a 0a20  refect Cloud:.. 
+00001f20: 2020 2060 6060 6261 7368 0a20 2020 2070     ```bash.    p
+00001f30: 7265 6665 6374 2062 6c6f 636b 2072 6567  refect block reg
+00001f40: 6973 7465 7220 2d6d 2070 7265 6665 6374  ister -m prefect
+00001f50: 5f64 6174 6162 7269 636b 730a 2020 2020  _databricks.    
+00001f60: 6060 600a 0a23 2323 2046 6565 6462 6163  ```..### Feedbac
+00001f70: 6b0a 0a49 6620 796f 7520 656e 636f 756e  k..If you encoun
+00001f80: 7465 7220 616e 7920 6275 6773 2077 6869  ter any bugs whi
+00001f90: 6c65 2075 7369 6e67 2060 7072 6566 6563  le using `prefec
+00001fa0: 742d 6461 7461 6272 6963 6b73 602c 2066  t-databricks`, f
+00001fb0: 6565 6c20 6672 6565 2074 6f20 6f70 656e  eel free to open
+00001fc0: 2061 6e20 6973 7375 6520 696e 2074 6865   an issue in the
+00001fd0: 205b 7072 6566 6563 742d 6461 7461 6272   [prefect-databr
+00001fe0: 6963 6b73 5d28 6874 7470 733a 2f2f 6769  icks](https://gi
+00001ff0: 7468 7562 2e63 6f6d 2f50 7265 6665 6374  thub.com/Prefect
+00002000: 4851 2f70 7265 6665 6374 2d64 6174 6162  HQ/prefect-datab
+00002010: 7269 636b 7329 2072 6570 6f73 6974 6f72  ricks) repositor
+00002020: 792e 0a0a 4966 2079 6f75 2068 6176 6520  y...If you have 
+00002030: 616e 7920 7175 6573 7469 6f6e 7320 6f72  any questions or
+00002040: 2069 7373 7565 7320 7768 696c 6520 7573   issues while us
+00002050: 696e 6720 6070 7265 6665 6374 2d64 6174  ing `prefect-dat
+00002060: 6162 7269 636b 7360 2c20 796f 7520 6361  abricks`, you ca
+00002070: 6e20 6669 6e64 2068 656c 7020 696e 2065  n find help in e
+00002080: 6974 6865 7220 7468 6520 5b50 7265 6665  ither the [Prefe
+00002090: 6374 2044 6973 636f 7572 7365 2066 6f72  ct Discourse for
+000020a0: 756d 5d28 6874 7470 733a 2f2f 6469 7363  um](https://disc
+000020b0: 6f75 7273 652e 7072 6566 6563 742e 696f  ourse.prefect.io
+000020c0: 2f29 206f 7220 7468 6520 5b50 7265 6665  /) or the [Prefe
+000020d0: 6374 2053 6c61 636b 2063 6f6d 6d75 6e69  ct Slack communi
+000020e0: 7479 5d28 6874 7470 733a 2f2f 7072 6566  ty](https://pref
+000020f0: 6563 742e 696f 2f73 6c61 636b 292e 0a0a  ect.io/slack)...
+00002100: 4665 656c 2066 7265 6520 746f 2073 7461  Feel free to sta
+00002110: 7220 6f72 2077 6174 6368 205b 6070 7265  r or watch [`pre
+00002120: 6665 6374 2d64 6174 6162 7269 636b 7360  fect-databricks`
+00002130: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002140: 2e63 6f6d 2f50 7265 6665 6374 4851 2f70  .com/PrefectHQ/p
+00002150: 7265 6665 6374 2d64 6174 6162 7269 636b  refect-databrick
+00002160: 7329 2066 6f72 2075 7064 6174 6573 2074  s) for updates t
+00002170: 6f6f 210a 0a23 2323 2043 6f6e 7472 6962  oo!..### Contrib
+00002180: 7574 696e 670a 0a49 6620 796f 7527 6420  uting..If you'd 
+00002190: 6c69 6b65 2074 6f20 6865 6c70 2063 6f6e  like to help con
+000021a0: 7472 6962 7574 6520 746f 2066 6978 2061  tribute to fix a
+000021b0: 6e20 6973 7375 6520 6f72 2061 6464 2061  n issue or add a
+000021c0: 2066 6561 7475 7265 2074 6f20 6070 7265   feature to `pre
+000021d0: 6665 6374 2d64 6174 6162 7269 636b 7360  fect-databricks`
+000021e0: 2c20 706c 6561 7365 205b 7072 6f70 6f73  , please [propos
+000021f0: 6520 6368 616e 6765 7320 7468 726f 7567  e changes throug
+00002200: 6820 6120 7075 6c6c 2072 6571 7565 7374  h a pull request
+00002210: 2066 726f 6d20 6120 666f 726b 206f 6620   from a fork of 
+00002220: 7468 6520 7265 706f 7369 746f 7279 5d28  the repository](
+00002230: 6874 7470 733a 2f2f 646f 6373 2e67 6974  https://docs.git
+00002240: 6875 622e 636f 6d2f 656e 2f70 756c 6c2d  hub.com/en/pull-
+00002250: 7265 7175 6573 7473 2f63 6f6c 6c61 626f  requests/collabo
+00002260: 7261 7469 6e67 2d77 6974 682d 7075 6c6c  rating-with-pull
+00002270: 2d72 6571 7565 7374 732f 7072 6f70 6f73  -requests/propos
+00002280: 696e 672d 6368 616e 6765 732d 746f 2d79  ing-changes-to-y
+00002290: 6f75 722d 776f 726b 2d77 6974 682d 7075  our-work-with-pu
+000022a0: 6c6c 2d72 6571 7565 7374 732f 6372 6561  ll-requests/crea
+000022b0: 7469 6e67 2d61 2d70 756c 6c2d 7265 7175  ting-a-pull-requ
+000022c0: 6573 742d 6672 6f6d 2d61 2d66 6f72 6b29  est-from-a-fork)
+000022d0: 2e0a 0a48 6572 6520 6172 6520 7468 6520  ...Here are the 
+000022e0: 7374 6570 733a 0a0a 312e 205b 466f 726b  steps:..1. [Fork
+000022f0: 2074 6865 2072 6570 6f73 6974 6f72 795d   the repository]
+00002300: 2868 7474 7073 3a2f 2f64 6f63 732e 6769  (https://docs.gi
+00002310: 7468 7562 2e63 6f6d 2f65 6e2f 6765 742d  thub.com/en/get-
+00002320: 7374 6172 7465 642f 7175 6963 6b73 7461  started/quicksta
+00002330: 7274 2f66 6f72 6b2d 612d 7265 706f 2366  rt/fork-a-repo#f
+00002340: 6f72 6b69 6e67 2d61 2d72 6570 6f73 6974  orking-a-reposit
+00002350: 6f72 7929 0a32 2e20 5b43 6c6f 6e65 2074  ory).2. [Clone t
+00002360: 6865 2066 6f72 6b65 6420 7265 706f 7369  he forked reposi
+00002370: 746f 7279 5d28 6874 7470 733a 2f2f 646f  tory](https://do
+00002380: 6373 2e67 6974 6875 622e 636f 6d2f 656e  cs.github.com/en
+00002390: 2f67 6574 2d73 7461 7274 6564 2f71 7569  /get-started/qui
+000023a0: 636b 7374 6172 742f 666f 726b 2d61 2d72  ckstart/fork-a-r
+000023b0: 6570 6f23 636c 6f6e 696e 672d 796f 7572  epo#cloning-your
+000023c0: 2d66 6f72 6b65 642d 7265 706f 7369 746f  -forked-reposito
+000023d0: 7279 290a 332e 2049 6e73 7461 6c6c 2074  ry).3. Install t
+000023e0: 6865 2072 6570 6f73 6974 6f72 7920 616e  he repository an
+000023f0: 6420 6974 7320 6465 7065 6e64 656e 6369  d its dependenci
+00002400: 6573 3a0a 6060 600a 7069 7020 696e 7374  es:.```.pip inst
+00002410: 616c 6c20 2d65 2022 2e5b 6465 765d 220a  all -e ".[dev]".
+00002420: 6060 600a 342e 204d 616b 6520 6465 7369  ```.4. Make desi
+00002430: 7265 6420 6368 616e 6765 730a 352e 2041  red changes.5. A
+00002440: 6464 2074 6573 7473 0a36 2e20 496e 7365  dd tests.6. Inse
+00002450: 7274 2061 6e20 656e 7472 7920 746f 205b  rt an entry to [
+00002460: 4348 414e 4745 4c4f 472e 6d64 5d28 6874  CHANGELOG.md](ht
+00002470: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002480: 2f50 7265 6665 6374 4851 2f70 7265 6665  /PrefectHQ/prefe
+00002490: 6374 2d64 6174 6162 7269 636b 732f 626c  ct-databricks/bl
+000024a0: 6f62 2f6d 6169 6e2f 4348 414e 4745 4c4f  ob/main/CHANGELO
+000024b0: 472e 6d64 290a 372e 2049 6e73 7461 6c6c  G.md).7. Install
+000024c0: 2060 7072 652d 636f 6d6d 6974 6020 746f   `pre-commit` to
+000024d0: 2070 6572 666f 726d 2071 7561 6c69 7479   perform quality
+000024e0: 2063 6865 636b 7320 7072 696f 7220 746f   checks prior to
+000024f0: 2063 6f6d 6d69 743a 0a60 6060 0a70 7265   commit:.```.pre
+00002500: 2d63 6f6d 6d69 7420 696e 7374 616c 6c0a  -commit install.
+00002510: 6060 600a 382e 2060 6769 7420 636f 6d6d  ```.8. `git comm
+00002520: 6974 602c 2060 6769 7420 7075 7368 602c  it`, `git push`,
+00002530: 2061 6e64 2063 7265 6174 6520 6120 7075   and create a pu
+00002540: 6c6c 2072 6571 7565 7374 0a              ll request.
```

### Comparing `prefect-databricks-0.1.4/prefect_databricks/credentials.py` & `prefect-databricks-0.1.5/prefect_databricks/credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         from prefect_databricks import DatabricksCredentials
         databricks_credentials_block = DatabricksCredentials.load("BLOCK_NAME")
         ```
     """
 
     _block_type_name = "Databricks Credentials"
     _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/5GTHI1PH2dTiantfps6Fnc/1c750fab7f4c14ea1b93a62b9fea6a94/databricks_logo_icon_170295.png?h=250"  # noqa
+    _documentation_url = "https://prefecthq.github.io/prefect-databricks/credentials/#prefect_databricks.credentials.DatabricksCredentials"  # noqa
 
     databricks_instance: str = Field(
         default=...,
         description="Databricks instance used in formatting the endpoint URL.",
     )
     token: SecretStr = Field(
         default=..., description="The token to authenticate with Databricks."
```

### Comparing `prefect-databricks-0.1.4/prefect_databricks/jobs.py` & `prefect-databricks-0.1.5/prefect_databricks/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,15 +780,15 @@
     contents = _unpack_contents(response, responses)
     return contents
 
 
 @task
 async def jobs_run_now(
     databricks_credentials: "DatabricksCredentials",
-    job_id: Optional[int] = None,
+    job_id: int,
     idempotency_token: Optional[str] = None,
     jar_params: Optional[List[str]] = None,
     notebook_params: Optional[Dict] = None,
     python_params: Optional[List[str]] = None,
     spark_submit_params: Optional[List[str]] = None,
     python_named_params: Optional[Dict] = None,
     pipeline_params: Optional[str] = None,
@@ -890,14 +890,19 @@
             A map from keys to values for jobs with Python wheel task, for example
             `'python_named_params': {'name': 'task', 'data':
             'dbfs:/path/to/data.json'}`, e.g.
             ```
             {"name": "task", "data": "dbfs:/path/to/data.json"}
             ```
         pipeline_params:
+            If `full_refresh` is set to true, trigger a full refresh on the
+            delta live table e.g.
+            ```
+                "pipeline_params": {"full_refresh": true}
+            ```
 
         sql_params:
             A map from keys to values for SQL tasks, for example `'sql_params':
             {'name': 'john doe', 'age': '35'}`. The SQL alert task does
             not support custom parameters, e.g.
             ```
             {"name": "john doe", "age": "35"}
```

### Comparing `prefect-databricks-0.1.4/prefect_databricks/models/jobs.py` & `prefect-databricks-0.1.5/prefect_databricks/models/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,14 +802,23 @@
     * `ASC`: Ascending order.
     """
 
     desc = "DESC"
     asc = "ASC"
 
 
+class RuntimeEngine(str, Enum):
+    """
+    Decides which runtime engine to be use, e.g. Standard vs. Photon. If unspecified, the runtime engine is inferred from spark_version.
+    """
+
+    standard = "STANDARD"
+    photon = "PHOTON"
+
+
 class LogSyncStatus(BaseModel):
     """
     See source code for the fields' description.
     """
 
     class Config:
         extra = Extra.allow
@@ -2452,14 +2461,23 @@
         description=(
             "The Spark version of the cluster. A list of available Spark versions can"
             " be retrieved by using the [Runtime"
             " versions](https://docs.databricks.com/dev-tools/api/latest/clusters.html#runtime-versions)"
             " API call."
         ),
     )
+    runtime_engine: Optional[RuntimeEngine] = Field(
+        None,
+        description=(
+            "Decides which runtime engine to be use, e.g. Standard vs. Photon. If "
+            "unspecified, the runtime engine is inferred from spark_version. "
+            "see https://docs.databricks.com/api-explorer/workspace/jobs/create "
+            " for more details"
+        ),
+    )
     ssh_public_keys: Optional[List[str]] = Field(
         None,
         description=(
             "SSH public key contents that are added to each Spark node in this cluster."
             " The corresponding private keys can be used to login with the user name"
             " `ubuntu` on port `2200`. Up to 10 keys can be specified."
         ),
```

### Comparing `prefect-databricks-0.1.4/prefect_databricks/rest.py` & `prefect-databricks-0.1.5/prefect_databricks/rest.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.4/prefect_databricks.egg-info/PKG-INFO` & `prefect-databricks-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7072 6566  : 2.1.Name: pref
 00000020: 6563 742d 6461 7461 6272 6963 6b73 0a56  ect-databricks.V
-00000030: 6572 7369 6f6e 3a20 302e 312e 340a 5375  ersion: 0.1.4.Su
+00000030: 6572 7369 6f6e 3a20 302e 312e 350a 5375  ersion: 0.1.5.Su
 00000040: 6d6d 6172 793a 2050 7265 6665 6374 2069  mmary: Prefect i
 00000050: 6e74 6567 7261 7469 6f6e 7320 696e 7465  ntegrations inte
 00000060: 7261 6374 696e 6720 7769 7468 2044 6174  racting with Dat
 00000070: 6162 7269 636b 730a 486f 6d65 2d70 6167  abricks.Home-pag
 00000080: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000090: 622e 636f 6d2f 5072 6566 6563 7448 512f  b.com/PrefectHQ/
 000000a0: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
@@ -51,425 +51,604 @@
 00000320: 6965 730a 5265 7175 6972 6573 2d50 7974  ies.Requires-Pyt
 00000330: 686f 6e3a 203e 3d33 2e37 0a44 6573 6372  hon: >=3.7.Descr
 00000340: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
 00000350: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
 00000360: 776e 0a50 726f 7669 6465 732d 4578 7472  wn.Provides-Extr
 00000370: 613a 2064 6576 0a4c 6963 656e 7365 2d46  a: dev.License-F
 00000380: 696c 653a 204c 4943 454e 5345 0a0a 2320  ile: LICENSE..# 
-00000390: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-000003a0: 6b73 0a0a 5669 7369 7420 7468 6520 6675  ks..Visit the fu
-000003b0: 6c6c 2064 6f63 7320 5b68 6572 655d 2868  ll docs [here](h
-000003c0: 7474 7073 3a2f 2f50 7265 6665 6374 4851  ttps://PrefectHQ
-000003d0: 2e67 6974 6875 622e 696f 2f70 7265 6665  .github.io/prefe
-000003e0: 6374 2d64 6174 6162 7269 636b 7329 2074  ct-databricks) t
-000003f0: 6f20 7365 6520 6164 6469 7469 6f6e 616c  o see additional
-00000400: 2065 7861 6d70 6c65 7320 616e 6420 7468   examples and th
-00000410: 6520 4150 4920 7265 6665 7265 6e63 652e  e API reference.
-00000420: 0a20 0a3c 7020 616c 6967 6e3d 2263 656e  . .<p align="cen
-00000430: 7465 7222 3e0a 2020 2020 3c61 2068 7265  ter">.    <a hre
-00000440: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
-00000450: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
-00000460: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
-00000470: 6b73 2f22 2061 6c74 3d22 5079 5049 2076  ks/" alt="PyPI v
-00000480: 6572 7369 6f6e 223e 0a20 2020 2020 2020  ersion">.       
-00000490: 203c 696d 6720 616c 743d 2250 7950 4922   <img alt="PyPI"
-000004a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-000004b0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000004c0: 692f 762f 7072 6566 6563 742d 6461 7461  i/v/prefect-data
-000004d0: 6272 6963 6b73 3f63 6f6c 6f72 3d30 3035  bricks?color=005
-000004e0: 3246 4626 6c61 6265 6c43 6f6c 6f72 3d30  2FF&labelColor=0
-000004f0: 3930 3432 3222 3e3c 2f61 3e0a 2020 2020  90422"></a>.    
-00000500: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000510: 2f67 6974 6875 622e 636f 6d2f 5072 6566  /github.com/Pref
-00000520: 6563 7448 512f 7072 6566 6563 742d 6461  ectHQ/prefect-da
-00000530: 7461 6272 6963 6b73 2f22 2061 6c74 3d22  tabricks/" alt="
-00000540: 5374 6172 7322 3e0a 2020 2020 2020 2020  Stars">.        
-00000550: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000560: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000570: 2f67 6974 6875 622f 7374 6172 732f 5072  /github/stars/Pr
-00000580: 6566 6563 7448 512f 7072 6566 6563 742d  efectHQ/prefect-
-00000590: 6461 7461 6272 6963 6b73 3f63 6f6c 6f72  databricks?color
-000005a0: 3d30 3035 3246 4626 6c61 6265 6c43 6f6c  =0052FF&labelCol
-000005b0: 6f72 3d30 3930 3432 3222 202f 3e3c 2f61  or=090422" /></a
-000005c0: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-000005d0: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-000005e0: 2f62 6164 6765 2f70 7265 6665 6374 2d64  /badge/prefect-d
-000005f0: 6174 6162 7269 636b 732f 2220 616c 743d  atabricks/" alt=
-00000600: 2244 6f77 6e6c 6f61 6473 223e 0a20 2020  "Downloads">.   
-00000610: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
-00000620: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000630: 6473 2e69 6f2f 7079 7069 2f64 6d2f 7072  ds.io/pypi/dm/pr
-00000640: 6566 6563 742d 6461 7461 6272 6963 6b73  efect-databricks
-00000650: 3f63 6f6c 6f72 3d30 3035 3246 4626 6c61  ?color=0052FF&la
-00000660: 6265 6c43 6f6c 6f72 3d30 3930 3432 3222  belColor=090422"
-00000670: 202f 3e3c 2f61 3e0a 2020 2020 3c61 2068   /></a>.    <a h
-00000680: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000690: 6875 622e 636f 6d2f 5072 6566 6563 7448  hub.com/PrefectH
-000006a0: 512f 7072 6566 6563 742d 6461 7461 6272  Q/prefect-databr
-000006b0: 6963 6b73 2f70 756c 7365 2220 616c 743d  icks/pulse" alt=
-000006c0: 2241 6374 6976 6974 7922 3e0a 2020 2020  "Activity">.    
-000006d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-000006e0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000006f0: 732e 696f 2f67 6974 6875 622f 636f 6d6d  s.io/github/comm
-00000700: 6974 2d61 6374 6976 6974 792f 6d2f 5072  it-activity/m/Pr
-00000710: 6566 6563 7448 512f 7072 6566 6563 742d  efectHQ/prefect-
-00000720: 6461 7461 6272 6963 6b73 3f63 6f6c 6f72  databricks?color
-00000730: 3d30 3035 3246 4626 6c61 6265 6c43 6f6c  =0052FF&labelCol
-00000740: 6f72 3d30 3930 3432 3222 202f 3e3c 2f61  or=090422" /></a
-00000750: 3e0a 2020 2020 3c62 723e 0a20 2020 203c  >.    <br>.    <
-00000760: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000770: 7072 6566 6563 742d 636f 6d6d 756e 6974  prefect-communit
-00000780: 792e 736c 6163 6b2e 636f 6d22 2061 6c74  y.slack.com" alt
-00000790: 3d22 536c 6163 6b22 3e0a 2020 2020 2020  ="Slack">.      
-000007a0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-000007b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000007c0: 696f 2f62 6164 6765 2f73 6c61 636b 2d6a  io/badge/slack-j
-000007d0: 6f69 6e5f 636f 6d6d 756e 6974 792d 7265  oin_community-re
-000007e0: 642e 7376 673f 636f 6c6f 723d 3030 3532  d.svg?color=0052
-000007f0: 4646 266c 6162 656c 436f 6c6f 723d 3039  FF&labelColor=09
-00000800: 3034 3232 266c 6f67 6f3d 736c 6163 6b22  0422&logo=slack"
-00000810: 202f 3e3c 2f61 3e0a 2020 2020 3c61 2068   /></a>.    <a h
-00000820: 7265 663d 2268 7474 7073 3a2f 2f64 6973  ref="https://dis
-00000830: 636f 7572 7365 2e70 7265 6665 6374 2e69  course.prefect.i
-00000840: 6f2f 2220 616c 743d 2244 6973 636f 7572  o/" alt="Discour
-00000850: 7365 223e 0a20 2020 2020 2020 203c 696d  se">.        <im
-00000860: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000870: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000880: 6467 652f 6469 7363 6f75 7273 652d 6272  dge/discourse-br
-00000890: 6f77 7365 5f66 6f72 756d 2d72 6564 2e73  owse_forum-red.s
-000008a0: 7667 3f63 6f6c 6f72 3d30 3035 3246 4626  vg?color=0052FF&
-000008b0: 6c61 6265 6c43 6f6c 6f72 3d30 3930 3432  labelColor=09042
-000008c0: 3226 6c6f 676f 3d64 6973 636f 7572 7365  2&logo=discourse
-000008d0: 2220 2f3e 3c2f 613e 0a3c 2f70 3e0a 0a23  " /></a>.</p>..#
-000008e0: 2320 5765 6c63 6f6d 6521 0a0a 5072 6566  # Welcome!..Pref
-000008f0: 6563 7420 696e 7465 6772 6174 696f 6e73  ect integrations
-00000900: 2066 6f72 2069 6e74 6572 6163 7469 6e67   for interacting
-00000910: 2077 6974 6820 4461 7461 6272 6963 6b73   with Databricks
-00000920: 0a0a 5468 6520 7461 736b 7320 7769 7468  ..The tasks with
-00000930: 696e 2074 6869 7320 636f 6c6c 6563 7469  in this collecti
-00000940: 6f6e 2077 6572 6520 6372 6561 7465 6420  on were created 
-00000950: 6279 2061 2063 6f64 6520 6765 6e65 7261  by a code genera
-00000960: 746f 7220 7573 696e 6720 7468 6520 7365  tor using the se
-00000970: 7276 6963 6527 7320 4f70 656e 4150 4920  rvice's OpenAPI 
-00000980: 7370 6563 2e0a 0a54 6865 2073 6572 7669  spec...The servi
-00000990: 6365 2773 2052 4553 5420 4150 4920 646f  ce's REST API do
-000009a0: 6375 6d65 6e74 6174 696f 6e20 6361 6e20  cumentation can 
-000009b0: 6265 2066 6f75 6e64 205b 6865 7265 5d28  be found [here](
-000009c0: 6874 7470 733a 2f2f 646f 6373 2e64 6174  https://docs.dat
-000009d0: 6162 7269 636b 732e 636f 6d2f 6465 762d  abricks.com/dev-
-000009e0: 746f 6f6c 732f 6170 692f 6c61 7465 7374  tools/api/latest
-000009f0: 2f69 6e64 6578 2e68 746d 6c29 2e0a 0a23  /index.html)...#
-00000a00: 2320 4765 7474 696e 6720 5374 6172 7465  # Getting Starte
-00000a10: 640a 0a23 2323 2050 7974 686f 6e20 7365  d..### Python se
-00000a20: 7475 700a 0a52 6571 7569 7265 7320 616e  tup..Requires an
-00000a30: 2069 6e73 7461 6c6c 6174 696f 6e20 6f66   installation of
-00000a40: 2050 7974 686f 6e20 332e 372b 2e0a 0a57   Python 3.7+...W
-00000a50: 6520 7265 636f 6d6d 656e 6420 7573 696e  e recommend usin
-00000a60: 6720 6120 5079 7468 6f6e 2076 6972 7475  g a Python virtu
-00000a70: 616c 2065 6e76 6972 6f6e 6d65 6e74 206d  al environment m
-00000a80: 616e 6167 6572 2073 7563 6820 6173 2070  anager such as p
-00000a90: 6970 656e 762c 2063 6f6e 6461 206f 7220  ipenv, conda or 
-00000aa0: 7669 7274 7561 6c65 6e76 2e0a 0a54 6865  virtualenv...The
-00000ab0: 7365 2074 6173 6b73 2061 7265 2064 6573  se tasks are des
-00000ac0: 6967 6e65 6420 746f 2077 6f72 6b20 7769  igned to work wi
-00000ad0: 7468 2050 7265 6665 6374 2032 2e20 466f  th Prefect 2. Fo
-00000ae0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-00000af0: 6f6e 2061 626f 7574 2068 6f77 2074 6f20  on about how to 
-00000b00: 7573 6520 5072 6566 6563 742c 2070 6c65  use Prefect, ple
-00000b10: 6173 6520 7265 6665 7220 746f 2074 6865  ase refer to the
-00000b20: 205b 5072 6566 6563 7420 646f 6375 6d65   [Prefect docume
-00000b30: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-00000b40: 2f6f 7269 6f6e 2d64 6f63 732e 7072 6566  /orion-docs.pref
-00000b50: 6563 742e 696f 2f29 2e0a 0a23 2323 2049  ect.io/)...### I
-00000b60: 6e73 7461 6c6c 6174 696f 6e0a 0a49 6e73  nstallation..Ins
-00000b70: 7461 6c6c 2060 7072 6566 6563 742d 6461  tall `prefect-da
-00000b80: 7461 6272 6963 6b73 6020 7769 7468 2060  tabricks` with `
-00000b90: 7069 7060 3a0a 0a60 6060 6261 7368 0a70  pip`:..```bash.p
-00000ba0: 6970 2069 6e73 7461 6c6c 2070 7265 6665  ip install prefe
-00000bb0: 6374 2d64 6174 6162 7269 636b 730a 6060  ct-databricks.``
-00000bc0: 600a 0a41 206c 6973 7420 6f66 2061 7661  `..A list of ava
-00000bd0: 696c 6162 6c65 2062 6c6f 636b 7320 696e  ilable blocks in
-00000be0: 2060 7072 6566 6563 742d 6461 7461 6272   `prefect-databr
-00000bf0: 6963 6b73 6020 616e 6420 7468 6569 7220  icks` and their 
-00000c00: 7365 7475 7020 696e 7374 7275 6374 696f  setup instructio
-00000c10: 6e73 2063 616e 2062 6520 666f 756e 6420  ns can be found 
-00000c20: 5b68 6572 655d 2868 7474 7073 3a2f 2f50  [here](https://P
-00000c30: 7265 6665 6374 4851 2e67 6974 6875 622e  refectHQ.github.
-00000c40: 696f 2f70 7265 6665 6374 2d64 6174 6162  io/prefect-datab
-00000c50: 7269 636b 732f 2362 6c6f 636b 732d 6361  ricks/#blocks-ca
-00000c60: 7461 6c6f 6729 2e0a 0a23 2323 204c 6973  talog)...### Lis
-00000c70: 7473 206a 6f62 7320 6f6e 2074 6865 2044  ts jobs on the D
-00000c80: 6174 6162 7269 636b 7320 696e 7374 616e  atabricks instan
-00000c90: 6365 0a0a 6060 6070 7974 686f 6e0a 6672  ce..```python.fr
-00000ca0: 6f6d 2070 7265 6665 6374 2069 6d70 6f72  om prefect impor
-00000cb0: 7420 666c 6f77 0a66 726f 6d20 7072 6566  t flow.from pref
-00000cc0: 6563 745f 6461 7461 6272 6963 6b73 2069  ect_databricks i
-00000cd0: 6d70 6f72 7420 4461 7461 6272 6963 6b73  mport Databricks
-00000ce0: 4372 6564 656e 7469 616c 730a 6672 6f6d  Credentials.from
-00000cf0: 2070 7265 6665 6374 5f64 6174 6162 7269   prefect_databri
-00000d00: 636b 732e 6a6f 6273 2069 6d70 6f72 7420  cks.jobs import 
-00000d10: 6a6f 6273 5f6c 6973 740a 0a0a 4066 6c6f  jobs_list...@flo
-00000d20: 770a 6465 6620 6578 616d 706c 655f 6578  w.def example_ex
-00000d30: 6563 7574 655f 656e 6470 6f69 6e74 5f66  ecute_endpoint_f
-00000d40: 6c6f 7728 293a 0a20 2020 2064 6174 6162  low():.    datab
-00000d50: 7269 636b 735f 6372 6564 656e 7469 616c  ricks_credential
-00000d60: 7320 3d20 4461 7461 6272 6963 6b73 4372  s = DatabricksCr
-00000d70: 6564 656e 7469 616c 732e 6c6f 6164 2822  edentials.load("
-00000d80: 6d79 2d62 6c6f 636b 2229 0a20 2020 206a  my-block").    j
-00000d90: 6f62 7320 3d20 6a6f 6273 5f6c 6973 7428  obs = jobs_list(
-00000da0: 0a20 2020 2020 2020 2064 6174 6162 7269  .        databri
-00000db0: 636b 735f 6372 6564 656e 7469 616c 732c  cks_credentials,
-00000dc0: 0a20 2020 2020 2020 206c 696d 6974 3d35  .        limit=5
-00000dd0: 0a20 2020 2029 0a20 2020 2072 6574 7572  .    ).    retur
-00000de0: 6e20 6a6f 6273 0a0a 6578 616d 706c 655f  n jobs..example_
-00000df0: 6578 6563 7574 655f 656e 6470 6f69 6e74  execute_endpoint
-00000e00: 5f66 6c6f 7728 290a 6060 600a 0a23 2323  _flow().```..###
-00000e10: 2055 7365 2060 7769 7468 5f6f 7074 696f   Use `with_optio
-00000e20: 6e73 6020 746f 2063 7573 746f 6d69 7a65  ns` to customize
-00000e30: 206f 7074 696f 6e73 206f 6e20 616e 7920   options on any 
-00000e40: 6578 6973 7469 6e67 2074 6173 6b20 6f72  existing task or
-00000e50: 2066 6c6f 770a 0a60 6060 7079 7468 6f6e   flow..```python
-00000e60: 0a63 7573 746f 6d5f 6578 616d 706c 655f  .custom_example_
-00000e70: 6578 6563 7574 655f 656e 6470 6f69 6e74  execute_endpoint
-00000e80: 5f66 6c6f 7720 3d20 6578 616d 706c 655f  _flow = example_
-00000e90: 6578 6563 7574 655f 656e 6470 6f69 6e74  execute_endpoint
-00000ea0: 5f66 6c6f 772e 7769 7468 5f6f 7074 696f  _flow.with_optio
-00000eb0: 6e73 280a 2020 2020 6e61 6d65 3d22 4d79  ns(.    name="My
-00000ec0: 2063 7573 746f 6d20 666c 6f77 206e 616d   custom flow nam
-00000ed0: 6522 2c0a 2020 2020 7265 7472 6965 733d  e",.    retries=
-00000ee0: 322c 0a20 2020 2072 6574 7279 5f64 656c  2,.    retry_del
-00000ef0: 6179 5f73 6563 6f6e 6473 3d31 302c 0a29  ay_seconds=10,.)
-00000f00: 0a60 6060 0a0a 2323 2320 4c61 756e 6368  .```..### Launch
-00000f10: 2061 206e 6577 2063 6c75 7374 6572 2061   a new cluster a
-00000f20: 6e64 2072 756e 2061 2044 6174 6162 7269  nd run a Databri
-00000f30: 636b 7320 6e6f 7465 626f 6f6b 0a0a 4e6f  cks notebook..No
-00000f40: 7465 626f 6f6b 206e 616d 6564 2060 6578  tebook named `ex
-00000f50: 616d 706c 652e 6970 796e 6260 206f 6e20  ample.ipynb` on 
-00000f60: 4461 7461 6272 6963 6b73 2077 6869 6368  Databricks which
-00000f70: 2061 6363 6570 7473 2061 206e 616d 6520   accepts a name 
-00000f80: 7061 7261 6d65 7465 723a 0a0a 6060 6070  parameter:..```p
-00000f90: 7974 686f 6e0a 6e61 6d65 203d 2064 6275  ython.name = dbu
-00000fa0: 7469 6c73 2e77 6964 6765 7473 2e67 6574  tils.widgets.get
-00000fb0: 2822 6e61 6d65 2229 0a6d 6573 7361 6765  ("name").message
-00000fc0: 203d 2066 2244 6f6e 2774 2077 6f72 7279   = f"Don't worry
-00000fd0: 207b 6e61 6d65 7d2c 2049 2067 6f74 2079   {name}, I got y
-00000fe0: 6f75 7220 7265 7175 6573 7421 2057 656c  our request! Wel
-00000ff0: 636f 6d65 2074 6f20 7072 6566 6563 742d  come to prefect-
-00001000: 6461 7461 6272 6963 6b73 2122 0a70 7269  databricks!".pri
-00001010: 6e74 286d 6573 7361 6765 290a 6060 600a  nt(message).```.
-00001020: 0a50 7265 6665 6374 2066 6c6f 7720 7468  .Prefect flow th
-00001030: 6174 206c 6175 6e63 6865 7320 6120 6e65  at launches a ne
-00001040: 7720 636c 7573 7465 7220 746f 2072 756e  w cluster to run
-00001050: 2060 6578 616d 706c 652e 6970 796e 6260   `example.ipynb`
-00001060: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
-00001070: 6d20 7072 6566 6563 7420 696d 706f 7274  m prefect import
-00001080: 2066 6c6f 770a 6672 6f6d 2070 7265 6665   flow.from prefe
-00001090: 6374 5f64 6174 6162 7269 636b 7320 696d  ct_databricks im
-000010a0: 706f 7274 2044 6174 6162 7269 636b 7343  port DatabricksC
-000010b0: 7265 6465 6e74 6961 6c73 0a66 726f 6d20  redentials.from 
-000010c0: 7072 6566 6563 745f 6461 7461 6272 6963  prefect_databric
-000010d0: 6b73 2e6a 6f62 7320 696d 706f 7274 206a  ks.jobs import j
-000010e0: 6f62 735f 7275 6e73 5f73 7562 6d69 740a  obs_runs_submit.
-000010f0: 6672 6f6d 2070 7265 6665 6374 5f64 6174  from prefect_dat
-00001100: 6162 7269 636b 732e 6d6f 6465 6c73 2e6a  abricks.models.j
-00001110: 6f62 7320 696d 706f 7274 2028 0a20 2020  obs import (.   
-00001120: 2041 7574 6f53 6361 6c65 2c0a 2020 2020   AutoScale,.    
-00001130: 4177 7341 7474 7269 6275 7465 732c 0a20  AwsAttributes,. 
-00001140: 2020 204a 6f62 5461 736b 5365 7474 696e     JobTaskSettin
-00001150: 6773 2c0a 2020 2020 4e6f 7465 626f 6f6b  gs,.    Notebook
-00001160: 5461 736b 2c0a 2020 2020 4e65 7743 6c75  Task,.    NewClu
-00001170: 7374 6572 2c0a 290a 0a0a 4066 6c6f 770a  ster,.)...@flow.
-00001180: 6465 6620 6a6f 6273 5f72 756e 735f 7375  def jobs_runs_su
-00001190: 626d 6974 5f66 6c6f 7728 6e6f 7465 626f  bmit_flow(notebo
-000011a0: 6f6b 5f70 6174 682c 202a 2a62 6173 655f  ok_path, **base_
-000011b0: 7061 7261 6d65 7465 7273 293a 0a20 2020  parameters):.   
-000011c0: 2064 6174 6162 7269 636b 735f 6372 6564   databricks_cred
-000011d0: 656e 7469 616c 7320 3d20 4461 7461 6272  entials = Databr
-000011e0: 6963 6b73 4372 6564 656e 7469 616c 732e  icksCredentials.
-000011f0: 6c6f 6164 2822 6d79 2d62 6c6f 636b 2229  load("my-block")
-00001200: 0a0a 2020 2020 2320 7370 6563 6966 7920  ..    # specify 
-00001210: 6e65 7720 636c 7573 7465 7220 7365 7474  new cluster sett
-00001220: 696e 6773 0a20 2020 2061 7773 5f61 7474  ings.    aws_att
-00001230: 7269 6275 7465 7320 3d20 4177 7341 7474  ributes = AwsAtt
-00001240: 7269 6275 7465 7328 0a20 2020 2020 2020  ributes(.       
-00001250: 2061 7661 696c 6162 696c 6974 793d 2253   availability="S
-00001260: 504f 5422 2c0a 2020 2020 2020 2020 7a6f  POT",.        zo
-00001270: 6e65 5f69 643d 2275 732d 7765 7374 2d32  ne_id="us-west-2
-00001280: 6122 2c0a 2020 2020 2020 2020 6562 735f  a",.        ebs_
-00001290: 766f 6c75 6d65 5f74 7970 653d 2247 454e  volume_type="GEN
-000012a0: 4552 414c 5f50 5552 504f 5345 5f53 5344  ERAL_PURPOSE_SSD
-000012b0: 222c 0a20 2020 2020 2020 2065 6273 5f76  ",.        ebs_v
-000012c0: 6f6c 756d 655f 636f 756e 743d 332c 0a20  olume_count=3,. 
-000012d0: 2020 2020 2020 2065 6273 5f76 6f6c 756d         ebs_volum
-000012e0: 655f 7369 7a65 3d31 3030 2c0a 2020 2020  e_size=100,.    
-000012f0: 290a 2020 2020 6175 746f 5f73 6361 6c65  ).    auto_scale
-00001300: 203d 2041 7574 6f53 6361 6c65 286d 696e   = AutoScale(min
-00001310: 5f77 6f72 6b65 7273 3d31 2c20 6d61 785f  _workers=1, max_
-00001320: 776f 726b 6572 733d 3229 0a20 2020 206e  workers=2).    n
-00001330: 6577 5f63 6c75 7374 6572 203d 204e 6577  ew_cluster = New
-00001340: 436c 7573 7465 7228 0a20 2020 2020 2020  Cluster(.       
-00001350: 2061 7773 5f61 7474 7269 6275 7465 733d   aws_attributes=
-00001360: 6177 735f 6174 7472 6962 7574 6573 2c0a  aws_attributes,.
-00001370: 2020 2020 2020 2020 6175 746f 7363 616c          autoscal
-00001380: 653d 6175 746f 5f73 6361 6c65 2c0a 2020  e=auto_scale,.  
-00001390: 2020 2020 2020 6e6f 6465 5f74 7970 655f        node_type_
-000013a0: 6964 3d22 6d34 2e6c 6172 6765 222c 0a20  id="m4.large",. 
-000013b0: 2020 2020 2020 2073 7061 726b 5f76 6572         spark_ver
-000013c0: 7369 6f6e 3d22 3130 2e34 2e78 2d73 6361  sion="10.4.x-sca
-000013d0: 6c61 322e 3132 222c 0a20 2020 2020 2020  la2.12",.       
-000013e0: 2073 7061 726b 5f63 6f6e 663d 7b22 7370   spark_conf={"sp
-000013f0: 6172 6b2e 7370 6563 756c 6174 696f 6e22  ark.speculation"
-00001400: 3a20 5472 7565 7d2c 0a20 2020 2029 0a0a  : True},.    )..
-00001410: 2020 2020 2320 7370 6563 6966 7920 6e6f      # specify no
-00001420: 7465 626f 6f6b 2074 6f20 7573 6520 616e  tebook to use an
-00001430: 6420 7061 7261 6d65 7465 7273 2074 6f20  d parameters to 
-00001440: 7061 7373 0a20 2020 206e 6f74 6562 6f6f  pass.    noteboo
-00001450: 6b5f 7461 736b 203d 204e 6f74 6562 6f6f  k_task = Noteboo
-00001460: 6b54 6173 6b28 0a20 2020 2020 2020 206e  kTask(.        n
-00001470: 6f74 6562 6f6f 6b5f 7061 7468 3d6e 6f74  otebook_path=not
-00001480: 6562 6f6f 6b5f 7061 7468 2c0a 2020 2020  ebook_path,.    
-00001490: 2020 2020 6261 7365 5f70 6172 616d 6574      base_paramet
-000014a0: 6572 733d 6261 7365 5f70 6172 616d 6574  ers=base_paramet
-000014b0: 6572 732c 0a20 2020 2029 0a0a 2020 2020  ers,.    )..    
-000014c0: 2320 636f 6d70 696c 6520 6a6f 6220 7461  # compile job ta
-000014d0: 736b 2073 6574 7469 6e67 730a 2020 2020  sk settings.    
-000014e0: 6a6f 625f 7461 736b 5f73 6574 7469 6e67  job_task_setting
-000014f0: 7320 3d20 4a6f 6254 6173 6b53 6574 7469  s = JobTaskSetti
-00001500: 6e67 7328 0a20 2020 2020 2020 206e 6577  ngs(.        new
-00001510: 5f63 6c75 7374 6572 3d6e 6577 5f63 6c75  _cluster=new_clu
-00001520: 7374 6572 2c0a 2020 2020 2020 2020 6e6f  ster,.        no
-00001530: 7465 626f 6f6b 5f74 6173 6b3d 6e6f 7465  tebook_task=note
-00001540: 626f 6f6b 5f74 6173 6b2c 0a20 2020 2020  book_task,.     
-00001550: 2020 2074 6173 6b5f 6b65 793d 2270 7265     task_key="pre
-00001560: 6665 6374 2d74 6173 6b22 0a20 2020 2029  fect-task".    )
-00001570: 0a0a 2020 2020 7275 6e20 3d20 6a6f 6273  ..    run = jobs
-00001580: 5f72 756e 735f 7375 626d 6974 280a 2020  _runs_submit(.  
-00001590: 2020 2020 2020 6461 7461 6272 6963 6b73        databricks
-000015a0: 5f63 7265 6465 6e74 6961 6c73 3d64 6174  _credentials=dat
-000015b0: 6162 7269 636b 735f 6372 6564 656e 7469  abricks_credenti
-000015c0: 616c 732c 0a20 2020 2020 2020 2072 756e  als,.        run
-000015d0: 5f6e 616d 653d 2270 7265 6665 6374 2d6a  _name="prefect-j
-000015e0: 6f62 222c 0a20 2020 2020 2020 2074 6173  ob",.        tas
-000015f0: 6b73 3d5b 6a6f 625f 7461 736b 5f73 6574  ks=[job_task_set
-00001600: 7469 6e67 735d 0a20 2020 2029 0a0a 2020  tings].    )..  
-00001610: 2020 7265 7475 726e 2072 756e 0a0a 0a6a    return run...j
-00001620: 6f62 735f 7275 6e73 5f73 7562 6d69 745f  obs_runs_submit_
-00001630: 666c 6f77 2822 2f55 7365 7273 2f75 7365  flow("/Users/use
-00001640: 726e 616d 6540 676d 6169 6c2e 636f 6d2f  rname@gmail.com/
-00001650: 6578 616d 706c 652e 6970 796e 6222 2c20  example.ipynb", 
-00001660: 6e61 6d65 3d22 4d61 7276 696e 2229 0a60  name="Marvin").`
-00001670: 6060 0a0a 4e6f 7465 2c20 696e 7374 6561  ``..Note, instea
-00001680: 6420 6f66 2075 7369 6e67 2074 6865 2062  d of using the b
-00001690: 7569 6c74 2d69 6e20 6d6f 6465 6c73 2c20  uilt-in models, 
-000016a0: 796f 7520 6d61 7920 616c 736f 2069 6e70  you may also inp
-000016b0: 7574 2076 616c 6964 204a 534f 4e2e 2046  ut valid JSON. F
-000016c0: 6f72 2065 7861 6d70 6c65 2c20 6041 7574  or example, `Aut
-000016d0: 6f53 6361 6c65 286d 696e 5f77 6f72 6b65  oScale(min_worke
-000016e0: 7273 3d31 2c20 6d61 785f 776f 726b 6572  rs=1, max_worker
-000016f0: 733d 3229 6020 6973 2065 7175 6976 616c  s=2)` is equival
-00001700: 656e 7420 746f 2060 7b22 6d69 6e5f 776f  ent to `{"min_wo
-00001710: 726b 6572 7322 3a20 312c 2022 6d61 785f  rkers": 1, "max_
-00001720: 776f 726b 6572 7322 3a20 327d 602e 0a0a  workers": 2}`...
-00001730: 466f 7220 6d6f 7265 2074 6970 7320 6f6e  For more tips on
-00001740: 2068 6f77 2074 6f20 7573 6520 7461 736b   how to use task
-00001750: 7320 616e 6420 666c 6f77 7320 696e 2061  s and flows in a
-00001760: 2043 6f6c 6c65 6374 696f 6e2c 2063 6865   Collection, che
-00001770: 636b 206f 7574 205b 5573 696e 6720 436f  ck out [Using Co
-00001780: 6c6c 6563 7469 6f6e 735d 2868 7474 7073  llections](https
-00001790: 3a2f 2f6f 7269 6f6e 2d64 6f63 732e 7072  ://orion-docs.pr
-000017a0: 6566 6563 742e 696f 2f63 6f6c 6c65 6374  efect.io/collect
-000017b0: 696f 6e73 2f75 7361 6765 2f29 210a 0a23  ions/usage/)!..#
-000017c0: 2320 5265 736f 7572 6365 730a 0a49 6620  # Resources..If 
-000017d0: 796f 7520 656e 636f 756e 7465 7220 616e  you encounter an
-000017e0: 7920 6275 6773 2077 6869 6c65 2075 7369  y bugs while usi
-000017f0: 6e67 2060 7072 6566 6563 742d 6461 7461  ng `prefect-data
-00001800: 6272 6963 6b73 602c 2066 6565 6c20 6672  bricks`, feel fr
-00001810: 6565 2074 6f20 6f70 656e 2061 6e20 6973  ee to open an is
-00001820: 7375 6520 696e 2074 6865 205b 7072 6566  sue in the [pref
-00001830: 6563 742d 6461 7461 6272 6963 6b73 5d28  ect-databricks](
-00001840: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001850: 6f6d 2f50 7265 6665 6374 4851 2f70 7265  om/PrefectHQ/pre
-00001860: 6665 6374 2d64 6174 6162 7269 636b 7329  fect-databricks)
-00001870: 2072 6570 6f73 6974 6f72 792e 0a0a 4966   repository...If
-00001880: 2079 6f75 2068 6176 6520 616e 7920 7175   you have any qu
-00001890: 6573 7469 6f6e 7320 6f72 2069 7373 7565  estions or issue
-000018a0: 7320 7768 696c 6520 7573 696e 6720 6070  s while using `p
-000018b0: 7265 6665 6374 2d64 6174 6162 7269 636b  refect-databrick
-000018c0: 7360 2c20 796f 7520 6361 6e20 6669 6e64  s`, you can find
-000018d0: 2068 656c 7020 696e 2065 6974 6865 7220   help in either 
-000018e0: 7468 6520 5b50 7265 6665 6374 2044 6973  the [Prefect Dis
-000018f0: 636f 7572 7365 2066 6f72 756d 5d28 6874  course forum](ht
-00001900: 7470 733a 2f2f 6469 7363 6f75 7273 652e  tps://discourse.
-00001910: 7072 6566 6563 742e 696f 2f29 206f 7220  prefect.io/) or 
-00001920: 7468 6520 5b50 7265 6665 6374 2053 6c61  the [Prefect Sla
-00001930: 636b 2063 6f6d 6d75 6e69 7479 5d28 6874  ck community](ht
-00001940: 7470 733a 2f2f 7072 6566 6563 742e 696f  tps://prefect.io
-00001950: 2f73 6c61 636b 292e 0a0a 4665 656c 2066  /slack)...Feel f
-00001960: 7265 6520 746f 2073 7461 7220 6f72 2077  ree to star or w
-00001970: 6174 6368 205b 6070 7265 6665 6374 2d64  atch [`prefect-d
-00001980: 6174 6162 7269 636b 7360 5d28 6874 7470  atabricks`](http
-00001990: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f50  s://github.com/P
-000019a0: 7265 6665 6374 4851 2f70 7265 6665 6374  refectHQ/prefect
-000019b0: 2d64 6174 6162 7269 636b 7329 2066 6f72  -databricks) for
-000019c0: 2075 7064 6174 6573 2074 6f6f 210a 0a23   updates too!..#
-000019d0: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
-000019e0: 4966 2079 6f75 2764 206c 696b 6520 746f  If you'd like to
-000019f0: 2068 656c 7020 636f 6e74 7269 6275 7465   help contribute
-00001a00: 2074 6f20 6669 7820 616e 2069 7373 7565   to fix an issue
-00001a10: 206f 7220 6164 6420 6120 6665 6174 7572   or add a featur
-00001a20: 6520 746f 2060 7072 6566 6563 742d 6461  e to `prefect-da
-00001a30: 7461 6272 6963 6b73 602c 2070 6c65 6173  tabricks`, pleas
-00001a40: 6520 5b70 726f 706f 7365 2063 6861 6e67  e [propose chang
-00001a50: 6573 2074 6872 6f75 6768 2061 2070 756c  es through a pul
-00001a60: 6c20 7265 7175 6573 7420 6672 6f6d 2061  l request from a
-00001a70: 2066 6f72 6b20 6f66 2074 6865 2072 6570   fork of the rep
-00001a80: 6f73 6974 6f72 795d 2868 7474 7073 3a2f  ository](https:/
-00001a90: 2f64 6f63 732e 6769 7468 7562 2e63 6f6d  /docs.github.com
-00001aa0: 2f65 6e2f 7075 6c6c 2d72 6571 7565 7374  /en/pull-request
-00001ab0: 732f 636f 6c6c 6162 6f72 6174 696e 672d  s/collaborating-
-00001ac0: 7769 7468 2d70 756c 6c2d 7265 7175 6573  with-pull-reques
-00001ad0: 7473 2f70 726f 706f 7369 6e67 2d63 6861  ts/proposing-cha
-00001ae0: 6e67 6573 2d74 6f2d 796f 7572 2d77 6f72  nges-to-your-wor
-00001af0: 6b2d 7769 7468 2d70 756c 6c2d 7265 7175  k-with-pull-requ
-00001b00: 6573 7473 2f63 7265 6174 696e 672d 612d  ests/creating-a-
-00001b10: 7075 6c6c 2d72 6571 7565 7374 2d66 726f  pull-request-fro
-00001b20: 6d2d 612d 666f 726b 292e 0a0a 4865 7265  m-a-fork)...Here
-00001b30: 2061 7265 2074 6865 2073 7465 7073 3a0a   are the steps:.
-00001b40: 312e 205b 466f 726b 2074 6865 2072 6570  1. [Fork the rep
-00001b50: 6f73 6974 6f72 795d 2868 7474 7073 3a2f  ository](https:/
-00001b60: 2f64 6f63 732e 6769 7468 7562 2e63 6f6d  /docs.github.com
-00001b70: 2f65 6e2f 6765 742d 7374 6172 7465 642f  /en/get-started/
-00001b80: 7175 6963 6b73 7461 7274 2f66 6f72 6b2d  quickstart/fork-
-00001b90: 612d 7265 706f 2366 6f72 6b69 6e67 2d61  a-repo#forking-a
-00001ba0: 2d72 6570 6f73 6974 6f72 7929 0a32 2e20  -repository).2. 
-00001bb0: 5b43 6c6f 6e65 2074 6865 2066 6f72 6b65  [Clone the forke
-00001bc0: 6420 7265 706f 7369 746f 7279 5d28 6874  d repository](ht
-00001bd0: 7470 733a 2f2f 646f 6373 2e67 6974 6875  tps://docs.githu
-00001be0: 622e 636f 6d2f 656e 2f67 6574 2d73 7461  b.com/en/get-sta
-00001bf0: 7274 6564 2f71 7569 636b 7374 6172 742f  rted/quickstart/
-00001c00: 666f 726b 2d61 2d72 6570 6f23 636c 6f6e  fork-a-repo#clon
-00001c10: 696e 672d 796f 7572 2d66 6f72 6b65 642d  ing-your-forked-
-00001c20: 7265 706f 7369 746f 7279 290a 332e 2049  repository).3. I
-00001c30: 6e73 7461 6c6c 2074 6865 2072 6570 6f73  nstall the repos
-00001c40: 6974 6f72 7920 616e 6420 6974 7320 6465  itory and its de
-00001c50: 7065 6e64 656e 6369 6573 3a0a 6060 600a  pendencies:.```.
-00001c60: 7069 7020 696e 7374 616c 6c20 2d65 2022  pip install -e "
-00001c70: 2e5b 6465 765d 220a 6060 600a 342e 204d  .[dev]".```.4. M
-00001c80: 616b 6520 6465 7369 7265 6420 6368 616e  ake desired chan
-00001c90: 6765 730a 352e 2041 6464 2074 6573 7473  ges.5. Add tests
-00001ca0: 0a36 2e20 496e 7365 7274 2061 6e20 656e  .6. Insert an en
-00001cb0: 7472 7920 746f 205b 4348 414e 4745 4c4f  try to [CHANGELO
-00001cc0: 472e 6d64 5d28 6874 7470 733a 2f2f 6769  G.md](https://gi
-00001cd0: 7468 7562 2e63 6f6d 2f50 7265 6665 6374  thub.com/Prefect
-00001ce0: 4851 2f70 7265 6665 6374 2d64 6174 6162  HQ/prefect-datab
-00001cf0: 7269 636b 732f 626c 6f62 2f6d 6169 6e2f  ricks/blob/main/
-00001d00: 4348 414e 4745 4c4f 472e 6d64 290a 372e  CHANGELOG.md).7.
-00001d10: 2049 6e73 7461 6c6c 2060 7072 652d 636f   Install `pre-co
-00001d20: 6d6d 6974 6020 746f 2070 6572 666f 726d  mmit` to perform
-00001d30: 2071 7561 6c69 7479 2063 6865 636b 7320   quality checks 
-00001d40: 7072 696f 7220 746f 2063 6f6d 6d69 743a  prior to commit:
-00001d50: 0a60 6060 0a70 7265 2d63 6f6d 6d69 7420  .```.pre-commit 
-00001d60: 696e 7374 616c 6c0a 6060 600a 382e 2060  install.```.8. `
-00001d70: 6769 7420 636f 6d6d 6974 602c 2060 6769  git commit`, `gi
-00001d80: 7420 7075 7368 602c 2061 6e64 2063 7265  t push`, and cre
-00001d90: 6174 6520 6120 7075 6c6c 2072 6571 7565  ate a pull reque
-00001da0: 7374 0a                                  st.
+00000390: 496e 7465 6772 6174 6520 4461 7461 6272  Integrate Databr
+000003a0: 6963 6b73 206a 6f62 7320 696e 746f 2079  icks jobs into y
+000003b0: 6f75 7220 6461 7461 666c 6f77 2077 6974  our dataflow wit
+000003c0: 6820 7072 6566 6563 742d 6461 7461 6272  h prefect-databr
+000003d0: 6963 6b73 0a20 0a3c 7020 616c 6967 6e3d  icks. .<p align=
+000003e0: 2263 656e 7465 7222 3e0a 2020 2020 3c69  "center">.    <i
+000003f0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000400: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
+00000410: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00000420: 6d2f 3135 3333 3139 3930 2f32 3139 3832  m/15331990/21982
+00000430: 3234 3339 2d37 3065 6338 3266 622d 6539  2439-70ec82fb-e9
+00000440: 3361 2d34 3938 332d 6265 6337 2d38 6338  3a-4983-bec7-8c8
+00000450: 3235 3066 6262 3761 632e 706e 6722 3e0a  250fbb7ac.png">.
+00000460: 2020 2020 3c62 723e 0a20 2020 203c 6120      <br>.    <a 
+00000470: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000480: 7069 2e70 7974 686f 6e2e 6f72 672f 7079  pi.python.org/py
+00000490: 7069 2f70 7265 6665 6374 2d64 6174 6162  pi/prefect-datab
+000004a0: 7269 636b 732f 2220 616c 743d 2250 7950  ricks/" alt="PyP
+000004b0: 4920 7665 7273 696f 6e22 3e0a 2020 2020  I version">.    
+000004c0: 2020 2020 3c69 6d67 2061 6c74 3d22 5079      <img alt="Py
+000004d0: 5049 2220 7372 633d 2268 7474 7073 3a2f  PI" src="https:/
+000004e0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000004f0: 7079 7069 2f76 2f70 7265 6665 6374 2d64  pypi/v/prefect-d
+00000500: 6174 6162 7269 636b 733f 636f 6c6f 723d  atabricks?color=
+00000510: 3030 3532 4646 266c 6162 656c 436f 6c6f  0052FF&labelColo
+00000520: 723d 3039 3034 3232 223e 3c2f 613e 0a20  r=090422"></a>. 
+00000530: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000540: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f50  s://github.com/P
+00000550: 7265 6665 6374 4851 2f70 7265 6665 6374  refectHQ/prefect
+00000560: 2d64 6174 6162 7269 636b 732f 2220 616c  -databricks/" al
+00000570: 743d 2253 7461 7273 223e 0a20 2020 2020  t="Stars">.     
+00000580: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000590: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000005a0: 2e69 6f2f 6769 7468 7562 2f73 7461 7273  .io/github/stars
+000005b0: 2f50 7265 6665 6374 4851 2f70 7265 6665  /PrefectHQ/prefe
+000005c0: 6374 2d64 6174 6162 7269 636b 733f 636f  ct-databricks?co
+000005d0: 6c6f 723d 3030 3532 4646 266c 6162 656c  lor=0052FF&label
+000005e0: 436f 6c6f 723d 3039 3034 3232 2220 2f3e  Color=090422" />
+000005f0: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00000600: 3d22 6874 7470 733a 2f2f 7065 7079 2e74  ="https://pepy.t
+00000610: 6563 682f 6261 6467 652f 7072 6566 6563  ech/badge/prefec
+00000620: 742d 6461 7461 6272 6963 6b73 2f22 2061  t-databricks/" a
+00000630: 6c74 3d22 446f 776e 6c6f 6164 7322 3e0a  lt="Downloads">.
+00000640: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000650: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000660: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
+00000670: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
+00000680: 636b 733f 636f 6c6f 723d 3030 3532 4646  cks?color=0052FF
+00000690: 266c 6162 656c 436f 6c6f 723d 3039 3034  &labelColor=0904
+000006a0: 3232 2220 2f3e 3c2f 613e 0a20 2020 203c  22" /></a>.    <
+000006b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000006c0: 6769 7468 7562 2e63 6f6d 2f50 7265 6665  github.com/Prefe
+000006d0: 6374 4851 2f70 7265 6665 6374 2d64 6174  ctHQ/prefect-dat
+000006e0: 6162 7269 636b 732f 7075 6c73 6522 2061  abricks/pulse" a
+000006f0: 6c74 3d22 4163 7469 7669 7479 223e 0a20  lt="Activity">. 
+00000700: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+00000710: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000720: 656c 6473 2e69 6f2f 6769 7468 7562 2f63  elds.io/github/c
+00000730: 6f6d 6d69 742d 6163 7469 7669 7479 2f6d  ommit-activity/m
+00000740: 2f50 7265 6665 6374 4851 2f70 7265 6665  /PrefectHQ/prefe
+00000750: 6374 2d64 6174 6162 7269 636b 733f 636f  ct-databricks?co
+00000760: 6c6f 723d 3030 3532 4646 266c 6162 656c  lor=0052FF&label
+00000770: 436f 6c6f 723d 3039 3034 3232 2220 2f3e  Color=090422" />
+00000780: 3c2f 613e 0a20 2020 203c 6272 3e0a 2020  </a>.    <br>.  
+00000790: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000007a0: 3a2f 2f70 7265 6665 6374 2d63 6f6d 6d75  ://prefect-commu
+000007b0: 6e69 7479 2e73 6c61 636b 2e63 6f6d 2220  nity.slack.com" 
+000007c0: 616c 743d 2253 6c61 636b 223e 0a20 2020  alt="Slack">.   
+000007d0: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+000007e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000007f0: 6473 2e69 6f2f 6261 6467 652f 736c 6163  ds.io/badge/slac
+00000800: 6b2d 6a6f 696e 5f63 6f6d 6d75 6e69 7479  k-join_community
+00000810: 2d72 6564 2e73 7667 3f63 6f6c 6f72 3d30  -red.svg?color=0
+00000820: 3035 3246 4626 6c61 6265 6c43 6f6c 6f72  052FF&labelColor
+00000830: 3d30 3930 3432 3226 6c6f 676f 3d73 6c61  =090422&logo=sla
+00000840: 636b 2220 2f3e 3c2f 613e 0a20 2020 203c  ck" /></a>.    <
+00000850: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000860: 6469 7363 6f75 7273 652e 7072 6566 6563  discourse.prefec
+00000870: 742e 696f 2f22 2061 6c74 3d22 4469 7363  t.io/" alt="Disc
+00000880: 6f75 7273 6522 3e0a 2020 2020 2020 2020  ourse">.        
+00000890: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000008a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000008b0: 2f62 6164 6765 2f64 6973 636f 7572 7365  /badge/discourse
+000008c0: 2d62 726f 7773 655f 666f 7275 6d2d 7265  -browse_forum-re
+000008d0: 642e 7376 673f 636f 6c6f 723d 3030 3532  d.svg?color=0052
+000008e0: 4646 266c 6162 656c 436f 6c6f 723d 3039  FF&labelColor=09
+000008f0: 3034 3232 266c 6f67 6f3d 6469 7363 6f75  0422&logo=discou
+00000900: 7273 6522 202f 3e3c 2f61 3e0a 3c2f 703e  rse" /></a>.</p>
+00000910: 0a0a 5669 7369 7420 7468 6520 6675 6c6c  ..Visit the full
+00000920: 2064 6f63 7320 5b68 6572 655d 2868 7474   docs [here](htt
+00000930: 7073 3a2f 2f50 7265 6665 6374 4851 2e67  ps://PrefectHQ.g
+00000940: 6974 6875 622e 696f 2f70 7265 6665 6374  ithub.io/prefect
+00000950: 2d64 6174 6162 7269 636b 7329 2074 6f20  -databricks) to 
+00000960: 7365 6520 6164 6469 7469 6f6e 616c 2065  see additional e
+00000970: 7861 6d70 6c65 7320 616e 6420 7468 6520  xamples and the 
+00000980: 4150 4920 7265 6665 7265 6e63 652e 0a0a  API reference...
+00000990: 5468 6520 7072 6566 6563 742d 6461 7461  The prefect-data
+000009a0: 6272 6963 6b73 2063 6f6c 6c65 6374 696f  bricks collectio
+000009b0: 6e20 6d61 6b65 7320 6974 2065 6173 7920  n makes it easy 
+000009c0: 746f 2063 6f6f 7264 6961 6e74 6520 4461  to coordiante Da
+000009d0: 7461 6272 6963 6b73 206a 6f62 7320 7769  tabricks jobs wi
+000009e0: 7468 206f 7468 6572 2074 6f6f 6c73 2069  th other tools i
+000009f0: 6e20 796f 7572 2064 6174 6120 7374 6163  n your data stac
+00000a00: 6b20 7573 696e 6720 5072 6566 6563 742e  k using Prefect.
+00000a10: 2043 6865 636b 206f 7574 2074 6865 2065   Check out the e
+00000a20: 7861 6d70 6c65 7320 6265 6c6f 7720 746f  xamples below to
+00000a30: 2067 6574 2073 7461 7274 6564 210a 0a23   get started!..#
+00000a40: 2320 4765 7474 696e 6720 5374 6172 7465  # Getting Starte
+00000a50: 640a 0a23 2323 2049 6e74 6567 7261 7465  d..### Integrate
+00000a60: 2077 6974 6820 5072 6566 6563 7420 666c   with Prefect fl
+00000a70: 6f77 730a 0a55 7369 6e67 2050 7265 6665  ows..Using Prefe
+00000a80: 6374 2077 6974 6820 4461 7461 6272 6963  ct with Databric
+00000a90: 6b73 2061 6c6c 6f77 7320 796f 7520 746f  ks allows you to
+00000aa0: 2064 6566 696e 6520 616e 6420 6f72 6368   define and orch
+00000ab0: 6573 7472 6174 6520 636f 6d70 6c65 7820  estrate complex 
+00000ac0: 6461 7461 2077 6f72 6b66 6c6f 7773 2074  data workflows t
+00000ad0: 6861 7420 7461 6b65 2061 6476 616e 7461  hat take advanta
+00000ae0: 6765 206f 6620 7468 6520 7363 616c 6162  ge of the scalab
+00000af0: 696c 6974 7920 616e 6420 7065 7266 6f72  ility and perfor
+00000b00: 6d61 6e63 6520 6f66 2044 6174 6162 7269  mance of Databri
+00000b10: 636b 732e 0a0a 5468 6973 2063 616e 2062  cks...This can b
+00000b20: 6520 6573 7065 6369 616c 6c79 2075 7365  e especially use
+00000b30: 6675 6c20 666f 7220 6461 7461 2d69 6e74  ful for data-int
+00000b40: 656e 7369 7665 2074 6173 6b73 2073 7563  ensive tasks suc
+00000b50: 6820 6173 2045 544c 2028 6578 7472 6163  h as ETL (extrac
+00000b60: 742c 2074 7261 6e73 666f 726d 2c20 6c6f  t, transform, lo
+00000b70: 6164 2920 7069 7065 6c69 6e65 732c 206d  ad) pipelines, m
+00000b80: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
+00000b90: 7472 6169 6e69 6e67 2061 6e64 2069 6e66  training and inf
+00000ba0: 6572 656e 6365 2c20 616e 6420 7265 616c  erence, and real
+00000bb0: 2d74 696d 6520 6461 7461 2070 726f 6365  -time data proce
+00000bc0: 7373 696e 672e 0a0a 4265 6c6f 7720 6973  ssing...Below is
+00000bd0: 2061 6e20 6578 616d 706c 6520 6f66 2068   an example of h
+00000be0: 6f77 2079 6f75 2063 616e 2069 6e63 6f72  ow you can incor
+00000bf0: 706f 7261 7465 2044 6174 6162 7269 636b  porate Databrick
+00000c00: 7320 6e6f 7465 626f 6f6b 7320 7769 7468  s notebooks with
+00000c10: 696e 2079 6f75 7220 5072 6566 6563 7420  in your Prefect 
+00000c20: 666c 6f77 732e 0a0a 4265 2073 7572 6520  flows...Be sure 
+00000c30: 746f 2069 6e73 7461 6c6c 205b 7072 6566  to install [pref
+00000c40: 6563 742d 6461 7461 6272 6963 6b73 5d28  ect-databricks](
+00000c50: 2369 6e73 7461 6c6c 6174 696f 6e29 2061  #installation) a
+00000c60: 6e64 205b 7361 7665 2061 2063 7265 6465  nd [save a crede
+00000c70: 6e74 6961 6c73 2062 6c6f 636b 5d28 2373  ntials block](#s
+00000c80: 6176 696e 672d 6372 6564 656e 7469 616c  aving-credential
+00000c90: 732d 746f 2d62 6c6f 636b 2920 746f 2072  s-to-block) to r
+00000ca0: 756e 2074 6865 2065 7861 6d70 6c65 7320  un the examples 
+00000cb0: 6265 6c6f 7721 0a0a 4966 2079 6f75 2064  below!..If you d
+00000cc0: 6f6e 2774 2068 6176 6520 616e 2065 7869  on't have an exi
+00000cd0: 7374 696e 6720 6e6f 7465 626f 6f6b 2072  sting notebook r
+00000ce0: 6561 6479 206f 6e20 4461 7461 6272 6963  eady on Databric
+00000cf0: 6b73 2c20 796f 7520 6361 6e20 636f 7079  ks, you can copy
+00000d00: 2074 6865 2066 6f6c 6c6f 7769 6e67 2c20   the following, 
+00000d10: 616e 6420 6e61 6d65 2069 7420 6065 7861  and name it `exa
+00000d20: 6d70 6c65 2e69 7079 6e62 602e 2054 6869  mple.ipynb`. Thi
+00000d30: 7320 6e6f 7465 626f 6f6b 2c20 6163 6365  s notebook, acce
+00000d40: 7074 7320 6120 6e61 6d65 2070 6172 616d  pts a name param
+00000d50: 6574 6572 2066 726f 6d20 7468 6520 666c  eter from the fl
+00000d60: 6f77 2061 6e64 2073 696d 706c 7920 7072  ow and simply pr
+00000d70: 696e 7473 2061 206d 6573 7361 6765 2e0a  ints a message..
+00000d80: 0a60 6060 7079 7468 6f6e 0a6e 616d 6520  .```python.name 
+00000d90: 3d20 6462 7574 696c 732e 7769 6467 6574  = dbutils.widget
+00000da0: 732e 6765 7428 226e 616d 6522 290a 6d65  s.get("name").me
+00000db0: 7373 6167 6520 3d20 6622 446f 6e27 7420  ssage = f"Don't 
+00000dc0: 776f 7272 7920 7b6e 616d 657d 2c20 4920  worry {name}, I 
+00000dd0: 676f 7420 796f 7572 2072 6571 7565 7374  got your request
+00000de0: 2120 5765 6c63 6f6d 6520 746f 2070 7265  ! Welcome to pre
+00000df0: 6665 6374 2d64 6174 6162 7269 636b 7321  fect-databricks!
+00000e00: 220a 7072 696e 7428 6d65 7373 6167 6529  ".print(message)
+00000e10: 0a60 6060 0a0a 4865 7265 2c20 7468 6520  .```..Here, the 
+00000e20: 666c 6f77 206c 6175 6e63 6865 7320 6120  flow launches a 
+00000e30: 6e65 7720 636c 7573 7465 7220 746f 2072  new cluster to r
+00000e40: 756e 2060 6578 616d 706c 652e 6970 796e  un `example.ipyn
+00000e50: 6260 2061 6e64 2077 6169 7473 2066 6f72  b` and waits for
+00000e60: 2074 6865 2063 6f6d 706c 6574 696f 6e20   the completion 
+00000e70: 6f66 2074 6865 206e 6f74 6562 6f6f 6b20  of the notebook 
+00000e80: 7275 6e2e 2052 6570 6c61 6365 2074 6865  run. Replace the
+00000e90: 2070 6c61 6365 686f 6c64 6572 7320 616e   placeholders an
+00000ea0: 6420 7275 6e2e 0a0a 6060 6070 7974 686f  d run...```pytho
+00000eb0: 6e0a 6672 6f6d 2070 7265 6665 6374 2069  n.from prefect i
+00000ec0: 6d70 6f72 7420 666c 6f77 0a66 726f 6d20  mport flow.from 
+00000ed0: 7072 6566 6563 745f 6461 7461 6272 6963  prefect_databric
+00000ee0: 6b73 2069 6d70 6f72 7420 4461 7461 6272  ks import Databr
+00000ef0: 6963 6b73 4372 6564 656e 7469 616c 730a  icksCredentials.
+00000f00: 6672 6f6d 2070 7265 6665 6374 5f64 6174  from prefect_dat
+00000f10: 6162 7269 636b 732e 666c 6f77 7320 696d  abricks.flows im
+00000f20: 706f 7274 206a 6f62 735f 7275 6e73 5f73  port jobs_runs_s
+00000f30: 7562 6d69 745f 616e 645f 7761 6974 5f66  ubmit_and_wait_f
+00000f40: 6f72 5f63 6f6d 706c 6574 696f 6e0a 6672  or_completion.fr
+00000f50: 6f6d 2070 7265 6665 6374 5f64 6174 6162  om prefect_datab
+00000f60: 7269 636b 732e 6d6f 6465 6c73 2e6a 6f62  ricks.models.job
+00000f70: 7320 696d 706f 7274 2028 0a20 2020 2041  s import (.    A
+00000f80: 7574 6f53 6361 6c65 2c0a 2020 2020 4177  utoScale,.    Aw
+00000f90: 7341 7474 7269 6275 7465 732c 0a20 2020  sAttributes,.   
+00000fa0: 204a 6f62 5461 736b 5365 7474 696e 6773   JobTaskSettings
+00000fb0: 2c0a 2020 2020 4e6f 7465 626f 6f6b 5461  ,.    NotebookTa
+00000fc0: 736b 2c0a 2020 2020 4e65 7743 6c75 7374  sk,.    NewClust
+00000fd0: 6572 2c0a 290a 0a0a 4066 6c6f 770a 6465  er,.)...@flow.de
+00000fe0: 6620 6a6f 6273 5f72 756e 735f 7375 626d  f jobs_runs_subm
+00000ff0: 6974 5f66 6c6f 7728 626c 6f63 6b5f 6e61  it_flow(block_na
+00001000: 6d65 3a20 7374 722c 206e 6f74 6562 6f6f  me: str, noteboo
+00001010: 6b5f 7061 7468 3a20 7374 722c 202a 2a62  k_path: str, **b
+00001020: 6173 655f 7061 7261 6d65 7465 7273 293a  ase_parameters):
+00001030: 0a20 2020 2064 6174 6162 7269 636b 735f  .    databricks_
+00001040: 6372 6564 656e 7469 616c 7320 3d20 4461  credentials = Da
+00001050: 7461 6272 6963 6b73 4372 6564 656e 7469  tabricksCredenti
+00001060: 616c 732e 6c6f 6164 2862 6c6f 636b 5f6e  als.load(block_n
+00001070: 616d 6529 0a0a 2020 2020 2320 7370 6563  ame)..    # spec
+00001080: 6966 7920 6e65 7720 636c 7573 7465 7220  ify new cluster 
+00001090: 7365 7474 696e 6773 0a20 2020 2061 7773  settings.    aws
+000010a0: 5f61 7474 7269 6275 7465 7320 3d20 4177  _attributes = Aw
+000010b0: 7341 7474 7269 6275 7465 7328 0a20 2020  sAttributes(.   
+000010c0: 2020 2020 2061 7661 696c 6162 696c 6974       availabilit
+000010d0: 793d 2253 504f 5422 2c0a 2020 2020 2020  y="SPOT",.      
+000010e0: 2020 7a6f 6e65 5f69 643d 2275 732d 7765    zone_id="us-we
+000010f0: 7374 2d32 6122 2c0a 2020 2020 2020 2020  st-2a",.        
+00001100: 6562 735f 766f 6c75 6d65 5f74 7970 653d  ebs_volume_type=
+00001110: 2247 454e 4552 414c 5f50 5552 504f 5345  "GENERAL_PURPOSE
+00001120: 5f53 5344 222c 0a20 2020 2020 2020 2065  _SSD",.        e
+00001130: 6273 5f76 6f6c 756d 655f 636f 756e 743d  bs_volume_count=
+00001140: 332c 0a20 2020 2020 2020 2065 6273 5f76  3,.        ebs_v
+00001150: 6f6c 756d 655f 7369 7a65 3d31 3030 2c0a  olume_size=100,.
+00001160: 2020 2020 290a 2020 2020 6175 746f 5f73      ).    auto_s
+00001170: 6361 6c65 203d 2041 7574 6f53 6361 6c65  cale = AutoScale
+00001180: 286d 696e 5f77 6f72 6b65 7273 3d31 2c20  (min_workers=1, 
+00001190: 6d61 785f 776f 726b 6572 733d 3229 0a20  max_workers=2). 
+000011a0: 2020 206e 6577 5f63 6c75 7374 6572 203d     new_cluster =
+000011b0: 204e 6577 436c 7573 7465 7228 0a20 2020   NewCluster(.   
+000011c0: 2020 2020 2061 7773 5f61 7474 7269 6275       aws_attribu
+000011d0: 7465 733d 6177 735f 6174 7472 6962 7574  tes=aws_attribut
+000011e0: 6573 2c0a 2020 2020 2020 2020 6175 746f  es,.        auto
+000011f0: 7363 616c 653d 6175 746f 5f73 6361 6c65  scale=auto_scale
+00001200: 2c0a 2020 2020 2020 2020 6e6f 6465 5f74  ,.        node_t
+00001210: 7970 655f 6964 3d22 6d34 2e6c 6172 6765  ype_id="m4.large
+00001220: 222c 0a20 2020 2020 2020 2073 7061 726b  ",.        spark
+00001230: 5f76 6572 7369 6f6e 3d22 3130 2e34 2e78  _version="10.4.x
+00001240: 2d73 6361 6c61 322e 3132 222c 0a20 2020  -scala2.12",.   
+00001250: 2020 2020 2073 7061 726b 5f63 6f6e 663d       spark_conf=
+00001260: 7b22 7370 6172 6b2e 7370 6563 756c 6174  {"spark.speculat
+00001270: 696f 6e22 3a20 5472 7565 7d2c 0a20 2020  ion": True},.   
+00001280: 2029 0a0a 2020 2020 2320 7370 6563 6966   )..    # specif
+00001290: 7920 6e6f 7465 626f 6f6b 2074 6f20 7573  y notebook to us
+000012a0: 6520 616e 6420 7061 7261 6d65 7465 7273  e and parameters
+000012b0: 2074 6f20 7061 7373 0a20 2020 206e 6f74   to pass.    not
+000012c0: 6562 6f6f 6b5f 7461 736b 203d 204e 6f74  ebook_task = Not
+000012d0: 6562 6f6f 6b54 6173 6b28 0a20 2020 2020  ebookTask(.     
+000012e0: 2020 206e 6f74 6562 6f6f 6b5f 7061 7468     notebook_path
+000012f0: 3d6e 6f74 6562 6f6f 6b5f 7061 7468 2c0a  =notebook_path,.
+00001300: 2020 2020 2020 2020 6261 7365 5f70 6172          base_par
+00001310: 616d 6574 6572 733d 6261 7365 5f70 6172  ameters=base_par
+00001320: 616d 6574 6572 732c 0a20 2020 2029 0a0a  ameters,.    )..
+00001330: 2020 2020 2320 636f 6d70 696c 6520 6a6f      # compile jo
+00001340: 6220 7461 736b 2073 6574 7469 6e67 730a  b task settings.
+00001350: 2020 2020 6a6f 625f 7461 736b 5f73 6574      job_task_set
+00001360: 7469 6e67 7320 3d20 4a6f 6254 6173 6b53  tings = JobTaskS
+00001370: 6574 7469 6e67 7328 0a20 2020 2020 2020  ettings(.       
+00001380: 206e 6577 5f63 6c75 7374 6572 3d6e 6577   new_cluster=new
+00001390: 5f63 6c75 7374 6572 2c0a 2020 2020 2020  _cluster,.      
+000013a0: 2020 6e6f 7465 626f 6f6b 5f74 6173 6b3d    notebook_task=
+000013b0: 6e6f 7465 626f 6f6b 5f74 6173 6b2c 0a20  notebook_task,. 
+000013c0: 2020 2020 2020 2074 6173 6b5f 6b65 793d         task_key=
+000013d0: 2270 7265 6665 6374 2d74 6173 6b22 0a20  "prefect-task". 
+000013e0: 2020 2029 0a0a 2020 2020 7275 6e20 3d20     )..    run = 
+000013f0: 6a6f 6273 5f72 756e 735f 7375 626d 6974  jobs_runs_submit
+00001400: 5f61 6e64 5f77 6169 745f 666f 725f 636f  _and_wait_for_co
+00001410: 6d70 6c65 7469 6f6e 280a 2020 2020 2020  mpletion(.      
+00001420: 2020 6461 7461 6272 6963 6b73 5f63 7265    databricks_cre
+00001430: 6465 6e74 6961 6c73 3d64 6174 6162 7269  dentials=databri
+00001440: 636b 735f 6372 6564 656e 7469 616c 732c  cks_credentials,
+00001450: 0a20 2020 2020 2020 2072 756e 5f6e 616d  .        run_nam
+00001460: 653d 2270 7265 6665 6374 2d6a 6f62 222c  e="prefect-job",
+00001470: 0a20 2020 2020 2020 2074 6173 6b73 3d5b  .        tasks=[
+00001480: 6a6f 625f 7461 736b 5f73 6574 7469 6e67  job_task_setting
+00001490: 735d 0a20 2020 2029 0a0a 2020 2020 7265  s].    )..    re
+000014a0: 7475 726e 2072 756e 0a0a 0a6a 6f62 735f  turn run...jobs_
+000014b0: 7275 6e73 5f73 7562 6d69 745f 666c 6f77  runs_submit_flow
+000014c0: 280a 2020 2020 626c 6f63 6b5f 6e61 6d65  (.    block_name
+000014d0: 3d22 424c 4f43 4b2d 4e41 4d45 2d50 4c41  ="BLOCK-NAME-PLA
+000014e0: 4345 484f 4c44 4552 220a 2020 2020 6e6f  CEHOLDER".    no
+000014f0: 7465 626f 6f6b 5f70 6174 683d 222f 5573  tebook_path="/Us
+00001500: 6572 732f 3c45 4d41 494c 5f41 4444 5245  ers/<EMAIL_ADDRE
+00001510: 5353 5f50 4c41 4345 484f 4c44 4552 3e2f  SS_PLACEHOLDER>/
+00001520: 6578 616d 706c 652e 6970 796e 6222 2c0a  example.ipynb",.
+00001530: 2020 2020 6e61 6d65 3d22 4d61 7276 696e      name="Marvin
+00001540: 220a 290a 6060 600a 0a55 706f 6e20 6578  ".).```..Upon ex
+00001550: 6563 7574 696f 6e2c 2074 6865 206e 6f74  ecution, the not
+00001560: 6562 6f6f 6b20 7275 6e20 7368 6f75 6c64  ebook run should
+00001570: 206f 7574 7075 743a 0a0a 6060 600a 446f   output:..```.Do
+00001580: 6e27 7420 776f 7272 7920 4d61 7276 696e  n't worry Marvin
+00001590: 2c20 4920 676f 7420 796f 7572 2072 6571  , I got your req
+000015a0: 7565 7374 2120 5765 6c63 6f6d 6520 746f  uest! Welcome to
+000015b0: 2070 7265 6665 6374 2d64 6174 6162 7269   prefect-databri
+000015c0: 636b 7321 0a60 6060 0a0a 2121 2120 696e  cks!.```..!!! in
+000015d0: 666f 2022 496e 7075 7420 6469 6374 696f  fo "Input dictio
+000015e0: 6e61 7269 6573 2069 6e20 7468 6520 706c  naries in the pl
+000015f0: 6163 6520 6f66 206d 6f64 656c 7322 0a20  ace of models". 
+00001600: 2020 200a 2020 2020 496e 7374 6561 6420     .    Instead 
+00001610: 6f66 2075 7369 6e67 2074 6865 2062 7569  of using the bui
+00001620: 6c74 2d69 6e20 6d6f 6465 6c73 2c20 796f  lt-in models, yo
+00001630: 7520 6d61 7920 616c 736f 2069 6e70 7574  u may also input
+00001640: 2061 2076 616c 6964 2064 6963 7469 6f6e   a valid diction
+00001650: 6172 792e 0a20 2020 200a 2020 2020 466f  ary..    .    Fo
+00001660: 7220 6578 616d 706c 652c 2074 6865 2066  r example, the f
+00001670: 6f6c 6c6f 7769 6e67 2061 7265 2065 7175  ollowing are equ
+00001680: 6976 616c 656e 743a 0a0a 2020 2020 6060  ivalent:..    ``
+00001690: 6070 7974 686f 6e0a 2020 2020 6175 746f  `python.    auto
+000016a0: 5f73 6361 6c65 3d41 7574 6f53 6361 6c65  _scale=AutoScale
+000016b0: 286d 696e 5f77 6f72 6b65 7273 3d31 2c20  (min_workers=1, 
+000016c0: 6d61 785f 776f 726b 6572 733d 3229 0a20  max_workers=2). 
+000016d0: 2020 2060 6060 0a0a 2020 2020 6060 6070     ```..    ```p
+000016e0: 7974 686f 6e0a 2020 2020 6175 746f 5f73  ython.    auto_s
+000016f0: 6361 6c65 3d7b 226d 696e 5f77 6f72 6b65  cale={"min_worke
+00001700: 7273 223a 2031 2c20 226d 6178 5f77 6f72  rs": 1, "max_wor
+00001710: 6b65 7273 223a 2032 7d0a 2020 2020 6060  kers": 2}.    ``
+00001720: 600a 0a49 6620 796f 7520 6861 7665 2061  `..If you have a
+00001730: 6e20 6578 6973 7469 6e67 2044 6174 6162  n existing Datab
+00001740: 7269 636b 7320 6a6f 622c 2079 6f75 2063  ricks job, you c
+00001750: 616e 2072 756e 2069 7420 7573 696e 6720  an run it using 
+00001760: 606a 6f62 735f 7275 6e73 5f73 7562 6d69  `jobs_runs_submi
+00001770: 745f 6279 5f69 645f 616e 645f 7761 6974  t_by_id_and_wait
+00001780: 5f66 6f72 5f63 6f6d 706c 6574 696f 6e60  _for_completion`
+00001790: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
+000017a0: 6d20 7072 6566 6563 7420 696d 706f 7274  m prefect import
+000017b0: 2066 6c6f 770a 0a66 726f 6d20 7072 6566   flow..from pref
+000017c0: 6563 745f 6461 7461 6272 6963 6b73 2069  ect_databricks i
+000017d0: 6d70 6f72 7420 4461 7461 6272 6963 6b73  mport Databricks
+000017e0: 4372 6564 656e 7469 616c 730a 6672 6f6d  Credentials.from
+000017f0: 2070 7265 6665 6374 5f64 6174 6162 7269   prefect_databri
+00001800: 636b 732e 666c 6f77 7320 696d 706f 7274  cks.flows import
+00001810: 2028 0a20 2020 206a 6f62 735f 7275 6e73   (.    jobs_runs
+00001820: 5f73 7562 6d69 745f 6279 5f69 645f 616e  _submit_by_id_an
+00001830: 645f 7761 6974 5f66 6f72 5f63 6f6d 706c  d_wait_for_compl
+00001840: 6574 696f 6e2c 0a29 0a0a 0a40 666c 6f77  etion,.)...@flow
+00001850: 0a64 6566 2065 7869 7374 696e 675f 6a6f  .def existing_jo
+00001860: 625f 7375 626d 6974 2864 6174 6162 7269  b_submit(databri
+00001870: 636b 735f 6372 6564 656e 7469 616c 735f  cks_credentials_
+00001880: 626c 6f63 6b5f 6e61 6d65 3a20 7374 722c  block_name: str,
+00001890: 206a 6f62 5f69 6429 3a0a 2020 2020 6461   job_id):.    da
+000018a0: 7461 6272 6963 6b73 5f63 7265 6465 6e74  tabricks_credent
+000018b0: 6961 6c73 203d 2044 6174 6162 7269 636b  ials = Databrick
+000018c0: 7343 7265 6465 6e74 6961 6c73 2e6c 6f61  sCredentials.loa
+000018d0: 6428 6e61 6d65 3d62 6c6f 636b 5f6e 616d  d(name=block_nam
+000018e0: 6529 0a0a 2020 2020 7275 6e20 3d20 6a6f  e)..    run = jo
+000018f0: 6273 5f72 756e 735f 7375 626d 6974 5f62  bs_runs_submit_b
+00001900: 795f 6964 5f61 6e64 5f77 6169 745f 666f  y_id_and_wait_fo
+00001910: 725f 636f 6d70 6c65 7469 6f6e 280a 2020  r_completion(.  
+00001920: 2020 2020 2020 6461 7461 6272 6963 6b73        databricks
+00001930: 5f63 7265 6465 6e74 6961 6c73 3d64 6174  _credentials=dat
+00001940: 6162 7269 636b 735f 6372 6564 656e 7469  abricks_credenti
+00001950: 616c 732c 206a 6f62 5f69 643d 6a6f 625f  als, job_id=job_
+00001960: 6964 0a20 2020 2029 0a0a 2020 2020 7265  id.    )..    re
+00001970: 7475 726e 2072 756e 0a0a 6578 6973 7469  turn run..existi
+00001980: 6e67 5f6a 6f62 5f73 7562 6d69 7428 6461  ng_job_submit(da
+00001990: 7461 6272 6963 6b73 5f63 7265 6465 6e74  tabricks_credent
+000019a0: 6961 6c73 5f62 6c6f 636b 5f6e 616d 653d  ials_block_name=
+000019b0: 2264 622d 6372 6564 7322 2c20 6a6f 625f  "db-creds", job_
+000019c0: 6964 3d22 594f 5552 2d4a 4f42 2d4e 414d  id="YOUR-JOB-NAM
+000019d0: 4522 290a 6060 600a 0a23 2320 5265 736f  E").```..## Reso
+000019e0: 7572 6365 730a 0a46 6f72 206d 6f72 6520  urces..For more 
+000019f0: 7469 7073 206f 6e20 686f 7720 746f 2075  tips on how to u
+00001a00: 7365 2074 6173 6b73 2061 6e64 2066 6c6f  se tasks and flo
+00001a10: 7773 2069 6e20 6120 436f 6c6c 6563 7469  ws in a Collecti
+00001a20: 6f6e 2c20 6368 6563 6b20 6f75 7420 5b55  on, check out [U
+00001a30: 7369 6e67 2043 6f6c 6c65 6374 696f 6e73  sing Collections
+00001a40: 5d28 6874 7470 733a 2f2f 6f72 696f 6e2d  ](https://orion-
+00001a50: 646f 6373 2e70 7265 6665 6374 2e69 6f2f  docs.prefect.io/
+00001a60: 636f 6c6c 6563 7469 6f6e 732f 7573 6167  collections/usag
+00001a70: 652f 2921 0a0a 4e6f 7465 2c20 7468 6520  e/)!..Note, the 
+00001a80: 7461 736b 7320 7769 7468 696e 2074 6869  tasks within thi
+00001a90: 7320 636f 6c6c 6563 7469 6f6e 2077 6572  s collection wer
+00001aa0: 6520 6372 6561 7465 6420 6279 2061 2063  e created by a c
+00001ab0: 6f64 6520 6765 6e65 7261 746f 7220 7573  ode generator us
+00001ac0: 696e 6720 7468 6520 7365 7276 6963 6527  ing the service'
+00001ad0: 7320 4f70 656e 4150 4920 7370 6563 2e0a  s OpenAPI spec..
+00001ae0: 0a54 6865 2073 6572 7669 6365 2773 2052  .The service's R
+00001af0: 4553 5420 4150 4920 646f 6375 6d65 6e74  EST API document
+00001b00: 6174 696f 6e20 6361 6e20 6265 2066 6f75  ation can be fou
+00001b10: 6e64 205b 6865 7265 5d28 6874 7470 733a  nd [here](https:
+00001b20: 2f2f 646f 6373 2e64 6174 6162 7269 636b  //docs.databrick
+00001b30: 732e 636f 6d2f 6465 762d 746f 6f6c 732f  s.com/dev-tools/
+00001b40: 6170 692f 6c61 7465 7374 2f69 6e64 6578  api/latest/index
+00001b50: 2e68 746d 6c29 2e0a 0a23 2323 2049 6e73  .html)...### Ins
+00001b60: 7461 6c6c 6174 696f 6e0a 0a49 6e73 7461  tallation..Insta
+00001b70: 6c6c 2060 7072 6566 6563 742d 6461 7461  ll `prefect-data
+00001b80: 6272 6963 6b73 6020 7769 7468 2060 7069  bricks` with `pi
+00001b90: 7060 3a0a 0a60 6060 6261 7368 0a70 6970  p`:..```bash.pip
+00001ba0: 2069 6e73 7461 6c6c 2070 7265 6665 6374   install prefect
+00001bb0: 2d64 6174 6162 7269 636b 730a 6060 600a  -databricks.```.
+00001bc0: 0a52 6571 7569 7265 7320 616e 2069 6e73  .Requires an ins
+00001bd0: 7461 6c6c 6174 696f 6e20 6f66 2050 7974  tallation of Pyt
+00001be0: 686f 6e20 332e 372b 2e0a 0a57 6520 7265  hon 3.7+...We re
+00001bf0: 636f 6d6d 656e 6420 7573 696e 6720 6120  commend using a 
+00001c00: 5079 7468 6f6e 2076 6972 7475 616c 2065  Python virtual e
+00001c10: 6e76 6972 6f6e 6d65 6e74 206d 616e 6167  nvironment manag
+00001c20: 6572 2073 7563 6820 6173 2070 6970 656e  er such as pipen
+00001c30: 762c 2063 6f6e 6461 206f 7220 7669 7274  v, conda or virt
+00001c40: 7561 6c65 6e76 2e0a 0a54 6865 7365 2074  ualenv...These t
+00001c50: 6173 6b73 2061 7265 2064 6573 6967 6e65  asks are designe
+00001c60: 6420 746f 2077 6f72 6b20 7769 7468 2050  d to work with P
+00001c70: 7265 6665 6374 2032 2e20 466f 7220 6d6f  refect 2. For mo
+00001c80: 7265 2069 6e66 6f72 6d61 7469 6f6e 2061  re information a
+00001c90: 626f 7574 2068 6f77 2074 6f20 7573 6520  bout how to use 
+00001ca0: 5072 6566 6563 742c 2070 6c65 6173 6520  Prefect, please 
+00001cb0: 7265 6665 7220 746f 2074 6865 205b 5072  refer to the [Pr
+00001cc0: 6566 6563 7420 646f 6375 6d65 6e74 6174  efect documentat
+00001cd0: 696f 6e5d 2868 7474 7073 3a2f 2f6f 7269  ion](https://ori
+00001ce0: 6f6e 2d64 6f63 732e 7072 6566 6563 742e  on-docs.prefect.
+00001cf0: 696f 2f29 2e0a 0a23 2323 2053 6176 696e  io/)...### Savin
+00001d00: 6720 4372 6564 656e 7469 616c 7320 746f  g Credentials to
+00001d10: 2042 6c6f 636b 0a0a 546f 2075 7365 2074   Block..To use t
+00001d20: 6865 2060 6c6f 6164 6020 6d65 7468 6f64  he `load` method
+00001d30: 206f 6e20 426c 6f63 6b73 2c20 796f 7520   on Blocks, you 
+00001d40: 6d75 7374 2061 6c72 6561 6479 2068 6176  must already hav
+00001d50: 6520 6120 626c 6f63 6b20 646f 6375 6d65  e a block docume
+00001d60: 6e74 205b 7361 7665 6420 7468 726f 7567  nt [saved throug
+00001d70: 6820 636f 6465 5d28 6874 7470 733a 2f2f  h code](https://
+00001d80: 6f72 696f 6e2d 646f 6373 2e70 7265 6665  orion-docs.prefe
+00001d90: 6374 2e69 6f2f 636f 6e63 6570 7473 2f62  ct.io/concepts/b
+00001da0: 6c6f 636b 732f 2373 6176 696e 672d 626c  locks/#saving-bl
+00001db0: 6f63 6b73 2920 6f72 205b 7361 7665 6420  ocks) or [saved 
+00001dc0: 7468 726f 7567 6820 7468 6520 5549 5d28  through the UI](
+00001dd0: 6874 7470 733a 2f2f 6f72 696f 6e2d 646f  https://orion-do
+00001de0: 6373 2e70 7265 6665 6374 2e69 6f2f 7569  cs.prefect.io/ui
+00001df0: 2f62 6c6f 636b 732f 292e 0a0a 4265 6c6f  /blocks/)...Belo
+00001e00: 7720 6973 2061 2077 616c 6b74 6872 6f75  w is a walkthrou
+00001e10: 6768 206f 6e20 7361 7669 6e67 2062 6c6f  gh on saving blo
+00001e20: 636b 2064 6f63 756d 656e 7473 2074 6872  ck documents thr
+00001e30: 6f75 6768 2063 6f64 653b 2073 696d 706c  ough code; simpl
+00001e40: 7920 6372 6561 7465 2061 2073 686f 7274  y create a short
+00001e50: 2073 6372 6970 742c 2072 6570 6c61 6369   script, replaci
+00001e60: 6e67 2074 6865 2070 6c61 6365 686f 6c64  ng the placehold
+00001e70: 6572 732e 200a 0a31 2e20 4865 6164 206f  ers. ..1. Head o
+00001e80: 7665 7220 746f 205b 4461 7461 6272 6963  ver to [Databric
+00001e90: 6b73 5d28 6874 7470 733a 2f2f 6163 636f  ks](https://acco
+00001ea0: 756e 7473 2e63 6c6f 7564 2e64 6174 6162  unts.cloud.datab
+00001eb0: 7269 636b 732e 636f 6d2f 292e 0a32 2e20  ricks.com/)..2. 
+00001ec0: 4c6f 6769 6e20 746f 2079 6f75 7220 4461  Login to your Da
+00001ed0: 7461 6272 6963 6b73 2061 6363 6f75 6e74  tabricks account
+00001ee0: 2061 6e64 2073 656c 6563 7420 6120 776f   and select a wo
+00001ef0: 726b 7370 6163 652e 0a33 2e20 4f6e 2074  rkspace..3. On t
+00001f00: 6865 2074 6f70 2072 6967 6874 2073 6964  he top right sid
+00001f10: 6520 6f66 2074 6865 206e 6176 2062 6172  e of the nav bar
+00001f20: 2c20 636c 6963 6b20 6f6e 2079 6f75 7220  , click on your 
+00001f30: 6163 636f 756e 7420 6e61 6d65 202d 3e20  account name -> 
+00001f40: 5573 6572 2053 6574 7469 6e67 732e 0a34  User Settings..4
+00001f50: 2e20 436c 6963 6b20 4163 6365 7373 2074  . Click Access t
+00001f60: 6f6b 656e 7320 2d3e 2047 656e 6572 6174  okens -> Generat
+00001f70: 6520 6e65 7720 746f 6b65 6e20 2d3e 2047  e new token -> G
+00001f80: 656e 6572 6174 6520 616e 6420 636f 7079  enerate and copy
+00001f90: 2074 6865 2074 6f6b 656e 2e0a 352e 204e   the token..5. N
+00001fa0: 6f74 6520 646f 776e 2079 6f75 7220 4461  ote down your Da
+00001fb0: 7461 6272 6963 6b73 2069 6e73 7461 6e63  tabricks instanc
+00001fc0: 6520 6672 6f6d 2074 6865 2062 726f 7773  e from the brows
+00001fd0: 6572 2055 524c 2c20 666f 726d 6174 7465  er URL, formatte
+00001fe0: 6420 6c69 6b65 2060 6874 7470 733a 2f2f  d like `https://
+00001ff0: 3c44 4154 4142 5249 434b 532d 494e 5354  <DATABRICKS-INST
+00002000: 414e 4345 3e2e 636c 6f75 642e 6461 7461  ANCE>.cloud.data
+00002010: 6272 6963 6b73 2e63 6f6d 2f60 0a36 2e20  bricks.com/`.6. 
+00002020: 4372 6561 7465 2061 2073 686f 7274 2073  Create a short s
+00002030: 6372 6970 742c 2072 6570 6c61 6369 6e67  cript, replacing
+00002040: 2074 6865 2070 6c61 6365 686f 6c64 6572   the placeholder
+00002050: 732e 0a0a 6060 6070 7974 686f 6e0a 6672  s...```python.fr
+00002060: 6f6d 2070 7265 6665 6374 5f64 6174 6162  om prefect_datab
+00002070: 7269 636b 7320 696d 706f 7274 2044 6174  ricks import Dat
+00002080: 6162 7269 636b 7343 7265 6465 6e74 6961  abricksCredentia
+00002090: 6c73 0a0a 6372 6564 656e 7469 616c 7320  ls..credentials 
+000020a0: 3d20 4461 7461 6272 6963 6b73 4372 6564  = DatabricksCred
+000020b0: 656e 7469 616c 7328 0a20 2020 2064 6174  entials(.    dat
+000020c0: 6162 7269 636b 735f 696e 7374 616e 6365  abricks_instance
+000020d0: 3d22 4441 5441 4252 4943 4b53 2d49 4e53  ="DATABRICKS-INS
+000020e0: 5441 4e43 452d 504c 4143 4548 4f4c 4445  TANCE-PLACEHOLDE
+000020f0: 5222 0a20 2020 2074 6f6b 656e 3d22 544f  R".    token="TO
+00002100: 4b45 4e2d 504c 4143 4548 4f4c 4445 5222  KEN-PLACEHOLDER"
+00002110: 0a29 0a0a 636f 6e6e 6563 746f 722e 7361  .)..connector.sa
+00002120: 7665 2822 424c 4f43 4b5f 4e41 4d45 2d50  ve("BLOCK_NAME-P
+00002130: 4c41 4345 484f 4c44 4552 2229 0a60 6060  LACEHOLDER").```
+00002140: 0a0a 436f 6e67 7261 7473 2120 596f 7520  ..Congrats! You 
+00002150: 6361 6e20 6e6f 7720 6561 7369 6c79 206c  can now easily l
+00002160: 6f61 6420 7468 6520 7361 7665 6420 626c  oad the saved bl
+00002170: 6f63 6b2c 2077 6869 6368 2068 6f6c 6473  ock, which holds
+00002180: 2079 6f75 7220 6372 6564 656e 7469 616c   your credential
+00002190: 733a 0a0a 6060 6070 7974 686f 6e0a 6672  s:..```python.fr
+000021a0: 6f6d 2070 7265 6665 6374 5f64 6174 6162  om prefect_datab
+000021b0: 7269 636b 7320 696d 706f 7274 2044 6174  ricks import Dat
+000021c0: 6162 7269 636b 7343 7265 6465 6e74 6961  abricksCredentia
+000021d0: 6c73 0a0a 4461 7461 6272 6963 6b73 4372  ls..DatabricksCr
+000021e0: 6564 656e 7469 616c 732e 6c6f 6164 2822  edentials.load("
+000021f0: 424c 4f43 4b5f 4e41 4d45 2d50 4c41 4345  BLOCK_NAME-PLACE
+00002200: 484f 4c44 4552 2229 0a60 6060 0a0a 2121  HOLDER").```..!!
+00002210: 2120 696e 666f 2022 5265 6769 7374 6572  ! info "Register
+00002220: 696e 6720 626c 6f63 6b73 220a 0a20 2020  ing blocks"..   
+00002230: 2052 6567 6973 7465 7220 626c 6f63 6b73   Register blocks
+00002240: 2069 6e20 7468 6973 206d 6f64 756c 6520   in this module 
+00002250: 746f 0a20 2020 205b 7669 6577 2061 6e64  to.    [view and
+00002260: 2065 6469 7420 7468 656d 5d28 6874 7470   edit them](http
+00002270: 733a 2f2f 6f72 696f 6e2d 646f 6373 2e70  s://orion-docs.p
+00002280: 7265 6665 6374 2e69 6f2f 7569 2f62 6c6f  refect.io/ui/blo
+00002290: 636b 732f 290a 2020 2020 6f6e 2050 7265  cks/).    on Pre
+000022a0: 6665 6374 2043 6c6f 7564 3a0a 0a20 2020  fect Cloud:..   
+000022b0: 2060 6060 6261 7368 0a20 2020 2070 7265   ```bash.    pre
+000022c0: 6665 6374 2062 6c6f 636b 2072 6567 6973  fect block regis
+000022d0: 7465 7220 2d6d 2070 7265 6665 6374 5f64  ter -m prefect_d
+000022e0: 6174 6162 7269 636b 730a 2020 2020 6060  atabricks.    ``
+000022f0: 600a 0a23 2323 2046 6565 6462 6163 6b0a  `..### Feedback.
+00002300: 0a49 6620 796f 7520 656e 636f 756e 7465  .If you encounte
+00002310: 7220 616e 7920 6275 6773 2077 6869 6c65  r any bugs while
+00002320: 2075 7369 6e67 2060 7072 6566 6563 742d   using `prefect-
+00002330: 6461 7461 6272 6963 6b73 602c 2066 6565  databricks`, fee
+00002340: 6c20 6672 6565 2074 6f20 6f70 656e 2061  l free to open a
+00002350: 6e20 6973 7375 6520 696e 2074 6865 205b  n issue in the [
+00002360: 7072 6566 6563 742d 6461 7461 6272 6963  prefect-databric
+00002370: 6b73 5d28 6874 7470 733a 2f2f 6769 7468  ks](https://gith
+00002380: 7562 2e63 6f6d 2f50 7265 6665 6374 4851  ub.com/PrefectHQ
+00002390: 2f70 7265 6665 6374 2d64 6174 6162 7269  /prefect-databri
+000023a0: 636b 7329 2072 6570 6f73 6974 6f72 792e  cks) repository.
+000023b0: 0a0a 4966 2079 6f75 2068 6176 6520 616e  ..If you have an
+000023c0: 7920 7175 6573 7469 6f6e 7320 6f72 2069  y questions or i
+000023d0: 7373 7565 7320 7768 696c 6520 7573 696e  ssues while usin
+000023e0: 6720 6070 7265 6665 6374 2d64 6174 6162  g `prefect-datab
+000023f0: 7269 636b 7360 2c20 796f 7520 6361 6e20  ricks`, you can 
+00002400: 6669 6e64 2068 656c 7020 696e 2065 6974  find help in eit
+00002410: 6865 7220 7468 6520 5b50 7265 6665 6374  her the [Prefect
+00002420: 2044 6973 636f 7572 7365 2066 6f72 756d   Discourse forum
+00002430: 5d28 6874 7470 733a 2f2f 6469 7363 6f75  ](https://discou
+00002440: 7273 652e 7072 6566 6563 742e 696f 2f29  rse.prefect.io/)
+00002450: 206f 7220 7468 6520 5b50 7265 6665 6374   or the [Prefect
+00002460: 2053 6c61 636b 2063 6f6d 6d75 6e69 7479   Slack community
+00002470: 5d28 6874 7470 733a 2f2f 7072 6566 6563  ](https://prefec
+00002480: 742e 696f 2f73 6c61 636b 292e 0a0a 4665  t.io/slack)...Fe
+00002490: 656c 2066 7265 6520 746f 2073 7461 7220  el free to star 
+000024a0: 6f72 2077 6174 6368 205b 6070 7265 6665  or watch [`prefe
+000024b0: 6374 2d64 6174 6162 7269 636b 7360 5d28  ct-databricks`](
+000024c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000024d0: 6f6d 2f50 7265 6665 6374 4851 2f70 7265  om/PrefectHQ/pre
+000024e0: 6665 6374 2d64 6174 6162 7269 636b 7329  fect-databricks)
+000024f0: 2066 6f72 2075 7064 6174 6573 2074 6f6f   for updates too
+00002500: 210a 0a23 2323 2043 6f6e 7472 6962 7574  !..### Contribut
+00002510: 696e 670a 0a49 6620 796f 7527 6420 6c69  ing..If you'd li
+00002520: 6b65 2074 6f20 6865 6c70 2063 6f6e 7472  ke to help contr
+00002530: 6962 7574 6520 746f 2066 6978 2061 6e20  ibute to fix an 
+00002540: 6973 7375 6520 6f72 2061 6464 2061 2066  issue or add a f
+00002550: 6561 7475 7265 2074 6f20 6070 7265 6665  eature to `prefe
+00002560: 6374 2d64 6174 6162 7269 636b 7360 2c20  ct-databricks`, 
+00002570: 706c 6561 7365 205b 7072 6f70 6f73 6520  please [propose 
+00002580: 6368 616e 6765 7320 7468 726f 7567 6820  changes through 
+00002590: 6120 7075 6c6c 2072 6571 7565 7374 2066  a pull request f
+000025a0: 726f 6d20 6120 666f 726b 206f 6620 7468  rom a fork of th
+000025b0: 6520 7265 706f 7369 746f 7279 5d28 6874  e repository](ht
+000025c0: 7470 733a 2f2f 646f 6373 2e67 6974 6875  tps://docs.githu
+000025d0: 622e 636f 6d2f 656e 2f70 756c 6c2d 7265  b.com/en/pull-re
+000025e0: 7175 6573 7473 2f63 6f6c 6c61 626f 7261  quests/collabora
+000025f0: 7469 6e67 2d77 6974 682d 7075 6c6c 2d72  ting-with-pull-r
+00002600: 6571 7565 7374 732f 7072 6f70 6f73 696e  equests/proposin
+00002610: 672d 6368 616e 6765 732d 746f 2d79 6f75  g-changes-to-you
+00002620: 722d 776f 726b 2d77 6974 682d 7075 6c6c  r-work-with-pull
+00002630: 2d72 6571 7565 7374 732f 6372 6561 7469  -requests/creati
+00002640: 6e67 2d61 2d70 756c 6c2d 7265 7175 6573  ng-a-pull-reques
+00002650: 742d 6672 6f6d 2d61 2d66 6f72 6b29 2e0a  t-from-a-fork)..
+00002660: 0a48 6572 6520 6172 6520 7468 6520 7374  .Here are the st
+00002670: 6570 733a 0a0a 312e 205b 466f 726b 2074  eps:..1. [Fork t
+00002680: 6865 2072 6570 6f73 6974 6f72 795d 2868  he repository](h
+00002690: 7474 7073 3a2f 2f64 6f63 732e 6769 7468  ttps://docs.gith
+000026a0: 7562 2e63 6f6d 2f65 6e2f 6765 742d 7374  ub.com/en/get-st
+000026b0: 6172 7465 642f 7175 6963 6b73 7461 7274  arted/quickstart
+000026c0: 2f66 6f72 6b2d 612d 7265 706f 2366 6f72  /fork-a-repo#for
+000026d0: 6b69 6e67 2d61 2d72 6570 6f73 6974 6f72  king-a-repositor
+000026e0: 7929 0a32 2e20 5b43 6c6f 6e65 2074 6865  y).2. [Clone the
+000026f0: 2066 6f72 6b65 6420 7265 706f 7369 746f   forked reposito
+00002700: 7279 5d28 6874 7470 733a 2f2f 646f 6373  ry](https://docs
+00002710: 2e67 6974 6875 622e 636f 6d2f 656e 2f67  .github.com/en/g
+00002720: 6574 2d73 7461 7274 6564 2f71 7569 636b  et-started/quick
+00002730: 7374 6172 742f 666f 726b 2d61 2d72 6570  start/fork-a-rep
+00002740: 6f23 636c 6f6e 696e 672d 796f 7572 2d66  o#cloning-your-f
+00002750: 6f72 6b65 642d 7265 706f 7369 746f 7279  orked-repository
+00002760: 290a 332e 2049 6e73 7461 6c6c 2074 6865  ).3. Install the
+00002770: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
+00002780: 6974 7320 6465 7065 6e64 656e 6369 6573  its dependencies
+00002790: 3a0a 6060 600a 7069 7020 696e 7374 616c  :.```.pip instal
+000027a0: 6c20 2d65 2022 2e5b 6465 765d 220a 6060  l -e ".[dev]".``
+000027b0: 600a 342e 204d 616b 6520 6465 7369 7265  `.4. Make desire
+000027c0: 6420 6368 616e 6765 730a 352e 2041 6464  d changes.5. Add
+000027d0: 2074 6573 7473 0a36 2e20 496e 7365 7274   tests.6. Insert
+000027e0: 2061 6e20 656e 7472 7920 746f 205b 4348   an entry to [CH
+000027f0: 414e 4745 4c4f 472e 6d64 5d28 6874 7470  ANGELOG.md](http
+00002800: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f50  s://github.com/P
+00002810: 7265 6665 6374 4851 2f70 7265 6665 6374  refectHQ/prefect
+00002820: 2d64 6174 6162 7269 636b 732f 626c 6f62  -databricks/blob
+00002830: 2f6d 6169 6e2f 4348 414e 4745 4c4f 472e  /main/CHANGELOG.
+00002840: 6d64 290a 372e 2049 6e73 7461 6c6c 2060  md).7. Install `
+00002850: 7072 652d 636f 6d6d 6974 6020 746f 2070  pre-commit` to p
+00002860: 6572 666f 726d 2071 7561 6c69 7479 2063  erform quality c
+00002870: 6865 636b 7320 7072 696f 7220 746f 2063  hecks prior to c
+00002880: 6f6d 6d69 743a 0a60 6060 0a70 7265 2d63  ommit:.```.pre-c
+00002890: 6f6d 6d69 7420 696e 7374 616c 6c0a 6060  ommit install.``
+000028a0: 600a 382e 2060 6769 7420 636f 6d6d 6974  `.8. `git commit
+000028b0: 602c 2060 6769 7420 7075 7368 602c 2061  `, `git push`, a
+000028c0: 6e64 2063 7265 6174 6520 6120 7075 6c6c  nd create a pull
+000028d0: 2072 6571 7565 7374 0a                    request.
```

### Comparing `prefect-databricks-0.1.4/prefect_databricks.egg-info/SOURCES.txt` & `prefect-databricks-0.1.5/prefect_databricks.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,8 +17,14 @@
 prefect_databricks.egg-info/dependency_links.txt
 prefect_databricks.egg-info/entry_points.txt
 prefect_databricks.egg-info/requires.txt
 prefect_databricks.egg-info/top_level.txt
 prefect_databricks/models/__init__.py
 prefect_databricks/models/jobs.py
 scripts/__init__.py
-scripts/generate.py
+scripts/generate.py
+tests/test_block_standards.py
+tests/test_credentials.py
+tests/test_flows.py
+tests/test_generate.py
+tests/test_jobs.py
+tests/test_rest.py
```

### Comparing `prefect-databricks-0.1.4/scripts/generate.py` & `prefect-databricks-0.1.5/scripts/generate.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.4/setup.cfg` & `prefect-databricks-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.4/setup.py` & `prefect-databricks-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-databricks-0.1.4/versioneer.py` & `prefect-databricks-0.1.5/versioneer.py`

 * *Files identical despite different names*

