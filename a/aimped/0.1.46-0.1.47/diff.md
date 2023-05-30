# Comparing `tmp/aimped-0.1.46.tar.gz` & `tmp/aimped-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.46.tar", last modified: Mon May 29 19:52:10 2023, max compression
+gzip compressed data, was "aimped-0.1.47.tar", last modified: Tue May 30 20:04:54 2023, max compression
```

## Comparing `aimped-0.1.46.tar` & `aimped-0.1.47.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.273401 aimped-0.1.46/
--rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.46/LICENSE
--rw-rw-rw-   0        0        0     1791 2023-05-29 19:52:10.274401 aimped-0.1.46/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.46/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.231400 aimped-0.1.46/aimped/
--rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.46/aimped/__init__.py
--rw-rw-rw-   0        0        0    12442 2023-05-29 19:36:23.000000 aimped-0.1.46/aimped/io_tasks.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.241400 aimped-0.1.46/aimped/model/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/model/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/model/load.py
--rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/models.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.242396 aimped-0.1.46/aimped/nitro/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nitro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.260400 aimped-0.1.46/aimped/nlp/
--rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/assertion.py
--rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/chunker.py
--rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/deid.py
--rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/ner.py
--rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/ner_cls_report.py
--rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/pipeline.py
--rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/regex_parser.py
--rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.46/aimped/nlp/relation.py
--rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.46/aimped/nlp/relation_visualizer.py
--rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/tokenizer.py
--rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/tools.py
--rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.46/aimped/nlp/translation.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.272398 aimped-0.1.46/aimped/test/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/__init__.py
--rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_assertion.py
--rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_chunk_merger.py
--rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_deid_pipeline.py
--rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_ner_results.py
--rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_regex_parser.py
--rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_relation_pipeline.py
--rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_tokenizer.py
--rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_translation_pipeline.py
--rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/utils.py
--rw-rw-rw-   0        0        0      130 2023-05-29 19:50:28.000000 aimped-0.1.46/aimped/version.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.238400 aimped-0.1.46/aimped.egg-info/
--rw-rw-rw-   0        0        0     1791 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-29 19:52:10.275400 aimped-0.1.46/setup.cfg
--rw-rw-rw-   0        0        0     1176 2023-05-29 19:50:28.000000 aimped-0.1.46/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.274802 aimped-0.1.47/
+-rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.47/LICENSE
+-rw-rw-rw-   0        0        0     1778 2023-05-30 20:04:54.274802 aimped-0.1.47/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.47/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.214818 aimped-0.1.47/aimped/
+-rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.47/aimped/__init__.py
+-rw-rw-rw-   0        0        0    12497 2023-05-30 19:12:19.000000 aimped-0.1.47/aimped/io_tasks.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.227804 aimped-0.1.47/aimped/model/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/model/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/model/load.py
+-rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/models.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.229800 aimped-0.1.47/aimped/nitro/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nitro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.255803 aimped-0.1.47/aimped/nlp/
+-rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/assertion.py
+-rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/chunker.py
+-rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/deid.py
+-rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/ner.py
+-rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/ner_cls_report.py
+-rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/pipeline.py
+-rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/regex_parser.py
+-rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.47/aimped/nlp/relation.py
+-rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.47/aimped/nlp/relation_visualizer.py
+-rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/tokenizer.py
+-rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/nlp/tools.py
+-rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.47/aimped/nlp/translation.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.273805 aimped-0.1.47/aimped/test/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/test/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/test/test_assertion.py
+-rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/test/test_chunk_merger.py
+-rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/test/test_deid_pipeline.py
+-rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/test/test_ner_results.py
+-rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/test/test_regex_parser.py
+-rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/test/test_relation_pipeline.py
+-rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/test/test_tokenizer.py
+-rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/test/test_translation_pipeline.py
+-rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.47/aimped/utils.py
+-rw-rw-rw-   0        0        0      130 2023-05-30 20:02:39.000000 aimped-0.1.47/aimped/version.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.224799 aimped-0.1.47/aimped.egg-info/
+-rw-rw-rw-   0        0        0     1778 2023-05-30 20:04:54.000000 aimped-0.1.47/aimped.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-05-30 20:04:54.000000 aimped-0.1.47/aimped.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 20:04:54.000000 aimped-0.1.47/aimped.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-30 20:04:54.000000 aimped-0.1.47/aimped.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 20:04:54.000000 aimped-0.1.47/aimped.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-30 20:04:54.276805 aimped-0.1.47/setup.cfg
+-rw-rw-rw-   0        0        0     1163 2023-05-30 20:04:44.000000 aimped-0.1.47/setup.py
```

### Comparing `aimped-0.1.46/LICENSE` & `aimped-0.1.47/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/PKG-INFO` & `aimped-0.1.47/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.46
+Version: 0.1.47
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.ml-hub.nioyatechai.com/
+Home-page: https://dev.aimped.ai/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aimped-0.1.46/README.md` & `aimped-0.1.47/README.md`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/io_tasks.py` & `aimped-0.1.47/aimped/io_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Description: This file contains standart input and output (sio) keys for each task
 
 from enum import Enum
 import json
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Union
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Extra, Field
 
 data_types = [
     'data_json',
     'data_pdf',
     'data_image',
     'data_svg',
     'data_audio',
@@ -30,14 +30,16 @@
 
 ################ Task: Text Classification ################
 
 class TextClassificationInput(BaseModel):
     """Input data for text classification task"""
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for classification.",
                                                                        "This is another example text for classification."])
+    class Config:
+        extra = Extra.allow
 
 class TextClassificationOutput(BaseModel):
     """Output data for text classification task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
         default={"data_json": {"result": None}},
```

### Comparing `aimped-0.1.46/aimped/model/load.py` & `aimped-0.1.47/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/assertion.py` & `aimped-0.1.47/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/chunker.py` & `aimped-0.1.47/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/deid.py` & `aimped-0.1.47/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/ner.py` & `aimped-0.1.47/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/ner_cls_report.py` & `aimped-0.1.47/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/pipeline.py` & `aimped-0.1.47/aimped/nlp/pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/regex_parser.py` & `aimped-0.1.47/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/relation.py` & `aimped-0.1.47/aimped/nlp/relation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/relation_visualizer.py` & `aimped-0.1.47/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/tokenizer.py` & `aimped-0.1.47/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/tools.py` & `aimped-0.1.47/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/nlp/translation.py` & `aimped-0.1.47/aimped/nlp/translation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/test/test_assertion.py` & `aimped-0.1.47/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/test/test_chunk_merger.py` & `aimped-0.1.47/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/test/test_deid_pipeline.py` & `aimped-0.1.47/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/test/test_ner_results.py` & `aimped-0.1.47/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/test/test_regex_parser.py` & `aimped-0.1.47/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/test/test_relation_pipeline.py` & `aimped-0.1.47/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/test/test_tokenizer.py` & `aimped-0.1.47/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/test/test_translation_pipeline.py` & `aimped-0.1.47/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped/utils.py` & `aimped-0.1.47/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/aimped.egg-info/PKG-INFO` & `aimped-0.1.47/aimped.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.46
+Version: 0.1.47
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.ml-hub.nioyatechai.com/
+Home-page: https://dev.aimped.ai/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aimped-0.1.46/aimped.egg-info/SOURCES.txt` & `aimped-0.1.47/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimped-0.1.46/setup.py` & `aimped-0.1.47/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     author="Russell C.",
     author_email="russell@aimped.com",
     maintainer="aimped",
     maintainer_email="contact@aimped.com",
     description="Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
-    url="https://dev.ml-hub.nioyatechai.com/", 
+    url="https://dev.aimped.ai/", 
     
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
```

