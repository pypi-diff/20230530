# Comparing `tmp/dojo_truant-2023.4.7.3.tar.gz` & `tmp/dojo_truant-2023.5.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_truant-2023.4.7.3.tar", last modified: Fri Apr  7 23:54:27 2023, max compression
+gzip compressed data, was "dojo_truant-2023.5.30.0.tar", last modified: Tue May 30 17:41:22 2023, max compression
```

## Comparing `dojo_truant-2023.4.7.3.tar` & `dojo_truant-2023.5.30.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:54:27.064855 dojo_truant-2023.4.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-07 23:54:27.064855 dojo_truant-2023.4.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:54:27.064855 dojo_truant-2023.4.7.3/dojo/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/dojo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/dojo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/dojo/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/dojo/dojo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/dojo/engagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/dojo/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/dojo/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/dojo/write_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:54:27.064855 dojo_truant-2023.4.7.3/dojo_truant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-07 23:54:27.000000 dojo_truant-2023.4.7.3/dojo_truant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-07 23:54:27.000000 dojo_truant-2023.4.7.3/dojo_truant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:54:27.000000 dojo_truant-2023.4.7.3/dojo_truant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 23:54:27.000000 dojo_truant-2023.4.7.3/dojo_truant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 23:54:27.000000 dojo_truant-2023.4.7.3/dojo_truant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-07 23:54:10.000000 dojo_truant-2023.4.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:54:27.064855 dojo_truant-2023.4.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:41:22.795643 dojo_truant-2023.5.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 17:41:22.795643 dojo_truant-2023.5.30.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:41:22.791643 dojo_truant-2023.5.30.0/dojo/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/development_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/dojo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/engagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/stub_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/dojo/write_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:41:22.795643 dojo_truant-2023.5.30.0/dojo_truant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 17:41:22.000000 dojo_truant-2023.5.30.0/dojo_truant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 17:41:22.000000 dojo_truant-2023.5.30.0/dojo_truant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:41:22.000000 dojo_truant-2023.5.30.0/dojo_truant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 17:41:22.000000 dojo_truant-2023.5.30.0/dojo_truant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 17:41:22.000000 dojo_truant-2023.5.30.0/dojo_truant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-30 17:41:06.000000 dojo_truant-2023.5.30.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 17:41:22.795643 dojo_truant-2023.5.30.0/setup.cfg
```

### Comparing `dojo_truant-2023.4.7.3/LICENSE.txt` & `dojo_truant-2023.5.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.4.7.3/PKG-INFO` & `dojo_truant-2023.5.30.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dojo_truant
-Version: 2023.4.7.3
+Version: 2023.5.30.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dojo_truant
 
 Potentially to be published but just enough of a python defect dojo client to get me where I need to go. It's truant
 because it's expected that there's features in defect dojo that I will likely not fully support.
```

### Comparing `dojo_truant-2023.4.7.3/dojo/api.py` & `dojo_truant-2023.5.30.0/dojo/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class DAPI:
     _allowed_methods = ["GET", "OPTIONS", "HEAD", "POST", "PUT", "PATCH", "DELETE"]
     _endpoint = None
     _post_endpoint = None
     _type = "Unknown"
     _model_validation = {}
     _obj_iterate = None
-    _comp_ignore_keys = ["updated", "created", "prefetch"]
+    _comp_ignore_keys = ["updated", "created", "prefetch", "target_start", "target_end"]
 
     _id_column = "id"
 
     def __init__(self, **kwargs):
 
         self.logger = logging.getLogger("DAPI")
         self.endpoint = kwargs.get("endpoint", self._endpoint)
@@ -217,25 +217,29 @@
 
         create_validation = self.kwargs.get("model_validation", self._model_validation)
 
         valid = True
 
         for k, v in self.data.items():
             if k not in create_validation.keys():
-                self.logger.warning("Item {} not in validation definition".format(k))
+                self.logger.warning("Item {} not in validation definition for {}".format(k, self.type))
                 valid = False
                 break
             else:
                 if "type" in create_validation[k].keys():
-                    if isinstance(v, create_validation[k]["type"]) is False:
-                        self.logger.warning("Factor {} is of an incorrect type.".format(k))
-                        valid = False
-                        break
-                    else:
-                        pass
+                    try:
+                        if isinstance(v, create_validation[k]["type"]) is False:
+                            self.logger.warning("Factor {} is of an incorrect type {}.".format(k, type(v)))
+                            valid = False
+                            break
+                        else:
+                            pass
+                    except TypeError as te:
+                        self.logger.error("Type Test for {} on {} is incorrectly specified.".format(k, self.type))
+                        raise te
                 # Other future validation rules
 
         if enforce_all is True:
             extra_keys = [k for k in self.data.keys() if k not in create_validation.keys()]
             missing_keys = [k for k in create_validation.keys() if
                             k not in self.data.keys() and create_validation[k].get("required", True) is True]
```

### Comparing `dojo_truant-2023.4.7.3/dojo/dojo_group.py` & `dojo_truant-2023.5.30.0/dojo/dojo_group.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.4.7.3/dojo/engagement.py` & `dojo_truant-2023.5.30.0/dojo/engagement.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         "requester": {"type": int,
                       "required": False},
         "preset": {"type": int,
                    "required": False},
         "report_type": {"type": int,
                         "required": False},
         "product": {"type": (int, dojo.Product),
-                    "required": False},
+                    "required": True},
         "build_server": {"type": int,
                          "required": False},
         "source_code_management_server": {"type": int,
                                           "required": False},
         "orchestration_engine": {"type": int,
                                  "required": False}
     }
```

### Comparing `dojo_truant-2023.4.7.3/dojo/product.py` & `dojo_truant-2023.5.30.0/dojo/product.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.4.7.3/dojo/product_type.py` & `dojo_truant-2023.5.30.0/dojo/product_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.4.7.3/dojo/write_chain.py` & `dojo_truant-2023.5.30.0/dojo/write_chain.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 
     logger = logging.getLogger("expand_data")
 
     expanded_data = None
     expanded_template = dict()
 
     for tk, tv in template.items():
-        expanded_template["I{}".format(tk)] = tv.chain_repr()
+        if isinstance(tk, str) and tk.startswith("N"):
+            expanded_template[tk] = tv.chain_repr()
+        elif isinstance(tk, int):
+            expanded_template["I{}".format(tk)] = tv.chain_repr()
+        else:
+            pass
+            #  Something else is happening here
 
     if isinstance(data, dict):
         expanded_data = dict()
         for k, v in data.items():
             if isinstance(v, (list, tuple)):
                 expanded_data[k] = [expand_data(vi, template) for vi in v]
             else:
@@ -75,14 +81,16 @@
                 "username": username,
                 "password": password}
 
     template_obj = None
     if chain is not None:
         template_obj = {}
         for x in range(0, len(chain)):
+
+            logger.debug("Processing : {}".format(chain[x]))
             # Search for Chain Item
             tdata = expand_data(chain[x]["data"], template_obj)
             sdata = expand_data(chain[x]["search_data"], template_obj)
 
             logger.info("TData: {}".format(tdata))
 
             dojo_obj = chain[x]["type"](
@@ -96,11 +104,13 @@
                 dojo_obj.new_obj()
             else:
                 # One Found Update Existing Object
                 logger.info("update obj: {}".format(json.dumps(tdata)))
                 dojo_obj.update_obj(tdata)
 
             template_obj[x] = dojo_obj
+            if chain.get("named", None) is not None:
+                template_obj["N{}".format(chain["named"])] = dojo_obj
     else:
         logger.warning("No Chain of Items Given")
 
     return template_obj
```

### Comparing `dojo_truant-2023.4.7.3/dojo_truant.egg-info/PKG-INFO` & `dojo_truant-2023.5.30.0/dojo_truant.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dojo-truant
-Version: 2023.4.7.3
+Version: 2023.5.30.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dojo_truant
 
 Potentially to be published but just enough of a python defect dojo client to get me where I need to go. It's truant
 because it's expected that there's features in defect dojo that I will likely not fully support.
```

### Comparing `dojo_truant-2023.4.7.3/pyproject.toml` & `dojo_truant-2023.5.30.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,21 +3,21 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dojo_truant"
-version = "2023.04.07.3"
+version = "2023.05.30.0"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@auditboard.com"},
 ]
 description = "A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 keywords = ["defectDojo"]
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "requests",
```

