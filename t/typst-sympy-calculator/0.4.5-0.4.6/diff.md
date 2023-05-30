# Comparing `tmp/typst_sympy_calculator-0.4.5-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 32211 bytes, number of entries: 14
+Zip file size: 33115 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat     7111 b- defN 23-May-30 15:03 DefaultTypstCalculator.py
 -rw-rw-rw-  2.0 fat     4242 b- defN 23-May-30 08:32 TypstCalculator.py
 -rw-rw-rw-  2.0 fat     9984 b- defN 23-May-30 15:34 TypstCalculatorServer.py
 -rw-rw-rw-  2.0 fat    21073 b- defN 23-May-30 11:08 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
 -rw-rw-rw-  2.0 fat    17356 b- defN 23-May-30 08:52 gen/TypstGrammarLexer.py
 -rw-rw-rw-  2.0 fat    10476 b- defN 23-May-30 08:50 gen/TypstGrammarListener.py
 -rw-rw-rw-  2.0 fat    94820 b- defN 23-May-30 08:52 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     9444 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1168 b- defN 23-May-30 15:34 typst_sympy_calculator-0.4.5.dist-info/RECORD
-14 files, 182426 bytes uncompressed, 30271 bytes compressed:  83.4%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    12770 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1169 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/RECORD
+14 files, 185753 bytes uncompressed, 31175 bytes compressed:  83.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.5.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.4.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.5.dist-info/METADATA
+Filename: typst_sympy_calculator-0.4.6.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.5.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.5.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.5.dist-info/RECORD
+Filename: typst_sympy_calculator-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `typst_sympy_calculator-0.4.5.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.4.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.4.5.dist-info/METADATA` & `typst_sympy_calculator-0.4.6.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.4.5
+Version: 0.4.6
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -44,24 +44,28 @@
 
 
 
 It is designed for providing **people writing in typst** a ability to calculate something when writing math expression. It is based on `Sympy` module in `Python`.
 
 
 
-The `typst-calculator` python package is a backend for a VS Code extension, and you also can use it just for parse typst math expression to sympy form in order to do things for yourself.
+The `typst-sympy-calculator` python package is a backend for a VS Code extension [`Typst Sympy Calculator`](https://github.com/OrangeX4/vscode-typst-sympy-calculator), and you also can use it just for parse typst math expression to sympy form in order to do things for yourself.
 
 
 
 
 
 ## Features
 
 
 
+![Demo](https://picgo-1258602555.cos.ap-nanjing.myqcloud.com/typst-sympy-calculator.gif)
+
+
+
 - **Default Math:**
 
     - [x] **Arithmetic:** Add (`+`), Sub (`-`), Dot Mul (`dot`), Cross Mul (`times`), Frac (`/`), Power (`^`), Abs (`|x|`), Sqrt (`sqrt`), etc...
 
     - [x] **Alphabet:** `a - z`, `A - Z`, `alpha - omega`, Subscript (`x_1`), Accent Bar(`hat(x)`), etc...
 
     - [x] **Common Functions:** `gcd`, `lcm`, `floor`, `ceil`, `max`, `min`, `log`, `ln`, `exp`, `sin`, `cos`, `tan`, `csc`, `sec`, `cot`, `arcsin`, `sinh`, `arsinh`, etc...
@@ -72,14 +76,16 @@
 
     - [ ] **Calculous:** Derivation (`dif/(dif x) (x^2 + 1)`), etc...
 
     - [ ] **Reduce:** Sum `sum_(k=1)^oo (1/2)^k`, Product `product_(k=1)^oo (1/2)^k`
 
     - [x] **Linear Algebra:** Matrix to raw echelon form `rref`, Determinant `det`, Transpose `^T`, Inverse `^(-1)`, etc...
 
+    - [x] **Relations:** `==`, `>`, `>=`, `<`, `<=`, etc...
+
     - [ ] **Solve Equation:** Single Equation `x + 1 = 2`, Multiple Equations `cases(x + y = 1, x - y = 2)`, etc...
 
     - [x] **Other:** Binomial `binom(n, k)` ...
 
 - **Custom Math (in typst file):**
 
     - [x] **Define Accents:** `#let acc(x) = math.accent(x, math.grave)`
@@ -106,15 +112,15 @@
 
     - [x] Complete `TypstMathPrinter` in `TypstConverter.py`
 
     - [ ] Custom Printer for `TypstCalculator.py` and `TypstCalculatorServer.py`
 
 - **VS Code Extension:**
 
-    - [ ] Develop a VS Code Extension for `Typst Calculator`
+    - [x] Develop a VS Code Extension for `Typst Calculator`
 
 
 
 
 
 ## Install
 
@@ -446,14 +452,286 @@
 
 assert expr == '0'
 
 ```
 
 
 
+### Variances
+
+
+
+You can **ASSIGN** variance a value using same assignment form in typst:
+
+
+
+```typst
+
+#let x = 1
+
+
+
+// Before
+
+$ x $
+
+
+
+// Shift + Ctrl + E
+
+// After
+
+$ x = 1 $
+
+```
+
+
+
+PS: You can use grammar like `y == x + 1` to describe the relation of equality.
+
+
+
+If you want to see the bonding of variances, you can press `Shift + Ctrl + P`, and input `typst-sympy-calculator: Show Current variances`, then you will get data like:
+
+
+
+```typst
+
+y = x + 1
+
+z = 2 x
+
+```
+
+
+
+### Functions
+
+
+
+You can **DEFINE** a function using same form in typst:
+
+
+
+```typst
+
+#let f = math.op("f")
+
+
+
+// Before
+
+$ f(1) + f(1) $
+
+
+
+// Shift + Ctrl + E
+
+// After
+
+$ f(1) + f(1) = 2 f(1) $
+
+```
+
+
+
+### Symbols
+
+
+
+You can **DEFINE** a symbol using same form in typst:
+
+
+
+```typst
+
+#let xy = math.italic("xy")
+
+#let email = symbol("🖂", ("stamped", "🖃"),)
+
+
+
+$ xy + email + email.stamped $
+
+```
+
+
+
+### Accents
+
+
+
+You can **DEFINE** a accent using same form in typst:
+
+
+
+```typst
+
+#let acc(x) = math.accent(x, math.grave)
+
+
+
+$ acc(x) $
+
+```
+
+
+
+### Decorators for Operators
+
+
+
+You can **DEFINE** a operator using same form in typst:
+
+
+
+```typst
+
+#let add = math.op("+")
+
+
+
+'''typst-calculator
+
+@additive_op()
+
+def convert_add(a, b):
+
+    return a + b
+
+'''
+
+
+
+// Before
+
+$ 1 add 1 $
+
+
+
+// Shift + Ctrl + E
+
+// After
+
+$ 1 add 1 = 2 $
+
+```
+
+
+
+Or just use `'''typst-sympy-calculator` or `'''python \n # typst-calculator` to define a operator.
+
+
+
+there are some decorators you can use:
+
+
+
+- `@operator(type='ADDITIVE_OP', convert_ast=convert_ast, name=name, ast=False)`: Define a common operator;
+
+- `@func()`: Define a function, receive args list; 
+
+- `@func_mat()`: Define a matrix function, receive single arg `matrix`;
+
+- `@constant()`: Define a constant, receive no args but only return a constant value;
+
+- `@relation_op()`: Define a relation operator, receive args `a` and `b`;
+
+- `@additive_op()`: Define a additive operator, receive args `a` and `b`;
+
+- `@mp_op()`: Define a multiplicative operator, receive args `a` and `b`;
+
+- `@postfix_op()`: Define a postfix operator, receive args `a`;
+
+- `@reduce_op()`: Define a reduce operator, NOT IMPLEMENTED YET;
+
+
+
+It is important that the function name MUST be `def convert_{operator_name}`, or you can use decorator arg `@func(name='operator_name')`, and the substring `_dot_` will be replaced by `.`.
+
+
+
+There are some examples (from [DefaultTypstCalculator.py](https://github.com/OrangeX4/typst-sympy-calculator/blob/main/DefaultTypstCalculator.py)):
+
+
+
+```python
+
+# Constants
+
+@constant()
+
+def convert_oo():
+
+    return sympy.oo
+
+
+
+# Relation Operators
+
+@relation_op()
+
+def convert_eq(a, b):
+
+    return sympy.Eq(a, b)
+
+
+
+# Additive Operators
+
+@additive_op()
+
+def convert_plus(a, b):
+
+    return a + b
+
+
+
+# Mp Operators
+
+@mp_op()
+
+def convert_times(a, b):
+
+    return a * b
+
+
+
+# Postfix Operators
+
+@postfix_op()
+
+def convert_degree(expr):
+
+    return expr / 180 * sympy.pi
+
+
+
+# Matrix
+
+@func_mat()
+
+def convert_mat(mat):
+
+    return sympy.Matrix(mat)
+
+
+
+# Functions
+
+@func()
+
+def convert_binom(n, k):
+
+    return sympy.binomial(n, k)
+
+```
+
+
+
 
 
 ## Contributing
 
 
 
 1. Clone it by `git clone https://github.com/OrangeX4/typst-calculator.git`
```

## Comparing `typst_sympy_calculator-0.4.5.dist-info/RECORD` & `typst_sympy_calculator-0.4.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 TypstCalculatorServer.py,sha256=NvFNnZeP2MbP-ICsIHX1dPOOVYlSn40q2FfulWWrAJg,9984
 TypstConverter.py,sha256=TjOPE9hIi2WEymjwol2yQ1yCqwTs7Ku4qSDoYRy0VRg,21073
 TypstParser.py,sha256=DITF_chsZwsHWesL80r56GffmrracxN-3VN-Oi3wfOE,5488
 gen/TypstGrammarLexer.py,sha256=Aikej0mIRul_3e7C1_-2s2F7uwvjUonnl2KF00ta57g,17356
 gen/TypstGrammarListener.py,sha256=xGPQlgbFCe87-de8BySwJkI-WihW4zrhuOYiyxtxKTc,10476
 gen/TypstGrammarParser.py,sha256=aHsN1SilWTuNnwetpk-5LBSB2XUxFC36PtV7YJLYx58,94820
 gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-typst_sympy_calculator-0.4.5.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
-typst_sympy_calculator-0.4.5.dist-info/METADATA,sha256=R50TYyr3BLWbhk8atF8iWefZS4YCZEhs2hiLrJh4NPo,9444
-typst_sympy_calculator-0.4.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-typst_sympy_calculator-0.4.5.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
-typst_sympy_calculator-0.4.5.dist-info/RECORD,,
+typst_sympy_calculator-0.4.6.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
+typst_sympy_calculator-0.4.6.dist-info/METADATA,sha256=y0uigTP8-6F7mNpTy1Q0HxCZ7nvG2ovfTqhbEtY8HXE,12770
+typst_sympy_calculator-0.4.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+typst_sympy_calculator-0.4.6.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
+typst_sympy_calculator-0.4.6.dist-info/RECORD,,
```

