# Comparing `tmp/typst_sympy_calculator-0.4.1-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 32071 bytes, number of entries: 14
+Zip file size: 32095 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat     7017 b- defN 23-May-30 09:58 DefaultTypstCalculator.py
 -rw-rw-rw-  2.0 fat     4242 b- defN 23-May-30 08:32 TypstCalculator.py
--rw-rw-rw-  2.0 fat     9647 b- defN 23-May-30 09:52 TypstCalculatorServer.py
+-rw-rw-rw-  2.0 fat     9666 b- defN 23-May-30 11:43 TypstCalculatorServer.py
 -rw-rw-rw-  2.0 fat    21073 b- defN 23-May-30 11:08 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
 -rw-rw-rw-  2.0 fat    17356 b- defN 23-May-30 08:52 gen/TypstGrammarLexer.py
 -rw-rw-rw-  2.0 fat    10476 b- defN 23-May-30 08:50 gen/TypstGrammarListener.py
 -rw-rw-rw-  2.0 fat    94820 b- defN 23-May-30 08:52 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     9263 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1168 b- defN 23-May-30 11:10 typst_sympy_calculator-0.4.1.dist-info/RECORD
-14 files, 181814 bytes uncompressed, 30131 bytes compressed:  83.4%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-30 11:47 typst_sympy_calculator-0.4.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     9263 b- defN 23-May-30 11:47 typst_sympy_calculator-0.4.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 11:47 typst_sympy_calculator-0.4.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 11:47 typst_sympy_calculator-0.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1168 b- defN 23-May-30 11:47 typst_sympy_calculator-0.4.2.dist-info/RECORD
+14 files, 181833 bytes uncompressed, 30155 bytes compressed:  83.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.1.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.4.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.1.dist-info/METADATA
+Filename: typst_sympy_calculator-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.1.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.1.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.1.dist-info/RECORD
+Filename: typst_sympy_calculator-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TypstCalculatorServer.py

```diff
@@ -1,14 +1,15 @@
 import sympy
 import math
 import re
 import os
 from TypstCalculator import TypstCalculator
 from DefaultTypstCalculator import get_default_calculator
 
+VERSION = '0.4.2'
 
 class TypstCalculatorServer:
 
     def __init__(self, calculator: TypstCalculator = None) -> None:
         if calculator is None:
             calculator = get_default_calculator()
         self.calculator = calculator
```

## Comparing `typst_sympy_calculator-0.4.1.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.4.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.4.1.dist-info/METADATA` & `typst_sympy_calculator-0.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.4.1
+Version: 0.4.2
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `typst_sympy_calculator-0.4.1.dist-info/RECORD` & `typst_sympy_calculator-0.4.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 DefaultTypstCalculator.py,sha256=1Y7BRIx6E4oJHO1VSv4irsgMcQY2i9MdAi6yoHz2dYs,7017
 TypstCalculator.py,sha256=bfCf1g_vPkTDBp3gi8uVwmuybG3HJEspF226CcqVhiI,4242
-TypstCalculatorServer.py,sha256=5ro4T-UTLhpOPh5f8mt6wkV-mAWXvBg4dVJDzwRslPk,9647
+TypstCalculatorServer.py,sha256=R2mdK9ojdlm71Ybn4NO-5VdvFduLpqyKfmQ2N6xqckI,9666
 TypstConverter.py,sha256=TjOPE9hIi2WEymjwol2yQ1yCqwTs7Ku4qSDoYRy0VRg,21073
 TypstParser.py,sha256=DITF_chsZwsHWesL80r56GffmrracxN-3VN-Oi3wfOE,5488
 gen/TypstGrammarLexer.py,sha256=Aikej0mIRul_3e7C1_-2s2F7uwvjUonnl2KF00ta57g,17356
 gen/TypstGrammarListener.py,sha256=xGPQlgbFCe87-de8BySwJkI-WihW4zrhuOYiyxtxKTc,10476
 gen/TypstGrammarParser.py,sha256=aHsN1SilWTuNnwetpk-5LBSB2XUxFC36PtV7YJLYx58,94820
 gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-typst_sympy_calculator-0.4.1.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
-typst_sympy_calculator-0.4.1.dist-info/METADATA,sha256=gVkJKpZ-3eNm0Xhhv5RWvcGfyWSZjY6AmBaKqI3iYMc,9263
-typst_sympy_calculator-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-typst_sympy_calculator-0.4.1.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
-typst_sympy_calculator-0.4.1.dist-info/RECORD,,
+typst_sympy_calculator-0.4.2.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
+typst_sympy_calculator-0.4.2.dist-info/METADATA,sha256=yZb6qFLjihNJXA599Svs-cwmaR8Zwvy1uLdT5eC74uE,9263
+typst_sympy_calculator-0.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+typst_sympy_calculator-0.4.2.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
+typst_sympy_calculator-0.4.2.dist-info/RECORD,,
```

