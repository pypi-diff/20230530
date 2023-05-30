# Comparing `tmp/thunno2-2.2.0.tar.gz` & `tmp/thunno2-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.2.0.tar", last modified: Sun May 14 14:37:49 2023, max compression
+gzip compressed data, was "thunno2-2.2.1.tar", last modified: Tue May 30 13:17:01 2023, max compression
```

## Comparing `thunno2-2.2.0.tar` & `thunno2-2.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-14 14:37:49.623927 thunno2-2.2.0/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-14 14:37:49.623806 thunno2-2.2.0/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-14 14:37:49.623962 thunno2-2.2.0/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.2.0/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-14 14:37:49.623095 thunno2-2.2.0/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.0/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.0/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.0/thunno2/canvas.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.0/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    55993 2023-05-13 16:16:20.000000 thunno2-2.2.0/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.2.0/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.0/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.2.0/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    56512 2023-05-13 16:16:20.000000 thunno2-2.2.0/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    33521 2023-05-14 14:36:33.000000 thunno2-2.2.0/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    26490 2023-05-14 14:36:33.000000 thunno2-2.2.0/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-05-01 08:52:47.000000 thunno2-2.2.0/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    81630 2023-05-13 16:16:20.000000 thunno2-2.2.0/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4526 2023-05-14 14:36:33.000000 thunno2-2.2.0/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-14 14:37:18.000000 thunno2-2.2.0/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-14 14:37:49.623637 thunno2-2.2.0/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      459 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-30 13:17:01.699792 thunno2-2.2.1/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-30 13:17:01.699669 thunno2-2.2.1/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-30 13:17:01.699831 thunno2-2.2.1/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.1/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-30 13:17:01.698978 thunno2-2.2.1/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.1/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.1/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.1/thunno2/canvas.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.1/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    56522 2023-05-30 13:11:50.000000 thunno2-2.2.1/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.1/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.1/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7253 2023-05-15 16:46:52.000000 thunno2-2.2.1/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    56820 2023-05-30 13:11:50.000000 thunno2-2.2.1/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    33860 2023-05-27 16:56:14.000000 thunno2-2.2.1/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    26658 2023-05-27 16:18:35.000000 thunno2-2.2.1/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-05-27 07:11:18.000000 thunno2-2.2.1/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    84691 2023-05-30 13:11:50.000000 thunno2-2.2.1/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4526 2023-05-14 14:36:33.000000 thunno2-2.2.1/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-30 13:12:03.000000 thunno2-2.2.1/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-30 13:17:01.699509 thunno2-2.2.1/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      459 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.2.0/PKG-INFO` & `thunno2-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.0
+Version: 2.2.1
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.0.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.1.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.2.0/setup.py` & `thunno2-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.0/thunno2/autoexplanation.py` & `thunno2-2.2.1/thunno2/autoexplanation.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.0/thunno2/canvas.py` & `thunno2-2.2.1/thunno2/canvas.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.0/thunno2/codepage.py` & `thunno2-2.2.1/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.0/thunno2/commands.py` & `thunno2-2.2.1/thunno2/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,29 +137,34 @@
 
     # Remove n items from the front
     def rmv(self, num, default=0):
         for _ in range(num):
             if list(self):
                 yield self.pop(0)
             else:
-                if ctx.other_il:
-                    x = ctx.other_il.pop(0)
-                    ctx.other_il.append(x)
-                    yield x
+                if (not ctx.vyxal_mode) or ctx.context is None:
+                    if ctx.other_il:
+                        x = ctx.other_il.pop(0)
+                        ctx.other_il.append(x)
+                        yield x
+                    else:
+                        yield default
                 else:
-                    yield default
+                    yield ctx.context
 
 
 class Context:
     def __init__(self):
         self.stack = Stack()
         self.og_input_list = []
         self.other_il = []
         self.implicit_print = True
         self.warnings = False
+        self.context = None
+        self.vyxal_mode = False
 
 
 ctx = Context()
 
 
 class VoidType:
     def __call__(self, *args, **kwds):
@@ -1417,21 +1422,21 @@
         },
         0,
         ("repeat",),
     ),
     "ṛ": Overload(
         2,
         {
-            (Number[0], Number[0]): cmp,
+            (Number[0], Number[0]): absolute_difference,
             (Number[0], str): zfill1,
             (str, Number[0]): zfill2,
             (str, str): surround,
         },
         2,
-        ("compare", "cmp", "zfill", "surround"),
+        ("absolute_difference", "zfill", "surround"),
     ),
     "ṣ": Overload(1, {Number: spaces, Iterable: suffixes}, 0, ("suffixes", "spaces")),
     "ṭ": Overload(3, {(Any[0], Any[0], Any[0]): triple_swap}, 0, ("triple_swap",)),
     "ẉ": Overload(
         2,
         {
             (Number[0], Number[0]): range_cartesian_power,
@@ -1563,21 +1568,25 @@
 random_digraphs_1 = {
     "C": Overload(1, {Any: cosine}, 1, ("cosine", "cos")),
     "D": Overload(1, {Any: degrees}, 1, ("degrees",)),
     "E": Overload(1, {Any: exponent}, 1, ("exponent",)),
     "F": Overload(1, {Any: nth_fibonacci_number}, 1, ("nth_fibonacci_number",)),
     "H": Overload(2, {(Any[0], Any[0]): hypotenuse}, 2, ("hypot", "hypotenuse")),
     "I": Overload(1, {Any: insignificant}, 1, ("insignificant",)),
+    "L": Overload(2, {(Any[0], Any[0]): logarithm}, 2, ("log", "logarithm")),
+    "N": Overload(1, {Any: ln}, 1, ("natural_log", "natural_logarithm")),
     "P": Overload(1, {Any: nth_prime}, 1, ("nth_prime",)),
     "R": Overload(1, {Any: radians}, 1, ("radians",)),
     "S": Overload(1, {Any: sine}, 1, ("sine", "sin")),
     "T": Overload(1, {Any: tangent}, 1, ("tangent", "tan")),
     "c": Overload(1, {Any: arc_cosine}, 1, ("arc_cosine", "arccos")),
+    "l": Overload(1, {Any: log10}, 1, ("log10", "common_log", "common_logarithm")),
     "s": Overload(1, {Any: arc_sine}, 1, ("arc_sine", "arcsin")),
     "t": Overload(1, {Any: arc_tangent}, 1, ("arc_tangent", "arctan")),
+    "ḷ": Overload(1, {Any: log2}, 1, ("log2", "log_base_2")),
     "&": Overload(2, {(Any[0], Any[0]): bitwise_and}, 2, ("bitwise_and",)),
     "|": Overload(2, {(Any[0], Any[0]): bitwise_or}, 2, ("bitwise_or",)),
     "^": Overload(2, {(Any[0], Any[0]): bitwise_xor}, 2, ("bitwise_xor",)),
     "~": Overload(1, {Any: bitwise_not}, 1, ("bitwise_not",)),
 }
 
 random_digraphs_2 = {
```

### Comparing `thunno2-2.2.0/thunno2/constants.py` & `thunno2-2.2.1/thunno2/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,18 @@
     "%": [1, 0],
     "&": [1, 1],
     "'": [1, -1],
     "(": [-1, 0],
     ")": [-1, 1],
     "*": [-1, -1],
     "+": [3, 5],
+    ",": "AEIOUaeiou",
+    "-": "aeiouAEIOU",
+    ".": "AEIOUYaeiouy",
+    "/": "aeiouyAEIOUY",
     "Ȧ": ascii_lowercase + ascii_uppercase + "0123456789",
     "Ḃ": "0123456789" + ascii_uppercase + ascii_lowercase,
     "Ċ": ascii_lowercase + ascii_uppercase + "0123456789_",
     "Ḋ": ascii_uppercase[::-1],
     "Ė": ascii_lowercase[::-1] + ascii_uppercase[::-1],
     "Ḟ": ascii_lowercase[::-1] + ascii_uppercase[::-1] + "9876543210_",
     "Ġ": ascii_uppercase + ascii_lowercase,
```

### Comparing `thunno2-2.2.0/thunno2/dictionary.py` & `thunno2-2.2.1/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.0/thunno2/flags.py` & `thunno2-2.2.1/thunno2/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         for inp in inputs:
             if isinstance(inp, (int, float)):
                 new_input.append(inp - flags.count("-"))
             else:
                 new_input.append(inp)
         inputs = new_input[:]
 
+    if "c" in flags:
+        commands.ctx.vyxal_mode = True
+
     return inputs
 
 
 def process_output_flags(flags, do_print=True):
     for flag in flags:
         if "J" == flag:
             commands.ctx.stack.push(helpers.empty_join(next(commands.ctx.stack.rmv(1))))
@@ -172,15 +175,15 @@
                 else:
                     new_inputs = [x]
             except:
                 new_inputs = [line]
             commands.ctx.og_input_list = new_inputs.copy()
             commands.ctx.other_il = new_inputs.copy()
             print(line, "--> ", end="")
-            interpreter.run(code, n=0, iteration_index=0)
+            interpreter.run(code, context=0, iteration_index=0)
             process_output_flags(new_flags)
         return None
 
     elif "C" in flags:
         new_flags = "".join(f for f in flags if f != "C")
         for l in inputs.splitlines():
             m = re.match(r"(.+) ?(?:=>|-+>) ?(.+)", l)
@@ -202,22 +205,22 @@
                     expected = output.strip()
             except Exception as e:
                 print(f"FAIL ❌ (Got error {e})")
                 continue
             commands.ctx.og_input_list = new_inputs.copy()
             commands.ctx.other_il = new_inputs.copy()
             print(line, "--> ", end="")
-            interpreter.run(code, n=0, iteration_index=0)
+            interpreter.run(code, context=0, iteration_index=0)
             process_output_flags(new_flags, False)
             actual_output = next(commands.ctx.stack.rmv(1))
             print(actual_output, end="\t")
             if actual_output == expected:
                 print("PASS ✅")
             else:
                 print(f"FAIL ❌ (Expected {expected})")
         return None
 
     inputs = process_input_flags(flags, inputs)
     commands.ctx.og_input_list = inputs.copy()
     commands.ctx.other_il = inputs.copy()
-    interpreter.run(code, n=0, iteration_index=0)
+    interpreter.run(code, context=0, iteration_index=0)
     process_output_flags(flags)
```

### Comparing `thunno2-2.2.0/thunno2/helpers.py` & `thunno2-2.2.1/thunno2/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -3040,7 +3040,31 @@
     return multidimensional_index(x, l)
 
 
 def vectorised_multidimensional_index(x, l):
     if not isinstance(x, list):
         return multidimensional_index(x, l)
     return [*map(lambda i, y=l: vectorised_multidimensional_index(i, y), x)]
+
+
+def absolute_difference(a, b):
+    return abs(b - a)
+
+
+@try_float_conversion
+def logarithm(a, b):
+    return math.log(b, a)
+
+
+@try_float_conversion
+def log10(a):
+    return math.log10(a)
+
+
+@try_float_conversion
+def ln(a):
+    return math.log(a)
+
+
+@try_float_conversion
+def log2(a):
+    return math.log2(a)
```

### Comparing `thunno2-2.2.0/thunno2/interpreter.py` & `thunno2-2.2.1/thunno2/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,20 @@
     "y": 2,  # y defaults to 2
     "ga": [],  # global array defaults to []
 }
 
 """RUN FUNCTION"""
 
 
-def run(code, *, n, iteration_index):
+def run(code, *, context=None, iteration_index=None):
+    if context is None:
+        n = 0
+    else:
+        n = context
+    ctx.context = context
     # while ctx.index < len(code):
     for chars, desc, info in code:
         if desc == "command" or desc == "digraph":
             if info != Void:
                 values = info()
                 for value in values:
                     ctx.stack.push(value)
@@ -468,52 +473,52 @@
         elif desc == "map":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
-                run(info, n=j, iteration_index=i)
+                run(info, context=j, iteration_index=i)
                 r.append(next(ctx.stack.rmv(1)))
             ctx.stack.push(r)
         elif desc == "filter":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
-                run(info, n=j, iteration_index=i)
+                run(info, context=j, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 if z:
                     r.append(j)
             ctx.stack.push(r)
         elif desc == "sort by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
-                run(info, n=j, iteration_index=i)
+                run(info, context=j, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 r.append((j, z))
             try:
                 sorted_list = sorted(r, key=lambda t: t[-1])
                 ctx.stack.push([p for p, q in sorted_list])
             except:
                 ctx.stack.push(x)
         elif desc == "group by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
-                run(info, n=j, iteration_index=i)
+                run(info, context=j, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 r.append((j, z))
             try:
                 d = []
                 for val, key in r:
                     for k, (i, j) in enumerate(d):
                         if key == i:
@@ -526,17 +531,16 @@
                 ctx.stack.push(x)
         elif desc == "fixed point":
             r = [Void]
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             i = 0
             while True:
                 ctx.stack = Stack(copy.deepcopy(old_stack))
-                run(info, n=r[-1], iteration_index=i)
+                run(info, context=r[-1], iteration_index=i)
                 k = (ctx.stack + ctx.other_il + [0])[0]
-                print(k)
                 r.append(k)
                 if r[-1] == r[-2]:
                     break
                 i += 1
             ctx.stack.push(r[1:])
         elif desc == "first n integers":
             a = next(ctx.stack.rmv(1))
@@ -546,15 +550,15 @@
                 x = 1
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             i = 1
             r = []
             while len(r) < x:
                 ctx.stack = Stack(copy.deepcopy(old_stack))
                 ctx.stack.push(i)
-                run(info, n=i, iteration_index=i - 1)
+                run(info, context=i, iteration_index=i - 1)
                 k = next(ctx.stack.rmv(1))
                 if k:
                     r.append(i)
                 i += 1
             ctx.stack.push(r)
         elif desc == "cumulative reduce by":
             a = next(ctx.stack.rmv(1))
@@ -562,15 +566,15 @@
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             if x:
                 r = [x.pop(0)]
                 for i, j in enumerate(x):
                     ctx.stack = Stack(copy.deepcopy(old_stack))
                     ctx.stack.push(r[-1])
                     ctx.stack.push(j)
-                    run(info, n=j, iteration_index=i)
+                    run(info, context=j, iteration_index=i)
                     r.append(next(ctx.stack.rmv(1)))
                 ctx.stack.push(r)
             else:
                 ctx.stack.push([])
         elif desc == "single function reduce by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
@@ -628,45 +632,50 @@
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             if x:
                 r = [x.pop(0)]
                 for i, j in enumerate(x):
                     ctx.stack = Stack(copy.deepcopy(old_stack))
                     ctx.stack.push(r[-1])
                     ctx.stack.push(j)
-                    run(info, n=j, iteration_index=i)
+                    run(info, context=j, iteration_index=i)
                     r.append(next(ctx.stack.rmv(1)))
                 ctx.stack.push(r[-1])
             else:
                 ctx.stack.push([])
         elif desc == "for loop":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             for i, j in enumerate(x):
                 if not isinstance(a, (int, float)):
                     ctx.stack.push(j)
-                run(info, n=j, iteration_index=i)
+                run(info, context=j, iteration_index=i)
         elif desc == "while loop":
             cond, body = info
             i = 0
             while True:
                 old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
-                run(cond, n=0, iteration_index=i)
+                run(cond, context=0, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 ctx.stack = Stack(copy.deepcopy(old_stack))
                 if not z:
                     break
-                run(body, n=0, iteration_index=i)
+                run(body, context=0, iteration_index=i)
+                i += 1
+        elif desc == "forever loop":
+            i = 0
+            while True:
+                run(info, context=0, iteration_index=i)
                 i += 1
         elif desc == "if statement":
             if_true, if_false = info
             a = next(ctx.stack.rmv(1))
             if a:
-                run(if_true, n=0, iteration_index=1)
+                run(if_true, context=0, iteration_index=1)
             else:
-                run(if_false, n=0, iteration_index=0)
+                run(if_false, context=0, iteration_index=0)
         elif desc == "execute without popping":
             if info != Void:
                 values = info(pop=False)
                 for value in values:
                     ctx.stack.push(value)
         elif desc == "pair apply":
             a = next(ctx.stack.rmv(1))
@@ -708,15 +717,15 @@
                 print(i)
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             k = 0
             while True:
                 ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
                 for j in x:
                     ctx.stack.push(j)
-                run(info, n=([0] + x)[-1], iteration_index=k)
+                run(info, context=([0] + x)[-1], iteration_index=k)
                 y = next(ctx.stack.rmv(1))
                 print(y)
                 x.append(y)
                 k += 1
         elif desc == "apply to every nth item":
             a = next(ctx.stack.rmv(1))
             try:
@@ -747,15 +756,15 @@
         elif desc == "adjacent group by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
-                run(info, n=j, iteration_index=i)
+                run(info, context=j, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 r.append((j, z))
             try:
                 d = []
                 last = None
                 for val, key in r:
                     if key == last:
@@ -802,11 +811,11 @@
 
 def test(cod, inp=(), stk=(), warn=True):
     ctx.stack = Stack(stk)
     ctx.og_input_list = list(inp)
     ctx.other_il = list(inp)
     ctx.warnings = warn
     tokenised = tokenise(cod)[1]
-    run(tokenised, n=0, iteration_index=0)
+    run(tokenised, context=0, iteration_index=0)
     print(ctx.stack)
     if ctx.implicit_print:
         print(ctx.stack[0])
```

### Comparing `thunno2-2.2.0/thunno2/lexer.py` & `thunno2-2.2.1/thunno2/lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,14 +595,18 @@
             try:
                 if code[index] == ";":
                     i, r2 = tokenise(code[index + 1 :], expected_end=")")
                     index += i
             except:
                 pass
             ret.append((char, "while loop", (r1, r2)))
+        elif char == "⁽":
+            i, r = tokenise(code[index + 1 :], expected_end="⁾")
+            index += i
+            ret.append((char, "forever loop", r))
         elif char == "?":
             i, r1 = tokenise(code[index + 1 :], expected_end=":;")
             index += i + 1
             r2 = []
             try:
                 if code[index] == ":":
                     i, r2 = tokenise(code[index + 1 :], expected_end=";")
```

### Comparing `thunno2-2.2.0/thunno2/run.py` & `thunno2-2.2.1/thunno2/run.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from thunno2 import lexer, version, flags, tokens, autoexplanation
-import sys
+from thunno2 import lexer, version, flags, tokens, autoexplanation, codepage
+import sys, time
 
 
 def from_terminal():
     print("Thunno", version.THUNNO_VERSION, "interpreter\n")
     print("\nFlags:")
     flags_list = input()
     code = ""
@@ -24,45 +24,84 @@
         inp = input()
     inputs = ""
     print("\nInput:")
     inp = input()
     while inp:
         inputs += inp + "\n"
         inp = input()
-    if "e" in flags_list:
-        print("\nExplanation:\n\n" + autoexplanation.auto_explain(code) + "\n")
+    if "U" in flags_list:
+        code = codepage.utf8_to_thunno2(code)
+    if "." in "".join(flags_list):
+        start_time = time.time()
     if "v" in flags_list:
         transpiled = tokens.transpile(code)
         print("\nTranspiled:")
         print(transpiled)
         print()
         _, tokenised = lexer.tokenise(transpiled)
     else:
         _, tokenised = lexer.tokenise(code)
+    if "." in "".join(flags_list):
+        lexed_time = time.time()
+    if "e" in flags_list:
+        print(
+            "\nExplanation:\n\n"
+            + autoexplanation.auto_explain(tokenised, tkn=False)
+            + "\n"
+        )
     print("\nOutput:")
     flags.run(flags_list, tokenised, inputs)
+    if "." in "".join(flags_list):
+        end_time = time.time()
+        times = [
+            (lexed_time - start_time) * 1000,
+            (end_time - lexed_time) * 1000,
+            (end_time - start_time) * 1000,
+        ]
+        print("\nTimings:")
+        print(f"Lexer: {times[0]:.3f}ms")
+        print(f"Program: {times[1]:.3f}ms")
+        print(f"Total: {times[2]:.3f}ms\n")
 
 
 def from_cmdline():
     args = sys.argv[1:]
     if not args:
         from_terminal()
         return None
     filename = args[0]
     flags_list = args[1:]
     sys.stderr.write("Thunno, v" + version.THUNNO_VERSION + "\n")
     try:
         with open(filename) as f:
             code = f.read()
-            if "e" in "".join(flags_list):
-                sys.stderr.write(
-                    "\nExplanation:\n\n" + autoexplanation.auto_explain(code) + "\n"
-                )
+            if "U" in "".join(flags_list):
+                code = codepage.utf8_to_thunno2(code)
+            if "." in "".join(flags_list):
+                start_time = time.time()
             if "v" in "".join(flags_list):
                 transpiled = tokens.transpile(code)
                 print("Transpiled:", transpiled, file=sys.stderr)
                 _, tokenised = lexer.tokenise(transpiled)
             else:
                 _, tokenised = lexer.tokenise(code)
+            if "." in "".join(flags_list):
+                lexed_time = time.time()
+            if "e" in "".join(flags_list):
+                sys.stderr.write(
+                    "\nExplanation:\n\n"
+                    + autoexplanation.auto_explain(tokenised, tkn=False)
+                    + "\n"
+                )
             flags.run("".join(flags_list), tokenised, sys.stdin.read())
+            if "." in "".join(flags_list):
+                end_time = time.time()
+                times = [
+                    (lexed_time - start_time) * 1000,
+                    (end_time - lexed_time) * 1000,
+                    (end_time - start_time) * 1000,
+                ]
+                sys.stderr.write(
+                    f"\nTimings:\nLexer: {times[0]:.3f}ms\nProgram: {times[1]:.3f}ms\nTotal: {times[2]:.3f}ms\n"
+                )
     except Exception as E:
         sys.stderr.write("An error occurred: " + repr(E))
```

### Comparing `thunno2-2.2.0/thunno2/tests.py` & `thunno2-2.2.1/thunno2/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,20 +133,24 @@
     "øv",
     "øV",
     "ø^",
     "µr",
     "ÆC",
     "ÆD",
     "ÆE",
+    "ÆL",
+    "ÆN",
     "ÆR",
     "ÆS",
     "ÆT",
     "Æc",
+    "Æl",
     "Æs",
     "Æt",
+    "Æḷ",
 ]
 
 
 def call(cmd, *stk):
     ctx.stack = Stack(stk)
     ctx.warnings = True
     tested_commands.append(cmd)
@@ -2442,18 +2446,19 @@
 )
 
 assert_eq(call("ọ", ["xyz", 123], "abc"), ["xyz", 123, "xyz", 123, "xyz", 123])
 assert_eq(call("ọ", [123, 456], ["abc", "def"]), ["abc", "def", "abc", "def"])
 
 # ṛ
 
-assert_eq(call("ṛ", 5, 3), -1)
-assert_eq(call("ṛ", 3, 5), 1)
+assert_eq(call("ṛ", 5, 3), 2)
+assert_eq(call("ṛ", 3, 5), 2)
 assert_eq(
-    call("ṛ", 10, [-10, -5, 0, 5, 10, 15, 20, 25, 30]), [-1, -1, -1, -1, 0, 1, 1, 1, 1]
+    call("ṛ", 10, [-10, -5, 0, 5, 10, 15, 20, 25, 30]),
+    [20, 15, 10, 5, 0, 5, 10, 15, 20],
 )
 
 assert_eq(call("ṛ", 8, "abcde"), "000abcde")
 assert_eq(call("ṛ", "abcde", 3), "abcde")
 assert_eq(
     call("ṛ", "xyz", [-10, -5, 0, 5, 10]),
     ["xyz0000000", "xyz00", "xyz", "00xyz", "0000000xyz"],
@@ -2932,14 +2937,48 @@
 
 assert_eq(
     call("ÆI", [-2, -1.5, -1, -0.5, 0, 0.5, 1, 1.5, 2]), [0, 0, 1, 1, 1, 1, 1, 0, 0]
 )
 
 assert_eq(call("ÆI", "abc"), ["abc"])
 
+# # ÆL
+#
+# assert_eq(call("ÆL", 3, 30), 3.0959032742893844)
+# assert_eq(call("ÆL", 10, 50), 1.6989700043360185)
+# assert_eq(
+#     call("ÆL", 2.5, [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]),
+#     [0.0, 0.75647079736603, 1.19897784671579, 1.51294159473206, 1.7564707973660298,
+#      1.95544864408182, 2.1236820163783645, 2.26941239209809, 2.39795569343158, 2.51294159473206]
+# )
+#
+# assert_eq(call("ÆL", "abc", "def"), ["abc", "def"])
+
+# # ÆN
+#
+# assert_eq(call("ÆN", 0.1), -2.3025850929940455)
+# assert_eq(call("ÆN", 0.25), -1.3862943611198906)
+# assert_eq(call("ÆN", 0.5), -0.6931471805599453)
+# assert_eq(call("ÆN", 0.75), -0.2876820724517809)
+# assert_eq(call("ÆN", 0.9), -0.10536051565782628)
+# assert_eq(call("ÆN", 1.0), 0.0)
+# assert_eq(call("ÆN", 1.3), 0.26236426446749106)
+#
+# assert_eq(call("ÆN", 2), 0.6931471805599453)
+# assert_eq(call("ÆN", 2.718281828459045), 1.0)
+# assert_eq(call("ÆN", 3.141592653589793), 1.1447298858494002)
+# assert_eq(call("ÆN", 4), 1.3862943611198906)
+# assert_eq(call("ÆN", 5), 1.6094379124341003)
+# assert_eq(call("ÆN", 7), 1.9459101490553132)
+#
+# assert_eq(call("ÆN", 10), 2.302585092994046)
+# assert_eq(call("ÆN", 53), 3.970291913552122)
+# assert_eq(call("ÆN", 54.59815003314423), 4.0)
+# assert_eq(call("ÆN", 99), 4.59511985013459)
+
 # ÆP
 
 assert_eq(call("ÆP", 0), 2)
 assert_eq(call("ÆP", 5), 13)
 assert_eq(call("ÆP", 1.23), 3)
 assert_eq(call("ÆP", [10, 11, 12, 13, 14]), [31, 37, 41, 43, 47])
 
@@ -2962,14 +3001,36 @@
 #
 # assert_eq(call("Æc", 0), 1.5707963267948966)  # ~ pi/2
 # assert_eq(call("Æc", 0.5), 1.0471975511965976)  # ~ pi/3
 # assert_eq(call("Æc", 0.707), 0.7855491633997437)  # ~ pi/4
 # assert_eq(call("Æc", 0.866), 0.5236495809318289)  # ~ pi/6
 # assert_eq(call("Æc", 1), 0.0)  # ~ 0
 
+# # Æl
+#
+# assert_eq(call("Æl", 0.1), -1.0)
+# assert_eq(call("Æl", 0.25), -0.6020599913279624)
+# assert_eq(call("Æl", 0.5), -0.3010299956639812)
+# assert_eq(call("Æl", 0.75), -0.12493873660829995)
+# assert_eq(call("Æl", 0.9), -0.045757490560675115)
+# assert_eq(call("Æl", 1.0), 0.0)
+# assert_eq(call("Æl", 1.3), 0.11394335230683679)
+#
+# assert_eq(call("Æl", 2), 0.3010299956639812)
+# assert_eq(call("Æl", 2.718281828459045), 0.4342944819032518)
+# assert_eq(call("Æl", 3.141592653589793), 0.49714987269413385)
+# assert_eq(call("Æl", 4), 0.6020599913279624)
+# assert_eq(call("Æl", 5), 0.6989700043360189)
+# assert_eq(call("Æl", 7), 0.8450980400142568)
+#
+# assert_eq(call("Æl", 10), 1.0)
+# assert_eq(call("Æl", 53), 1.724275869600789)
+# assert_eq(call("Æl", 54.59815003314423), 1.7371779276130073)
+# assert_eq(call("Æl", 99), 1.99563519459755)
+
 # # Æs
 #
 # assert_eq(call("Æs", 0), 0.0)  # ~ 0
 # assert_eq(call("Æs", 0.5), 0.5235987755982988)  # ~ pi/6
 # assert_eq(call("Æs", 0.707), 0.785247163395153)  # ~ pi/4
 # assert_eq(call("Æs", 0.866), 1.0471467458630677)  # ~ pi/3
 # assert_eq(call("Æs", 1), 1.5707963267948966)  # ~ pi/2
@@ -2977,14 +3038,36 @@
 # # Æt
 #
 # assert_eq(call("Æt", 0), 0.0)  # ~ 0
 # assert_eq(call("Æt", 0.577), 0.5233360338618205)  # ~ pi/6
 # assert_eq(call("Æt", 1), 0.7853981633974483)  # ~ pi/4
 # assert_eq(call("Æt", 1.732), 1.0471848490249274)  # ~ pi/3
 
+# # Æḷ
+#
+# assert_eq(call("Æḷ", 0.1), -3.321928094887362)
+# assert_eq(call("Æḷ", 0.25), -2.0)
+# assert_eq(call("Æḷ", 0.5), -1.0)
+# assert_eq(call("Æḷ", 0.75), -0.4150374992788438)
+# assert_eq(call("Æḷ", 0.9), -0.15200309344504995)
+# assert_eq(call("Æḷ", 1.0), 0.0)
+# assert_eq(call("Æḷ", 1.3), 0.37851162325372983)
+#
+# assert_eq(call("Æḷ", 2), 1.0)
+# assert_eq(call("Æḷ", 2.718281828459045), 1.4426950408889634)
+# assert_eq(call("Æḷ", 3.141592653589793), 1.6514961294723187)
+# assert_eq(call("Æḷ", 4), 2.0)
+# assert_eq(call("Æḷ", 5), 2.321928094887362)
+# assert_eq(call("Æḷ", 7), 2.807354922057604)
+#
+# assert_eq(call("Æḷ", 10), 3.321928094887362)
+# assert_eq(call("Æḷ", 53), 5.727920454563199)
+# assert_eq(call("Æḷ", 54.59815003314423), 5.7707801635558535)
+# assert_eq(call("Æḷ", 99), 6.6293566200796095)
+
 # Æ&
 
 assert_eq(call("Æ&", 123, 456), 72)
 assert_eq(call("Æ&", -12.34, 56.78), 48)
 
 assert_eq(
     call("Æ&", 100, [0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100]),
```

### Comparing `thunno2-2.2.0/thunno2/tokens.py` & `thunno2-2.2.1/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.0/thunno2.egg-info/PKG-INFO` & `thunno2-2.2.1/thunno2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.0
+Version: 2.2.1
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.0.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.1.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

