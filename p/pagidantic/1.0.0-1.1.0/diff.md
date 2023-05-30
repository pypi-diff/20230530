# Comparing `tmp/pagidantic-1.0.0.tar.gz` & `tmp/pagidantic-1.1.0.tar.gz`

## Comparing `pagidantic-1.0.0.tar` & `pagidantic-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pagidantic-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pagidantic-1.0.0/codecov.yml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pagidantic-1.0.0/.github/CODEOWNERS
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pagidantic-1.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pagidantic-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0    17272 2020-02-02 00:00:00.000000 pagidantic-1.0.0/.github/logo.png
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pagidantic-1.0.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pagidantic-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pagidantic-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pagidantic-1.0.0/pagidantic/__init__.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 pagidantic-1.0.0/pagidantic/dict.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pagidantic-1.0.0/pagidantic/factory.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 pagidantic-1.0.0/pagidantic/page.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pagidantic-1.0.0/pagidantic/pagidantic.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 pagidantic-1.0.0/pagidantic/paginator.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pagidantic-1.0.0/pagidantic/set.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pagidantic-1.0.0/scripts/clean.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pagidantic-1.0.0/scripts/format.sh
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pagidantic-1.0.0/scripts/lint.sh
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 pagidantic-1.0.0/scripts/test.sh
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pagidantic-1.0.0/scripts/test_html.sh
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pagidantic-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pagidantic-1.0.0/tests/test_pagidantic_factory.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 pagidantic-1.0.0/tests/test_pagidantic_paginator.py
--rw-r--r--   0        0        0    10073 2020-02-02 00:00:00.000000 pagidantic-1.0.0/tests/test_pagidantic_paginator_default.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pagidantic-1.0.0/tests/test_pagidantic_proxy.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pagidantic-1.0.0/tests/test_version.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 pagidantic-1.0.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pagidantic-1.0.0/LICENSE
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pagidantic-1.0.0/README.md
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 pagidantic-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 pagidantic-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pagidantic-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pagidantic-1.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pagidantic-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0    17272 2020-02-02 00:00:00.000000 pagidantic-1.1.0/.github/logo.png
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 pagidantic-1.1.0/.github/workflows/cache.yml
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pagidantic-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 pagidantic-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pagidantic-1.1.0/pagidantic/__init__.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pagidantic-1.1.0/pagidantic/dict.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pagidantic-1.1.0/pagidantic/factory.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 pagidantic-1.1.0/pagidantic/page.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 pagidantic-1.1.0/pagidantic/pagidantic.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pagidantic-1.1.0/pagidantic/paginator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pagidantic-1.1.0/pagidantic/py.typed
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 pagidantic-1.1.0/pagidantic/set.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pagidantic-1.1.0/scripts/clean.sh
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pagidantic-1.1.0/scripts/example.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pagidantic-1.1.0/scripts/format.sh
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pagidantic-1.1.0/scripts/lint.sh
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 pagidantic-1.1.0/scripts/test.sh
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pagidantic-1.1.0/scripts/test_html.sh
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pagidantic-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pagidantic-1.1.0/tests/test_pagidantic_factory.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 pagidantic-1.1.0/tests/test_pagidantic_paginator.py
+-rw-r--r--   0        0        0    10073 2020-02-02 00:00:00.000000 pagidantic-1.1.0/tests/test_pagidantic_paginator_default.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pagidantic-1.1.0/tests/test_pagidantic_proxy.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pagidantic-1.1.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pagidantic-1.1.0/tests/example/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pagidantic-1.1.0/tests/example/example.py
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 pagidantic-1.1.0/tests/example/generated.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 pagidantic-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pagidantic-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pagidantic-1.1.0/README.md
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 pagidantic-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 pagidantic-1.1.0/PKG-INFO
```

### Comparing `pagidantic-1.0.0/.pre-commit-config.yaml` & `pagidantic-1.1.0/.pre-commit-config.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# See https://pre-commit.com for more information
-# See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
     -   id: check-added-large-files
     -   id: check-toml
     -   id: check-yaml
@@ -15,24 +13,21 @@
     rev: v3.3.1
     hooks:
     -   id: pyupgrade
         args:
         - --py3-plus
         - --keep-runtime-typing
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.229
+    rev: v0.0.236
     hooks:
     -   id: ruff
         args:
         - --fix
 -   repo: https://github.com/pycqa/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
     -   id: isort
         name: isort (python)
 -   repo: https://github.com/psf/black
     rev: 22.12.0
     hooks:
     -   id: black
-ci:
-    autofix_commit_msg: 🎨 [pre-commit.ci] Auto format from pre-commit.com hooks
-    autoupdate_commit_msg: ⬆ [pre-commit.ci] pre-commit autoupdate
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pagidantic-1.0.0/.github/logo.png` & `pagidantic-1.1.0/.github/logo.png`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/.github/workflows/release.yml` & `pagidantic-1.1.0/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,14 @@
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-publish
       - name: Install build dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install build
       - name: Build distribution
         run: python -m build
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.6.4
+        uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
```

### Comparing `pagidantic-1.0.0/.github/workflows/test.yml` & `pagidantic-1.1.0/.github/workflows/test.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,71 @@
 name: Test Suite
 
 on:
   push:
     branches:
       - main
-  pull_request:
-    types: [opened, synchronize]
+  pull_request: {}
 
 jobs:
-  tests:
+  lint:
     runs-on: ubuntu-latest
-    timeout-minutes: 30
     strategy:
       matrix:
-        python-version: ["3.9","3.10", "3.11"]
+        python-version: ["3.11"]
+      fail-fast: false
+    steps:
+      - uses: actions/checkout@v3
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install Dependencies
+        run: pip install -e .[lint]
+      - uses: pre-commit/action@v3.0.0
+        with:
+          extra_args: --all-files --verbose
+      - name: check Static Analysis
+        run: bash scripts/lint.sh
 
+  test:
+    name: test on python ${{ matrix.python-version }}
+    runs-on: ubuntu-latest
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
-          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test-v02
+          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test
       - name: Upgrade pip
         run: |
           python -m pip install --upgrade pip
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install -e .[test]
       - name: Test with pytest
         run: bash scripts/test.sh
       - name: Upload coverage
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
         uses: codecov/codecov-action@v3
+      - name: Test Simple Example
+        run: bash scripts/example.sh
+  # https://github.com/marketplace/actions/alls-green#why used for branch protection checks
+  check:
+    if: always()
+    needs: [lint, test]
+    runs-on: ubuntu-latest
+    steps:
+      - name: Decide whether the needed jobs succeeded or failed
+        uses: re-actors/alls-green@release/v1
+        with:
+          jobs: ${{ toJSON(needs) }}
```

### Comparing `pagidantic-1.0.0/pagidantic/__init__.py` & `pagidantic-1.1.0/pagidantic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 It's easy to use, lightweight, and easy to integrate with existing projects.
 
 It helps in creating efficient pagination solution with minimal code, while maintaining type checking and data validation with Pydantic.
 """
 
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 from pagidantic.dict import PagidanticDict
 from pagidantic.factory import PagidanticFactory
 from pagidantic.page import Page
 from pagidantic.pagidantic import pagidantic
 from pagidantic.paginator import Paginator
 from pagidantic.set import PagidanticSet
```

### Comparing `pagidantic-1.0.0/pagidantic/dict.py` & `pagidantic-1.1.0/pagidantic/set.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+from typing import Any, List
+
 from pagidantic.paginator import Paginator
 
 
-class PagidanticDict(Paginator):
+class PagidanticSet(Paginator):
     """
-    Initialize a Paginator for paginating a dictionary.
+    Initialize a Paginator for paginating a set.
 
-    :param object_list: The dictionary to be paginated.
+    :param object_list: The set to be paginated.
     :type object_list: dict
     :param page_limit: Number of items per page.
     :type page_limit: int, optional
     :param start_page: The page to start pagination from.
     :type start_page: int, optional
     """
 
-    def __init__(self, object_list: dict, page_limit: int = 10, start_page: int = 0):
+    def __init__(
+        self, object_list: List[Any], page_limit: int = 10, start_page: int = 0
+    ):
         self.object_list = object_list
         super().__init__(
-            object_list=self._dict_to_list(),
+            object_list=self._set_to_list(),
             page_limit=page_limit,
             start_page=start_page,
         )
 
-    def _dict_to_list(self) -> list[dict]:
-        """Transform dict to list of dicts."""
-        if not isinstance(self.object_list, dict):
-            raise TypeError(f"Expected dict object, not {type(self.object_list)}")
-        return [{k: v} for k, v in self.object_list.items()]
+    def _set_to_list(self) -> List[Any]:
+        """Transform set to list of sets."""
+        if not isinstance(self.object_list, set):
+            raise TypeError(f"Expected set object, not {type(self.object_list)}")
+        return list(self.object_list)
```

### Comparing `pagidantic-1.0.0/pagidantic/factory.py` & `pagidantic-1.1.0/pagidantic/factory.py`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/pagidantic/page.py` & `pagidantic-1.1.0/pagidantic/page.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 class Page:
     """
     A Page object, which contains a list of objects and some additional information such as the current page number and
     the paginator instance.
     """
 
-    def __init__(self, object_list: Sequence, page_number: int, paginator):
+    def __init__(
+        self, object_list: Sequence[object], page_number: int, paginator: object
+    ):
         """
         Initialize a Page object with a list of objects, the current page number, and a paginator instance.
 
         :param object_list: A list of objects to be paginated.
         :type object_list: Sequence
         :param page_number: The current page number.
         :type page_number: int
@@ -25,27 +27,27 @@
     def has_next(self) -> bool:
         """
         Check if paginator has next page.
 
         :return: True if the paginator has a next page, False otherwise.
         :rtype: bool
         """
-        return self.page_number < self.paginator.total_pages
+        return self.page_number < self.paginator.total_pages  # type: ignore
 
     def has_previous(self) -> bool:
         """
         Check if paginator has previous page.
 
         :return: True if the paginator has a previous page, False otherwise.
         :rtype: bool
         """
         return self.page_number > 0
 
     @property
-    def count(self):
+    def count(self) -> int:
         """
         Return a number of page objects.
 
         :return: The number of objects in the current page.
         :rtype: int
         """
         return len(self.object_list)
```

### Comparing `pagidantic-1.0.0/pagidantic/pagidantic.py` & `pagidantic-1.1.0/pagidantic/pagidantic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-from typing import Type, Union
+from typing import Any, List, Set, Tuple, Type, Union
 
 from pagidantic.factory import PagidanticFactory
 from pagidantic.paginator import Paginator
 
 
 def pagidantic(
-    object_list: Union[list, tuple, dict, set],
+    object_list: Union[
+        list[List[Any]],
+        tuple[Tuple[Any]],
+        dict[Any, Any],
+        set[Set[Any]],
+    ],
     page_limit: int = 10,
     start_page: int = 0,
-):
+) -> Paginator:
     """
     This function create a paginator instance based on the type of the object list passed
 
     :param object_list: list, tuple, dict or set of objects to be paginated.
     :type object_list: Union[list, tuple, dict, set]
     :param page_limit: Number of items per page.
     :type page_limit: int, optional
     :param start_page: The page to start pagination from.
     :type start_page: int, optional
     :return: paginator instance
     :rtype: Paginator
     """
-    factory = PagidanticFactory(type(object_list).__name__)
+    factory = PagidanticFactory(objects_type=type(object_list).__name__)
     paginator: Type[Paginator] = factory.get_paginator()
     return paginator(
         object_list=object_list,
         page_limit=page_limit,
         start_page=start_page,
     )
```

### Comparing `pagidantic-1.0.0/pagidantic/paginator.py` & `pagidantic-1.1.0/pagidantic/paginator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 from functools import cached_property
-from typing import Sequence, Union
+from typing import Any, Dict, Generator, List, Sequence, Set, Tuple, Union
 
 from pydantic.dataclasses import dataclass
 
 from pagidantic.page import Page
 
 
 @dataclass
@@ -14,41 +14,46 @@
 
     Arguments:
         :object_list: list of sequential objects that will be split across pages.
         :page_limit: number of objects per page.
         :start_page: number of page from which paginator will start.
     """
 
-    object_list: Union[list, tuple, dict, set]
+    object_list: Union[
+        List[Any],
+        Tuple[Any],
+        Dict[Any, Any],
+        Set[Any],
+    ]
     page_limit: int = 10
     start_page: int = 0
 
-    def __post_init_post_parse__(self):
+    def __post_init_post_parse__(self) -> None:
         """Executed after initial validation. Set initial page."""
         self.page: Page = self._page(
             object_list=self.get_objects(self.start_page),
             page_number=self.start_page,
             paginator=self,
         )
 
-    def __iter__(self):
+    def __iter__(self) -> Generator["Page", None, None]:
         """Iterate over paginator pages. Every iteration updates paginator page object."""
         for _ in self.page_range:
             yield self.page
             self.get_next()
 
-    def get_objects(self, page_number: int) -> Sequence:
+    def get_objects(self, page_number: int) -> Sequence[Any]:
         """Retrieve page list of data."""
         if not isinstance(page_number, int):
             raise TypeError(f"{page_number} expected to be int.")
         n = self.page_limit * page_number
-        return self.object_list[n : n + self.page_limit]
+        return self.object_list[n : n + self.page_limit]  # type: ignore
 
     @property
-    def response(self):
+    def response(self) -> Dict[str, Any]:
         """Retrieve response result property."""
         data = {
             "data": self.page.object_list,
             "page_number": self.page.page_number,
             "has_next": self.has_next,
             "has_previous": self.has_previous,
         }
@@ -61,76 +66,76 @@
 
     @property
     def has_previous(self) -> bool:
         """Page's "has previous" method."""
         return self.page.has_previous()
 
     def get_next(self) -> None:
-        """Get next page. Overrides paginator\'s page attribute"""
+        """Get next page. Overrides paginator's page attribute"""
         if self.has_next:
             self.page.page_number += 1
             next_page = self._page(
                 object_list=self.get_objects(self.page.page_number),
                 page_number=self.page.page_number,
                 paginator=self,
             )
-            self.page = next_page  # noqa
+            self.page = next_page
 
     def get_previous(self) -> None:
-        """Get previous page. Overrides paginator\'s page attribute."""
+        """Get previous page. Overrides paginator's page attribute."""
         if self.has_previous:
             self.page.page_number -= 1
             previous_page = self._page(
                 object_list=self.get_objects(self.page.page_number),
                 page_number=self.page.page_number,
                 paginator=self,
             )
-            self.page = previous_page  # noqa
+            self.page = previous_page
 
     @staticmethod
-    def _page(*args, **kwargs) -> Page:
+    def _page(*args: Any, **kwargs: Any) -> Page:
         """Returns Page object."""
         return Page(*args, **kwargs)
 
-    def get_page_response(self, page_number: int = 0):
+    def get_page_response(self, page_number: int = 0) -> Dict[str, Any]:
         """
         Get response of requested page number.
         number=0 equals first page.
         """
         if not isinstance(page_number, int):
             raise TypeError(f"{page_number} expected to be int.")
         page = self._page(
             object_list=self.get_objects(page_number),
             page_number=page_number,
             paginator=self,
         )
         data = {
             "data": page.object_list,
-            "page_number": page_number,
+            "page_number": page.page_number,
             "has_next": page.has_next(),
             "has_previous": page.has_previous(),
         }
         return self._create_response(**data)
 
     @cached_property
-    def total(self):
+    def total(self) -> int:
         """Return the total number of objects, across all pages."""
         return len(self.object_list)
 
     @property
-    def total_pages(self):
+    def total_pages(self) -> int:
         """Number of total pages. Lack of additional pages means total is 0."""
         return 0 if self.total == 0 else math.ceil(self.total / self.page_limit) - 1
 
     @property
-    def page_range(self):
+    def page_range(self) -> range:
         """Return a range of pages."""
         return range(self.total_pages + 1 - self.start_page)
 
-    def _create_response(self, **kwargs):
+    def _create_response(self, **kwargs: Any) -> Dict[str, Any]:
         """Creates json response object."""
         return {
             "total_pages": self.total_pages,
             "data": kwargs["data"],
             "page_number": kwargs["page_number"],
             "has_next": kwargs["has_next"],
             "has_previous": kwargs["has_previous"],
```

### Comparing `pagidantic-1.0.0/pagidantic/set.py` & `pagidantic-1.1.0/pagidantic/dict.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+from typing import Any, Dict, List
+
 from pagidantic.paginator import Paginator
 
 
-class PagidanticSet(Paginator):
+class PagidanticDict(Paginator):
     """
-    Initialize a Paginator for paginating a set.
+    Initialize a Paginator for paginating a dictionary.
 
-    :param object_list: The set to be paginated.
+    :param object_list: The dictionary to be paginated.
     :type object_list: dict
     :param page_limit: Number of items per page.
     :type page_limit: int, optional
     :param start_page: The page to start pagination from.
     :type start_page: int, optional
     """
 
-    def __init__(self, object_list: set, page_limit: int = 10, start_page: int = 0):
-        self.object_list = object_list
+    def __init__(
+        self, object_list: Dict[Any, Any], page_limit: int = 10, start_page: int = 0
+    ):
+        self.object_list: Dict[Any, Any] = object_list
         super().__init__(
-            object_list=self._set_to_list(),
+            object_list=self._dict_to_list(),
             page_limit=page_limit,
             start_page=start_page,
         )
 
-    def _set_to_list(self) -> list[set]:
-        """Transform set to list of sets."""
-        if not isinstance(self.object_list, set):
-            raise TypeError(f"Expected set object, not {type(self.object_list)}")
-        return list(self.object_list)
+    def _dict_to_list(self) -> List[Dict[Any, Any]]:
+        """Transform dict to list of dicts."""
+        if not isinstance(self.object_list, dict):
+            raise TypeError(f"Expected dict object, not {type(self.object_list)}")
+        return [{k: v} for k, v in self.object_list.items()]
```

### Comparing `pagidantic-1.0.0/scripts/clean.sh` & `pagidantic-1.1.0/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/tests/conftest.py` & `pagidantic-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/tests/test_pagidantic_factory.py` & `pagidantic-1.1.0/tests/test_pagidantic_factory.py`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/tests/test_pagidantic_paginator.py` & `pagidantic-1.1.0/tests/test_pagidantic_paginator.py`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/tests/test_pagidantic_paginator_default.py` & `pagidantic-1.1.0/tests/test_pagidantic_paginator_default.py`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/tests/test_pagidantic_proxy.py` & `pagidantic-1.1.0/tests/test_pagidantic_proxy.py`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/.gitignore` & `pagidantic-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/LICENSE` & `pagidantic-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/README.md` & `pagidantic-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pagidantic-1.0.0/pyproject.toml` & `pagidantic-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,44 +12,46 @@
     { name = "Yasser Tahiri", email = "hello@yezz.me" },
 ]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
+    "Development Status :: 5 - Production/Stable",
+    "Framework :: Pydantic",
+    "Framework :: Pydantic :: 1",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "typing-extensions >=3.7.4,<4.5.0",
+    "typing-extensions >=3.7.4,<4.7.0",
     "pydantic >=1.6.2,!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/yezz123/pagidantic"
 Funding = 'https://github.com/sponsors/yezz123'
 
 [project.optional-dependencies]
 lint = [
-    "pre-commit==2.21.0",
-    "mypy==0.991",
+    "mypy==1.3.0",
+    "pre-commit==3.3.2",
 ]
 test = [
-    "pytest==7.2.1",
-    "pytest-asyncio == 0.20.3",
-    "codecov==2.1.12",
-    "pytest-cov==4.0.0",
+    "pytest==7.3.1",
+    "pytest-asyncio == 0.21.0",
+    "pytest-cov==4.1.0",
 ]
 
 
 [tool.hatch.version]
 path = "pagidantic/__init__.py"
 
 [tool.isort]
@@ -76,27 +78,44 @@
 
 [tool.ruff.isort]
 known-third-party = ["pydantic", "typing_extensions"]
 
 [tool.mypy]
 plugins = "pydantic.mypy"
 follow_imports = "silent"
+python_version = '3.10'
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
 check_untyped_defs = true
 ignore_missing_imports = true
 disallow_untyped_defs = true
+show_error_codes = true
+no_implicit_reexport = false
+warn_unused_configs = true
+disallow_subclassing_any = true
+disallow_incomplete_defs = true
+disallow_untyped_decorators = true
+disallow_untyped_calls = true
+implicit_optional = true
 
 [[tool.mypy.overrides]]
 module = "pagidantic.tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 
+[tool.coverage.run]
+parallel = true
+source = [
+    "tests",
+    "pagidantic"
+]
+context = '${CONTEXT}'
+
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
     "raise NotImplemented",
     "@overload",
```

### Comparing `pagidantic-1.0.0/PKG-INFO` & `pagidantic-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: pagidantic
-Version: 1.0.0
+Version: 1.1.0
 Summary: Pagination using Pydantic. Easy to use, lightweight, and easy to integrate with existing projects.
 Project-URL: Homepage, https://github.com/yezz123/pagidantic
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: pydantic!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0,>=1.6.2
-Requires-Dist: typing-extensions<4.5.0,>=3.7.4
+Requires-Dist: typing-extensions<4.7.0,>=3.7.4
 Provides-Extra: lint
-Requires-Dist: mypy==0.991; extra == 'lint'
-Requires-Dist: pre-commit==2.21.0; extra == 'lint'
+Requires-Dist: mypy==1.3.0; extra == 'lint'
+Requires-Dist: pre-commit==3.3.2; extra == 'lint'
 Provides-Extra: test
-Requires-Dist: codecov==2.1.12; extra == 'test'
-Requires-Dist: pytest-asyncio==0.20.3; extra == 'test'
-Requires-Dist: pytest-cov==4.0.0; extra == 'test'
-Requires-Dist: pytest==7.2.1; extra == 'test'
+Requires-Dist: pytest-asyncio==0.21.0; extra == 'test'
+Requires-Dist: pytest-cov==4.1.0; extra == 'test'
+Requires-Dist: pytest==7.3.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![Logo](https://raw.githubusercontent.com/yezz123/pagidantic/main/.github/logo.png)
 
 <p align="center">
     <em>Pagination using Pydantic. Easy to use, lightweight, and easy to integrate with existing projects ✨</em>
 </p>
```

