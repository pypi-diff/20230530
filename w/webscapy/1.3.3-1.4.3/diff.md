# Comparing `tmp/webscapy-1.3.3.tar.gz` & `tmp/webscapy-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscapy-1.3.3.tar", last modified: Sun May 28 11:12:40 2023, max compression
+gzip compressed data, was "webscapy-1.4.3.tar", last modified: Tue May 30 01:32:34 2023, max compression
```

## Comparing `webscapy-1.3.3.tar` & `webscapy-1.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 11:12:40.482298 webscapy-1.3.3/
--rw-rw-rw-   0        0        0     4741 2023-05-28 11:12:40.480309 webscapy-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4446 2023-05-28 11:11:47.000000 webscapy-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 11:12:40.483303 webscapy-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-05-28 11:12:27.000000 webscapy-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:12:40.415587 webscapy-1.3.3/webscapy/
--rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.3.3/webscapy/__init__.py
--rw-rw-rw-   0        0        0     4177 2023-05-28 10:00:29.000000 webscapy-1.3.3/webscapy/webscapy.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:12:40.473299 webscapy-1.3.3/webscapy.egg-info/
--rw-rw-rw-   0        0        0     4741 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-28 11:12:40.000000 webscapy-1.3.3/webscapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 01:32:34.812758 webscapy-1.4.3/
+-rw-rw-rw-   0        0        0     5494 2023-05-30 01:32:34.812758 webscapy-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5199 2023-05-30 01:29:16.000000 webscapy-1.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 01:32:34.812758 webscapy-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-05-30 01:32:17.000000 webscapy-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 01:32:34.736556 webscapy-1.4.3/webscapy/
+-rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.4.3/webscapy/__init__.py
+-rw-rw-rw-   0        0        0     4458 2023-05-30 01:25:00.000000 webscapy-1.4.3/webscapy/webscapy.py
+drwxrwxrwx   0        0        0        0 2023-05-30 01:32:34.805158 webscapy-1.4.3/webscapy.egg-info/
+-rw-rw-rw-   0        0        0     5494 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/top_level.txt
```

### Comparing `webscapy-1.3.3/PKG-INFO` & `webscapy-1.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscapy
-Version: 1.3.3
+Version: 1.4.3
 Summary: Selenium built for scraping instead of testing
 Author: Rahul Raj
 Project-URL: Documentation, https://pypi.org/project/webscapy/
 Project-URL: Source, https://pypi.org/project/webscapy/
 Description-Content-Type: text/markdown
 
 # Webscapy: Selenium Configured for Webscraping
@@ -15,17 +15,17 @@
 
 ## Features
 
 1. <b>Automated Browser Interaction:</b> Webscapy enables you to automate browser actions, such as clicking buttons, filling forms, scrolling, and navigating between web pages. With a user-friendly interface, you can easily simulate human-like interactions with the target website.
 
 2. <b>Undetected Mode:</b> Webscapy includes built-in mechanisms to bypass anti-bot measures, including Cloudflare protection. It provides an undetected mode that reduces the chances of detection and allows for seamless scraping even from websites with strict security measures.
 
-   | Undetected Mode (Off) | Undetected Mode (On) |
-   | :-------------------: | :------------------: |
-   |        ![image](https://github.com/dusklight00/webscapy/assets/71203637/d8325500-3793-4f26-b7dd-15e5da7ee100)        |       ![image](https://github.com/dusklight00/webscapy/assets/71203637/7344470a-6924-4556-a72e-a27638e410bd)        |
+   |                                         Undetected Mode (Off)                                          |                                          Undetected Mode (On)                                          |
+   | :----------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
+   | ![image](https://github.com/dusklight00/webscapy/assets/71203637/d8325500-3793-4f26-b7dd-15e5da7ee100) | ![image](https://github.com/dusklight00/webscapy/assets/71203637/7344470a-6924-4556-a72e-a27638e410bd) |
 
 3. <b>Headless Browsers:</b> Webscapy supports headless browser operations, allowing you to scrape websites without displaying the browser window. This feature is useful for running scraping tasks in the background or on headless servers.
 
 4. <b>Element Load Waiting:</b> The package offers flexible options for waiting until specific elements are loaded on the web page. You can wait for elements to appear, disappear, or become interactable before performing further actions. This ensures that your scraping script synchronizes with the dynamic behavior of websites.
 
 5. <b>Execute JavaScript Code:</b> Webscapy allows you to execute custom JavaScript code within the browser. This feature enables you to interact with JavaScript-based functionalities on web pages, manipulate the DOM, or extract data that is not easily accessible through traditional scraping techniques.
 
@@ -109,24 +109,53 @@
 ```python
 ELEMENT_XPATH = "..."
 
 element = driver.load_element(ELEMENT_XPATH)
 element.click()
 ```
 
+## Execute Javascript Code
+
+You can execute any javascript code on the site using the following method
+
+```python
+code = "..."
+driver.execute_script(code)
+```
+
 ## Network Activity Data
 
 You can get network activity data after waiting for a while using commands like `time.sleep(...)`
 
 ```python
 network_data = driver.get_network_data()
 
 print(network_data)
 ```
 
+## Cookie Handling
+
+You can add cookies using the following method
+
+1. Add a single cookie
+
+```python
+cookie = {
+   "name": "cookie1",
+   "value": "value1"
+}
+driver.add_cookie(cookie)
+```
+
+2. Import cookie from JSON
+
+```
+driver.load_cookie_json("cookie.json")
+```
+
 ## Close the driver
 
 Always close the driver after using it to save memory, or avoid memory leaks
 
 ```python
 driver.close()
 ```
```

### Comparing `webscapy-1.3.3/README.md` & `webscapy-1.4.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 ## Features
 
 1. <b>Automated Browser Interaction:</b> Webscapy enables you to automate browser actions, such as clicking buttons, filling forms, scrolling, and navigating between web pages. With a user-friendly interface, you can easily simulate human-like interactions with the target website.
 
 2. <b>Undetected Mode:</b> Webscapy includes built-in mechanisms to bypass anti-bot measures, including Cloudflare protection. It provides an undetected mode that reduces the chances of detection and allows for seamless scraping even from websites with strict security measures.
 
-   | Undetected Mode (Off) | Undetected Mode (On) |
-   | :-------------------: | :------------------: |
-   |        ![image](https://github.com/dusklight00/webscapy/assets/71203637/d8325500-3793-4f26-b7dd-15e5da7ee100)        |       ![image](https://github.com/dusklight00/webscapy/assets/71203637/7344470a-6924-4556-a72e-a27638e410bd)        |
+   |                                         Undetected Mode (Off)                                          |                                          Undetected Mode (On)                                          |
+   | :----------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
+   | ![image](https://github.com/dusklight00/webscapy/assets/71203637/d8325500-3793-4f26-b7dd-15e5da7ee100) | ![image](https://github.com/dusklight00/webscapy/assets/71203637/7344470a-6924-4556-a72e-a27638e410bd) |
 
 3. <b>Headless Browsers:</b> Webscapy supports headless browser operations, allowing you to scrape websites without displaying the browser window. This feature is useful for running scraping tasks in the background or on headless servers.
 
 4. <b>Element Load Waiting:</b> The package offers flexible options for waiting until specific elements are loaded on the web page. You can wait for elements to appear, disappear, or become interactable before performing further actions. This ensures that your scraping script synchronizes with the dynamic behavior of websites.
 
 5. <b>Execute JavaScript Code:</b> Webscapy allows you to execute custom JavaScript code within the browser. This feature enables you to interact with JavaScript-based functionalities on web pages, manipulate the DOM, or extract data that is not easily accessible through traditional scraping techniques.
 
@@ -100,24 +100,53 @@
 ```python
 ELEMENT_XPATH = "..."
 
 element = driver.load_element(ELEMENT_XPATH)
 element.click()
 ```
 
+## Execute Javascript Code
+
+You can execute any javascript code on the site using the following method
+
+```python
+code = "..."
+driver.execute_script(code)
+```
+
 ## Network Activity Data
 
 You can get network activity data after waiting for a while using commands like `time.sleep(...)`
 
 ```python
 network_data = driver.get_network_data()
 
 print(network_data)
 ```
 
+## Cookie Handling
+
+You can add cookies using the following method
+
+1. Add a single cookie
+
+```python
+cookie = {
+   "name": "cookie1",
+   "value": "value1"
+}
+driver.add_cookie(cookie)
+```
+
+2. Import cookie from JSON
+
+```
+driver.load_cookie_json("cookie.json")
+```
+
 ## Close the driver
 
 Always close the driver after using it to save memory, or avoid memory leaks
 
 ```python
 driver.close()
 ```
```

### Comparing `webscapy-1.3.3/setup.py` & `webscapy-1.4.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="webscapy",
-    version="1.3.3",
+    version="1.4.3",
     description="Selenium built for scraping instead of testing",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Rahul Raj",
     packages=["webscapy"],
     zip_safe=False,
     project_urls={
```

### Comparing `webscapy-1.3.3/webscapy/webscapy.py` & `webscapy-1.4.3/webscapy/webscapy.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,89 +5,102 @@
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 from selenium.webdriver.chrome.options import Options
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.action_chains import ActionChains
 from webdriver_manager.chrome import ChromeDriverManager
 import undetected_chromedriver as uc
+import json
+
 
 class Webscapy:
-    def __init__(self, headless = True, executable_path = None, remote_url = None, undetected = False, version = None):
+    def __init__(
+        self,
+        headless=True,
+        executable_path=None,
+        remote_url=None,
+        undetected=False,
+        version=None,
+    ):
         self.setup_driver(headless, executable_path, remote_url, undetected, version)
 
-    def setup_driver(self, headless = True, executable_path = None, remote_url = None, undetected = False, version = None):
+    def setup_driver(
+        self,
+        headless=True,
+        executable_path=None,
+        remote_url=None,
+        undetected=False,
+        version=None,
+    ):
         if remote_url is not None:
             self.create_remote_driver(remote_url)
         else:
             if undetected:
                 self.create_undetected_driver(headless, executable_path, version)
             else:
                 self.create_offline_driver(headless, executable_path)
-    
-    def create_undetected_driver(self, headless = True, executable_path = None, version = None):
+
+    def create_undetected_driver(
+        self, headless=True, executable_path=None, version=None
+    ):
         if executable_path is None:
             chrome_manager = ChromeDriverManager()
             executable_path = chrome_manager.install()
-            version = int(chrome_manager.driver.get_browser_version_from_os().split(".")[0])
+            version = int(
+                chrome_manager.driver.get_browser_version_from_os().split(".")[0]
+            )
         elif version is None:
             raise Exception("Version of the executable path is not provided")
         options = uc.ChromeOptions()
         options.headless = headless
         self.driver = uc.Chrome(
             use_subprocess=True,
             driver_executable_path=executable_path,
             version_main=version,
-            options=options
+            options=options,
         )
 
-
-    def create_remote_driver(self, remote_url = None):
+    def create_remote_driver(self, remote_url=None):
         chrome_options = webdriver.ChromeOptions()
         chrome_options.set_capability("browserVersion", "67")
         chrome_options.set_capability("platformName", "Windows XP")
         self.driver = webdriver.Remote(
-            command_executor = remote_url, 
-            options = chrome_options
+            command_executor=remote_url, options=chrome_options
         )
 
-    def create_offline_driver(self, headless = True, executable_path = None):
+    def create_offline_driver(self, headless=True, executable_path=None):
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_argument("--log-level=3")
-        chrome_options.add_argument('--disable-gpu')
+        chrome_options.add_argument("--disable-gpu")
         if headless:
-            chrome_options.add_argument('--headless')
+            chrome_options.add_argument("--headless")
         service = Service(ChromeDriverManager().install())
         if executable_path is not None:
             self.driver = webdriver.Chrome(
-                service = service, 
-                options = chrome_options,
-                executable_path = executable_path
+                service=service, options=chrome_options, executable_path=executable_path
             )
         else:
-            self.driver = webdriver.Chrome(
-                service = service, 
-                options = chrome_options
-            )
+            self.driver = webdriver.Chrome(service=service, options=chrome_options)
 
     def load_wait(self, xpath):
         delay = 9999
         try:
             WebDriverWait(self.driver, delay).until(
                 EC.presence_of_element_located((By.XPATH, xpath))
             )
             return True
         except TimeoutException:
             return False
-    
+
     def load_element(self, xpath):
-        return self.driver.find_element('xpath', xpath)
+        return self.driver.find_element("xpath", xpath)
 
     def get(self, url):
         self.driver.get(url)
-    
+
     def get_network_data(self):
         network_data_retriever_script = """
             const performance = window.performance || 
                             window.mozPerformance || 
                             window.msPerformance || 
                             window.webkitPerformance || 
                             {};
@@ -96,10 +109,19 @@
 
             return network;
         """
 
         network_data = self.driver.execute_script(network_data_retriever_script)
 
         return network_data
-    
+
+    def add_cookie(self, cookie):
+        self.driver.add_cookie(cookie)
+
+    def load_cookie_json(self, path):
+        file = open(path, "r")
+        cookies = json.load(file)
+        for cookie in cookies:
+            self.add_cookie(cookie)
+
     def close(self):
-        self.driver.close()
+        self.driver.close()
```

### Comparing `webscapy-1.3.3/webscapy.egg-info/PKG-INFO` & `webscapy-1.4.3/webscapy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscapy
-Version: 1.3.3
+Version: 1.4.3
 Summary: Selenium built for scraping instead of testing
 Author: Rahul Raj
 Project-URL: Documentation, https://pypi.org/project/webscapy/
 Project-URL: Source, https://pypi.org/project/webscapy/
 Description-Content-Type: text/markdown
 
 # Webscapy: Selenium Configured for Webscraping
@@ -15,17 +15,17 @@
 
 ## Features
 
 1. <b>Automated Browser Interaction:</b> Webscapy enables you to automate browser actions, such as clicking buttons, filling forms, scrolling, and navigating between web pages. With a user-friendly interface, you can easily simulate human-like interactions with the target website.
 
 2. <b>Undetected Mode:</b> Webscapy includes built-in mechanisms to bypass anti-bot measures, including Cloudflare protection. It provides an undetected mode that reduces the chances of detection and allows for seamless scraping even from websites with strict security measures.
 
-   | Undetected Mode (Off) | Undetected Mode (On) |
-   | :-------------------: | :------------------: |
-   |        ![image](https://github.com/dusklight00/webscapy/assets/71203637/d8325500-3793-4f26-b7dd-15e5da7ee100)        |       ![image](https://github.com/dusklight00/webscapy/assets/71203637/7344470a-6924-4556-a72e-a27638e410bd)        |
+   |                                         Undetected Mode (Off)                                          |                                          Undetected Mode (On)                                          |
+   | :----------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
+   | ![image](https://github.com/dusklight00/webscapy/assets/71203637/d8325500-3793-4f26-b7dd-15e5da7ee100) | ![image](https://github.com/dusklight00/webscapy/assets/71203637/7344470a-6924-4556-a72e-a27638e410bd) |
 
 3. <b>Headless Browsers:</b> Webscapy supports headless browser operations, allowing you to scrape websites without displaying the browser window. This feature is useful for running scraping tasks in the background or on headless servers.
 
 4. <b>Element Load Waiting:</b> The package offers flexible options for waiting until specific elements are loaded on the web page. You can wait for elements to appear, disappear, or become interactable before performing further actions. This ensures that your scraping script synchronizes with the dynamic behavior of websites.
 
 5. <b>Execute JavaScript Code:</b> Webscapy allows you to execute custom JavaScript code within the browser. This feature enables you to interact with JavaScript-based functionalities on web pages, manipulate the DOM, or extract data that is not easily accessible through traditional scraping techniques.
 
@@ -109,24 +109,53 @@
 ```python
 ELEMENT_XPATH = "..."
 
 element = driver.load_element(ELEMENT_XPATH)
 element.click()
 ```
 
+## Execute Javascript Code
+
+You can execute any javascript code on the site using the following method
+
+```python
+code = "..."
+driver.execute_script(code)
+```
+
 ## Network Activity Data
 
 You can get network activity data after waiting for a while using commands like `time.sleep(...)`
 
 ```python
 network_data = driver.get_network_data()
 
 print(network_data)
 ```
 
+## Cookie Handling
+
+You can add cookies using the following method
+
+1. Add a single cookie
+
+```python
+cookie = {
+   "name": "cookie1",
+   "value": "value1"
+}
+driver.add_cookie(cookie)
+```
+
+2. Import cookie from JSON
+
+```
+driver.load_cookie_json("cookie.json")
+```
+
 ## Close the driver
 
 Always close the driver after using it to save memory, or avoid memory leaks
 
 ```python
 driver.close()
 ```
```

