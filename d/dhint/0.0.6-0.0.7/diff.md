# Comparing `tmp/dhint-0.0.6.tar.gz` & `tmp/dhint-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhint-0.0.6.tar", max compression
+gzip compressed data, was "dhint-0.0.7.tar", max compression
```

## Comparing `dhint-0.0.6.tar` & `dhint-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,27 @@
--rw-r--r--   0        0        0      247 2023-05-28 18:11:56.153127 dhint-0.0.6/dhint/__init__.py
--rw-r--r--   0        0        0    12346 2023-05-28 21:49:45.365627 dhint-0.0.6/dhint/base.py
--rw-r--r--   0        0        0     4068 2023-05-27 02:24:55.001024 dhint-0.0.6/dhint/collections.py
--rw-r--r--   0        0        0     5276 2023-05-28 21:49:45.368265 dhint-0.0.6/dhint/descriptors.py
--rw-r--r--   0        0        0     2111 2023-05-21 17:56:59.467134 dhint-0.0.6/dhint/functions.py
--rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.6/dhint/hints.py
--rw-r--r--   0        0        0     1459 2023-05-26 03:01:24.856969 dhint-0.0.6/dhint/json_encoder.py
--rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.6/dhint/protocols.py
--rw-r--r--   0        0        0     1466 2023-05-26 12:08:08.808018 dhint-0.0.6/dhint/subdescriptor.py
--rw-r--r--   0        0        0     9880 2023-05-25 18:15:02.476932 dhint-0.0.6/dhint/type_hint.py
--rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.6/dhint/types.py
--rw-r--r--   0        0        0      330 2023-05-28 21:51:27.869541 dhint-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      616 2023-05-28 21:51:47.466280 dhint-0.0.6/setup.py
--rw-r--r--   0        0        0      382 2023-05-28 21:51:47.466514 dhint-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      256 2023-05-30 02:04:47.119981 dhint-0.0.7/dhint/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-29 21:25:54.398280 dhint-0.0.7/dhint/base/__init__.py
+-rw-r--r--   0        0        0      311 2023-05-29 21:26:44.999717 dhint-0.0.7/dhint/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9730 2023-05-30 02:04:47.206837 dhint-0.0.7/dhint/base/__pycache__/_meta.cpython-39.pyc
+-rw-r--r--   0        0        0     2019 2023-05-29 20:55:46.212056 dhint-0.0.7/dhint/base/__pycache__/base_enum.cpython-39.pyc
+-rw-r--r--   0        0        0     1620 2023-05-29 21:06:46.698181 dhint-0.0.7/dhint/base/__pycache__/collections.cpython-39.pyc
+-rw-r--r--   0        0        0     1359 2023-05-30 02:04:47.204675 dhint-0.0.7/dhint/base/__pycache__/datamodel.cpython-39.pyc
+-rw-r--r--   0        0        0    10159 2023-05-29 21:22:24.209570 dhint-0.0.7/dhint/base/__pycache__/descriptor.cpython-39.pyc
+-rw-r--r--   0        0        0     1245 2023-05-29 21:26:45.006946 dhint-0.0.7/dhint/base/__pycache__/detamodel.cpython-39.pyc
+-rw-r--r--   0        0        0     6695 2023-05-30 02:04:47.122660 dhint-0.0.7/dhint/base/_meta.py
+-rw-r--r--   0        0        0     1125 2023-05-29 20:55:46.168796 dhint-0.0.7/dhint/base/base_enum.py
+-rw-r--r--   0        0        0      837 2023-05-29 21:06:13.237219 dhint-0.0.7/dhint/base/collections.py
+-rw-r--r--   0        0        0      611 2023-05-30 02:04:47.126353 dhint-0.0.7/dhint/base/datamodel.py
+-rw-r--r--   0        0        0     8454 2023-05-29 21:22:24.128278 dhint-0.0.7/dhint/base/descriptor.py
+-rw-r--r--   0        0        0      664 2023-05-29 21:25:54.390832 dhint-0.0.7/dhint/base/detamodel.py
+-rw-r--r--   0        0        0     4068 2023-05-27 02:24:55.001024 dhint-0.0.7/dhint/collections.py
+-rw-r--r--   0        0        0     5667 2023-05-29 00:53:58.892079 dhint-0.0.7/dhint/descriptors.py
+-rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.7/dhint/function_types.py
+-rw-r--r--   0        0        0     2504 2023-05-29 21:49:14.357625 dhint-0.0.7/dhint/functions.py
+-rw-r--r--   0        0        0     1425 2023-05-24 11:39:17.174355 dhint-0.0.7/dhint/hints.py
+-rw-r--r--   0        0        0     1468 2023-05-30 02:04:47.124525 dhint-0.0.7/dhint/json_encoder.py
+-rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.7/dhint/protocols.py
+-rw-r--r--   0        0        0     1466 2023-05-26 12:08:08.808018 dhint-0.0.7/dhint/subdescriptor.py
+-rw-r--r--   0        0        0     9889 2023-05-30 02:04:47.117134 dhint-0.0.7/dhint/type_hint.py
+-rw-r--r--   0        0        0      330 2023-05-30 02:07:46.909720 dhint-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      630 2023-05-30 02:07:59.513324 dhint-0.0.7/setup.py
+-rw-r--r--   0        0        0      382 2023-05-30 02:07:59.513540 dhint-0.0.7/PKG-INFO
```

### Comparing `dhint-0.0.6/dhint/collections.py` & `dhint-0.0.7/dhint/collections.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.6/dhint/descriptors.py` & `dhint-0.0.7/dhint/descriptors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 __all__ = ['Descriptor', 'Validator', 'NumberValidator', 'StringValidator', 'DateTimeValidator', 'DateValidator',
            'TextAreaValidator', 'IntValidator', 'FloatValidator', 'SelfKeyValidator', 'DecimalValidator',
-           'AutoValidator', 'PasswordValidator', 'BytesValidator', 'AutoUpdateValidator']
+           'AutoValidator', 'PasswordValidator', 'BytesValidator', 'AutoUpdateValidator', 'SelectValidator']
 
 import datetime
 from decimal import Decimal
 from typing import Optional, Callable
 from .base import *
 from .type_hint import *
 
 
 class Descriptor(BaseDescriptor):
     
+    @property
+    def type_hint(self) -> TypeHint:
+        return TypeHint(self.field_type)
+    
     def parse(self, value):
         return Parser.get(value, self.field_type)
 
-    def validate(self, value):
+    def validate(self, value) -> None:
         if any([value is None, value == '']):
             if self.is_required:
                 raise ValueError(f'{self.fullname}: o valor não pode ser nulo.')
         else:
-            if not TypeHint(self.field_type).check_type(value):
+            if not self.type_hint.check_type(value):
                 raise ValueError(f'{self.fullname}: o tipo de "{value}" ({type(value)}) não corresponde ao esperado ({self.field_type}).')
     
 
 class Validator(Descriptor):
+    
     def __init__(self, *args, **kwargs):
         self._predicate: Optional[Callable] = kwargs.pop('predicate', None)
         super().__init__(*args, **kwargs)
         
     @property
     def predicate(self):
         return self._predicate
@@ -35,15 +40,14 @@
     def validate(self, value):
         super().validate(value)
         if self.predicate:
             if self.predicate(value) is False:
                 raise ValueError(f'{self.fullname}: o predicativo é falso para "{value}".')
 
 
-    
 class DateTimeValidator(Validator):
     FIELD_TYPE = datetime.datetime
     HTML_TAG = 'input'
     INPUT_TYPE = 'datetime-local'
     
     def __init__(self, *args, **kwargs):
         self._min: Optional[float, int, Decimal] = kwargs.pop('min', None)
@@ -78,15 +82,14 @@
     INPUT_TYPE = 'number'
     
     def __init__(self, *args, **kwargs):
         self._step: Optional[float, int] = kwargs.pop('step', None)
         super().__init__(*args, **kwargs)
     
 
-
 class IntValidator(NumberValidator):
     FIELD_TYPE = int
 
 
 class FloatValidator(NumberValidator):
     FIELD_TYPE = float
     
@@ -133,14 +136,22 @@
         super().__init__(*args, **kwargs)
         
     @property
     def height(self):
         return self._height
     
     
+class SelectValidator(TextAreaValidator):
+    HTML_TAG = 'select'
+    FIELD_TYPE = None
+    
+    def options(self, default: str = None):
+        return self.type_hint.expected_type.options(default)
+    
+    
 class SelfKeyValidator(StringValidator):
     INPUT_TYPE = 'hidden'
     FROZEN = True
     
     
 class PasswordValidator(StringValidator):
     FIELD_TYPE = bytes
@@ -163,14 +174,18 @@
     def __set__(self, instance, value):
         setattr(instance, self.private_name, value)
         if any([value is None, value == '']):
             value = self.func(instance)
         setattr(instance, self.private_name, value)
         
     @property
+    def is_required(self):
+        return False
+        
+    @property
     def repr(self) -> bool:
         return False
         
     @property
     def func(self):
         return self._func
```

### Comparing `dhint-0.0.6/dhint/functions.py` & `dhint-0.0.7/dhint/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,40 @@
 from __future__ import annotations
 
-__all__ = ['slug', 'normalize', 'normalize_lower', 'hyphen_to_underscore', 'underscore_to_hyphen',
-           'remove_extra_whitespaces', 'underscore_text', 'titlecase', 'getter', 'map_setter']
+__all__ = [
+        'slug',
+        'normalize',
+        'normalize_lower',
+        'hyphen_to_underscore',
+        'underscore_to_hyphen',
+        'remove_extra_whitespaces',
+        'underscore_text',
+        'titlecase',
+        'getter',
+        'map_setter',
+        'last',
+        'first',
+        'keyattr',
+        'keyitem',
+        'key'
+    ]
 
 import re
-from typing import Any, Mapping
+from typing import Any
+from operator import getitem, attrgetter, itemgetter
 from unidecode import unidecode
 
 
+first = lambda x: getitem(x, 0)
+last = lambda x: getitem(x, -1)
+keyattr = attrgetter('key')
+keyitem = itemgetter('key')
+key = lambda x: keyitem(x) if isinstance(x, dict) else keyattr(x)
+
+
 def map_setter(obj: dict) -> dict:
     for k, v in obj.items():
         setattr(obj, k, property(lambda obj: obj[k]))
     return obj
     
 
 def getter(obj: Any, prop: str, default: Any = None) -> Any:
```

### Comparing `dhint-0.0.6/dhint/hints.py` & `dhint-0.0.7/dhint/hints.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.6/dhint/json_encoder.py` & `dhint-0.0.7/dhint/json_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import json
 import datetime
 from enum import Enum
 from dataclasses import asdict
 from collections import UserString
 from typing import Any
-from .types import *
+from .function_types import *
 from .collections import *
 from .hints import *
 
 
 class JsonEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, datetime.datetime):
```

### Comparing `dhint-0.0.6/dhint/subdescriptor.py` & `dhint-0.0.7/dhint/subdescriptor.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.6/dhint/type_hint.py` & `dhint-0.0.7/dhint/type_hint.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import datetime
 from abc import ABC
 from collections import ChainMap, deque
 from typing import Union
 from decimal import Decimal
 from typing import Any, get_args, get_origin
 from .collections import *
-from .types import *
+from .function_types import *
 from .protocols import *
 from .hints import *
 from .base import *
 
 
 class Parser(ABC):
     @classmethod
```

### Comparing `dhint-0.0.6/dhint/types.py` & `dhint-0.0.7/dhint/function_types.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.6/setup.py` & `dhint-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['dhint']
+['dhint', 'dhint.base']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0', 'typing-extensions>=4.6.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'dhint',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

