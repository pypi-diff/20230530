# Comparing `tmp/nepattern-0.5.8.tar.gz` & `tmp/nepattern-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.5.8.tar", last modified: Thu May 25 16:55:50 2023, max compression
+gzip compressed data, was "nepattern-0.5.9.tar", last modified: Tue May 30 14:55:16 2023, max compression
```

## Comparing `nepattern-0.5.8.tar` & `nepattern-0.5.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.8/LICENSE
--rw-r--r--   0        0        0      723 2023-05-25 16:53:52.239559 nepattern-0.5.8/nepattern/__init__.py
--rw-r--r--   0        0        0    10865 2023-05-25 16:54:49.230259 nepattern-0.5.8/nepattern/base.py
--rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.8/nepattern/context.py
--rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.8/nepattern/context.pyi
--rw-r--r--   0        0        0    15999 2023-05-25 16:54:58.101916 nepattern-0.5.8/nepattern/core.py
--rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.8/nepattern/exception.py
--rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.8/nepattern/i18n/.config.json
--rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.8/nepattern/i18n/en-US.json
--rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.8/nepattern/i18n/zh-CN.json
--rw-r--r--   0        0        0    10438 2023-05-25 16:53:52.258975 nepattern-0.5.8/nepattern/main.py
--rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.8/nepattern/util.py
--rw-r--r--   0        0        0     1738 2023-05-25 16:54:58.015909 nepattern-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.8/README.md
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.9/LICENSE
+-rw-r--r--   0        0        0      723 2023-05-25 16:53:52.239559 nepattern-0.5.9/nepattern/__init__.py
+-rw-r--r--   0        0        0    10949 2023-05-30 14:42:47.794432 nepattern-0.5.9/nepattern/base.py
+-rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.9/nepattern/context.py
+-rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.9/nepattern/context.pyi
+-rw-r--r--   0        0        0    15999 2023-05-25 16:54:58.101916 nepattern-0.5.9/nepattern/core.py
+-rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.9/nepattern/exception.py
+-rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.9/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.9/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.9/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0    10554 2023-05-30 14:42:47.808432 nepattern-0.5.9/nepattern/main.py
+-rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.9/nepattern/util.py
+-rw-r--r--   0        0        0     1738 2023-05-30 14:42:47.773463 nepattern-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.9/README.md
+-rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.9/PKG-INFO
```

### Comparing `nepattern-0.5.8/LICENSE` & `nepattern-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.8/nepattern/__init__.py` & `nepattern-0.5.9/nepattern/__init__.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.8/nepattern/base.py` & `nepattern-0.5.9/nepattern/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any, Dict, Iterable, Literal, TypeVar, Match
 
 from tarina import Empty
 from tarina.lang import lang
 
 from .core import BasePattern, MatchMode, ValidateResult, ResultFlag
 from .exception import MatchFailed
+from .util import TPattern
 
 
 class DirectPattern(BasePattern):
     """直接判断"""
     def __init__(self, target: Any, alias: str | None = None):
         self.target = target
         super().__init__("", MatchMode.TYPE_CONVERT, type(target), alias=alias or str(target))
@@ -56,16 +57,17 @@
                 value=None if default is Empty else default, flag=ResultFlag.DEFAULT  # type: ignore
             )
         return ValidateResult(input_, flag=ResultFlag.VALID)
 
 class RegexPattern(BasePattern[Match[str]]):
     """针对正则的特化匹配，支持正则组"""
 
-    def __init__(self, pattern: str, alias: str | None = None):
-        super().__init__(pattern, origin=Match[str], alias=alias or "regex[:group]")  # type: ignore
+    def __init__(self, pattern: str | TPattern, alias: str | None = None):
+        super().__init__("", origin=Match[str], alias=alias or "regex[:group]")  # type: ignore
+        self.regex_pattern = re.compile(pattern)
 
     def match(self, input_: str | Any) -> Match[str]:
         if not isinstance(input_, str):
             raise MatchFailed(
                 lang.require("nepattern", "type_error").format(target=input_)
             )
         if mat := self.regex_pattern.match(input_):
```

### Comparing `nepattern-0.5.8/nepattern/context.py` & `nepattern-0.5.9/nepattern/context.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.8/nepattern/context.pyi` & `nepattern-0.5.9/nepattern/context.pyi`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.8/nepattern/core.py` & `nepattern-0.5.9/nepattern/core.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.8/nepattern/main.py` & `nepattern-0.5.9/nepattern/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 except ImportError:
     from typing_extensions import Annotated, get_args, get_origin
 
 
 from .context import global_patterns, all_patterns
 from .core import BasePattern, MatchMode
 from .base import UnionPattern, MappingPattern, SequencePattern, RegexPattern, SwitchPattern, DirectPattern
-from .util import AllParam, GenericAlias, RawStr, CGenericAlias
+from .util import AllParam, GenericAlias, RawStr, CGenericAlias, TPattern
 
 _Contents = (Union, types.UnionType, Literal) if sys.version_info >= (3, 10) else (Union, Literal)  # pragma: no cover
 
 
 AnyOne = BasePattern(r".+", MatchMode.KEEP, Any, alias="any")
 """匹配任意内容的表达式"""
 
@@ -213,14 +213,16 @@
             else list(_)
             if (_ := get_args(anno))
             else [anno],
             origin=Any if sig.return_annotation == Empty else sig.return_annotation,
             converter=item if len(sig.parameters) == 2 else lambda _, x: item(x),
             model=MatchMode.TYPE_CONVERT,
         )
+    if isinstance(item, TPattern):
+        return RegexPattern(item.pattern, alias=f"'{item.pattern}'")
     if isinstance(item, str):
         if item.startswith("re:"):
             pat = item[3:]
             return BasePattern(pat, alias=f"'{pat}'")
         if item.startswith("rep:"):
             pat = item[4:]
             return RegexPattern(pat, alias=f"'{pat}'")
```

### Comparing `nepattern-0.5.8/nepattern/util.py` & `nepattern-0.5.9/nepattern/util.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.8/pyproject.toml` & `nepattern-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nepattern"
-version = "0.5.8"
+version = "0.5.9"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
     "tarina>=0.3.3",
```

### Comparing `nepattern-0.5.8/README.md` & `nepattern-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.8/PKG-INFO` & `nepattern-0.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.5.8
+Version: 0.5.9
 Summary: a complex pattern, support typing
 License: MIT
 Keywords: typing,pattern,converter,validator
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

