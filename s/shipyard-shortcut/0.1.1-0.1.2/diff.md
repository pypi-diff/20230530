# Comparing `tmp/shipyard_shortcut-0.1.1.tar.gz` & `tmp/shipyard_shortcut-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_shortcut-0.1.1.tar", max compression
+gzip compressed data, was "shipyard_shortcut-0.1.2.tar", max compression
```

## Comparing `shipyard_shortcut-0.1.1.tar` & `shipyard_shortcut-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3717 2023-05-23 20:47:26.013626 shipyard_shortcut-0.1.1/README.md
--rw-r--r--   0        0        0      618 2023-05-23 20:50:33.169412 shipyard_shortcut-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       93 2023-05-23 17:16:20.929501 shipyard_shortcut-0.1.1/shipyard_shortcut/__init__.py
--rw-r--r--   0        0        0      904 2023-05-23 17:24:11.820053 shipyard_shortcut-0.1.1/shipyard_shortcut/cli/add_comment.py
--rw-r--r--   0        0        0     1985 2023-05-24 02:43:06.027871 shipyard_shortcut-0.1.1/shipyard_shortcut/cli/create_ticket.py
--rw-r--r--   0        0        0     2185 2023-05-24 02:43:06.024139 shipyard_shortcut-0.1.1/shipyard_shortcut/cli/edit_ticket.py
--rw-r--r--   0        0        0      781 2023-05-23 17:14:38.300077 shipyard_shortcut-0.1.1/shipyard_shortcut/error_handler.py
--rw-r--r--   0        0        0     8355 2023-05-23 20:32:32.455002 shipyard_shortcut-0.1.1/shipyard_shortcut/shortcut.py
--rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 shipyard_shortcut-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3722 2023-05-30 13:23:10.342632 shipyard_shortcut-0.1.2/README.md
+-rw-r--r--   0        0        0      618 2023-05-30 13:25:43.735912 shipyard_shortcut-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-05-25 13:51:48.292105 shipyard_shortcut-0.1.2/shipyard_shortcut/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-30 13:21:53.620981 shipyard_shortcut-0.1.2/shipyard_shortcut/cli/add_comment.py
+-rw-r--r--   0        0        0     1985 2023-05-25 13:51:48.292792 shipyard_shortcut-0.1.2/shipyard_shortcut/cli/create_ticket.py
+-rw-r--r--   0        0        0     2185 2023-05-25 13:51:48.293295 shipyard_shortcut-0.1.2/shipyard_shortcut/cli/edit_ticket.py
+-rw-r--r--   0        0        0      781 2023-05-25 13:51:48.293489 shipyard_shortcut-0.1.2/shipyard_shortcut/error_handler.py
+-rw-r--r--   0        0        0     8379 2023-05-30 13:23:10.337976 shipyard_shortcut-0.1.2/shipyard_shortcut/shortcut.py
+-rw-r--r--   0        0        0     4273 1970-01-01 00:00:00.000000 shipyard_shortcut-0.1.2/PKG-INFO
```

### Comparing `shipyard_shortcut-0.1.1/README.md` & `shipyard_shortcut-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 * **--story-type:** (optional) The new type of the story. Possible values are 'feature', 'bug', or 'chore'.
 * **--labels:** (optional) Comma-separated labels to assign to the story.
 * **--deadline:** (optional) The new deadline for the story.
 * **--tasks:** (optional) Comma-separated tasks to add to the story.
 * **Note:** If --labels or --tasks are provided, they should be comma-separated values.
 
 ## Authentication
-Step 1: Go to https://app.shortcut.com/shipyardapp/settings/account/api-tokens to generate an API token.
+Step 1: Go to https://app.shortcut.com/<workspace_name>/settings/account/api-tokens to generate an API token.
 Step 2: Give the token a memorable name and click "Generate Token".
 ## Finding the Workflow State ID in Shortcut:
 1. **Navigate to the Shortcut Board:** Go to the Shortcut board where you want to find the workflow state ID.
 
 2. **Locate the Workflow State:** Identify the specific workflow state you are interested in.
 
 3. **Access Workflow State Options:** Click on the ellipsis (...) button associated with the workflow state.
```

### Comparing `shipyard_shortcut-0.1.1/pyproject.toml` & `shipyard_shortcut-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-shortcut"
-version = "0.1.1"
+version = "0.1.2"
 description = "A local client for connecting and working with the shortcut app"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>"]
 readme = "README.md"
 packages = [{include = "shipyard_shortcut"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `shipyard_shortcut-0.1.1/shipyard_shortcut/cli/add_comment.py` & `shipyard_shortcut-0.1.2/shipyard_shortcut/cli/add_comment.py`

 * *Files identical despite different names*

### Comparing `shipyard_shortcut-0.1.1/shipyard_shortcut/cli/create_ticket.py` & `shipyard_shortcut-0.1.2/shipyard_shortcut/cli/create_ticket.py`

 * *Files identical despite different names*

### Comparing `shipyard_shortcut-0.1.1/shipyard_shortcut/cli/edit_ticket.py` & `shipyard_shortcut-0.1.2/shipyard_shortcut/cli/edit_ticket.py`

 * *Files identical despite different names*

### Comparing `shipyard_shortcut-0.1.1/shipyard_shortcut/error_handler.py` & `shipyard_shortcut-0.1.2/shipyard_shortcut/error_handler.py`

 * *Files identical despite different names*

### Comparing `shipyard_shortcut-0.1.1/shipyard_shortcut/shortcut.py` & `shipyard_shortcut-0.1.2/shipyard_shortcut/shortcut.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
             **kwargs
         }
         self.logger.info(f'Creating story with the following details: {data}')
         try:
             response = self._request('stories', method='POST', data=data)
         except Exception as error:
             self.logger.error(f'Failed to create story: {error}')
+            raise error
         else:
             self.logger.info('Story successfully created')
             return response
 
     def update_ticket(self,
                       story_id: int, **kwargs):
         """
```

### Comparing `shipyard_shortcut-0.1.1/PKG-INFO` & `shipyard_shortcut-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-shortcut
-Version: 0.1.1
+Version: 0.1.2
 Summary: A local client for connecting and working with the shortcut app
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -56,15 +56,15 @@
 * **--story-type:** (optional) The new type of the story. Possible values are 'feature', 'bug', or 'chore'.
 * **--labels:** (optional) Comma-separated labels to assign to the story.
 * **--deadline:** (optional) The new deadline for the story.
 * **--tasks:** (optional) Comma-separated tasks to add to the story.
 * **Note:** If --labels or --tasks are provided, they should be comma-separated values.
 
 ## Authentication
-Step 1: Go to https://app.shortcut.com/shipyardapp/settings/account/api-tokens to generate an API token.
+Step 1: Go to https://app.shortcut.com/<workspace_name>/settings/account/api-tokens to generate an API token.
 Step 2: Give the token a memorable name and click "Generate Token".
 ## Finding the Workflow State ID in Shortcut:
 1. **Navigate to the Shortcut Board:** Go to the Shortcut board where you want to find the workflow state ID.
 
 2. **Locate the Workflow State:** Identify the specific workflow state you are interested in.
 
 3. **Access Workflow State Options:** Click on the ellipsis (...) button associated with the workflow state.
```

