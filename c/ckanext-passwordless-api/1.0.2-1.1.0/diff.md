# Comparing `tmp/ckanext-passwordless-api-1.0.2.tar.gz` & `tmp/ckanext-passwordless-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-passwordless-api-1.0.2.tar", last modified: Mon Apr  3 18:54:14 2023, max compression
+gzip compressed data, was "ckanext-passwordless-api-1.1.0.tar", last modified: Tue May 30 17:45:10 2023, max compression
```

## Comparing `ckanext-passwordless-api-1.0.2.tar` & `ckanext-passwordless-api-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1184 2023-04-03 18:53:55.333785 ckanext-passwordless-api-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1060 2023-02-27 14:49:50.624520 ckanext-passwordless-api-1.0.2/LICENSE
--rw-r--r--   0        0        0     6466 2023-04-03 18:09:43.437296 ckanext-passwordless-api-1.0.2/README.md
--rw-r--r--   0        0        0      230 2023-02-27 14:49:50.624520 ckanext-passwordless-api-1.0.2/ckanext/__init__.py
--rw-r--r--   0        0        0      235 2023-02-27 14:49:50.624520 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/__init__.py
--rw-r--r--   0        0        0       43 2023-04-03 18:53:55.337785 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/__version__.py
--rw-r--r--   0        0        0    11568 2023-04-03 18:53:55.337785 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/logic.py
--rw-r--r--   0        0        0     2403 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/mailer.py
--rw-r--r--   0        0        0     4205 2023-04-03 18:09:43.437296 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/plugin.py
--rw-r--r--   0        0        0      488 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/templates/reset_key.txt
--rw-r--r--   0        0        0     1014 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/templates/welcome_user.txt
--rw-r--r--   0        0        0       49 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/tests/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-03 18:09:43.437296 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/tests/test_plugin.py
--rw-r--r--   0        0        0     7159 2023-04-03 18:09:43.437296 ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/util.py
--rw-r--r--   0        0        0     2203 2023-04-03 18:53:55.337785 ckanext-passwordless-api-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     7312 1970-01-01 00:00:00.000000 ckanext-passwordless-api-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1416 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1060 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7054 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/README.md
+-rw-r--r--   0        0        0      230 2023-02-27 14:49:50.624520 ckanext-passwordless-api-1.1.0/ckanext/__init__.py
+-rw-r--r--   0        0        0      235 2023-02-27 14:49:50.624520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/__version__.py
+-rw-r--r--   0        0        0    13137 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/logic.py
+-rw-r--r--   0        0        0     2403 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/mailer.py
+-rw-r--r--   0        0        0     4268 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/plugin.py
+-rw-r--r--   0        0        0      488 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/templates/reset_key.txt
+-rw-r--r--   0        0        0     1014 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/templates/welcome_user.txt
+-rw-r--r--   0        0        0       49 2023-02-27 14:49:50.628520 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/tests/__init__.py
+-rw-r--r--   0        0        0     1430 2023-04-03 18:09:43.437296 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/tests/test_plugin.py
+-rw-r--r--   0        0        0     7658 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/util.py
+-rw-r--r--   0        0        0     2203 2023-05-30 17:44:50.322838 ckanext-passwordless-api-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7900 1970-01-01 00:00:00.000000 ckanext-passwordless-api-1.1.0/PKG-INFO
```

### Comparing `ckanext-passwordless-api-1.0.2/CHANGELOG.md` & `ckanext-passwordless-api-1.1.0/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+## 1.1.0 (2023-05-30)
+
+### Feat
+
+- add option to anonymise usernames
+- add introspect endpoint, verify token only
+
+### Refactor
+
+- improve log message for when user is deleted
+- tweak to plugin init logic
+- correct link to license
+
 ## 1.0.2 (2023-04-03)
 
 ### Fix
 
 - remove ckan.types until upgrade 2.10
 
 ## 1.0.1 (2023-04-03)
```

### Comparing `ckanext-passwordless-api-1.0.2/LICENSE` & `ckanext-passwordless-api-1.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 WSL
+Copyright (c) 2023 WSL
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ckanext-passwordless-api-1.0.2/README.md` & `ckanext-passwordless-api-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 <div align="center">
   <a href="https://pypi.org/project/ckanext-passwordless_api" target="_blank">
       <img src="https://img.shields.io/pypi/v/ckanext-passwordless_api?color=%2334D058&label=pypi%20package" alt="Package version">
   </a>
   <a href="https://pypistats.org/packages/ckanext-passwordless_api" target="_blank">
       <img src="https://img.shields.io/pypi/dm/ckanext-passwordless_api.svg" alt="Downloads">
   </a>
-  <a href="https://gitlabext.wsl.ch/EnviDat/ckanext-passwordless_api/-/raw/main/LICENCE" target="_blank">
+  <a href="https://gitlabext.wsl.ch/EnviDat/ckanext-passwordless_api/-/raw/main/LICENSE" target="_blank">
       <img src="https://img.shields.io/github/license/EnviDat/ckanext-passwordless_api.svg" alt="Licence">
   </a>
 </div>
 
 ---
 
 **Documentation**: <a href="https://envidat.gitlab-pages.wsl.ch/ckanext-passwordless_api/" target="_blank">https://envidat.gitlab-pages.wsl.ch/ckanext-passwordless_api/</a>
@@ -75,22 +75,28 @@
   - Default: None, samesite value is set to `Lax`.
 - **passwordless_api.cookie_http_only**
   - Description: Use a httpOnly cookie, recommended.
   - Default: true.
 - **passwordless_api.cookie_path**
   - Description: Set a specific path to use the cookie, e.g. `/api`.
   - Default: `/` (all paths).
+- **passwordless_api.anonymous_usernames**
+  - Description: Set to true to anonymise usernames when generated.
+  - Default: false.
+- **passwordless_api.anonymous_domain_exceptions**
+  - Description: Email domain exceptions that should not be anonymised, if enabled.
+  - Default: None.
 
 ## Endpoints
 
 **POST**
 
 - **<CKAN_HOST>/api/3/action/passwordless_request_reset_key**
   - Description: Request a login token for a given email.
-  - Creates user if they do not exist & sends welcome email.
+    - Creates user if they do not exist & sends welcome email.
   - Param1: email (str).
 - **<CKAN_HOST>/api/3/action/passwordless_request_api_token**
   - Description: Request an API token, given the email and login token (reset_key).
   - Param1: email (str).
   - Param2: key (str).
 - **<CKAN_HOST>/api/3/action/passwordless_request_api_token_azure_ad**
   - Description: Request an API token, given the email and Azure AD token.
@@ -102,16 +108,21 @@
 
 **GET**
 
 - **<CKAN_HOST>/api/3/action/passwordless_revoke_api_token**
   - Description: If logged in, revoke the current API token.
 - **<CKAN_HOST>/api/3/action/passwordless_get_user**
   - Description: Get user details, given their API token.
-    Also resets and returns a new API token (i.e. renewal).
-    Fails silently if the user is not logged in.
+    - Also resets and returns a new API token (i.e. renewal).
+    - Fails silently if the user is not logged in.
+    - Use the core `user_show` action if refresh is not required.
+- **<CKAN_HOST>/api/3/action/passwordless_introspect**
+  - Description: Verify if the API token is valid for a user.
+    - This does not renew the token in the same call.
+    - Mostly useful for auth checking in microservice APIs.
 
 ## Using the cookie in an Authorization header
 
 If configured, the cookie containing an API token can't do much on it's own.
 
 It is possible to extract the cookie value using frontend JS and pass to the CKAN backend, but this makes your site vulnerable to XSS attacks.
```

#### html2text {}

```diff
@@ -31,46 +31,53 @@
 respect, required if cookie set. - Default: None. -
 **passwordless_api.cookie_samesite** - Description: To change the cookie
 samesite value to `Strict`. Only enable this if you know what you are doing. -
 Default: None, samesite value is set to `Lax`. -
 **passwordless_api.cookie_http_only** - Description: Use a httpOnly cookie,
 recommended. - Default: true. - **passwordless_api.cookie_path** - Description:
 Set a specific path to use the cookie, e.g. `/api`. - Default: `/` (all paths).
-## Endpoints **POST** - **/api/3/action/passwordless_request_reset_key** -
+- **passwordless_api.anonymous_usernames** - Description: Set to true to
+anonymise usernames when generated. - Default: false. -
+**passwordless_api.anonymous_domain_exceptions** - Description: Email domain
+exceptions that should not be anonymised, if enabled. - Default: None. ##
+Endpoints **POST** - **/api/3/action/passwordless_request_reset_key** -
 Description: Request a login token for a given email. - Creates user if they do
 not exist & sends welcome email. - Param1: email (str). - **/api/3/action/
 passwordless_request_api_token** - Description: Request an API token, given the
 email and login token (reset_key). - Param1: email (str). - Param2: key (str).
 - **/api/3/action/passwordless_request_api_token_azure_ad** - Description:
 Request an API token, given the email and Azure AD token. - Param1: email
 (str). - Param2: token (str). - **/api/3/action/passwordless_revoke_api_token**
 - Description: Revoke an API token. - Param1: token (str). **GET** - **/api/3/
 action/passwordless_revoke_api_token** - Description: If logged in, revoke the
 current API token. - **/api/3/action/passwordless_get_user** - Description: Get
-user details, given their API token. Also resets and returns a new API token
-(i.e. renewal). Fails silently if the user is not logged in. ## Using the
-cookie in an Authorization header If configured, the cookie containing an API
-token can't do much on it's own. It is possible to extract the cookie value
-using frontend JS and pass to the CKAN backend, but this makes your site
-vulnerable to XSS attacks. Instead the cookie should be stored in a secure way:
-- `samesite=Lax` with `domain=YOUR_DOMAIN` to help prevent CSRF. -
-`samesite=Strict` is even more secure, but significantly impacts UX for your
-site. - `secure` to help prevent man-in-the-middle. - `httpOnly` to help
-prevent XSS. - Setting this means the cookie can no longer be accessed from
-your JS code. Then a middleware must be used to convert the cookie value into a
-header than CKAN can interpret: **NGINX server example** (nginx is the default/
-recommended server to reverse proxy CKAN) (https://docs.ckan.org/en/latest/
-maintaining/installing/deployment.html) ```nginx # Add the cookie-based API
-token to the request Authorization header # This is passed to the CKAN backend
-& read automatically by CKAN proxy_set_header 'Authorization' $cookie_$
-{AUTH_COOKIE_NAME}; # If using caching omit the cookie proxy_cache_bypass
-$cookie_${AUTH_COOKIE_NAME}; proxy_no_cache $cookie_${AUTH_COOKIE_NAME}; ```
-**Apache server example** ```apache SetEnvIf Cookie "(^|;\ *)$
-{AUTH_COOKIE_NAME}=([^;\ ]+)" ckan_cookie_value=$2 RequestHeader set
-Authorization "%{ckan_cookie_value}e" ``` ## Notes - It is also recommended to
-disable access to the API via cookie, to help prevent CSRF:
-`ckan.auth.disable_cookie_auth_in_api = true` - The configuration for API
-tokens can be configured in core: ```ini api_token.nbytes = 60
-api_token.jwt.decode.secret = string:YOUR_SUPER_SECRET_STRING
+user details, given their API token. - Also resets and returns a new API token
+(i.e. renewal). - Fails silently if the user is not logged in. - Use the core
+`user_show` action if refresh is not required. - **/api/3/action/
+passwordless_introspect** - Description: Verify if the API token is valid for a
+user. - This does not renew the token in the same call. - Mostly useful for
+auth checking in microservice APIs. ## Using the cookie in an Authorization
+header If configured, the cookie containing an API token can't do much on it's
+own. It is possible to extract the cookie value using frontend JS and pass to
+the CKAN backend, but this makes your site vulnerable to XSS attacks. Instead
+the cookie should be stored in a secure way: - `samesite=Lax` with
+`domain=YOUR_DOMAIN` to help prevent CSRF. - `samesite=Strict` is even more
+secure, but significantly impacts UX for your site. - `secure` to help prevent
+man-in-the-middle. - `httpOnly` to help prevent XSS. - Setting this means the
+cookie can no longer be accessed from your JS code. Then a middleware must be
+used to convert the cookie value into a header than CKAN can interpret: **NGINX
+server example** (nginx is the default/recommended server to reverse proxy
+CKAN) (https://docs.ckan.org/en/latest/maintaining/installing/deployment.html)
+```nginx # Add the cookie-based API token to the request Authorization header #
+This is passed to the CKAN backend & read automatically by CKAN
+proxy_set_header 'Authorization' $cookie_${AUTH_COOKIE_NAME}; # If using
+caching omit the cookie proxy_cache_bypass $cookie_${AUTH_COOKIE_NAME};
+proxy_no_cache $cookie_${AUTH_COOKIE_NAME}; ``` **Apache server example**
+```apache SetEnvIf Cookie "(^|;\ *)${AUTH_COOKIE_NAME}=([^;\ ]+)"
+ckan_cookie_value=$2 RequestHeader set Authorization "%{ckan_cookie_value}e"
+``` ## Notes - It is also recommended to disable access to the API via cookie,
+to help prevent CSRF: `ckan.auth.disable_cookie_auth_in_api = true` - The
+configuration for API tokens can be configured in core: ```ini api_token.nbytes
+= 60 api_token.jwt.decode.secret = string:YOUR_SUPER_SECRET_STRING
 api_token.jwt.algorithm = HS256 # expire_api_token plugin (unit = 1 day in
 seconds, lifetime = 3 days) expire_api_token.default_lifetime = 3
 expire_api_token.default_unit = 86400 ```
```

### Comparing `ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/logic.py` & `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/logic.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         user = _create_user(email)
         log.debug(f"Created user {str(email)}")
 
     if user:
         # make sure is not deleted
         if user.state == "deleted":
             raise toolkit.ValidationError(
-                {"user": f"User with email {email} was deleted"}
+                {"user": f"User with email {email} was deleted already. Contact Admin."}
             )
         try:
             send_user_reset_key(user)
 
         except mailer.MailerException as e:
             log.error(f"Could not send token link: {str(e)}")
             raise mailer.MailerException from e(
@@ -340,17 +340,77 @@
         )
 
     except Exception as e:
         log.error(str(e))
         log.warning(f"Could not find a user for ID: {user_id}")
         return {"message": f"could not find a user for id: {user_id}"}
 
-    if user:
+    if _check_token_valid(context, data_dict):
         expiry = config.get("expire_api_token.default_lifetime", 3)
         units = config.get("expire_api_token.default_unit", 86400)
         token_json = util.renew_main_token(user_id, expiry, units)
         return {
             "user": user,
             "token": token_json.get("token"),
         }
 
     return {"message": "failed"}
+
+
+@side_effect_free
+def check_token_valid(
+    context,  #: Context,
+    data_dict,  #: DataDict,
+):
+    """Check if the token is valid and user is authenticated.
+
+    Allows for verifying user auth without renewing token.
+    Useful for verifying a token from microservices.
+
+    Returns:
+        bool: True if valid, False if not.
+    """
+    if _check_token_valid(context, data_dict):
+        return True
+
+    return False
+
+
+def _check_token_valid(
+    context,  #: Context,
+    data_dict,  #: DataDict,
+):
+    """Verify the JWT API token.
+
+    Returns:
+        bool: True if valid, False if not.
+    """
+    log.debug("start function _check_token_valid")
+
+    if (user_id := context.get("user", "")) != "":
+        log.debug("User ID extracted from context user key")
+    elif user_obj := context.get("auth_user_obj", None):
+        log.debug("User ID extracted from context auth_user_obj key")
+        user_id = user_obj.id
+    else:
+        return {
+            "message": "API token is invalid or missing from Authorization header",
+        }
+
+    user = None
+    try:
+        log.info(f"Getting user details with user_id: {user_id}")
+        user = toolkit.get_action("user_show")(
+            data_dict={
+                "id": user_id,
+            },
+        )
+
+    except Exception as e:
+        log.error(str(e))
+        log.warning(f"Could not find a user for ID: {user_id}")
+        return {"message": f"could not find a user for id: {user_id}"}
+
+    if user:
+        return True
+
+    return False
```

### Comparing `ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/mailer.py` & `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/mailer.py`

 * *Files identical despite different names*

### Comparing `ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/plugin.py` & `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from json import loads as load_json
 
 from ckan.plugins import SingletonPlugin, implements, interfaces, toolkit
 
 from ckanext.passwordless_api.logic import (
+    check_token_valid,
     get_current_user_and_renew_api_token,
     request_api_token,
     request_api_token_azure_ad,
     request_reset_key,
     revoke_api_token_no_auth,
 )
 
@@ -64,33 +65,33 @@
         """Actions to be accessible via the API."""
         return {
             "passwordless_request_reset_key": request_reset_key,
             "passwordless_request_api_token": request_api_token,
             "passwordless_request_api_token_azure_ad": request_api_token_azure_ad,
             "passwordless_revoke_api_token": revoke_api_token_no_auth,
             "passwordless_get_user": get_current_user_and_renew_api_token,
+            "passwordless_introspect": check_token_valid,
         }
 
-    # IActions
+    # IMiddleware
     def make_middleware(self, app, config):
         """Create middleware for the Flask app."""
 
         @app.after_request
         def add_api_token_cookie(response):
             """If cookie settings in config, add API token to cookie."""
             if not config.get("passwordless_api.cookie_name", None):
                 return response
 
             try:
                 # token present in both renew_api_token and get_user
-                token = load_json(response.data).get("result").get("token")
-                if not token:
+                if not (token := load_json(response.data).get("result").get("token")):
                     return response
-            except Exception:
-                return response
+            except Exception as e:
+                return e
 
             log.debug(
                 "Adding cookie to response with vars: "
                 f"key={self.cookie_name} | value={token} | "
                 f"max_age={self.cookie_expiry} | domain={self.cookie_domain} | "
                 f"secure={self.cookie_secure} | httponly={self.cookie_http_only} | "
                 f"samesite={self.cookie_samesite}"
```

### Comparing `ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/templates/welcome_user.txt` & `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/templates/welcome_user.txt`

 * *Files identical despite different names*

### Comparing `ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/tests/test_plugin.py` & `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-passwordless-api-1.0.2/ckanext/passwordless_api/util.py` & `ckanext-passwordless-api-1.1.0/ckanext/passwordless_api/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Separated helper utils to keep logic file clean."""
 
 import logging
 from datetime import datetime, timedelta
+from json import loads as load_json
 from re import match as regexmatch
 from uuid import uuid4
 
 from ckan import logic
+from ckan.common import config
 from ckan.lib.redis import connect_to_redis
 from ckan.model import User
 from ckan.plugins import toolkit
 from dateutil import parser as dateparser
 
 log = logging.getLogger(__name__)
 
@@ -46,17 +48,32 @@
 
     log.warning(f"No matching users found for email: {email}")
     return None
 
 
 def get_new_username(email: str):
     """Generate a new username and check does not exist."""
-    offset = 0
     email = email.lower()
-    username = generate_user_name(email)
+
+    anonymous_usernames = bool(
+        load_json(config.get("passwordless_api.anonymous_usernames", "false"))
+    )
+    domain_exceptions = config.get("passwordless_api.anonymous_domain_exceptions", "")
+
+    username = (
+        generate_user_name(email)
+        if not anonymous_usernames
+        else (
+            generate_user_name(email)
+            if not domain_exceptions or email.endswith(tuple(domain_exceptions))
+            else str(uuid4())
+        )
+    )
+
+    offset = 0
     while offset < 100000:
         try:
             toolkit.get_action("user_show")(
                 context={"ignore_auth": True},
                 data_dict={"id": username},
             )
             log.debug(f"User creation: {username} exists. Attempting next...")
```

### Comparing `ckanext-passwordless-api-1.0.2/pyproject.toml` & `ckanext-passwordless-api-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: Utilities",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
-version = "1.0.2"
+version = "1.1.0"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points."ckan.plugins"]
 passwordless_api = "ckanext.passwordless_api.plugin:PasswordlessAPIPlugin"
 
@@ -61,15 +61,15 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest-ckan>=0.0.12",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.2"
+version = "1.1.0"
 version_files = [
     "pyproject.toml:version",
     "ckanext/passwordless_api/__version__.py",
     "docs/openapi.yaml:version",
 ]
 
 [tool.isort]
```

### Comparing `ckanext-passwordless-api-1.0.2/PKG-INFO` & `ckanext-passwordless-api-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-passwordless_api
-Version: 1.0.2
+Version: 1.1.0
 Summary: Extension to allow paswordless login to the CKAN API
 License: MIT
 Keywords: CKAN,passwordless,token,auth
 Author-email: Sam Woodcock <sam.woodcock@protonmail.com>
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -25,15 +25,15 @@
 <div align="center">
   <a href="https://pypi.org/project/ckanext-passwordless_api" target="_blank">
       <img src="https://img.shields.io/pypi/v/ckanext-passwordless_api?color=%2334D058&label=pypi%20package" alt="Package version">
   </a>
   <a href="https://pypistats.org/packages/ckanext-passwordless_api" target="_blank">
       <img src="https://img.shields.io/pypi/dm/ckanext-passwordless_api.svg" alt="Downloads">
   </a>
-  <a href="https://gitlabext.wsl.ch/EnviDat/ckanext-passwordless_api/-/raw/main/LICENCE" target="_blank">
+  <a href="https://gitlabext.wsl.ch/EnviDat/ckanext-passwordless_api/-/raw/main/LICENSE" target="_blank">
       <img src="https://img.shields.io/github/license/EnviDat/ckanext-passwordless_api.svg" alt="Licence">
   </a>
 </div>
 
 ---
 
 **Documentation**: <a href="https://envidat.gitlab-pages.wsl.ch/ckanext-passwordless_api/" target="_blank">https://envidat.gitlab-pages.wsl.ch/ckanext-passwordless_api/</a>
@@ -94,22 +94,28 @@
   - Default: None, samesite value is set to `Lax`.
 - **passwordless_api.cookie_http_only**
   - Description: Use a httpOnly cookie, recommended.
   - Default: true.
 - **passwordless_api.cookie_path**
   - Description: Set a specific path to use the cookie, e.g. `/api`.
   - Default: `/` (all paths).
+- **passwordless_api.anonymous_usernames**
+  - Description: Set to true to anonymise usernames when generated.
+  - Default: false.
+- **passwordless_api.anonymous_domain_exceptions**
+  - Description: Email domain exceptions that should not be anonymised, if enabled.
+  - Default: None.
 
 ## Endpoints
 
 **POST**
 
 - **<CKAN_HOST>/api/3/action/passwordless_request_reset_key**
   - Description: Request a login token for a given email.
-  - Creates user if they do not exist & sends welcome email.
+    - Creates user if they do not exist & sends welcome email.
   - Param1: email (str).
 - **<CKAN_HOST>/api/3/action/passwordless_request_api_token**
   - Description: Request an API token, given the email and login token (reset_key).
   - Param1: email (str).
   - Param2: key (str).
 - **<CKAN_HOST>/api/3/action/passwordless_request_api_token_azure_ad**
   - Description: Request an API token, given the email and Azure AD token.
@@ -121,16 +127,21 @@
 
 **GET**
 
 - **<CKAN_HOST>/api/3/action/passwordless_revoke_api_token**
   - Description: If logged in, revoke the current API token.
 - **<CKAN_HOST>/api/3/action/passwordless_get_user**
   - Description: Get user details, given their API token.
-    Also resets and returns a new API token (i.e. renewal).
-    Fails silently if the user is not logged in.
+    - Also resets and returns a new API token (i.e. renewal).
+    - Fails silently if the user is not logged in.
+    - Use the core `user_show` action if refresh is not required.
+- **<CKAN_HOST>/api/3/action/passwordless_introspect**
+  - Description: Verify if the API token is valid for a user.
+    - This does not renew the token in the same call.
+    - Mostly useful for auth checking in microservice APIs.
 
 ## Using the cookie in an Authorization header
 
 If configured, the cookie containing an API token can't do much on it's own.
 
 It is possible to extract the cookie value using frontend JS and pass to the CKAN backend, but this makes your site vulnerable to XSS attacks.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ckanext-passwordless_api Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: ckanext-passwordless_api Version: 1.1.0 Summary:
 Extension to allow paswordless login to the CKAN API License: MIT Keywords:
 CKAN,passwordless,token,auth Author-email: Sam Woodcock
 woodcock@protonmail.com> Requires-Python: >=3.8 Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities Project-URL: documentation, https://
@@ -42,46 +42,53 @@
 respect, required if cookie set. - Default: None. -
 **passwordless_api.cookie_samesite** - Description: To change the cookie
 samesite value to `Strict`. Only enable this if you know what you are doing. -
 Default: None, samesite value is set to `Lax`. -
 **passwordless_api.cookie_http_only** - Description: Use a httpOnly cookie,
 recommended. - Default: true. - **passwordless_api.cookie_path** - Description:
 Set a specific path to use the cookie, e.g. `/api`. - Default: `/` (all paths).
-## Endpoints **POST** - **/api/3/action/passwordless_request_reset_key** -
+- **passwordless_api.anonymous_usernames** - Description: Set to true to
+anonymise usernames when generated. - Default: false. -
+**passwordless_api.anonymous_domain_exceptions** - Description: Email domain
+exceptions that should not be anonymised, if enabled. - Default: None. ##
+Endpoints **POST** - **/api/3/action/passwordless_request_reset_key** -
 Description: Request a login token for a given email. - Creates user if they do
 not exist & sends welcome email. - Param1: email (str). - **/api/3/action/
 passwordless_request_api_token** - Description: Request an API token, given the
 email and login token (reset_key). - Param1: email (str). - Param2: key (str).
 - **/api/3/action/passwordless_request_api_token_azure_ad** - Description:
 Request an API token, given the email and Azure AD token. - Param1: email
 (str). - Param2: token (str). - **/api/3/action/passwordless_revoke_api_token**
 - Description: Revoke an API token. - Param1: token (str). **GET** - **/api/3/
 action/passwordless_revoke_api_token** - Description: If logged in, revoke the
 current API token. - **/api/3/action/passwordless_get_user** - Description: Get
-user details, given their API token. Also resets and returns a new API token
-(i.e. renewal). Fails silently if the user is not logged in. ## Using the
-cookie in an Authorization header If configured, the cookie containing an API
-token can't do much on it's own. It is possible to extract the cookie value
-using frontend JS and pass to the CKAN backend, but this makes your site
-vulnerable to XSS attacks. Instead the cookie should be stored in a secure way:
-- `samesite=Lax` with `domain=YOUR_DOMAIN` to help prevent CSRF. -
-`samesite=Strict` is even more secure, but significantly impacts UX for your
-site. - `secure` to help prevent man-in-the-middle. - `httpOnly` to help
-prevent XSS. - Setting this means the cookie can no longer be accessed from
-your JS code. Then a middleware must be used to convert the cookie value into a
-header than CKAN can interpret: **NGINX server example** (nginx is the default/
-recommended server to reverse proxy CKAN) (https://docs.ckan.org/en/latest/
-maintaining/installing/deployment.html) ```nginx # Add the cookie-based API
-token to the request Authorization header # This is passed to the CKAN backend
-& read automatically by CKAN proxy_set_header 'Authorization' $cookie_$
-{AUTH_COOKIE_NAME}; # If using caching omit the cookie proxy_cache_bypass
-$cookie_${AUTH_COOKIE_NAME}; proxy_no_cache $cookie_${AUTH_COOKIE_NAME}; ```
-**Apache server example** ```apache SetEnvIf Cookie "(^|;\ *)$
-{AUTH_COOKIE_NAME}=([^;\ ]+)" ckan_cookie_value=$2 RequestHeader set
-Authorization "%{ckan_cookie_value}e" ``` ## Notes - It is also recommended to
-disable access to the API via cookie, to help prevent CSRF:
-`ckan.auth.disable_cookie_auth_in_api = true` - The configuration for API
-tokens can be configured in core: ```ini api_token.nbytes = 60
-api_token.jwt.decode.secret = string:YOUR_SUPER_SECRET_STRING
+user details, given their API token. - Also resets and returns a new API token
+(i.e. renewal). - Fails silently if the user is not logged in. - Use the core
+`user_show` action if refresh is not required. - **/api/3/action/
+passwordless_introspect** - Description: Verify if the API token is valid for a
+user. - This does not renew the token in the same call. - Mostly useful for
+auth checking in microservice APIs. ## Using the cookie in an Authorization
+header If configured, the cookie containing an API token can't do much on it's
+own. It is possible to extract the cookie value using frontend JS and pass to
+the CKAN backend, but this makes your site vulnerable to XSS attacks. Instead
+the cookie should be stored in a secure way: - `samesite=Lax` with
+`domain=YOUR_DOMAIN` to help prevent CSRF. - `samesite=Strict` is even more
+secure, but significantly impacts UX for your site. - `secure` to help prevent
+man-in-the-middle. - `httpOnly` to help prevent XSS. - Setting this means the
+cookie can no longer be accessed from your JS code. Then a middleware must be
+used to convert the cookie value into a header than CKAN can interpret: **NGINX
+server example** (nginx is the default/recommended server to reverse proxy
+CKAN) (https://docs.ckan.org/en/latest/maintaining/installing/deployment.html)
+```nginx # Add the cookie-based API token to the request Authorization header #
+This is passed to the CKAN backend & read automatically by CKAN
+proxy_set_header 'Authorization' $cookie_${AUTH_COOKIE_NAME}; # If using
+caching omit the cookie proxy_cache_bypass $cookie_${AUTH_COOKIE_NAME};
+proxy_no_cache $cookie_${AUTH_COOKIE_NAME}; ``` **Apache server example**
+```apache SetEnvIf Cookie "(^|;\ *)${AUTH_COOKIE_NAME}=([^;\ ]+)"
+ckan_cookie_value=$2 RequestHeader set Authorization "%{ckan_cookie_value}e"
+``` ## Notes - It is also recommended to disable access to the API via cookie,
+to help prevent CSRF: `ckan.auth.disable_cookie_auth_in_api = true` - The
+configuration for API tokens can be configured in core: ```ini api_token.nbytes
+= 60 api_token.jwt.decode.secret = string:YOUR_SUPER_SECRET_STRING
 api_token.jwt.algorithm = HS256 # expire_api_token plugin (unit = 1 day in
 seconds, lifetime = 3 days) expire_api_token.default_lifetime = 3
 expire_api_token.default_unit = 86400 ```
```

