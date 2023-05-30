# Comparing `tmp/dataset_librarian-0.0.0.dev1.tar.gz` & `tmp/dataset_librarian-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_librarian-0.0.0.dev1.tar", last modified: Fri May 26 08:30:31 2023, max compression
+gzip compressed data, was "dataset_librarian-1.0.0.tar", last modified: Tue May 30 19:27:31 2023, max compression
```

## Comparing `dataset_librarian-0.0.0.dev1.tar` & `dataset_librarian-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,32 @@
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     4570 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     4105 2023-05-25 19:30:11.000000 dataset_librarian-0.0.0.dev1/README.md
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      608 2023-05-26 08:30:22.000000 dataset_librarian-0.0.0.dev1/pyproject.toml
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/setup.cfg
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/src/
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/src/dataset_librarian/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:36:44.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian/__init__.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/src/dataset_librarian/subpackage/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:36:44.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian/subpackage/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       34 2023-05-05 17:36:44.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian/subpackage/test.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-26 08:30:31.112306 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     4570 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      368 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/SOURCES.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/dependency_links.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       16 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/requires.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       18 2023-05-26 08:30:31.000000 dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/top_level.txt
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-30 19:27:31.788910 dataset_librarian-1.0.0/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3974 2023-05-30 19:27:31.788910 dataset_librarian-1.0.0/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3424 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/README.md
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      804 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/pyproject.toml
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-05-30 19:27:31.788910 dataset_librarian-1.0.0/setup.cfg
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-30 19:27:31.784910 dataset_librarian-1.0.0/src/
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-30 19:27:31.788910 dataset_librarian-1.0.0/src/dataset_librarian/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3944 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/dataset.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-30 19:27:31.788910 dataset_librarian-1.0.0/src/dataset_librarian/dataset_api/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/dataset_api/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2302 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/dataset_api/download.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3484 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/dataset_api/preprocess.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2425 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/datasets_urls.json
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-30 19:27:31.788910 dataset_librarian-1.0.0/src/dataset_librarian/scripts/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/scripts/__init__.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-30 19:27:31.788910 dataset_librarian-1.0.0/src/dataset_librarian/scripts/brca/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/scripts/brca/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2410 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/scripts/brca/create_data_split.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     8135 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/scripts/brca/prepare_nlp_data.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)    10700 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/scripts/brca/prepare_vision_data.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-30 19:27:31.788910 dataset_librarian-1.0.0/src/dataset_librarian/scripts/mvtec-ad/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/scripts/mvtec-ad/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2746 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/scripts/mvtec-ad/csv_generator_mvtec.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     1928 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/src/dataset_librarian/terms_and_conditions.txt
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-30 19:27:31.788910 dataset_librarian-1.0.0/src/dataset_librarian.egg-info/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3974 2023-05-30 19:27:30.000000 dataset_librarian-1.0.0/src/dataset_librarian.egg-info/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      939 2023-05-30 19:27:31.000000 dataset_librarian-1.0.0/src/dataset_librarian.egg-info/SOURCES.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-05-30 19:27:30.000000 dataset_librarian-1.0.0/src/dataset_librarian.egg-info/dependency_links.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       77 2023-05-30 19:27:30.000000 dataset_librarian-1.0.0/src/dataset_librarian.egg-info/requires.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       18 2023-05-30 19:27:30.000000 dataset_librarian-1.0.0/src/dataset_librarian.egg-info/top_level.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)   102383 2023-05-30 19:23:51.000000 dataset_librarian-1.0.0/third-party-programs.txt
```

### Comparing `dataset_librarian-0.0.0.dev1/PKG-INFO` & `dataset_librarian-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,27 @@
 Metadata-Version: 2.1
 Name: dataset_librarian
-Version: 0.0.0.dev1
-Summary: Package Placeholder
+Version: 1.0.0
+Summary: Dataset librarian is a tool to download and apply the preprocessing needed for the list of supported datasets
 Author-email: IntelAI <IntelAI@intel.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/markdown
 
-# Dataset API
-
-## Dataset API structure
-```
-dataset_api
-├── conda
-│   └── recipes
-│       ├── py38_recipe
-│       └── py39_recipe
-├── src
-│   └── dataset_librarian
-│       ├── dataset_api
-│       ├── scripts
-│       ├── __init__.py
-│       ├── dataset.py
-│       ├── datasets_urls.json
-├── MANIFEST.in
-├── README.md
-├── pyproject.toml
-└── requirements.txt
-```
-
-## Environment setup
-Clone the [Model Zoo for Intel® Architecture](https://github.com/IntelAI/models) repository and navigate to the `dataset_api` directory.
+# Dataset Librarian
 
+## Installation Process
 ```bash
-# Step 1 (recommended): Create and activate a virtual environment
-## Option 1: Using virtualenv
-virtualenv -p python3 venv
-. venv/bin/activate
-## Option 2: Using conda
-conda create -n venv python=<3.8 or 3.9> -c conda-forge
-conda activate venv
-
-# Step 2: Installing package
-## Option 1: Installing from source code
-cd models/datasets/dataset_api
-python -m pip install --upgrade pip build setuptools wheel
-python -m pip install .
-## Option 2: Installing from PyPI
 python -m pip install dataset-librarian
 ```
-PyPI package can be found [here](https://pypi.org/project/dataset-librarian/).
+For more information check the [dataset-librarian PyPI package](https://pypi.org/project/dataset-librarian/)
 
 ## Datasets
 | Dataset name | Description | Download | Preprocessing | command |
 | ------------ | ----------- | -------- | --------------| ------- |
 | `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory>` |
 | `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python -m dataset_librarian.dataset -n tabformer --download` |
 | `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python -m dataset_librarian.dataset -n dureader-vis --download` |
@@ -82,7 +46,16 @@
 
 # Download the datasets
 download_dataset('brca', <path to the raw dataset directory>)
 
 # Preprocess the datasets
 preprocess_dataset('brca', <path to the raw dataset directory>)
 ```
+## Building for source
+Clone the [Model Zoo for Intel® Architecture](https://github.com/IntelAI/models) repository and navigate to the `dataset_api` directory.
+
+```bash
+git clone https://github.com/IntelAI/models.git
+cd models/datasets/dataset_api
+python -m pip install --upgrade pip build setuptools wheel
+python -m pip install .
+```
```

### Comparing `dataset_librarian-0.0.0.dev1/README.md` & `dataset_librarian-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,14 @@
-# Dataset API
-
-## Dataset API structure
-```
-dataset_api
-├── conda
-│   └── recipes
-│       ├── py38_recipe
-│       └── py39_recipe
-├── src
-│   └── dataset_librarian
-│       ├── dataset_api
-│       ├── scripts
-│       ├── __init__.py
-│       ├── dataset.py
-│       ├── datasets_urls.json
-├── MANIFEST.in
-├── README.md
-├── pyproject.toml
-└── requirements.txt
-```
-
-## Environment setup
-Clone the [Model Zoo for Intel® Architecture](https://github.com/IntelAI/models) repository and navigate to the `dataset_api` directory.
+# Dataset Librarian
 
+## Installation Process
 ```bash
-# Step 1 (recommended): Create and activate a virtual environment
-## Option 1: Using virtualenv
-virtualenv -p python3 venv
-. venv/bin/activate
-## Option 2: Using conda
-conda create -n venv python=<3.8 or 3.9> -c conda-forge
-conda activate venv
-
-# Step 2: Installing package
-## Option 1: Installing from source code
-cd models/datasets/dataset_api
-python -m pip install --upgrade pip build setuptools wheel
-python -m pip install .
-## Option 2: Installing from PyPI
 python -m pip install dataset-librarian
 ```
-PyPI package can be found [here](https://pypi.org/project/dataset-librarian/).
+For more information check the [dataset-librarian PyPI package](https://pypi.org/project/dataset-librarian/)
 
 ## Datasets
 | Dataset name | Description | Download | Preprocessing | command |
 | ------------ | ----------- | -------- | --------------| ------- |
 | `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory>` |
 | `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python -m dataset_librarian.dataset -n tabformer --download` |
 | `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python -m dataset_librarian.dataset -n dureader-vis --download` |
@@ -69,7 +33,16 @@
 
 # Download the datasets
 download_dataset('brca', <path to the raw dataset directory>)
 
 # Preprocess the datasets
 preprocess_dataset('brca', <path to the raw dataset directory>)
 ```
+## Building for source
+Clone the [Model Zoo for Intel® Architecture](https://github.com/IntelAI/models) repository and navigate to the `dataset_api` directory.
+
+```bash
+git clone https://github.com/IntelAI/models.git
+cd models/datasets/dataset_api
+python -m pip install --upgrade pip build setuptools wheel
+python -m pip install .
+```
```

### Comparing `dataset_librarian-0.0.0.dev1/pyproject.toml` & `dataset_librarian-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset_librarian"
-version = "0.0.0dev1"
+version = "1.0.0"
 requires-python = ">=3.8,<3.10"
 authors = [
     { name="IntelAI", email="IntelAI@intel.com"}
 ]
-description = "Package Placeholder"
+description = "Dataset librarian is a tool to download and apply the preprocessing needed for the list of supported datasets"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    "packaging >=23.0"
-]
+    "pandas",
+    "tqdm",
+    "docx2txt",
+    "openpyxl",
+    "pillow",
+    "scikit-learn-intelex",
+    "python-dotenv",
+    "wget"
+]
```

### Comparing `dataset_librarian-0.0.0.dev1/src/dataset_librarian.egg-info/PKG-INFO` & `dataset_librarian-1.0.0/src/dataset_librarian.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,27 @@
 Metadata-Version: 2.1
 Name: dataset-librarian
-Version: 0.0.0.dev1
-Summary: Package Placeholder
+Version: 1.0.0
+Summary: Dataset librarian is a tool to download and apply the preprocessing needed for the list of supported datasets
 Author-email: IntelAI <IntelAI@intel.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/markdown
 
-# Dataset API
-
-## Dataset API structure
-```
-dataset_api
-├── conda
-│   └── recipes
-│       ├── py38_recipe
-│       └── py39_recipe
-├── src
-│   └── dataset_librarian
-│       ├── dataset_api
-│       ├── scripts
-│       ├── __init__.py
-│       ├── dataset.py
-│       ├── datasets_urls.json
-├── MANIFEST.in
-├── README.md
-├── pyproject.toml
-└── requirements.txt
-```
-
-## Environment setup
-Clone the [Model Zoo for Intel® Architecture](https://github.com/IntelAI/models) repository and navigate to the `dataset_api` directory.
+# Dataset Librarian
 
+## Installation Process
 ```bash
-# Step 1 (recommended): Create and activate a virtual environment
-## Option 1: Using virtualenv
-virtualenv -p python3 venv
-. venv/bin/activate
-## Option 2: Using conda
-conda create -n venv python=<3.8 or 3.9> -c conda-forge
-conda activate venv
-
-# Step 2: Installing package
-## Option 1: Installing from source code
-cd models/datasets/dataset_api
-python -m pip install --upgrade pip build setuptools wheel
-python -m pip install .
-## Option 2: Installing from PyPI
 python -m pip install dataset-librarian
 ```
-PyPI package can be found [here](https://pypi.org/project/dataset-librarian/).
+For more information check the [dataset-librarian PyPI package](https://pypi.org/project/dataset-librarian/)
 
 ## Datasets
 | Dataset name | Description | Download | Preprocessing | command |
 | ------------ | ----------- | -------- | --------------| ------- |
 | `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory>` |
 | `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python -m dataset_librarian.dataset -n tabformer --download` |
 | `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python -m dataset_librarian.dataset -n dureader-vis --download` |
@@ -82,7 +46,16 @@
 
 # Download the datasets
 download_dataset('brca', <path to the raw dataset directory>)
 
 # Preprocess the datasets
 preprocess_dataset('brca', <path to the raw dataset directory>)
 ```
+## Building for source
+Clone the [Model Zoo for Intel® Architecture](https://github.com/IntelAI/models) repository and navigate to the `dataset_api` directory.
+
+```bash
+git clone https://github.com/IntelAI/models.git
+cd models/datasets/dataset_api
+python -m pip install --upgrade pip build setuptools wheel
+python -m pip install .
+```
```

