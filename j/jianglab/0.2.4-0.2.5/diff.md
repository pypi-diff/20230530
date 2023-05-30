# Comparing `tmp/jianglab-0.2.4.tar.gz` & `tmp/jianglab-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.2.4.tar", last modified: Tue May 30 15:42:00 2023, max compression
+gzip compressed data, was "jianglab-0.2.5.tar", last modified: Tue May 30 15:46:31 2023, max compression
```

## Comparing `jianglab-0.2.4.tar` & `jianglab-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:42:00.967654 jianglab-0.2.4/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:42:00.967335 jianglab-0.2.4/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.4/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:42:00.964206 jianglab-0.2.4/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.2.4/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    12510 2023-05-30 15:41:30.000000 jianglab-0.2.4/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.2.4/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:42:00.966683 jianglab-0.2.4/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:42:00.000000 jianglab-0.2.4/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-05-30 15:42:00.000000 jianglab-0.2.4/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-05-30 15:42:00.000000 jianglab-0.2.4/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       87 2023-05-30 15:42:00.000000 jianglab-0.2.4/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-05-30 15:42:00.000000 jianglab-0.2.4/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-05-30 15:42:00.967770 jianglab-0.2.4/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      892 2023-05-30 15:41:57.000000 jianglab-0.2.4/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:46:31.530737 jianglab-0.2.5/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:46:31.530407 jianglab-0.2.5/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.5/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:46:31.527366 jianglab-0.2.5/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.2.5/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    12611 2023-05-30 15:46:17.000000 jianglab-0.2.5/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.2.5/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:46:31.529874 jianglab-0.2.5/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:46:31.000000 jianglab-0.2.5/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-05-30 15:46:31.000000 jianglab-0.2.5/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-05-30 15:46:31.000000 jianglab-0.2.5/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       87 2023-05-30 15:46:31.000000 jianglab-0.2.5/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-05-30 15:46:31.000000 jianglab-0.2.5/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-05-30 15:46:31.530854 jianglab-0.2.5/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      892 2023-05-30 15:46:26.000000 jianglab-0.2.5/setup.py
```

### Comparing `jianglab-0.2.4/PKG-INFO` & `jianglab-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.4/README.md` & `jianglab-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.2.4/jianglab/common_functions.py` & `jianglab-0.2.5/jianglab/common_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,23 +196,26 @@
         tree.create_node(tag=tag, identifier=node_id, parent=parent_id)
         
         if isinstance(value, dict):
             dict_to_tree(value, parent_id=node_id, tree=tree)
 
     return tree
 
-def import_gsheet(sheet_name = params.sheet_name,
-                cred = params.google_cred
+def import_gsheet(sheet_name = "MEA dashboard",
+                cred = "./credentials/vibrant-epsilon-169702-467fddc26dfc.json"
                 ):
 
     for i in range(3):# search parent folder
         if not os.path.exists(cred): 
             cred = "." + cred
 
-    scope = params.scope
+    scope = [
+    "https://spreadsheets.google.com/feeds",
+    "https://www.googleapis.com/auth/drive",
+    ]
     creds_obj = ServiceAccountCredentials.from_json_keyfile_name(cred, scope)
     client = gspread.authorize(creds_obj)
     sheet = client.open(sheet_name).sheet1.get_all_records()
     df = pd.DataFrame.from_dict(sheet)
     df.to_csv("../gsheet_table.csv", index = False)
     return df
 
@@ -235,15 +238,15 @@
 def save_instance(filename, instance):
     with open(filename, "wb") as file_:
         pickle.dump(instance, file_, -1)
 
 def load_instance(filename):
     return pickle.load(open(filename, "rb", -1))
 
-def find_3d_local_min_general(arr, neighbor_size =  params.center_search_range):
+def find_3d_local_min_general(arr, neighbor_size = (6,6,6)):
     if arr.shape[0] != 0:
         counter = 0
         neighbor_size = np.array(neighbor_size)
         pad =  (neighbor_size/2).astype(np.int)
         arr_pad = np.pad(arr, ((pad[0],pad[0]), (pad[1],pad[1]), (pad[2],pad[2])), 'constant', constant_values = arr.max())
         arr_pad = arr_pad.astype(np.int)
         center_list = []
```

### Comparing `jianglab-0.2.4/jianglab.egg-info/PKG-INFO` & `jianglab-0.2.5/jianglab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.4/setup.py` & `jianglab-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.2.4',
+    version='0.2.5',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

