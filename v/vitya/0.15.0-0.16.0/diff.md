# Comparing `tmp/vitya-0.15.0.tar.gz` & `tmp/vitya-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vitya-0.15.0.tar", last modified: Mon May 29 15:13:12 2023, max compression
+gzip compressed data, was "dist/vitya-0.16.0.tar", last modified: Tue May 30 13:40:54 2023, max compression
```

## Comparing `vitya-0.15.0.tar` & `vitya-0.16.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-29 15:13:09.000000 vitya-0.15.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-29 15:13:12.000000 vitya-0.15.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-29 15:13:09.000000 vitya-0.15.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-29 15:13:09.000000 vitya-0.15.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:13:12.000000 vitya-0.15.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-29 15:13:09.000000 vitya-0.15.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-05-29 15:13:09.000000 vitya-0.15.0/tests/test_vitya.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/errors_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya/payment_order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya/payment_order/payments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-30 13:40:48.000000 vitya-0.16.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-30 13:40:54.000000 vitya-0.16.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-30 13:40:48.000000 vitya-0.16.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 13:40:48.000000 vitya-0.16.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:40:54.000000 vitya-0.16.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-30 13:40:48.000000 vitya-0.16.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-05-30 13:40:48.000000 vitya-0.16.0/tests/test_vitya.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/errors_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya/payment_order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28540 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya/payment_order/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/payments/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/payment_order/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-30 13:40:48.000000 vitya-0.16.0/vitya/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 13:40:54.000000 vitya-0.16.0/vitya.egg-info/top_level.txt
```

### Comparing `vitya-0.15.0/LICENSE` & `vitya-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/PKG-INFO` & `vitya-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.15.0
+Version: 0.16.0
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.15.0/README.md` & `vitya-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/setup.py` & `vitya-0.16.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='vitya',
-    version='0.15.0',
+    version='0.16.0',
     author='hicebank.ru',
     author_email='inyutin@hicebank.ru',
     description='Validators for different russian banking values',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/hicebank/vitya',
     packages=setuptools.find_packages(),
```

### Comparing `vitya-0.15.0/tests/test_vitya.py` & `vitya-0.16.0/tests/test_vitya.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya/errors.py` & `vitya-0.16.0/vitya/errors.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya/payment_order/enums.py` & `vitya-0.16.0/vitya/payment_order/enums.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya/payment_order/errors.py` & `vitya-0.16.0/vitya/payment_order/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,19 +503,14 @@
 
 
 class ReasonValidationTypeError(ReasonValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должно быть строкой'
 
 
-class ReasonValidationFNSOnlyEmptyError(ReasonValidationError):
-    description = 'for fns only empty allowed'
-    description_ru = 'для платежей в ФНС значение должно быть пустым'
-
-
 class ReasonValidationValueLenError(ReasonValidationError):
     description = 'must be 2 chars'
     description_ru = 'должно состоять из 2 символов'
 
 
 class ReasonValidationValueErrorCustoms(ReasonValidationError):
     description = f'for customs payment value must be in {CUSTOMS_REASONS}'
```

### Comparing `vitya-0.15.0/vitya/payment_order/fields.py` & `vitya-0.16.0/vitya/payment_order/fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya/payment_order/payments/checkers.py` & `vitya-0.16.0/vitya/payment_order/payments/checkers.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya/payment_order/payments/checks.py` & `vitya-0.16.0/vitya/payment_order/payments/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     PayerKPPValidationINN12OnlyEmptyError,
     PayerStatusValidationCustoms05NotAllowedError,
     PayerStatusValidationNullNotAllowedError,
     PaymentTypeValueError,
     PurposeCodeValidationFlError,
     PurposeCodeValidationNullError,
     PurposeValidationIPNDSError,
-    ReasonValidationFNSOnlyEmptyError,
     ReasonValidationValueErrorCustoms,
     TaxPeriodValidationBOValueLenError,
     TaxPeriodValidationCustomsEmptyNotAllowed,
     TaxPeriodValidationCustomsValueLenError,
     TaxPeriodValidationFNS01OnlyEmpty,
     TaxPeriodValidationFNS02EmptyNotAllowed,
     TaxPeriodValidationFNSEmptyNotAllowed,
@@ -314,19 +313,15 @@
 def check_reason(
     value: Optional[Reason],
     payment_type: PaymentType,
 ) -> Optional[Reason]:
     if not payment_type.is_budget:
         return None
 
-    if payment_type in {PaymentType.CUSTOMS, PaymentType.BUDGET_OTHER} and value is None:
-        return None
-    if payment_type == PaymentType.FNS:
-        if value is not None:
-            raise ReasonValidationFNSOnlyEmptyError
+    if payment_type.is_budget and value is None:
         return None
     if payment_type == PaymentType.CUSTOMS and value not in CUSTOMS_REASONS:
         raise ReasonValidationValueErrorCustoms
     return value
 
 
 def check_tax_period(
```

### Comparing `vitya-0.15.0/vitya/payment_order/payments/constants.py` & `vitya-0.16.0/vitya/payment_order/payments/constants.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya/payment_order/payments/tools.py` & `vitya-0.16.0/vitya/payment_order/payments/tools.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya/payment_order/validators.py` & `vitya-0.16.0/vitya/payment_order/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya/pydantic_fields.py` & `vitya-0.16.0/vitya/pydantic_fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya/validators.py` & `vitya-0.16.0/vitya/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.15.0/vitya.egg-info/PKG-INFO` & `vitya-0.16.0/vitya.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.15.0
+Version: 0.16.0
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.15.0/vitya.egg-info/SOURCES.txt` & `vitya-0.16.0/vitya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

