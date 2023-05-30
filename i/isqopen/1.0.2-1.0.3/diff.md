# Comparing `tmp/isqopen-1.0.2.tar.gz` & `tmp/isqopen-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isqopen-1.0.2.tar", last modified: Wed May 24 10:19:57 2023, max compression
+gzip compressed data, was "dist/isqopen-1.0.3.tar", last modified: Tue May 30 02:39:13 2023, max compression
```

## Comparing `isqopen-1.0.2.tar` & `isqopen-1.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.737680 isqopen-1.0.2/
--rw-r--r--   0 huazhelou   (501) staff       (20)     1093 2022-09-07 10:16:53.000000 isqopen-1.0.2/LICENSE
--rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-05-24 10:19:57.737844 isqopen-1.0.2/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)      734 2022-09-24 07:03:24.000000 isqopen-1.0.2/README.md
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.728250 isqopen-1.0.2/isq/
--rw-r--r--   0 huazhelou   (501) staff       (20)      247 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/__init__.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.731938 isqopen-1.0.2/isq/compile/
--rw-r--r--   0 huazhelou   (501) staff       (20)     5836 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/QSyn.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    11380 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/Simplify.py
--rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5152 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/matlab_gsvd.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    14686 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/parser.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    22701 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/parsetab.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    27584 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/passes.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5050 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/qtypes.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2183 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/tokrules.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2539 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/tools.py
--rw-r--r--   0 huazhelou   (501) staff       (20)       18 2023-05-24 10:17:35.000000 isqopen-1.0.2/isq/config.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.733715 isqopen-1.0.2/isq/device/
--rw-r--r--   0 huazhelou   (501) staff       (20)      142 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     6547 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/device.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     1882 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/grad.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     3166 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/task.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     4293 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/translate.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.734467 isqopen-1.0.2/isq/draw/
--rw-r--r--   0 huazhelou   (501) staff       (20)       26 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/draw/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     7986 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/draw/drawer.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2652 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/errors.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     1221 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/globalVar.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    10006 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/mapping.py
--rw-r--r--   0 huazhelou   (501) staff       (20)      250 2023-05-24 10:17:35.000000 isqopen-1.0.2/isq/qpu.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     6707 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/quantum.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.735461 isqopen-1.0.2/isq/simulate/
--rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:17:35.000000 isqopen-1.0.2/isq/simulate/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    12918 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/simulate/operation.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5256 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/simulate/simulator.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.737412 isqopen-1.0.2/isqopen.egg-info/
--rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)      775 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/SOURCES.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/dependency_links.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/not-zip-safe
--rw-r--r--   0 huazhelou   (501) staff       (20)       57 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/requires.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        4 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/top_level.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-05-24 10:19:57.738368 isqopen-1.0.2/setup.cfg
--rw-r--r--   0 huazhelou   (501) staff       (20)      738 2023-05-24 10:19:36.000000 isqopen-1.0.2/setup.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.916114 isqopen-1.0.3/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1093 2022-09-07 10:16:53.000000 isqopen-1.0.3/LICENSE
+-rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-05-30 02:39:13.916269 isqopen-1.0.3/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)      734 2022-09-24 07:03:24.000000 isqopen-1.0.3/README.md
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.889571 isqopen-1.0.3/isq/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      273 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/__init__.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.903533 isqopen-1.0.3/isq/compile/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5836 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/QSyn.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    11380 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/Simplify.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5152 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/matlab_gsvd.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    15317 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/parser.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    25877 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/parsetab.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    36609 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/passes.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5111 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/qtypes.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2227 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/tokrules.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2539 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/tools.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)       18 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/config.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.907285 isqopen-1.0.3/isq/device/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      142 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     6745 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/device.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1882 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/grad.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     3166 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/task.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5354 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/translate.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.908686 isqopen-1.0.3/isq/draw/
+-rw-r--r--   0 huazhelou   (501) staff       (20)       26 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/draw/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     7986 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/draw/drawer.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2652 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/errors.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)      644 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/globalVar.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    10006 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/mapping.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)      250 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/qpu.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     6707 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/quantum.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.910880 isqopen-1.0.3/isq/simulate/
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/simulate/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    13705 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/simulate/operation.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5523 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/simulate/simulator.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.915709 isqopen-1.0.3/isqopen.egg-info/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)      775 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/SOURCES.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/dependency_links.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/not-zip-safe
+-rw-r--r--   0 huazhelou   (501) staff       (20)       57 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/requires.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        4 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/top_level.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-05-30 02:39:13.917122 isqopen-1.0.3/setup.cfg
+-rw-r--r--   0 huazhelou   (501) staff       (20)      738 2023-05-30 02:37:49.000000 isqopen-1.0.3/setup.py
```

### Comparing `isqopen-1.0.2/LICENSE` & `isqopen-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/PKG-INFO` & `isqopen-1.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isqopen
-Version: 1.0.2
+Version: 1.0.3
 Summary: isq quantum kernel
 Author: Lou Huazhe
 Author-email: louhz@arclightquantum.com
 Platform: python 3.8+
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `isqopen-1.0.2/README.md` & `isqopen-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/compile/QSyn.py` & `isqopen-1.0.3/isq/compile/QSyn.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/compile/Simplify.py` & `isqopen-1.0.3/isq/compile/Simplify.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/compile/matlab_gsvd.py` & `isqopen-1.0.3/isq/compile/matlab_gsvd.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/compile/parser.py` & `isqopen-1.0.3/isq/compile/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,28 @@
     yacc
 )
 import typing as T
 from typing import (cast, List, Any)
 from .qtypes import *
 from . import tokrules
 from .tokrules import tokens
-from isq.globalVar import msgDic
-import numpy as np
-import sys
-import logging
 from isq.config import debug_mode
 from isq.errors import *
 from .passes import PartialEvaluation
 import time
 
 
 current_line = 0
 current_ID = ''
 
 class IR:
     def __init__(self):
         self.out = ""
-        self.error: Any = None
+        self.code = ''
+        self.msg = ''
 
 def trace_time(timer, reason: str):
     t = time.time()
     if debug_mode:
         print("Time cost for {}: {}s".format(reason, t-timer))
     return t
 
@@ -97,20 +94,31 @@
     '''varDef : defclause
               | varDef defclause'''
     if (len(p) == 2):
         p[0] = Node("defBlock",[p[1]])
     else:
         p[0] = Node("defBlock",p[1].children+[p[2]])
 
+
 def p_defclause(p):
-    ''' defclause : QBIT seen_Qbit id_list ';' '''
+    ''' defclause : QBIT seen_Qbit id_list ';'
+        | QCOUPLE id_list ';'
+        | VAR ID '=' NUMBER ';'
+        | VAR ID '[' NUMBER ']' '=' '{' matrixContents '}' ';' '''
     global current_line
     if debug_mode == True:
         print("qbit defining")
-    p[0] = Node("qbitDef", p[3], None, p.lineno(0))
+    if len(p) == 4:
+        p[0] = Node("qtupleDef", p[2], None, p.lineno(0))
+    elif len(p) == 5:
+        p[0] = Node("qbitDef", p[3], None, p.lineno(0))
+    elif len(p) == 6:
+        p[0] = Node("classDef", [p[2]], p[4], p.lineno(0))
+    else:
+        p[0] = Node("classDef", [p[2], p[4]], p[8], p.lineno(0))
 
 def p_seen_Qbit(p):
     '''seen_Qbit : '''
 
 #def p_seen_Int(p):
 #    '''seen_Int : '''
     
@@ -274,15 +282,15 @@
             ThrowUndefinedVariable(p.lineno(1), arr_name)
         if(not is_array(arr_ty)):
             ThrowTypeMismatch(p.lineno(1), "int[]", stringify_type(arr_ty))
         arr_ty2 = T.cast(ArrayType, arr_ty)
         if(not is_int(arr_ty2)):
             ThrowTypeMismatch(p.lineno(1), "int[]", stringify_type(arr_ty))
         '''
-        p3[0]=Node("intExprArrayRef", [p3[3]], p3[1])
+        p3[0]=Node("intExprArrayRef", [p3[3]], p3[1], p.lineno(1))
     elif(len(p)==4):
         # bracket
         p4=T.cast(Arg_IntExprAtom4, p)
         p4[0]=p4[2]
     elif(len(p)==8):
         # measurement
         p5=T.cast(Arg_IntExprAtom5, p)
@@ -353,27 +361,34 @@
     else:
         p[0] = Node('ifStat', [p[3], p[5], p[4]], [p[8], p[12]], p.lineno(1))
 
 def p_qbitUnitaryStatement(p):
     ''' qbitUnitaryStatement : uGate '<' qubitListExpr '>' ';' 
         | uGate '(' qubitListExpr  ')' ';' 
         | rGate '<' intExpr ',' qubitListExpr '>' ';'
-        | rGate '(' intExpr ',' qubitListExpr ')' ';' '''
+        | rGate '(' intExpr ',' qubitListExpr ')' ';' 
+        | rxyGate '(' intExpr ',' intExpr ',' qubitListExpr ')' ';'
+        | rxyGate '<' intExpr ',' intExpr ',' qubitListExpr '>' ';' '''
     #''' qbitUnitaryStatement : id_list '=' uGate '[' id_list ']' ';' '''
     if (p.lineno(1) != p.lineno(len(p)-1)):
         ErrorThrow('in line ' + str(p.lineno(1)))
     
     if len(p) == 6:
         p[0] = Node('unitStat',p[3], [p[1]], p.lineno(1))
-    else:
+    elif len(p) == 8:
         p[0] = Node('unitStat',p[5], [p[1], p[3]], p.lineno(1))
-        
+    else:
+        p[0] = Node('unitStat',p[7], [p[1], p[3], p[5]], p.lineno(1))
     # turn tuple (qID, index) to string 'qID[index]'
     #print(listU)
-    
+
+def p_rxyGate(p):
+    ''' rxyGate : RXY '''
+    p[0] = p[1]    
+
 def p_rGate(p):
     ''' rGate : RX
               | RY
               | RZ '''
     p[0] = p[1]
     
 def p_uGate(p):
@@ -425,15 +440,15 @@
     y - z + x == 8
     for (i=1i<0i++)
     (x,y) = CX(x,y)
     
 '''
 
 
-def compile(ir: IR, data, target='isq', gate = {}, par = {}, args = None):
+def compile(ir: IR, data, target='isq', gate = {}, hardware=None, par = {}, args = None):
 
     pre_time = time.time()
     try:
         lexer = lex.lex(module = tokrules)
         lexer.input(data)
         pre_time = trace_time(pre_time, "lex")
 
@@ -446,15 +461,15 @@
         s = T.cast(Node, parser.parse(data, tracking = True))
         pre_time = trace_time(pre_time, "yacc")
         # if debug_mode == True:
         # print(s.type)
         
         #s = passes.flatten_qbitdef_list(s)
         #globalVar.trace_time("flatten")
-        mypass = PartialEvaluation(gate, par, target, args)
+        mypass = PartialEvaluation(gate, par, target, args, hardware)
         ir.out = mypass.visitProgram(s)
         pre_time = trace_time(pre_time, "partial evaluation")
         #return 0
         #if globalVar.print_ast:
         #    print(json.dumps(s, default=vars, indent=4))
         #    return 0
         # construct symbol table for procedure calls
@@ -481,9 +496,10 @@
             print("compilation succeed!")
 
         #if debug_mode == True:
         #   print("------------------------the compilation result------------------------")
         return 0
 
     except CompileError as e:
-        ir.error = "{}: {}".format(msgDic[e.code], e.msg)
+        ir.code = e.code
+        ir.msg = e.msg
         return -1
```

### Comparing `isqopen-1.0.2/isq/compile/passes.py` & `isqopen-1.0.3/isq/compile/passes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from .qtypes import *
 import typing as T
-import copy
 from isq.errors import *
 import numpy as np
-import time
 from .tools import decompose
-
+import json
 """
 Flatten defBlock into a list of definitions.
 This makes qbitDef children Tuple[var_array|var] -> List[var_array|var]
 """
 '''
 def flatten_qbitdef_list(s: Node)->Node:
     defs = T.cast(Node, s.children[0])
@@ -41,21 +39,28 @@
         ], q[0])
 
 """
 Partial evaluation, unrolling all loops and perform all integer computations.
 After partial evaluation all qubit arguments should be constants.
 """
 
+default_config = {
+    "qubit_number": 66,
+    "qubit_id": [],
+	"topo": [[1, 7], [1, 8], [2, 8], [2, 9], [3, 9], [3, 10], [4, 10], [4, 11], [5, 11], [5, 12], [6, 12], [7, 13], [8, 14], [8, 13], [9, 15], [9, 14], [10, 16], [10, 15], [11, 17], [11, 16], [12, 18], [12, 17], [13, 19], [13, 20], [14, 20], [14, 21], [15, 21], [15, 22], [16, 22], [16, 23], [17, 23], [17, 24], [18, 24], [19, 25], [20, 26], [20, 25], [21, 27], [21, 26], [22, 28], [22, 27], [23, 29], [23, 28], [24, 30], [24, 29], [25, 31], [25, 32], [26, 32], [26, 33], [27, 33], [27, 34], [28, 34], [28, 35], [29, 35], [29, 36], [30, 36], [31, 37], [32, 38], [32, 37], [33, 39], [33, 38], [34, 40], [34, 39], [35, 41], [35, 40], [36, 42], [36, 41], [37, 43], [37, 44], [38, 44], [38, 45], [39, 45], [39, 46], [40, 46], [40, 47], [41, 47], [41, 48], [42, 48], [43, 49], [44, 50], [44, 49], [45, 51], [45, 50], [46, 52], [46, 51], [47, 53], [47, 52], [48, 54], [48, 53], [49, 55], [49, 56], [50, 56], [50, 57], [51, 57], [51, 58], [52, 58], [52, 59], [53, 59], [53, 60], [54, 60], [55, 61], [56, 62], [56, 61], [57, 63], [57, 62], [58, 64], [58, 63], [59, 65], [59, 64], [60, 66], [60, 65]],
+    "tuple": {"66": ["0", "6"], "67": ["0", "7"], "68": ["1", "7"], "69": ["1", "8"], "70": ["2", "8"], "71": ["2", "9"], "72": ["3", "9"], "73": ["3", "10"], "74": ["4", "10"], "75": ["4", "11"], "76": ["5", "11"], "77": ["6", "12"], "78": ["7", "12"], "79": ["7", "13"], "80": ["8", "13"], "81": ["8", "14"], "82": ["9", "14"], "83": ["9", "15"], "84": ["10", "15"], "85": ["10", "16"], "86": ["11", "16"], "87": ["11", "17"], "88": ["12", "18"], "89": ["12", "19"], "90": ["13", "19"], "91": ["13", "20"], "92": ["14", "20"], "93": ["14", "21"], "94": ["15", "21"], "95": ["15", "22"], "96": ["16", "22"], "97": ["16", "23"], "98": ["17", "23"], "99": ["18", "24"], "100": ["19", "24"], "101": ["19", "25"], "102": ["20", "25"], "103": ["20", "26"], "104": ["21", "26"], "105": ["21", "27"], "106": ["22", "27"], "107": ["22", "28"], "108": ["23", "28"], "109": ["23", "29"], "110": ["24", "30"], "111": ["24", "31"], "112": ["25", "31"], "113": ["25", "32"], "114": ["26", "32"], "115": ["26", "33"], "116": ["27", "33"], "117": ["27", "34"], "118": ["28", "34"], "119": ["28", "35"], "120": ["29", "35"], "121": ["30", "36"], "122": ["31", "36"], "123": ["31", "37"], "124": ["32", "37"], "125": ["32", "38"], "126": ["33", "38"], "127": ["33", "39"], "128": ["34", "39"], "129": ["34", "40"], "130": ["35", "40"], "131": ["35", "41"], "132": ["36", "42"], "133": ["36", "43"], "134": ["37", "43"], "135": ["37", "44"], "136": ["38", "44"], "137": ["38", "45"], "138": ["39", "45"], "139": ["39", "46"], "140": ["40", "46"], "141": ["40", "47"], "142": ["41", "47"], "143": ["42", "48"], "144": ["43", "48"], "145": ["43", "49"], "146": ["44", "49"], "147": ["44", "50"], "148": ["45", "50"], "149": ["45", "51"], "150": ["46", "51"], "151": ["46", "52"], "152": ["47", "52"], "153": ["47", "53"], "154": ["48", "54"], "155": ["48", "55"], "156": ["49", "55"], "157": ["49", "56"], "158": ["50", "56"], "159": ["50", "57"], "160": ["51", "57"], "161": ["51", "58"], "162": ["52", "58"], "163": ["52", "59"], "164": ["53", "59"], "165": ["54", "60"], "166": ["55", "60"], "167": ["55", "61"], "168": ["56", "61"], "169": ["56", "62"], "170": ["57", "62"], "171": ["57", "63"], "172": ["58", "63"], "173": ["58", "64"], "174": ["59", "64"], "175": ["59", "65"]}
+}
+
 class PartialEvaluation(object):
     sym_table: T.Dict[str, int]
     current_pos: T.Optional[int]
     polytope_vars: T.List[str]
     measured_qubits: T.Set[str]
     emitted_insns: T.List[Node]
-    def __init__(self, addgate = {},  paramdic = {}, target = 'isq', args = None, module = 'ir'):
+    def __init__(self, addgate = {},  paramdic = {}, target = 'isq', args = None, hardware = None, module = 'ir'):
         self.measured_qubits=set()
         self.polytope_vars=[]
         self.sym_table={}
         self.current_pos=None
         self.emitted_insns=[]
         self.out = []
 
@@ -81,15 +86,15 @@
 
         self.for_cnt = 0
         self.for_val = []
         self.for_key = {}
         self.lamb = {}
         self.grad = False
 
-        self.gateset = set(['H','X','Y','Z','S','T','CZ','CY', 'CX','CNOT', 'M', 'RX', 'RY', 'RZ', 'SD', 'TD', 'X2M', 'X2P', 'Y2M', 'Y2P'])
+        self.gateset = set(['H','X','Y','Z','S','T','CZ','CY', 'CX','CNOT', 'M', 'RX', 'RY', 'RZ', 'SD', 'TD', 'X2M', 'X2P', 'Y2M', 'Y2P', 'RXY'])
         self.openqasm_gate = {
             'H': 'h',
             'X': 'x',
             'Y': 'y',
             'Z': 'z',
             'X2P': 'rx(pi/2)',
             'X2M': 'rx(-pi/2)',
@@ -106,15 +111,37 @@
             'M': 'measure',
             'RX': 'rx',
             'RY': 'ry',
             'RZ': 'rz'
         }
         self.indextime = 0.0
         self.out_pos = 0
-  
+
+        json_data = default_config
+        self.hardware = hardware
+        if self.hardware:
+            with open(self.hardware, 'r', encoding='utf8') as fp:
+                json_data = json.load(fp)
+
+        self.qnum = json_data['qubit_number']
+        self.qid = json_data['qubit_id']
+        self.tuple = json_data['tuple']
+        self.topo = {}
+        if len(self.qid) == 0:
+            self.qid = list(range(1, self.qnum+1))
+        topo = json_data['topo']
+        for x, y in topo:
+            x = str(x)
+            y = str(y)
+            if x not in self.topo:
+                self.topo[x] = set()
+            if y not in self.topo:
+                self.topo[y] = set()
+            self.topo[x].add(y)
+            self.topo[y].add(x)
 
     def visitProgram(self, s: Node)->Node:
         #print(self.varDic)
         new_prog = []
         if s.leaf != None:
             for p in s.leaf:
                 self.visitGateDef(p)
@@ -181,27 +208,38 @@
             
         if s.val == None:
             #judge gate and qbit number
             gateL = T.cast(T.Tuple[list], s.leaf)
             gate = gateL[0]
             gateq_cnt = 0
             if gate in self.gateset:
-                if gate in ['H','X','Y','Z','S','T', 'RX', 'RY', 'RZ', 'SD', 'TD', 'X2M', 'X2P', 'Y2M', 'Y2P']:
+                if gate in ['H','X','Y','Z','S','T', 'RX', 'RY', 'RZ', 'SD', 'TD', 'X2M', 'X2P', 'Y2M', 'Y2P', 'RXY']:
                     if gate in ['RX', 'RY', 'RZ']:
                         self.grad = False
                         tmps = self.evaluateIntExpr(gateL[1], 1)
                         if self.grad: gateL[1] = (gateL[1], self.grad)
                         else: gateL[1] = (tmps, self.grad)
+                    elif gate == 'RXY':
+                        self.grad = False
+                        phi = self.evaluateIntExpr(gateL[1], 1)
+                        if self.grad: gateL[1] = (gateL[1], self.grad)
+                        else: gateL[1] = (phi, self.grad)
+                        self.grad = False
+                        theta = self.evaluateIntExpr(gateL[2], 1)
+                        if self.grad: gateL[2] = (gateL[2], self.grad)
+                        else: gateL[2] = (theta, self.grad)
                     gateq_cnt = 1
                     if len(s.children.children) != 1:
                         ErrorThrow('in line {}, gate size does not coincide with the qubit number'.format(s.pos))
+                '''
                 else:
                     gateq_cnt = 2
                     if len(s.children.children) != 2:
                         ErrorThrow('in line {}, gate size does not coincide with the qubit number'.format(s.pos))
+                '''
             else:
                 gateInfo = self.gateDic.get(gate)
                 if gateInfo == None:
                     ErrorThrow('in line {}, gate not defined'.format(s.pos))
                 if gateInfo[0] != len(s.children.children):
                     ErrorThrow('in line {}, gate size does not coincide with the qubit number'.format(s.pos))
                 gateq_cnt = gateInfo[0]
@@ -319,15 +357,15 @@
                 ThrowTypeMismatch(s.pos, "qbit", stringify_type(qbit_ty))
             return (T.cast(str, s.leaf), 0, self.qDic.get(s.leaf))
         elif s.type=="qubitArrayRef":
             arr_name=s.leaf
             arr_ty = self.queryVariable(arr_name)
             if(arr_ty==None):
                 ThrowUndefinedVariable(s.pos, arr_name)
-            if(not is_array(arr_ty, "qbit")):
+            if(not is_array(arr_ty, "qbit")) and (not is_array(arr_ty, "qtuple")):
                 ThrowTypeMismatch(s.pos, "qbit[]", stringify_type(arr_ty))
             size = self.qubit_array_size(T.cast(str, s.leaf))
             indices = self.evaluateRangeAndSection(s.children[0])
             '''
             for index in indices:
                 if index >= size:
                     ThrowArrayOutOfBound(self.error_pos(), index, T.cast(str, s.leaf), size)
@@ -364,15 +402,15 @@
                 res += ','
             res = res[:-1]+']'
             return res#list(map(lambda x: self.evaluateIntExpr(x), s.children))
         else:
             ICE("Unknown range/section type: "+s.type)
             
     def evaluateIntExpr(self, s: Node, allow_type = 0)->int:
-
+        
         need_type = (int)
         if allow_type == 1:
             need_type = (int, float)
 
         if s.type=="intExprVar":
             var_name=s.leaf
             if var_name == 'pi': return str(np.pi)
@@ -557,60 +595,92 @@
 
         if not flag:
             ErrorThrow(res)
         
         self.gateDef[p[0]] = res
         
     def visitVarDef(self, s:Node):
-        for p in s.children: 
-            if (len(p) == 1):
-                if (self.proc_key != ''):
-                    if (self.localVarDic[self.proc_key].get(p[0]) != None):
-                        ErrorThrow('in line ' + str(s.pos) + ', '+ p[0] + "redeclaration!")
-                    self.localVarDic[self.proc_key][p[0]] = self.var_type
-                else:
-                    if (self.varDic.get(p[0]) != None):
-                        ErrorThrow('in line ' + str(s.pos) + ', '+ p[0] + "redeclaration!")
-                    self.varDic[p[0]] = self.var_type
+        if s.type == 'qbitDef' or s.type == 'qtupleDef':
+            self.var_type = 'qbit'
+            if s.type == 'qtupleDef': self.var_type = 'qtuple'
+            for p in s.children: 
+                if (len(p) == 1):
+                    if (self.proc_key != ''):
+                        if (self.localVarDic[self.proc_key].get(p[0]) != None):
+                            ErrorThrow('in line ' + str(s.pos) + ', '+ p[0] + "redeclaration!")
+                        self.localVarDic[self.proc_key][p[0]] = self.var_type
+                    else:
+                        if (self.varDic.get(p[0]) != None):
+                            ErrorThrow('in line ' + str(s.pos) + ', '+ p[0] + "redeclaration!")
+                        self.varDic[p[0]] = self.var_type
+                else:
+                    p1: VarKey = p[0]
+                    p3: int = p[1]
+                    if type(p[1]) != int:
+                        ErrorThrow('in line ' + str(s.pos) + ', '+ p[1] + "is not an integer!")
+                    if (self.proc_key != ''):
+                        if (self.localVarDic[self.proc_key].get(p[0]) != None):
+                            ErrorThrow('in line ' + str(s.pos) + ', '+ p[0] + "redeclaration!")
+                        self.localVarDic[self.proc_key][p1] = (self.var_type,p3)
+                    else:
+                        if (self.varDic.get(p[0]) != None):
+                            ErrorThrow('in line ' + str(p.pos) + ', '+ p[0] + " redeclaration!")
+                        self.varDic[p1] = (self.var_type, p3)
+        elif s.type == 'classDef':
+            c, l = s.children, s.leaf
+            cid = c[0]
+            if (self.proc_key != ''):
+                if (self.localVarDic[self.proc_key].get(cid) != None):
+                    ErrorThrow('in line ' + str(s.pos) + ', '+ cid + "redeclaration!")
+                else:
+                    if (self.varDic.get(cid) != None):
+                        ErrorThrow('in line ' + str(s.pos) + ', '+ cid + "redeclaration!")
+
+            if len(c) == 1:
+                self.param[c[0]] = l
             else:
-                p1: VarKey = p[0]
-                p3: int = p[1]
-                if type(p[1]) != int:
-                    ErrorThrow('in line ' + str(s.pos) + ', '+ p[1] + "is not an integer!")
-                if (self.proc_key != ''):
-                    if (self.localVarDic[self.proc_key].get(p[0]) != None):
-                        ErrorThrow('in line ' + str(s.pos) + ', '+ p[0] + "redeclaration!")
-                    self.localVarDic[self.proc_key][p1] = (self.var_type,p3)
-                else:
-                    if (self.varDic.get(p[0]) != None):
-                        ErrorThrow('in line ' + str(p.pos) + ', '+ p[0] + " redeclaration!")
-                    self.varDic[p1] = (self.var_type, p3)
+                if type(c[1]) != int:
+                    ErrorThrow('in line ' + str(s.pos) + ', '+ c[1] + "is not an integer!")
+                vals = [eval(v) for v in l.split(',')]
+                if len(vals) != c[1]: ErrorThrow(f'in line {s.pos}, need {c[1]} but give {len(vals)} values')
+                self.param[c[0]] = vals
+            #print(self.param)
     
     def construct_globalVar(self):
         
         self.qDic = {}
         self.cDic = {}
         self.q_cnt = 0
         self.c_cnt = 0
+        self.qt_cnt = self.qnum
         for key in self.varDic:
             if (self.varDic[key] == 'qbit'):
                 self.qDic[key] = self.q_cnt
                 self.q_cnt = self.q_cnt + 1
             elif (self.varDic[key] == 'int'):
                 self.cDic[key] = self.c_cnt
                 self.c_cnt = self.c_cnt + 1
+            elif (self.varDic[key] == 'qtuple'):
+                self.qDic[key] = self.qt_cnt
+                self.qt_cnt += 1
             elif self.varDic[key][0] == 'int':
                 self.cDic[key] = self.c_cnt
                 tt = T.cast(int, self.varDic[key][1])
                 self.c_cnt = self.c_cnt + tt
             elif self.varDic[key][0] == 'qbit':
                 self.qDic[key] = self.q_cnt
                 tt = T.cast(int, self.varDic[key][1])
                 self.q_cnt = self.q_cnt + tt
-    
+            elif self.varDic[key][0] == 'qtuple':
+                self.qDic[key] = self.qt_cnt
+                tt = T.cast(int, self.varDic[key][1])
+                self.qt_cnt += tt
+        if self.q_cnt > self.qnum: ErrorThrow(f'qubit number can not be greater than {self.qnum}!')
+        if self.qt_cnt > self.qnum + len(self.tuple): ErrorThrow(f'qtuple number can not be greater than {len(self.tuple)}!')
+        
     def queryVariable(self, name: VarKey)-> T.Optional[VarType]:
         localparas = self.localVarDic.get(self.proc_key)
         if(localparas!=None and name in localparas):
             return localparas[name]
         else:
             return self.varDic.get(name)
     
@@ -651,45 +721,52 @@
             offset = q[1]
         index = self.qDic.get(qid)
         if(index==None):
             ICE("bad variable")
         index += offset
         return "Q{:0>2d}".format(index+1)
 
-    def get_qop(self, gate, qbit, param):
+    def get_qop(self, gate, qbit, param, pos):
         
         if self.target == 'openqasm':
+            if gate == 'RXY':
+                ErrorThrow(f'openqasm can not support RXY, please decompose first')
             s = self.openqasm_gate[gate]
             if gate == 'M':
-                s += f' q[{int(qbit[0])-1}] -> c[{self.m_cnt}]'
+                s += f' q[{int(qbit[0])}] -> c[{self.m_cnt}]'
                 self.m_cnt += 1
             else:
                 if gate in ['RX', 'RY', 'RZ']:
                     s += f'({param[0]})'
                 
                 if gate in ['CNOT', 'CX', 'CY', 'CZ']:
                     s += f' q[{int(qbit[0])-1}], q[{int(qbit[1])-1}]'
                 else:
                     s += f' q[{int(qbit[0])-1}]'
             return s+';'
         else:
+            qbit = [str(int(q)+1) for q in qbit]
             s = gate
             if gate in ['CNOT', 'CX', 'CY', 'CZ']:
+                if self.hardware:
+                    if (qbit[0] not in self.topo) or (qbit[1] not in self.topo[qbit[0]]):
+                        ErrorThrow("in line {}, CZ can only operate adjacent qubit. [{}, {}] not adjacent\n".format(pos, qbit[0], qbit[1]))
                 s = f"{gate} Q{qbit[0]} Q{qbit[1]}"
             else:    
                 for q in qbit:
                     s += f' Q{q}'
                 if param:
-                    s += f' {param[0]}'
+                    for p in param:
+                        s += f' {p}'
             return s
 
     def print(self, val, pos):
 
         gate = val[0][0]
-        theta = 0.0
+        phi, theta = 0.0, 0.0
         if len(val[0]) == 2:
             t, f = val[0][1]
             try:
                 if f:
                     theta = self.evaluateTheta(t)
                 else:
                     if t not in self.lamb:
@@ -699,14 +776,37 @@
                     #theta = eval(self.lamb[val[0][1]], self.param)
                     theta %= 4*np.pi
                     if theta > 2*np.pi: theta -= 4*np.pi
                     # theta /= 2
                     # theta= round(theta,4)
             except Exception as e:
                 ErrorThrow('in line {}, expression calc error: {}'.format(pos, str(e)))
+        elif len(val[0]) == 3:
+            t1, f1 = val[0][1]
+            t2, f2 = val[0][2]
+            try:
+                if f1:
+                    phi = self.evaluateTheta(t1)
+                else:
+                    if t1 not in self.lamb:
+                        self.lamb[t1] = eval("lambda {}:{}".format("args", t1), self.param)
+                    phi = self.lamb[t1](self.for_val)
+                    phi %= 2*np.pi
+                    if phi > np.pi: phi -= 2*np.pi
+
+                if f2:
+                    theta = self.evaluateTheta(t2)
+                else:
+                    if t2 not in self.lamb:
+                        self.lamb[t2] = eval("lambda {}:{}".format("args", t2), self.param)
+                    theta = self.lamb[t2](self.for_val)
+                    theta %= 4*np.pi
+                    if theta > 2*np.pi: theta -= 4*np.pi
+            except Exception as e:
+                ErrorThrow('in line {}, expression calc error: {}'.format(pos, str(e)))
 
         qlist = []
         try:
             for q in val[1]:
                 if q[1] == 0:
                     qlist.append([0])
                 else:  
@@ -725,15 +825,15 @@
         for i in range(len(qlist[0])):
             qbit = []
             for id in range(gateq_cnt):
 
                 offset=qlist[id][i]
                 if not isinstance(offset, int):
                     ErrorThrow('in line {}, index need int'.format(pos))
-                qid = "{}".format(val[1][id][2]+offset+1)    
+                qid = "{}".format(val[1][id][2]+offset)    
                 
                 if val[1][id][1] > 0 and offset >= val[1][id][1]:
                     ThrowArrayOutOfBound(self.error_pos(), offset, val[1][id][0], val[1][id][1])
 
                 if qid in self.measured_qubits:
                     if val[1][id][1] == 0:
                         ThrowAlreadyMeasured(self.error_pos(), val[1][id][0])
@@ -741,30 +841,43 @@
                         ThrowAlreadyMeasured(self.error_pos(), val[1][id][0], offset)    
                 qbit.append(qid)
 
             if(len(set(qbit))!=len(qbit)):
                 ThrowDuplicateQubit(self.error_pos())
 
             if gate in self.gateset:
+                if gate in ['H','X','Y','Z','S','T', 'RX', 'RY', 'RZ', 'SD', 'TD', 'X2M', 'X2P', 'Y2M', 'Y2P', 'RXY','M']:
+                    if int(qbit[0]) >= self.qnum: ErrorThrow(f'in line {pos}, {gate} can not be used on qubits')
+                else:
+                    if len(qbit) == 2:
+                       if int(qbit[0]) >= self.qnum or int(qbit[1]) >= self.qnum: ErrorThrow(f'in line {pos}, {gate} should be used on a qtuple or two qubits')
+                    elif len(qbit) == 1:
+                        if int(qbit[0]) < self.qnum: ErrorThrow(f'in line {pos}, {gate} should be used on a qtuple or two qubits')
+                        if qbit[0] not in self.tuple: ErrorThrow(f'in line {pos}, tuple {qbit[0]} is not support, please check your backend config')
+                        qbit = list(self.tuple[qbit[0]])
                 s = gate
                 param = []
                 if gate in ['RX', 'RY', 'RZ']:
                     param.append(theta)
-
-                self.no_indent_out_append(self.get_qop(s, qbit, param))
+                elif gate == 'RXY':
+                    param = [phi, theta]
+                self.no_indent_out_append(self.get_qop(s, qbit, param, pos))
                 if gate == 'M':
                     self.measured_qubits.add(qbit[0])
             else:
+                for q in qbit:
+                    if int(q) > 65 : ErrorThrow(f'in line {s.pos}, {gate} can not be used on qtuple')
+
                 gateInfo = self.gateDic.get(gate)
                 for g in gateInfo[1]:
                     s = g[0]
                     param = []
                     if g[0] in ['CNOT', 'CX', 'CY', 'CZ']:
                         l,r = T.cast(T.Tuple[int, int], g[2])
                         qbit_g = [qbit[l], qbit[r]]
                     else:
                         l = T.cast(int, g[2])
                         qbit_g = [qbit[l]]
                         if g[0] in ['RX', 'RY', 'RZ']:
                             param = [str(g[1])]
-                    self.no_indent_out_append(self.get_qop(s, qbit_g, param))
+                    self.no_indent_out_append(self.get_qop(s, qbit_g, param, pos))
```

### Comparing `isqopen-1.0.2/isq/compile/qtypes.py` & `isqopen-1.0.3/isq/compile/qtypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 import inspect
 import sys
 
 ProcedureKey = str
 GateKey = str
 VarKey = str
 QbitType = Literal["qbit"]
+QTupleType = Literal["qtuple"]
 IntType = Literal["int"]
 ProcType = Literal["proc"]
 GateType = Tuple[Literal["gate"], bool]
 ArrayType = Tuple["VarType", int]
-VarType = Union[QbitType, IntType, ProcType, GateType, ArrayType]
+VarType = Union[QbitType, QTupleType, IntType, ProcType, GateType, ArrayType]
 RegisterId = int
 
 DecomposedGate = Tuple[str, float, Union[int, Tuple[int, int]]]
 
 def is_int(ty: VarType)->bool:
     return ty=="int"
 def is_qbit(ty: VarType)->bool:
-    return ty=="qbit"
+    return ty=="qbit" or ty == 'qtuple'
 def is_proc(ty: VarType)->bool:
     return ty=="proc"
 def is_array(ty: VarType, elm: T.Optional[VarType] = None)->bool:
     if(not isinstance(ty, list) and not isinstance(ty, tuple)):
         return False
     if(not isinstance(ty[1], int)):
         return False
```

### Comparing `isqopen-1.0.2/isq/compile/tokrules.py` & `isqopen-1.0.3/isq/compile/tokrules.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,15 +51,16 @@
     #'to' : 'TO',
     #'while' : 'WHILE',
     #'do'  :  'DO',
     #'od'  :  'OD',
     'procedure' : 'PROCEDURE',
     #'local' : 'LOCAL',
     'main' : 'MAIN',
-    #'int' : 'INT',
+    'var': "VAR",
+    'qcouple': "QCOUPLE",
     'qbit' : 'QBIT',
     'H' : 'H',
     'X' : 'X',
     'Y' : 'Y',
     'Z' : 'Z',
     'S' : 'S',
     'T' : 'T',
@@ -72,14 +73,15 @@
     'CNOT': 'CNOT',
     'TD': 'TD',
     'SD': 'SD',
     'X2P': 'X2P',
     'X2M': 'X2M',
     'Y2P': 'Y2P',
     'Y2M': 'Y2M',
+    'RXY': 'RXY',
     'M' : 'M',
     'defgate' : 'DEFGATE'
     #'print' : 'PRINT',
     #'multipleGate' : 'MULTIPLEGATE',
     #'..' : 'RANGE'
     }
```

### Comparing `isqopen-1.0.2/isq/compile/tools.py` & `isqopen-1.0.3/isq/compile/tools.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/device/device.py` & `isqopen-1.0.3/isq/device/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from isq.config import debug_mode
 from isq.simulate.simulator import simulate, getprobs
 import random
 from isq.quantum import quantumCor
 from .translate import translate_to_aws, translate_to_qcis, split_rotation_gates
 from .task import *
 from .grad import optv
-from isq.draw.drawer import Drawer
 import logging
-from isq.globalVar import isq_env
+from isq.globalVar import isq_env, msgDic
 
 try:
     from ezQpy import *
     isq_env.set_env('qcis', True)
 except:
     pass
 
@@ -28,20 +27,21 @@
     s = ""
     for _ in range(10):
         s += chr(random.randint(97, 122))
     return s
 
 class Device(ABC):
 
-    def __init__(self, name, shots = 1000, max_wait_time = 600, logger=logging.getLogger(__name__)):
+    def __init__(self, name, shots = 1000, max_wait_time = 600, hardware = None, logger=logging.getLogger(__name__)):
         self._name = name
         self._shots = shots
         self._max_wait_time = max_wait_time
         self._ir = ''
         self.logger = logger
+        self.hardware = hardware
         pass
 
     @abstractmethod
     def run(self, isq_str = '', file = None,  **kwargs):
         pass
 
     def get_ir(self):
@@ -52,31 +52,31 @@
         args, kw = self.getargs(kwargs)
         kw.update(args)
         if file:
             with open(file, 'r') as f:
                 isq_str = f.read()
 
         ir = IR()
-        res = compile(ir, isq_str, target, quantumCor.getGate(), kw)
-        if res == -1: raise CoreError(ir.error)
+        res = compile(ir, isq_str, target, quantumCor.getGate(), self.hardware, kw)
+        if res == -1: raise CoreError(f'{msgDic[ir.code]}:{ir.msg}')
         res_ir = ir.out
         if target == 'qcis':
             res_ir = translate_to_qcis(res_ir)
         return res_ir
     
     def compile_with_par(self, isq_str = '', file = None, target = 'isq', **kwargs):
 
         args, kw = self.getargs(kwargs)
         if file:
             with open(file, 'r') as f:
                 isq_str = f.read()
         
         ir = IR()
-        res = compile(ir, isq_str, target, quantumCor.getGate(), kw, args)
-        if res == -1: raise CoreError(ir.error)
+        res = compile(ir, isq_str, target, quantumCor.getGate(), self.hardware, kw, args)
+        if res == -1: raise CoreError(f'{msgDic[ir.code]}:{ir.msg}')
         self._ir = ir.out
         return args
 
     def simulate(self, ir):
         return dict(simulate(ir, self._shots))
     
     def getargs(self, kwargs):
@@ -86,14 +86,15 @@
             if isinstance(v, optv):
                 args[k] = v._value
                 v = v._value
             kw[k] = v
         return args, kw
     
     def draw_circuit(self, showparam=False):
+        from isq.draw.drawer import Drawer
         if self._ir:
             dw = Drawer(showparam=showparam)
             dw.plot(self._ir)
 
     @property
     def shots(self):
         return self._shots
@@ -101,17 +102,17 @@
     @property
     def max_wait_time(self):
         return self._max_wait_time
         
 
 class LocalDevice(Device):
 
-    def __init__(self, shots = 100, max_wait_time = 60, name = None, mode = 'fast', logger=logging.getLogger(__name__)):
+    def __init__(self, shots = 100, max_wait_time = 60, name = None, mode = 'fast', hardware=None, logger=logging.getLogger(__name__)):
         if name == None: name = "local_device"
-        super().__init__(name, shots, max_wait_time, logger)
+        super().__init__(name, shots, max_wait_time, hardware, logger)
         
         if mode not in ['normal', 'fast']:
             raise CoreError('"{}" simulate mode is not support, only ["fast", "normal"]'.format(mode))
         self._mode = mode
 
 
     def run(self, isq_str = '', file = None, **kwargs):
@@ -137,22 +138,23 @@
     def __init__(
         self,
         login_key = None,
         machine_name = None,
         shots = 1000,
         max_wait_time = 60,
         name = None,
+        hardware = None,
         logger=logging.getLogger(__name__),
     ):
         if name == None: name = "qcis_device"
         
         if not isq_env.get_env('qcis'):
             raise Exception("ezQpy is not supported in this env, please install ezQpy first")
 
-        super().__init__(name, shots, max_wait_time, logger)
+        super().__init__(name, shots, max_wait_time, hardware, logger)
 
         self._account = Account(login_key=login_key, machine_name=machine_name)
         self._qid = 0
     
     def run(
         self,
         isq_str = '',
```

### Comparing `isqopen-1.0.2/isq/device/grad.py` & `isqopen-1.0.3/isq/device/grad.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/device/task.py` & `isqopen-1.0.3/isq/device/task.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/device/translate.py` & `isqopen-1.0.3/isq/device/translate.py`

 * *Files 17% similar despite different names*

```diff
@@ -113,16 +113,37 @@
     return circuit, q_measure
 
 
 def split_rotation_gates(qir):
     ir_list = qir.split("\n")
     ir_list_copy = ir_list.copy()
     for i, ir in enumerate(ir_list):
-        if any([ir.startswith("RX"), ir.startswith("RY"), ir.startswith("RZ")]):
+        if ir.startswith("RXY"):
+            ir_list_copy_list = ir_list_copy[i].split()
+            if float(ir_list_copy_list[3]) > pi or float(ir_list_copy_list[3]) < -pi:
+                q, phi, theta = ir_list_copy_list[1], float(ir_list_copy_list[2]), float(ir_list_copy_list[3])
+                decompose = []
+                phi1 = pi / 2 - phi
+                if abs(phi1) > pi:
+                    decompose.append(f"RZ {q} {phi1/2}")
+                    decompose.append(f"RZ {q} {phi1/2}")
+                else: decompose.append(f"RZ {q} {phi1}")
+                decompose.append(f"X2P {q}")
+                decompose.append(f"RZ {q} {theta / 2}")
+                decompose.append(f"RZ {q} {theta / 2}")
+                decompose.append(f"X2M {q}")
+                phi2 = phi - pi / 2
+                if abs(phi2) > pi:
+                    decompose.append(f"RZ {q} {phi2/2}")
+                    decompose.append(f"RZ {q} {phi2/2}")
+                else: decompose.append(f"RZ {q} {phi2}")
+                ir_list_copy[i] = "\n".join(decompose)
+        elif any([ir.startswith("RX"), ir.startswith("RY"), ir.startswith("RZ")]):
             ir_list_copy_list = ir_list_copy[i].split()
             if float(ir_list_copy_list[2]) > pi or float(ir_list_copy_list[2]) < -pi:
                 ir_list_copy_list_new = ir_list_copy_list.copy()
                 ir_list_copy_list_new[2] = str(float(ir_list_copy_list[2]) / 2)
                 ir_list_copy_new = " ".join(ir_list_copy_list_new)
                 new_str = ir_list_copy_new + "\n" + ir_list_copy_new
                 ir_list_copy[i] = new_str
+
     return "\n".join(ir_list_copy)
```

### Comparing `isqopen-1.0.2/isq/draw/drawer.py` & `isqopen-1.0.3/isq/draw/drawer.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/errors.py` & `isqopen-1.0.3/isq/errors.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/mapping.py` & `isqopen-1.0.3/isq/mapping.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/quantum.py` & `isqopen-1.0.3/isq/quantum.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/isq/simulate/operation.py` & `isqopen-1.0.3/isq/simulate/operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,25 @@
         return jnp.array([[jnp.exp(-1j*theta),0],[0,jnp.exp(1j*theta)]], dtype=complex)
     elif np_mod == 2:
         theta_ = torch.div(theta, 2).reshape(-1)
         return torch.cat((torch.exp(-1j*theta_),torch.zeros(1),torch.zeros(1),torch.exp(1j*theta_))).reshape(2, 2).type(torch.cfloat)
     if np_mod == 0:
         theta /= 2
         return anp.array([[anp.exp(-1j*theta),0],[0,anp.exp(1j*theta)]], dtype=complex)
+def RXY(phi, theta):
+    if np_mod == 1:
+        theta /= 2
+        return jnp.array([[jnp.cos(theta), -1j*jnp.exp(-1j*phi)*jnp.sin(theta)],[-1j*jnp.exp(1j*phi)*jnp.sin(theta),jnp.cos(theta)]], dtype=complex)
+    elif np_mod == 2:
+        phi_ = torch.div(theta, 1).reshape(-1)
+        theta_ = torch.div(theta, 2).reshape(-1)
+        return torch.cat((torch.cos(theta_), -1j*torch.exp(-1j*phi_)*torch.sin(theta_), -1j*torch.exp(1j*phi_)*torch.sin(theta_), torch.cos(theta_))).reshape(2, 2).type(torch.cfloat)
+    if np_mod == 0:
+        theta /= 2
+        return anp.array([[anp.cos(theta), -1j*anp.exp(-1j*phi)*anp.sin(theta)],[-1j*anp.exp(1j*phi)*anp.sin(theta),anp.cos(theta)]], dtype=complex)
 def X2P():
     if np_mod == 1: return jnp.sqrt(2)/2 * jnp.array([[1, -1j], [-1j, 1]], dtype=complex)
     elif np_mod == 2: return torch.sqrt(torch.tensor(2))/2 * torch.tensor([[1, -1j], [-1j, 1]], dtype=torch.cfloat)
     return anp.sqrt(2)/2 * anp.array([[1, -1j], [-1j, 1]], dtype=complex)
 def X2M():
     if np_mod == 1: return jnp.sqrt(2)/2 * jnp.array([[1, 1j], [1j, 1]], dtype=complex)
     elif np_mod == 2: return torch.sqrt(torch.tensor(2))/2 * torch.tensor([[1, 1j], [1j, 1]], dtype=torch.cfloat)
@@ -143,20 +154,22 @@
     elif np_mod == 2: return torch.ravel(state)
     return anp.ravel(state)
 
 
 def single_rotate_gate(state, gate, qnum, target, theta):
     state = reshape_single(state, qnum, target)
     if gate == 'RX':
-        state = RX(theta) @ state[:,]
+        state = RX(theta[0]) @ state[:,]
     elif gate == 'RY':
-        state = RY(theta) @ state[:,]
+        state = RY(theta[0]) @ state[:,]
     elif gate == 'RZ':
-        state = RZ(theta) @ state[:,]
-    
+        state = RZ(theta[0]) @ state[:,]
+    elif gate == 'RXY':
+        state = RXY(theta[0], theta[1]) @ state[:,]
+        
     if np_mod == 1: return jnp.ravel(state)
     elif np_mod == 2: return torch.ravel(state)
     return anp.ravel(state)
 
 def multi_gate(state, gate, qnum, ctrl, target):
     if ctrl < target:
         state = reshape_double(state, qnum, ctrl, target)
```

### Comparing `isqopen-1.0.2/isq/simulate/simulator.py` & `isqopen-1.0.3/isq/simulate/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from autograd import numpy as anp
 import time
 from isq.errors import *
 from collections import defaultdict
 from .operation import *
 from isq.globalVar import isq_env
 
-gate_list = ['H', 'X', 'Y', 'Z', 'S', 'T', 'RZ', 'RX', 'RY', 'SD', 'TD', 'X2M', 'X2P', 'Y2M', 'Y2P', 'CZ', 'CY', 'CX', 'CNOT', 'M']
+gate_list = ['H', 'X', 'Y', 'Z', 'S', 'T', 'RZ', 'RX', 'RY', 'SD', 'TD', 'X2M', 'X2P', 'Y2M', 'Y2P', 'CZ', 'CY', 'CX', 'CNOT', 'M', 'RXY']
 
 def check(line_data):
     
     qdic = {}
     qnum = 0
     for idx, line in enumerate(line_data):
         line = line.strip()
         if not line:
             continue
         strArr = line.split(' ')
         if strArr[0] not in gate_list:
             raise CoreError('simulate error: in line {}, gate error'.format(idx))
-        if len(strArr) < 2 or len(strArr) > 3:
+        if len(strArr) < 2 or len(strArr) > 4:
             raise CoreError('simulate error: in line {}, qbit number error'.format(idx))
         if strArr[1][0] != 'Q' or not strArr[1][1:].isdigit():
             raise CoreError('simulate error: in line {}, qbit syntax error'.format(idx))
 
         if strArr[1] not in qdic:
             qdic[strArr[1]] = qnum
             qnum += 1
@@ -38,15 +38,17 @@
 
             if strArr[2] not in qdic:
                 qdic[strArr[2]] = qnum
                 qnum += 1
         if strArr[0] in ['RX', 'RY', 'RZ']:
             if len(strArr) != 3:
                 raise CoreError('simulate error: in line {}, qbit number error'.format(idx))
-    
+        if strArr[0] == 'RXY':
+            if len(strArr) != 4:
+                raise CoreError('simulate error: in line {}, qbit number error'.format(idx))
     if qnum > 22:
         raise CoreError('simulate error: qbit number out of 22, can not simulate')
 
     return qnum, qdic
 
 def getstate(line_data, qnum, qdic, mod, **kwargs):
 
@@ -75,16 +77,19 @@
         qid1 = qdic[strArr[1]]
         if strArr[0] == 'M':
             mq.append(qid1)
         else:
             if strArr[0] in ['CZ','CY','CX','CNOT']:
                 qid2 = qdic[strArr[2]]
                 state = multi_gate(state, strArr[0], qnum, qid1, qid2)
-            elif strArr[0] in ['RX', 'RY', 'RZ']:
-                state = single_rotate_gate(state, strArr[0], qnum, qid1, eval(strArr[2], kwargs))
+            elif strArr[0] in ['RX', 'RY', 'RZ', 'RXY']:
+                theta = []
+                for v in strArr[2:]:
+                    theta.append(eval(v, kwargs))
+                state = single_rotate_gate(state, strArr[0], qnum, qid1, theta)
             else:
                 state = single_gate(state, strArr[0], qnum, qid1)
     
     return state, mq
 
 def simulate(data, run_time = 100, fast = False, mod = 0):
```

### Comparing `isqopen-1.0.2/isqopen.egg-info/PKG-INFO` & `isqopen-1.0.3/isqopen.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isqopen
-Version: 1.0.2
+Version: 1.0.3
 Summary: isq quantum kernel
 Author: Lou Huazhe
 Author-email: louhz@arclightquantum.com
 Platform: python 3.8+
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `isqopen-1.0.2/isqopen.egg-info/SOURCES.txt` & `isqopen-1.0.3/isqopen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.2/setup.py` & `isqopen-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "isqopen",
-    version = "1.0.2",
+    version = "1.0.3",
     keyword = {"isq", "quantum", "cor"},
     description = "isq quantum kernel",
     platforms='python 3.8+',
     long_description=long_description,
 	long_description_content_type="text/markdown",
     author = "Lou Huazhe",
     author_email = "louhz@arclightquantum.com",
```

