# Comparing `tmp/mikan_card_downloader-1.1.0.tar.gz` & `tmp/mikan_card_downloader-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-1.1.0.tar", max compression
+gzip compressed data, was "mikan_card_downloader-1.1.1.tar", max compression
```

## Comparing `mikan_card_downloader-1.1.0.tar` & `mikan_card_downloader-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.1.0/LICENSE
--rw-r--r--   0        0        0     1041 2023-05-06 20:00:28.315898 mikan_card_downloader-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.0/src/mikan/__init__.py
--rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.0/src/mikan/classes.py
--rw-r--r--   0        0        0     1491 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.0/src/mikan/config.py
--rw-r--r--   0        0        0     3294 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.0/src/mikan/downloader.py
--rw-r--r--   0        0        0     5958 2023-05-05 21:55:44.145052 mikan_card_downloader-1.1.0/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.1.0/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     2383 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.0/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.0/src/mikan/py.typed
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1041 2023-05-30 17:24:07.287889 mikan_card_downloader-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.1/src/mikan/__init__.py
+-rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.1/src/mikan/classes.py
+-rw-r--r--   0        0        0     1491 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.1/src/mikan/config.py
+-rw-r--r--   0        0        0     3294 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.1/src/mikan/downloader.py
+-rw-r--r--   0        0        0     5973 2023-05-30 17:19:50.146741 mikan_card_downloader-1.1.1/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.1.1/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     2383 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.1/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.1/src/mikan/py.typed
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.1.1/PKG-INFO
```

### Comparing `mikan_card_downloader-1.1.0/LICENSE` & `mikan_card_downloader-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.0/pyproject.toml` & `mikan_card_downloader-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "1.1.0"
+version = "1.1.1"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
```

### Comparing `mikan_card_downloader-1.1.0/src/mikan/classes.py` & `mikan_card_downloader-1.1.1/src/mikan/classes.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.0/src/mikan/config.py` & `mikan_card_downloader-1.1.1/src/mikan/config.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.0/src/mikan/downloader.py` & `mikan_card_downloader-1.1.1/src/mikan/downloader.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.0/src/mikan/html_parser.py` & `mikan_card_downloader-1.1.1/src/mikan/html_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,16 @@
 
             current_num += 1
 
     async def add_item_to_object_list(self, item: int) -> None:
         i, obj = await self.item_parser.create_item(
             await self.request_url_data(f"{self.img_type.url_template}{item}")
         )
-        self.objs[self.img_type.results_dir][i] = obj
-        print(f"Getting item {i}.")
+        self.objs[self.img_type.results_dir][str(item)] = obj
+        print(f"Getting item {item}.")
 
 
 class SIFListParser:
     def __init__(self) -> None:
         self.items: list[list[int]] = []
 
     async def get_page(self, num: Any) -> list[int]:
@@ -164,15 +164,15 @@
 
         raise ItemParsingException("An error occured while getting a card.")
 
 
 class StillParser:
     async def create_item(self, data: aiohttp.ClientResponse) -> tuple[str, list[str]]:
         page = bs4.BeautifulSoup(await data.text(), features="lxml")
-        pattern = re.compile(r"(\d+)")
+        pattern = re.compile(r"(.+)Still")
 
         if isinstance(top_item := page.find(class_="top-item"), bs4.Tag):
             links = top_item.find_all("a")
             url: str = links[0].get("href")
 
             if match := pattern.search(url.split("/")[-1]):
                 return match.group(1), [url]
```

### Comparing `mikan_card_downloader-1.1.0/src/mikan/json_utils.py` & `mikan_card_downloader-1.1.1/src/mikan/json_utils.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.0/src/mikan/main.py` & `mikan_card_downloader-1.1.1/src/mikan/main.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.0/PKG-INFO` & `mikan_card_downloader-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikan-card-downloader
-Version: 1.1.0
+Version: 1.1.1
 Summary: Downloads cards and stills from SIFAS and SIF.
 License: GPLv3
 Author: DemonicSavage
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

