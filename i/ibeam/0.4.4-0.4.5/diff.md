# Comparing `tmp/ibeam-0.4.4.tar.gz` & `tmp/ibeam-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ibeam-0.4.4.tar", last modified: Mon May 15 23:30:34 2023, max compression
+gzip compressed data, was "ibeam-0.4.5.tar", last modified: Tue May 30 17:45:19 2023, max compression
```

## Comparing `ibeam-0.4.4.tar` & `ibeam-0.4.5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.4.4/LICENSE
--rw-rw-rw-   0        0        0    10486 2023-05-15 23:30:34.000000 ibeam-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     9800 2022-08-31 12:47:22.000000 ibeam-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/ibeam/
--rw-rw-rw-   0        0        0       74 2023-05-15 18:50:41.000000 ibeam-0.4.4/ibeam/__init__.py
--rw-rw-rw-   0        0        0      349 2021-06-21 13:45:43.000000 ibeam-0.4.4/ibeam/config.py
--rw-rw-rw-   0        0        0     3850 2023-05-04 18:30:06.000000 ibeam-0.4.4/ibeam/ibeam_starter.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/ibeam/src/
--rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.4.4/ibeam/src/__init__.py
--rw-rw-rw-   0        0        0    19816 2023-05-09 19:20:47.000000 ibeam-0.4.4/ibeam/src/authenticate.py
--rw-rw-rw-   0        0        0    15614 2023-05-04 18:33:34.000000 ibeam-0.4.4/ibeam/src/gateway_client.py
--rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.4.4/ibeam/src/health_server.py
--rw-rw-rw-   0        0        0     7805 2023-05-04 18:33:34.000000 ibeam-0.4.4/ibeam/src/http_handler.py
--rw-rw-rw-   0        0        0     1314 2023-05-04 18:33:34.000000 ibeam-0.4.4/ibeam/src/inputs_handler.py
--rw-rw-rw-   0        0        0     1668 2022-04-07 12:15:07.000000 ibeam-0.4.4/ibeam/src/logs.py
--rw-rw-rw-   0        0        0     1851 2023-05-04 18:30:58.000000 ibeam-0.4.4/ibeam/src/process_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/
--rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/__init__.py
--rw-rw-rw-   0        0        0     2941 2021-06-21 13:45:43.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/external_request_handler.py
--rw-rw-rw-   0        0        0     5387 2023-05-04 18:33:34.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/google_msg_handler.py
--rw-rw-rw-   0        0        0     2975 2023-05-03 22:42:05.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/notification_resend_handler.py
--rw-rw-rw-   0        0        0      264 2021-06-21 13:45:43.000000 ibeam-0.4.4/ibeam/src/two_fa_handlers/two_fa_handler.py
--rw-rw-rw-   0        0        0     2682 2023-04-01 23:25:13.000000 ibeam-0.4.4/ibeam/src/two_fa_selector.py
--rw-rw-rw-   0        0        0     6087 2023-05-03 22:26:29.000000 ibeam-0.4.4/ibeam/src/var.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:30:34.000000 ibeam-0.4.4/ibeam.egg-info/
--rw-rw-rw-   0        0        0    10486 2023-05-15 23:30:32.000000 ibeam-0.4.4/ibeam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-05-15 23:30:33.000000 ibeam-0.4.4/ibeam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 23:30:32.000000 ibeam-0.4.4/ibeam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-05-15 23:30:32.000000 ibeam-0.4.4/ibeam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 23:30:32.000000 ibeam-0.4.4/ibeam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-15 23:30:34.000000 ibeam-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1378 2022-04-07 12:19:21.000000 ibeam-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.555596 ibeam-0.4.5/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0    10463 2023-05-30 17:45:19.555596 ibeam-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9800 2022-08-31 12:47:22.000000 ibeam-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.445764 ibeam-0.4.5/ibeam/
+-rw-rw-rw-   0        0        0       74 2023-05-30 17:03:40.000000 ibeam-0.4.5/ibeam/__init__.py
+-rw-rw-rw-   0        0        0      349 2021-06-21 13:45:43.000000 ibeam-0.4.5/ibeam/config.py
+-rw-rw-rw-   0        0        0     3850 2023-05-04 18:30:06.000000 ibeam-0.4.5/ibeam/ibeam_starter.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.524350 ibeam-0.4.5/ibeam/src/
+-rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.4.5/ibeam/src/__init__.py
+-rw-rw-rw-   0        0        0    20947 2023-05-23 19:26:05.000000 ibeam-0.4.5/ibeam/src/authenticate.py
+-rw-rw-rw-   0        0        0    15619 2023-05-16 12:49:10.000000 ibeam-0.4.5/ibeam/src/gateway_client.py
+-rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.4.5/ibeam/src/health_server.py
+-rw-rw-rw-   0        0        0     7805 2023-05-04 18:33:34.000000 ibeam-0.4.5/ibeam/src/http_handler.py
+-rw-rw-rw-   0        0        0     1314 2023-05-04 18:33:34.000000 ibeam-0.4.5/ibeam/src/inputs_handler.py
+-rw-rw-rw-   0        0        0     1668 2022-04-07 12:15:07.000000 ibeam-0.4.5/ibeam/src/logs.py
+-rw-rw-rw-   0        0        0     1851 2023-05-04 18:30:58.000000 ibeam-0.4.5/ibeam/src/process_utils.py
+-rw-rw-rw-   0        0        0      305 2023-05-23 18:02:24.000000 ibeam-0.4.5/ibeam/src/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.539973 ibeam-0.4.5/ibeam/src/two_fa_handlers/
+-rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/__init__.py
+-rw-rw-rw-   0        0        0     2941 2021-06-21 13:45:43.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/external_request_handler.py
+-rw-rw-rw-   0        0        0     5387 2023-05-04 18:33:34.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/google_msg_handler.py
+-rw-rw-rw-   0        0        0     2975 2023-05-03 22:42:05.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/notification_resend_handler.py
+-rw-rw-rw-   0        0        0      264 2021-06-21 13:45:43.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/two_fa_handler.py
+-rw-rw-rw-   0        0        0     2682 2023-04-01 23:25:13.000000 ibeam-0.4.5/ibeam/src/two_fa_selector.py
+-rw-rw-rw-   0        0        0     6087 2023-05-03 22:26:29.000000 ibeam-0.4.5/ibeam/src/var.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.477018 ibeam-0.4.5/ibeam.egg-info/
+-rw-rw-rw-   0        0        0    10463 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-30 17:45:19.555596 ibeam-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1378 2023-05-16 19:48:03.000000 ibeam-0.4.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ibeam-0.4.4/LICENSE` & `ibeam-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/PKG-INFO` & `ibeam-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.4.4
+Version: 0.4.5
 Summary: IBeam is an authentication and maintenance tool used for the Interactive Brokers Client Portal Web API Gateway.
 Home-page: https://github.com/Voyz/ibeam
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: interactive brokers,algo trading,algorithmic trading,data flow,quant,trading
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -255,9 +254,7 @@
 [advanced-secrets]: https://github.com/Voyz/ibeam/wiki/Advanced-Secrets
 
 [troubleshooting]: https://github.com/Voyz/ibeam/wiki/Troubleshooting
 
 [issues]: https://github.com/Voyz/ibeam/issues
 
 [gateway]: https://interactivebrokers.github.io/cpwebapi/
-
-
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: ibeam Version: 0.4.4 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.4.5 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
-brokers,algo trading,algorithmic trading,data flow,quant,trading Platform:
-UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown License-File: LICENSE *This library is
-currently being beta-tested. See something that's broken? Did we get something
-wrong? [Create an issue and let us know!][issues]*
+brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
+text/markdown License-File: LICENSE *This library is currently being beta-
+tested. See something that's broken? Did we get something wrong? [Create an
+issue and let us know!][issues]*
                                  [IBeam_logo]
     [https://img.shields.io/badge/License-Apache%202.0-blue.svg] [https://
                   img.shields.io/pypi/v/ibeam?label=version]
 IBeam is an authentication and maintenance tool used for the [Interactive
 Brokers Client Portal Web API Gateway.][gateway] Features: * **Facilitates
 continuous headless run of the Gateway.** * **No physical display required** -
 virtual display buffer can be used instead. * **No interaction from the user
```

### Comparing `ibeam-0.4.4/README.md` & `ibeam-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/ibeam_starter.py` & `ibeam-0.4.5/ibeam/ibeam_starter.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/authenticate.py` & `ibeam-0.4.5/ibeam/src/authenticate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import os
 import sys
 import time
-import traceback
 from datetime import datetime
 from pathlib import Path
 import tempfile
 from typing import Union, Optional
 
 from cryptography.fernet import Fernet
 from pyvirtualdisplay import Display
@@ -16,14 +15,15 @@
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support.ui import Select
 
 import ibeam
 from ibeam.src import var
+from ibeam.src.py_utils import exception_to_string
 from ibeam.src.two_fa_handlers.two_fa_handler import TwoFaHandler
 
 _LOGGER = logging.getLogger('ibeam.' + Path(__file__).stem)
 
 _DRIVER_NAMES = {}
 _FAILED_ATTEMPTS = 0
 
@@ -56,14 +56,15 @@
         options.add_argument("--incognito")  # this allows 2FA method to be selected every time
     options.add_argument('--ignore-ssl-errors=yes')
     options.add_argument('--ignore-certificate-errors')
     options.add_argument(f'--remote-debugging-port={9222 + driver_index}')
     options.add_argument('--useAutomationExtension=false')
     options.add_argument('--disable-extensions')
     options.add_argument('--dns-prefetch-disable')
+    options.add_argument('--disable-features=VizDisplayCompositor')
     options.add_argument(f'--user-data-dir={tempfile.gettempdir()}/ibeam-chrome-{name}')
     driver = webdriver.Chrome(driver_path, options=options)
     if driver is None:
         _LOGGER.error('Unable to create a new chrome driver.')
 
     return driver
 
@@ -83,15 +84,15 @@
             locators = locators
         self.locators = locators
         self.text = text_
 
     def __call__(self, driver):
         for locator in self.locators:
             try:
-                element = EC._find_element(driver, locator)
+                element = driver.find_element(*locator)
                 if self.text in element.text:
                     return element
             except StaleElementReferenceException:
                 continue
         return False
 
 
@@ -167,15 +168,14 @@
     """ Check for the IBRK website version. Currently, there are various versions shown to users and we want to know which one we are operating on.
 
     Versions:
 
     * 1 = available until March 2023
     * 2 = available from March 2023
     """
-
     try:
         user_name_present = EC.presence_of_element_located((By.NAME, 'user_name'))
         WebDriverWait(driver, 5).until(user_name_present)
         return 1
     except TimeoutException as e:
         pass
 
@@ -200,18 +200,21 @@
     elements['SUCCESS_EL_TEXT'] = var.SUCCESS_EL_TEXT
     elements['IBKEY_PROMO_EL_CLASS'] = var.IBKEY_PROMO_EL_CLASS
     elements['TWO_FA_EL_ID'] = var.TWO_FA_EL_ID
     elements['TWO_FA_NOTIFICATION_EL'] = var.TWO_FA_NOTIFICATION_EL
     elements['TWO_FA_INPUT_EL_ID'] = var.TWO_FA_INPUT_EL_ID
     elements['TWO_FA_SELECT_EL_ID'] = var.TWO_FA_SELECT_EL_ID
 
-    if var.USER_NAME_EL is not None:
+
+    if var.USER_NAME_EL is not None and var.USER_NAME_EL != elements['USER_NAME_EL']:
+        _LOGGER.warning(f'USER_NAME_EL is forced to "{var.USER_NAME_EL}", contrary to the element found on the website: "{elements["USER_NAME_EL"]}"')
         elements['USER_NAME_EL'] = var.USER_NAME_EL
 
-    if var.ERROR_EL is not None:
+    if var.ERROR_EL is not None and var.ERROR_EL != elements['ERROR_EL']:
+        _LOGGER.warning(f'ERROR_EL is forced to "{var.ERROR_EL}", contrary to the element found on the website: "{elements["ERROR_EL"]}"')
         elements['ERROR_EL'] = var.ERROR_EL
 
     return elements
 
 
 def authenticate_gateway(driver_path,
                          account,
@@ -230,29 +233,32 @@
     :return: Whether authentication was successful and whether IBeam should shut down
     :rtype: (bool, bool)
     """
     base_url = base_url if base_url is not None else var.GATEWAY_BASE_URL
     display = None
     success = False
     driver = None
+    website_version = -1
+    elements = {}
     try:
         _LOGGER.info(f'Loading auth webpage at {base_url + var.ROUTE_AUTH}')
         if sys.platform == 'linux':
-            display = Display(visible=0, size=(800, 600))
+            display = Display(visible=False, size=(800, 600))
             display.start()
 
         driver = start_driver(base_url, driver_path)
         if driver is None:
             return False, False
 
         driver.get(base_url + var.ROUTE_AUTH)
 
         website_version = check_version(driver)
 
         elements = create_elements(_VERSIONS[website_version])
+        _LOGGER.debug(f'Elements: {elements}')
 
         # wait for the page to load
         user_name_present = EC.presence_of_element_located((By.NAME, elements['USER_NAME_EL']))
         WebDriverWait(driver, 15).until(user_name_present)
         _LOGGER.info('Gateway auth webpage loaded')
 
         immediate_attempts = 0
@@ -260,30 +266,30 @@
         while immediate_attempts < max(var.MAX_IMMEDIATE_ATTEMPTS, 1):
             immediate_attempts += 1
             _LOGGER.info(f'Login attempt number {immediate_attempts}')
 
             # time.sleep(300)
 
             # input credentials
-            user_name_el = driver.find_element_by_name(elements['USER_NAME_EL'])
-            password_el = driver.find_element_by_name(elements['PASSWORD_EL'])
+            user_name_el = driver.find_element(By.NAME, elements['USER_NAME_EL'])
+            password_el = driver.find_element(By.NAME, elements['PASSWORD_EL'])
             user_name_el.send_keys(account)
 
             if key is None:
                 password_el.send_keys(password)
             else:
                 password_el.send_keys(Fernet(key).decrypt(password.encode('utf-8')).decode("utf-8"))
 
             password_el.send_keys(Keys.TAB)
 
             # small buffer to prevent race-condition on client side
             time.sleep(5)
             # submit the form
             _LOGGER.info('Submitting the form')
-            submit_form_el = driver.find_element_by_css_selector(elements['SUBMIT_EL'])
+            submit_form_el = driver.find_element(By.CSS_SELECTOR, elements['SUBMIT_EL'])
             submit_form_el.click()
 
             # observe results - either success or 2FA request
             success_present = text_to_be_present_in_element([(By.TAG_NAME, 'pre'), (By.TAG_NAME, 'body')],
                                                             elements['SUCCESS_EL_TEXT'])
             two_factor_input_present = EC.visibility_of_element_located((By.ID, elements['TWO_FA_EL_ID']))
 
@@ -303,15 +309,15 @@
                        ibkey_promo_skip_clickable))
 
             trigger_identifier = identify_trigger(trigger, elements)
             _LOGGER.debug(f'trigger: {trigger_identifier}')
 
             if trigger_identifier == elements['TWO_FA_SELECT_EL_ID']:
                 _LOGGER.info(f'Required to select a 2FA method.')
-                select_el = driver.find_element_by_id(elements['TWO_FA_SELECT_EL_ID'])
+                select_el = driver.find_element(By.ID, elements['TWO_FA_SELECT_EL_ID'])
                 select = Select(select_el)
                 select.select_by_visible_text(var.TWO_FA_SELECT_TARGET)
 
                 trigger = WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
                     any_of(success_present,
                            two_factor_input_present,
                            two_factor_notification,
@@ -345,21 +351,21 @@
                     return False, True
 
                 two_fa_code = handle_two_fa(two_fa_handler)
 
                 if two_fa_code is None:
                     _LOGGER.warning(f'No 2FA code returned. Aborting authentication.')
                 else:
-                    two_fa_el = driver.find_elements_by_id(elements['TWO_FA_INPUT_EL_ID'])
+                    two_fa_el = driver.find_elements(By.ID, elements['TWO_FA_INPUT_EL_ID'])
                     WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
                         EC.element_to_be_clickable((By.ID, elements['TWO_FA_INPUT_EL_ID'])))
                     two_fa_el[0].send_keys(two_fa_code)
 
                     _LOGGER.info('Submitting the 2FA form')
-                    submit_form_el = driver.find_element_by_css_selector(elements['SUBMIT_EL'])
+                    submit_form_el = driver.find_element(By.CSS_SELECTOR, elements['SUBMIT_EL'])
                     WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
                         EC.element_to_be_clickable((By.CSS_SELECTOR, elements['SUBMIT_EL'])))
                     submit_form_el.click()
 
                     trigger = WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
                         any_of(success_present, ibkey_promo_skip_clickable, error_displayed))
                     trigger_identifier = identify_trigger(trigger, elements)
@@ -398,17 +404,23 @@
                 _LOGGER.info('Webpage displayed "Client login succeeds"')
                 _FAILED_ATTEMPTS = 0
                 success = True
                 break
 
         time.sleep(2)
     except TimeoutException as e:
-        exception_line = traceback.format_tb(sys.exc_info()[2])[0].replace('\n', '')
-        _LOGGER.error(
-            f'Timeout reached when waiting for authentication. Consider increasing IBEAM_PAGE_LOAD_TIMEOUT. Error: "{e.msg}" at {exception_line}')
+
+        try:
+            website_loaded = EC.presence_of_element_located((By.CLASS_NAME, 'login'))
+            WebDriverWait(driver, 5).until(website_loaded)
+        except TimeoutException as ee:
+            _LOGGER.error(f'Timeout reached when waiting for authentication. The website seems to not be loaded correctly. Consider increasing IBEAM_PAGE_LOAD_TIMEOUT. \nWebsite URL: {base_url + var.ROUTE_AUTH} \nIBEAM_PAGE_LOAD_TIMEOUT: {var.PAGE_LOAD_TIMEOUT} \nException:\n{exception_to_string(e)}')
+        else:
+            _LOGGER.error(f'Timeout reached searching for website elements, but the website seems to be loaded correctly. It is possible the setup is incorrect. \nWebsite version: {website_version} \nDOM elements searched for: {elements}. \nException:\n{exception_to_string(e)}')
+
         save_screenshot(driver, '__timeout-exception')
         success = False
     except Exception as e:
         try:
             raise RuntimeError('Error encountered during authentication') from e
         except Exception as full_e:
             _LOGGER.exception(full_e)
```

### Comparing `ibeam-0.4.4/ibeam/src/gateway_client.py` & `ibeam-0.4.5/ibeam/src/gateway_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         self._scheduler.start()
         try:
             while True:
                 time.sleep(1)
         except KeyboardInterrupt as e:
             _LOGGER.info('Keyboard interrupt, shutting down.')
             pass
-        self._scheduler.shutdown(False)
+        self._scheduler.shutdown(wait=False)
 
     def _maintenance(self):
         _LOGGER.info('Maintenance')
 
         success, shutdown = self.start_and_authenticate(request_retries=var.REQUEST_RETRIES)
 
         if shutdown:
```

### Comparing `ibeam-0.4.4/ibeam/src/health_server.py` & `ibeam-0.4.5/ibeam/src/health_server.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/http_handler.py` & `ibeam-0.4.5/ibeam/src/http_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/inputs_handler.py` & `ibeam-0.4.5/ibeam/src/inputs_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/logs.py` & `ibeam-0.4.5/ibeam/src/logs.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/process_utils.py` & `ibeam-0.4.5/ibeam/src/process_utils.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/two_fa_handlers/external_request_handler.py` & `ibeam-0.4.5/ibeam/src/two_fa_handlers/external_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/two_fa_handlers/google_msg_handler.py` & `ibeam-0.4.5/ibeam/src/two_fa_handlers/google_msg_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/two_fa_handlers/notification_resend_handler.py` & `ibeam-0.4.5/ibeam/src/two_fa_handlers/notification_resend_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/two_fa_selector.py` & `ibeam-0.4.5/ibeam/src/two_fa_selector.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam/src/var.py` & `ibeam-0.4.5/ibeam/src/var.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.4/ibeam.egg-info/PKG-INFO` & `ibeam-0.4.5/ibeam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.4.4
+Version: 0.4.5
 Summary: IBeam is an authentication and maintenance tool used for the Interactive Brokers Client Portal Web API Gateway.
 Home-page: https://github.com/Voyz/ibeam
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: interactive brokers,algo trading,algorithmic trading,data flow,quant,trading
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -255,9 +254,7 @@
 [advanced-secrets]: https://github.com/Voyz/ibeam/wiki/Advanced-Secrets
 
 [troubleshooting]: https://github.com/Voyz/ibeam/wiki/Troubleshooting
 
 [issues]: https://github.com/Voyz/ibeam/issues
 
 [gateway]: https://interactivebrokers.github.io/cpwebapi/
-
-
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: ibeam Version: 0.4.4 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.4.5 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
-brokers,algo trading,algorithmic trading,data flow,quant,trading Platform:
-UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown License-File: LICENSE *This library is
-currently being beta-tested. See something that's broken? Did we get something
-wrong? [Create an issue and let us know!][issues]*
+brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
+text/markdown License-File: LICENSE *This library is currently being beta-
+tested. See something that's broken? Did we get something wrong? [Create an
+issue and let us know!][issues]*
                                  [IBeam_logo]
     [https://img.shields.io/badge/License-Apache%202.0-blue.svg] [https://
                   img.shields.io/pypi/v/ibeam?label=version]
 IBeam is an authentication and maintenance tool used for the [Interactive
 Brokers Client Portal Web API Gateway.][gateway] Features: * **Facilitates
 continuous headless run of the Gateway.** * **No physical display required** -
 virtual display buffer can be used instead. * **No interaction from the user
```

### Comparing `ibeam-0.4.4/ibeam.egg-info/SOURCES.txt` & `ibeam-0.4.5/ibeam.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ibeam/src/authenticate.py
 ibeam/src/gateway_client.py
 ibeam/src/health_server.py
 ibeam/src/http_handler.py
 ibeam/src/inputs_handler.py
 ibeam/src/logs.py
 ibeam/src/process_utils.py
+ibeam/src/py_utils.py
 ibeam/src/two_fa_selector.py
 ibeam/src/var.py
 ibeam/src/two_fa_handlers/__init__.py
 ibeam/src/two_fa_handlers/external_request_handler.py
 ibeam/src/two_fa_handlers/google_msg_handler.py
 ibeam/src/two_fa_handlers/notification_resend_handler.py
 ibeam/src/two_fa_handlers/two_fa_handler.py
```

### Comparing `ibeam-0.4.4/setup.py` & `ibeam-0.4.5/setup.py`

 * *Files identical despite different names*

