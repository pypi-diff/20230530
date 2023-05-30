# Comparing `tmp/corpus_judge-0.0.2.tar.gz` & `tmp/corpus_judge-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus_judge-0.0.2.tar", max compression
+gzip compressed data, was "corpus_judge-0.0.3.tar", max compression
```

## Comparing `corpus_judge-0.0.2.tar` & `corpus_judge-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1491 2023-05-28 20:04:11.444523 corpus_judge-0.0.2/LICENSE
--rw-r--r--   0        0        0      250 2023-05-28 20:00:18.687607 corpus_judge-0.0.2/README.md
--rw-r--r--   0        0        0      153 2023-05-28 20:44:53.654068 corpus_judge-0.0.2/corpus_judge/__init__.py
--rw-r--r--   0        0        0     6750 2023-05-28 20:43:59.813913 corpus_judge-0.0.2/corpus_judge/justice_model.py
--rw-r--r--   0        0        0    11934 2023-05-28 20:13:51.190037 corpus_judge-0.0.2/corpus_judge/justice_name.py
--rw-r--r--   0        0        0     9654 2023-05-28 20:45:49.114547 corpus_judge-0.0.2/corpus_judge/justice_select.py
--rw-r--r--   0        0        0    45229 2023-05-28 19:46:46.811633 corpus_judge-0.0.2/corpus_judge/sc.yaml
--rw-r--r--   0        0        0     1227 2023-05-28 20:44:13.923099 corpus_judge-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 corpus_judge-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-05-28 20:04:11.444523 corpus_judge-0.0.3/LICENSE
+-rw-r--r--   0        0        0      250 2023-05-28 20:00:18.687607 corpus_judge-0.0.3/README.md
+-rw-r--r--   0        0        0      153 2023-05-28 20:44:53.654068 corpus_judge-0.0.3/corpus_judge/__init__.py
+-rw-r--r--   0        0        0     6750 2023-05-28 20:43:59.813913 corpus_judge-0.0.3/corpus_judge/justice_model.py
+-rw-r--r--   0        0        0    14172 2023-05-30 00:36:45.835164 corpus_judge-0.0.3/corpus_judge/justice_name.py
+-rw-r--r--   0        0        0     9709 2023-05-30 00:16:54.038433 corpus_judge-0.0.3/corpus_judge/justice_select.py
+-rw-r--r--   0        0        0    45229 2023-05-28 19:46:46.811633 corpus_judge-0.0.3/corpus_judge/sc.yaml
+-rw-r--r--   0        0        0     1227 2023-05-30 00:38:56.169412 corpus_judge-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 corpus_judge-0.0.3/PKG-INFO
```

### Comparing `corpus_judge-0.0.2/LICENSE` & `corpus_judge-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.2/corpus_judge/justice_model.py` & `corpus_judge-0.0.3/corpus_judge/justice_model.py`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.2/corpus_judge/justice_name.py` & `corpus_judge-0.0.3/corpus_judge/justice_name.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,124 @@
 import re
 from enum import Enum
 from typing import NamedTuple, Self
 
 from unidecode import unidecode
 
 IS_PER_CURIAM = re.compile(r"per\s+curiam", re.I)  # type: ignore
+FULLNAME_STYLE = re.compile(
+    r"""
+        ^
+            (Chief\s+)?
+            Justice\s+
+            .*
+            \s+
+            (?P<surname>
+                [\w-]+
+                (,?
+                \s+
+                    (
+                        Jr\.|
+                        Sr\.|
+                        I{2,}
+                    )
+                )?
+            )
+        $
+    """,
+    re.I | re.X,
+)
+
+
+def initialize_name(text: str):
+    """Remove unnecessary text and make uniform accented content."""
+    text = unidecode(text)
+    text = text.lower()
+    text = text.strip(",.: ")
+    return text
+
+
+def limit_modern_to_terminal_text(text: str):
+    """Modern convention uses the
+
+    Examples:
+        >>> limit_modern_to_terminal_text('Chief Justice Alexander G. Gesmundo')
+        'gesmundo'
+        >>> limit_modern_to_terminal_text('Justice Marvic M.V.F. Leonen')
+        'leonen'
+        >>> limit_modern_to_terminal_text('Justice Antonio T. Kho, Jr.')
+        'kho, jr.'
+        >>> limit_modern_to_terminal_text('Justice Estela M. Perlas-Bernabe')
+        'perlas-bernabe'
+    """
+    if match := FULLNAME_STYLE.search(text):
+        return match.group("surname").strip().lower()
+    return text
 
 
 class OpinionWriterName(NamedTuple):
     writer: str | None = None
     per_curiam: bool = False
 
     @classmethod
     def extract(cls, text: str | None) -> Self | None:
         """Will mark `per_curiam` to be True if the regex pattern matches,
         else, will clean the writer represented by the text, if possible.
 
+        Examples:
+            >>> OpinionWriterName.extract('Justice Marvic M.V.F. Leonen')
+            OpinionWriterName(writer='leonen', per_curiam=False)
+            >>> OpinionWriterName.extract('Justice Filomena D. Signh') # note bad spelling
+            OpinionWriterName(writer='singh', per_curiam=False)
+
         Args:
             text (str | None): Text to evaluate.
 
         Returns:
             Self | None: Instance representing the writer.
-        """
+        """  # noqa: E501
         if not text:
             return None
         if text:
             if IS_PER_CURIAM.search(text):
                 return cls(per_curiam=True)
-            return cls(writer=cls.clean(text))
+            # if text is modern, e.g. from the 2023 SC website, adjust the text
+            # prior to clean() since the clean function was intended for the
+            # more traditional elibrary.
+            text = limit_modern_to_terminal_text(text)
+            writer = cls.clean(text)  # check proper
+            return cls(writer=writer)
 
     @classmethod
     def clean(cls, text: str) -> str | None:
-        """Each `ponente` name stored in the database can me uniform, e.g.:
+        """Each `ponente` name stored in the database can be uniform. Will
+        parse text, apply some cleaning steps, and result in a lower-cased form
+        of the original `text`, e.g.:
+
+        Some constraints:
+
+        1. Must be more than 4 characters
+        2. Must be less than 40 characters
 
         Examples:
             >>> OpinionWriterName.clean("REYES , J.B.L, Acting C.J.") # sample name 1
             'reyes, j.b.l.'
             >>> OpinionWriterName.clean("REYES, J, B. L. J.") # sample name 2
             'reyes, j.b.l.'
         """
 
         no_asterisk = re.sub(r"\[?(\*)+\]?", "", text)
-        surname = init_surnames(no_asterisk)
-        no_suffix = TitleSuffixClean.clean_end(surname).strip()
-        repl = CommonTypos.replace_value(no_suffix).strip()
+        name = initialize_name(no_asterisk)
+        no_suffix = TitleSuffix.cull(name).strip()
+        repl = CommonTypos.replace(no_suffix).strip()
         res = repl + "." if repl.endswith((" jr", " sr")) else repl
-        return res if 4 < len(res) < 20 else None
+        return res if 4 < len(res) < 40 else None
 
 
-class TitleSuffixClean(Enum):
+class TitleSuffix(Enum):
     """The order matters: will try to match the old style first."""
 
     CHIEF = re.compile(
         r"""
         ,?
         \s*
         (
@@ -96,17 +162,23 @@
         )
         $
         """,
         re.I | re.X,
     )
 
     @classmethod
-    def clean_end(cls, candidate: str):
-        """If one of the members matches, return the replacement."""
-        for _, member in cls.__members__.items():
+    def cull(cls, candidate: str):
+        """If one of the members matches, return the replacement.
+
+        Examples:
+            >>> TitleSuffix.CHIEF.cull('REYES , J.B.L, Acting C.J.')
+            'REYES , J.B.L'
+
+        """
+        for member in cls:
             if member.value.search(candidate):
                 return member.value.sub("", candidate)
         return candidate
 
 
 class CommonTypos(Enum):
     AVANC = (
@@ -609,29 +681,41 @@
             ^diokno[,\s]+m\.?
             """,
             re.I | re.X,
         ),
         "diokno",
     )
 
+    LAZARO = (
+        re.compile(
+            r"""
+           ^la(.*?)-javier$
+            """,
+            re.I | re.X,
+        ),
+        "lazaro-javier",
+    )
+
+    SINGH = (
+        re.compile(
+            r"""
+            ^signh$
+            """,
+            re.I | re.X,
+        ),
+        "singh",
+    )
+
     @classmethod
-    def replace_value(cls, candidate: str) -> str:
+    def replace(cls, candidate: str) -> str:
         """If member matches `candidate`, return replacement specified in value.
 
         Args:
             candidate (str): Name of the justice which may contain typos.
 
         Returns:
             str: Corrected name, if possible; otherwise just the candidate text.
         """
-        for _, member in cls.__members__.items():
+        for member in cls:
             if member.value[0].search(candidate):
                 return member.value[1]
         return candidate
-
-
-def init_surnames(text: str):
-    """Remove unnecessary text and make uniform accented content."""
-    text = unidecode(text)
-    text = text.lower()
-    text = text.strip(",.: ")
-    return text
```

### Comparing `corpus_judge-0.0.2/corpus_judge/justice_select.py` & `corpus_judge-0.0.3/corpus_judge/justice_select.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         try:
             return parse(self.date_str).date()
         except Exception:
             return None
 
     @property
     def src(self):
+        """This may either be just the last name or the full name."""
         return OpinionWriterName.extract(self.text)
 
     @property
     def candidate(self) -> str | None:
         return self.src and self.src.writer
 
     @property
@@ -79,15 +80,15 @@
             ),
             order_by="start_term desc",
         )
         return list(results)
 
     @property
     def choice(self) -> dict | None:
-        """Based on `get_active_on_date()`, match the cleaned_name to either the alias
+        """Based on `@rows`, match the cleaned_name to either the alias
         of the justice or the justice's last name; on match, determine whether the
         designation should be 'C.J.' or 'J.'
 
         Examples:
             >>> import yaml
             >>> from pathlib import Path
             >>> from sqlpyd import Connection
```

### Comparing `corpus_judge-0.0.2/corpus_judge/sc.yaml` & `corpus_judge-0.0.3/corpus_judge/sc.yaml`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.2/pyproject.toml` & `corpus_judge-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "corpus-judge"
 description = "Cleaning, setting Justices"
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/corpus-judge"
 documentation = "https://justmars.github.io/corpus-judge"
 classifiers = [
   "Programming Language :: Python :: 3.11",
```

### Comparing `corpus_judge-0.0.2/PKG-INFO` & `corpus_judge-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corpus-judge
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cleaning, setting Justices
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

