# Comparing `tmp/rich_argparse-1.1.0.tar.gz` & `tmp/rich_argparse-1.1.1.tar.gz`

## Comparing `rich_argparse-1.1.0.tar` & `rich_argparse-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    20947 2020-02-02 00:00:00.000000 rich_argparse-1.1.0/rich_argparse.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 rich_argparse-1.1.0/rich_argparse-stubs/__init__.pyi
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rich_argparse-1.1.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rich_argparse-1.1.0/LICENSE
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 rich_argparse-1.1.0/README.md
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rich_argparse-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 rich_argparse-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    21224 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/rich_argparse.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/rich_argparse-stubs/__init__.pyi
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/LICENSE
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/README.md
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/PKG-INFO
```

### Comparing `rich_argparse-1.1.0/rich_argparse.py` & `rich_argparse-1.1.1/rich_argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,34 +79,44 @@
     def __init__(
         self,
         prog: str,
         indent_increment: int = 2,
         max_help_position: int = 24,
         width: int | None = None,
     ) -> None:
-        from rich.console import Console
-        from rich.theme import Theme
-
         super().__init__(prog, indent_increment, max_help_position, width)
-        self.console = Console(theme=Theme(self.styles))
+        self._console: Console | None = None
 
         # https://docs.python.org/3/library/stdtypes.html#printf-style-string-formatting
         self._printf_style_pattern = re.compile(
             r"""
             %                               # Percent character
-            (?:\((?P<mapping>[^)]*)\))      # Mapping key (not optional for argparse)
+            (?:\((?P<mapping>[^)]*)\))?     # Mapping key
             (?P<flag>[#0\-+ ])?             # Conversion Flags
             (?P<width>\*|\d+)?              # Minimum field width
             (?P<precision>\.(?:\*?|\d*))?   # Precision
             [hlL]?                          # Length modifier (ignored)
             (?P<format>[diouxXeEfFgGcrsa%]) # Conversion type
             """,
             re.VERBOSE,
         )
 
+    @property
+    def console(self) -> Console:  # deprecate?
+        if self._console is None:
+            from rich.console import Console
+            from rich.theme import Theme
+
+            self._console = Console(theme=Theme(self.styles))
+        return self._console
+
+    @console.setter
+    def console(self, console: Console) -> None:  # is this needed?
+        self._console = console
+
     class _Section(argparse.HelpFormatter._Section):  # type: ignore[misc]
         def __init__(
             self, formatter: RichHelpFormatter, parent: Self | None, heading: str | None = None
         ) -> None:
             if heading is not None:
                 heading = f"{type(formatter).group_name_formatter(heading)}:"
             super().__init__(formatter, parent, heading)
```

### Comparing `rich_argparse-1.1.0/rich_argparse-stubs/__init__.pyi` & `rich_argparse-1.1.1/rich_argparse-stubs/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 from rich.text import Span, Text
 
 class RichHelpFormatter(argparse.HelpFormatter):
     group_name_formatter: ClassVar[Callable[[str], str]]
     styles: ClassVar[dict[str, StyleType]]
     highlights: ClassVar[list[str]]
     usage_markup: ClassVar[bool]
-    console: Console
+    _console: Console | None
     _printf_style_pattern: re.Pattern[str]
 
     class _Section(argparse.HelpFormatter._Section):  # type: ignore[misc]
         rich_items: list[RenderableType]
         rich_actions: list[tuple[Text, Text | None]]
         def __init__(
             self, formatter: RichHelpFormatter, parent: Self | None, heading: str | None = None
         ) -> None: ...
         def __rich_console__(self, console: Console, options: ConsoleOptions) -> RenderResult: ...
 
+    @property
+    def console(self) -> Console: ...
+    @console.setter
+    def console(self, console: Console) -> None: ...
     def _rich_prog_spans(self, usage: str) -> Iterator[Span]: ...
     def _rich_usage_spans(
         self, text: str, start: int, actions: Iterable[Action]
     ) -> Iterator[Span]: ...
     def _rich_whitespace_sub(self, text: Text) -> Text: ...
     def _rich_expand_help(self, action: Action) -> Text: ...
     def _rich_format_text(self, text: str) -> Text: ...
```

### Comparing `rich_argparse-1.1.0/LICENSE` & `rich_argparse-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_argparse-1.1.0/README.md` & `rich_argparse-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rich_argparse-1.1.0/pyproject.toml` & `rich_argparse-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.11.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rich_argparse"
-version = "1.1.0"
+version = "1.1.1"
 description = "A rich help formatter for argparse"
 authors = [
   {name="Ali Hamdan", email="ali.hamdan.dev@gmail.com"},
 ]
 readme = "README.md"
 license = "MIT"
 classifiers = [
@@ -47,18 +47,15 @@
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py37,py38,py39,py310,py311,py312
 skip_missing_interpreters = true
 
 [testenv]
-deps =
-  pytest
-  coverage[toml]
-  covdefaults
+deps = -rtests/requirements.txt
 commands =
   coverage run -m pytest {posargs}
   coverage report
   coverage html
 """
 
 [tool.black]
```

### Comparing `rich_argparse-1.1.0/PKG-INFO` & `rich_argparse-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich_argparse
-Version: 1.1.0
+Version: 1.1.1
 Summary: A rich help formatter for argparse
 Project-URL: Homepage, https://github.com/hamdanal/rich-argparse
 Project-URL: Documentation, https://github.com/hamdanal/rich-argparse#rich-argparse
 Project-URL: Issue-Tracker, https://github.com/hamdanal/rich-argparse/issues
 Project-URL: Changelog, https://github.com/hamdanal/rich-argparse/blob/main/CHANGELOG.md
 Author-email: Ali Hamdan <ali.hamdan.dev@gmail.com>
 License-Expression: MIT
```

