# Comparing `tmp/typst_sympy_calculator-0.4.0-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 31641 bytes, number of entries: 14
+Zip file size: 32071 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat     7017 b- defN 23-May-30 09:58 DefaultTypstCalculator.py
 -rw-rw-rw-  2.0 fat     4242 b- defN 23-May-30 08:32 TypstCalculator.py
 -rw-rw-rw-  2.0 fat     9647 b- defN 23-May-30 09:52 TypstCalculatorServer.py
--rw-rw-rw-  2.0 fat    19053 b- defN 23-May-30 08:52 TypstConverter.py
+-rw-rw-rw-  2.0 fat    21073 b- defN 23-May-30 11:08 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
 -rw-rw-rw-  2.0 fat    17356 b- defN 23-May-30 08:52 gen/TypstGrammarLexer.py
 -rw-rw-rw-  2.0 fat    10476 b- defN 23-May-30 08:50 gen/TypstGrammarListener.py
 -rw-rw-rw-  2.0 fat    94820 b- defN 23-May-30 08:52 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-30 10:44 typst_sympy_calculator-0.4.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     9137 b- defN 23-May-30 10:44 typst_sympy_calculator-0.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 10:44 typst_sympy_calculator-0.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 10:44 typst_sympy_calculator-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1168 b- defN 23-May-30 10:44 typst_sympy_calculator-0.4.0.dist-info/RECORD
-14 files, 179668 bytes uncompressed, 29701 bytes compressed:  83.5%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     9263 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1168 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/RECORD
+14 files, 181814 bytes uncompressed, 30131 bytes compressed:  83.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.0.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.4.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.0.dist-info/METADATA
+Filename: typst_sympy_calculator-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.0.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.0.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.0.dist-info/RECORD
+Filename: typst_sympy_calculator-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TypstConverter.py

```diff
@@ -3,32 +3,72 @@
 from TypstParser import TypstMathParser
 from functools import wraps, reduce
 from typing import Callable
 
 
 class TypstMathPrinter(StrPrinter):
 
+    def paren(self, expr):
+        return '(' + self.doprint(expr) + ')' if expr.is_Add else self.doprint(expr)
+
     def _print_Mul(self, expr):
-        def paren(expr):
-            return '(' + self.doprint(expr) + ')' if expr.is_Add else self.doprint(expr)
-        return reduce(lambda x, y: x + ' ' + y, map(paren, expr.args))
+        return reduce(lambda x, y: x + ' ' + y, map(self.paren, expr.args))
     
     # matrix form: mat(1, 2; 3, 4)
     def _print_MatrixBase(self, expr):
         n, m, mat_flattern = expr.args
         res = 'mat('
         rows = [mat_flattern[i:i+m] for i in range(0, n*m, m)]
         res += '; '.join(map(lambda row: ', '.join(map(self.doprint, row)), rows))
         res += ')'
         return res
+
+    def _print_Limit(self, expr):
+        e, z = expr.args
+        return "lim_(%s -> %s) %s" % (self._print(z), self._print(z), self._print(e))
+
+    def _print_Integral(self, expr):
+        e, lims = expr.args
+        if len(lims) > 1:
+            return "integral_%s^%s %s dif %s" % (self.paren(lims[1]), self.paren(lims[2]), self._print(e), self._print(lims[0]))
+        else:
+            return "integral %s dif %s" % (self._print(e), self._print(lims))
     
+    def _print_Sum(self, expr):
+        e, lims = expr.args
+        return "sum_(%s = %s)^%s %s" % (self._print(lims[0]), self._print(lims[1]), self.paren(lims[2]), self._print(e))
+
+    def _print_Product(self, expr):
+        e, lims = expr.args
+        return "product_(%s = %s)^%s %s" % (self._print(lims[0]), self._print(lims[1]), self.paren(lims[2]), self._print(e))
+
+    def _print_factorial(self, expr):
+        return "%s!" % self._print(expr.args[0])
+
+    def _print_Derivative(self, expr):
+        e = expr.args[0]
+        wrt = expr.args[1]
+        return "dif / (dif %s) (%s)" % (self._print(wrt), self._print(e))
+    
+    def _print_Abs(self, expr):
+        return "|%s|" % self._print(expr.args[0])
+
+    def _print_Equality(self, expr):
+        return "%s = %s" % (self._print(expr.args[0]), self._print(expr.args[1]))
+
     # using ^ but not ** for power
     def _print_Pow(self, expr):
         b, e = expr.args
         base = self.doprint(b) if b.is_Atom else '(' + self.doprint(b) + ')'
+        if e is sympy.S.Half:
+            return "sqrt(%s)" % self.doprint(b)
+        if -e is sympy.S.Half:
+            return "1 / sqrt(%s)" % self.doprint(b)
+        if e is -sympy.S.One:
+            return "1 / %s" % base
         if e.is_Atom or e.is_Pow:
             return base + '^' + self.doprint(e)
         else:
             return base + '^' + '(' + self.doprint(e) + ')'
 
 
 class TypstMathConverter(object):
@@ -480,29 +520,41 @@
         return sympy.matrices.Matrix(mat)
     
     convertor.define_symbol_base('x')
     convertor.define_symbol_base('y')
     convertor.define_symbol_base('z')
     expr = convertor.sympy('1 + sin^2 1/2 + x + 1')
     typst = convertor.typst(sympy.simplify(expr))
-    print(typst)
+    assert typst == 'x + (sin(1/2))^2 + 2'
 
     expr = convertor.sympy('(x y)^y^(z+1)')
     typst = convertor.typst(sympy.simplify(expr))
-    print(typst)
+    assert typst == '(x y)^y^(z + 1)'
 
     expr = convertor.sympy('mat(x + y, 2; z, 4)')
     typst = convertor.typst(sympy.simplify(expr))
-    print(typst)
+    assert typst == 'mat(x + y, 2; z, 4)'
 
     convertor.define_function('f_1')
     expr = convertor.sympy('f_1^2(1) + f_1(1)')
     typst = convertor.typst(sympy.simplify(expr))
-    print(typst)
+    assert typst == '(f_1(1) + 1) f_1(1)'
 
     expr = convertor.sympy('x * y * z')
     typst = convertor.typst(expr)
     assert typst == 'x y z'
 
     expr = convertor.sympy('(x + 1) * y * z')
     typst = convertor.typst(expr)
-    assert typst == 'y z (x + 1)'
+    assert typst == 'y z (x + 1)'
+
+    expr = convertor.sympy('(x + 1) * y^(1/2)')
+    typst = convertor.typst(expr)
+    assert typst == 'sqrt(y) (x + 1)'
+
+    expr = convertor.sympy('|x|')
+    typst = convertor.typst(expr)
+    assert typst == '|x|'
+
+    expr = convertor.sympy('integral_1^2 x^2 dif x')
+    typst = convertor.typst(expr)
+    assert typst == 'integral_1^2 x^2 dif x'
```

## Comparing `typst_sympy_calculator-0.4.0.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.4.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.4.0.dist-info/METADATA` & `typst_sympy_calculator-0.4.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,18 +24,20 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: sympy (>=1.4)
 Requires-Dist: antlr4-python3-runtime (==4.7.2)
 
-# Typst Sympy Calculator
+![Logo](https://picgo-1258602555.cos.ap-nanjing.myqcloud.com/icon.png)
 
 
 
+# [Typst Sympy Calculator](https://github.com/OrangeX4/typst-sympy-calculator)
+
 
 
 ## About
 
 
 
 `Typst Sympy Calculator` parses **Typst Math Expressions** and converts it into the equivalent **SymPy form**. Then, **calculate it** and convert to typst math text. 
@@ -98,15 +100,15 @@
 
             return a + b
 
         ```
 
 - **Typst Math Printer:**
 
-    - [ ] Complete Typst Math Printer in `TypstConverter.py`
+    - [x] Complete `TypstMathPrinter` in `TypstConverter.py`
 
     - [ ] Custom Printer for `TypstCalculator.py` and `TypstCalculatorServer.py`
 
 - **VS Code Extension:**
 
     - [ ] Develop a VS Code Extension for `Typst Calculator`
```

## Comparing `typst_sympy_calculator-0.4.0.dist-info/RECORD` & `typst_sympy_calculator-0.4.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 DefaultTypstCalculator.py,sha256=1Y7BRIx6E4oJHO1VSv4irsgMcQY2i9MdAi6yoHz2dYs,7017
 TypstCalculator.py,sha256=bfCf1g_vPkTDBp3gi8uVwmuybG3HJEspF226CcqVhiI,4242
 TypstCalculatorServer.py,sha256=5ro4T-UTLhpOPh5f8mt6wkV-mAWXvBg4dVJDzwRslPk,9647
-TypstConverter.py,sha256=z6w2AeH0ob8idnlcPnL2kZ-7crPXd5vkaK31uprQz0A,19053
+TypstConverter.py,sha256=TjOPE9hIi2WEymjwol2yQ1yCqwTs7Ku4qSDoYRy0VRg,21073
 TypstParser.py,sha256=DITF_chsZwsHWesL80r56GffmrracxN-3VN-Oi3wfOE,5488
 gen/TypstGrammarLexer.py,sha256=Aikej0mIRul_3e7C1_-2s2F7uwvjUonnl2KF00ta57g,17356
 gen/TypstGrammarListener.py,sha256=xGPQlgbFCe87-de8BySwJkI-WihW4zrhuOYiyxtxKTc,10476
 gen/TypstGrammarParser.py,sha256=aHsN1SilWTuNnwetpk-5LBSB2XUxFC36PtV7YJLYx58,94820
 gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-typst_sympy_calculator-0.4.0.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
-typst_sympy_calculator-0.4.0.dist-info/METADATA,sha256=H-a3-yV_0pP8qYnrxIJ1VGdTe6vG40dRrKNEsuSANks,9137
-typst_sympy_calculator-0.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-typst_sympy_calculator-0.4.0.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
-typst_sympy_calculator-0.4.0.dist-info/RECORD,,
+typst_sympy_calculator-0.4.1.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
+typst_sympy_calculator-0.4.1.dist-info/METADATA,sha256=gVkJKpZ-3eNm0Xhhv5RWvcGfyWSZjY6AmBaKqI3iYMc,9263
+typst_sympy_calculator-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+typst_sympy_calculator-0.4.1.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
+typst_sympy_calculator-0.4.1.dist-info/RECORD,,
```

