# Comparing `tmp/wicked_expressions-0.6.1.tar.gz` & `tmp/wicked_expressions-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.6.1.tar", max compression
+gzip compressed data, was "wicked_expressions-0.6.2.tar", max compression
```

## Comparing `wicked_expressions-0.6.1.tar` & `wicked_expressions-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-05-25 20:58:54.292242 wicked_expressions-0.6.1/LICENSE
--rw-r--r--   0        0        0     2119 2023-05-25 20:58:54.292242 wicked_expressions-0.6.1/README.md
--rw-r--r--   0        0        0     1219 2023-05-25 21:00:52.877227 wicked_expressions-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      321 2023-05-25 21:00:52.853227 wicked_expressions-0.6.1/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      823 2023-05-25 20:58:54.300243 wicked_expressions-0.6.1/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     7975 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      305 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     1850 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      341 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8524 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0      375 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/rebindable.bolt
--rw-r--r--   0        0        0      596 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/safe_load.bolt
--rw-r--r--   0        0        0     3118 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1221 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     5253 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-05-25 20:58:54.304242 wicked_expressions-0.6.1/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-30 11:35:04.948978 wicked_expressions-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2119 2023-05-30 11:35:04.948978 wicked_expressions-0.6.2/README.md
+-rw-r--r--   0        0        0     1219 2023-05-30 11:36:41.251602 wicked_expressions-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-05-30 11:36:41.231601 wicked_expressions-0.6.2/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      709 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     9460 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      305 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     1850 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      341 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8436 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0      375 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/rebindable.bolt
+-rw-r--r--   0        0        0      596 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/safe_load.bolt
+-rw-r--r--   0        0        0     3118 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1221 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     5253 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-05-30 11:35:04.960978 wicked_expressions-0.6.2/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.6.2/PKG-INFO
```

### Comparing `wicked_expressions-0.6.1/LICENSE` & `wicked_expressions-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.1/README.md` & `wicked_expressions-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.1/pyproject.toml` & `wicked_expressions-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.6.1"
+version = "0.6.2"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.6.1/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.6.2/wicked_expressions/modules/api.bolt`

 * *Files 19% similar despite different names*

```diff
@@ -15,10 +15,8 @@
 Scoreboard = ctx.inject(internal_api.Scoreboard)
 Data = ctx.inject(internal_api.Data)
 
 this = Data.entity('@s')
 
 
 ExpressionComparison.monkeypatch(Scoreboard, Data, ScoreSource, DataSource)
-StoreExpressionValue.monkeypatch(ScoreSource, DataSource)
-GetExpressionValue.monkeypatch(ScoreSource, DataSource)
 # DataStash.monkeypatch(Scoreboard, Data)
```

### Comparing `wicked_expressions-0.6.1/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.6.2/wicked_expressions/modules/comparison.bolt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from contextlib import contextmanager
+from bolt_expressions import ExpressionNode
+from bolt import Runtime
 
 from ./utils import Rebindable, parse_holder
 from ./config import Config
 
 
+runtime = ctx.inject(Runtime)
+
+
 class ExpressionComparison(Rebindable):
+    last_bool_check = None
+    incr_index = 0
     _INVERTED_OPERATOR = {
         '==': '!=',
         '!=': '==',
         '<': '>=',
         '>': '<=',
         '<=': '>',
         '>=': '<'
@@ -16,90 +23,131 @@
 
     def __init__(self, arg_0, operator='==', arg_1=None, initialized=False, check_exists=False):
         self.arg_0 = arg_0
         self.operator = operator
         self.arg_1 = arg_1
         self.initialized = initialized
         self.check_exists = check_exists
+        self.temp_scoreboard = self.Scoreboard(Config.SCOREBOARD_ROOT)
+        self.temp_storage = self.Data.storage(Config.STORAGE_ROOT)
 
     @classmethod
     def monkeypatch(cls, Scoreboard, Data, ScoreSource, DataSource):
+        cls.Scoreboard = Scoreboard
+        cls.Data = Data
         cls.ScoreSource = ScoreSource
         cls.DataSource = DataSource
-        cls.temp_scoreboard = Scoreboard(Config.SCOREBOARD_ROOT)
-        cls.temp_storage = Data.storage(Config.STORAGE_ROOT)
+
+    @classmethod
+    def incr(cls):
+        tmp = cls.incr_index
+        cls.incr_index += 1
+        return tmp
+
+    @contextmanager
+    def autonest(self):
+        nest_path = ~/nested_{self.incr()}
+
+        with runtime.scope() as commands:
+            yield True
+        if not commands:
+            return
+        if score foo tmp matches 10:
+            if len(commands) == 1:
+                runtime.commands.append(commands[0])
+            else:
+                execute function nest_path:
+                    runtime.commands.extend(commands)
 
     @contextmanager
     def __branch__(self):
         score_count = 0
-        
+
         if isinstance(self.arg_0, self.ScoreSource):
             score_count += 1
         if isinstance(self.arg_1, self.ScoreSource):
             score_count += 1
         
+        if not isinstance(self.arg_1, ExpressionNode) and self.arg_1 in (True, False):
+            self.arg_1 = int(self.arg_1)
+
         # exists check
         if self.check_exists:
             if isinstance(self.arg_0, self.ScoreSource):
                 with self.compare_score_to_score(self.arg_0, self.arg_0):
-                    yield True
+                    with self.autonest():
+                        yield True
             elif isinstance(self.arg_0, self.DataSource):
                 with self.check_data_exists(self.arg_0):
-                    yield True
-        
+                    with self.autonest():
+                        yield True
+
         # pseudo bool check
         # Any :: None
         elif self.arg_1 is None:
             with self.check_boolean(self.arg_0):
-                yield True
-        
+                with self.autonest():
+                    yield True
+
         # ScoreSource :: ScoreSource
         elif score_count == 2:
             with self.compare_score_to_score(self.arg_0, self.arg_1):
-                yield True
+                with self.autonest():
+                    yield True
         
         # ScoreSource :: Any || Any :: ScoreSource
         elif score_count == 1:
             # Any = DataSource
             if isinstance(self.arg_0, self.DataSource) or isinstance(self.arg_1, self.DataSource):
                 with self.compare_any_to_any(self.arg_0, self.arg_1):
-                    yield True
+                    with self.autonest():
+                        yield True
             # Any = ScoreSource
             else:
                 with self.compare_score_to_constant(self.arg_0, self.arg_1):
-                    yield True
+                    with self.autonest():
+                        yield True
     
         # DataSource :: DataSource
         elif score_count == 0:
             if self.operator in ('==', '!='):
                 with self.compare_data_to_data(self.arg_0, self.arg_1):
-                    yield True
+                    with self.autonest():
+                        yield True
             else:
                 with self.compare_any_to_any(self.arg_0, self.arg_1):
-                    yield True
+                    with self.autonest():
+                        yield True
 
         self.initialized = True
 
     def __not__(self):
-        return ExpressionComparison(self.arg_0, self._INVERTED_OPERATOR[self.operator], self.arg_1, initialized=self.initialized, check_exists=self.check_exists)
+        return self.__class__(self.arg_0, self._INVERTED_OPERATOR[self.operator], self.arg_1, initialized=self.initialized, check_exists=self.check_exists)
 
     @contextmanager
     def check_boolean(self, arg_0):
         temp = self.temp_scoreboard['$temp']
 
-        if not self.initialized:
+        if self.last_bool_check != str(arg_0):       # hacky fix since initializing doesnt work here
             temp = arg_0
 
         if self.operator == '==':
             if score temp.holder temp.obj matches 1:
                 yield True
         elif self.operator == '!=':
             if score temp.holder temp.obj matches 0:
                 yield True
 
+        # self.last_bool_check = str(arg_0)
+        self._set_last_bool_check(str(arg_0))
+
+    @classmethod
+    def _set_last_bool_check(cls, value):
+        cls.last_bool_check = value
+
     @contextmanager
     def compare_score_to_constant(self, arg_0, arg_1):
         arg_0_holder = parse_holder(arg_0.holder)
 
         if self.operator == '==':
             if score arg_0_holder arg_0.obj matches arg_1:
                 yield True
```

### Comparing `wicked_expressions-0.6.1/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.6.2/wicked_expressions/modules/internal_api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.1/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.6.2/wicked_expressions/modules/raw_operations.bolt`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from contextlib import contextmanager
+import bolt_expressions.sources as sources
 from ./utils import Rebindable, parse_holder
 
 
 class StoreExpressionValue(Rebindable):
     @contextmanager
     def __call__(self, expression, mode='result', type='int', scale=1):
-        if isinstance(expression, self.ScoreSource):
+        if isinstance(expression, sources.ScoreSource):
             holder = parse_holder(expression.holder)
 
             if mode == 'result':
                 store result score holder expression.obj:
                     yield True
             elif mode == 'success':
                 store success score holder expression.obj:
                     yield True
 
-        elif isinstance(expression, self.DataSource):
+        elif isinstance(expression, sources.DataSource):
             if expression._type == 'storage':
                 if mode == 'result':
                     if type == 'byte':
                         store result storage expression._target expression._path byte scale:
                             yield True
                     elif type == 'double':
                         store result storage expression._target expression._path double scale:
@@ -132,25 +133,20 @@
                     elif type == 'long':
                         store success block expression._target expression._path long scale:
                             yield True
                     elif type == 'short':
                         store success block expression._target expression._path short scale:
                             yield True
 
-    @classmethod
-    def monkeypatch(cls, ScoreSource, DataSource):
-        cls.ScoreSource = ScoreSource
-        cls.DataSource = DataSource
-
 class GetExpressionValue(Rebindable):
     def __call__(self, expression, scale=1):
-        if isinstance(expression, self.ScoreSource):
+        if isinstance(expression, sources.ScoreSource):
             holder = parse_holder(expression.holder)
             scoreboard players get holder expression.obj
-        elif isinstance(expression, self.DataSource):
+        elif isinstance(expression, sources.DataSource):
             if expression._type == 'storage':
                 if scale is None:
                     data get storage expression._target expression._path
                 else:
                     data get storage expression._target expression._path scale
             elif expression._type == 'entity':
                 holder = parse_holder(expression._target)
```

### Comparing `wicked_expressions-0.6.1/wicked_expressions/modules/safe_load.bolt` & `wicked_expressions-0.6.2/wicked_expressions/modules/safe_load.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.1/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.6.2/wicked_expressions/modules/sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.1/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.6.2/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.1/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.6.2/wicked_expressions/modules/var.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.1/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.6.2/wicked_expressions/modules/var_sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.6.1/PKG-INFO` & `wicked_expressions-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.6.1
+Version: 0.6.2
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

