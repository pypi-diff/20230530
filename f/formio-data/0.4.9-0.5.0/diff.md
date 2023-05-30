# Comparing `tmp/formio-data-0.4.9.tar.gz` & `tmp/formio-data-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formio-data-0.4.9.tar", max compression
+gzip compressed data, was "formio-data-0.5.0.tar", max compression
```

## Comparing `formio-data-0.4.9.tar` & `formio-data-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2022-06-23 06:15:09.395447 formio-data-0.4.9/LICENSE
--rw-r--r--   0        0        0     5572 2022-07-12 10:29:21.994562 formio-data-0.4.9/README.md
--rw-r--r--   0        0        0      171 2022-06-23 06:15:09.396448 formio-data-0.4.9/formiodata/__init__.py
--rw-r--r--   0        0        0     3483 2022-06-23 06:15:09.396448 formio-data-0.4.9/formiodata/builder.py
--rw-r--r--   0        0        0    35077 2023-01-12 15:57:13.521403 formio-data-0.4.9/formiodata/components.py
--rw-r--r--   0        0        0     4198 2023-01-12 16:10:10.025916 formio-data-0.4.9/formiodata/form.py
--rw-r--r--   0        0        0      979 2022-06-23 06:15:09.396448 formio-data-0.4.9/formiodata/utils.py
--rw-r--r--   0        0        0      541 2023-01-12 15:57:34.426432 formio-data-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     6637 2023-01-12 16:14:46.875304 formio-data-0.4.9/setup.py
--rw-r--r--   0        0        0     6348 2023-01-12 16:14:46.876249 formio-data-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-06-23 06:15:09.395447 formio-data-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5572 2022-07-12 10:29:21.994562 formio-data-0.5.0/README.md
+-rw-r--r--   0        0        0      171 2022-06-23 06:15:09.396448 formio-data-0.5.0/formiodata/__init__.py
+-rw-r--r--   0        0        0     3483 2022-06-23 06:15:09.396448 formio-data-0.5.0/formiodata/builder.py
+-rw-r--r--   0        0        0    35319 2023-05-30 13:46:54.126671 formio-data-0.5.0/formiodata/components.py
+-rw-r--r--   0        0        0     4204 2023-01-13 07:53:22.436294 formio-data-0.5.0/formiodata/form.py
+-rw-r--r--   0        0        0      979 2022-06-23 06:15:09.396448 formio-data-0.5.0/formiodata/utils.py
+-rw-r--r--   0        0        0      541 2023-05-30 13:52:36.684801 formio-data-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6637 2023-05-30 13:53:06.987544 formio-data-0.5.0/setup.py
+-rw-r--r--   0        0        0     6348 2023-05-30 13:53:06.988501 formio-data-0.5.0/PKG-INFO
```

### Comparing `formio-data-0.4.9/LICENSE` & `formio-data-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formio-data-0.4.9/README.md` & `formio-data-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `formio-data-0.4.9/formiodata/builder.py` & `formio-data-0.5.0/formiodata/builder.py`

 * *Files identical despite different names*

### Comparing `formio-data-0.4.9/formiodata/components.py` & `formio-data-0.5.0/formiodata/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,16 @@
     def hidden(self):
         return self.raw.get('hidden')
 
     def _encode_value(self, value):
         return value
 
     def render(self):
-        self.html_component = '<p>%s</p>' % self.value
+        if self.value is not None:
+            self.html_component = '<p>%s</p>' % self.value
 
     @property
     def conditionally_visible(self):
         """
         If conditional visibility applies, evaluate to see if it is visible.
         Note that the component can also be hidden, which is a separate concept.
 
@@ -905,31 +906,31 @@
                     tab['components'].append(component_obj)
 
             self.tabs.append(tab)
 
 
 # Data components
 
-class datagridComponent(Component):
+class baseGridComponent(Component):
 
     class gridRow:
         """Not *really* a component, but it implements the same
         partial interface with input_components and components.
         TODO: Consider if there should be a shared base component for
         this (ComponentOwner?)
         """
-        def __init__(self, datagrid, data):
-            self.datagrid = datagrid
-            self.builder = datagrid.builder
+        def __init__(self, grid, data):
+            self.grid = grid
+            self.builder = grid.builder
             self.input_components = {}
             self.components = OrderedDict()
-            self.form = datagrid.form
+            self.form = grid.form
             self.row = data
             self.html_component = ''
-            datagrid.create_component_objects(self, data)
+            grid.create_component_objects(self, data)
 
         def render(self):
             html_components = []
             for component in self.components.values():
                 if component.is_visible:
                     component.render()
                 else:
@@ -943,15 +944,15 @@
         self.input_components = {}
         self.rows = []
         super().__init__(raw, builder, **kwargs)
         self.form = {'value': []}
 
     def create_component_objects(self, parent, data):
         """This is a weird one, it creates component object for the
-        "blueprint" inside the Builder, with parent = dataGrid, and in
+        "blueprint" inside the Builder, with parent = grid, and in
         a form on each grid row with parent = gridRow
         """
         for component in self.raw.get('components', []):
             # Only determine and load class if component type.
             if 'type' in component:
                 component_obj = parent.builder.get_component_object(component)
                 component_obj.load(component_owner=parent, parent=parent, data=data, all_data=self._all_data)
@@ -991,15 +992,15 @@
             else:
                 label = comp['label']
             labels[comp['key']] = label
         return labels
 
     @property
     def is_form_component(self):
-        # NOTE: A datagrid is not _really_ a form component, but it
+        # NOTE: A grid is not _really_ a form component, but it
         # has a key in the JSON for loading the form, so it acts as
         # such, and it will create an entry in the "input_components"
         # property of its owner.
         return True
 
     @property
     def child_component_owner(self):
@@ -1011,14 +1012,26 @@
 
     def render(self):
         for row in self.rows:
             row.render()
         self.html_component = '<table>'+(''.join([row.html_component for row in self.rows]))+'</table>'
 
 
+class datagridComponent(baseGridComponent):
+    # XXX should we move the initEmpty from base
+    pass
+
+
+class editgridComponent(baseGridComponent):
+
+    @property
+    def initEmpty(self):
+        return self.raw.get('openWhenEmpty')
+
+
 # Premium components
 
 class fileComponent(Component):
 
     def __init__(self, raw, builder, **kwargs):
         super().__init__(raw, builder, **kwargs)
```

### Comparing `formio-data-0.4.9/formiodata/form.py` & `formio-data-0.5.0/formiodata/form.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,17 +69,19 @@
         return self._input
 
     @property
     def data(self):
         logging.warning('DEPRECATION WARNING: data attr/property shall be deleted in a future version.')
         return self._data
 
-    def get_component_from_path(self, component_path):
+    def get_component_by_path(self, component_path):
         """
-        Get component object from path (provided by the Formio.js JS/API)
+        Get component object by path
+
+        (Eg provided by the Formio.js JS/API).
         Especially handy for data Components eg datagridComponent.
 
         Example path:
         dataGrid[0].lastname => lastname in the first row [0] of a datagrid
 
         # Example path_nodes:
         # dataGrid[0].lastname => ['dataGrid[0]', 'lastname']
@@ -88,15 +90,15 @@
         @return component: a Component object
         """
         path_nodes = component_path.split('.')
         # Example path_nodes:
         # dataGrid[0].lastname => ['dataGrid[0]', 'lastname']
         components = self.input_components
         for path_node in path_nodes:
-            # get the component_owner eg row in datagrid
+            # eg: regex search '[0]' in 'dataGrid[0]'
             m = re.search(r"\[([A-Za-z0-9_]+)\]", path_node)
             if m:
                 idx_notation = m.group(0)  # eg: '[0]', '[1]', etc
                 idx = int(m.group(1))  # eg: 0, 1, etc
                 key = path_node.replace(idx_notation, '')
                 component = components[key]
                 if hasattr(component, 'rows'):
```

### Comparing `formio-data-0.4.9/formiodata/utils.py` & `formio-data-0.5.0/formiodata/utils.py`

 * *Files identical despite different names*

### Comparing `formio-data-0.4.9/pyproject.toml` & `formio-data-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formio-data"
-version = "0.4.9"
+version = "0.5.0"
 homepage = "https://github.com/novacode-nl/python-formio-data"
 description = "formio.js JSON-data API"
 readme = "README.md"
 authors = ["Bob Leers <bob@novacode.nl>"]
 license = "MIT"
 packages = [ { include = "formiodata/**/*.py" } ]
 exclude = ["tests/*"]
```

### Comparing `formio-data-0.4.9/setup.py` & `formio-data-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 extras_require = \
 {':python_version <= "3.6"': ['python-dateutil>=2.8.2,<3.0.0'],
  'json_logic': ['json_logic_qubit>=0.9.1,<0.10.0']}
 
 setup_kwargs = {
     'name': 'formio-data',
-    'version': '0.4.9',
+    'version': '0.5.0',
     'description': 'formio.js JSON-data API',
     'long_description': '# formio-data (Python)\n\nformio.js (JSON Form Builder) data API for Python.\n\nFor information about the formio.js project, see https://github.com/formio/formio.js\n\n## Introduction\n\n**python-formio-data** is a Python package, which loads and transforms\nformio.js **Builder JSON** and **Form JSON** into **usable Python objects**.  It\'s main\naim is to provide easy access to a Form its components/fields, also\ncaptured as **Python objects**, which makes this API very versatile and usable.\n\n**Notes about terms:**\n  - **Builder:** The Form Builder which is the design/blueprint of a Form.\n  - **Form:** A filled-in Form, aka Form submission.\n  - **Component:** Input (field) or layout component in the Form Builder and Form.\n\n## Features\n\n  - Compatible with Python 3.6 and later\n  - Constructor of the **Builder** and **Form** class, only requires\n    the JSON and an optional language code for translations.\n  - Get a Form object its Components as a usable object e.g. datetime, boolean, dict (for select component) etc.\n  - Open source (MIT License)\n\n## Installation\n\nThe source code is currently hosted on GitHub at:\nhttps://github.com/novacode-nl/python-formio-data\n\n### PyPI - Python Package Index\n\nBinary installers for the latest released version are available at the [Python\nPackage Index](https://pypi.python.org/pypi/formio-data)\n\n```sh\npip(3) install formio-data\n```\n\n#### Optional dependencies\n\nTo support conditional visibility using JSON logic, you can install\nthe `json-logic-qubit` package (the `json-logic` package it is forked\noff of is currently unmaintained).  It\'s also possible to install it\nvia the pip feature `json_logic` like so:\n\n```sh\npip(3) install -U formio-data[json_logic]\n```\n\n### Source Install with Poetry (recommended)\n\nConvenient for developers. Also useful for running the (unit)tests.\n\n```sh\ngit clone git@github.com:novacode-nl/python-formio-data.git\npoetry install\n```\n\n#### Optional dependencies\n\nWhen working in the project itself, use\n\n```sh\npoetry install -E json_logic\n```\n\n### Source Install with pip\n\nOptional dependencies need to be installed separately.\n\n```sh\npip(3) install -U -e python-formio-data\n```\n\n## Using direnv\n\nYou can use [nixpkgs](https://nixos.org/) to run a self-contained\nPython environment without any additional setup.  Once you\'ve\ninstalled nixpkgs, switch into the directory and type "nix-shell" to\nget a shell from which the correct Python with packages is available.\n\nIf you\'re using [direnv](https://direnv.net/), use `direnv allow`\nafter changing into the project directory and you\'re good to go.  Also\nconsider [nix-direnv](https://github.com/nix-community/nix-direnv) to\nspeed up the experience (it can re-use a cached local installation).\n\n## License\n[MIT](LICENSE)\n\n## Contributing\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.\n\n## Usage examples\n\nFor more examples of usage, see the unit-tests.\n\n``` python\n>> from formiodata import Builder, Form\n>>\n# builder_json is a formio.js Builder JSON document (text/string)\n# form_json is a formio.js Form JSON document (text/string)\n>>\n>> builder = Builder(builder_json)\n>> form = Form(builder, form_json)\n\n##################\n# input components\n##################\n\n# textfield label\n>> print(form.input_components[\'firstname\'].label)\n\'First Name\'\n\n# textfield value\n>> print(form.input_components[\'firstname\'].value)\n\'Bob\'\n\n# datetime label\n>> print(form.input_components[\'birthday\'].label)\n\'Birthday\'\n\n# datetime value\n>> print(form.input_components[\'birthday\'].value)\ndatetime.date(2009 10 16)\n\n# datagrid (rows property)\n>> print(form.input_components[\'datagridMeasurements\'].rows)\n[\n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}, \n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}\n]\n\n>> for row in form.input_components[\'datagridMeasurements\'].rows:\n>>    dtime = row[\'measurementDatetime\']\n>>    fahrenheit = row[\'measurementFahrenheit\']\n>>    print(%s: %s, %s: %s\' % (dt.label, dt.value, fahrenheit.label, fahrenheit.value))\n\nDatetime: datetime.datetime(2021, 5, 8, 11, 39, 0, 296487), Fahrenheit: 122\nDatetime: datetime.datetime(2021, 5, 8, 11, 41, 5, 919943), Fahrenheit: 131\n\n# alternative example, by getattr\n>> print(form.data.firstname.label)\n\'First Name\'\n\n>> print(form.data.firstname.value)\n\'Bob\'\n\n#################################\n# components (layout, input etc.)\n#################################\n\n# columns\n>> print(form.components[\'addressColumns\'])\n<columnsComponent>\n\n>> print(form.components[\'addressColumns\'].rows)\n[ \n  {\'firstName\': <textfieldComponent>, \'lastName: <textfieldComponent>}, \n  {\'email\': <emailComponent>, \'companyName: <textfieldComponent>}\n]\n```\n\n## Unit tests\n\n**Note:**\n\nInternet access is recommended for running the `filecStorageUrlComponentTestCase`, because this also tests the URL Storage (type).\\\nIf no internet access, this test won\'t fail and a WARNING shall be logged regarding a ConnectionError.\n\n### Run all unittests\n\nFrom toplevel directory:\n\n```\npoetry install -E json_logic  # if you haven\'t already\npoetry run python -m unittest\n```\n\n### Run component unittests\n\nAll Components, from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_component_*.py\n```\n\nNested components (complexity), from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_nested_components.py\n```\n\n### Run specific component unittest\n\n```\npoetry run python -m unittest tests.test_component_day.dayComponentTestCase.test_get_form_dayMonthYear\n```\n',
     'author': 'Bob Leers',
     'author_email': 'bob@novacode.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/novacode-nl/python-formio-data',
```

### Comparing `formio-data-0.4.9/PKG-INFO` & `formio-data-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formio-data
-Version: 0.4.9
+Version: 0.5.0
 Summary: formio.js JSON-data API
 Home-page: https://github.com/novacode-nl/python-formio-data
 License: MIT
 Author: Bob Leers
 Author-email: bob@novacode.nl
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

