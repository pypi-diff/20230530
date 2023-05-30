# Comparing `tmp/json-to-github-actions-1.0.0.tar.gz` & `tmp/json-to-github-actions-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-to-github-actions-1.0.0.tar", last modified: Mon May 29 09:39:49 2023, max compression
+gzip compressed data, was "json-to-github-actions-1.0.1.tar", last modified: Tue May 30 00:50:34 2023, max compression
```

## Comparing `json-to-github-actions-1.0.0.tar` & `json-to-github-actions-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-29 09:39:49.209490 json-to-github-actions-1.0.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1518 2023-05-29 09:39:49.209373 json-to-github-actions-1.0.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1411 2023-05-29 09:39:48.000000 json-to-github-actions-1.0.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-29 09:39:49.209202 json-to-github-actions-1.0.0/json_to_github_actions.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1518 2023-05-29 09:39:49.000000 json-to-github-actions-1.0.0/json_to_github_actions.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-29 09:39:49.000000 json-to-github-actions-1.0.0/json_to_github_actions.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-29 09:39:49.000000 json-to-github-actions-1.0.0/json_to_github_actions.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-05-29 09:39:49.000000 json-to-github-actions-1.0.0/json_to_github_actions.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       21 2023-05-29 09:39:49.000000 json-to-github-actions-1.0.0/json_to_github_actions.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-29 09:39:49.000000 json-to-github-actions-1.0.0/json_to_github_actions.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     4188 2023-05-29 09:39:48.000000 json-to-github-actions-1.0.0/json_to_github_actions.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-29 09:39:49.209527 json-to-github-actions-1.0.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-29 09:39:48.000000 json-to-github-actions-1.0.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-30 00:50:34.047896 json-to-github-actions-1.0.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2099 2023-05-30 00:50:34.047764 json-to-github-actions-1.0.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1992 2023-05-30 00:50:33.000000 json-to-github-actions-1.0.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-30 00:50:34.047586 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2099 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       21 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-30 00:50:34.000000 json-to-github-actions-1.0.1/json_to_github_actions.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     4188 2023-05-30 00:50:33.000000 json-to-github-actions-1.0.1/json_to_github_actions.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-30 00:50:34.047932 json-to-github-actions-1.0.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-30 00:50:33.000000 json-to-github-actions-1.0.1/setup.py
```

### Comparing `json-to-github-actions-1.0.0/PKG-INFO` & `json-to-github-actions-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,70 @@
-Metadata-Version: 2.1
-Name: json-to-github-actions
-Version: 1.0.0
-Description-Content-Type: text/markdown
-
 # JSON 轉 GitHub Actions YAML
+```
+🐔動機: 全球免費20 VMs運算，有感試用，可以把 python 或 julia 放到 github actions 算 
+💣地雷: 格式轉換會存在很多 bugs, 要先生最終無 bugs .yml 才反推轉換的 .py 此套件程式碼
+🧪實驗: Roy julia套件清物聯網資料已經分散兩台 VMs (每個4GB .zip處理55分鐘)運算成功
+🧾待辦: 雖然可分散運算了，但運算結果還需要轉化為 github release .zip 抓回來結果
 這個 Python 套件能將 JSON 格式轉化為 GitHub Actions 的 YAML 格式。
+```
 
 ## 安裝
-將 `json_to_github_actions.py` 放到您的專案資料夾中
+python3 -m pip install json-to-github-actions
 
 ## CLI 用法
 ```
 python json_to_github_actions.py --json_file [json_file] --yaml_file [yaml_file]
 ```
 
 範例：
 ```bash
 python json_to_github_actions.py --json_file input.json --yaml_file output.yaml
 ```
-
 輸入 `json_file` 是您的 JSON 檔案路徑，並將產生的 GitHub Actions YAML 檔案保存到給定的 `yaml_file` 路徑。
-
 ## 套件 import 用法
 首先，將 `json_to_github_actions.py` 腳本導入您的專案。
 
 ```python
 from json_to_github_actions import json_to_github_actions
 ```
-
 然後您可以調用 `json_to_github_actions()` 函數將 JSON 輸入轉換為 YAML 格式。
 
-```python
-json_data = '''
+```json
 {
-  "repo_url": "https://github.com/user/repo",
-  "script_dir": "scripts",
-  "script_name": "main.py",
+  "repo_url": "https://github.com/user_name/json_to_github_actions.git",
+  "script_name": "add_two_numbers.py",
+  "script_dir": "/add_two_numbers/",
   "execution_environment": [
     {
       "language": "python",
       "version": "3.8",
-      "installation_command": "pip install -r requirements.txt"
+      "installation_command": "python -m pip install -r requirements.txt"
     }
   ],
+  "max_parallel": 3,
   "json_parameters": [
-    {"param1": "value1", "param2": 42},
-    {"param1": "value2", "param2": 24}
+    {
+      "a": 1,
+      "b": 2
+    },
+    {
+      "a": 3,
+      "b": 4
+    },
+    {
+      "a": 5,
+      "b": 6
+    },
+    {
+      "a": 7,
+      "b": 8
+    }
   ],
-  "max_parallel": 2
+  "copy_dirs_outputs": []
 }
+
 '''
 
 yaml_data = json_to_github_actions(json_data)
 ```
 
 這將把 JSON 格式的數據轉換為適用於 GitHub Actions 的 YAML 格式。之後，您可以選擇將 `yaml_data` 保存到檔案中。
```

### Comparing `json-to-github-actions-1.0.0/json_to_github_actions.egg-info/PKG-INFO` & `json-to-github-actions-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,75 @@
 Metadata-Version: 2.1
 Name: json-to-github-actions
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # JSON 轉 GitHub Actions YAML
+```
+🐔動機: 全球免費20 VMs運算，有感試用，可以把 python 或 julia 放到 github actions 算 
+💣地雷: 格式轉換會存在很多 bugs, 要先生最終無 bugs .yml 才反推轉換的 .py 此套件程式碼
+🧪實驗: Roy julia套件清物聯網資料已經分散兩台 VMs (每個4GB .zip處理55分鐘)運算成功
+🧾待辦: 雖然可分散運算了，但運算結果還需要轉化為 github release .zip 抓回來結果
 這個 Python 套件能將 JSON 格式轉化為 GitHub Actions 的 YAML 格式。
+```
 
 ## 安裝
-將 `json_to_github_actions.py` 放到您的專案資料夾中
+python3 -m pip install json-to-github-actions
 
 ## CLI 用法
 ```
 python json_to_github_actions.py --json_file [json_file] --yaml_file [yaml_file]
 ```
 
 範例：
 ```bash
 python json_to_github_actions.py --json_file input.json --yaml_file output.yaml
 ```
-
 輸入 `json_file` 是您的 JSON 檔案路徑，並將產生的 GitHub Actions YAML 檔案保存到給定的 `yaml_file` 路徑。
-
 ## 套件 import 用法
 首先，將 `json_to_github_actions.py` 腳本導入您的專案。
 
 ```python
 from json_to_github_actions import json_to_github_actions
 ```
-
 然後您可以調用 `json_to_github_actions()` 函數將 JSON 輸入轉換為 YAML 格式。
 
-```python
-json_data = '''
+```json
 {
-  "repo_url": "https://github.com/user/repo",
-  "script_dir": "scripts",
-  "script_name": "main.py",
+  "repo_url": "https://github.com/user_name/json_to_github_actions.git",
+  "script_name": "add_two_numbers.py",
+  "script_dir": "/add_two_numbers/",
   "execution_environment": [
     {
       "language": "python",
       "version": "3.8",
-      "installation_command": "pip install -r requirements.txt"
+      "installation_command": "python -m pip install -r requirements.txt"
     }
   ],
+  "max_parallel": 3,
   "json_parameters": [
-    {"param1": "value1", "param2": 42},
-    {"param1": "value2", "param2": 24}
+    {
+      "a": 1,
+      "b": 2
+    },
+    {
+      "a": 3,
+      "b": 4
+    },
+    {
+      "a": 5,
+      "b": 6
+    },
+    {
+      "a": 7,
+      "b": 8
+    }
   ],
-  "max_parallel": 2
+  "copy_dirs_outputs": []
 }
+
 '''
 
 yaml_data = json_to_github_actions(json_data)
 ```
 
 這將把 JSON 格式的數據轉換為適用於 GitHub Actions 的 YAML 格式。之後，您可以選擇將 `yaml_data` 保存到檔案中。
```

### Comparing `json-to-github-actions-1.0.0/json_to_github_actions.py` & `json-to-github-actions-1.0.1/json_to_github_actions.py`

 * *Files identical despite different names*

### Comparing `json-to-github-actions-1.0.0/setup.py` & `json-to-github-actions-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="json-to-github-actions",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     py_modules=['json_to_github_actions'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'json_to_github_actions = json_to_github_actions:main',
         ],
```

