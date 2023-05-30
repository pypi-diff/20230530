# Comparing `tmp/xdeps-0.0.9.tar.gz` & `tmp/xdeps-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdeps-0.0.9.tar", last modified: Sat Sep 17 13:34:40 2022, max compression
+gzip compressed data, was "xdeps-0.1.0.tar", last modified: Tue May 30 19:19:39 2023, max compression
```

## Comparing `xdeps-0.0.9.tar` & `xdeps-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-09-17 13:34:40.477910 xdeps-0.0.9/
--rw-r--r--   0 giadarol   (501) staff       (20)      561 2022-09-17 13:34:40.477551 xdeps-0.0.9/PKG-INFO
--rw-r--r--   0 giadarol   (501) staff       (20)       38 2022-09-17 13:34:40.478091 xdeps-0.0.9/setup.cfg
--rw-r--r--   0 giadarol   (501) staff       (20)      984 2022-09-17 13:34:23.000000 xdeps-0.0.9/setup.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-09-17 13:34:40.474830 xdeps-0.0.9/xdeps/
--rw-r--r--   0 giadarol   (501) staff       (20)      236 2022-06-09 08:10:13.000000 xdeps-0.0.9/xdeps/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)     4950 2022-06-09 08:10:13.000000 xdeps-0.0.9/xdeps/madxutils.py
--rw-r--r--   0 giadarol   (501) staff       (20)    18677 2022-09-17 09:53:49.000000 xdeps-0.0.9/xdeps/refs.py
--rw-r--r--   0 giadarol   (501) staff       (20)     2071 2022-06-09 08:10:13.000000 xdeps-0.0.9/xdeps/sorting.py
--rw-r--r--   0 giadarol   (501) staff       (20)    11429 2022-09-17 09:53:49.000000 xdeps-0.0.9/xdeps/tasks.py
--rw-r--r--   0 giadarol   (501) staff       (20)      926 2022-06-09 08:10:13.000000 xdeps-0.0.9/xdeps/utils.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-09-17 13:34:40.477104 xdeps-0.0.9/xdeps.egg-info/
--rw-r--r--   0 giadarol   (501) staff       (20)      561 2022-09-17 13:34:40.000000 xdeps-0.0.9/xdeps.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (501) staff       (20)      250 2022-09-17 13:34:40.000000 xdeps-0.0.9/xdeps.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (501) staff       (20)        1 2022-09-17 13:34:40.000000 xdeps-0.0.9/xdeps.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (501) staff       (20)        5 2022-09-17 13:34:40.000000 xdeps-0.0.9/xdeps.egg-info/requires.txt
--rw-r--r--   0 giadarol   (501) staff       (20)        6 2022-09-17 13:34:40.000000 xdeps-0.0.9/xdeps.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:19:39.649571 xdeps-0.1.0/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:37.000000 xdeps-0.1.0/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-05-30 19:19:39.649420 xdeps-0.1.0/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-05-30 19:19:39.649618 xdeps-0.1.0/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1253 2023-03-23 11:04:37.000000 xdeps-0.1.0/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:19:39.644337 xdeps-0.1.0/xdeps/
+-rw-r--r--   0 giadarol   (503) staff       (20)      391 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-05-30 19:19:10.000000 xdeps-0.1.0/xdeps/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/general.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5506 2023-04-05 12:43:31.000000 xdeps-0.1.0/xdeps/madxutils.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:19:39.649187 xdeps-0.1.0/xdeps/optimize/
+-rw-r--r--   0 giadarol   (503) staff       (20)      118 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/optimize/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3511 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/optimize/jacobian.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    11173 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/optimize/optimize.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    21520 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/refs.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2093 2023-04-05 12:43:31.000000 xdeps-0.1.0/xdeps/sorting.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    14604 2023-05-23 20:23:29.000000 xdeps-0.1.0/xdeps/tasks.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      932 2023-04-05 12:43:31.000000 xdeps-0.1.0/xdeps/utils.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:19:39.648398 xdeps-0.1.0/xdeps.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      374 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       21 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/top_level.txt
```

### Comparing `xdeps-0.0.9/PKG-INFO` & `xdeps-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: xdeps
-Version: 0.0.9
+Version: 0.1.0
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
+Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
-Download-URL: https://pypi.python.org/pypi/xdeps
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Documentation, https://xsuite.readthedocs.io/
 Project-URL: Source Code, https://github.com/xsuite/xdeps
-Description: Data dependency manager
-        
-        This package is part of the Xsuite collection.
-Platform: UNKNOWN
+Provides-Extra: tests
+License-File: LICENSE
+
+Data dependency manager
+
+This package is part of the Xsuite collection.
```

### Comparing `xdeps-0.0.9/setup.py` & `xdeps-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # copyright ############################### #
 # This file is part of the Xdeps Package.   #
 # Copyright (c) CERN, 2021.                 #
 # ######################################### #
 
 from setuptools import setup, find_packages
+from pathlib import Path
+
+version_file = Path(__file__).parent / 'xdeps/_version.py'
+dd = {}
+with open(version_file.absolute(), 'r') as fp:
+    exec(fp.read(), dd)
+__version__ = dd['__version__']
 
 setup(
         name='xdeps',
-        version='0.0.9',
+        version=__version__,
         description='Data dependency manager',
         long_description=("Data dependency manager\n"
                          "\nThis package is part of the Xsuite collection."),
         author='Riccardo De Maria',
         author_email='riccardo.de.maria@cern.ch',
         packages=find_packages(),
         install_requires=['lark'],
@@ -19,8 +26,11 @@
         license='Apache 2.0',
         download_url="https://pypi.python.org/pypi/xdeps",
         project_urls={
             "Bug Tracker": "https://github.com/xsuite/xsuite/issues",
             "Documentation": 'https://xsuite.readthedocs.io/',
             "Source Code": "https://github.com/xsuite/xdeps",
         },
+        extras_require={
+            'tests': ['pytest'],
+        },
 )
```

### Comparing `xdeps-0.0.9/xdeps/madxutils.py` & `xdeps-0.1.0/xdeps/madxutils.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,143 +29,164 @@
          | "-" atom         -> neg
          | "+" atom         -> pos
          | NAME             -> var
          | NAME "->" NAME   -> getitem
          | NAME "(" sum ("," sum)* ")" -> call
          | "(" sum ")"
 
-    NAME: /[a-z_\.][a-z0-9_\.%]*/
+    NAME: /[a-z_\\.][a-z0-9_\\.%]*/
     %import common.NUMBER
     %import common.WS_INLINE
     %ignore WS_INLINE
 """
 
+
 @v_args(inline=True)
 class MadxEval(Transformer):
     from operator import add, sub, mul, truediv as div
     from operator import neg, pos, pow
+
     number = float
 
-    def __init__(self,variables,functions,elements,get='item'):
+    def __init__(self, variables, functions, elements, get="item"):
+        """
+        variables: dict of variables
+        elements: dict of elements
+        functions: module of functions such as `math` or `numpy`
+
+        get: 'item' if items in elements support el['key'], 'attr' if they support el.key
+        """
         self.variables = variables
         self.functions = functions
-        self.elements  = elements
-        grammar=calc_grammar
-        if get == 'attr':
-            grammar=grammar.replace('getitem','getattr')
-        self.eval=Lark(grammar, parser='lalr',
-                         transformer=self).parse
+        self.elements = elements
+        grammar = calc_grammar
+        if get == "attr":
+            grammar = grammar.replace("getitem", "getattr")
+        self.eval = Lark(grammar, parser="lalr", transformer=self).parse
 
     def assign_var(self, name, value):
         self.variables[name] = value
         return value
 
-    def call(self,name,*args):
-        ff=getattr(self.functions,name)
+    def call(self, name, *args):
+        ff = getattr(self.functions, name)
         return ff(*args)
 
-    def getitem(self,name,key):
-        return self.elements[name[1]][key]
+    def getitem(self, name, key):
+        return self.elements[name.value][key.value]
 
-    def getattr(self,name,key):
-        return getattr(self.elements[name[1]],key)
+    def getattr(self, name, key):
+        return getattr(self.elements[name], key)
 
     def var(self, name):
         try:
             return self.variables[name.value]
         except KeyError:
             raise Exception("Variable not found: %s" % name)
 
+
 def test():
     import math
     from collections import defaultdict
-    madx=MadxEval(defaultdict(lambda :0),{},math)
+
+    madx = MadxEval(defaultdict(lambda: 0), math, {})
     print(madx.eval("+1+2^-2"))
     print(madx.eval("a.b"))
     print(madx.eval("1+a.b*-3"))
     print(madx.eval("sin(3)^2"))
 
 
 class Mix:
-    __slots__=('_v','_r')
-    def __init__(self,data,refs):
-        object.__setattr__(self,'_v',data)
-        object.__setattr__(self,'_r',refs)
+    __slots__ = ("_v", "_r")
+
+    def __init__(self, data, refs):
+        object.__setattr__(self, "_v", data)
+        object.__setattr__(self, "_r", refs)
 
-    def __getattr__(self,key):
+    def __getattr__(self, key):
         return self._v[key]
 
-    def __getitem__(self,key):
+    def __getitem__(self, key):
         return self._v[key]
 
-    def __setattr__(self,key,value):
-        self._r[key]=value
+    def __setattr__(self, key, value):
+        self._r[key] = value
 
-    def __setitem__(self,key,value):
-        self._r[key]=value
+    def __setitem__(self, key, value):
+        self._r[key] = value
 
-    def _eval(self,expr):
+    def _eval(self, expr):
         return self._r._eval(expr)
 
+
 class MadxEnv:
-    def __init__(self,mad=None):
-        self._variables=defaultdict(lambda :0)
-        self._elements={}
-        self.manager=Manager()
-        self._vref=self.manager.ref(self._variables,'v')
-        self._eref=self.manager.ref(self._elements,'e')
-        self._fref=self.manager.ref(math,'f')
-        self.madexpr=MadxEval(self._vref,self._fref,self._eref).eval
-        self.madeval=MadxEval(self._variables,math,self._elements).eval
-        self.v=Mix(self._variables,self._vref)
-        self.e=Mix(self._elements,self._eref)
+    def __init__(self, mad=None):
+        self._variables = defaultdict(lambda: 0)
+        self._elements = {}
+        self.manager = Manager()
+        self._vref = self.manager.ref(self._variables, "v")
+        self._eref = self.manager.ref(self._elements, "e")
+        self._fref = self.manager.ref(math, "f")
+        self.madexpr = MadxEval(self._vref, self._fref, self._eref).eval
+        self.madeval = MadxEval(self._variables, math, self._elements).eval
+        self.v = Mix(self._variables, self._vref)
+        self.e = Mix(self._elements, self._eref)
         if mad is not None:
-           self.read_state(mad)
+            self.read_state(mad)
 
     def dump(self):
-        return {'variables':self._variables,
-             'elements':self._elements,
-             'xdeps':self.manager.dump()}
-
-    def load(self,data):
-        self._variables.update(data['variables'])
-        self._elements.update(data['elements'])
-        self.manager.load(data['xdeps'])
+        return {
+            "variables": self._variables,
+            "elements": self._elements,
+            "xdeps": self.manager.dump(),
+        }
+
+    def load(self, data):
+        self._variables.update(data["variables"])
+        self._elements.update(data["elements"])
+        self.manager.load(data["xdeps"])
 
-    def to_json(self,filename):
+    def to_json(self, filename):
         import json
-        json.dump(self.dump(),open(filename,'w'))
+
+        json.dump(self.dump(), open(filename, "w"))
 
     @classmethod
-    def from_json(cls,filename):
+    def from_json(cls, filename):
         import json
-        self=cls()
+
+        self = cls()
         self.load(json.load(open(filename)))
         return self
 
-    def read_state(self,mad):
-        for name,par in mad.globals.cmdpar.items():
+    def read_state(self, mad):
+        elemdata = AttrDict()
+        elem = mad.beam
+        for parname, par in elem.cmdpar.items():
+            elemdata[parname] = par.value
+        self._elements['beam']=elemdata
+
+        for name, par in mad.globals.cmdpar.items():
             if par.expr is None:
-                self._variables[name]=par.value
+                self._variables[name] = par.value
             else:
-                self._vref[name]=self.madexpr(par.expr)
+                self._vref[name] = self.madexpr(par.expr)
 
-        for name,elem in mad.elements.items():
-            elemdata=AttrDict()
+        for name, elem in mad.elements.items():
+            elemdata = AttrDict()
             for parname, par in elem.cmdpar.items():
-                elemdata[parname]=par.value
-            self._elements[name]=elemdata
+                elemdata[parname] = par.value
+            self._elements[name] = elemdata
 
-        for name,elem in mad.elements.items():
+        for name, elem in mad.elements.items():
             for parname, par in elem.cmdpar.items():
                 if par.expr is not None:
-                    if par.dtype==12: # handle lists
-                        for ii,ee in enumerate(par.expr):
+                    if par.dtype == 12:  # handle lists
+                        for ii, ee in enumerate(par.expr):
                             if ee is not None:
-                                self._eref[name][parname][ii]=self.madexpr(ee)
+                                self._eref[name][parname][ii] = self.madexpr(ee)
                     else:
-                        self._eref[name][parname]=self.madexpr(par.expr)
+                        self._eref[name][parname] = self.madexpr(par.expr)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test()
-
```

### Comparing `xdeps-0.0.9/xdeps/refs.py` & `xdeps-0.1.0/xdeps/refs.py`

 * *Files 18% similar despite different names*

```diff
@@ -96,14 +96,17 @@
             return self._get_value(){sy}other"""
         print(fmt)
 
 
 class ARef:
     __slots__ = ()
 
+    def __init__(self, *args, **kwargs):
+        raise ValueError("Cannot instantiate ARef")
+
     @staticmethod
     def _mk_value(value):
         if isinstance(value, ARef):
             return value._get_value()
         else:
             return value
 
@@ -115,178 +118,192 @@
     def __call__(self, *args, **kwargs):
         return CallRef(self, args, kwargs)
 
     def __getitem__(self, item):
         return ItemRef(self, item, self._manager)
 
     def __getattr__(self, attr):
-        if attr.startswith('__array_'): #numpy crashes without
-            #print(self,attr)
+        if attr.startswith("__array_"):  # numpy crashes without
+            # print(self,attr)
             raise AttributeError
+        if attr == '_manager':
+            raise RuntimeError("This should not happen...")
         return AttrRef(self, attr, self._manager)
 
+    # Untested:
+
+    # def __getstate__(self):
+    #     raise ValueError("Cannot pickle ARef")
+
+    # def __setstate__(self, state):
+    #     raise ValueError("Cannot pickle ARef")
+
     # numerical unary  operator
     def __neg__(self):
-        return NegRef(self) # type: ignore
+        return NegRef(self)  # type: ignore
 
     def __pos__(self):
-        return PosRef(self) # type: ignore
+        return PosRef(self)  # type: ignore
 
     def __invert__(self):
-        return InvertRef(self) # type: ignore
- 
+        return InvertRef(self)  # type: ignore
+
     # numerical binary operators
 
     def __add__(self, other):
-        return AddRef(self, other) # type: ignore
- 
+        return AddRef(self, other)  # type: ignore
+
     def __radd__(self, other):
-        return AddRef(other, self) # type: ignore
+        return AddRef(other, self)  # type: ignore
 
     def __sub__(self, other):
-        return SubRef(self, other) # type: ignore
+        return SubRef(self, other)  # type: ignore
 
     def __rsub__(self, other):
-        return SubRef(other, self) # type: ignore
+        return SubRef(other, self)  # type: ignore
 
     def __mul__(self, other):
-        return MulRef(self, other) # type: ignore
+        return MulRef(self, other)  # type: ignore
 
     def __rmul__(self, other):
-        return MulRef(other, self) # type: ignore
+        return MulRef(other, self)  # type: ignore
 
     def __matmul__(self, other):
-        return MatmulRef(self, other) # type: ignore
+        return MatmulRef(self, other)  # type: ignore
 
     def __rmatmul__(self, other):
-        return MatmulRef(other, self) # type: ignore
+        return MatmulRef(other, self)  # type: ignore
 
     def __truediv__(self, other):
-        return TruedivRef(self, other) # type: ignore
+        return TruedivRef(self, other)  # type: ignore
 
     def __rtruediv__(self, other):
-        return TruedivRef(other, self) # type: ignore
+        return TruedivRef(other, self)  # type: ignore
 
     def __floordiv__(self, other):
-        return FloordivRef(self, other) # type: ignore
+        return FloordivRef(self, other)  # type: ignore
 
     def __rfloordiv__(self, other):
-        return FloordivRef(other, self) # type: ignore
+        return FloordivRef(other, self)  # type: ignore
 
     def __mod__(self, other):
-        return ModRef(self, other) # type: ignore
+        return ModRef(self, other)  # type: ignore
 
     def __rmod__(self, other):
-        return ModRef(other, self) # type: ignore
+        return ModRef(other, self)  # type: ignore
 
     def __pow__(self, other):
-        return PowRef(self, other) # type: ignore
+        return PowRef(self, other)  # type: ignore
 
     def __rpow__(self, other):
-        return PowRef(other, self) # type: ignore
+        return PowRef(other, self)  # type: ignore
 
     def __and__(self, other):
-        return AndRef(self, other) # type: ignore
+        return AndRef(self, other)  # type: ignore
 
     def __rand__(self, other):
-        return AndRef(other, self) # type: ignore
+        return AndRef(other, self)  # type: ignore
 
     def __or__(self, other):
-        return OrRef(self, other) # type: ignore
+        return OrRef(self, other)  # type: ignore
 
     def __ror__(self, other):
-        return OrRef(other, self) # type: ignore
+        return OrRef(other, self)  # type: ignore
 
     def __xor__(self, other):
-        return XorRef(self, other) # type: ignore
+        return XorRef(self, other)  # type: ignore
 
     def __rxor__(self, other):
-        return XorRef(other, self) # type: ignore
+        return XorRef(other, self)  # type: ignore
 
     def __lt__(self, other):
-        return LtRef(self, other) # type: ignore
+        return LtRef(self, other)  # type: ignore
 
     def __rlt__(self, other):
-        return LtRef(other, self) # type: ignore
+        return LtRef(other, self)  # type: ignore
 
     def __le__(self, other):
-        return LeRef(self, other) # type: ignore
+        return LeRef(self, other)  # type: ignore
 
     def __rle__(self, other):
-        return LeRef(other, self) # type: ignore
+        return LeRef(other, self)  # type: ignore
 
     def __eq__(self, other):
-        return EqRef(self, other) # type: ignore
+        return EqRef(self, other)  # type: ignore
 
     def __req__(self, other):
-        return EqRef(other, self) # type: ignore
+        return EqRef(other, self)  # type: ignore
 
     def __ne__(self, other):
-        return NeRef(self, other) # type: ignore
+        return NeRef(self, other)  # type: ignore
 
     def __rne__(self, other):
-        return NeRef(other, self) # type: ignore
+        return NeRef(other, self)  # type: ignore
 
     def __ge__(self, other):
-        return GeRef(self, other) # type: ignore
+        return GeRef(self, other)  # type: ignore
 
     def __rge__(self, other):
-        return GeRef(other, self) # type: ignore
+        return GeRef(other, self)  # type: ignore
 
     def __gt__(self, other):
-        return GtRef(self, other) # type: ignore
+        return GtRef(self, other)  # type: ignore
 
     def __rgt__(self, other):
-        return GtRef(other, self) # type: ignore
+        return GtRef(other, self)  # type: ignore
 
     def __rshift__(self, other):
-        return RshiftRef(self, other) # type: ignore
+        return RshiftRef(self, other)  # type: ignore
 
     def __rrshift__(self, other):
-        return RshiftRef(other, self) # type: ignore
+        return RshiftRef(other, self)  # type: ignore
 
     def __lshift__(self, other):
-        return LshiftRef(self, other) # type: ignore
+        return LshiftRef(self, other)  # type: ignore
 
     def __rlshift__(self, other):
-        return LshiftRef(other, self) # type: ignore
+        return LshiftRef(other, self)  # type: ignore
 
     def __divmod__(self, other):
-        return BDivmodRef(self, other) # type: ignore
+        return BDivmodRef(self, other)  # type: ignore
 
     def __pow__(self, other):
-        return PowRef(self, other) # type: ignore
+        return PowRef(self, other)  # type: ignore
 
     def __round__(self, other=0):
-        return BRoundRef(self, other) # type: ignore
+        return BRoundRef(self, other)  # type: ignore
 
     def __trunc__(self, other):
-        return BTruncRef(self, other) # type: ignore
+        return BTruncRef(self, other)  # type: ignore
 
     def __floor__(self, other):
-        return BFloorRef(self, other) # type: ignore
+        return BFloorRef(self, other)  # type: ignore
 
     def __ceil__(self, other):
-        return BCeilRef(self, other) # type: ignore
+        return BCeilRef(self, other)  # type: ignore
 
     def __abs__(self):
-        return BAbsRef(self) # type: ignore
+        return BAbsRef(self)  # type: ignore
 
     def __complex__(self):
-        return BComplexRef(self) # type: ignore
+        return BComplexRef(self)  # type: ignore
 
     def __int__(self):
-        return BIntRef(self) # type: ignore
+        return BIntRef(self)  # type: ignore
 
     def __float__(self):
-        return BFloatRef(self) # type: ignore
+        return BFloatRef(self)  # type: ignore
+
 
 class MutableRef(ARef):
     __slots__ = ()
 
+    def __init__(self, *args, **kwargs):
+        raise ValueError("Cannot instantiate MutableRef")
+
     def __setitem__(self, key, value):
         ref = ItemRef(self, key, self._manager)
         self._manager.set_value(ref, value)
 
     def __setattr__(self, attr, value):
         if attr[0] == "_" and attr in ["_expr", "_exec"]:
             raise ValueError(f"`{attr}` is a special keyword and cannot be assigned.")
@@ -313,48 +330,47 @@
     @property
     def _expr(self):
         if self in self._manager.tasks:
             task = self._manager.tasks[self]
             if hasattr(task, "expr"):
                 return task.expr
 
-    def _info(self,limit=10):
+    def _info(self, limit=10):
         print(f"#  {self}._get_value()")
         try:
-            value=self._get_value()
+            value = self._get_value()
             print(f"   {self} = {value}")
-        except :
+        except:
             print(f"#  {self} has no value")
         print()
 
         if self in self._manager.tasks:
             task = self._manager.tasks[self]
             print(f"#  {self}._expr")
-            print(f"   {task}" )
+            print(f"   {task}")
             print()
-            if hasattr(task,'info'):
+            if hasattr(task, "info"):
                 task.info()
         else:
             print(f"#  {self}._expr is None")
             print()
 
-        refs=self._manager.find_deps([self])[1:]
-        if len(refs)==0:
+        refs = self._manager.find_deps([self])[1:]
+        if len(refs) == 0:
             print(f"#  {self} does not influence any target")
             print()
         else:
             print(f"#  {self}._find_dependant_targets()")
             for tt in refs[:limit]:
                 if tt._expr is not None:
                     print(f"   {tt}")
-            if len(refs)>limit:
+            if len(refs) > limit:
                 print(f"   ... set _info(limit={len(refs)}) to get all lines")
             print()
 
-
     def __iadd__(self, other):
         newexpr = self._expr
         if newexpr:
             return newexpr + other
         else:
             return self._get_value() + other
 
@@ -392,15 +408,15 @@
             return newexpr * other
         else:
             return self._get_value() * other
 
     def __ipow__(self, other):
         newexpr = self._expr
         if newexpr:
-            return newexpr ** other
+            return newexpr**other
         else:
             return self._get_value() ** other
 
     def __irshift__(self, other):
         newexpr = self._expr
         if newexpr:
             return newexpr >> other
@@ -433,14 +449,24 @@
     __slots__ = ("_owner", "_key", "_manager")
 
     def __init__(self, _owner, _key, _manager=None):
         object.__setattr__(self, "_owner", _owner)
         object.__setattr__(self, "_key", _key)
         object.__setattr__(self, "_manager", _manager)
 
+    # Untested:
+
+    # def __getstate__(self):
+    #     return self._owner, self._key, self._manager
+
+    # def __setstate__(self, state):
+    #     object.__setattr__(self, "_owner", state[0])
+    #     object.__setattr__(self, "_key", state[1])
+    #     object.__setattr__(self, "_manager", state[2])
+
     def __hash__(self):
         if isinstance(self._owner, ARef):
             own = self._owner
         else:
             own = id(self._owner)
         return hash((own, self._key))
 
@@ -472,14 +498,24 @@
     __slots__ = ("_owner", "_manager", "_label")
 
     def __init__(self, _owner, _manager=None, _label="_"):
         object.__setattr__(self, "_owner", _owner)
         object.__setattr__(self, "_manager", _manager)
         object.__setattr__(self, "_label", _label)
 
+    # Untested:
+
+    # def __getstate__(self):
+    #     return self._owner, self._manager, self._label
+
+    # def __setstate__(self, state):
+    #     object.__setattr__(self, "_owner", state[0])
+    #     object.__setattr__(self, "_manager", state[1])
+    #     object.__setattr__(self, "_label", state[2])
+
     def __hash__(self):
         return hash(self._label)
 
     def __repr__(self):
         return self._label
 
     def _get_value(self):
@@ -490,14 +526,24 @@
     __slots__ = ("_owner", "_key", "_manager")
 
     def __init__(self, _owner, __key, _manager=None):
         object.__setattr__(self, "_owner", _owner)
         object.__setattr__(self, "_key", __key)
         object.__setattr__(self, "_manager", _manager)
 
+    # Untested:
+
+    # def __getstate__(self):
+    #     return self._owner, self._key, self._manager
+
+    # def __setstate__(self, state):
+    #     object.__setattr__(self, "_owner", state[0])
+    #     object.__setattr__(self, "_key", state[1])
+    #     object.__setattr__(self, "_manager", state[2])
+
     def __hash__(self):
         if isinstance(self._owner, ARef):
             own = self._owner
         else:
             own = id(self._owner)
         return hash((own, self._key))
 
@@ -530,14 +576,25 @@
 
     def __init__(self, _owner, _key, _manager=None, _default=0):
         object.__setattr__(self, "_owner", _owner)
         object.__setattr__(self, "_key", _key)
         object.__setattr__(self, "_manager", _manager)
         object.__setattr__(self, "_default", _default)
 
+    # Untested:
+
+    # def __getstate__(self):
+    #     return self._owner, self._key, self._manager, self._default
+
+    # def __setstate__(self, state):
+    #     object.__setattr__(self, "_owner", state[0])
+    #     object.__setattr__(self, "_key", state[1])
+    #     object.__setattr__(self, "_manager", state[2])
+    #     object.__setattr__(self, "_default", state[3])
+
     def __hash__(self):
         if isinstance(self._owner, ARef):
             own = self._owner
         else:
             own = id(self._owner)
         return hash((own, self._key))
 
@@ -562,27 +619,45 @@
         return out
 
     def __repr__(self):
         return f"{self._owner}[{repr(self._key)}]"
 
 
 class ObjectAttrRef(Ref):
+
+    # Untested:
+
+    # def __getstate__(self):
+    #     return self._manager
+
+    # def __setstate__(self, state):
+    #     object.__setattr__(self, "_manager", state)
+
     def __getattr__(self, attr):
         return ItemDefaultRef(self, attr, self._manager)
 
     def __setattr__(self, attr, value):
         ref = ItemDefaultRef(self, attr, self._manager)
         self._manager.set_value(ref, value)
 
 
 @dataclass(frozen=True)
 class BinOpRef(ARef):
     _a: object
     _b: object
 
+    # Untested:
+
+    # def __getstate__(self):
+    #     return self._a, self._b
+
+    # def __setstate__(self, state):
+    #     object.__setattr__(self, "_a", state[0])
+    #     object.__setattr__(self, "_b", state[1])
+
     def _get_value(self):
         a = ARef._mk_value(self._a)
         b = ARef._mk_value(self._b)
         return self._op(a, b)
 
     def _get_dependencies(self, out=None):
         a = self._a
@@ -599,14 +674,22 @@
         return f"({self._a}{self._st}{self._b})"
 
 
 @dataclass(frozen=True)
 class UnOpRef(ARef):
     _a: object
 
+    # Untested:
+
+    # def __getstate__(self):
+    #     return self._a
+
+    # def __setstate__(self, state):
+    #     object.__setattr__(self, "_a", state)
+
     def _get_value(self):
         a = ARef._mk_value(self._a)
         return self._op(a)
 
     def _get_dependencies(self, out=None):
         a = self._a
         if out is None:
@@ -619,14 +702,22 @@
         return f"({self._st}{self._a})"
 
 
 @dataclass(frozen=True)
 class BuiltinRef(ARef):
     _a: object
 
+    # Untested:
+
+    # def __getstate__(self):
+    #     return self._a
+
+    # def __setstate__(self, state):
+    #     object.__setattr__(self, "_a", state)
+
     def _get_value(self):
         a = ARef._mk_value(self._a)
         return self._op(a)
 
     def _get_dependencies(self, out=None):
         a = self._a
         if out is None:
@@ -641,14 +732,24 @@
 
 @dataclass(frozen=True)
 class CallRef(ARef):
     _func: object
     _args: tuple
     _kwargs: tuple
 
+    # Untested:
+
+    # def __getstate__(self):
+    #     return self._func, self._args, self._kwargs
+
+    # def __setstate__(self, state):
+    #     object.__setattr__(self, "_func", state[0])
+    #     object.__setattr__(self, "_args", state[1])
+    #     object.__setattr__(self, "_kwargs", state[2])
+
     def _get_value(self):
         func = ARef._mk_value(self._func)
         args = [ARef._mk_value(a) for a in self._args]
         kwargs = {n: ARef._mk_value(v) for n, v in self._kwargs}
         return func(*args, **kwargs)
 
     def _get_dependencies(self, out=None):
```

### Comparing `xdeps-0.0.9/xdeps/sorting.py` & `xdeps-0.1.0/xdeps/sorting.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,78 +6,75 @@
 from collections import deque
 
 try:
     from functools import reduce
 except:
     pass
 
+
 def _dfs(graph, source, stack, visited):
     visited.add(source)
 
-    for neighbour in graph.get(source,[]):
+    for neighbour in graph.get(source, []):
         if neighbour not in visited:
             _dfs(graph, neighbour, stack, visited)
 
     stack.appendleft(source)
 
-def toposort(graph,start=None):
+
+def toposort(graph, start=None):
     stack = deque()
     visited = set()
 
     if start is None:
-        start=reduce(set.union, graph.values(),graph.keys())
+        start = reduce(set.union, graph.values(), graph.keys())
 
     for vertex in start:
         if vertex not in visited:
             _dfs(graph, vertex, stack, visited)
 
     return list(stack)
 
+
 def toposort2(graph, start):
     seen = set()
     stack = []
     order = []
-    q=start[:]
+    q = start[:]
     while q:
         v = q.pop()
         if v not in seen:
-            seen.add(v) # no need to append to path any more
-            q.extend(graph.get(v,[]))
-            while stack and v not in graph.get(stack[-1],[]):
-                order.insert(0,stack.pop())
+            seen.add(v)  # no need to append to path any more
+            q.extend(graph.get(v, []))
+            while stack and v not in graph.get(stack[-1], []):
+                order.insert(0, stack.pop())
             stack.append(v)
 
-    return (stack + order)   # new return value!
-
-
+    return stack + order  # new return value!
 
 
 def depsort(deps):
-    data={k: set(v) for k,v in deps.items()}
+    data = {k: set(v) for k, v in deps.items()}
     extra_items_in_deps = reduce(set.union, data.values()) - set(data.keys())
-    data.update({item:set() for item in extra_items_in_deps})
+    data.update({item: set() for item in extra_items_in_deps})
     while True:
-        ordered = set(item for item,dep in data.items() if not dep)
+        ordered = set(item for item, dep in data.items() if not dep)
         if not ordered:
             break
         yield list(ordered)
-        data = {item: (dep - ordered) for item,dep in data.items()
-                if item not in ordered}
+        data = {
+            item: (dep - ordered) for item, dep in data.items() if item not in ordered
+        }
     assert not data, "A cyclic dependency exists amongst %r" % data
 
 
-
 def reverse_graph(dep_graph):
     """
     dep[4]=[3,1] means 4 depends on 3 and 1
     rdep[3]=[4]  means 3 is needed by 4
     rdep[1]=[4]  means 3 is needed by 4
     """
-    rdeps={}
-    for t,deps in dep_graph.items():
+    rdeps = {}
+    for t, deps in dep_graph.items():
         for dd in deps:
-          rdeps.setdefault(dd,[]).append(t)
+            rdeps.setdefault(dd, []).append(t)
     return rdeps
-
-
-
-
```

### Comparing `xdeps-0.0.9/xdeps/tasks.py` & `xdeps-0.1.0/xdeps/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,39 +2,56 @@
 # This file is part of the Xdeps Package.   #
 # Copyright (c) CERN, 2021.                 #
 # ######################################### #
 
 from dataclasses import dataclass, field
 from collections import defaultdict
 import logging
+from copy import deepcopy
 
 from .refs import ARef, Ref, ObjectAttrRef
 from .refs import AttrRef, CallRef, ItemRef
 from .utils import os_display_png, mpl_display_png, ipy_display_png
 from .utils import AttrDict
 from .sorting import toposort
 
 logger = logging.getLogger(__name__)
 
 
+def dct_merge(dct1, dct2):
+    return {**dct1, **dct2}
+
+
+def _check_root_owner(t, ref):
+    if hasattr(t, "_owner"):
+        if t._owner is ref:
+            return True
+        else:
+            return _check_root_owner(t._owner, ref)
+    else:
+        return False
+
+
 class FuncWrapper:
     def __init__(self, func):
         self.func = func
 
     def __call__(self, *args, **kwargs):
         return CallRef(self.func, args, tuple(kwargs.items()))
 
 
 class Task:
     taskid: object
     targets: set
     dependencies: set
+
     def run(self):
         raise NotImplemented
 
+
 class GenericTask(Task):
     taskid: object
     action: object
     targets: set
     dependencies: set
 
     def __repr__(self):
@@ -116,82 +133,89 @@
     deptasks: ref -> all tasks that has ref as dependency
     tartasks: ref -> all tasks that has ref as target
     containers: label -> controlled container
     """
 
     def __init__(self):
         self.tasks = {}
-        self.rdeps = defaultdict(set)
-        self.rtasks = defaultdict(set)
-        self.deptasks = defaultdict(set)
-        self.tartasks = defaultdict(set)
         self.containers = {}
+        self.rdeps = defaultdict(list)
+        self.rtasks = defaultdict(list)
+        self.deptasks = defaultdict(list)
+        self.tartasks = defaultdict(list)
 
     def ref(self, container=None, label="_"):
         """Return a ref to an instance (or dict) associated to a label.
 
         Label must be unique.
         """
         if container is None:
             container = AttrDict()
         objref = Ref(container, self, label)
         assert label not in self.containers
         self.containers[label] = objref
         return objref
 
-
     def set_value(self, ref, value):
         """Set a value pointed by a ref and execute all tasks that depends on ref.
 
         If the value is a Ref, create a new task from the ref.
         """
-        logger.info("set_value %s %s",ref,value)
+        logger.info("set_value %s %s", ref, value)
         if ref in self.tasks:
             self.unregister(ref)
         if isinstance(value, ARef):  # value is an expression
-            self.register(ref, ExprTask(ref, value))
+            self.register(ExprTask(ref, value))
             value = value._get_value()  # to be updated
         ref._set_value(value)
         self._run_tasks(self.find_tasks(ref._get_dependencies()))
 
     def _run_tasks(self, tasks):
         for task in tasks:
-            logger.info("Run %s",task)
+            logger.info("Run %s", task)
             task.run()
 
-    def register(self, taskid, task):
+    def register(self, task):
         """Register a new task identified by taskid"""
-        #logger.info("register %s",taskid)
+        # logger.info("register %s",taskid)
+        taskid = task.taskid
         self.tasks[taskid] = task
         for dep in task.dependencies:
-            #logger.info("%s have an impact on %s",dep,task.targets)
-            self.rdeps[dep].update(task.targets)
-            #logger.info("%s is used by T:%s",dep,taskid)
-            self.deptasks[dep].add(taskid)
+            # logger.info("%s have an impact on %s",dep,task.targets)
+            self.rdeps[dep].extend(task.targets)
+            # logger.info("%s is used by T:%s",dep,taskid)
+            self.deptasks[dep].append(taskid)
             for deptask in self.tartasks[dep]:
-                #logger.info("%s modifies deps of T:%s",deptask,taskid)
-                self.rtasks[deptask].add(taskid)
+                # logger.info("%s modifies deps of T:%s",deptask,taskid)
+                self.rtasks[deptask].append(taskid)
         for tar in task.targets:
-            #logger.info("%s is modified by T:%s",tar,taskid)
-            self.tartasks[tar].add(taskid)
+            # logger.info("%s is modified by T:%s",tar,taskid)
+            self.tartasks[tar].append(taskid)
             for deptask in self.deptasks[tar]:
-                #logger.info("T:%s modifies deps of T:%s",taskid,deptask)
-                self.rtasks[taskid].add(deptask)
+                # logger.info("T:%s modifies deps of T:%s",taskid,deptask)
+                self.rtasks[taskid].append(deptask)
 
     def unregister(self, taskid):
         """Unregister the task identified by taskid"""
         task = self.tasks[taskid]
         for dep in task.dependencies:
             for target in task.targets:
-                self.rdeps[dep].remove(target)
-            self.deptasks[dep].remove(taskid)
+                if target in self.rdeps[dep]:
+                    self.rdeps[dep].remove(target)
+            if dep in self.rtasks[dep]:
+                self.rtasks[dep].remove(taskid)
+            if taskid in self.deptasks[dep]:
+                self.deptasks[dep].remove(taskid)
         for tar in task.targets:
             self.tartasks[tar].remove(taskid)
             for deptask in self.deptasks[tar]:
-                self.rtasks[taskid].remove(deptask)
+                if taskid in self.rtasks[deptask]:
+                    self.rtasks[taskid].remove(deptask)
+        if taskid in self.rtasks:
+            del self.rtasks[taskid]
         del self.tasks[taskid]
 
     def find_deps(self, start_set):
         """Find all refs that depends on ref in start_seps"""
         assert type(start_set) in (list, tuple, set)
         deps = toposort(self.rdeps, start_set)
         return deps
@@ -215,37 +239,58 @@
 
     def find_tasks(self, start_deps=None):
         """Find all tasks that depend on the refs in start_deps"""
         if start_deps is None:
             start_deps = self.rdeps
         return [self.tasks[taskid] for taskid in self.find_taskids(start_deps)]
 
+    def iter_expr_tasks_owner(self, ref):
+        """Return all ExprTask defintions that write registered container"""
+        for t in self.find_tasks():
+            # TODO check for all targets or limit to ExprTask
+            if _check_root_owner(t.taskid, ref):
+                yield str(t.taskid), str(t.expr)
+
+    def copy_expr_from(self, mgr, name, bindings=None):
+        """
+        Copy expression from another manager
+
+        name: one of toplevel container in mgr
+        bindings: dictionary mapping old container names into new container refs
+        """
+        ref = mgr.containers[name]
+        if bindings is None:
+            cmbdct = self.containers
+        else:
+            cmbdct = dct_merge(self.containers, bindings)
+        self.load(mgr.iter_expr_tasks_owner(ref), cmbdct)
+
     def mk_fun(self, name, **kwargs):
         """Write a python function that executes a set of tasks in order of dependencies:
-            name: name of the functions
-            kwards:
-                the keys are used to defined the argument name of the functions
-                the values are the refs that will be set
+        name: name of the functions
+        kwards:
+            the keys are used to defined the argument name of the functions
+            the values are the refs that will be set
         """
         varlist, start = list(zip(*kwargs.items()))
         tasks = self.find_tasks(start)
         fdef = [f"def {name}({','.join(varlist)}):"]
         for vname, vref in kwargs.items():
             fdef.append(f"  {vref} = {vname}")
         for tt in tasks:
             fdef.append(f"  {tt}")
         fdef = "\n".join(fdef)
         return fdef
 
-    def gen_fun(self,name, **kwargs):
+    def gen_fun(self, name, **kwargs):
         """Return a python function that executes a set of tasks in order of dependencies:
-            name: name of the functions
-            kwards:
-                the keys are used to defined the argument name of the functions
-                the values are the refs that will be set
+        name: name of the functions
+        kwards:
+            the keys are used to defined the argument name of the functions
+            the values are the refs that will be set
         """
         fdef = self.mk_fun(name, **kwargs)
         gbl = {}
         lcl = {}
         gbl.update((k, r._owner) for k, r in self.containers.items())
         exec(fdef, gbl, lcl)
         return lcl[name]
@@ -305,33 +350,39 @@
             mpl_display_png(png)
         elif backend == "os":
             os_display_png(png)
         elif backend == "ipy":
             ipy_display_png(png)
         return pdot
 
-
     def dump(self):
-        """Dump in json all ExprTask defined in the manager
-        """
+        """Dump in json all ExprTask defined in the manager"""
         data = [
-            (str(t.taskid), str(t.expr))
-            for t in self.find_tasks(self.rdeps)
-            if isinstance(t, ExprTask)
+            (str(tt.taskid), str(tt.expr))
+            # for t in self.find_tasks(self.rdeps)
+            for tt in self.tasks.values()
+            if isinstance(tt, ExprTask)
         ]
         return data
 
-    def load(self, dump):
-        """Reload the expressions in dump
+    def load(self, dump, dct=None):
+        """Reload the expressions in dump  using container in dct
+
+        dump: list of (lhs,rhs) pairs
+        dct: dictionary of named references of containers,
+             self containers by default
+
         """
+        if dct is None:
+            dct = self.containers
         for lhs, rhs in dump:
-            lhs = eval(lhs, {}, self.containers)
-            rhs = eval(rhs, {}, self.containers)
+            lhs = eval(lhs, {}, dct)
+            rhs = eval(rhs, {}, dct)
             task = ExprTask(lhs, rhs)
-            self.register(task.taskid, task)
+            self.register(task)
 
     def newenv(self, label="_", data=None):
         "Experimental"
         if data is None:
             data = AttrDict()
         ref = self.ref(data, label=label)
         return DepEnv(data, ref)
@@ -340,7 +391,50 @@
         "Experimental"
         if container is None:
             container = AttrDict()
         objref = ObjectAttrRef(container, self, label)
         assert label not in self.containers
         self.containers[label] = objref
         return objref
+
+    def cleanup(self):
+        """
+        Remove empty sets from dicts
+        """
+        for dct in self.rdeps, self.rtasks, self.deptasks, self.tartasks:
+            for kk, ss in list(dct.items()):
+                if len(ss) == 0:
+                    del dct[kk]
+
+    def copy(self):
+        """
+        Create a copy of in new manager
+        """
+        other = Manager()
+        other.containers = deepcopy(self.containers)
+        other.tasks = deepcopy(self.tasks)
+        other.rdeps = deepcopy(self.rdeps)
+        other.rtasks = deepcopy(self.rtasks)
+        other.deptasks = deepcopy(self.deptasks)
+        other.tartasks = deepcopy(self.tartasks)
+        return other
+
+    def rebuild(self):
+        self.cleanup()
+        other = Manager()
+        other.containers.update(self.containers)
+        for task in self.tasks.values():
+            other.register(task)
+        other.cleanup()
+        return other
+
+    def verify(self, dcts=("rdeps", "rtasks", "deptasks", "tartasks")):
+        other = self.rebuild()
+        for dct in dcts:
+            odct = getattr(other, dct)
+            sdct = getattr(self, dct)
+            for kk, ss in list(sdct.items()):
+                if set(ss) != set(odct[kk]):
+                    print(f"{dct}[{kk}] not consistent")
+                    print(f"{dct}[{kk}] self - check:", set(ss) - set(odct[kk]))
+                    print(f"{dct}[{kk}] check - self:", set(odct[kk]) - set(ss))
+                    # raise (ValueError(f"{self} is not consistent in {dct}[{kk}]"))
```

### Comparing `xdeps-0.0.9/xdeps/utils.py` & `xdeps-0.1.0/xdeps/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # copyright ############################### #
 # This file is part of the Xdeps Package.   #
 # Copyright (c) CERN, 2021.                 #
 # ######################################### #
 
+
 def mpl_display_png(png):
     import io
     import matplotlib.pyplot as plt
     import matplotlib.image as mpimg
 
     sio = io.BytesIO()
     sio.write(png)
     sio.seek(0)
     img = mpimg.imread(sio)
-    imgplot = plt.imshow(img, aspect='auto')
-    #imgplot = plt.imshow(img)
+    imgplot = plt.imshow(img, aspect="auto")
+    # imgplot = plt.imshow(img)
     plt.xticks([])
     plt.yticks([])
 
+
 def os_display_png(png):
     import os
-    with open("/tmp/out.png",'wb') as fh:
+
+    with open("/tmp/out.png", "wb") as fh:
         fh.write(png)
     os.system("(display /tmp/out.png && rm /tmp/out.png)&")
 
+
 def ipy_display_png(png):
     from IPython.display import Image, display
+
     plt = Image(png)
     display(plt)
 
+
 class AttrDict(dict):
     def __init__(self, *args, **kwargs):
         super(AttrDict, self).__init__(*args, **kwargs)
         self.__dict__ = self
-
-
```

### Comparing `xdeps-0.0.9/xdeps.egg-info/PKG-INFO` & `xdeps-0.1.0/xdeps.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: xdeps
-Version: 0.0.9
+Version: 0.1.0
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
+Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
-Download-URL: https://pypi.python.org/pypi/xdeps
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Documentation, https://xsuite.readthedocs.io/
 Project-URL: Source Code, https://github.com/xsuite/xdeps
-Description: Data dependency manager
-        
-        This package is part of the Xsuite collection.
-Platform: UNKNOWN
+Provides-Extra: tests
+License-File: LICENSE
+
+Data dependency manager
+
+This package is part of the Xsuite collection.
```

