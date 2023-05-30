# Comparing `tmp/torch_exid-0.1.2.tar.gz` & `tmp/torch_exid-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_exid-0.1.2.tar", max compression
+gzip compressed data, was "torch_exid-0.1.3.tar", max compression
```

## Comparing `torch_exid-0.1.2.tar` & `torch_exid-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:57:48.668360 torch_exid-0.1.2/LICENSE
--rw-r--r--   0        0        0     3500 2023-05-30 12:08:05.911047 torch_exid-0.1.2/README.md
--rw-r--r--   0        0        0      472 2023-05-30 12:08:40.040405 torch_exid-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       65 2023-05-30 12:08:30.606940 torch_exid-0.1.2/src/torch_exid/__init__.py
--rw-r--r--   0        0        0     6126 2023-05-30 12:08:24.013256 torch_exid-0.1.2/src/torch_exid/exid.py
--rw-r--r--   0        0        0     4395 2023-05-30 12:09:08.602413 torch_exid-0.1.2/setup.py
--rw-r--r--   0        0        0     4056 2023-05-30 12:09:08.602597 torch_exid-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:57:48.668360 torch_exid-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3500 2023-05-30 12:08:05.911047 torch_exid-0.1.3/README.md
+-rw-r--r--   0        0        0      509 2023-05-30 12:17:28.037382 torch_exid-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-05-30 12:17:04.766262 torch_exid-0.1.3/src/torch_exid/__init__.py
+-rw-r--r--   0        0        0     6126 2023-05-30 12:08:24.013256 torch_exid-0.1.3/src/torch_exid/exid.py
+-rw-r--r--   0        0        0     4395 2023-05-30 12:17:57.047912 torch_exid-0.1.3/setup.py
+-rw-r--r--   0        0        0     4056 2023-05-30 12:17:57.048097 torch_exid-0.1.3/PKG-INFO
```

### Comparing `torch_exid-0.1.2/LICENSE` & `torch_exid-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_exid-0.1.2/README.md` & `torch_exid-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `torch_exid-0.1.2/src/torch_exid/exid.py` & `torch_exid-0.1.3/src/torch_exid/exid.py`

 * *Files identical despite different names*

### Comparing `torch_exid-0.1.2/setup.py` & `torch_exid-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'torch-exid',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'An extension of PyTorch IterableDataset, this package introduces functionalities for shuffling, limiting, and offsetting data.',
     'long_description': '# Extended Iterable Dataset for PyTorch\nAn extension of PyTorch [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset), this package introduces functionalities for shuffling, limiting, and offsetting data.\n\n## Installation\n\nDirectly from [PyPI](https://pypi.org/project/torch_exid/):\n```bash\npip install torch-exid\n```\n\nOr using [Poetry](https://python-poetry.org/):\n```bash\npoetry add torch-exid\n```\n\n## Usage\nBegin by subclassing `ExtendedIterableDataset` and implement the `generator` method to yield items.\n\nHere\'s a simple example using an `IntegersDataset`:\n```python\nfrom torch_exid import ExtendedIterableDataset\n\nclass IntegersDataset(ExtendedIterableDataset):\n    def generator(self) -> Iterator[int]:\n        n = 0\n        while True:\n            yield n\n            n += 1\n\n# Will print out integers 0, 1, ..., 9:\nfor n in IntegersDataset(limit=10):\n    print(n)\n```\n\n## Constructor Parameters\n`ExtendedIterableDataset` introduces several parameters to provide additional control:\n\n### limit: int\nSets the maximum number of data points to return. If negative, all data points are returned. Default is `-1` (return all data).\n```python\n# Will print out "0, 1, 2"\nfor n in IntegersDataset(limit=3)\n    print(n)\n```\n\n### offset: int\nDetermines the number of initial data points to skip. Default is `0`.\n```python\n# Will print out "2, 3, 4"\nfor n in IntegersDataset(limit=3, offset=2)\n    print(n)\n```\n\n### shuffle_buffer: int\nThis specifies the buffer size for shuffling. If greater than `1`, data is buffered and shuffled prior to being returned. If set to `1` (default), no shuffling occurs.\n\n```python\n# Will print out "0, 1, 3, 2" for the first time...\nfor n in IntegersDataset(limit=4, shuffle_buffer=2)\n    print(n)\n\n# ...and 1, 0, 2, 3 second time\nfor n in IntegersDataset(limit=4, shuffle_buffer=2)\n    print(n)\n```\n\n### shuffle_seed: int\nDefines the seed for the random number generator used in shuffling. If not provided, a random seed is used:\n\n```python\n# Will print out "1, 0, 3, 2" both times:\nfor n in IntegersDataset(limit=4, shuffle_buffer=2, shuffle_seed=42)\n    print(n)\n\nfor n in IntegersDataset(limit=4, shuffle_buffer=2, shuffle_seed=42)\n    print(n)\n```\n\n### transforms: List[Callable[[Any], Any]]\nA list of transformations to apply to the data. Default is an empty list.\n```python\nds = IntegersDataset(\n    limit=3,\n    transforms=[\n        lambda n: n + 1,\n        lambda n: n ** 2,\n    ],\n)\n\n# Will print out "1, 4, 9"\nfor n in ds:\n    print(n)\n```\n\nIn addition to the above, any arguments or keyword arguments for the [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) superclass can also be passed.\n\n## Contributing\nContributions are greatly appreciated! Improvement can be made by submitting issues, proposing new features, or submitting pull requests with bug fixes or new functionalities.\n\n### Getting started with contributing\nHere are the steps to get started with development:\n```bash\n# Clone the repository:\ngit clone https://github.com/arlegotin/torch_exid.git\ncd torch_exid\n\n# Install the project and its dependencies using Poetry:\npoetry install\n\n# Spawn a shell within the virtual environment:\npoetry shell\n\n# Run tests to ensure everything is working correctly:\npytest tests/\n```\n\nPlease ensure all changes are accompanied by relevant unit tests, and that all tests pass before submitting a pull request. This helps maintain the quality and reliability of the project.\n',
     'author': 'Artem Legotin',
     'author_email': 'hello@artemlegotin.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `torch_exid-0.1.2/PKG-INFO` & `torch_exid-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-exid
-Version: 0.1.2
+Version: 0.1.3
 Summary: An extension of PyTorch IterableDataset, this package introduces functionalities for shuffling, limiting, and offsetting data.
 Author: Artem Legotin
 Author-email: hello@artemlegotin.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

