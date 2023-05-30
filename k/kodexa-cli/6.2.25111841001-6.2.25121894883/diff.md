# Comparing `tmp/kodexa_cli-6.2.25111841001.tar.gz` & `tmp/kodexa_cli-6.2.25121894883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa_cli-6.2.25111841001.tar", max compression
+gzip compressed data, was "kodexa_cli-6.2.25121894883.tar", max compression
```

## Comparing `kodexa_cli-6.2.25111841001.tar` & `kodexa_cli-6.2.25121894883.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-05-29 12:23:36.528296 kodexa_cli-6.2.25111841001/LICENSE
--rw-r--r--   0        0        0     2707 2023-05-29 12:23:36.528296 kodexa_cli-6.2.25111841001/README.md
--rw-r--r--   0        0        0       64 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/__init__.py
--rw-r--r--   0        0        0    23500 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/cli.py
--rw-r--r--   0        0        0     7641 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/documentation.py
--rw-r--r--   0        0        0      134 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/action.jinja2
--rw-r--r--   0        0        0     1356 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/assistant.jinja2
--rw-r--r--   0        0        0     1021 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/content-taxon.jinja2
--rw-r--r--   0        0        0      328 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/data-store.jinja2
--rw-r--r--   0        0        0      707 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/document-store.jinja2
--rw-r--r--   0        0        0       30 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/extension-pack.jinja2
--rw-r--r--   0        0        0      818 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/header.jinja2
--rw-r--r--   0        0        0      343 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/index.jinja2
--rw-r--r--   0        0        0       30 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/model-runtime.jinja2
--rw-r--r--   0        0        0     2999 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/model.jinja2
--rw-r--r--   0        0        0     1137 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/options.jinja2
--rw-r--r--   0        0        0        0 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/overview.jinja2
--rw-r--r--   0        0        0      922 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/processing-taxon.jinja2
--rw-r--r--   0        0        0       30 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/project-template.jinja2
--rw-r--r--   0        0        0       30 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/store.jinja2
--rw-r--r--   0        0        0      492 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxon.jinja2
--rw-r--r--   0        0        0      273 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxonomy-labels.jinja2
--rw-r--r--   0        0        0      534 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxonomy-structure.jinja2
--rw-r--r--   0        0        0      269 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxonomy.jinja2
--rw-r--r--   0        0        0      780 2023-05-29 12:23:57.812385 kodexa_cli-6.2.25111841001/pyproject.toml
--rw-r--r--   0        0        0     3665 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25111841001/setup.py
--rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25111841001/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 13:09:27.584240 kodexa_cli-6.2.25121894883/LICENSE
+-rw-r--r--   0        0        0     2707 2023-05-30 13:09:27.584240 kodexa_cli-6.2.25121894883/README.md
+-rw-r--r--   0        0        0       64 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/__init__.py
+-rw-r--r--   0        0        0    25219 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/cli.py
+-rw-r--r--   0        0        0     7641 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/documentation.py
+-rw-r--r--   0        0        0      134 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/action.jinja2
+-rw-r--r--   0        0        0     1356 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/assistant.jinja2
+-rw-r--r--   0        0        0     1021 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/content-taxon.jinja2
+-rw-r--r--   0        0        0      328 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/data-store.jinja2
+-rw-r--r--   0        0        0      707 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/document-store.jinja2
+-rw-r--r--   0        0        0       30 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/extension-pack.jinja2
+-rw-r--r--   0        0        0      818 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/header.jinja2
+-rw-r--r--   0        0        0      343 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/index.jinja2
+-rw-r--r--   0        0        0       30 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/model-runtime.jinja2
+-rw-r--r--   0        0        0     2999 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/model.jinja2
+-rw-r--r--   0        0        0     1137 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/options.jinja2
+-rw-r--r--   0        0        0        0 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/overview.jinja2
+-rw-r--r--   0        0        0      922 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/processing-taxon.jinja2
+-rw-r--r--   0        0        0       30 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/project-template.jinja2
+-rw-r--r--   0        0        0       30 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/store.jinja2
+-rw-r--r--   0        0        0      492 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/taxon.jinja2
+-rw-r--r--   0        0        0      273 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/taxonomy-labels.jinja2
+-rw-r--r--   0        0        0      534 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/taxonomy-structure.jinja2
+-rw-r--r--   0        0        0      269 2023-05-30 13:09:27.588240 kodexa_cli-6.2.25121894883/kodexa_cli/templates/taxonomy.jinja2
+-rw-r--r--   0        0        0      780 2023-05-30 13:09:53.464183 kodexa_cli-6.2.25121894883/pyproject.toml
+-rw-r--r--   0        0        0     3665 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25121894883/setup.py
+-rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25121894883/PKG-INFO
```

### Comparing `kodexa_cli-6.2.25111841001/LICENSE` & `kodexa_cli-6.2.25121894883/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/README.md` & `kodexa_cli-6.2.25121894883/README.md`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/cli.py` & `kodexa_cli-6.2.25121894883/kodexa_cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 import logging
 import os
 import os.path
 import sys
 import tarfile
 from getpass import getpass
 from typing import Optional
+from shutil import copyfile
 
 import click
 import wrapt
 import yaml
-from kodexa.platform.client import DEFAULT_COLUMNS
+from kodexa.model import ModelContentMetadata
+from kodexa.platform.client import DEFAULT_COLUMNS, ModelStoreEndpoint
 from rich import print
 
 logging.root.addHandler(logging.StreamHandler(sys.stdout))
 
 from kodexa import KodexaClient
 from kodexa.platform.kodexa import ExtensionHelper, KodexaPlatform
 
@@ -68,14 +70,34 @@
             else:
                 raise Exception('Conflict at %s' % '.'.join(path + [str(key)]))
         else:
             a[key] = b[key]
     return a
 
 
+class MetadataHelper:
+    """ """
+
+    @staticmethod
+    def load_metadata(path) -> dict:
+
+        if os.path.exists(os.path.join(path, 'dharma.json')):
+            dharma_metadata_file = open(os.path.join(path, 'dharma.json'))
+            dharma_metadata = json.loads(dharma_metadata_file.read())
+        elif os.path.exists(os.path.join(path, 'dharma.yml')):
+            dharma_metadata_file = open(os.path.join(path, 'dharma.yml'))
+            dharma_metadata = yaml.safe_load(dharma_metadata_file.read())
+        elif os.path.exists(os.path.join(path, 'kodexa.yml')):
+            dharma_metadata_file = open(os.path.join(path, 'kodexa.yml'))
+            dharma_metadata = yaml.safe_load(dharma_metadata_file.read())
+        else:
+            raise Exception("Unable to find a kodexa.yml file describing your extension")
+        return dharma_metadata
+
+
 # Change the options to below to suit the actual options for your task (or
 # tasks).
 @click.group()
 @click.option("--verbose", "-v", count=True, help="Enable verbose output.")
 @pass_info
 def cli(info: Info, verbose: int):
     # Use the verbosity count to determine the logging level...
@@ -604,37 +626,53 @@
               help='Path to the output folder (defaults to dist under current)')
 @click.option('--version', default=os.getenv('VERSION'), help='Version number (defaults to 1.0.0)')
 @pass_info
 def package(_: Info, path: str, output: str, version: str):
     """
     Package an extension pack based on the kodexa.yml file
     """
-    metadata_obj = ExtensionHelper.load_metadata(path)
+    metadata_obj = MetadataHelper.load_metadata(path)
+
     print("Preparing to pack")
     try:
         os.makedirs(output)
     except OSError as e:
         import errno
         if e.errno != errno.EEXIST:
             raise
 
     metadata_obj['version'] = version if version is not None else '1.0.0'
-
-    if 'source' in metadata_obj and 'location' in metadata_obj['source']:
-        metadata_obj['source']['location'] = metadata_obj['source']['location'].format(**metadata_obj)
-
     versioned_metadata = os.path.join(output, f"{metadata_obj['slug']}-{metadata_obj['version']}.json")
 
-    unversioned_metadata = os.path.join(output, "kodexa.json")
-    with open(versioned_metadata, 'w') as outfile:
-        json.dump(metadata_obj, outfile)
-
-    from shutil import copyfile
-    copyfile(versioned_metadata, unversioned_metadata)
+    def build_json():
+        versioned_metadata = os.path.join(output, f"{metadata_obj['slug']}-{metadata_obj['version']}.json")
+        unversioned_metadata = os.path.join(output, "kodexa.json")
+        with open(versioned_metadata, 'w') as outfile:
+            json.dump(metadata_obj, outfile)
+
+        copyfile(versioned_metadata, unversioned_metadata)
+
+    if 'type' not in metadata_obj:
+        metadata_obj['type'] = 'extensionPack'
+
+    if metadata_obj['type'] == 'extensionPack':
+        if 'source' in metadata_obj and 'location' in metadata_obj['source']:
+            metadata_obj['source']['location'] = metadata_obj['source']['location'].format(**metadata_obj)
+        build_json()
+
+        print("Extension pack has been packaged :tada:")
+
+    elif metadata_obj['type'] == 'STORE' and metadata_obj['storeType'] == 'MODEL':
+        model_content_metadata = ModelContentMetadata.parse_obj(metadata_obj['metadata'])
+        build_json()
+
+        # This will create the training.zip - we will then need to change the filename
+        ModelStoreEndpoint.build_implementation_zip(model_content_metadata)
+        versioned_implementation = os.path.join(output, f"{metadata_obj['slug']}-{metadata_obj['version']}.zip")
+        copyfile('implementation.zip', versioned_implementation)
+
+        # Delete the implementation
+        os.remove('implementation.zip')
+        print("Model has been packaged :tada:")
 
-    output_filename = f"{metadata_obj['slug']}-{metadata_obj['version']}.tar.gz"
-    with tarfile.open(output_filename, "w:gz") as tar:
-        tar.add(output, arcname=os.path.basename(output))
-
-    os.rename(output_filename, os.path.join(output, output_filename))
-
-    print("Extension has been packaged :tada:")
+    else:
+        print("[RED]We don't know how to package this type of metadata[/RED]")
```

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/documentation.py` & `kodexa_cli-6.2.25121894883/kodexa_cli/documentation.py`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/templates/assistant.jinja2` & `kodexa_cli-6.2.25121894883/kodexa_cli/templates/assistant.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/templates/content-taxon.jinja2` & `kodexa_cli-6.2.25121894883/kodexa_cli/templates/content-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/templates/document-store.jinja2` & `kodexa_cli-6.2.25121894883/kodexa_cli/templates/document-store.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/templates/header.jinja2` & `kodexa_cli-6.2.25121894883/kodexa_cli/templates/header.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/templates/model.jinja2` & `kodexa_cli-6.2.25121894883/kodexa_cli/templates/model.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/templates/options.jinja2` & `kodexa_cli-6.2.25121894883/kodexa_cli/templates/options.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/templates/processing-taxon.jinja2` & `kodexa_cli-6.2.25121894883/kodexa_cli/templates/processing-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxonomy-structure.jinja2` & `kodexa_cli-6.2.25121894883/kodexa_cli/templates/taxonomy-structure.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25111841001/pyproject.toml` & `kodexa_cli-6.2.25121894883/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa-cli"
-version = "6.2.25111841001"
+version = "6.2.25121894883"
 description = "Command Line Tools for Kodexa"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>", "John Patrick Sese <jp@kodexa.com>"]
 readme = "README.md"
 packages = [{include = "kodexa_cli"}]
 
 [tool.poetry.scripts]
 kodexa = 'kodexa_cli:cli'
```

### Comparing `kodexa_cli-6.2.25111841001/setup.py` & `kodexa_cli-6.2.25121894883/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'rich==13.3.5']
 
 entry_points = \
 {'console_scripts': ['kodexa = kodexa_cli:cli']}
 
 setup_kwargs = {
     'name': 'kodexa-cli',
-    'version': '6.2.25111841001',
+    'version': '6.2.25121894883',
     'description': 'Command Line Tools for Kodexa',
     'long_description': '# Kodexa Command Line Tools\n\n[![Kodexa CLI Python Package](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml/badge.svg)](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Command Line Tools\n\nThis repository contains the command line tools for Kodexa. The tools are the primary way to interact with Kodexa. It\nallows you to configure components and manage aspects of your Kodexa Platform installation.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch.\nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa_cli-6.2.25111841001/PKG-INFO` & `kodexa_cli-6.2.25121894883/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa-cli
-Version: 6.2.25111841001
+Version: 6.2.25121894883
 Summary: Command Line Tools for Kodexa
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

