# Comparing `tmp/IMDBTraktSyncer-1.3.5.tar.gz` & `tmp/IMDBTraktSyncer-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.3.5.tar", last modified: Sun May 28 13:21:32 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.3.6.tar", last modified: Mon May 29 23:51:47 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.3.5.tar` & `IMDBTraktSyncer-1.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 13:21:32.589567 IMDBTraktSyncer-1.3.5/
-drwxrwxrwx   0        0        0        0 2023-05-28 13:21:32.568568 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    22309 2023-05-25 05:33:53.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3858 2023-05-28 12:08:18.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     7752 2023-05-24 22:03:34.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:21:32.586566 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    11969 2023-05-28 13:21:32.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-28 13:21:32.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 13:21:32.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-28 13:21:32.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-28 13:21:32.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 13:21:32.000000 IMDBTraktSyncer-1.3.5/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.5/LICENSE
--rw-rw-rw-   0        0        0    11969 2023-05-28 13:21:32.588567 IMDBTraktSyncer-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    11226 2023-05-28 12:23:51.000000 IMDBTraktSyncer-1.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 13:21:32.589567 IMDBTraktSyncer-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-05-28 13:21:30.000000 IMDBTraktSyncer-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 23:51:47.634969 IMDBTraktSyncer-1.3.6/
+drwxrwxrwx   0        0        0        0 2023-05-29 23:51:47.601962 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    23224 2023-05-29 23:47:18.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3858 2023-05-28 12:08:18.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     7844 2023-05-29 23:40:21.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-29 23:51:47.631975 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    11969 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0    11969 2023-05-29 23:51:47.633976 IMDBTraktSyncer-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11226 2023-05-29 23:50:45.000000 IMDBTraktSyncer-1.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 23:51:47.634969 IMDBTraktSyncer-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-05-29 23:51:10.000000 IMDBTraktSyncer-1.3.6/setup.py
```

### Comparing `IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import SessionNotCreatedException
+from selenium.webdriver.common.action_chains import ActionChains
 try:
     from IMDBTraktSyncer import checkChromedriver
     from IMDBTraktSyncer import verifyCredentials as VC
     from IMDBTraktSyncer import traktData
     from IMDBTraktSyncer import imdbData
     from IMDBTraktSyncer import errorHandling as EH
 except ImportError:
@@ -39,14 +40,15 @@
         
         #Start web driver
         print('Starting webdriver...')
         options = Options()
         options.add_argument("--headless=new")
         options.add_argument('--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3')
         options.add_experimental_option("prefs", {"download.default_directory": directory, "download.directory_upgrade": True, "download.prompt_for_download": False, "credentials_enable_service": False, "profile.password_manager_enabled": False})
+        options.add_argument('--window-size=1920,1080')
         options.add_argument("--disable-save-password-bubble")
         options.add_argument("--disable-infobars")
         options.add_argument("--disable-autofill-for-password-fields")
         options.add_argument('--disable-notifications')
         options.add_argument("--disable-third-party-cookies")
         options.add_argument("--disable-dev-shm-usage")
         options.add_argument("--no-sandbox")
@@ -65,28 +67,28 @@
                 print(f"Error: {extract_message}")
                 print("See this link for details on how to fix: https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16")
                 raise SystemExit
             else:
                 raise
 
         wait = WebDriverWait(driver, 10)
-
+        
         driver.get('https://www.imdb.com/registration/signin')
 
         # wait for sign in link to appear and then click it
         sign_in_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'a.list-group-item > .auth-provider-text')))
         if 'IMDb' in sign_in_link.text:
             sign_in_link.click()
 
         # wait for email input field and password input field to appear, then enter credentials and submit
         email_input = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, "input[type='email']")))[0]
         password_input = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, "input[type='password']")))[0]
         email_input.send_keys(imdb_username)
         password_input.send_keys(imdb_password)
-        submit_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input[type='submit']")))
+        submit_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "input[type='submit']")))
         submit_button.click()
 
         time.sleep(2)
 
         # go to IMDB homepage
         driver.get('https://www.imdb.com/')
 
@@ -191,28 +193,33 @@
             # Set IMDB Watchlist Items
             if imdb_watchlist_to_set:
                 print('Setting IMDB Watchlist Items')
                 
                 # Count the total number of items
                 num_items = len(imdb_watchlist_to_set)
                 item_count = 0
-                
+                                
                 for item in imdb_watchlist_to_set:
                     try:
                         item_count += 1
                         year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
                         print(f"Adding item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist")
                         
                         driver.get(f'https://www.imdb.com/title/{item["ID"]}/')
-                                            
+                        
+                        # Scroll the page to bring the element into view
                         watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
+                        driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
+                        
+                        # Wait for the element to be clickable
+                        watchlist_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
                         
                         # Check if item is already in watchlist otherwise skip it
                         if 'ipc-icon--done' not in watchlist_button.get_attribute('innerHTML'):
-                            watchlist_button.click()
+                            driver.execute_script("arguments[0].click();", watchlist_button)
                             time.sleep(1)
                     except (NoSuchElementException, TimeoutException):
                         print(f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['ID']})")
                         pass
 
                 
                 print('Setting IMDB Watchlist Items Complete')
@@ -282,24 +289,28 @@
             print('Setting IMDB Ratings')
 
             # loop through each movie and TV show rating and submit rating on IMDB website
             for i, item in enumerate(imdb_ratings_to_set, 1):
                 year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
                 print(f'Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB')
                 driver.get(f'https://www.imdb.com/title/{item["ID"]}/')
+                
+                # Wait until rate button is located and scroll to it
+                button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
+                driver.execute_script("arguments[0].scrollIntoView(true);", button)
 
                 # click on "Rate" button and select rating option, then submit rating
-                button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button.ipc-btn span')))
+                button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
                 try:
                     element_rating_bar = button.find_element(By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating__unrated"]')
                     if element_rating_bar:
                         driver.execute_script("arguments[0].click();", button)
-                        rating_option_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
+                        rating_option_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
                         driver.execute_script("arguments[0].click();", rating_option_element)
-                        submit_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
+                        submit_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
                         submit_element.click()
                         time.sleep(1)
                 except (NoSuchElementException, TimeoutException):
                     print(f'Failed to rate {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB ({item["ID"]})')
                     pass
 
             print('Setting IMDB Ratings Complete')
@@ -378,34 +389,34 @@
                                 
                                 review_title_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.klondike-input")))
                                 review_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "textarea.klondike-textarea")))
                                 
                                 review_title_input.send_keys("My Review")
                                 review_input.send_keys(review["Comment"])
                                 
-                                no_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(2)")))
-                                yes_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(1)")))
+                                no_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(2)")))
+                                yes_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "ul.klondike-userreview-spoiler li:nth-child(1)")))
                                 
                                 if review["Spoiler"]:
                                     yes_element.click()                        
                                 else:
                                     no_element.click()
                                                         
-                                submit_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.a-button-input[type='submit']")))
+                                submit_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "input.a-button-input[type='submit']")))
 
                                 submit_button.click()
                                 
                                 time.sleep(3) # wait for rating to submit
                             except (NoSuchElementException, TimeoutException):
                                 print(f"Failed to submit review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB ({item['ID']})")
                                 pass
                         
                         print('Setting IMDB Reviews Complete')
                     else:
-                        print('IMDB reviews were submitted within the last 7 days. Skipping IMDB review submission.')
+                        print('IMDB reviews were submitted within the last 10 days. Skipping IMDB review submission.')
                 else:
                     print('No IMDB Reviews To Set')
             else:
                 print('There was an error getting IMDB reviews. See exception. Skipping reviews submissions.')
 
         #Close web driver
         print("Closing webdriver...")
```

### Comparing `IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/imdbData.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     print('Processing IMDB Data')
     
     #Get IMDB Watchlist Items
     try:
         driver.get('https://www.imdb.com/list/watchlist')
 
         csv_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".export a")))
+        driver.execute_script("arguments[0].scrollIntoView(true);", csv_link)
         csv_link.click()
 
         #Wait for csv download to complete
         time.sleep(8)
 
         imdb_watchlist = []
 
@@ -64,18 +65,18 @@
         imdb_watchlist = []
         pass
     
     # Get IMDB Ratings
     try:
         driver.get('https://www.imdb.com/list/ratings')
 
-        dropdown = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".circle")))
+        dropdown = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, ".circle")))
         dropdown.click()
 
-        csv_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".pop-up-menu-list-items a.pop-up-menu-list-item-link")))
+        csv_link = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, ".pop-up-menu-list-items a.pop-up-menu-list-item-link")))
         csv_link.click()
 
         #Wait for csv download to complete
         time.sleep(8)
 
         imdb_ratings = []
 
@@ -120,15 +121,15 @@
             if results:
                 media_type = results[0].get('type')
                 return media_type
         return None
 
     #Get IMDB Reviews
     driver.get('https://www.imdb.com/profile')
-    reviews_link = driver.find_element(By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")
+    reviews_link = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")))
     reviews_link.click()
 
     reviews = []
     errors_found_getting_imdb_reviews = False
     while True:
         try:
             try:
```

### Comparing `IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.5/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.5/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.5
+Version: 1.3.6
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.3.5/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.5/LICENSE` & `IMDBTraktSyncer-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.5/PKG-INFO` & `IMDBTraktSyncer-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.5
+Version: 1.3.6
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.3.5/README.md` & `IMDBTraktSyncer-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.5/setup.py` & `IMDBTraktSyncer-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.3.5'
+VERSION = '1.3.6'
 DESCRIPTION = 'This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

