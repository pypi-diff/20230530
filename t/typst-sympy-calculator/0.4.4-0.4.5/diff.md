# Comparing `tmp/typst_sympy_calculator-0.4.4-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 32125 bytes, number of entries: 14
+Zip file size: 32211 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat     7111 b- defN 23-May-30 15:03 DefaultTypstCalculator.py
 -rw-rw-rw-  2.0 fat     4242 b- defN 23-May-30 08:32 TypstCalculator.py
--rw-rw-rw-  2.0 fat     9751 b- defN 23-May-30 14:47 TypstCalculatorServer.py
+-rw-rw-rw-  2.0 fat     9984 b- defN 23-May-30 15:34 TypstCalculatorServer.py
 -rw-rw-rw-  2.0 fat    21073 b- defN 23-May-30 11:08 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
 -rw-rw-rw-  2.0 fat    17356 b- defN 23-May-30 08:52 gen/TypstGrammarLexer.py
 -rw-rw-rw-  2.0 fat    10476 b- defN 23-May-30 08:50 gen/TypstGrammarListener.py
 -rw-rw-rw-  2.0 fat    94820 b- defN 23-May-30 08:52 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-30 15:03 typst_sympy_calculator-0.4.4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     9263 b- defN 23-May-30 15:03 typst_sympy_calculator-0.4.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 15:03 typst_sympy_calculator-0.4.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 15:03 typst_sympy_calculator-0.4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1168 b- defN 23-May-30 15:03 typst_sympy_calculator-0.4.4.dist-info/RECORD
-14 files, 182012 bytes uncompressed, 30185 bytes compressed:  83.4%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     9444 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1168 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/RECORD
+14 files, 182426 bytes uncompressed, 30271 bytes compressed:  83.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.4.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.4.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.4.dist-info/METADATA
+Filename: typst_sympy_calculator-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.4.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.4.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.4.dist-info/RECORD
+Filename: typst_sympy_calculator-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TypstCalculatorServer.py

```diff
@@ -3,43 +3,45 @@
 import re
 import os
 from TypstCalculator import TypstCalculator
 from DefaultTypstCalculator import get_default_calculator
 
 VERSION = '0.4.2'
 
+
 class TypstCalculatorServer:
 
-    def __init__(self, calculator: TypstCalculator = None) -> None:
+    def __init__(self, calculator: TypstCalculator = None, precision=15) -> None:
         if calculator is None:
             calculator = get_default_calculator()
         self.calculator = calculator
+        self.precision = precision
         self.cache_variance_names = []
         self.cache_mode = True
 
     @property
     def var(self):
         return self.calculator.var
 
     @property
     def variances(self):
         return self.calculator.variances
-    
+
     @property
     def return_text(self):
         return self.calculator.return_text
-    
+
     @return_text.setter
     def return_text(self, value):
         self.calculator.return_text = value
 
     @property
     def enable_subs(self):
         return self.calculator.enable_subs
-    
+
     @enable_subs.setter
     def enable_subs(self, value):
         self.calculator.enable_subs = value
 
     def init(self, typst_file: str) -> list:
         self.cache_mode = False
         typst_content = ''
@@ -54,15 +56,16 @@
                 if 'TYPST_ROOT' in os.environ:
                     root = os.environ['TYPST_ROOT']
                     absolute_path = os.path.join(root, import_path[1:])
                 else:
                     absolute_path = import_path
             else:
                 # Convert '../../path/to/typst'
-                absolute_path = os.path.abspath(os.path.join(os.path.dirname(typst_file), import_path))
+                absolute_path = os.path.abspath(os.path.join(
+                    os.path.dirname(typst_file), import_path))
             res.append(absolute_path)
             self.load_with_file(absolute_path)
         self.cache_mode = True
         return res
 
     def load_with_file(self, typst_file: str):
         typst_content = ''
@@ -158,20 +161,23 @@
         ```typst-calculator
         test()
         ```
         '''
         pattern1 = r'\s*```python\s*\n\s*# typst-calculator\s*\n([\d\D]*?)```'
         pattern2 = r'\s*```py\s*\n\s*# typst-calculator\s*\n([\d\D]*?)```'
         pattern3 = r'\s*```typst-calculator\s*\n([\d\D]*?)```'
+        pattern4 = r'\s*```typst-sympy-calculator\s*\n([\d\D]*?)```'
         for match in re.finditer(pattern1, typst_content):
             self.exec(match.group(1))
         for match in re.finditer(pattern2, typst_content):
             self.exec(match.group(1))
         for match in re.finditer(pattern3, typst_content):
             self.exec(match.group(1))
+        for match in re.finditer(pattern4, typst_content):
+            self.exec(match.group(1))
 
     def find_and_define_accent(self, typst_content: str):
         '''
         #let acc(x) = math.accent(x, math.grave)
         '''
         pattern = r'#let\s+([a-zA-z][a-zA-z0-9]*)\(\s*([_a-zA-z][_\-a-zA-z0-9]*)\s*\)\s*=\s*math\.accent'
         for match in re.finditer(pattern, typst_content):
@@ -251,8 +257,8 @@
     expr = server.simplify('b + 1', typst_file)
     print(expr)
     expr = server.simplify('cmat(1, 2)', typst_file)
     print(expr)
     expr = server.simplify('f(1) + f(1)', typst_file)
     print(expr)
     expr = server.simplify('xy + mail + mail.stamped', typst_file)
-    print(expr)
+    print(expr)
```

## Comparing `typst_sympy_calculator-0.4.4.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.4.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.4.4.dist-info/METADATA` & `typst_sympy_calculator-0.4.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.4.4
+Version: 0.4.5
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -172,14 +172,18 @@
 
 
 
 It is a top-down design, so you can use `TypstCalculatorServer` directly, or use `TypstCalculator` with `TypstConverter`.
 
 
 
+**RECOMMEND: see the usage of decorators like `@func()` in [DefaultTypstCalculator.py](https://github.com/OrangeX4/typst-sympy-calculator/blob/main/DefaultTypstCalculator.py).**
+
+
+
 For the usage, you can see the unit test part `if __name__ == '__main__':` in each files.
 
 
 
 
 
 ### Sympy Expressions and Typst Math Text
```

## Comparing `typst_sympy_calculator-0.4.4.dist-info/RECORD` & `typst_sympy_calculator-0.4.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 DefaultTypstCalculator.py,sha256=SpwQmZJ3SCXlFTFbXdD1e3nPywwzVztrlYCFEhzxd34,7111
 TypstCalculator.py,sha256=bfCf1g_vPkTDBp3gi8uVwmuybG3HJEspF226CcqVhiI,4242
-TypstCalculatorServer.py,sha256=zZttdalodR7MCBMP5IhBuZbrIDE2sPGeHTPJSXiuLZM,9751
+TypstCalculatorServer.py,sha256=NvFNnZeP2MbP-ICsIHX1dPOOVYlSn40q2FfulWWrAJg,9984
 TypstConverter.py,sha256=TjOPE9hIi2WEymjwol2yQ1yCqwTs7Ku4qSDoYRy0VRg,21073
 TypstParser.py,sha256=DITF_chsZwsHWesL80r56GffmrracxN-3VN-Oi3wfOE,5488
 gen/TypstGrammarLexer.py,sha256=Aikej0mIRul_3e7C1_-2s2F7uwvjUonnl2KF00ta57g,17356
 gen/TypstGrammarListener.py,sha256=xGPQlgbFCe87-de8BySwJkI-WihW4zrhuOYiyxtxKTc,10476
 gen/TypstGrammarParser.py,sha256=aHsN1SilWTuNnwetpk-5LBSB2XUxFC36PtV7YJLYx58,94820
 gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-typst_sympy_calculator-0.4.4.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
-typst_sympy_calculator-0.4.4.dist-info/METADATA,sha256=_ephh8zLjrORukGzx1ZSqQCVMOV5GKkDkEJgujKn41w,9263
-typst_sympy_calculator-0.4.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-typst_sympy_calculator-0.4.4.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
-typst_sympy_calculator-0.4.4.dist-info/RECORD,,
+typst_sympy_calculator-0.4.5.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
+typst_sympy_calculator-0.4.5.dist-info/METADATA,sha256=R50TYyr3BLWbhk8atF8iWefZS4YCZEhs2hiLrJh4NPo,9444
+typst_sympy_calculator-0.4.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+typst_sympy_calculator-0.4.5.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
+typst_sympy_calculator-0.4.5.dist-info/RECORD,,
```

