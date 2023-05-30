# Comparing `tmp/squaredown-1.4.2.tar.gz` & `tmp/squaredown-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squaredown-1.4.2.tar", max compression
+gzip compressed data, was "squaredown-1.4.3.tar", max compression
```

## Comparing `squaredown-1.4.2.tar` & `squaredown-1.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1079 2020-08-22 21:27:12.749605 squaredown-1.4.2/LICENSE
--rw-r--r--   0        0        0     1405 2022-11-02 16:59:09.235680 squaredown-1.4.2/README.md
--rw-r--r--   0        0        0      884 2023-03-17 14:49:57.753965 squaredown-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      259 2023-03-17 14:50:04.810022 squaredown-1.4.2/squaredown/__init__.py
--rw-r--r--   0        0        0     5629 2022-11-03 03:18:23.859642 squaredown-1.4.2/squaredown/catalog.py
--rw-r--r--   0        0        0     3128 2022-11-03 03:03:40.528656 squaredown-1.4.2/squaredown/connector.py
--rw-r--r--   0        0        0    12628 2021-02-23 14:21:00.968617 squaredown-1.4.2/squaredown/i_square.py
--rw-r--r--   0        0        0     4088 2022-11-03 03:18:23.863642 squaredown-1.4.2/squaredown/itemizations.py
--rw-r--r--   0        0        0     2244 2022-11-03 03:18:23.863642 squaredown-1.4.2/squaredown/locations.py
--rw-r--r--   0        0        0      987 2021-02-23 14:21:00.968617 squaredown-1.4.2/squaredown/logging_config.json
--rw-r--r--   0        0        0    16566 2023-03-17 14:49:24.417698 squaredown-1.4.2/squaredown/orders.py
--rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 squaredown-1.4.2/setup.py
--rw-r--r--   0        0        0     2217 1970-01-01 00:00:00.000000 squaredown-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2020-08-22 21:27:12.749605 squaredown-1.4.3/LICENSE
+-rw-r--r--   0        0        0     1405 2022-11-02 16:59:09.235680 squaredown-1.4.3/README.md
+-rw-r--r--   0        0        0      884 2023-05-30 19:57:48.818305 squaredown-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-05-30 19:58:01.902402 squaredown-1.4.3/squaredown/__init__.py
+-rw-r--r--   0        0        0     5629 2022-11-03 03:18:23.859642 squaredown-1.4.3/squaredown/catalog.py
+-rw-r--r--   0        0        0     3128 2022-11-03 03:03:40.528656 squaredown-1.4.3/squaredown/connector.py
+-rw-r--r--   0        0        0    12628 2021-02-23 14:21:00.968617 squaredown-1.4.3/squaredown/i_square.py
+-rw-r--r--   0        0        0     4088 2022-11-03 03:18:23.863642 squaredown-1.4.3/squaredown/itemizations.py
+-rw-r--r--   0        0        0     2244 2022-11-03 03:18:23.863642 squaredown-1.4.3/squaredown/locations.py
+-rw-r--r--   0        0        0      987 2021-02-23 14:21:00.968617 squaredown-1.4.3/squaredown/logging_config.json
+-rw-r--r--   0        0        0    16660 2023-05-30 19:57:27.010138 squaredown-1.4.3/squaredown/orders.py
+-rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 squaredown-1.4.3/setup.py
+-rw-r--r--   0        0        0     2217 1970-01-01 00:00:00.000000 squaredown-1.4.3/PKG-INFO
```

### Comparing `squaredown-1.4.2/LICENSE` & `squaredown-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.2/README.md` & `squaredown-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.2/pyproject.toml` & `squaredown-1.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squaredown"
-version = "1.4.2"
+version = "1.4.3"
 description = "Customized Square interface"
 authors = ["Jason Romano <aracnid@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aracnid/squaredown"
 keywords = ["python", "square", "mongodb"]
 packages = [{include = "squaredown"}]
```

### Comparing `squaredown-1.4.2/squaredown/catalog.py` & `squaredown-1.4.3/squaredown/catalog.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.2/squaredown/connector.py` & `squaredown-1.4.3/squaredown/connector.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.2/squaredown/i_square.py` & `squaredown-1.4.3/squaredown/i_square.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.2/squaredown/itemizations.py` & `squaredown-1.4.3/squaredown/itemizations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.2/squaredown/locations.py` & `squaredown-1.4.3/squaredown/locations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.2/squaredown/logging_config.json` & `squaredown-1.4.3/squaredown/logging_config.json`

 * *Files identical despite different names*

### Comparing `squaredown-1.4.2/squaredown/orders.py` & `squaredown-1.4.3/squaredown/orders.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,20 +57,24 @@
 
         Returns:
             None
         """
         # read the orders
         orders = self.read_orders(from_raw, **kwargs)
 
+        # end if no orders
+        if not orders or len(orders) == 0:
+            logger.info(f'orders processed: 0')
+            return
+
         # check last updated object for duplicate
-        if len(orders) > 0:
-            order = orders[0]
-            if order['id'] == self.props.last_id:
-                if self.decode_datetime(order['updated_at']) == self.props.last_updated:
-                    orders.pop(0)
+        order = orders[0]
+        if order['id'] == self.props.last_id:
+            if self.decode_datetime(order['updated_at']) == self.props.last_updated:
+                orders.pop(0)
 
         update_count = 0
         for order in tqdm(orders, desc='orders'):
             # save the raw order
             if not from_raw:
                 self.save_raw_order(order)
```

### Comparing `squaredown-1.4.2/setup.py` & `squaredown-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'aracnid-utils>=1.0,<2.0',
  'i-mongodb>=2.0,<3.0',
  'squareup>=19.1,<20.0',
  'tqdm>=4.64,<5.0']
 
 setup_kwargs = {
     'name': 'squaredown',
-    'version': '1.4.2',
+    'version': '1.4.3',
     'description': 'Customized Square interface',
     'long_description': '# Squaredown\n\nWe use Square as our point of sale system for our businesses. It works really well for most applications, but it takes too long to produce reports in a way that meets our business needs and the process is just too manual. We needed an automated way to produce our customized reports either at a click of a button or on a schedule. To do that we download the Square data into a MongoDB database. This is the code that we use to connect Square to MongoDB.\n\n## Getting Started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nThis package supports the following version of Python. It probably supports older versions, but they have not been tested.\n\n- Python 3.10 or later\n\n### Installing\n\nInstall the latest package using pip.\n\n```bash\n$ pip install squaredown\n```\n\nEnd with an example of getting some data out of the system or using it for a little demo\n\n## Running the tests\n\nExplain how to run the automated tests for this system\n\n```bash\n$ python -m pytest\n```\n\n## Usage\n\nTODO\n\n## Authors\n\n- **Jason Romano** - [Aracnid](https://github.com/aracnid)\n\nSee also the list of [contributors](https://github.com/lakeannebrewhouse/squaredown/contributors) who participated in this project.\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details\n',
     'author': 'Jason Romano',
     'author_email': 'aracnid@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/aracnid/squaredown',
```

### Comparing `squaredown-1.4.2/PKG-INFO` & `squaredown-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squaredown
-Version: 1.4.2
+Version: 1.4.3
 Summary: Customized Square interface
 Home-page: https://github.com/aracnid/squaredown
 License: MIT
 Keywords: python,square,mongodb
 Author: Jason Romano
 Author-email: aracnid@gmail.com
 Requires-Python: >=3.10,<4.0
```

