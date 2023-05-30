# Comparing `tmp/nettowel-0.5.0.tar.gz` & `tmp/nettowel-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettowel-0.5.0.tar", max compression
+gzip compressed data, was "nettowel-0.5.1.tar", max compression
```

## Comparing `nettowel-0.5.0.tar` & `nettowel-0.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11357 2022-07-23 13:31:35.813924 nettowel-0.5.0/LICENSE
--rw-r--r--   0        0        0     3568 2022-07-23 13:31:54.410173 nettowel-0.5.0/README.md
--rw-r--r--   0        0        0       39 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/__init__.py
--rw-r--r--   0        0        0       73 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/__main__.py
--rw-r--r--   0        0        0      441 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/_common.py
--rw-r--r--   0        0        0        0 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/__init__.py
--rw-r--r--   0        0        0     3140 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/_common.py
--rw-r--r--   0        0        0       62 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/_output.py
--rw-r--r--   0        0        0     1084 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/diff.py
--rw-r--r--   0        0        0      507 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/help.py
--rw-r--r--   0        0        0     1448 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/ip.py
--rw-r--r--   0        0        0    10255 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/jinja.py
--rw-r--r--   0        0        0      316 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/logging.py
--rw-r--r--   0        0        0     2445 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/main.py
--rw-r--r--   0        0        0      643 2022-07-23 13:31:35.821925 nettowel-0.5.0/nettowel/cli/napalm.py
--rw-r--r--   0        0        0     6929 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/cli/netmiko.py
--rw-r--r--   0        0        0      642 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/cli/nornir.py
--rw-r--r--   0        0        0     1102 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/cli/pandas.py
--rw-r--r--   0        0        0    12299 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/cli/restconf.py
--rw-r--r--   0        0        0      643 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/cli/scrapli.py
--rw-r--r--   0        0        0      655 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/cli/textfsm.py
--rw-r--r--   0        0        0     3908 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/cli/ttp.py
--rw-r--r--   0        0        0     1125 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/cli/yaml.py
--rw-r--r--   0        0        0      931 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/exceptions.py
--rw-r--r--   0        0        0     3142 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/jinja.py
--rw-r--r--   0        0        0      133 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/logger.py
--rw-r--r--   0        0        0     2539 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/netmiko.py
--rw-r--r--   0        0        0      731 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/pandas.py
--rw-r--r--   0        0        0        0 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/py.typed
--rw-r--r--   0        0        0     2080 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/restconf.py
--rw-r--r--   0        0        0      621 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/ttp.py
--rw-r--r--   0        0        0      270 2022-07-23 13:31:35.825925 nettowel-0.5.0/nettowel/yaml.py
--rw-r--r--   0        0        0     3050 2022-07-23 13:31:35.825925 nettowel-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5325 2022-07-23 13:31:56.123779 nettowel-0.5.0/setup.py
--rw-r--r--   0        0        0     5343 2022-07-23 13:31:56.124224 nettowel-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 07:46:29.939791 nettowel-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4149 2023-05-30 07:46:53.171877 nettowel-0.5.1/README.md
+-rw-r--r--   0        0        0       39 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/__init__.py
+-rw-r--r--   0        0        0       73 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/__main__.py
+-rw-r--r--   0        0        0      441 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/_common.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/__init__.py
+-rw-r--r--   0        0        0     3140 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/_common.py
+-rw-r--r--   0        0        0       62 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/_output.py
+-rw-r--r--   0        0        0     1084 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/diff.py
+-rw-r--r--   0        0        0      507 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/help.py
+-rw-r--r--   0        0        0     1448 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/ip.py
+-rw-r--r--   0        0        0    10255 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/jinja.py
+-rw-r--r--   0        0        0      316 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/logging.py
+-rw-r--r--   0        0        0     2801 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/main.py
+-rw-r--r--   0        0        0      643 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/napalm.py
+-rw-r--r--   0        0        0     6929 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/netmiko.py
+-rw-r--r--   0        0        0      642 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/nornir.py
+-rw-r--r--   0        0        0     1102 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/pandas.py
+-rw-r--r--   0        0        0    12319 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/restconf.py
+-rw-r--r--   0        0        0      643 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/scrapli.py
+-rw-r--r--   0        0        0      655 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/textfsm.py
+-rw-r--r--   0        0        0     3908 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/ttp.py
+-rw-r--r--   0        0        0     2627 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/cli/yaml.py
+-rw-r--r--   0        0        0      986 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/exceptions.py
+-rw-r--r--   0        0        0     3142 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/jinja.py
+-rw-r--r--   0        0        0      133 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/logger.py
+-rw-r--r--   0        0        0     2659 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/netmiko.py
+-rw-r--r--   0        0        0      731 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/pandas.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/py.typed
+-rw-r--r--   0        0        0     2094 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/restconf.py
+-rw-r--r--   0        0        0      613 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/trogon_tui.py
+-rw-r--r--   0        0        0      621 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/ttp.py
+-rw-r--r--   0        0        0      799 2023-05-30 07:46:29.951791 nettowel-0.5.1/nettowel/yaml.py
+-rw-r--r--   0        0        0     2966 2023-05-30 07:46:29.951791 nettowel-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 nettowel-0.5.1/PKG-INFO
```

### Comparing `nettowel-0.5.0/LICENSE` & `nettowel-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/README.md` & `nettowel-0.5.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-# nettowel
+[![PyPI versions](https://img.shields.io/pypi/pyversions/nettowel.svg)](https://pypi.python.org/pypi/nettowel/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
+[![Downloads](https://pepy.tech/badge/nettowel)](https://pepy.tech/project/nettowel)
+
+# NetTowel
 Collection of useful network automation functions 
 
+
 > ⚠️ `nettowel` is under heavy construction and not production ready. Feedback is highly appreciated.
 
 
 ## Install
 
 You can install it directly from pypi
 
@@ -21,14 +27,15 @@
 - ttp
 - textfsm
 - napalm
 - netmiko
 - scrapli
 - nornir
 - pandas
+- tui
 
 ```bash
 pip install nettowel[jinja]
 pip install nettowel[full]
 ```
 
 ## Install from source
@@ -113,14 +120,24 @@
 ![ip info](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/ip-info.png)
 
 #### network-info
 
 ![network info](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/network-info.png)
 
 
+### YAML
+
+#### load
+
+![yaml load](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/yaml-load.png)
+
+#### dump
+
+![yaml dump](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/yaml-dump.png)
+
 ### Help
 
 ![Help QRcode](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/nettowel-help.png)
 
 
 ### Settings
 
@@ -130,32 +147,12 @@
 
 
 ### Piping
 
 ![piping](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/piping.png)
 
 
+### TUI
 
-## Building CLI Docs
-
-**At the moment `typer-cli` is not ready for typer 0.4.0**
-
-```
-typer nettowel/cli/main.py utils docs --name nettowel --output CLI.md
-```
-
-## Contributing
-
-### Run tests:
-
-```bash
-make tests
-```
-
-
-### Bump version:
+Using [Trogon](https://github.com/Textualize/trogon) a TUI (Terminal User Interface) can be generated to edit and run the NetTowel command.
 
-Steps: patch, minor, major, prepatch, preminor, premajor, prerelease.
-
-```bash
-make bump ARGS=patch
-```
+![TUI](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/trogon.png)
```

### Comparing `nettowel-0.5.0/nettowel/cli/_common.py` & `nettowel-0.5.1/nettowel/cli/_common.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/diff.py` & `nettowel-0.5.1/nettowel/cli/diff.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/ip.py` & `nettowel-0.5.1/nettowel/cli/ip.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/jinja.py` & `nettowel-0.5.1/nettowel/cli/jinja.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/main.py` & `nettowel-0.5.1/nettowel/cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from nettowel.cli.napalm import app as napalm_app
 from nettowel.cli.netmiko import app as netmiko_app
 from nettowel.cli.scrapli import app as scrapli_app
 from nettowel.cli.restconf import app as restconf_app
 from nettowel.cli.pandas import app as pandas_app
 from nettowel.cli.help import get_qrcode, HELP_MARKDOWN
 
+from nettowel.exceptions import NettowelDependencyMissing
+
 app = get_typer_app(help="Awesome collection of network automation functions")
 
 for subapp, name in [
     (ipaddress_app, "ipaddress"),
     (jinja_app, "jinja"),
     (ttp_app, "ttp"),
     (textfsm_app, "textFSM"),
@@ -70,13 +72,24 @@
         title="[blue]Help",
         expand=False,
         border_style="green",
     )
     print(top)
 
 
+@app.command(help="Textual/Trogon TUI")
+def tui(ctx: typer.Context) -> None:
+    try:
+        from nettowel.trogon_tui import run_trogon_tui
+
+        run_trogon_tui(app=app, ctx=ctx)
+    except NettowelDependencyMissing as exc:
+        typer.echo(str(exc), err=True)
+        raise typer.Exit(1)
+
+
 def run() -> None:
     app()
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `nettowel-0.5.0/nettowel/cli/napalm.py` & `nettowel-0.5.1/nettowel/cli/napalm.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/netmiko.py` & `nettowel-0.5.1/nettowel/cli/netmiko.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/nornir.py` & `nettowel-0.5.1/nettowel/cli/nornir.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/pandas.py` & `nettowel-0.5.1/nettowel/cli/pandas.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/restconf.py` & `nettowel-0.5.1/nettowel/cli/restconf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import Union, Optional
 import sys
 import typer
 from urllib.parse import quote
 from rich import print_json, print
 from rich.syntax import Syntax
 from rich.prompt import Prompt
 from rich.json import JSON
@@ -25,15 +25,15 @@
     password: str,
     port: int,
     send_xml: bool,
     return_xml: bool,
     json: bool,
     raw: bool,
     verify: bool,
-    data_file: typer.FileText = None,
+    data_file: Optional[typer.FileText] = None,
 ) -> None:
     try:
         if not user:
             user = Prompt.ask("Enter username")
         if not password:
             password = Prompt.ask(f"Enter password for user {user}", password=True)
```

### Comparing `nettowel-0.5.0/nettowel/cli/scrapli.py` & `nettowel-0.5.1/nettowel/cli/scrapli.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/textfsm.py` & `nettowel-0.5.1/nettowel/cli/textfsm.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/ttp.py` & `nettowel-0.5.1/nettowel/cli/ttp.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/cli/yaml.py` & `nettowel-0.5.1/nettowel/cli/yaml.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,96 @@
 import typer
-from rich import inspect as rich_inspect
-from rich import print_json
+from rich import print_json, print
+from rich.panel import Panel
+from rich.syntax import Syntax
+from rich.json import JSON
+
+from nettowel.cli._common import (
+    auto_complete_paths,
+    read_yaml,
+    get_typer_app,
+)
+from nettowel.yaml import dump as yaml_dump
+from nettowel.exceptions import NettowelInputError
 
-from nettowel.cli._common import get_members, cleanup_dict, get_typer_app
-
-
-app = get_typer_app(help="Templating (Jinja2) functions")
+app = get_typer_app(help="YAML functions")
 
 
 @app.command()
 def load(
     ctx: typer.Context,
-    # demo: str,
-    json: bool = typer.Option(default=False, help="json output"),
+    data_file_name: typer.FileText = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        resolve_path=True,
+        allow_dash=True,
+        metavar="YAML",
+        help="YAML Data",
+        autocompletion=auto_complete_paths,
+    ),
+    json: bool = typer.Option(False, "--json", help="JSON output"),
+    raw: bool = typer.Option(False, "--raw", help="Raw result output"),
 ) -> None:
     try:
-        raise NotImplementedError("Not Implemented Yet")
-        if json:
-            print_json(data=None)
+        data = read_yaml(data_file_name)
+        if json or raw:
+            print_json(data=data)
         else:
-            rich_inspect(None)
+            data_output = JSON.from_data(data)
+            print(Panel(data_output, title="[yellow]Data", border_style="blue"))
         raise typer.Exit(0)
-
-    except NotImplementedError as exc:
-        typer.echo(exc)
-        raise typer.Exit(1)
+    except NettowelInputError as exc:
+        typer.echo("Input is not valide", err=True)
+        typer.echo(str(exc), err=True)
+        raise typer.Exit(3)
 
 
 @app.command()
 def dump(
     ctx: typer.Context,
-    demo: str,
-    json: bool = typer.Option(default=False, help="json output"),
+    data_file_name: typer.FileText = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        resolve_path=True,
+        allow_dash=True,
+        metavar="YAML",
+        help="YAML Data",
+        autocompletion=auto_complete_paths,
+    ),
+    json: bool = typer.Option(False, "--json", help="JSON output"),
+    raw: bool = typer.Option(False, "--raw", help="Raw result output"),
 ) -> None:
     try:
-        demo_obj = {"a": 1}
-        data = get_members(demo_obj)
+        data = read_yaml(data_file_name)
+        result = yaml_dump(data).strip()
         if json:
-            print_json(data=cleanup_dict(data))
+            print_json(data={"yaml": result})
+        elif raw:
+            print(result)
         else:
-            rich_inspect(demo_obj)
+            print(
+                Panel(
+                    Syntax(
+                        result,
+                        "yaml",
+                        line_numbers=True,
+                        indent_guides=True,
+                    ),
+                    border_style="blue",
+                    title="[yellow]YAML",
+                )
+            )
         raise typer.Exit(0)
-
-    except ValueError as exc:
-        typer.echo(exc)
-        raise typer.Exit(1)
+    except NettowelInputError as exc:
+        typer.echo("Input is not valide", err=True)
+        typer.echo(str(exc), err=True)
+        raise typer.Exit(3)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `nettowel-0.5.0/nettowel/exceptions.py` & `nettowel-0.5.1/nettowel/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,7 +35,11 @@
         self,
         error_str: str,
         server_msg: Any,
     ) -> None:
         self.error_str = error_str
         self.server_msg = server_msg
         super().__init__(self.error_str)
+
+
+class NettowelInputError(NettowelException):
+    ...
```

### Comparing `nettowel-0.5.0/nettowel/jinja.py` & `nettowel-0.5.1/nettowel/jinja.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/netmiko.py` & `nettowel-0.5.1/nettowel/netmiko.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List
+from typing import Any, List, Optional
 from nettowel._common import needs
 from nettowel.logger import log
 from nettowel.exceptions import NettowelTimeoutError
 
 _module = "netmiko"
 
 try:
@@ -24,26 +24,26 @@
     return list(NETMIKO_DEVICE_TYPES.keys())
 
 
 def send_command(
     cmd: str,
     device_type: str,
     host: str,
-    username: str = None,
-    password: str = None,
+    username: Optional[str] = None,
+    password: Optional[str] = None,
     port: int = 22,
     secret: str = "",
     use_textfsm: bool = False,
     use_ttp: bool = False,
-    ttp_template: str = None,
+    ttp_template: Optional[str] = None,
     use_genie: bool = False,
-    ssh_config_file: str = None,
+    ssh_config_file: Optional[str] = None,
     use_keys: bool = False,
-    key_file: str = None,
-    session_log: str = None,
+    key_file: Optional[str] = None,
+    session_log: Optional[str] = None,
 ) -> str:
     try:
         device: BaseConnection = ConnectHandler(
             device_type=device_type,
             host=host,
             username=username,
             password=password,
@@ -68,22 +68,22 @@
         )
     except NetmikoTimeoutException as esc:
         raise NettowelTimeoutError(str(esc))
 
 
 def autodetect(
     host: str,
-    username: str = None,
-    password: str = None,
+    username: Optional[str] = None,
+    password: Optional[str] = None,
     port: int = 22,
     secret: str = "",
-    ssh_config_file: str = None,
+    ssh_config_file: Optional[str] = None,
     use_keys: bool = False,
-    key_file: str = None,
-    session_log: str = None,
+    key_file: Optional[str] = None,
+    session_log: Optional[str] = None,
 ) -> str:
     guesser = SSHDetect(
         device_type="autodetect",
         host=host,
         username=username,
         password=password,
         port=port,
```

### Comparing `nettowel-0.5.0/nettowel/pandas.py` & `nettowel-0.5.1/nettowel/pandas.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/nettowel/restconf.py` & `nettowel-0.5.1/nettowel/restconf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List
+from typing import Any, Optional
 import json
 from nettowel.logger import log
 from nettowel.exceptions import NettowelRestconfError
 
 import requests
 import urllib3
 
@@ -19,15 +19,15 @@
 
 
 def send_request(
     method: str,
     url: str,
     username: str,
     password: str,
-    data: str = None,
+    data: Optional[str] = None,
     verify: bool = True,
     send_xml: bool = False,
     return_xml: bool = False,
 ) -> Any:
     try:
         headers = {
             "Content-Type": content_type["xml"] if send_xml else content_type["json"],
```

### Comparing `nettowel-0.5.0/nettowel/ttp.py` & `nettowel-0.5.1/nettowel/ttp.py`

 * *Files identical despite different names*

### Comparing `nettowel-0.5.0/pyproject.toml` & `nettowel-0.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,84 @@
 [tool.poetry]
 name = "nettowel"
-version = "0.5.0"
+version = "0.5.1"
 description = "Network Automation Collection"
 authors = ["ubaumann <github@m.ubaumann.ch>"]
 license = "Apache 2.0"
 readme = "README.md"
-repository = "https://github.com/InfrastructureAsCode-ch/nettowel/tree"
+repository = "https://github.com/InfrastructureAsCode-ch/nettowel"
 classifiers = [
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-typer = "^0.6"
-rich = "^12"
+typer = "^0.9"
+rich = "^12|^13"
 Jinja2 = {version = "^3.0.3", optional = true}
-ttp = {version = "^0.8.4", optional = true}
-textfsm = {version = "^1.1.2", optional = true}
-napalm = {version = "^3", optional = true}
+ttp = {version = "^0.9", optional = true}
+textfsm = {version = "^1.1", optional = true}
+napalm = {version = "^4", optional = true}
 netmiko = {version = "^4", optional = true}
-scrapli = {version = "^2022.1.30", optional = true}
-nornir = {version = "^3.2.0", optional = true}
+scrapli = {version = "^2023.1.30", optional = true}
+nornir = {version = "^3.2", optional = true}
 "ruamel.yaml" = "^0.17.21"
 jinja2schema = {version = "^0.1.4", optional = true}
 qrcode = "^7.3.1"
-python-dotenv = "^0.20.0"
+python-dotenv = "^1"
 requests = "^2.27.1"
-# nornir-napalm = {version = "^0.2.0", optional = true}
-# nornir-scrapli = {version = "^2022.1.30", optional = true}
-# nornir-utils = {version = "^0.2.0", optional = true}
-# nornir-jinja2 = {version = "^0.2.0", optional = true}
-# nornir-pyxl = {version = "^1.0.1", optional = true}
-# nornir-http = {version = "^0.1.1", optional = true}
-# nornir-netmiko = {git = "https://github.com/ktbyers/nornir_netmiko.git", rev = "develop", optional = true}
-# nornir-rich = {git = "https://github.com/InfrastructureAsCode-ch/nornir_rich.git", rev = "develop", optional = true}
-pandas = {version = "^1", optional = true}
+nornir-napalm = {version = "^0.4", optional = true}
+nornir-scrapli = {version = "^2023.1.30", optional = true}
+nornir-utils = {version = "^0.2.0", optional = true}
+nornir-jinja2 = {version = "^0.2.0", optional = true}
+nornir-pyxl = {version = "^1.0.1", optional = true}
+nornir-http = {version = "^0.1", optional = true}
+nornir-netmiko = {version = "^1.0.0", optional = true}
+nornir-rich = {version = "^0.1", optional = true}
+pandas = {version = "^2", optional = true}
+trogon = {version = "^0.4.0", optional = true}
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
-pytest = "^7.0.1"
-mypy = "^0.942"
+black = "^22|^23"
+pytest = "^7"
+mypy = "^0.942|^1"
 types-requests = "^2.27.20"
 
 [tool.poetry.extras]
 jinja = ["Jinja2", "jinja2schema"]
 ttp = ["ttp"]
 textfsm = ["textfsm"]
 napalm = ["napalm"]
 netmiko = ["netmiko"]
 scrapli = ["scrapli"]
-# nornir = ["nornir", "nornir-napalm", "nornir-scrapli", "nornir-utils", "nornir-jinja2", "nornir-pyxl", "nornir-http", "nornir-netmiko", "nornir-rich"]
+nornir = ["nornir", "nornir-napalm", "nornir-scrapli", "nornir-utils", "nornir-jinja2", "nornir-pyxl", "nornir-http", "nornir-netmiko", "nornir-rich"]
 pandas = ["pandas"]
+tui = ["trogon"]
 full = [
     "Jinja2", 
     "jinja2schema", 
     "ttp", 
     "textfsm", 
     "napalm", 
     "netmiko", 
     "scrapli", 
     "nornir", 
-#    "nornir-napalm", 
-#    "nornir-scrapli", 
-#    "nornir-utils", 
-#    "nornir-jinja2", 
-#    "nornir-pyxl", 
-#    "nornir-http", 
-#    "nornir-netmiko", 
-#    "nornir-rich", 
-    "pandas"
+    "nornir-napalm", 
+    "nornir-scrapli", 
+    "nornir-utils", 
+    "nornir-jinja2", 
+    "nornir-pyxl", 
+    "nornir-http", 
+    "nornir-netmiko", 
+    "nornir-rich", 
+    "pandas",
+    "trogon"
 ]
 
 [tool.poetry.scripts]
 nettowel = 'nettowel.cli.main:run'
 nt = 'nettowel.cli.main:run'
 
 [build-system]
```

### Comparing `nettowel-0.5.0/PKG-INFO` & `nettowel-0.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 Metadata-Version: 2.1
 Name: nettowel
-Version: 0.5.0
+Version: 0.5.1
 Summary: Network Automation Collection
-Home-page: https://github.com/InfrastructureAsCode-ch/nettowel/tree
+Home-page: https://github.com/InfrastructureAsCode-ch/nettowel
 License: Apache 2.0
 Author: ubaumann
 Author-email: github@m.ubaumann.ch
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: full
 Provides-Extra: jinja
 Provides-Extra: napalm
 Provides-Extra: netmiko
+Provides-Extra: nornir
 Provides-Extra: pandas
 Provides-Extra: scrapli
 Provides-Extra: textfsm
 Provides-Extra: ttp
-Requires-Dist: Jinja2 (>=3.0.3,<4.0.0); extra == "jinja" or extra == "full"
-Requires-Dist: jinja2schema (>=0.1.4,<0.2.0); extra == "jinja" or extra == "full"
-Requires-Dist: napalm (>=3,<4); extra == "napalm" or extra == "full"
-Requires-Dist: netmiko (>=4,<5); extra == "netmiko" or extra == "full"
-Requires-Dist: nornir (>=3.2.0,<4.0.0); extra == "full"
-Requires-Dist: pandas (>=1,<2); extra == "pandas" or extra == "full"
-Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Provides-Extra: tui
+Requires-Dist: Jinja2 (>=3.0.3,<4.0.0) ; extra == "jinja" or extra == "full"
+Requires-Dist: jinja2schema (>=0.1.4,<0.2.0) ; extra == "jinja" or extra == "full"
+Requires-Dist: napalm (>=4,<5) ; extra == "napalm" or extra == "full"
+Requires-Dist: netmiko (>=4,<5) ; extra == "netmiko" or extra == "full"
+Requires-Dist: nornir (>=3.2,<4.0) ; extra == "nornir" or extra == "full"
+Requires-Dist: nornir-http (>=0.1,<0.2) ; extra == "nornir" or extra == "full"
+Requires-Dist: nornir-jinja2 (>=0.2.0,<0.3.0) ; extra == "nornir" or extra == "full"
+Requires-Dist: nornir-napalm (>=0.4,<0.5) ; extra == "nornir" or extra == "full"
+Requires-Dist: nornir-netmiko (>=1.0.0,<2.0.0) ; extra == "nornir" or extra == "full"
+Requires-Dist: nornir-pyxl (>=1.0.1,<2.0.0) ; extra == "nornir" or extra == "full"
+Requires-Dist: nornir-rich (>=0.1,<0.2) ; extra == "nornir" or extra == "full"
+Requires-Dist: nornir-scrapli (>=2023.1.30,<2024.0.0) ; extra == "nornir" or extra == "full"
+Requires-Dist: nornir-utils (>=0.2.0,<0.3.0) ; extra == "nornir" or extra == "full"
+Requires-Dist: pandas (>=2,<3) ; extra == "pandas" or extra == "full"
+Requires-Dist: python-dotenv (>=1,<2)
 Requires-Dist: qrcode (>=7.3.1,<8.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: rich (>=12,<13)
+Requires-Dist: rich (>=12,<14)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
-Requires-Dist: scrapli (>=2022.1.30,<2023.0.0); extra == "scrapli" or extra == "full"
-Requires-Dist: textfsm (>=1.1.2,<2.0.0); extra == "textfsm" or extra == "full"
-Requires-Dist: ttp (>=0.8.4,<0.9.0); extra == "ttp" or extra == "full"
-Requires-Dist: typer (>=0.6,<0.7)
-Project-URL: Repository, https://github.com/InfrastructureAsCode-ch/nettowel/tree
+Requires-Dist: scrapli (>=2023.1.30,<2024.0.0) ; extra == "scrapli" or extra == "full"
+Requires-Dist: textfsm (>=1.1,<2.0) ; extra == "textfsm" or extra == "full"
+Requires-Dist: trogon (>=0.4.0,<0.5.0) ; extra == "tui" or extra == "full"
+Requires-Dist: ttp (>=0.9,<0.10) ; extra == "ttp" or extra == "full"
+Requires-Dist: typer (>=0.9,<0.10)
+Project-URL: Repository, https://github.com/InfrastructureAsCode-ch/nettowel
 Description-Content-Type: text/markdown
 
-# nettowel
+[![PyPI versions](https://img.shields.io/pypi/pyversions/nettowel.svg)](https://pypi.python.org/pypi/nettowel/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
+[![Downloads](https://pepy.tech/badge/nettowel)](https://pepy.tech/project/nettowel)
+
+# NetTowel
 Collection of useful network automation functions 
 
+
 > ⚠️ `nettowel` is under heavy construction and not production ready. Feedback is highly appreciated.
 
 
 ## Install
 
 You can install it directly from pypi
 
@@ -62,14 +80,15 @@
 - ttp
 - textfsm
 - napalm
 - netmiko
 - scrapli
 - nornir
 - pandas
+- tui
 
 ```bash
 pip install nettowel[jinja]
 pip install nettowel[full]
 ```
 
 ## Install from source
@@ -154,14 +173,24 @@
 ![ip info](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/ip-info.png)
 
 #### network-info
 
 ![network info](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/network-info.png)
 
 
+### YAML
+
+#### load
+
+![yaml load](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/yaml-load.png)
+
+#### dump
+
+![yaml dump](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/yaml-dump.png)
+
 ### Help
 
 ![Help QRcode](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/nettowel-help.png)
 
 
 ### Settings
 
@@ -171,32 +200,13 @@
 
 
 ### Piping
 
 ![piping](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/piping.png)
 
 
+### TUI
 
-## Building CLI Docs
-
-**At the moment `typer-cli` is not ready for typer 0.4.0**
-
-```
-typer nettowel/cli/main.py utils docs --name nettowel --output CLI.md
-```
-
-## Contributing
+Using [Trogon](https://github.com/Textualize/trogon) a TUI (Terminal User Interface) can be generated to edit and run the NetTowel command.
 
-### Run tests:
-
-```bash
-make tests
-```
+![TUI](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nettowel/main/imgs/trogon.png)
 
-
-### Bump version:
-
-Steps: patch, minor, major, prepatch, preminor, premajor, prerelease.
-
-```bash
-make bump ARGS=patch
-```
```

