# Comparing `tmp/telegram_text-0.1.1.tar.gz` & `tmp/telegram_text-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_text-0.1.1.tar", max compression
+gzip compressed data, was "telegram_text-0.1.2.tar", max compression
```

## Comparing `telegram_text-0.1.1.tar` & `telegram_text-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1073 2022-05-06 16:29:16.746086 telegram_text-0.1.1/LICENSE
--rw-r--r--   0        0        0     2897 2022-12-29 20:23:01.116307 telegram_text-0.1.1/README.md
--rw-r--r--   0        0        0     1259 2022-12-29 20:23:01.120259 telegram_text-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      571 2022-12-29 20:23:01.120895 telegram_text-0.1.1/telegram_text/__init__.py
--rw-r--r--   0        0        0     4848 2022-12-29 20:23:01.121502 telegram_text-0.1.1/telegram_text/bases.py
--rw-r--r--   0        0        0      781 2022-12-28 20:14:32.952146 telegram_text-0.1.1/telegram_text/custom.py
--rw-r--r--   0        0        0     3089 2022-12-29 20:23:01.121904 telegram_text-0.1.1/telegram_text/elements.py
--rw-r--r--   0        0        0     2124 2022-12-29 20:23:01.122349 telegram_text-0.1.1/telegram_text/markdown.py
--rw-r--r--   0        0        0     3431 2022-12-29 20:23:01.122789 telegram_text-0.1.1/telegram_text/styles.py
--rw-r--r--   0        0        0     3698 2022-12-29 20:23:23.446056 telegram_text-0.1.1/setup.py
--rw-r--r--   0        0        0     3852 2022-12-29 20:23:23.446445 telegram_text-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-30 21:29:42.337829 telegram_text-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3128 2023-05-30 21:29:42.341829 telegram_text-0.1.2/README.md
+-rw-r--r--   0        0        0     1228 2023-05-30 21:29:42.349830 telegram_text-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      571 2023-05-30 21:29:42.349830 telegram_text-0.1.2/telegram_text/__init__.py
+-rw-r--r--   0        0        0     4848 2023-05-30 21:29:42.349830 telegram_text-0.1.2/telegram_text/bases.py
+-rw-r--r--   0        0        0      781 2023-05-30 21:29:42.349830 telegram_text-0.1.2/telegram_text/custom.py
+-rw-r--r--   0        0        0     3089 2023-05-30 21:29:42.349830 telegram_text-0.1.2/telegram_text/elements.py
+-rw-r--r--   0        0        0     2124 2023-05-30 21:29:42.349830 telegram_text-0.1.2/telegram_text/markdown.py
+-rw-r--r--   0        0        0     3431 2023-05-30 21:29:42.349830 telegram_text-0.1.2/telegram_text/styles.py
+-rw-r--r--   0        0        0     4083 1970-01-01 00:00:00.000000 telegram_text-0.1.2/PKG-INFO
```

### Comparing `telegram_text-0.1.1/LICENSE` & `telegram_text-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_text-0.1.1/README.md` & `telegram_text-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ### Installation
 Install using `pip install telegram-text` or `poetry add telegram-text`
 
 Also, `telegram-text` is integrated into following packages:
 
 | Module | Installation | Import | Documentation |
 | ------ | ------------ | ------ | ------------- |
+| [python-telegram](https://github.com/alexander-akhmetov/python-telegram) | `pip install python-telegram` | `from telegram.text import ...` | [Readme](https://github.com/alexander-akhmetov/python-telegram/blob/master/README.md) |
 | [OrigamiBot](https://github.com/cmd410/OrigamiBot) | `pip install origamibot[telegram-text]` | `from origamibot.text import ...` | [Release](https://github.com/cmd410/OrigamiBot/releases/tag/v2.3.0) |
 | [TGramBot](https://github.com/KeralaBots/TGramBot) | `pip install tgrambot` | `from tgrambot.text import ...` | [Readme](https://github.com/KeralaBots/TGramBot/blob/alpha/README.md) |
 
 ### Basic Example
 
 ```python
 from telegram_text import Bold, Italic, Underline
```

### Comparing `telegram_text-0.1.1/pyproject.toml` & `telegram_text-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 [tool.poetry]
 name = "telegram_text"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python markup module for Telegram messenger. This module provides a rich list of components to build any possible markup fast and render it to specific html or MarkdownV2 formats."
 authors = ["Vladimir Alinsky <Vladimir@Alinsky.tech>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://telegram-text.alinsky.tech"
 repository = "https://github.com/SKY-ALIN/telegram-text"
 keywords = ["telegram", "markup", "markdown", "formating"]
-include = [
-    "LICENSE",
-]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.0"
+pytest = "^7.3.1"
 pylint = "^2.13.9"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 Sphinx = "^4"
 flake8 = "^5.0.4"
 furo = "^2022.9.29"
 m2r2 = "^0.3.2"
-sphinx-copybutton = "^0.5.0"
+sphinx-copybutton = "^0.5.2"
 no-optional = "^0.4.0"
-isort = "^5.11.4"
-mypy = "^0.991"
+isort = "^5.11.5"
+mypy = "^1.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `telegram_text-0.1.1/telegram_text/__init__.py` & `telegram_text-0.1.2/telegram_text/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .bases import Chain, PlainText, Text
 from .custom import TOMLSection
 from .elements import Hashtag, InlineUser, Link, User
 from .markdown import OrderedList, UnorderedList
 from .styles import Bold, Code, InlineCode, Italic, Spoiler, Strikethrough, Underline
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 __all__ = [
     "Chain",
     "PlainText",
     "Text",
 
     "Bold",
     "Code",
```

### Comparing `telegram_text-0.1.1/telegram_text/bases.py` & `telegram_text-0.1.2/telegram_text/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         return self.text
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: '{self.text}'>"
 
 
 class PlainText(Text):
-    """Basic text element you can safety use. This element implements escaping
+    """Basic text element you can safely use. This element implements escaping
     logic.
     """
 
     escaping_chars = ('_', '*', '[', ']', '(', ')', '~', '`', '>', '#', '+', '-', '=', '|', '{', '}', '.', '!')
     """Tuple of character that will be escaped according to Telegram specification."""
 
     def _escape(self, text: str) -> str:
```

### Comparing `telegram_text-0.1.1/telegram_text/custom.py` & `telegram_text-0.1.2/telegram_text/custom.py`

 * *Files identical despite different names*

### Comparing `telegram_text-0.1.1/telegram_text/elements.py` & `telegram_text-0.1.2/telegram_text/elements.py`

 * *Files identical despite different names*

### Comparing `telegram_text-0.1.1/telegram_text/markdown.py` & `telegram_text-0.1.2/telegram_text/markdown.py`

 * *Files identical despite different names*

### Comparing `telegram_text-0.1.1/telegram_text/styles.py` & `telegram_text-0.1.2/telegram_text/styles.py`

 * *Files identical despite different names*

### Comparing `telegram_text-0.1.1/PKG-INFO` & `telegram_text-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: telegram-text
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python markup module for Telegram messenger. This module provides a rich list of components to build any possible markup fast and render it to specific html or MarkdownV2 formats.
 Home-page: https://telegram-text.alinsky.tech
 License: MIT
 Keywords: telegram,markup,markdown,formating
 Author: Vladimir Alinsky
 Author-email: Vladimir@Alinsky.tech
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/SKY-ALIN/telegram-text
 Description-Content-Type: text/markdown
 
 # telegram-text
 **Python markup module for Telegram messenger.
 This module provides a rich list of components to build any possible
 markup fast and render it to specific _html_ and _MarkdownV2_ formats.**
@@ -36,14 +36,15 @@
 ### Installation
 Install using `pip install telegram-text` or `poetry add telegram-text`
 
 Also, `telegram-text` is integrated into following packages:
 
 | Module | Installation | Import | Documentation |
 | ------ | ------------ | ------ | ------------- |
+| [python-telegram](https://github.com/alexander-akhmetov/python-telegram) | `pip install python-telegram` | `from telegram.text import ...` | [Readme](https://github.com/alexander-akhmetov/python-telegram/blob/master/README.md) |
 | [OrigamiBot](https://github.com/cmd410/OrigamiBot) | `pip install origamibot[telegram-text]` | `from origamibot.text import ...` | [Release](https://github.com/cmd410/OrigamiBot/releases/tag/v2.3.0) |
 | [TGramBot](https://github.com/KeralaBots/TGramBot) | `pip install tgrambot` | `from tgrambot.text import ...` | [Readme](https://github.com/KeralaBots/TGramBot/blob/alpha/README.md) |
 
 ### Basic Example
 
 ```python
 from telegram_text import Bold, Italic, Underline
```

