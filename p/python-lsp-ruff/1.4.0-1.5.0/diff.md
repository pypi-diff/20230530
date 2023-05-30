# Comparing `tmp/python-lsp-ruff-1.4.0.tar.gz` & `tmp/python-lsp-ruff-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lsp-ruff-1.4.0.tar", last modified: Tue Apr 11 13:35:16 2023, max compression
+gzip compressed data, was "python-lsp-ruff-1.5.0.tar", last modified: Tue May 30 09:06:21 2023, max compression
```

## Comparing `python-lsp-ruff-1.4.0.tar` & `python-lsp-ruff-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/
--rw-r--r--   0 juli      (1000) juli      (1000)     1138 2022-12-05 16:14:35.000000 python-lsp-ruff-1.4.0/LICENSE
--rw-r--r--   0 juli      (1000) juli      (1000)     3732 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/PKG-INFO
--rw-r--r--   0 juli      (1000) juli      (1000)     3312 2023-04-11 13:29:01.000000 python-lsp-ruff-1.4.0/README.md
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-11 13:35:16.681051 python-lsp-ruff-1.4.0/pylsp_ruff/
--rw-r--r--   0 juli      (1000) juli      (1000)        0 2022-12-01 22:28:29.000000 python-lsp-ruff-1.4.0/pylsp_ruff/__init__.py
--rw-r--r--   0 juli      (1000) juli      (1000)    16250 2023-04-11 13:29:01.000000 python-lsp-ruff-1.4.0/pylsp_ruff/plugin.py
--rw-r--r--   0 juli      (1000) juli      (1000)      436 2023-04-02 21:39:03.000000 python-lsp-ruff-1.4.0/pylsp_ruff/ruff.py
--rw-r--r--   0 juli      (1000) juli      (1000)     1628 2023-04-10 17:55:44.000000 python-lsp-ruff-1.4.0/pylsp_ruff/settings.py
--rw-r--r--   0 juli      (1000) juli      (1000)      876 2023-04-11 13:31:40.000000 python-lsp-ruff-1.4.0/pyproject.toml
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/
--rw-r--r--   0 juli      (1000) juli      (1000)     3732 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/PKG-INFO
--rw-r--r--   0 juli      (1000) juli      (1000)      414 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/SOURCES.txt
--rw-r--r--   0 juli      (1000) juli      (1000)        1 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/dependency_links.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       33 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/entry_points.txt
--rw-r--r--   0 juli      (1000) juli      (1000)      121 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/requires.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       11 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/top_level.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       38 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/setup.cfg
--rw-r--r--   0 juli      (1000) juli      (1000)       69 2023-01-14 19:42:55.000000 python-lsp-ruff-1.4.0/setup.py
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/tests/
--rw-r--r--   0 juli      (1000) juli      (1000)     3960 2023-04-11 11:39:49.000000 python-lsp-ruff-1.4.0/tests/test_code_actions.py
--rw-r--r--   0 juli      (1000) juli      (1000)     6832 2023-04-10 17:38:09.000000 python-lsp-ruff-1.4.0/tests/test_ruff_lint.py
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/
+-rw-r--r--   0 juli      (1000) juli      (1000)     1138 2022-12-05 16:14:35.000000 python-lsp-ruff-1.5.0/LICENSE
+-rw-r--r--   0 juli      (1000) juli      (1000)     4733 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/PKG-INFO
+-rw-r--r--   0 juli      (1000) juli      (1000)     4313 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/README.md
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-30 09:06:21.781838 python-lsp-ruff-1.5.0/pylsp_ruff/
+-rw-r--r--   0 juli      (1000) juli      (1000)        0 2022-12-01 22:28:29.000000 python-lsp-ruff-1.5.0/pylsp_ruff/__init__.py
+-rw-r--r--   0 juli      (1000) juli      (1000)    17445 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/pylsp_ruff/plugin.py
+-rw-r--r--   0 juli      (1000) juli      (1000)      436 2023-05-30 07:34:43.000000 python-lsp-ruff-1.5.0/pylsp_ruff/ruff.py
+-rw-r--r--   0 juli      (1000) juli      (1000)     1677 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/pylsp_ruff/settings.py
+-rw-r--r--   0 juli      (1000) juli      (1000)      876 2023-05-30 09:01:11.000000 python-lsp-ruff-1.5.0/pyproject.toml
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/
+-rw-r--r--   0 juli      (1000) juli      (1000)     4733 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/PKG-INFO
+-rw-r--r--   0 juli      (1000) juli      (1000)      414 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/SOURCES.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)        1 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/dependency_links.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       33 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/entry_points.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)      121 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/requires.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       11 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/top_level.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       38 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/setup.cfg
+-rw-r--r--   0 juli      (1000) juli      (1000)       69 2023-01-14 19:42:55.000000 python-lsp-ruff-1.5.0/setup.py
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/tests/
+-rw-r--r--   0 juli      (1000) juli      (1000)     4179 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/tests/test_code_actions.py
+-rw-r--r--   0 juli      (1000) juli      (1000)     7100 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/tests/test_ruff_lint.py
```

### Comparing `python-lsp-ruff-1.4.0/LICENSE` & `python-lsp-ruff-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-1.4.0/PKG-INFO` & `python-lsp-ruff-1.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: python-lsp-ruff
-Version: 1.4.0
-Summary: Ruff linting plugin for pylsp
-Author-email: Julian Hossbach <julian.hossbach@gmx.de>
-License: MIT
-Project-URL: Homepage, https://github.com/python-lsp/python-lsp-ruff
-Project-URL: Bug Tracker, https://github.com/python-lsp/python-lsp-ruff/issues
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # python-lsp-ruff
 
 [![PyPi](https://img.shields.io/pypi/v/python-lsp-ruff.svg)](https://pypi.org/project/python-lsp-ruff)
 [![Anaconda](https://anaconda.org/conda-forge/python-lsp-ruff/badges/version.svg)](https://anaconda.org/conda-forge/python-lsp-ruff)
 [![Python](https://github.com/python-lsp/python-lsp-ruff/actions/workflows/python.yml/badge.svg)](https://github.com/python-lsp/python-lsp-ruff/actions/workflows/python.yml)
 
 `python-lsp-ruff` is a plugin for `python-lsp-server` that adds linting, code action and formatting capabilities that are provided by [ruff](https://github.com/charliermarsh/ruff),
@@ -75,9 +62,21 @@
  - `pylsp.plugins.ruff.ignore`: Error codes to ignore.
  - `pylsp.plugins.ruff.extendIgnore`: Same as ignore, but append to existing ignores.
  - `pylsp.plugins.ruff.lineLength`: Set the line-length for length checks.
  - `pylsp.plugins.ruff.perFileIgnores`: File-specific error codes to be ignored.
  - `pylsp.plugins.ruff.select`: List of error codes to enable.
  - `pylsp.plugins.ruff.extendSelect`: Same as select, but append to existing error codes.
  - `pylsp.plugins.ruff.format`: List of error codes to fix during formatting. The default is `["I"]`, any additional codes are appended to this list.
+ - `pylsp.plugins.ruff.severities`: Dictionary of custom severity levels for specific codes, see [below](#custom-severities).
 
 For more information on the configuration visit [Ruff's homepage](https://beta.ruff.rs/docs/configuration/).
+
+## Custom severities
+
+By default all diagnostics are marked as warning, except for `"E999"` and all error codes starting with `"F"`, which are displayed as errors.
+This default can be changed through the `pylsp.plugins.ruff.severities` option, which takes the error code as a key and any of
+`"E"`, `"W"`, `"I"` and `"H"` to be displayed as errors, warnings, information and hints, respectively.
+For more information on the diagnostic severities please refer to
+[the official LSP reference](https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#diagnosticSeverity).
+
+Note that `python-lsp-ruff` does *not* accept regex, and it will *not* check whether the error code exists. If the custom severity level is not displayed,
+please check first that the error code is correct and that the given value is one of the possible keys from above.
```

### Comparing `python-lsp-ruff-1.4.0/README.md` & `python-lsp-ruff-1.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: python-lsp-ruff
+Version: 1.5.0
+Summary: Ruff linting plugin for pylsp
+Author-email: Julian Hossbach <julian.hossbach@gmx.de>
+License: MIT
+Project-URL: Homepage, https://github.com/python-lsp/python-lsp-ruff
+Project-URL: Bug Tracker, https://github.com/python-lsp/python-lsp-ruff/issues
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # python-lsp-ruff
 
 [![PyPi](https://img.shields.io/pypi/v/python-lsp-ruff.svg)](https://pypi.org/project/python-lsp-ruff)
 [![Anaconda](https://anaconda.org/conda-forge/python-lsp-ruff/badges/version.svg)](https://anaconda.org/conda-forge/python-lsp-ruff)
 [![Python](https://github.com/python-lsp/python-lsp-ruff/actions/workflows/python.yml/badge.svg)](https://github.com/python-lsp/python-lsp-ruff/actions/workflows/python.yml)
 
 `python-lsp-ruff` is a plugin for `python-lsp-server` that adds linting, code action and formatting capabilities that are provided by [ruff](https://github.com/charliermarsh/ruff),
@@ -62,9 +75,21 @@
  - `pylsp.plugins.ruff.ignore`: Error codes to ignore.
  - `pylsp.plugins.ruff.extendIgnore`: Same as ignore, but append to existing ignores.
  - `pylsp.plugins.ruff.lineLength`: Set the line-length for length checks.
  - `pylsp.plugins.ruff.perFileIgnores`: File-specific error codes to be ignored.
  - `pylsp.plugins.ruff.select`: List of error codes to enable.
  - `pylsp.plugins.ruff.extendSelect`: Same as select, but append to existing error codes.
  - `pylsp.plugins.ruff.format`: List of error codes to fix during formatting. The default is `["I"]`, any additional codes are appended to this list.
+ - `pylsp.plugins.ruff.severities`: Dictionary of custom severity levels for specific codes, see [below](#custom-severities).
 
 For more information on the configuration visit [Ruff's homepage](https://beta.ruff.rs/docs/configuration/).
+
+## Custom severities
+
+By default all diagnostics are marked as warning, except for `"E999"` and all error codes starting with `"F"`, which are displayed as errors.
+This default can be changed through the `pylsp.plugins.ruff.severities` option, which takes the error code as a key and any of
+`"E"`, `"W"`, `"I"` and `"H"` to be displayed as errors, warnings, information and hints, respectively.
+For more information on the diagnostic severities please refer to
+[the official LSP reference](https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#diagnosticSeverity).
+
+Note that `python-lsp-ruff` does *not* accept regex, and it will *not* check whether the error code exists. If the custom severity level is not displayed,
+please check first that the error code is correct and that the given value is one of the possible keys from above.
```

### Comparing `python-lsp-ruff-1.4.0/pylsp_ruff/plugin.py` & `python-lsp-ruff-1.5.0/pylsp_ruff/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,14 +49,21 @@
     "F401",  # `module` imported but unused
     "F504",  # % format unused named arguments
     "F522",  # .format(...) unused named arguments
     "F523",  # .format(...) unused positional arguments
     "F841",  # local variable `name` is assigned to but never used
 }
 
+DIAGNOSTIC_SEVERITIES = {
+    "E": DiagnosticSeverity.Error,
+    "W": DiagnosticSeverity.Warning,
+    "I": DiagnosticSeverity.Information,
+    "H": DiagnosticSeverity.Hint,
+}
+
 
 @hookimpl
 def pylsp_settings():
     log.debug("Initializing pylsp_ruff")
     # this plugin disables flake8, mccabe, and pycodestyle by default
     settings = {
         "plugins": {
@@ -87,15 +94,18 @@
     outcome = yield
     result = outcome.get_result()
     if result:
         source = result[0]["newText"]
     else:
         source = document.source
 
-    new_text = run_ruff_format(workspace, document.path, document_source=source)
+    settings = load_settings(workspace=workspace, document_path=document.path)
+    new_text = run_ruff_format(
+        settings=settings, document_path=document.path, document_source=source
+    )
 
     # Avoid applying empty text edit
     if new_text == source:
         return
 
     range = Range(
         start=Position(line=0, character=0),
@@ -118,20 +128,21 @@
     document : pylsp.workspace.Document
         Document to apply ruff on.
 
     Returns
     -------
     List of dicts containing the diagnostics.
     """
-    checks = run_ruff_check(workspace, document)
-    diagnostics = [create_diagnostic(c) for c in checks]
+    settings = load_settings(workspace, document.path)
+    checks = run_ruff_check(document=document, settings=settings)
+    diagnostics = [create_diagnostic(check=c, settings=settings) for c in checks]
     return converter.unstructure(diagnostics)
 
 
-def create_diagnostic(check: RuffCheck) -> Diagnostic:
+def create_diagnostic(check: RuffCheck, settings: PluginSettings) -> Diagnostic:
     # Adapt range to LSP specification (zero-based)
     range = Range(
         start=Position(
             line=check.location.row - 1,
             character=check.location.column - 1,
         ),
         end=Position(
@@ -142,14 +153,20 @@
 
     # Ruff intends to implement severity codes in the future,
     # see https://github.com/charliermarsh/ruff/issues/645.
     severity = DiagnosticSeverity.Warning
     if check.code == "E999" or check.code[0] == "F":
         severity = DiagnosticSeverity.Error
 
+    # Override severity with custom severity if possible, use default otherwise
+    if settings.severities is not None:
+        custom_sev = settings.severities.get(check.code, None)
+        if custom_sev is not None:
+            severity = DIAGNOSTIC_SEVERITIES.get(custom_sev, severity)
+
     tags = []
     if check.code in UNNECESSITY_CODES:
         tags = [DiagnosticTag.Unnecessary]
 
     return Diagnostic(
         source=DIAGNOSTIC_SOURCE,
         code=check.code,
@@ -189,50 +206,61 @@
     -------
     List of dicts containing the code actions.
     """
     log.debug(f"textDocument/codeAction: {document} {range} {context}")
 
     _context = converter.structure(context, CodeActionContext)
     diagnostics = _context.diagnostics
-    diagnostics_with_fixes = [d for d in diagnostics if d.data]
 
     code_actions = []
     has_organize_imports = False
 
-    for diagnostic in diagnostics_with_fixes:
-        fix = converter.structure(diagnostic.data, RuffFix)
+    for diagnostic in diagnostics:
+        code_actions.append(
+            create_disable_code_action(document=document, diagnostic=diagnostic)
+        )
+
+        if diagnostic.data:  # Has fix
+            fix = converter.structure(diagnostic.data, RuffFix)
 
-        if diagnostic.code == "I001":
-            code_actions.append(
-                create_organize_imports_code_action(document, diagnostic, fix)
-            )
-            has_organize_imports = True
-        else:
-            code_actions.extend(
-                [
-                    create_fix_code_action(document, diagnostic, fix),
-                    create_disable_code_action(document, diagnostic),
-                ]
-            )
+            if diagnostic.code == "I001":
+                code_actions.append(
+                    create_organize_imports_code_action(
+                        document=document, diagnostic=diagnostic, fix=fix
+                    )
+                )
+                has_organize_imports = True
+            else:
+                code_actions.append(
+                    create_fix_code_action(
+                        document=document, diagnostic=diagnostic, fix=fix
+                    ),
+                )
 
-    checks = run_ruff_check(workspace, document)
+    settings = load_settings(workspace=workspace, document_path=document.path)
+    checks = run_ruff_check(document=document, settings=settings)
     checks_with_fixes = [c for c in checks if c.fix]
     checks_organize_imports = [c for c in checks_with_fixes if c.code == "I001"]
 
     if not has_organize_imports and checks_organize_imports:
         check = checks_organize_imports[0]
         fix = check.fix  # type: ignore
-        diagnostic = create_diagnostic(check)
-        code_actions.append(
-            create_organize_imports_code_action(document, diagnostic, fix),
+        diagnostic = create_diagnostic(check=check, settings=settings)
+        code_actions.extend(
+            [
+                create_organize_imports_code_action(
+                    document=document, diagnostic=diagnostic, fix=fix
+                ),
+                create_disable_code_action(document=document, diagnostic=diagnostic),
+            ]
         )
 
     if checks_with_fixes:
         code_actions.append(
-            create_fix_all_code_action(workspace, document),
+            create_fix_all_code_action(document=document, settings=settings),
         )
 
     return converter.unstructure(code_actions)
 
 
 def create_fix_code_action(
     document: Document,
@@ -302,21 +330,21 @@
         kind=kind,
         diagnostics=[diagnostic],
         edit=workspace_edit,
     )
 
 
 def create_fix_all_code_action(
-    workspace: Workspace,
     document: Document,
+    settings: PluginSettings,
 ) -> CodeAction:
     title = "Ruff: Fix All"
     kind = CodeActionKind.SourceFixAll
 
-    new_text = run_ruff_fix(workspace, document)
+    new_text = run_ruff_fix(document=document, settings=settings)
     range = Range(
         start=Position(line=0, character=0),
         end=Position(line=len(document.lines), character=0),
     )
     text_edit = TextEdit(range=range, new_text=new_text)
     workspace_edit = WorkspaceEdit(changes={document.uri: [text_edit]})
     return CodeAction(
@@ -328,95 +356,97 @@
 
 def create_text_edits(fix: RuffFix) -> List[TextEdit]:
     edits = []
     for edit in fix.edits:
         range = Range(
             start=Position(
                 line=edit.location.row - 1,
-                character=edit.location.column,  # yes, no -1
+                character=edit.location.column - 1,
             ),
             end=Position(
                 line=edit.end_location.row - 1,
-                character=edit.end_location.column,  # yes, no -1
+                character=edit.end_location.column - 1,
             ),
         )
         edits.append(TextEdit(range=range, new_text=edit.content))
     return edits
 
 
-def run_ruff_check(workspace: Workspace, document: Document) -> List[RuffCheck]:
+def run_ruff_check(document: Document, settings: PluginSettings) -> List[RuffCheck]:
     result = run_ruff(
-        workspace, document_path=document.path, document_source=document.source
+        document_path=document.path,
+        document_source=document.source,
+        settings=settings,
     )
     try:
         result = json.loads(result)
     except json.JSONDecodeError:
         result = []  # type: ignore
     return converter.structure(result, List[RuffCheck])
 
 
-def run_ruff_fix(workspace: Workspace, document: Document) -> str:
+def run_ruff_fix(document: Document, settings: PluginSettings) -> str:
     result = run_ruff(
-        workspace,
         document_path=document.path,
         document_source=document.source,
         fix=True,
+        settings=settings,
     )
     return result
 
 
 def run_ruff_format(
-    workspace: Workspace, document_path: str, document_source: str
+    settings: PluginSettings,
+    document_path: str,
+    document_source: str,
 ) -> str:
-    settings = load_settings(workspace, document_path)
     fixable_codes = ["I"]
     if settings.format:
         fixable_codes.extend(settings.format)
     extra_arguments = [
         f"--fixable={','.join(fixable_codes)}",
     ]
     result = run_ruff(
-        workspace,
-        document_path,
-        document_source,
+        settings=settings,
+        document_path=document_path,
+        document_source=document_source,
         fix=True,
         extra_arguments=extra_arguments,
     )
     return result
 
 
 def run_ruff(
-    workspace: Workspace,
+    settings: PluginSettings,
     document_path: str,
     document_source: str,
     fix: bool = False,
     extra_arguments: Optional[List[str]] = None,
 ) -> str:
     """
     Run ruff on the given document and the given arguments.
 
     Parameters
     ----------
-    workspace : pyls.workspace.Workspace
-        Workspace to run ruff in.
+    settings : PluginSettings
+        Settings to use.
     document_path : str
         Path to file to run ruff on.
     document_source : str
         Document source or to apply ruff on.
         Needed when the source differs from the file source, e.g. during formatting.
     fix : bool
         Whether to run fix or no-fix.
     extra_arguments : List[str]
         Extra arguments to pass to ruff.
 
     Returns
     -------
     String containing the result in json format.
     """
-    settings = load_settings(workspace, document_path)
     executable = settings.executable
     arguments = build_arguments(document_path, settings, fix, extra_arguments)
 
     log.debug(f"Calling {executable} with args: {arguments} on '{document_path}'")
     try:
         cmd = [executable]
         cmd.extend(arguments)
@@ -552,10 +582,11 @@
         # Leave config to pyproject.toml
         return PluginSettings(
             enabled=plugin_settings.executable,
             executable=plugin_settings.executable,
             extend_ignore=plugin_settings.extend_ignore,
             extend_select=plugin_settings.extend_select,
             format=plugin_settings.format,
+            severities=plugin_settings.severities,
         )
 
     return plugin_settings
```

### Comparing `python-lsp-ruff-1.4.0/pylsp_ruff/settings.py` & `python-lsp-ruff-1.5.0/pylsp_ruff/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
     ignore: Optional[List[str]] = None
     extend_ignore: Optional[List[str]] = None
     per_file_ignores: Optional[Dict[str, List[str]]] = None
 
     format: Optional[List[str]] = None
 
+    severities: Optional[Dict[str, str]] = None
+
 
 def to_camel_case(snake_str: str) -> str:
     components = snake_str.split("_")
     return components[0] + "".join(x.title() for x in components[1:])
 
 
 def to_camel_case_unstructure(converter, klass):
```

### Comparing `python-lsp-ruff-1.4.0/pyproject.toml` & `python-lsp-ruff-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-lsp-ruff"
 authors = [
   {name = "Julian Hossbach", email = "julian.hossbach@gmx.de"}
 ]
-version = "1.4.0"
+version = "1.5.0"
 description = "Ruff linting plugin for pylsp"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
 dependencies = [
   "ruff>=0.0.260",
   "python-lsp-server",
```

### Comparing `python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/PKG-INFO` & `python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-ruff
-Version: 1.4.0
+Version: 1.5.0
 Summary: Ruff linting plugin for pylsp
 Author-email: Julian Hossbach <julian.hossbach@gmx.de>
 License: MIT
 Project-URL: Homepage, https://github.com/python-lsp/python-lsp-ruff
 Project-URL: Bug Tracker, https://github.com/python-lsp/python-lsp-ruff/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -75,9 +75,21 @@
  - `pylsp.plugins.ruff.ignore`: Error codes to ignore.
  - `pylsp.plugins.ruff.extendIgnore`: Same as ignore, but append to existing ignores.
  - `pylsp.plugins.ruff.lineLength`: Set the line-length for length checks.
  - `pylsp.plugins.ruff.perFileIgnores`: File-specific error codes to be ignored.
  - `pylsp.plugins.ruff.select`: List of error codes to enable.
  - `pylsp.plugins.ruff.extendSelect`: Same as select, but append to existing error codes.
  - `pylsp.plugins.ruff.format`: List of error codes to fix during formatting. The default is `["I"]`, any additional codes are appended to this list.
+ - `pylsp.plugins.ruff.severities`: Dictionary of custom severity levels for specific codes, see [below](#custom-severities).
 
 For more information on the configuration visit [Ruff's homepage](https://beta.ruff.rs/docs/configuration/).
+
+## Custom severities
+
+By default all diagnostics are marked as warning, except for `"E999"` and all error codes starting with `"F"`, which are displayed as errors.
+This default can be changed through the `pylsp.plugins.ruff.severities` option, which takes the error code as a key and any of
+`"E"`, `"W"`, `"I"` and `"H"` to be displayed as errors, warnings, information and hints, respectively.
+For more information on the diagnostic severities please refer to
+[the official LSP reference](https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#diagnosticSeverity).
+
+Note that `python-lsp-ruff` does *not* accept regex, and it will *not* check whether the error code exists. If the custom severity level is not displayed,
+please check first that the error code is correct and that the given value is one of the possible keys from above.
```

### Comparing `python-lsp-ruff-1.4.0/tests/test_code_actions.py` & `python-lsp-ruff-1.5.0/tests/test_code_actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     "Ruff (F841): Disable for this line",
     "Ruff: Fix All",
 ]
 
 codeactions_import = [
     "Ruff: Organize imports",
     "Ruff: Fix All",
+    "Ruff (I001): Disable for this line",
 ]
 
 
 def temp_document(doc_text, workspace):
     with tempfile.NamedTemporaryFile(
         mode="w", dir=workspace.root_path, delete=False
     ) as temp_file:
@@ -111,22 +112,24 @@
     expected_str = dedent(
         """
         def f():
             pass
         """
     )
     _, doc = temp_document(codeaction_str, workspace)
-    fixed_str = ruff_lint.run_ruff_fix(workspace, doc)
+    settings = ruff_lint.load_settings(workspace, doc.path)
+    fixed_str = ruff_lint.run_ruff_fix(doc, settings)
     assert fixed_str == expected_str
 
 
 def test_format_document_default_settings(workspace):
     _, doc = temp_document(import_str, workspace)
+    settings = ruff_lint.load_settings(workspace, doc.path)
     formatted_str = ruff_lint.run_ruff_format(
-        workspace, document_path=doc.path, document_source=doc.source
+        settings, document_path=doc.path, document_source=doc.source
     )
     assert formatted_str == import_str
 
 
 def test_format_document_settings(workspace):
     expected_str = dedent(
         """
@@ -141,11 +144,12 @@
                     "select": ["I"],
                     "format": ["I001"],
                 }
             }
         }
     )
     _, doc = temp_document(import_str, workspace)
+    settings = ruff_lint.load_settings(workspace, doc.path)
     formatted_str = ruff_lint.run_ruff_format(
-        workspace, document_path=doc.path, document_source=doc.source
+        settings, document_path=doc.path, document_source=doc.source
     )
     assert formatted_str == expected_str
```

### Comparing `python-lsp-ruff-1.4.0/tests/test_ruff_lint.py` & `python-lsp-ruff-1.5.0/tests/test_ruff_lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,14 +186,15 @@
     ]
 
     workspace._config.update(
         {
             "plugins": {
                 "ruff": {
                     "extendIgnore": ["D104"],
+                    "severities": {"E402": "E", "D103": "I"},
                 }
             }
         }
     )
 
     diags = ruff_lint.pylsp_lint(workspace, doc)
 
@@ -202,14 +203,21 @@
         _list.append(diag["code"])
     # Assert that ignore, extend-ignore and extend-select is working as intended
     assert "E402" in _list
     assert "D103" in _list
     assert "D104" not in _list
     assert "F841" not in _list
 
+    # Check custom severities
+    for diag in diags:
+        if diag["code"] == "E402":
+            assert diag["severity"] == 1
+        if diag["code"] == "D103":
+            assert diag["severity"] == 3
+
     # Excludes
     doc_uri = uris.from_fs_path(os.path.join(workspace.root_path, "blah/__init__.py"))
     workspace.put_document(doc_uri, doc_str)
 
     ruff_settings = get_ruff_settings(
         workspace, workspace.get_document(doc_uri), config_str
     )
```

