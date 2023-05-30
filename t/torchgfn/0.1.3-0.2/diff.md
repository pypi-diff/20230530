# Comparing `tmp/torchgfn-0.1.3.tar.gz` & `tmp/torchgfn-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchgfn-0.1.3.tar", max compression
+gzip compressed data, was "torchgfn-0.2.tar", max compression
```

## Comparing `torchgfn-0.1.3.tar` & `torchgfn-0.2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0    14216 2023-05-23 22:16:40.320592 torchgfn-0.1.3/README.md
--rw-r--r--   0        0        0     3017 2023-05-23 22:46:07.195189 torchgfn-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      144 2023-05-23 21:43:33.680879 torchgfn-0.1.3/src/gfn/__init__.py
--rw-r--r--   0        0        0      103 2023-05-23 21:43:33.681872 torchgfn-0.1.3/src/gfn/containers/__init__.py
--rw-r--r--   0        0        0     2153 2023-05-23 21:43:33.682462 torchgfn-0.1.3/src/gfn/containers/base.py
--rw-r--r--   0        0        0     3584 2023-05-23 21:43:33.683072 torchgfn-0.1.3/src/gfn/containers/replay_buffer.py
--rw-r--r--   0        0        0    13197 2023-05-23 21:43:33.683961 torchgfn-0.1.3/src/gfn/containers/states.py
--rw-r--r--   0        0        0    11797 2023-05-23 21:43:33.684612 torchgfn-0.1.3/src/gfn/containers/trajectories.py
--rw-r--r--   0        0        0     7389 2023-05-23 21:43:33.685009 torchgfn-0.1.3/src/gfn/containers/transitions.py
--rw-r--r--   0        0        0     3593 2023-05-23 21:43:33.685389 torchgfn-0.1.3/src/gfn/distributions.py
--rw-r--r--   0        0        0       95 2023-05-23 21:43:33.685659 torchgfn-0.1.3/src/gfn/envs/__init__.py
--rw-r--r--   0        0        0     7424 2023-05-23 21:43:33.685892 torchgfn-0.1.3/src/gfn/envs/discrete_ebm.py
--rw-r--r--   0        0        0     8212 2023-05-23 21:43:33.686097 torchgfn-0.1.3/src/gfn/envs/env.py
--rw-r--r--   0        0        0     8634 2023-05-23 21:43:33.686287 torchgfn-0.1.3/src/gfn/envs/hypergrid.py
--rw-r--r--   0        0        0      125 2023-05-23 21:43:33.686564 torchgfn-0.1.3/src/gfn/envs/preprocessors/__init__.py
--rw-r--r--   0        0        0     1852 2023-05-23 21:43:33.686741 torchgfn-0.1.3/src/gfn/envs/preprocessors/base.py
--rw-r--r--   0        0        0     2268 2023-05-23 21:43:33.687020 torchgfn-0.1.3/src/gfn/envs/preprocessors/hot.py
--rw-r--r--   0        0        0     6545 2023-05-23 21:43:33.687254 torchgfn-0.1.3/src/gfn/estimators.py
--rw-r--r--   0        0        0      481 2023-05-23 21:43:33.687485 torchgfn-0.1.3/src/gfn/losses/__init__.py
--rw-r--r--   0        0        0     9125 2023-05-23 21:43:33.687692 torchgfn-0.1.3/src/gfn/losses/base.py
--rw-r--r--   0        0        0     6150 2023-05-23 21:43:33.687915 torchgfn-0.1.3/src/gfn/losses/detailed_balance.py
--rw-r--r--   0        0        0     4939 2023-05-23 21:43:33.688099 torchgfn-0.1.3/src/gfn/losses/flow_matching.py
--rw-r--r--   0        0        0    14025 2023-05-23 21:43:33.688347 torchgfn-0.1.3/src/gfn/losses/sub_trajectory_balance.py
--rw-r--r--   0        0        0     3703 2023-05-23 21:43:33.688679 torchgfn-0.1.3/src/gfn/losses/trajectory_balance.py
--rw-r--r--   0        0        0     5330 2023-05-23 21:43:33.689127 torchgfn-0.1.3/src/gfn/modules.py
--rw-r--r--   0        0        0      172 2023-05-23 21:43:33.689466 torchgfn-0.1.3/src/gfn/samplers/__init__.py
--rw-r--r--   0        0        0     5479 2023-05-23 21:43:33.689714 torchgfn-0.1.3/src/gfn/samplers/actions_samplers.py
--rw-r--r--   0        0        0     4705 2023-05-23 21:43:33.690029 torchgfn-0.1.3/src/gfn/samplers/trajectories_sampler.py
--rw-r--r--   0        0        0     3383 2023-05-23 21:43:33.690578 torchgfn-0.1.3/src/gfn/utils.py
--rw-r--r--   0        0        0    15679 1970-01-01 00:00:00.000000 torchgfn-0.1.3/setup.py
--rw-r--r--   0        0        0    15542 1970-01-01 00:00:00.000000 torchgfn-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    14346 2023-05-30 14:17:28.832385 torchgfn-0.2/README.md
+-rw-r--r--   0        0        0     3204 2023-05-30 14:17:28.832830 torchgfn-0.2/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-05-30 14:25:24.260364 torchgfn-0.2/src/gfn/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-30 14:17:27.272751 torchgfn-0.2/src/gfn/containers/__init__.py
+-rw-r--r--   0        0        0     2153 2023-05-03 09:42:02.656970 torchgfn-0.2/src/gfn/containers/base.py
+-rw-r--r--   0        0        0     3584 2023-05-30 14:17:27.272875 torchgfn-0.2/src/gfn/containers/replay_buffer.py
+-rw-r--r--   0        0        0    13197 2023-05-30 14:17:27.272991 torchgfn-0.2/src/gfn/containers/states.py
+-rw-r--r--   0        0        0    11797 2023-05-30 14:17:27.273148 torchgfn-0.2/src/gfn/containers/trajectories.py
+-rw-r--r--   0        0        0     7389 2023-05-30 14:17:27.273305 torchgfn-0.2/src/gfn/containers/transitions.py
+-rw-r--r--   0        0        0     3593 2023-05-30 14:17:27.273426 torchgfn-0.2/src/gfn/distributions.py
+-rw-r--r--   0        0        0       95 2023-05-30 14:17:27.273545 torchgfn-0.2/src/gfn/envs/__init__.py
+-rw-r--r--   0        0        0     7424 2023-05-30 14:17:27.273669 torchgfn-0.2/src/gfn/envs/discrete_ebm.py
+-rw-r--r--   0        0        0     8212 2023-05-30 14:17:27.273791 torchgfn-0.2/src/gfn/envs/env.py
+-rw-r--r--   0        0        0     8634 2023-05-30 14:17:27.274056 torchgfn-0.2/src/gfn/envs/hypergrid.py
+-rw-r--r--   0        0        0      125 2022-11-08 17:34:55.632486 torchgfn-0.2/src/gfn/envs/preprocessors/__init__.py
+-rw-r--r--   0        0        0     1852 2023-05-30 14:17:27.274298 torchgfn-0.2/src/gfn/envs/preprocessors/base.py
+-rw-r--r--   0        0        0     2268 2023-05-30 14:17:27.274443 torchgfn-0.2/src/gfn/envs/preprocessors/hot.py
+-rw-r--r--   0        0        0     6545 2023-05-30 14:17:27.274599 torchgfn-0.2/src/gfn/estimators.py
+-rw-r--r--   0        0        0      481 2023-04-28 10:00:41.421203 torchgfn-0.2/src/gfn/losses/__init__.py
+-rw-r--r--   0        0        0     9125 2023-05-30 14:17:27.274753 torchgfn-0.2/src/gfn/losses/base.py
+-rw-r--r--   0        0        0     6150 2023-05-30 14:17:27.274902 torchgfn-0.2/src/gfn/losses/detailed_balance.py
+-rw-r--r--   0        0        0     4939 2023-05-30 14:17:27.275035 torchgfn-0.2/src/gfn/losses/flow_matching.py
+-rw-r--r--   0        0        0    14025 2023-05-30 14:17:27.275192 torchgfn-0.2/src/gfn/losses/sub_trajectory_balance.py
+-rw-r--r--   0        0        0     3703 2023-05-30 14:17:27.275333 torchgfn-0.2/src/gfn/losses/trajectory_balance.py
+-rw-r--r--   0        0        0     5330 2023-05-30 14:17:27.275429 torchgfn-0.2/src/gfn/modules.py
+-rw-r--r--   0        0        0      172 2023-05-30 14:17:27.275544 torchgfn-0.2/src/gfn/samplers/__init__.py
+-rw-r--r--   0        0        0     5479 2023-05-30 14:17:27.275690 torchgfn-0.2/src/gfn/samplers/actions_samplers.py
+-rw-r--r--   0        0        0     4705 2023-05-30 14:17:27.275816 torchgfn-0.2/src/gfn/samplers/trajectories_sampler.py
+-rw-r--r--   0        0        0     3383 2023-05-30 14:17:27.275897 torchgfn-0.2/src/gfn/utils.py
+-rw-r--r--   0        0        0    15889 1970-01-01 00:00:00.000000 torchgfn-0.2/PKG-INFO
```

### Comparing `torchgfn-0.1.3/README.md` & `torchgfn-0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,40 +19,48 @@
 
 
 
 ## Installing the packages
 
 The codebase requires python >= 3.10
 
+To install the latest stable version:
+
+```bash
+pip install torchgfn
+```
+
+Optionally, to run scripts:
+
+```bash
+pip install torchgfn[scripts]
+```
+
+To install the cutting edge version (from the `main` branch):
+
 ```bash
 git clone https://github.com/saleml/gfn.git
-conda create -n gfn python=3.10
+conda create -n gfn python=3.11
 conda activate gfn
 cd gfn
 pip install .
 ```
 
-Optionally, to run scripts, and for [wandb](https://wandb.ai) logging
-
-```bash
-pip install .[scripts]
-wandb login
-```
 
 ## About this repo
 
 This repo serves the purpose of fast prototyping [GFlowNet](https://arxiv.org/abs/2111.09266) related algorithms. It decouples the environment definition, the sampling process, and the parametrization used for the GFN loss.
 
 An example script is provided [here](https://github.com/saleml/gfn/blob/master/scripts/train.py). To run the code, use one of the following:
 
 ```bash
-python train.py --env HyperGrid --env.ndim 4 --env.height 8 --n_iterations 100000 --loss TB
-python train.py --env DiscreteEBM --env.ndim 4 --env.alpha 0.5 --n_iterations 10000 --batch_size 64 --temperature 2.
-python train.py --env HyperGrid --env.ndim 2 --env.height 64 --n_iterations 100000 --loss DB --replay_buffer_size 1000 --logit_PB.module_name Uniform --optim sgd --optim.lr 5e-3
-python train.py --env HyperGrid --env.ndim 4 --env.height 8 --env.R0 0.01 --loss FM --optim adam --optim.lr 1e-4
+python train.py --env hypergrid --env.ndim 4 --env.height 8 --n_iterations 100000 --loss trajectory-balance
+python train.py --env discrete-ebm --env.ndim 4 --env.alpha 0.5 --n_iterations 10000 --batch_size 64 --sampler.temperature 2.
+python train.py --env hypergrid --env.ndim 2 --env.height 64 --n_iterations 100000 --loss detailed-balance --logit_PB.module_name Uniform --optim adam --optim.lr 1e-3 --batch_size 64
+python train.py --env hypergrid --env.ndim 4 --env.height 8 --env.R0 0.01 --loss flowmatching --optim adam --optim.lr 1e-4
 ```
 
 ### Example, in a few lines
 
 (⬇️ This example require the [`tqdm`](https://github.com/tqdm/tqdm) package to run. `pip install tqdm` or install all extra requirements with `pip install .[scripts]`)
 
 ```python
```

### Comparing `torchgfn-0.1.3/pyproject.toml` & `torchgfn-0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "torchgfn"
 packages = [{include = "gfn", from = "src"}]
-version = "0.1.3"
-description = "A torch inplementation of GFlowNets"
+version = "0.2"
+description = "A torch implementation of GFlowNets"
 authors = ["Salem Lahou <salemlahlou9@gmail.com>", "Joseph Viviano <joseph@viviano.ca>", "Victor Schmidt <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -51,14 +51,15 @@
     "sphinx-math-dollar",
     "sphinx",
     "tox",
     "black",
     "myst-parser"
 ]
 scripts = ["tqdm", "wandb", "simple-parsing"]
+all = ["pre-commit", "pytest", "renku-sphinx-theme", "sphinx_rtd_theme", "sphinx-autoapi", "sphinx-math-dollar", "sphinx", "tox", "black", "myst-parser", "tqdm", "wandb", "simple-parsing"]
 
 [project.urls]
 "Homepage" = "https://gfn.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/saleml/gfn/issues"
 
 
 # TODO: Could use for examples? Or something else?
```

### Comparing `torchgfn-0.1.3/src/gfn/containers/base.py` & `torchgfn-0.2/src/gfn/containers/base.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/containers/replay_buffer.py` & `torchgfn-0.2/src/gfn/containers/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/containers/states.py` & `torchgfn-0.2/src/gfn/containers/states.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/containers/trajectories.py` & `torchgfn-0.2/src/gfn/containers/trajectories.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/containers/transitions.py` & `torchgfn-0.2/src/gfn/containers/transitions.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/distributions.py` & `torchgfn-0.2/src/gfn/distributions.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/envs/discrete_ebm.py` & `torchgfn-0.2/src/gfn/envs/discrete_ebm.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/envs/env.py` & `torchgfn-0.2/src/gfn/envs/env.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/envs/hypergrid.py` & `torchgfn-0.2/src/gfn/envs/hypergrid.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/envs/preprocessors/base.py` & `torchgfn-0.2/src/gfn/envs/preprocessors/base.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/envs/preprocessors/hot.py` & `torchgfn-0.2/src/gfn/envs/preprocessors/hot.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/estimators.py` & `torchgfn-0.2/src/gfn/estimators.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/losses/base.py` & `torchgfn-0.2/src/gfn/losses/base.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/losses/detailed_balance.py` & `torchgfn-0.2/src/gfn/losses/detailed_balance.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/losses/flow_matching.py` & `torchgfn-0.2/src/gfn/losses/flow_matching.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/losses/sub_trajectory_balance.py` & `torchgfn-0.2/src/gfn/losses/sub_trajectory_balance.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/losses/trajectory_balance.py` & `torchgfn-0.2/src/gfn/losses/trajectory_balance.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/modules.py` & `torchgfn-0.2/src/gfn/modules.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/samplers/actions_samplers.py` & `torchgfn-0.2/src/gfn/samplers/actions_samplers.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/samplers/trajectories_sampler.py` & `torchgfn-0.2/src/gfn/samplers/trajectories_sampler.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/src/gfn/utils.py` & `torchgfn-0.2/src/gfn/utils.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.3/setup.py` & `torchgfn-0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,244 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: torchgfn
+Version: 0.2
+Summary: A torch implementation of GFlowNets
+License: MIT
+Author: Salem Lahou
+Author-email: salemlahlou9@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: dev
+Provides-Extra: scripts
+Requires-Dist: black (==22.3.0) ; extra == "dev" or extra == "all"
+Requires-Dist: einops (>=0.6.1)
+Requires-Dist: gymnasium (>=0.28.1)
+Requires-Dist: myst-parser ; extra == "dev" or extra == "all"
+Requires-Dist: numpy (>=1.21.2)
+Requires-Dist: pre-commit ; extra == "dev" or extra == "all"
+Requires-Dist: pytest ; extra == "dev" or extra == "all"
+Requires-Dist: renku-sphinx-theme ; extra == "dev" or extra == "all"
+Requires-Dist: simple-parsing (==0.0.20) ; extra == "scripts" or extra == "all"
+Requires-Dist: sphinx ; extra == "dev" or extra == "all"
+Requires-Dist: sphinx-autoapi ; extra == "dev" or extra == "all"
+Requires-Dist: sphinx-math-dollar ; extra == "dev" or extra == "all"
+Requires-Dist: sphinx_rtd_theme ; extra == "dev" or extra == "all"
+Requires-Dist: torch (>=1.9.0)
+Requires-Dist: torchtyping (>=0.1.4)
+Requires-Dist: tox ; extra == "dev" or extra == "all"
+Requires-Dist: tqdm ; extra == "scripts" or extra == "all"
+Requires-Dist: wandb ; extra == "scripts" or extra == "all"
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+<p align="center">
+    <a>
+	    <img src='https://img.shields.io/badge/python-3.10%2B-blueviolet' alt='Python' />
+	</a>
+	<a href='https://gfn.readthedocs.io/en/latest/?badge=latest'>
+    	<img src='https://readthedocs.org/projects/gfn/badge/?version=latest' alt='Documentation Status' />
+	</a>
+    <a>
+	    <img src='https://img.shields.io/badge/code%20style-black-black' />
+	</a>
+</p>
 
-packages = \
-['gfn',
- 'gfn.containers',
- 'gfn.envs',
- 'gfn.envs.preprocessors',
- 'gfn.losses',
- 'gfn.samplers']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['einops>=0.6.1',
- 'gymnasium>=0.28.1',
- 'numpy>=1.21.2',
- 'torch>=1.9.0',
- 'torchtyping>=0.1.4']
-
-extras_require = \
-{'dev': ['pre-commit',
-         'pytest',
-         'renku-sphinx-theme',
-         'sphinx_rtd_theme',
-         'sphinx-autoapi',
-         'sphinx-math-dollar',
-         'sphinx',
-         'tox',
-         'black==22.3.0',
-         'myst-parser'],
- 'scripts': ['tqdm', 'wandb', 'simple-parsing==0.0.20']}
-
-setup_kwargs = {
-    'name': 'torchgfn',
-    'version': '0.1.3',
-    'description': 'A torch inplementation of GFlowNets',
-    'long_description': '<p align="center">\n    <a>\n\t    <img src=\'https://img.shields.io/badge/python-3.10%2B-blueviolet\' alt=\'Python\' />\n\t</a>\n\t<a href=\'https://gfn.readthedocs.io/en/latest/?badge=latest\'>\n    \t<img src=\'https://readthedocs.org/projects/gfn/badge/?version=latest\' alt=\'Documentation Status\' />\n\t</a>\n    <a>\n\t    <img src=\'https://img.shields.io/badge/code%20style-black-black\' />\n\t</a>\n</p>\n\n</p>\n<p align="center">\n  <a href="https://gfn.readthedocs.io/en/latest/">Documentation</a> ~ <a href="https://github.com/saleml/gfn">Code</a>\n</p>\n\n# gfn: a Python package for GFlowNets\n\n\n\n## Installing the packages\n\nThe codebase requires python >= 3.10\n\n```bash\ngit clone https://github.com/saleml/gfn.git\nconda create -n gfn python=3.10\nconda activate gfn\ncd gfn\npip install .\n```\n\nOptionally, to run scripts, and for [wandb](https://wandb.ai) logging\n\n```bash\npip install .[scripts]\nwandb login\n```\n\n## About this repo\n\nThis repo serves the purpose of fast prototyping [GFlowNet](https://arxiv.org/abs/2111.09266) related algorithms. It decouples the environment definition, the sampling process, and the parametrization used for the GFN loss.\n\nAn example script is provided [here](https://github.com/saleml/gfn/blob/master/scripts/train.py). To run the code, use one of the following:\n\n```bash\npython train.py --env HyperGrid --env.ndim 4 --env.height 8 --n_iterations 100000 --loss TB\npython train.py --env DiscreteEBM --env.ndim 4 --env.alpha 0.5 --n_iterations 10000 --batch_size 64 --temperature 2.\npython train.py --env HyperGrid --env.ndim 2 --env.height 64 --n_iterations 100000 --loss DB --replay_buffer_size 1000 --logit_PB.module_name Uniform --optim sgd --optim.lr 5e-3\npython train.py --env HyperGrid --env.ndim 4 --env.height 8 --env.R0 0.01 --loss FM --optim adam --optim.lr 1e-4\n```\n\n### Example, in a few lines\n\n(⬇️ This example require the [`tqdm`](https://github.com/tqdm/tqdm) package to run. `pip install tqdm` or install all extra requirements with `pip install .[scripts]`)\n\n```python\nimport torch\nfrom tqdm import tqdm\n\nfrom gfn import LogitPBEstimator, LogitPFEstimator, LogZEstimator\nfrom gfn.envs import HyperGrid\nfrom gfn.losses import TBParametrization, TrajectoryBalance\nfrom gfn.samplers import DiscreteActionsSampler, TrajectoriesSampler\n\nif __name__ == "__main__":\n\n    env = HyperGrid(ndim=4, height=8, R0=0.01)  # Grid of size 8x8x8x8\n\n    logit_PF = LogitPFEstimator(env=env, module_name="NeuralNet")\n    logit_PB = LogitPBEstimator(\n        env=env,\n        module_name="NeuralNet",\n        torso=logit_PF.module.torso,  # To share parameters between PF and PB\n    )\n    logZ = LogZEstimator(torch.tensor(0.0))\n\n    parametrization = TBParametrization(logit_PF, logit_PB, logZ)\n\n    actions_sampler = DiscreteActionsSampler(estimator=logit_PF)\n    trajectories_sampler = TrajectoriesSampler(env=env, actions_sampler=actions_sampler)\n\n    loss_fn = TrajectoryBalance(parametrization=parametrization)\n\n    params = [\n        {\n            "params": [\n                val for key, val in parametrization.parameters.items() if "logZ" not in key\n            ],\n            "lr": 0.001,\n        },\n        {"params": [val for key, val in parametrization.parameters.items() if "logZ" in key], "lr": 0.1},\n    ]\n    optimizer = torch.optim.Adam(params)\n\n    for i in (pbar := tqdm(range(1000))):\n        trajectories = trajectories_sampler.sample(n_trajectories=16)\n        optimizer.zero_grad()\n        loss = loss_fn(trajectories)\n        loss.backward()\n        optimizer.step()\n        if i % 25 == 0:\n            pbar.set_postfix({"loss": loss.item()})\n\n```\n\n## Contributing\n\nBefore the first commit:\n\n```bash\npip install .[dev]\npre-commit install\npre-commit run --all-files\n```\n\nRun `pre-commit` after staging, and before committing. Make sure all the tests pass (By running `pytest`).\nThe codebase uses `black` formatter.\n\nTo make the docs locally:\n```bash\ncd docs\nmake html\nopen build/html/index.html\n```\n\n## Details about the codebase\n\n### Defining an environment\n\nA pointed DAG environment (or GFN environment, or environment for short) is a representation for the pointed DAG. The abstract class [Env](https://github.com/saleml/gfn/blob/master/src/gfn/envs/env.py) specifies the requirements for a valid environment definition. To obtain such a representation, the environment needs to specify the following attributes, properties, or methods:\n\n- The `action_space`. Which should be a `gymnasium.spaces.Discrete` object for discrete environments. The last action should correspond to the exit action.\n- The initial state `s_0`, as a `torch.Tensor` of arbitrary dimension.\n- (Optional) The sink state `s_f`, as a `torch.Tensor` of the same shape as `s_0`, used to represent complete trajectories only (within a batch of trajectories of different lengths), and never processed by any model. If not specified, it is set to `torch.full_like(s_0, -float(\'inf\'))`.\n- The method `make_States_class` that creates a subclass of [States](https://github.com/saleml/gfn/blob/master/src/gfn/containers/states.py). The instances of the resulting class should represent a batch of states of arbitrary shape, which is useful to define a trajectory, or a batch of trajectories. `s_0` and `s_f`, along with a tuple called `state_shape` should be defined as class variables, and the subclass (of `States`) should implement masking methods, that specify which actions are possible, in a discrete environment.\n- The methods `maskless_step` and `maskless_backward_step` that specify how an action changes a state (going forward and backward). These functions do not need to handle masking, checking whether actions are allowed, checking whether a state is the sink state, etc... These checks are handled in `Env.step` and `Env.backward_step`\n- The `log_reward` function that assigns a nonnegative reward to every terminating state (i.e. state with all $s_f$ as a child in the DAG). If `log_reward` is not implemented, `reward` needs to be.\n\nIf the states (as represented in the `States` class) need to be transformed to another format before being processed (by neural networks for example), then the environment should define a `preprocessor` attribute, which should be an instance of the [base preprocessor class](https://github.com/saleml/gfn/blob/master/src/gfn/envs/preprocessors/base.py). If no preprocessor is defined, the states are used as is (actually transformed using  [`IdentityPreprocessor`](https://github.com/saleml/gfn/blob/master/src/gfn/envs/preprocessors/base.py), which transforms the state tensors to `FloatTensor`s). Implementing your own preprocessor requires defining the `preprocess` function, and the `output_shape` attribute, which is a tuple representing the shape of *one* preprocessed state.\n\nOptionally, you can define a static `get_states_indices` method that assigns a unique integer number to each state if the environment allows it, and a `n_states` property that returns an integer representing the number of states (excluding $s_f$) in the environment. `get_terminating_states_indices` can also be implemented and serves the purpose of uniquely identifying terminating states of the environment.\n\nFor more details, take a look at [HyperGrid](https://github.com/saleml/gfn/blob/master/src/gfn/envs/hypergrid.py), an environment where all states are terminating states, or at [DiscreteEBM](https://github.com/saleml/gfn/blob/master/src/gfn/envs/discrete_ebm.py), where all trajectories are of the same length but only some states are terminating.\n\n### Other containers\n\nBesides the `States` class, other containers of states are available:\n\n- [Transitions](https://github.com/saleml/gfn/blob/master/src/gfn/containers/transitions.py), representing a batch of transitions $s \\rightarrow s\'$.\n- [Trajectories](https://github.com/saleml/gfn/blob/master/src/gfn/containers/trajectories.py), representing a batch of complete trajectories $\\tau = s_0 \\rightarrow s_1 \\rightarrow \\dots \\rightarrow s_n \\rightarrow s_f$.\n\nThese containers can either be instantiated using a `States` object, or can be initialized as empty containers that can be populated on the fly, allowing the usage of [ReplayBuffer](https://github.com/saleml/gfn/blob/master/src/gfn/containers/replay_buffer.py)s.\n\nThey inherit from the base `Container` [class](https://github.com/saleml/gfn/blob/master/src/gfn/containers/base.py), indicating some helpful methods.\n\nIn most cases, one needs to sample complete trajectories. From a batch of trajectories, a batch of states and batch of transitions can be defined using `Trajectories.to_transitions()` and `Trajectories.to_states()`. These exclude meaningless transitions and states that were added to the batch of trajectories to allow for efficient batching.\n\n### Estimators and Modules\n\nTraining GFlowNets requires one or multiple estimators. As of now, only discrete environments are handled. All estimators are subclasses of [FunctionEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py), implementing a `__call__` function that takes as input a batch of [States](https://github.com/saleml/gfn/blob/master/src/gfn/containers/states.py).\n\n- [LogEdgeFlowEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions)` tensor representing $\\log F(s \\rightarrow s\')$, including when $s\' = s_f$.\n- [LogStateFlowEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, 1)` tensor representing $\\log F(s)$. When used with `forward_looking=True`, $\\log F(s)$ is parametrized as the sum of a function approximator and $\\log R(s)$ - which is only possible for environments where all states are terminating.\n- [LogitPFEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions)` tensor representing $logit(s\' \\mid s)$, such that $P_F(s\' \\mid s) = softmax_{s\'}\\ logit(s\' \\mid s)$, including when $s\' = s_f$.\n- [LogitPBEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions - 1)` tensor representing $logit(s\' \\mid s)$, such that $P_B(s\' \\mid s) = softmax_{s\'}\\ logit(s\' \\mid s)$.\n\nDefining an estimator requires the environment, and a [module](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) instance. Modules inherit from the [GFNModule](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) class, which can be seen as an extension of `torch.nn.Module`. Alternatively, a module is created by providing which module type to use (e.g. "NeuralNet" or "Uniform" or "Zero"). A Basic MLP is provided as the [NeuralNet](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) class, but any function approximator should be possible.\n\nSaid differently, a `States` object is first transformed via the environment\'s preprocessor to a `(*batch_shape, *output_shape)` float tensor. The preprocessor\'s output shape should match the module input shape (if any). The preprocessed states are then passed as inputs to the module, returning the desired output (either flows or probabilities over children in the DAG).\n\nEach module has a `named_parameters` functions that returns a dictionary of the learnable parameters. This attribute is transferred to the corresponding estimator.\n\nAdditionally, a [LogZEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py) is provided, which is a container for a scalar tensor representing $\\log Z$, the log-partition function, useful for the Trajectory Balance loss for example. This estimator also has a `named_parameters` function.\n\n### Samplers\n\nAn [ActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py) object defines how actions are sampled at each state of the DAG. As of now, only [DiscreteActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py)s are implemented. The require an estimator (of $P_F$, $P_B$, or edge flows) defining the action probabilities. These estimators can contain any type of modules (including random action sampling for example). A [BackwardDiscreteActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py) class is provided to sample parents of a state, which is helpful to sample trajectories starting from their last states.\n\nThey are at the core of [TrajectoriesSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/trajectories_sampler.py)s, which implements the `sample_trajectories` method, that sample a batch of trajectories starting from a given set of initial states or starting from $s_0$.\n\n### Losses\n\nGFlowNets can be trained with different losses, each of which requires a different parametrization. A parametrization is a dataclass, which can be seen as a container of different estimators. Each parametrization defines a distribution over trajectories, via the `parametrization.Pi` method, and a distribution over terminating states, via the `parametrization.P_T` method. Both distributions should be instances of the classes defined [here](https://github.com/saleml/gfn/blob/master/src/gfn/distributions.py).\n\nThe base classes for losses and parametrizations are provided [here](https://github.com/saleml/gfn/blob/master/src/gfn/losses/base.py).\n\nCurrently, the implemented losses are:\n\n- Flow Matching\n- Detailed Balance\n- Trajectory Balance\n- Sub-Trajectory Balance. By default, each sub-trajectory is weighted geometrically (within the trajectory) depending on its length. This corresponds to the strategy defined [here](https://www.semanticscholar.org/reader/f2c32fe3f7f3e2e9d36d833e32ec55fc93f900f5). Other strategies exist and are implemented [here](https://github.com/saleml/gfn/blob/master/src/gfn/losses/sub_trajectory_balance.py).\n- Log Partition Variance loss. Introduced [here](https://arxiv.org/abs/2302.05446)\n\n### Solving for the flows using Dynamic Programming\n\nA simple script that propagates trajectories rewards through the DAG to define edge flows in a deterministic way (by visiting each edge once only) is provided [here](https://github.com/saleml/gfn/blob/master/scripts/dynamic_programming.py). Do not use the script on large environments !\n',
-    'author': 'Salem Lahou',
-    'author_email': 'salemlahlou9@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.10,<4.0',
-}
+</p>
+<p align="center">
+  <a href="https://gfn.readthedocs.io/en/latest/">Documentation</a> ~ <a href="https://github.com/saleml/gfn">Code</a>
+</p>
 
+# gfn: a Python package for GFlowNets
+
+
+
+## Installing the packages
+
+The codebase requires python >= 3.10
+
+To install the latest stable version:
+
+```bash
+pip install torchgfn
+```
+
+Optionally, to run scripts:
+
+```bash
+pip install torchgfn[scripts]
+```
+
+To install the cutting edge version (from the `main` branch):
+
+```bash
+git clone https://github.com/saleml/gfn.git
+conda create -n gfn python=3.11
+conda activate gfn
+cd gfn
+pip install .
+```
+
+
+## About this repo
+
+This repo serves the purpose of fast prototyping [GFlowNet](https://arxiv.org/abs/2111.09266) related algorithms. It decouples the environment definition, the sampling process, and the parametrization used for the GFN loss.
+
+An example script is provided [here](https://github.com/saleml/gfn/blob/master/scripts/train.py). To run the code, use one of the following:
+
+```bash
+python train.py --env hypergrid --env.ndim 4 --env.height 8 --n_iterations 100000 --loss trajectory-balance
+python train.py --env discrete-ebm --env.ndim 4 --env.alpha 0.5 --n_iterations 10000 --batch_size 64 --sampler.temperature 2.
+python train.py --env hypergrid --env.ndim 2 --env.height 64 --n_iterations 100000 --loss detailed-balance --logit_PB.module_name Uniform --optim adam --optim.lr 1e-3 --batch_size 64
+python train.py --env hypergrid --env.ndim 4 --env.height 8 --env.R0 0.01 --loss flowmatching --optim adam --optim.lr 1e-4
+```
+
+### Example, in a few lines
+
+(⬇️ This example require the [`tqdm`](https://github.com/tqdm/tqdm) package to run. `pip install tqdm` or install all extra requirements with `pip install .[scripts]`)
+
+```python
+import torch
+from tqdm import tqdm
+
+from gfn import LogitPBEstimator, LogitPFEstimator, LogZEstimator
+from gfn.envs import HyperGrid
+from gfn.losses import TBParametrization, TrajectoryBalance
+from gfn.samplers import DiscreteActionsSampler, TrajectoriesSampler
+
+if __name__ == "__main__":
+
+    env = HyperGrid(ndim=4, height=8, R0=0.01)  # Grid of size 8x8x8x8
+
+    logit_PF = LogitPFEstimator(env=env, module_name="NeuralNet")
+    logit_PB = LogitPBEstimator(
+        env=env,
+        module_name="NeuralNet",
+        torso=logit_PF.module.torso,  # To share parameters between PF and PB
+    )
+    logZ = LogZEstimator(torch.tensor(0.0))
+
+    parametrization = TBParametrization(logit_PF, logit_PB, logZ)
+
+    actions_sampler = DiscreteActionsSampler(estimator=logit_PF)
+    trajectories_sampler = TrajectoriesSampler(env=env, actions_sampler=actions_sampler)
+
+    loss_fn = TrajectoryBalance(parametrization=parametrization)
+
+    params = [
+        {
+            "params": [
+                val for key, val in parametrization.parameters.items() if "logZ" not in key
+            ],
+            "lr": 0.001,
+        },
+        {"params": [val for key, val in parametrization.parameters.items() if "logZ" in key], "lr": 0.1},
+    ]
+    optimizer = torch.optim.Adam(params)
+
+    for i in (pbar := tqdm(range(1000))):
+        trajectories = trajectories_sampler.sample(n_trajectories=16)
+        optimizer.zero_grad()
+        loss = loss_fn(trajectories)
+        loss.backward()
+        optimizer.step()
+        if i % 25 == 0:
+            pbar.set_postfix({"loss": loss.item()})
+
+```
+
+## Contributing
+
+Before the first commit:
+
+```bash
+pip install .[dev]
+pre-commit install
+pre-commit run --all-files
+```
+
+Run `pre-commit` after staging, and before committing. Make sure all the tests pass (By running `pytest`).
+The codebase uses `black` formatter.
+
+To make the docs locally:
+```bash
+cd docs
+make html
+open build/html/index.html
+```
+
+## Details about the codebase
+
+### Defining an environment
+
+A pointed DAG environment (or GFN environment, or environment for short) is a representation for the pointed DAG. The abstract class [Env](https://github.com/saleml/gfn/blob/master/src/gfn/envs/env.py) specifies the requirements for a valid environment definition. To obtain such a representation, the environment needs to specify the following attributes, properties, or methods:
+
+- The `action_space`. Which should be a `gymnasium.spaces.Discrete` object for discrete environments. The last action should correspond to the exit action.
+- The initial state `s_0`, as a `torch.Tensor` of arbitrary dimension.
+- (Optional) The sink state `s_f`, as a `torch.Tensor` of the same shape as `s_0`, used to represent complete trajectories only (within a batch of trajectories of different lengths), and never processed by any model. If not specified, it is set to `torch.full_like(s_0, -float('inf'))`.
+- The method `make_States_class` that creates a subclass of [States](https://github.com/saleml/gfn/blob/master/src/gfn/containers/states.py). The instances of the resulting class should represent a batch of states of arbitrary shape, which is useful to define a trajectory, or a batch of trajectories. `s_0` and `s_f`, along with a tuple called `state_shape` should be defined as class variables, and the subclass (of `States`) should implement masking methods, that specify which actions are possible, in a discrete environment.
+- The methods `maskless_step` and `maskless_backward_step` that specify how an action changes a state (going forward and backward). These functions do not need to handle masking, checking whether actions are allowed, checking whether a state is the sink state, etc... These checks are handled in `Env.step` and `Env.backward_step`
+- The `log_reward` function that assigns a nonnegative reward to every terminating state (i.e. state with all $s_f$ as a child in the DAG). If `log_reward` is not implemented, `reward` needs to be.
+
+If the states (as represented in the `States` class) need to be transformed to another format before being processed (by neural networks for example), then the environment should define a `preprocessor` attribute, which should be an instance of the [base preprocessor class](https://github.com/saleml/gfn/blob/master/src/gfn/envs/preprocessors/base.py). If no preprocessor is defined, the states are used as is (actually transformed using  [`IdentityPreprocessor`](https://github.com/saleml/gfn/blob/master/src/gfn/envs/preprocessors/base.py), which transforms the state tensors to `FloatTensor`s). Implementing your own preprocessor requires defining the `preprocess` function, and the `output_shape` attribute, which is a tuple representing the shape of *one* preprocessed state.
+
+Optionally, you can define a static `get_states_indices` method that assigns a unique integer number to each state if the environment allows it, and a `n_states` property that returns an integer representing the number of states (excluding $s_f$) in the environment. `get_terminating_states_indices` can also be implemented and serves the purpose of uniquely identifying terminating states of the environment.
+
+For more details, take a look at [HyperGrid](https://github.com/saleml/gfn/blob/master/src/gfn/envs/hypergrid.py), an environment where all states are terminating states, or at [DiscreteEBM](https://github.com/saleml/gfn/blob/master/src/gfn/envs/discrete_ebm.py), where all trajectories are of the same length but only some states are terminating.
+
+### Other containers
+
+Besides the `States` class, other containers of states are available:
+
+- [Transitions](https://github.com/saleml/gfn/blob/master/src/gfn/containers/transitions.py), representing a batch of transitions $s \rightarrow s'$.
+- [Trajectories](https://github.com/saleml/gfn/blob/master/src/gfn/containers/trajectories.py), representing a batch of complete trajectories $\tau = s_0 \rightarrow s_1 \rightarrow \dots \rightarrow s_n \rightarrow s_f$.
+
+These containers can either be instantiated using a `States` object, or can be initialized as empty containers that can be populated on the fly, allowing the usage of [ReplayBuffer](https://github.com/saleml/gfn/blob/master/src/gfn/containers/replay_buffer.py)s.
+
+They inherit from the base `Container` [class](https://github.com/saleml/gfn/blob/master/src/gfn/containers/base.py), indicating some helpful methods.
+
+In most cases, one needs to sample complete trajectories. From a batch of trajectories, a batch of states and batch of transitions can be defined using `Trajectories.to_transitions()` and `Trajectories.to_states()`. These exclude meaningless transitions and states that were added to the batch of trajectories to allow for efficient batching.
+
+### Estimators and Modules
+
+Training GFlowNets requires one or multiple estimators. As of now, only discrete environments are handled. All estimators are subclasses of [FunctionEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py), implementing a `__call__` function that takes as input a batch of [States](https://github.com/saleml/gfn/blob/master/src/gfn/containers/states.py).
+
+- [LogEdgeFlowEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions)` tensor representing $\log F(s \rightarrow s')$, including when $s' = s_f$.
+- [LogStateFlowEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, 1)` tensor representing $\log F(s)$. When used with `forward_looking=True`, $\log F(s)$ is parametrized as the sum of a function approximator and $\log R(s)$ - which is only possible for environments where all states are terminating.
+- [LogitPFEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions)` tensor representing $logit(s' \mid s)$, such that $P_F(s' \mid s) = softmax_{s'}\ logit(s' \mid s)$, including when $s' = s_f$.
+- [LogitPBEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py). It outputs a `(*batch_shape, n_actions - 1)` tensor representing $logit(s' \mid s)$, such that $P_B(s' \mid s) = softmax_{s'}\ logit(s' \mid s)$.
+
+Defining an estimator requires the environment, and a [module](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) instance. Modules inherit from the [GFNModule](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) class, which can be seen as an extension of `torch.nn.Module`. Alternatively, a module is created by providing which module type to use (e.g. "NeuralNet" or "Uniform" or "Zero"). A Basic MLP is provided as the [NeuralNet](https://github.com/saleml/gfn/blob/master/src/gfn/modules.py) class, but any function approximator should be possible.
+
+Said differently, a `States` object is first transformed via the environment's preprocessor to a `(*batch_shape, *output_shape)` float tensor. The preprocessor's output shape should match the module input shape (if any). The preprocessed states are then passed as inputs to the module, returning the desired output (either flows or probabilities over children in the DAG).
+
+Each module has a `named_parameters` functions that returns a dictionary of the learnable parameters. This attribute is transferred to the corresponding estimator.
+
+Additionally, a [LogZEstimator](https://github.com/saleml/gfn/blob/master/src/gfn/estimators.py) is provided, which is a container for a scalar tensor representing $\log Z$, the log-partition function, useful for the Trajectory Balance loss for example. This estimator also has a `named_parameters` function.
+
+### Samplers
+
+An [ActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py) object defines how actions are sampled at each state of the DAG. As of now, only [DiscreteActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py)s are implemented. The require an estimator (of $P_F$, $P_B$, or edge flows) defining the action probabilities. These estimators can contain any type of modules (including random action sampling for example). A [BackwardDiscreteActionsSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/actions_samplers.py) class is provided to sample parents of a state, which is helpful to sample trajectories starting from their last states.
+
+They are at the core of [TrajectoriesSampler](https://github.com/saleml/gfn/blob/master/src/gfn/samplers/trajectories_sampler.py)s, which implements the `sample_trajectories` method, that sample a batch of trajectories starting from a given set of initial states or starting from $s_0$.
+
+### Losses
+
+GFlowNets can be trained with different losses, each of which requires a different parametrization. A parametrization is a dataclass, which can be seen as a container of different estimators. Each parametrization defines a distribution over trajectories, via the `parametrization.Pi` method, and a distribution over terminating states, via the `parametrization.P_T` method. Both distributions should be instances of the classes defined [here](https://github.com/saleml/gfn/blob/master/src/gfn/distributions.py).
+
+The base classes for losses and parametrizations are provided [here](https://github.com/saleml/gfn/blob/master/src/gfn/losses/base.py).
+
+Currently, the implemented losses are:
+
+- Flow Matching
+- Detailed Balance
+- Trajectory Balance
+- Sub-Trajectory Balance. By default, each sub-trajectory is weighted geometrically (within the trajectory) depending on its length. This corresponds to the strategy defined [here](https://www.semanticscholar.org/reader/f2c32fe3f7f3e2e9d36d833e32ec55fc93f900f5). Other strategies exist and are implemented [here](https://github.com/saleml/gfn/blob/master/src/gfn/losses/sub_trajectory_balance.py).
+- Log Partition Variance loss. Introduced [here](https://arxiv.org/abs/2302.05446)
+
+### Solving for the flows using Dynamic Programming
+
+A simple script that propagates trajectories rewards through the DAG to define edge flows in a deterministic way (by visiting each edge once only) is provided [here](https://github.com/saleml/gfn/blob/master/scripts/dynamic_programming.py). Do not use the script on large environments !
 
-setup(**setup_kwargs)
```

