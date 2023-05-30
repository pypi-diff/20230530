# Comparing `tmp/onecode-0.1.0-py3-none-any.whl.zip` & `tmp/onecode-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 71446 bytes, number of entries: 51
+Zip file size: 78775 bytes, number of entries: 53
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 onecode/__init__.py
--rw-r--r--  2.0 unx      160 b- defN 80-Jan-01 00:00 onecode/base/__init__.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 onecode/base/__init__.py
 -rw-r--r--  2.0 unx      714 b- defN 80-Jan-01 00:00 onecode/base/decorator.py
--rw-r--r--  2.0 unx     5151 b- defN 80-Jan-01 00:00 onecode/base/enums.py
--rw-r--r--  2.0 unx     7422 b- defN 80-Jan-01 00:00 onecode/base/logger.py
--rw-r--r--  2.0 unx    12359 b- defN 80-Jan-01 00:00 onecode/base/project.py
+-rw-r--r--  2.0 unx     5729 b- defN 80-Jan-01 00:00 onecode/base/enums.py
+-rw-r--r--  2.0 unx     7963 b- defN 80-Jan-01 00:00 onecode/base/logger.py
+-rw-r--r--  2.0 unx    12896 b- defN 80-Jan-01 00:00 onecode/base/project.py
 -rw-r--r--  2.0 unx      482 b- defN 80-Jan-01 00:00 onecode/base/singleton.py
 -rw-r--r--  2.0 unx      115 b- defN 80-Jan-01 00:00 onecode/cli/__init__.py
 -rw-r--r--  2.0 unx     2693 b- defN 80-Jan-01 00:00 onecode/cli/add.py
 -rw-r--r--  2.0 unx     3883 b- defN 80-Jan-01 00:00 onecode/cli/create.py
 -rw-r--r--  2.0 unx     6029 b- defN 80-Jan-01 00:00 onecode/cli/extract.py
 -rw-r--r--  2.0 unx     1946 b- defN 80-Jan-01 00:00 onecode/cli/skeleton/.gitignore
 -rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 onecode/cli/skeleton/LICENSE
@@ -16,38 +16,40 @@
 -rw-r--r--  2.0 unx      138 b- defN 80-Jan-01 00:00 onecode/cli/skeleton/data/README.md
 -rw-r--r--  2.0 unx       62 b- defN 80-Jan-01 00:00 onecode/cli/skeleton/flows/README.md
 -rw-r--r--  2.0 unx      310 b- defN 80-Jan-01 00:00 onecode/cli/skeleton/flows/onecode_ext/README.md
 -rw-r--r--  2.0 unx       61 b- defN 80-Jan-01 00:00 onecode/cli/skeleton/flows/onecode_ext/__init__.py
 -rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 onecode/cli/skeleton/flows/onecode_ext/input_elements/__init__.py
 -rw-r--r--  2.0 unx       69 b- defN 80-Jan-01 00:00 onecode/cli/skeleton/flows/onecode_ext/output_elements/__init__.py
 -rw-r--r--  2.0 unx     3363 b- defN 80-Jan-01 00:00 onecode/cli/skeleton/main.py
--rw-r--r--  2.0 unx    12881 b- defN 80-Jan-01 00:00 onecode/cli/start.py
+-rw-r--r--  2.0 unx    14618 b- defN 80-Jan-01 00:00 onecode/cli/start.py
 -rw-r--r--  2.0 unx     8073 b- defN 80-Jan-01 00:00 onecode/cli/utils.py
 -rw-r--r--  2.0 unx      196 b- defN 80-Jan-01 00:00 onecode/elements/__init__.py
 -rw-r--r--  2.0 unx      162 b- defN 80-Jan-01 00:00 onecode/elements/input/__init__.py
--rw-r--r--  2.0 unx     3570 b- defN 80-Jan-01 00:00 onecode/elements/input/checkbox.py
--rw-r--r--  2.0 unx     5634 b- defN 80-Jan-01 00:00 onecode/elements/input/csv_reader.py
--rw-r--r--  2.0 unx     6919 b- defN 80-Jan-01 00:00 onecode/elements/input/dropdown.py
--rw-r--r--  2.0 unx     7925 b- defN 80-Jan-01 00:00 onecode/elements/input/file_input.py
--rw-r--r--  2.0 unx     4659 b- defN 80-Jan-01 00:00 onecode/elements/input/number_input.py
--rw-r--r--  2.0 unx     4887 b- defN 80-Jan-01 00:00 onecode/elements/input/radio_button.py
--rw-r--r--  2.0 unx     4729 b- defN 80-Jan-01 00:00 onecode/elements/input/slider.py
--rw-r--r--  2.0 unx     4421 b- defN 80-Jan-01 00:00 onecode/elements/input/text_input.py
--rw-r--r--  2.0 unx    18308 b- defN 80-Jan-01 00:00 onecode/elements/input_element.py
+-rw-r--r--  2.0 unx     3809 b- defN 80-Jan-01 00:00 onecode/elements/input/checkbox.py
+-rw-r--r--  2.0 unx     6087 b- defN 80-Jan-01 00:00 onecode/elements/input/csv_reader.py
+-rw-r--r--  2.0 unx     7159 b- defN 80-Jan-01 00:00 onecode/elements/input/dropdown.py
+-rw-r--r--  2.0 unx     8708 b- defN 80-Jan-01 00:00 onecode/elements/input/file_input.py
+-rw-r--r--  2.0 unx     6651 b- defN 80-Jan-01 00:00 onecode/elements/input/folder_input.py
+-rw-r--r--  2.0 unx     4897 b- defN 80-Jan-01 00:00 onecode/elements/input/number_input.py
+-rw-r--r--  2.0 unx     5126 b- defN 80-Jan-01 00:00 onecode/elements/input/radio_button.py
+-rw-r--r--  2.0 unx     4967 b- defN 80-Jan-01 00:00 onecode/elements/input/slider.py
+-rw-r--r--  2.0 unx     4660 b- defN 80-Jan-01 00:00 onecode/elements/input/text_input.py
+-rw-r--r--  2.0 unx    19642 b- defN 80-Jan-01 00:00 onecode/elements/input_element.py
 -rw-r--r--  2.0 unx      164 b- defN 80-Jan-01 00:00 onecode/elements/output/__init__.py
--rw-r--r--  2.0 unx     3909 b- defN 80-Jan-01 00:00 onecode/elements/output/csv_output.py
--rw-r--r--  2.0 unx     3435 b- defN 80-Jan-01 00:00 onecode/elements/output/file_output.py
--rw-r--r--  2.0 unx     3867 b- defN 80-Jan-01 00:00 onecode/elements/output/image_output.py
--rw-r--r--  2.0 unx     3694 b- defN 80-Jan-01 00:00 onecode/elements/output/text_output.py
--rw-r--r--  2.0 unx    11408 b- defN 80-Jan-01 00:00 onecode/elements/output_element.py
+-rw-r--r--  2.0 unx     4362 b- defN 80-Jan-01 00:00 onecode/elements/output/csv_output.py
+-rw-r--r--  2.0 unx     3674 b- defN 80-Jan-01 00:00 onecode/elements/output/file_output.py
+-rw-r--r--  2.0 unx     4106 b- defN 80-Jan-01 00:00 onecode/elements/output/image_output.py
+-rw-r--r--  2.0 unx     4007 b- defN 80-Jan-01 00:00 onecode/elements/output/plotly_output.py
+-rw-r--r--  2.0 unx     3933 b- defN 80-Jan-01 00:00 onecode/elements/output/text_output.py
+-rw-r--r--  2.0 unx    12900 b- defN 80-Jan-01 00:00 onecode/elements/output_element.py
 -rw-r--r--  2.0 unx      217 b- defN 80-Jan-01 00:00 onecode/utils/__init__.py
 -rw-r--r--  2.0 unx     1089 b- defN 80-Jan-01 00:00 onecode/utils/format.py
--rw-r--r--  2.0 unx     2896 b- defN 80-Jan-01 00:00 onecode/utils/import_input.py
--rw-r--r--  2.0 unx     3688 b- defN 80-Jan-01 00:00 onecode/utils/import_output.py
--rw-r--r--  2.0 unx     1499 b- defN 80-Jan-01 00:00 onecode/utils/module.py
+-rw-r--r--  2.0 unx     3618 b- defN 80-Jan-01 00:00 onecode/utils/import_input.py
+-rw-r--r--  2.0 unx     4416 b- defN 80-Jan-01 00:00 onecode/utils/import_output.py
+-rw-r--r--  2.0 unx     1655 b- defN 80-Jan-01 00:00 onecode/utils/module.py
 -rw-r--r--  2.0 unx      692 b- defN 80-Jan-01 00:00 onecode/utils/typing.py
--rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 onecode-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6141 b- defN 80-Jan-01 00:00 onecode-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 onecode-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      169 b- defN 80-Jan-01 00:00 onecode-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     4448 b- defN 16-Jan-01 00:00 onecode-0.1.0.dist-info/RECORD
-51 files, 177461 bytes uncompressed, 64318 bytes compressed:  63.8%
+?rw-r--r--  2.0 unx      169 b- defN 16-Jan-01 00:00 onecode-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 onecode-0.2.0.dist-info/LICENSE
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 onecode-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     6185 b- defN 16-Jan-01 00:00 onecode-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     4640 b- defN 16-Jan-01 00:00 onecode-0.2.0.dist-info/RECORD
+53 files, 200039 bytes uncompressed, 71339 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -81,14 +81,17 @@
 
 Filename: onecode/elements/input/dropdown.py
 Comment: 
 
 Filename: onecode/elements/input/file_input.py
 Comment: 
 
+Filename: onecode/elements/input/folder_input.py
+Comment: 
+
 Filename: onecode/elements/input/number_input.py
 Comment: 
 
 Filename: onecode/elements/input/radio_button.py
 Comment: 
 
 Filename: onecode/elements/input/slider.py
@@ -108,14 +111,17 @@
 
 Filename: onecode/elements/output/file_output.py
 Comment: 
 
 Filename: onecode/elements/output/image_output.py
 Comment: 
 
+Filename: onecode/elements/output/plotly_output.py
+Comment: 
+
 Filename: onecode/elements/output/text_output.py
 Comment: 
 
 Filename: onecode/elements/output_element.py
 Comment: 
 
 Filename: onecode/utils/__init__.py
@@ -132,23 +138,23 @@
 
 Filename: onecode/utils/module.py
 Comment: 
 
 Filename: onecode/utils/typing.py
 Comment: 
 
-Filename: onecode-0.1.0.dist-info/LICENSE
+Filename: onecode-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: onecode-0.1.0.dist-info/METADATA
+Filename: onecode-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: onecode-0.1.0.dist-info/WHEEL
+Filename: onecode-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: onecode-0.1.0.dist-info/entry_points.txt
+Filename: onecode-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: onecode-0.1.0.dist-info/RECORD
+Filename: onecode-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onecode/__init__.py

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 
 from .base import *
 from .elements import *
 from .utils import *
```

## onecode/base/__init__.py

```diff
@@ -1,6 +1,7 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
+from .decorator import *
 from .enums import *
 from .logger import *
 from .project import *
```

## onecode/base/enums.py

```diff
@@ -10,29 +10,37 @@
 
     - `ONECODE_PROJECT_DATA`: use this variable to overwrite default data location
     :octicons-arrow-both-24: `"ONECODE_PROJECT_DATA"`
     - `ONECODE_CONFIG_FILE`: name of the file containing OneCode project configurations
     :octicons-arrow-both-24: `".onecode.json"`
     - `ONECODE_DO_TYPECHECK`: set to 1 to force runtime type-checking with Pydantic
     :octicons-arrow-both-24: `"ONECODE_DO_TYPECHECK"`
+    - `ONECODE_LOGGER_NAME`: base logger name to avoid logging conflict with other loggers
+    :octicons-arrow-both-24: `|OneCode|`
 
     """
     ONECODE_PROJECT_DATA    = "ONECODE_PROJECT_DATA"    # noqa: E-221
     ONECODE_CONFIG_FILE     = ".onecode.json"           # noqa: E-221
     ONECODE_DO_TYPECHECK    = "ONECODE_DO_TYPECHECK"    # noqa: E-221
+    ONECODE_LOGGER_NAME     = "|OneCode|"               # noqa: E-221
 
 
 class ConfigOption(str, Enum):
     """
     Available options to control the configuration of the project.
 
-    - `FLUSH_STDOUT`: to force flushing the logger :octicons-arrow-both-24: `"FLUSH_STDOUT"`
+    - `FLUSH_STDOUT`: to force flushing the logger :octicons-arrow-both-24: `"FLUSH_STDOUT": False`
+    - `LOGGER_COLOR`: to color the logs by default when resetting the logger
+        :octicons-arrow-both-24: `"LOGGER_COLOR": True`
+    - `LOGGER_TIMESTAMP`: to timestamp the logs :octicons-arrow-both-24: `"LOGGER_TIMESTAMP": True`
 
     """
-    FLUSH_STDOUT        = "FLUSH_STDOUT"        # noqa: E-221
+    FLUSH_STDOUT        = "FLUSH_STDOUT"            # noqa: E-221
+    LOGGER_COLOR        = "LOGGER_COLOR"            # noqa: E-221
+    LOGGER_TIMESTAMP    = "LOGGER_TIMESTAMP"        # noqa: E-221
 
 
 class Mode(str, Enum):
     """
     Available modes to run OneCode projects:
 
     - `CONSOLE`: return the initial element class. Typically used in the interactive Python console.
```

## onecode/base/logger.py

```diff
@@ -4,15 +4,15 @@
 import inspect
 import logging
 import os
 import sys
 from typing import Optional
 
 from .decorator import check_type
-from .enums import ConfigOption
+from .enums import ConfigOption, Env
 from .project import Project
 from .singleton import Singleton
 
 
 class ColoredFormatter(logging.Formatter):
     """
     Logger class formatting messages in a specific way with colors interpretable
@@ -58,15 +58,17 @@
                 for more info.
 
         Returns:
             The formatted text.
 
         """
         flow = Project().current_flow if Project().current_flow is not None else ''
-        format = f"%(asctime)s [%(levelname)s] {flow} - %(name)s:%(lineno)d - %(message)s"
+        format = f"[%(levelname)s] {flow} - %(name)s:%(lineno)d - %(message)s"
+        if Project().get_config(ConfigOption.LOGGER_TIMESTAMP):
+            format = f"%(asctime)s {format}"
 
         formats = {
             logging.DEBUG: f"{self.GREY}{format}{self.RESET}",
             logging.INFO: f"{self.GREY}{format}{self.RESET}",
             logging.WARNING: f"{self.YELLOW}{format}{self.RESET}",
             logging.ERROR: f"{self.RED}{format}{self.RESET}",
             logging.CRITICAL: f"{self.BOLD_RED}{format}{self.RESET}",
@@ -102,44 +104,46 @@
         Logger.error("error")
         Logger.critical("critical")
         ```
 
     """
 
     def __init__(self):
-        self.set_level(logging.INFO)
         self.reset()
 
     def reset(self) -> None:
         """
-        Remove all added handlers attached to the logger (see `logging.removeHandler()` for more
-        info) and reset to the default console stream handler with the
-        [ColoredFormatter][onecode.ColoredFormatter].
+        Remove all added handlers attached to the OneCode logger (see `logging.removeHandler()`
+        for more info) and reset to the default console stream handler with the
+        [ColoredFormatter][onecode.ColoredFormatter] with `INFO` level.
 
         """
-        logger = logging.getLogger()
-        while logger.hasHandlers():
+        logger = logging.getLogger(Env.ONECODE_LOGGER_NAME)
+        while len(logger.handlers) > 0:
             logger.removeHandler(logger.handlers[0])
 
         handler = logging.StreamHandler(sys.stdout)
-        handler.setFormatter(ColoredFormatter())
-        logging.getLogger().addHandler(handler)
+        handler.setFormatter(ColoredFormatter(Project().get_config(ConfigOption.LOGGER_COLOR)))
+        logging.getLogger(Env.ONECODE_LOGGER_NAME).addHandler(handler)
+        self.set_level(logging.INFO)
 
     @check_type
     def add_handler(
         self,
-        handler: Optional[logging.Handler] = None
+        handler: Optional[logging.Handler] = None,
+        root_logger: bool = True
     ) -> None:
         """
         Add an extra handler in addition to the default console stream one.
         Nothing is done if handler is None.
 
         Args:
             handler: New handler to add.
-
+            root_logger: If True, add the handler at the root logging, otherwise
+                as a child of the `|OneCode|` logger.
 
         !!! example
             ```py
             import logging
 
             from onecode import Logger
 
@@ -147,31 +151,32 @@
             handler = logging.FileHandler("debug.log")
             Logger().add_handler(handler)
             Logger.error('oops!')   # will print to console in red and to file "debug.log"
             ```
 
         """
         if handler is not None:
-            logging.getLogger().addHandler(handler)
+            namespace = Env.ONECODE_LOGGER_NAME if not root_logger else None
+            logging.getLogger(namespace).addHandler(handler)
 
     @check_type
     def set_level(
         self,
         level: int
     ) -> None:
         """
-        Set the logger level. Default logging is INFO.
+        Set the OneCode logger level. Default logging is INFO.
 
         Args:
             level: Numerical value to set the logging level to. See
                 [logging levels](https://docs.python.org/3/library/logging.html#logging-levels) for
                 more information.
 
         """
-        logging.getLogger().setLevel(level)
+        logging.getLogger(Env.ONECODE_LOGGER_NAME).setLevel(level)
 
     @check_type
     def logger(
         self,
         stacklevel: int = 1,
     ) -> logging.Logger:
         """
@@ -186,15 +191,15 @@
 
         Returns:
             Python Logger object.
 
         """
         stack = inspect.stack()
         file = os.path.basename(stack[stacklevel].filename) if len(stack) > stacklevel else None
-        return logging.getLogger(file)
+        return logging.getLogger(f'{Env.ONECODE_LOGGER_NAME}.{file}')
 
     @staticmethod
     def _flush() -> None:
         """
         Force flush to stdout if `ConfigOption.FLUSH_STDOUT` is True. See
             [Project.config][onecode.Project.config] for more information.
```

## onecode/base/project.py

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
+import ast
 import json
 import os
 import sys
 from typing import Any, Dict, Optional, Set, Union
 
 import pydash
 from flufl.lock import Lock
@@ -68,16 +69,25 @@
         this_module = sys.modules[__name__].__name__.split('.')[0]
         self._registered_elements = {
             ent for ent in self._registered_elements if ent.startswith(f'{this_module}.')
         }
         self._mode = Mode.CONSOLE
         self._flow = None
         self._data = None
+
+        # get string config from env variables starting with ONECODE_CONFIG_
+        # get flag config from env variables starting with ONECODE_FLAG_
         self._config = {
-            ConfigOption.FLUSH_STDOUT: False
+            ConfigOption.FLUSH_STDOUT: False,
+            ConfigOption.LOGGER_COLOR: True,
+            ConfigOption.LOGGER_TIMESTAMP: True,
+            **{k[len("ONECODE_CONFIG_"):]: os.environ[k]
+                for k in os.environ if k.startswith("ONECODE_CONFIG_")},
+            **{k[len("ONECODE_FLAG_"):]: bool(ast.literal_eval(os.environ[k]))
+                for k in os.environ if k.startswith("ONECODE_FLAG_")},
         }
 
     @property
     def registered_elements(self) -> Set[str]:
         """
         Get the list of registered elements (`InputElement` and `OutputElement`).
         Once a library is registered, it is required to register the elements that need to be
```

## onecode/cli/start.py

```diff
@@ -91,14 +91,61 @@
             print(f"=> {code['loc']}")
             print('Error ', e)
 
     return streamlit_input, list(streamlit_output)
 
 
 @check_type
+def get_import_statements(calls: List[Dict[str, str]]):
+    """
+    Get the import and init statements from the elements called.
+
+    Args:
+        calls: List of `{"func": <function_name>, "loc": <code_to_eval>}` where `func` is the name
+            of the function corresponding to the `InputElement` (i-e its snake case form - see the
+            element developer section for more info), and `loc` is the "line of code" to evaluate
+            through the Python interpreter.
+
+    Returns:
+        The pair of two sets containing respectively imports statements and init statements.
+
+    !!! example
+        ```py
+        # getting statements from a single call of FileInput element
+        get_import_statements(
+            [{"func": "onecode.file_input", "loc": "onecode.file_input('file', 'a.txt')"}]
+        )
+        ```
+
+        ```py title="Output"
+        {"import tkinter as tk", "from tkinter import filedialog"}, {'_root = tk.Tk()\n
+        _root.withdraw()\n
+        _root.wm_attributes('-topmost', 1)'}
+        ```
+
+    """
+    imports = set()
+    init = set()
+
+    for code in calls:
+        try:
+            i1 = eval(f"{code['func']}_imports")
+            i2 = eval(f"{code['func']}_init")
+            imports.update(i1)
+            init.add(i2)
+
+        except Exception as e:
+            print(f"=> {code['func']}_imports")
+            print(f"=> {code['func']}_init")
+            print('Error ', e)
+
+    return imports, init
+
+
+@check_type
 def prepare_streamlit_file(
     project_path: str,
     to_file: str
 ) -> None:
     """
     Prepare the Streamlit App Python file from the given OneCode project and dump it to the
     specified file.
@@ -110,45 +157,54 @@
     """
     Project().mode = Mode.STREAMLIT
 
     statements = process_call_graph(project_path)
     menu_entries = statements.keys()
 
     all_st_outputs = set()
+    all_import_libs = set()
+    all_init_libs = set()
+
+    for k, v in statements.items():
+        imports, init = get_import_statements(v["calls"])
+        all_import_libs.update(imports)
+        all_init_libs.update(init)
+
+    import_statements = '\n'.join(sorted(all_import_libs))
+    init_statements = '\n'.join(sorted(all_init_libs))
 
     with open(to_file, 'w') as f:
         f.write(f"""###########################################
 #    !! THIS FILE IS AUTO-GENERATED !!    #
 ###########################################
 
 import ast
 import json
 import logging
 import os
-import tkinter as tk
 import traceback
 import uuid
-from tkinter import filedialog
 from typing import Dict, List
 
-import numpy as np
 import pydash
 import streamlit as st
 from main import main
-from pyarrow import csv as pacsv
 from streamlit_image_select import image_select
 from streamlit_option_menu import option_menu
 from streamlit_tree_select import tree_select
 
 from onecode import ColoredFormatter
 
-_root = tk.Tk()
-_root.withdraw()
-_root.wm_attributes('-topmost', 1)
+# Imports from Elements
+{import_statements}
+
+# Init from Elements
+{init_statements}
 
+# OneCode init
 {Keyword.DATA} = {{}}
 _placeholders = {{}}
 
 
 def _write_logs(id: str) -> None:
     if f'__logs__{{id}}' in st.session_state:
         with _placeholders[id].container():
@@ -410,10 +466,10 @@
     sys.argv = [sys.argv[0]]
 
     prepare_streamlit_file(os.getcwd(), 'app.py')
 
     Project().mode = Mode.EXECUTE
     os.environ['STREAMLIT_RUN_TARGET'] = 'app.py'
     os.environ['STREAMLIT_SERVER_MAX_UPLOAD_SIZE'] = '4000'
-    os.environ['STREAMLIT_GATHER_USAGE_STATS'] = '0'
+    os.environ['STREAMLIT_BROWSER_GATHER_USAGE_STATS'] = '0'
 
     main_run()
```

## onecode/elements/input/checkbox.py

```diff
@@ -1,26 +1,27 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
-from typing import List, Optional, Union
+from typing import Any, List, Optional, Union
 
 from ...base.decorator import check_type
 from ..input_element import InputElement
 
 
 class Checkbox(InputElement):
     @check_type
     def __init__(
         self,
         key: str,
         value: Optional[Union[bool, List[bool]]],
         label: Optional[str] = None,
         count: Optional[Union[int, str]] = None,
         optional: Union[bool, str] = False,
-        hide_when_disabled: bool = False
+        hide_when_disabled: bool = False,
+        **kwargs: Any
     ):
         """
         A simple checkbox with a label. Value is either True, False or None.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -36,14 +37,16 @@
                 [Using Expressions][using-runtime-expressions-in-elements] for more information).
             optional: Specify whether the value may be None. `optional` can either be a fixed
                 boolean (`False` or `True`) or a conditional expression dependent of other elements
                 (see [Using Expressions][using-runtime-expressions-in-elements] for more
                 information).
             hide_when_disabled: If element is optional, set it to True to hide it from the
                 interface, otherwise it will be shown disabled.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -65,15 +68,16 @@
         """
         super().__init__(
             key,
             value,
             label,
             count,
             optional,
-            hide_when_disabled
+            hide_when_disabled,
+            **kwargs
         )
 
     @property
     def _value_type(self) -> type:
         """
         Get the Checkbox value type: boolean `bool`.
```

## onecode/elements/input/csv_reader.py

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
 import os
-from typing import List, Optional, Union
+from typing import Any, List, Optional, Union
 
 import pandas as pd
 from pyarrow import csv as pacsv
 
 from ...base.decorator import check_type
 from ...base.project import Project
 from ..input_element import InputElement
@@ -18,15 +18,16 @@
         self,
         key: str,
         value: Optional[Union[str, List[str]]],
         label: Optional[str] = None,
         count: Optional[Union[int, str]] = None,
         optional: Union[bool, str] = False,
         hide_when_disabled: bool = False,
-        tags: Optional[List[str]] = None
+        tags: Optional[List[str]] = None,
+        **kwargs: Any
     ):
         """
         A CSV-file reader returning a Pandas DataFrame and displayed as a table in Streamlit.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -44,14 +45,16 @@
                 boolean (`False` or `True`) or a conditional expression dependent of other elements
                 (see [Using Expressions][using-runtime-expressions-in-elements] for more
                 information).
             hide_when_disabled: If element is optional, set it to True to hide it from the
                 interface, otherwise it will be shown disabled.
             tags: Optional meta-data information about the expected file. This information is only
                 used by the `Mode.EXTRACT_ALL` when dumping attributes to JSON.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -73,15 +76,16 @@
         super().__init__(
             key,
             value,
             label,
             count,
             optional,
             hide_when_disabled,
-            tags=tags
+            tags=tags,
+            **kwargs
         )
 
     @property
     def _value_type(self) -> type:
         """
         Get the CsvReader value type: Pandas DataFrame `pd.DataFrame`.
 
@@ -123,14 +127,23 @@
         Raises:
             ValueError: if the DataFrame is empty.
 
         """
         if value.empty:
             raise ValueError(f"[{self.key}] Empty dataframe")
 
+    @staticmethod
+    def imports() -> List[str]:
+        """
+        Returns:
+            Python import statements required by the Streamlit code.
+
+        """
+        return ["from pyarrow import csv as pacsv"]
+
     @check_type
     def streamlit(
         self,
         id: str
     ) -> str:
         """
         Returns:
```

## onecode/elements/input/dropdown.py

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
-from typing import List, Optional, Union
+from typing import Any, List, Optional, Union
 
 from ...base.decorator import check_type
 from ...utils.format import convert_expr
 from ..input_element import InputElement
 
 
 class Dropdown(InputElement):
@@ -19,15 +19,16 @@
             List[List[Union[str, int, float]]]
         ]],
         label: Optional[str] = None,
         count: Optional[Union[int, str]] = None,
         optional: Union[bool, str] = False,
         hide_when_disabled: bool = False,
         options: Union[List, str] = [],
-        multiple: bool = False
+        multiple: bool = False,
+        **kwargs: Any
     ):
         """
         A single or multipe choice dropdown menu.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -49,14 +50,17 @@
                 interface, otherwise it will be shown disabled.
             options: List all possible options available in the dropdown menu. This list may either
                 be fixed or dynamic (to a certain extent): in the latter case, use
                 [Expressions][using-runtime-expressions-in-elements] in a similar way as `optional`
                 and `count`. See example below.
             multiple: Set to True if multiple choice is allowed, otherwise only a single element can
                 be selected.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
+
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             Fixed options:
@@ -103,15 +107,16 @@
             key,
             value,
             label,
             count,
             optional,
             hide_when_disabled,
             options=options,
-            multiple=multiple
+            multiple=multiple,
+            **kwargs
         )
 
     @property
     def _value_type(self) -> type:
         """
         Get the Dropdown value type: either a list of string `list[str]` when the
         Dropdown is multiple choice, otherwise a single string `str`.
```

## onecode/elements/input/file_input.py

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
 import os
-from typing import List, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union
 
 from ...base.decorator import check_type
 from ...base.project import Project
 from ...utils.typing import is_type
 from ..input_element import InputElement
 
 
@@ -18,15 +18,16 @@
         value: Optional[Union[str, List[str], List[List[str]]]],
         label: Optional[str] = None,
         count: Optional[Union[int, str]] = None,
         optional: Union[bool, str] = False,
         hide_when_disabled: bool = False,
         types: List[Tuple[str, str]] = None,
         multiple: bool = False,
-        tags: Optional[List[str]] = None
+        tags: Optional[List[str]] = None,
+        **kwargs: Any
     ):
         """
         A single or multiple file selector.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -52,14 +53,16 @@
             types: List of filters allowing to narrow file selection within Streamlit. Each filter
                 must be a pair of (name, list of allowed extensions), e.g.
                 `("Image", ".jpg .png .jpeg")`. You may use the FileFilter enums for convenience.
             multiple: Set to True if multiple choice is allowed, otherwise only a single element can
                 be selected.
             tags: Optional meta-data information about the expected file. This information is only
                 used by the `Mode.EXTRACT_ALL` when dumping attributes to JSON.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -85,15 +88,16 @@
             value,
             label,
             count,
             optional,
             hide_when_disabled,
             types=types,
             multiple=multiple,
-            tags=tags
+            tags=tags,
+            **kwargs
         )
 
     @property
     def _value_type(self) -> type:
         """
         Get the FileInput value type: either a list of string `list[str]` when the
         FileInput is multiple file selection, otherwise a single string `str`.
@@ -153,14 +157,38 @@
         """
         if self.multiple:
             for v in value:
                 self._validate_file_value(v)
         else:
             self._validate_file_value(value)
 
+    @staticmethod
+    def imports() -> List[str]:
+        """
+        Returns:
+            Python import statements required by the Streamlit code.
+
+        """
+        return [
+            "import tkinter as tk",
+            "from tkinter import filedialog"
+        ]
+
+    @staticmethod
+    def init() -> str:
+        """
+        Returns:
+            The Python statements that must be initialized before being used by the Streamlit code.
+
+        """
+        return """_root = tk.Tk()
+_root.withdraw()
+_root.wm_attributes('-topmost', 1)
+"""
+
     @check_type
     def streamlit(
         self,
         id: str
     ) -> str:
         """
         Returns:
```

## onecode/elements/input/number_input.py

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
-from typing import List, Optional, Union
+from typing import Any, List, Optional, Union
 
 from ...base.decorator import check_type
 from ..input_element import InputElement
 
 
 class NumberInput(InputElement):
     @check_type
@@ -15,15 +15,16 @@
         value: Optional[Union[float, List[float]]],
         label: Optional[str] = None,
         count: Optional[Union[int, str]] = None,
         optional: Union[bool, str] = False,
         hide_when_disabled: bool = False,
         min: float = None,
         max: float = None,
-        step: float = None
+        step: float = None,
+        **kwargs: Any
     ):
         """
         A field for numerical values.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -42,14 +43,16 @@
                 (see [Using Expressions][using-runtime-expressions-in-elements] for more
                 information).
             hide_when_disabled: If element is optional, set it to True to hide it from the
                 interface, otherwise it will be shown disabled.
             min: Optionally limit the possible values with a lower bound.
             max: Optionally limit the possible values with an upper bound.
             step: Optionally set a step used when increment/decrement button are used.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -76,14 +79,15 @@
             label,
             count,
             optional,
             hide_when_disabled,
             min=min,
             max=max,
             step=step,
+            **kwargs
         )
 
     @property
     def _value_type(self) -> type:
         """
         Get the NumberInput value type: floating point number `float`.
```

## onecode/elements/input/radio_button.py

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
-from typing import List, Optional, Union
+from typing import Any, List, Optional, Union
 
 import pydash
 
 from ...base.decorator import check_type
 from ..input_element import InputElement
 
 
@@ -16,15 +16,16 @@
         key: str,
         value: Optional[Union[str, List[str]]],
         label: Optional[str] = None,
         count: Optional[Union[int, str]] = None,
         optional: Union[bool, str] = False,
         hide_when_disabled: bool = False,
         options: List[str] = [],
-        horizontal: bool = False
+        horizontal: bool = False,
+        **kwargs: Any
     ):
         """
         A single choice represented as a group of exclusive radio buttons.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -45,14 +46,16 @@
             hide_when_disabled: If element is optional, set it to True to hide it from the
                 interface, otherwise it will be shown disabled.
             options: List all possible options available. This list may either be fixed or dynamic
                 (to a certain extent): in the latter case, use expressions in a similar  way as
                 `optional` and `count`. See example below.
             horizontal: Set to True to have radio buttons displayed horizontally, otherwise radio
                 buttons will be displayed vertically.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             Fixed options:
@@ -95,15 +98,16 @@
             key,
             value,
             label,
             count,
             optional,
             hide_when_disabled,
             options=options,
-            horizontal=horizontal
+            horizontal=horizontal,
+            **kwargs
         )
 
     @property
     def _value_type(self) -> type:
         """
         Get the RadioButton value type: string `str`.
```

## onecode/elements/input/slider.py

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
-from typing import List, Optional, Union
+from typing import Any, List, Optional, Union
 
 from ...base.decorator import check_type
 from ..input_element import InputElement
 
 
 class Slider(InputElement):
     @check_type
@@ -15,15 +15,16 @@
         value: Optional[Union[float, List[float]]],
         label: Optional[str] = None,
         count: Optional[Union[int, str]] = None,
         optional: Union[bool, str] = False,
         hide_when_disabled: bool = False,
         min: float = 0.,
         max: float = 1.,
-        step: float = 0.1
+        step: float = 0.1,
+        **kwargs: Any
     ):
         """
         A slider for numerical values.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -42,14 +43,16 @@
                 (see [Using Expressions][using-runtime-expressions-in-elements] for more
                 information).
             hide_when_disabled: If element is optional, set it to True to hide it from the
                 interface, otherwise it will be shown disabled.
             min: Mandatory lower bound, defaults to 0.
             max: Mandatory upper bound, defaults to 1.
             step: Mandatory step used when incrementing/decrementing the slider, defaults to 0.1.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -81,14 +84,15 @@
             label,
             count,
             optional,
             hide_when_disabled,
             min=float(min),
             max=float(max),
             step=float(step),
+            **kwargs
         )
 
     @property
     def _value_type(self) -> type:
         """
         Get the Slider value type: floating point or integer number `float|int`.
```

## onecode/elements/input/text_input.py

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
-from typing import List, Optional, Union
+from typing import Any, List, Optional, Union
 
 from ...base.decorator import check_type
 from ..input_element import InputElement
 
 
 class TextInput(InputElement):
     @check_type
@@ -15,15 +15,16 @@
         value: Optional[Union[str, List[str]]],
         label: Optional[str] = None,
         count: Optional[Union[int, str]] = None,
         optional: Union[bool, str] = False,
         hide_when_disabled: bool = False,
         max_chars: int = None,
         placeholder: str = None,
-        multiline: Union[bool, int] = False
+        multiline: Union[bool, int] = False,
+        **kwargs: Any
     ):
         """
         A simple text field.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -42,14 +43,16 @@
                 (see [Using Expressions][using-runtime-expressions-in-elements] for more
                 information).
             hide_when_disabled: If element is optional, set it to True to hide it from the
                 interface, otherwise it will be shown disabled.
             max_chars: Maximum number of characters allowed for this text field.
             placeholder: Placeholder text shown whenever there is no value.
             multiline: Set to True or a height in pixels to make it multiline text area.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -74,15 +77,16 @@
             value,
             label,
             count,
             optional,
             hide_when_disabled,
             max_chars=max_chars,
             placeholder=placeholder,
-            multiline=multiline
+            multiline=multiline,
+            **kwargs
         )
 
     @property
     def _value_type(self) -> type:
         """
         Get the TextInput value type: string `str`.
```

## onecode/elements/input_element.py

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
 from abc import ABC, abstractmethod
-from typing import Any, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union
 
 import pydash
 from slugify import slugify
 
 from ..base.decorator import check_type
 from ..base.enums import Keyword
 from ..base.project import Project
@@ -122,14 +122,23 @@
         if len(invalid_args) > 0:
             raise AttributeError(f'The following parameters are reserved: {invalid_args}')
 
         self._extra_args = pydash.omit(kwargs, reserved_args)
         self.__dict__.update(self._extra_args)
 
     @property
+    def kind(self) -> str:
+        """
+        Returns:
+            The element class name.
+
+        """
+        return type(self).__name__
+
+    @property
     def label(self) -> str:
         """
         Get the label with triple-quotes and escaped to handle human-readable string.
         It is primarly meant to be directly used in the Streamlit generated code for the
         `label` parameter.
         See [`streamlit()`][onecode.InputElement.streamlit] for more information.
 
@@ -192,14 +201,55 @@
             def _value_type(self) -> type:
                 return Union[str, bool]
             ```
 
         """
         pass
 
+    @staticmethod
+    def imports() -> List[str]:
+        """
+        Re-implement this function in case your Streamlit code requires specific Python package
+        import. This function should return a list of import statement as string.
+
+        Note that the following packages are already imported (not needed to return them in that
+        list): `os`, `json`, `uuid`, `pydash`, `streamlit as st`.
+
+        !!! example
+            ```py
+            @staticmethod
+            def imports() -> List[str]:
+                return [
+                    "import numpy as np",
+                    "import plotly"
+                ]
+            ```
+
+        """
+        return []
+
+    @staticmethod
+    def init() -> str:
+        """
+        Re-implement this function in case your Streamlit code requires specific initialization
+        statements. Note that all variables starting with a `_` are reserved.
+
+        !!! example
+            ```py
+            @staticmethod
+            def init() -> str:
+                return '''
+                    def x(angle):
+                        return np.deg2rad(angle%360)
+                '''
+            ```
+
+        """
+        return ''
+
     @abstractmethod
     def streamlit(
         self,
         id: str
     ) -> str:   # pragma: no cover
         """
         You must re-implement this function to return the expected Streamlit block code for
@@ -422,15 +472,15 @@
             The full parameter set constituting this element as a dictionnary.
 
         """
         k, v = self._extract()
 
         params = {
             "key": self.key,
-            "kind": type(self).__name__,
+            "kind": self.kind,
             "label": self._label,
             "value": v,
             "count": self.count,
             "optional": self.optional,
             "disabled": self.disabled,
         }
         pydash.merge(params, self._extra_args)
```

## onecode/elements/output/csv_output.py

```diff
@@ -1,26 +1,27 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
 import os
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from ...base.decorator import check_type
 from ...base.project import Project
 from ..output_element import OutputElement
 
 
 class CsvOutput(OutputElement):
     @check_type
     def __init__(
         self,
         key: str,
         value: str,
         label: Optional[str] = None,
-        tags: Optional[List[str]] = None
+        tags: Optional[List[str]] = None,
+        **kwargs: Any
     ):
         """
         A CSV table with a label on top.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -30,14 +31,16 @@
                 [examples projects](https://github.com/deeplime-io/onecode/tree/main/examples)).
             value: Path to the output CSV file which must have a `.csv` extension. Unless absolute,
                 a path is relative to the `outputs` folder of the flow currently running.
             label: Typically to be used by Streamlit for display purpose only. If not defined, it
                 will default to the `key`.
             tags: Optional meta-data information about the expected file. This information is only
                 used when the JSON output attributes are written to the output manifest.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -58,15 +61,16 @@
             ```
 
         """
         super().__init__(
             key,
             value,
             label,
-            tags=tags
+            tags=tags,
+            **kwargs
         )
 
     @property
     def value(self) -> str:
         """
         Returns:
             The path or list of paths for the output file(s): if paths are not absolute, then
@@ -93,14 +97,23 @@
 
         if ext.lower() not in valid_ext:
             raise ValueError(
                 f"[{self.key}] Invalid CSV extension: {ext} (accepted: {', '.join(valid_ext)})"
             )
 
     @staticmethod
+    def imports() -> List[str]:
+        """
+        Returns:
+            Python import statements required by the Streamlit code.
+
+        """
+        return ["from pyarrow import csv as pacsv"]
+
+    @staticmethod
     def streamlit() -> str:
         """
         Returns:
             The Streamlit code to show a table corresponding to the output CSV file.
 
         """
         return """
```

## onecode/elements/output/file_output.py

```diff
@@ -1,25 +1,26 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from ...base.decorator import check_type
 from ...base.project import Project
 from ..output_element import OutputElement
 
 
 class FileOutput(OutputElement):
     @check_type
     def __init__(
         self,
         key: str,
         value: str,
         label: Optional[str] = None,
-        tags: Optional[List[str]] = None
+        tags: Optional[List[str]] = None,
+        **kwargs: Any
     ):
         """
         Basic information about the file, such as size and file path.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -29,14 +30,16 @@
                 [examples projects](https://github.com/deeplime-io/onecode/tree/main/examples)).
             value: Path to the output file. Unless absolute, a path is relative to the `outputs`
                 folder of the flow currently running.
             label: Typically to be used by Streamlit for display purpose only. If not defined, it
                 will default to the `key`.
             tags: Optional meta-data information about the expected file. This information is only
                 used when the JSON output attributes are written to the output manifest.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -57,15 +60,16 @@
             ```
 
         """
         super().__init__(
             key,
             value,
             label,
-            tags=tags
+            tags=tags,
+            **kwargs
         )
 
     @property
     def value(self) -> str:
         """
         Returns:
             The path or list of paths for the output file(s): if paths are not absolute, then
```

## onecode/elements/output/image_output.py

```diff
@@ -1,26 +1,27 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
 import os
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from ...base.decorator import check_type
 from ...base.project import Project
 from ..output_element import OutputElement
 
 
 class ImageOutput(OutputElement):
     @check_type
     def __init__(
         self,
         key: str,
         value: str,
         label: Optional[str] = None,
-        tags: Optional[List[str]] = None
+        tags: Optional[List[str]] = None,
+        **kwargs: Any
     ):
         """
         An image as part of the image carousel.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -31,14 +32,16 @@
             value: Path to the output image file which must have a `.jpg`, `.jpeg`, `.png` or `.svg`
                 extension. Unless absolute, a path is relative to the `outputs` folder of the flow
                 currently running.
             label: Typically to be used by Streamlit for display purpose only. If not defined, it
                 will default to the `key`.
             tags: Optional meta-data information about the expected file. This information is only
                 used when the JSON output attributes are written to the output manifest.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -59,15 +62,16 @@
             ```
 
         """
         super().__init__(
             key,
             value,
             label,
-            tags=tags
+            tags=tags,
+            **kwargs
         )
 
     @property
     def value(self) -> str:
         """
         Returns:
             The path or list of paths for the output file(s): if paths are not absolute, then
```

## onecode/elements/output/text_output.py

```diff
@@ -1,26 +1,27 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from ...base.decorator import check_type
 from ...base.project import Project
 from ..output_element import OutputElement
 
 
 class TextOutput(OutputElement):
     @check_type
     def __init__(
         self,
         key: str,
         value: str,
         label: Optional[str] = None,
         tags: Optional[List[str]] = None,
-        truncate_at: int = 50000
+        truncate_at: int = 50000,
+        **kwargs: Any
     ):
         """
         A text file preview.
 
         Args:
             key: ID of the element. It must be unique as it is the key used to story data in
                 Project(), otherwise it will lead to conflicts at runtime in both execution and
@@ -31,14 +32,16 @@
             value: Path to the output CSV file which must have a `.csv` extension. Unless absolute,
                 a path is relative to the `outputs` folder of the flow currently running.
             label: Typically to be used by Streamlit for display purpose only. If not defined, it
                 will default to the `key`.
             tags: Optional meta-data information about the expected file. This information is only
                 used when the JSON output attributes are written to the output manifest.
             truncate_at: Truncate the preview at the specified number of characters.
+            **kwargs: Extra user meta-data to attach to the element. Argument names cannot overwrite
+                existing attributes or methods name such as `streamlit`, `_value`, etc.
 
         Raises:
             ValueError: if the `key` is empty or starts with `_`.
             AttributeError: if one the `kwargs` conflicts with an existing attribute or method.
 
         !!! example
             ```py
@@ -61,15 +64,16 @@
 
         """
         super().__init__(
             key,
             value,
             label,
             tags=tags,
-            truncate_at=truncate_at
+            truncate_at=truncate_at,
+            **kwargs
         )
 
     @property
     def value(self) -> str:
         """
         Returns:
             The path or list of paths for the output file(s): if paths are not absolute, then
```

## onecode/elements/output_element.py

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2023 DeepLime <contact@deeplime.io>
 # SPDX-License-Identifier: MIT
 
 import inspect
 from abc import ABC, abstractmethod
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 import pydash
 from slugify import slugify
 
 from ..base.decorator import check_type
 from ..base.project import Project
 from ..utils.format import indent_block
@@ -98,14 +98,23 @@
         if len(invalid_args) > 0:
             raise AttributeError(f'The following parameters are reserved: {invalid_args}')
 
         self._extra_args = pydash.omit(kwargs, reserved_args)
         self.__dict__.update(self._extra_args)
 
     @property
+    def kind(self) -> str:
+        """
+        Returns:
+            The element class name.
+
+        """
+        return type(self).__name__
+
+    @property
     def label(self) -> str:
         """
         Get the label with triple-quotes and escaped to handle human-readable string.
         It is primarly meant to be directly used in the Streamlit generated code for the
         `label` parameter.
         See [`streamlit()`][onecode.OutputElement.streamlit] for more information.
 
@@ -136,14 +145,55 @@
         Returns:
             By default, the same as the initial value.
 
         """
         return self._value
 
     @staticmethod
+    def imports() -> List[str]:
+        """
+        Re-implement this function in case your Streamlit code requires specific Python package
+        import. This function should return a list of import statement as string.
+
+        Note that the following packages are already imported (not needed to return them in that
+        list): `os`, `json`, `uuid`, `pydash`, `streamlit as st`.
+
+        !!! example
+            ```py
+            @staticmethod
+            def imports() -> List[str]:
+                return [
+                    "import numpy as np",
+                    "import plotly"
+                ]
+            ```
+
+        """
+        return []
+
+    @staticmethod
+    def init() -> str:
+        """
+        Re-implement this function in case your Streamlit code requires specific initialization
+        statements. Note that all variables starting with a `_` are reserved.
+
+        !!! example
+            ```py
+            @staticmethod
+            def init() -> str:
+                return '''
+                    def x(angle):
+                        return np.deg2rad(angle%360)
+                '''
+            ```
+
+        """
+        return ''
+
+    @staticmethod
     @abstractmethod
     def streamlit() -> str:   # pragma: no cover
         """
         You must re-implement this function to return the expected Streamlit block code for
         this element. This block code will be written out to the generated Streamlit App code.
 
         You should write this block code as the body of a static function yielding all internal
@@ -250,15 +300,15 @@
         val = self.value
         self._validate(val)
 
         params = {
             "key": self.key,
             "label": self._label,
             "value": val,
-            "kind": type(self).__name__
+            "kind": self.kind
         }
         pydash.merge(params, self._extra_args)
         Project().write_output(params)
 
         return self.value
 
     def _load_then_execute(self) -> Any:
@@ -295,20 +345,25 @@
 
         Returns:
             The block code generated by this `OutputElement` to be written out to the generated
             Streamlit app code.
 
         """
         # Get the _extra_args names to allow them in the function definition to be returned
+        # Remove **kwargs from the signature
+        extra_args = [*inspect.signature(cls).parameters]
+        if extra_args[-1] == "kwargs":
+            del extra_args[-1]
+
         params = pydash.uniq(
-            ['key', 'label', 'value', 'kind'] + [*inspect.signature(cls).parameters]
+            ['key', 'label', 'value', 'kind'] + extra_args
         )
 
         code_gen = f"""
-def _{cls.__name__}({'=None, '.join(params)}=None):
+def _{cls.__name__}({'=None, '.join(params)}=None, **kwargs):
 """
         code_gen += indent_block(cls.streamlit())
         code_gen += "\n"
 
         return code_gen
 
     @staticmethod
```

## onecode/utils/import_input.py

```diff
@@ -37,19 +37,30 @@
             # This makes a convenient usage in the client code:
             x = onecode.file_input('test', 'file,txt')
 
             # Rather than writing:
             x = onecode.FileInput('test', 'file.txt')()
             ```
 
-    5. export a new variable specifying the type of element being `INPUT`.
+    5. export:
+        1. a new variable specifying the type of element being `INPUT`.
+        2. a new function returning the element import statements.
+        3. a new function returning the element init statements.
 
         !!! example
             ```py
             file_input_type = ElementType.INPUT
+
+            def _file_input_importdef():
+                return FileInput.imports()
+            file_input_imports = _file_input_importdef
+
+            def _file_input_initdef():
+                return FileInput.init()
+            file_input_init = _file_input_initdef
             ```
         This is used internally by OneCode interpreter.
 
     Args:
         init_file: path to the __init__.py file located in the same directory as the input elements.
         module_name: Python name of the module to import the elements under. The module will then be
             available for importing using regular Python import statements.
@@ -71,13 +82,21 @@
                 def _x(*args, **kwargs):
                     return cls(*args, **kwargs)()
                 return _x
 
             def _typedef():
                 return ElementType.INPUT
 
+            def _importdef(cls):
+                return cls.imports()
+
+            def _initdef(cls):
+                return cls.init()
+
             setattr(sys.modules[module_name], _filename, _xdef(_cls))
             setattr(sys.modules[module_name], f'{_filename}_type', _typedef())
+            setattr(sys.modules[module_name], f'{_filename}_imports', _importdef(_cls))
+            setattr(sys.modules[module_name], f'{_filename}_init', _initdef(_cls))
             setattr(sys.modules[module_name], _ent, _cls)
 
         except AttributeError:   # pragma: no cover
             pass
```

## onecode/utils/import_output.py

```diff
@@ -46,19 +46,30 @@
             # Or for dynamically defined parameters:
             x = onecode.file_output('test', os.path.join(os.getcwd(), f'file_{my_var},txt')
 
             # Rather than writing:
             x = onecode.FileOutput('test', 'file.txt')()
             ```
 
-    5. export a new variable specifying the type of element being `OUTPUT`.
+    5. export:
+        1. a new variable specifying the type of element being `OUTPUT`.
+        2. a new function returning the element import statements.
+        3. a new function returning the element init statements.
 
         !!! example
             ```py
             file_output_type = ElementType.OUTPUT
+
+            def _file_output_importdef():
+                return FileInput.imports()
+            file_output_imports = _file_output_importdef
+
+            def _file_output_initdef():
+                return FileInput.init()
+            file_output_init = _file_output_initdef
             ```
         This is used internally by OneCode interpreter
 
     Args:
         init_file: path to the __init__.py file located in the same directory as the input elements.
         module_name: Python name of the module to import the elements under. The module will then be
             available for importing using regular Python import statements.
@@ -82,13 +93,21 @@
                     return getattr(cls, "static_call")(cls) if empty_ctor \
                         else cls(*args, **kwargs)()
                 return _x
 
             def _typedef():
                 return ElementType.OUTPUT
 
+            def _importdef(cls):
+                return cls.imports()
+
+            def _initdef(cls):
+                return cls.init()
+
             setattr(sys.modules[module_name], _filename, _xdef(_cls))
             setattr(sys.modules[module_name], f'{_filename}_type', _typedef())
+            setattr(sys.modules[module_name], f'{_filename}_imports', _importdef(_cls))
+            setattr(sys.modules[module_name], f'{_filename}_init', _initdef(_cls))
             setattr(sys.modules[module_name], _ent, _cls)
 
         except AttributeError:   # pragma: no cover
             pass
```

## onecode/utils/module.py

```diff
@@ -8,38 +8,43 @@
 from types import ModuleType
 from typing import Optional
 
 from ..base.decorator import check_type
 
 
 @check_type
-def register_ext_module(project_path: str = os.getcwd()) -> Optional[ModuleType]:
+def register_ext_module(
+    project_path: str = os.getcwd(),
+    module_name: str = "onecode_ext",
+) -> Optional[ModuleType]:
     """
-    Register the OneCode Extension module named `onecode_ext`. `onecode_ext` module is shipped by
-    default with any OneCode project. As soon as the developer creates new elements as part of this
-    module, the `onecode_ext` will be registered. See [Extending OneCode][extending-onecode] for
-    more information.
+    Register the OneCode Extension module with the specified module name: it must match the folder
+    name located in the `flows` directory of the OneCode project.
+
+    Note that a `onecode_ext` module is shipped by default with any OneCode project. As soon as the
+    developer creates new elements as part of this module, the `onecode_ext` will be registered.
+    See [Extending OneCode][extending-onecode] for more information.
 
     !!! info
         It is not required to call this function explicitely. It is already done automatically as
         part of the OneCode project under `main.py`.
 
     Args:
         project_path: Path to the root of the OneCode project.
 
     Returns:
         The module if it contains Python code, otherwise None.
 
     """
-    code_ext_path = os.path.join(project_path, 'flows', 'onecode_ext')
+    code_ext_path = os.path.join(project_path, 'flows', module_name)
     py_files = [f for f in Path(code_ext_path).rglob("*.[pP][yY]") if f.name != '__init__.py']
 
     if len(py_files) > 0:
         spec = importlib.util.spec_from_file_location(
-            "onecode_ext",
+            module_name,
             os.path.join(code_ext_path, "__init__.py")
         )
         module = importlib.util.module_from_spec(spec)
         sys.modules[spec.name] = module
         spec.loader.exec_module(module)
 
         return module
```

## Comparing `onecode-0.1.0.dist-info/LICENSE` & `onecode-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `onecode-0.1.0.dist-info/METADATA` & `onecode-0.2.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onecode
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python skeleton and library for OneCode projects
 Home-page: https://github.com/deeplime-io/onecode
 License: MIT
 Keywords: onecode,procedures
 Author: DeepLime
 Author-email: contact@deeplime.io
 Requires-Python: >=3.7,<3.11
@@ -13,49 +13,50 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Code Generators
 Provides-Extra: developer
 Provides-Extra: docs
 Provides-Extra: tech-expert
+Requires-Dist: altair (<5); extra == "tech-expert" or extra == "developer"
 Requires-Dist: astunparse (>=1.6.3,<2.0.0)
-Requires-Dist: datatest (>=0.11.1,<0.12.0) ; extra == "developer"
+Requires-Dist: datatest (>=0.11.1,<0.12.0); extra == "developer"
 Requires-Dist: flufl.lock (>=7.1.1,<8.0.0)
-Requires-Dist: griffe (==0.25.0) ; extra == "docs"
+Requires-Dist: griffe (==0.25.0); extra == "docs"
 Requires-Dist: inquirerpy (>=0.3.3,<0.4.0)
-Requires-Dist: markdown-katex (==202112.1034) ; extra == "docs"
-Requires-Dist: mike (==1.1.2) ; extra == "docs"
-Requires-Dist: mkdocs (==1.4.2) ; extra == "docs"
-Requires-Dist: mkdocs-jupyter (==0.21.0) ; extra == "docs"
-Requires-Dist: mkdocs-material (==8.5.10) ; extra == "docs"
-Requires-Dist: mkdocstrings (==0.19.0) ; extra == "docs"
-Requires-Dist: mkdocstrings-python (==0.7.1) ; extra == "docs"
+Requires-Dist: markdown-katex (==202112.1034); extra == "docs"
+Requires-Dist: mike (==1.1.2); extra == "docs"
+Requires-Dist: mkdocs (==1.4.2); extra == "docs"
+Requires-Dist: mkdocs-jupyter (==0.21.0); extra == "docs"
+Requires-Dist: mkdocs-material (==8.5.10); extra == "docs"
+Requires-Dist: mkdocstrings (==0.19.0); extra == "docs"
+Requires-Dist: mkdocstrings-python (==0.7.1); extra == "docs"
 Requires-Dist: onecode-pycg (>=0.0.7,<0.0.8)
-Requires-Dist: pandas (>=1.4.0,<2.0.0)
-Requires-Dist: pyarrow (>=6.0.0,<7.0.0)
+Requires-Dist: pandas (>=1.4.0)
+Requires-Dist: pyarrow (>=6.0.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: pydash (>=5.1.0,<6.0.0)
-Requires-Dist: pytest (>=6.0.2,<7.0.0) ; extra == "developer"
-Requires-Dist: pytest-cov (>=2.10.1,<3.0.0) ; extra == "developer"
-Requires-Dist: pytest-xdist (>=3.1.0,<4.0.0) ; extra == "developer"
+Requires-Dist: pytest (>=6.0.2,<7.0.0); extra == "developer"
+Requires-Dist: pytest-cov (>=2.10.1,<3.0.0); extra == "developer"
+Requires-Dist: pytest-xdist (>=3.1.0,<4.0.0); extra == "developer"
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
-Requires-Dist: streamlit (>=1.12.0,<1.18) ; extra == "tech-expert" or extra == "developer"
-Requires-Dist: streamlit-image-select (>=0.5.1,<0.6.0) ; extra == "tech-expert" or extra == "developer"
-Requires-Dist: streamlit-option-menu (>=0.3.2,<0.4.0) ; extra == "tech-expert" or extra == "developer"
-Requires-Dist: streamlit_tree_select (>=0.0.5,<0.0.6) ; extra == "tech-expert" or extra == "developer"
-Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "developer"
+Requires-Dist: streamlit (>=1.12.0,<1.18); extra == "tech-expert" or extra == "developer"
+Requires-Dist: streamlit-image-select (>=0.5.1,<0.6.0); extra == "tech-expert" or extra == "developer"
+Requires-Dist: streamlit-option-menu (>=0.3.2,<0.4.0); extra == "tech-expert" or extra == "developer"
+Requires-Dist: streamlit_tree_select (>=0.0.5,<0.0.6); extra == "tech-expert" or extra == "developer"
+Requires-Dist: toml (>=0.10.2,<0.11.0); extra == "developer"
 Requires-Dist: typeguard (>=2.13.3,<3.0.0)
 Requires-Dist: yaspin (>=2.1.0,<3.0.0)
 Project-URL: Documentation, https://deeplime-io.github.io/onecode
 Project-URL: Repository, https://github.com/deeplime-io/onecode
 Description-Content-Type: text/markdown
 
 ![onecode_logo](https://github.com/deeplime-io/onecode/raw/main/docs/assets/onecode.jpg)
```

## Comparing `onecode-0.1.0.dist-info/RECORD` & `onecode-0.2.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-onecode/__init__.py,sha256=p_H92fSuhcxJnDLR2PUovKD3WUkJ2WkYRLgB4vAVA6Q,183
-onecode/base/__init__.py,sha256=m0m9AiZ7STKuVa1LxwD3FvksKX_i9rELUYL3x-epfzY,160
+onecode/__init__.py,sha256=yEnyAEr00Y2IMNU5TZyO6vVNZiHkrJLHqU4S5-VWK9U,183
+onecode/base/__init__.py,sha256=r0nBrRtglwYUlBTXlJe3fpcRjX95CK1MlS1ErTn3gZY,185
 onecode/base/decorator.py,sha256=6mkugfoq9VPbCkigEvOJZ4_RPIZ0WBE94cNIDgUxs4I,714
-onecode/base/enums.py,sha256=fzAin9SxJ5RuarKs7mqkfPK6y_ff_Ds1GfiXi0jVUoc,5151
-onecode/base/logger.py,sha256=P1PXuoOxbbp2cvAz0rg4MzX-6iviqprdKFhKYEkqye0,7422
-onecode/base/project.py,sha256=8Rgv1w-p4oQ0oYCWWav0bjPPGsM3kmNXwbvLZtxDJ6g,12359
+onecode/base/enums.py,sha256=OnABi2Rvwf6yLDneaEMT5OLE-7Bk6ieD4j116ZEqrS0,5729
+onecode/base/logger.py,sha256=nCQN2H1QO1iWQH6cVeCUyk7VTeqqw9v5Eay9J24tnj0,7963
+onecode/base/project.py,sha256=vaqB76z1bHwgK6pshkXDITpx2qc5mXDJoIPu6ehO3sQ,12896
 onecode/base/singleton.py,sha256=1yDuOvbaql1_FA9bcjWJCo5g4l2oDbmF2j4U8hBpccA,482
 onecode/cli/__init__.py,sha256=E6RTMZXnyNFy0YoNvk4q2oiYrmzSkXsPk-raO3IKtIU,115
 onecode/cli/add.py,sha256=9o4mkgSPDgH-DF-6rg2U9FaBkw0yznb83avtQNG5vWk,2693
 onecode/cli/create.py,sha256=_jmRzu32fpVIWdBgP7TRtQiSybhmqfO-G4xlHUj5Rdc,3883
 onecode/cli/extract.py,sha256=czZY9crHF5vaRakt0Ig8iPUqLo0fNpEQjYgemKXWRGk,6029
 onecode/cli/skeleton/.gitignore,sha256=yXKwjiECKmcw4GPMyw2AKSQXh126dnMrxTT1XGhqc44,1946
 onecode/cli/skeleton/LICENSE,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
@@ -15,37 +15,39 @@
 onecode/cli/skeleton/data/README.md,sha256=qNLKuG7pjz4Df6mvJsB68cG17W_olHcInHGccNSG9ik,138
 onecode/cli/skeleton/flows/README.md,sha256=hX0e23rlTtpYcaYoKTQMSm0l8R4S1ewp0VTteSIe-JE,62
 onecode/cli/skeleton/flows/onecode_ext/README.md,sha256=EgQcQt20lCPRYsQApMI_a_OarWeO_W5iDpG0QTQCsRQ,310
 onecode/cli/skeleton/flows/onecode_ext/__init__.py,sha256=8mW3U1XiFedmO1Oka8QC-goCogB5LNUg75vsvyZZf-w,61
 onecode/cli/skeleton/flows/onecode_ext/input_elements/__init__.py,sha256=WyXazFy_4uPJsLbhvtVhwzAz12o3wegsgUPQJmj2obY,67
 onecode/cli/skeleton/flows/onecode_ext/output_elements/__init__.py,sha256=5MnT8JRs0fcOgWSt6erf8jFPifUPtdRmSWsFsbJ6MDw,69
 onecode/cli/skeleton/main.py,sha256=Q9A38oxGeXLG-XQLYJI1aSDYjMi1ndHzDIg-AohJFJ4,3363
-onecode/cli/start.py,sha256=Gvih8H63cxO8FIW692HedER2qUQI-itWqnNlkDF2Ujc,12881
+onecode/cli/start.py,sha256=XipaS_h58X9om30XlJeI9mWcj-pvqjZjgqh2QLZ6tbI,14618
 onecode/cli/utils.py,sha256=Xmw3pIsVDCx1hfPWjGWAA5pLy8RjOQq2-DD8g-6DA24,8073
 onecode/elements/__init__.py,sha256=rf3uofycvzH4AtvR03d2344wVUUJXaDvdd5qlQrC3ZM,196
 onecode/elements/input/__init__.py,sha256=6dqleLWaihtRAC-KHYYLQjx5AhnjPR4vfiT0ILjlZ4k,162
-onecode/elements/input/checkbox.py,sha256=0xskMgvcS8YWpDF0TYo0MuSmtxJ-BGjaAR_GvlsT1Hk,3570
-onecode/elements/input/csv_reader.py,sha256=60aODvAp5gg-xqegEVpIXUDzePVnl_vdIeHuWqeQcTA,5634
-onecode/elements/input/dropdown.py,sha256=INKyb_vDfZ9QSROns1uQXBY19_z6-x8mGG6GB4kyEuQ,6919
-onecode/elements/input/file_input.py,sha256=Gb7k97N96SFXRhHdUFF3nLxdY2wxZRwhZh_c_Q__E0g,7925
-onecode/elements/input/number_input.py,sha256=vkGFCTTKzGUQkiIx4Sy18OZJlk5bO0wZsevJ2yQVQqs,4659
-onecode/elements/input/radio_button.py,sha256=r477rBUjAe3UT7MQPu2q9WU1PgA0SsxEDwYln33j2H8,4887
-onecode/elements/input/slider.py,sha256=N2GRxoaubt4vdQeBQdl8NOkB2_wCBP8UhiN_8OXYaxk,4729
-onecode/elements/input/text_input.py,sha256=wgUqjooJZXWmJ4Kumu4fE5eOfXSNbsOFWeo_8evRT9o,4421
-onecode/elements/input_element.py,sha256=BPZY_5EWZkn4wPW2QXXxYpXhjV5lu9JGWzFFaQBC7rs,18308
+onecode/elements/input/checkbox.py,sha256=pcZSVxSm26J3BDq0Bs43PHF6p_0QK7z6euKkapc5NOQ,3809
+onecode/elements/input/csv_reader.py,sha256=E8NjMmd-8rAtbyD_m-A3agsBtq8wtxXwBIX7B-SE93o,6087
+onecode/elements/input/dropdown.py,sha256=9lEfIAlrx7ZDovBundb878_j5nYeiF8s7PjrbGsLHCA,7159
+onecode/elements/input/file_input.py,sha256=9u8VY9rBM6OB8cl6UmAubfXK-OW_pdwY64AxXplyj_M,8708
+onecode/elements/input/folder_input.py,sha256=H17e2RBo8tH1r7H8gL4xKxb9099b53mhuIL1nLgfpEE,6651
+onecode/elements/input/number_input.py,sha256=Sb85coEpSJUAUC4r1mTEHjASFbKv3RDMEjo0JUP03wk,4897
+onecode/elements/input/radio_button.py,sha256=CQKn_8UtfYD0Y0h-6NRkodOTU0-dCnJGaqVXW_ER6FA,5126
+onecode/elements/input/slider.py,sha256=kIKxoK_rVr2XQ1OOYdHjcZUuH_7d_tCoxi8wSpxdJro,4967
+onecode/elements/input/text_input.py,sha256=QGWydgoXw2rl5GRFffL_UFiYcdk4hU8fH6awM0sV7nk,4660
+onecode/elements/input_element.py,sha256=7s6SuPSp_xgGXsHuMBCjlity_WEraqCv6wnypYq50JY,19642
 onecode/elements/output/__init__.py,sha256=eDVCf5vm3ZMRCxwEOvOy1-zvYKraBEo4Ok04gdet_cc,164
-onecode/elements/output/csv_output.py,sha256=PJyMtHYKIOg5Ggh91qZsbGW62uavE2dFg2e2XYjRrvk,3909
-onecode/elements/output/file_output.py,sha256=JE35XDGt_pRBifb6fcq7MG7RZvFX1XFZRLFtWt5ycLY,3435
-onecode/elements/output/image_output.py,sha256=f1yhbQnVVVXmugi6OhlAhy3wmnxHCmIHSyF1gWyvd9k,3867
-onecode/elements/output/text_output.py,sha256=24hycNVXCe5n5tQ7WiGq5T5jFX3hg92xMu7TzIkjyZA,3694
-onecode/elements/output_element.py,sha256=Gz5mnwmoW5xuMLaXB98S0pMz9OU3zAYwzrZbkK2aris,11408
+onecode/elements/output/csv_output.py,sha256=ITmpRlkh7-ysNBt6pHyK5VGOJo-svVLePj90V7HXRRA,4362
+onecode/elements/output/file_output.py,sha256=4-itB63Npfe0ivMT4bqhcSahzCgmPGbLLfzr_jD28E8,3674
+onecode/elements/output/image_output.py,sha256=ZwAdquU1sMBOX77yOAvekSeu8osth73PDh4l3fgeUXw,4106
+onecode/elements/output/plotly_output.py,sha256=qYJZWiuiSUiBlj-ho3c-Haii2HssFH3BDTfGYolAroA,4007
+onecode/elements/output/text_output.py,sha256=tdhDQsAfysW-R3o9XsKYpkGK-WUs8ehzZi6q8KmmxmA,3933
+onecode/elements/output_element.py,sha256=UUZZA0iaC_l4gbUDc2ccNOtM4w2vm0KK2BWOJorT5BY,12900
 onecode/utils/__init__.py,sha256=v5pCZdf8U8r9p4-aDMahrD7JG5_2b-IjCuVlgrH2xxw,217
 onecode/utils/format.py,sha256=ed8BS34_zXZgQbiCIWG2UFnSIK5Pv8YanZYrXo6S9Ms,1089
-onecode/utils/import_input.py,sha256=hzmOAQZjCSi0fJplqWrgf_7QfF0pn6NJI-iVflloLro,2896
-onecode/utils/import_output.py,sha256=ChjrF-E3XErGas943DOq2vxmV2Q6q-C6eLxtqqQQpoI,3688
-onecode/utils/module.py,sha256=qgckF1QrVHzYArfTzMVVphJW90GF4QHeCREyrKYC2Wc,1499
+onecode/utils/import_input.py,sha256=evv2rAiOzlsDFGXj3HGhzXd-4pTd2qOMtnzQHBB9Kd8,3618
+onecode/utils/import_output.py,sha256=brwqFl7i-HI20wbMQJxOJRiSecVSGCM0m5FvfDHDhH4,4416
+onecode/utils/module.py,sha256=dtdVccnU6rpYftCRWOtoJ5pehsueFUTH4uit6Jy75Bc,1655
 onecode/utils/typing.py,sha256=sK4Z6GCeU-sC5fVwDT1LZsbHCSdGJIapkMnYWucWiHc,692
-onecode-0.1.0.dist-info/LICENSE,sha256=YNGjVtsBDBrKEGZ4k7k5j37ADm7ovbKdtKrGOvLc8Qs,1069
-onecode-0.1.0.dist-info/METADATA,sha256=f9eKVrUYGOlO1uvhzKYUvQEYqjVj18gsLvsHD1w-C2g,6141
-onecode-0.1.0.dist-info/WHEEL,sha256=UTbu2d3PIo7FtACOQrq825bNtQhldwLx2SG2oh0Fl8Q,88
-onecode-0.1.0.dist-info/entry_points.txt,sha256=JzOvWgpdLE7UVvSjXTr75YFYodd7AqSAQAz_nmJvxFI,169
-onecode-0.1.0.dist-info/RECORD,,
+onecode-0.2.0.dist-info/entry_points.txt,sha256=JzOvWgpdLE7UVvSjXTr75YFYodd7AqSAQAz_nmJvxFI,169
+onecode-0.2.0.dist-info/LICENSE,sha256=YNGjVtsBDBrKEGZ4k7k5j37ADm7ovbKdtKrGOvLc8Qs,1069
+onecode-0.2.0.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
+onecode-0.2.0.dist-info/METADATA,sha256=Vex1T4n9BKZisQTDNVtyjXznSAQv26OgPr3mXQ6QnyA,6185
+onecode-0.2.0.dist-info/RECORD,,
```

