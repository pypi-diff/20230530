# Comparing `tmp/ckanext-search-tweaks-0.4.12.tar.gz` & `tmp/ckanext-search-tweaks-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-search-tweaks-0.4.12.tar", last modified: Thu Mar 16 09:45:36 2023, max compression
+gzip compressed data, was "ckanext-search-tweaks-0.5.0.tar", last modified: Tue May 30 13:54:53 2023, max compression
```

## Comparing `ckanext-search-tweaks-0.4.12.tar` & `ckanext-search-tweaks-0.5.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)    34500 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/LICENSE
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      211 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/MANIFEST.in
--rw-rw-r--   0 cherry    (1000) cherry    (1000)    11954 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/PKG-INFO
--rw-rw-r--   0 cherry    (1000) cherry    (1000)    11415 2023-03-16 09:32:49.000000 ckanext-search-tweaks-0.4.12/README.md
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      221 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/__init__.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      518 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/__init__.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/__init__.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/assets/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      584 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/assets/advanced-search.css
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2328 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/assets/advanced-search.js
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      439 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/assets/webassets.yml
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     3118 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/plugin.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/templates/
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/templates/advanced_search/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     4266 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/templates/advanced_search/search_form.html
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      321 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/cli.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/__init__.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/assets/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      490 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/assets/search-tweaks-reflect-range-in-label.js
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      184 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/assets/webassets.yml
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1458 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/plugin.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/templates/
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/templates/search_tweaks/
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/templates/search_tweaks/field_relevance/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1118 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/templates/search_tweaks/field_relevance/promote.html
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     3298 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/views.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      727 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/interfaces.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     4071 2023-03-16 09:21:17.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/plugin.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1498 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2638 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/cli.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2425 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/plugin.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1810 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/score.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     5020 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/storage.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1401 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      250 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/cli.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     4393 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/helpers.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      572 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/plugin.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.764915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/templates/
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/templates/search_tweaks/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      654 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/templates/search_tweaks/did_you_mean.html
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      662 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/conftest.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/query_relevance/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/query_relevance/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2217 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/query_relevance/test_plugin.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1140 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/query_relevance/test_score.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2821 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/query_relevance/test_storage.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/spellcheck/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/spellcheck/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2551 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/spellcheck/test_plugin.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     4795 2023-03-16 09:37:53.000000 ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/test_plugin.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)    11954 2023-03-16 09:45:36.000000 ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/PKG-INFO
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2251 2023-03-16 09:45:36.000000 ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/SOURCES.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        1 2023-03-16 09:45:36.000000 ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/dependency_links.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      514 2023-03-16 09:45:36.000000 ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/entry_points.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-03-16 09:45:36.000000 ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/namespace_packages.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)       47 2023-03-16 09:45:36.000000 ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/requires.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-03-16 09:45:36.000000 ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/top_level.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      608 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/pyproject.toml
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-03-16 08:43:21.000000 ckanext-search-tweaks-0.4.12/requirements.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      625 2023-03-16 09:45:36.768915 ckanext-search-tweaks-0.4.12/setup.cfg
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     4255 2023-03-16 09:39:13.000000 ckanext-search-tweaks-0.4.12/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11953 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11415 2023-03-17 07:52:39.000000 ckanext-search-tweaks-0.5.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      518 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      584 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/assets/advanced-search.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2328 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/assets/advanced-search.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      439 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3231 2023-05-30 13:53:37.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.263791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/templates/advanced_search/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4266 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/templates/advanced_search/search_form.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      321 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/cli.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      490 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/assets/search-tweaks-reflect-range-in-label.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      184 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1380 2023-05-30 13:53:36.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.263791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.263791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/templates/search_tweaks/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/templates/search_tweaks/field_relevance/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1118 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/templates/search_tweaks/field_relevance/promote.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3225 2023-05-30 13:01:26.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/views.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      715 2023-05-30 13:01:26.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/interfaces.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4035 2023-05-30 13:01:26.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1498 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2576 2023-05-30 12:58:29.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2352 2023-05-30 13:01:26.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1810 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/score.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5020 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/storage.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1401 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      250 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4334 2023-05-30 13:52:45.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      572 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.263791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/templates/search_tweaks/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      654 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/templates/search_tweaks/did_you_mean.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      662 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/query_relevance/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/query_relevance/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2196 2023-05-30 13:01:26.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/query_relevance/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1140 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/query_relevance/test_score.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2821 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/query_relevance/test_storage.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/spellcheck/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/spellcheck/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2521 2023-05-30 13:01:26.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/spellcheck/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4657 2023-05-30 13:03:14.000000 ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/test_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11953 2023-05-30 13:54:53.000000 ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2251 2023-05-30 13:54:53.000000 ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-30 13:54:53.000000 ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      514 2023-05-30 13:54:53.000000 ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-30 13:54:53.000000 ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       47 2023-05-30 13:54:53.000000 ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-30 13:54:53.000000 ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4174 2023-05-30 12:58:29.000000 ckanext-search-tweaks-0.5.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-09 18:25:07.000000 ckanext-search-tweaks-0.5.0/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      625 2023-05-30 13:54:53.273791 ckanext-search-tweaks-0.5.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4241 2023-05-30 13:53:31.000000 ckanext-search-tweaks-0.5.0/setup.py
```

### Comparing `ckanext-search-tweaks-0.4.12/LICENSE` & `ckanext-search-tweaks-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/PKG-INFO` & `ckanext-search-tweaks-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-search-tweaks
-Version: 0.4.12
+Version: 0.5.0
 Home-page: https://github.com/DataShades/ckanext-search-tweaks
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-search-tweaks-0.4.12/README.md` & `ckanext-search-tweaks-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/__init__.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/assets/advanced-search.css` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/assets/advanced-search.css`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/assets/advanced-search.js` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/assets/advanced-search.js`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/plugin.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
+
 import json
 from typing import Any
+
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
 from ckan.exceptions import CkanConfigurationException
 
 CONFIG_FORM_DEFINITION = "ckanext.search_tweaks.advanced_search.fields"
 CONFIG_FIELD_ORDER = "ckanext.search_tweaks.advanced_search.order"
 
@@ -71,31 +73,35 @@
         try:
             from ckanext.composite_search.interfaces import ICompositeSearch
         except ImportError:
             raise CkanConfigurationException(
                 "ckanext-composite-search is not installed"
             )
         if not p.plugin_loaded("composite_search"):
-            raise CkanConfigurationException(
-                "`composite_search` plugin must be enabled in order to use advanced search"
-            )
+            msg = "Advanced search requires `composite_search` plugin"
+            raise CkanConfigurationException(msg)
         if not list(p.PluginImplementations(ICompositeSearch)):
-            raise CkanConfigurationException(
-                "Advanced search requires plugin that implements ICompositeSearch."
-                + " Consider enabling `default_composite_search` plugins."
+            msg = (
+                "Advanced search requires plugin that implements"
+                + " ICompositeSearch. Consider enabling "
+                + "`default_composite_search` plugins."
             )
+            raise CkanConfigurationException(msg)
 
     # ITemplateHelpers
 
     def get_helpers(self):
         return {
             "advanced_search_form_config": form_config,
         }
 
     # IPackageController
 
-    def before_search(self, search_params: dict[str, Any]):
+    def before_dataset_search(self, search_params: dict[str, Any]):
         solr_q = search_params.get("extras", {}).get("ext_solr_q", None)
         if solr_q:
             search_params.setdefault("q", "")
             search_params["q"] += " " + solr_q
         return search_params
+
+    if not tk.check_ckan_version("2.10"):
+        before_search = before_dataset_search
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/advanced_search/templates/advanced_search/search_form.html` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/advanced_search/templates/advanced_search/search_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/plugin.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 
-from typing import Any, Optional
+from typing import Any
 
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
 
-from . import views
-from ..interfaces import ISearchTweaks
 from .. import feature_disabled
+from ..interfaces import ISearchTweaks
+from . import views
 
 CONFIG_BOOST_FN = "ckanext.search_tweaks.field_relevance.boost_function"
 
 DEFAULT_BOOST_FN = None
 
 
 class FieldRelevancePlugin(p.SingletonPlugin):
     p.implements(ISearchTweaks, inherit=True)
     p.implements(p.IAuthFunctions)
     p.implements(p.IBlueprint)
     p.implements(p.IConfigurer, inherit=True)
 
     # ISearchTweaks
-    def get_search_boost_fn(
-        self, search_params: dict[str, Any]
-    ) -> Optional[str]:
+    def get_search_boost_fn(self, search_params: dict[str, Any]) -> str | None:
         if feature_disabled("field_boost", search_params):
             return
 
         return tk.config.get(CONFIG_BOOST_FN, DEFAULT_BOOST_FN)
 
     # IBlueprint
 
@@ -36,22 +34,21 @@
 
     # IConfigurer
 
     def update_config(self, config):
         tk.add_template_directory(config, "templates")
         tk.add_resource("assets", "search_tweaks_field_relevance")
 
-
     # IAuthFunctions
     def get_auth_functions(self):
         return {
-            "search_tweaks_field_relevance_promote": search_tweaks_field_relevance_promote,
+            "search_tweaks_field_relevance_promote": promote_auth,
         }
 
 
-def search_tweaks_field_relevance_promote(context, data_dict):
+def promote_auth(context, data_dict):
     try:
         tk.check_access("package_update", context, data_dict)
     except tk.NotAuthorized:
         return {"success": False}
 
     return {"success": True}
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/templates/search_tweaks/field_relevance/promote.html` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/templates/search_tweaks/field_relevance/promote.html`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/field_relevance/views.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/field_relevance/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
+
 from typing import Any, Optional
 
 from flask import Blueprint
 from flask.views import MethodView
 
 import ckan.model as model
 import ckan.plugins.toolkit as tk
 
 CONFIG_ENABLE_PROMOTION_ROUTE = (
     "ckanext.search_tweaks.field_relevance.blueprint.promotion.enabled"
 )
-CONFIG_PROMOTION_PATH = (
-    "ckanext.search_tweaks.field_relevance.blueprint.promotion.path"
-)
+CONFIG_PROMOTION_PATH = "ckanext.search_tweaks.field_relevance.blueprint.promotion.path"
 CONFIG_MAX_PROMOTION = (
     "ckanext.search_tweaks.field_relevance.blueprint.promotion.max_value"
 )
 CONFIG_PROMOTION_FIELD = (
     "ckanext.search_tweaks.field_relevance.blueprint.promotion.field_name"
 )
 
@@ -26,22 +25,18 @@
 DEFAULT_PROMOTION_FIELD = "promotion_level"
 
 field_relevance = Blueprint("search_tweaks_field_relevance", __name__)
 
 
 def get_blueprints():
     if tk.asbool(
-        tk.config.get(
-            CONFIG_ENABLE_PROMOTION_ROUTE, DEFAULT_ENABLE_PROMOTION_ROUTE
-        )
+        tk.config.get(CONFIG_ENABLE_PROMOTION_ROUTE, DEFAULT_ENABLE_PROMOTION_ROUTE)
     ):
         path = tk.config.get(CONFIG_PROMOTION_PATH, DEFAULT_PROMOTION_PATH)
-        field_relevance.add_url_rule(
-            path, view_func=PromoteView.as_view("promote")
-        )
+        field_relevance.add_url_rule(path, view_func=PromoteView.as_view("promote"))
 
     return [field_relevance]
 
 
 class PromoteView(MethodView):
     def _check_access(self, id: str) -> None:
         try:
@@ -96,10 +91,8 @@
             "data": data or pkg_dict,
             "max_promotion": tk.asint(
                 tk.config.get(CONFIG_MAX_PROMOTION, DEFAULT_MAX_PROMOTION)
             ),
             "field_name": field,
         }
 
-        return tk.render(
-            "search_tweaks/field_relevance/promote.html", extra_vars
-        )
+        return tk.render("search_tweaks/field_relevance/promote.html", extra_vars)
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/interfaces.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
+
 from typing import Any, Optional
 
 from ckan.plugins.interfaces import Interface
+
 from . import CONFIG_PREFER_BOOST
 
 
 class ISearchTweaks(Interface):
-    def get_search_boost_fn(
-        self, search_params: dict[str, Any]
-    ) -> Optional[str]:
+    def get_search_boost_fn(self, search_params: dict[str, Any]) -> Optional[str]:
         f"""Return Solr's boost function applicable to the current search.
 
         Note: it will be applied as `boost` when `{CONFIG_PREFER_BOOST}`
         enabled and as `bf` otherwise.
 
         """
         return None
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/plugin.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from __future__ import annotations
 
 import logging
-
 from typing import Any, Dict
+
 import ckan.plugins as plugins
 import ckan.plugins.toolkit as tk
 from ckan.lib.search.query import QUERY_FIELDS
 
-from . import cli, boost_preffered, feature_disabled
+from . import boost_preffered, cli, feature_disabled
 from .interfaces import ISearchTweaks
 
 log = logging.getLogger(__name__)
 
 SearchParams = Dict[str, Any]
 
 CONFIG_QF = "ckanext.search_tweaks.common.qf"
 CONFIG_FUZZY = "ckanext.search_tweaks.common.fuzzy_search.enabled"
 CONFIG_FUZZY_DISTANCE = "ckanext.search_tweaks.common.fuzzy_search.distance"
 CONFIG_MM = "ckanext.search_tweaks.common.mm"
-CONFIG_FUZZY_KEEP_ORIGINAL = (
-    "ckanext.search_tweaks.common.fuzzy_search.keep_original"
-)
+CONFIG_FUZZY_KEEP_ORIGINAL = "ckanext.search_tweaks.common.fuzzy_search.keep_original"
 
 DEFAULT_QF = QUERY_FIELDS
 DEFAULT_FUZZY = False
 DEFAULT_FUZZY_DISTANCE = 1
 DEFAULT_MM = "1"
 DEFAULT_FUZZY_KEEP_ORIGINAL = True
 
@@ -79,17 +77,15 @@
         search_params["bf"] = f"sum({search_params['bf']},{extra_bf})"
 
 
 def _set_qf(search_params: SearchParams) -> None:
     if feature_disabled("qf", search_params):
         return
 
-    default_qf: str = search_params.get("qf") or tk.config.get(
-        CONFIG_QF, DEFAULT_QF
-    )
+    default_qf: str = search_params.get("qf") or tk.config.get(CONFIG_QF, DEFAULT_QF)
     search_params.setdefault("qf", default_qf)
     for plugin in plugins.PluginImplementations(ISearchTweaks):
         extra_qf = plugin.get_extra_qf(search_params)
         if not extra_qf:
             continue
         search_params["qf"] += " " + extra_qf
 
@@ -125,17 +121,15 @@
     ):
         search_params["q"] = f"({fuzzy_q}) OR ({q})"
     else:
         search_params["q"] = fuzzy_q
 
 
 def _get_fuzzy_distance() -> int:
-    distance = tk.asint(
-        tk.config.get(CONFIG_FUZZY_DISTANCE, DEFAULT_FUZZY_DISTANCE)
-    )
+    distance = tk.asint(tk.config.get(CONFIG_FUZZY_DISTANCE, DEFAULT_FUZZY_DISTANCE))
     if distance < 0:
         log.warning("Cannot use negative fuzzy distance: %s.", distance)
         distance = 0
     elif distance > 2:
         log.warning(
             "Cannot use fuzzy distance greater than 2: %s. Reduce it to top boundary",
             distance,
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/__init__.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/cli.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,15 @@
     if not date:
         date = datetime.date.today()
     with freezegun.freeze_time(date):
         reader = csv.DictReader(source)
         for row in reader:
             pkg = model.Package.get(row["package_id"])
             if not pkg:
-                click.secho(
-                    f"Package {row['package_id']} does not exists", fg="red"
-                )
+                click.secho(f"Package {row['package_id']} does not exists", fg="red")
                 continue
             score = QueryScore(pkg.id, row["search_query"])
             score.reset()
             score.increase(int(row["count_of_hits"]))
     click.secho("Done", fg="green")
 
 
@@ -54,15 +52,15 @@
     click.secho("Done", fg="green")
 
 
 @query.command()
 def align():
     """Remove old records."""
     rows = QueryScore.get_all()
-    for (id_, query, _) in rows:
+    for id_, query, _ in rows:
         score = QueryScore(id_, query)
         score.align()
 
 
 @query.command()
 @click.option("--days", "-d", type=int, default=1)
 @click.argument("file")
@@ -76,17 +74,15 @@
     If redis is up for N days and more, it contains relevant stats. We can
     safely export them and overwrite old snapshot.
 
     """
     conn = connect_to_redis()
     uptime = conn.info()["uptime_in_days"]
     if uptime >= days:
-        click.secho(
-            f"Redis runs for {uptime} days. Creating snapshot..", fg="green"
-        )
+        click.secho(f"Redis runs for {uptime} days. Creating snapshot..", fg="green")
         ctx.invoke(export, output=click.File("w")(file))
     else:
         click.secho(
             f"Redis runs for {uptime} days. Restore stats from snapshot..",
             fg="red",
         )
         ctx.invoke(import_source, source=click.File()(file))
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/plugin.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
+
 from string import Template
 from typing import Any, Optional
 
 import ckan.plugins as plugins
 import ckan.plugins.toolkit as tk
 
-from . import QueryScore, normalize_query, update_score_by_url
-
+from .. import feature_disabled
 from ..cli import attach_relevance_command
 from ..interfaces import ISearchTweaks
-from .. import feature_disabled
-from . import cli
+from . import QueryScore, cli, normalize_query, update_score_by_url
 
 CONFIG_BOOST_STRING = "ckanext.search_tweaks.query_relevance.boost_function"
 CONFIG_RELEVANCE_PREFIX = "ckanext.search_tweaks.query_relevance.field_prefix"
 
 DEFAULT_BOOST_STRING = "scale(def($field,0),1,1.2)"
 DEFAULT_RELEVANCE_PREFIX = "query_relevance_"
 
@@ -28,41 +27,35 @@
 
     def configure(self, config):
         attach_relevance_command(cli.query)
 
     # IPackageController
 
     def before_index(self, pkg_dict):
-        prefix = tk.config.get(
-            CONFIG_RELEVANCE_PREFIX, DEFAULT_RELEVANCE_PREFIX
-        )
+        prefix = tk.config.get(CONFIG_RELEVANCE_PREFIX, DEFAULT_RELEVANCE_PREFIX)
 
-        for (_, query, score) in QueryScore.get_for(pkg_dict["id"]):
+        for _, query, score in QueryScore.get_for(pkg_dict["id"]):
             query = query.replace(" ", "_")
             pkg_dict[prefix + query] = score
 
         return pkg_dict
 
     def read(self, entity):
         # update search relevance only for WEB-requests. Any kind of
         # CLI/search-index manipulations has no effect on it
         if tk.request and tk.get_endpoint() == (entity.type, "read"):
             update_score_by_url(entity)
 
     # ISearchTweaks
 
-    def get_search_boost_fn(
-        self, search_params: dict[str, Any]
-    ) -> Optional[str]:
+    def get_search_boost_fn(self, search_params: dict[str, Any]) -> Optional[str]:
         if feature_disabled("query_boost", search_params):
             return
 
-        prefix = tk.config.get(
-            CONFIG_RELEVANCE_PREFIX, DEFAULT_RELEVANCE_PREFIX
-        )
+        prefix = tk.config.get(CONFIG_RELEVANCE_PREFIX, DEFAULT_RELEVANCE_PREFIX)
         disabled = tk.asbool(
             search_params.get("extras", {}).get(
                 "ext_search_tweaks_disable_relevance", False
             )
         )
 
         if not search_params.get("q") or disabled:
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/score.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/score.py`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/query_relevance/storage.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/query_relevance/storage.py`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/__init__.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/helpers.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 
 from functools import total_ordering
 from typing import Any, Optional
 
 import ckan.plugins.toolkit as tk
 from ckan.lib.search.common import make_connection
 
-from . import (
-    get_spellcheck_params,
-    CONFIG_SHOW_ONLY_MORE,
-    DEFAULT_SHOW_ONLY_MORE,
-)
+from . import CONFIG_SHOW_ONLY_MORE, DEFAULT_SHOW_ONLY_MORE, get_spellcheck_params
 
 CONFIG_MAX_SUGGESTIONS = "ckanext.search_tweaks.spellcheck.max_suggestions"
 CONFIG_SUGGESTION_FOR_SINGLE = (
     "ckanext.search_tweaks.spellcheck.single_term_prefer_suggestion"
 )
 
 DEFAULT_MAX_SUGGESTIONS = 1
@@ -52,42 +48,34 @@
 
     if not max_suggestions:
         max_suggestions = tk.asint(
             tk.config.get(CONFIG_MAX_SUGGESTIONS, DEFAULT_MAX_SUGGESTIONS)
         )
 
     use_suggestion_for_single = tk.asbool(
-        tk.config.get(
-            CONFIG_SUGGESTION_FOR_SINGLE, DEFAULT_SUGGESTION_FOR_SINGLE
-        )
+        tk.config.get(CONFIG_SUGGESTION_FOR_SINGLE, DEFAULT_SUGGESTION_FOR_SINGLE)
     )
     terms = q.split()
     if len(terms) == 1 and use_suggestion_for_single:
         # TODO: check min hits
         return spellcheck.suggestions.get(terms[0], [])[:max_suggestions]
 
     collations = [
-        str(c)
-        for c in spellcheck.best_collations(max_suggestions)
-        if min_hits < c
+        str(c) for c in spellcheck.best_collations(max_suggestions) if min_hits < c
     ]
 
     if len(collations) < max_suggestions:
         # this is a bit tricky part. We are collecting brand new query from the
         # best suggestions for each separate token in the original
         # query. Result of this operation is likely to be the nonesense from
         # the human's point of view, but Solr will gladely accept it.
 
         # TODO: check min hits
         new_q = " ".join(
-            [
-                spellcheck.suggestions[w][0]
-                for w in terms
-                if w in spellcheck.suggestions
-            ]
+            [spellcheck.suggestions[w][0] for w in terms if w in spellcheck.suggestions]
         )
         if new_q:
             collations.append(new_q)
 
     return collations
 
 
@@ -138,15 +126,19 @@
 
 
 class SpellcheckResult:
     collations: list[Collation]
     suggestions: dict[str, list[str]]
 
     def __repr__(self):
-        return f"<Spellcheck(collations={self.collations}, suggestions={self.suggestions})>"
+        return (
+            "<Spellcheck("
+            + f"collations={self.collations}, suggestions={self.suggestions}"
+            + ")>"
+        )
 
     def __init__(self, collations: list[Any], suggestions: list[Any]):
         self.collations = [Collation(item) for item in collations[1::2]]
         self.suggestions = dict(
             zip(suggestions[::2], [s["suggestion"] for s in suggestions[1::2]])
         )
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/plugin.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/spellcheck/templates/search_tweaks/did_you_mean.html` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/spellcheck/templates/search_tweaks/did_you_mean.html`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/conftest.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/query_relevance/test_plugin.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/query_relevance/test_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 import ckan.model as model
+
 import ckanext.search_tweaks.query_relevance as relevance
 
 
 @pytest.mark.usefixtures("with_request_context")
 class TestPathHasScore:
     @pytest.mark.parametrize(
         "path, has_score",
@@ -41,17 +42,15 @@
             ("/organization/valid", True),
             ("/group/valid", True),
             ("/organization/invalid", False),
         ],
     )
     def test_group_referrer(self, path, has_score, monkeypatch):
         pkg = model.Package(type="dataset")
-        monkeypatch.setattr(
-            model.Group, "get", lambda _: model.Group(name="valid")
-        )
+        monkeypatch.setattr(model.Group, "get", lambda _: model.Group(name="valid"))
         assert relevance._path_has_score_for(path, pkg) is has_score
 
 
 @pytest.mark.usefixtures("with_request_context")
 class TestUpdateScore:
     @pytest.mark.parametrize(
         "url, repeat, value",
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/query_relevance/test_score.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/query_relevance/test_score.py`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/query_relevance/test_storage.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/query_relevance/test_storage.py`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/spellcheck/test_plugin.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/spellcheck/test_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,26 @@
 
 import pytest
 from bs4 import BeautifulSoup
 
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
 from ckan.tests.factories import Dataset
-from ckanext.search_tweaks.spellcheck import (
-    CONFIG_SHOW_ONLY_MORE,
-    rebuild_dictionary,
-)
 
+from ckanext.search_tweaks.spellcheck import CONFIG_SHOW_ONLY_MORE, rebuild_dictionary
 
-@pytest.mark.ckan_config(
-    "ckan.plugins", "search_tweaks search_tweaks_spellcheck"
-)
+
+@pytest.mark.ckan_config("ckan.plugins", "search_tweaks search_tweaks_spellcheck")
 @pytest.mark.usefixtures("with_plugins")
 class TestSpellcheck:
     def test_plugin_loaded(self):
         assert p.plugin_loaded("search_tweaks_spellcheck")
 
 
-@pytest.mark.ckan_config(
-    "ckan.plugins", "search_tweaks search_tweaks_spellcheck"
-)
+@pytest.mark.ckan_config("ckan.plugins", "search_tweaks search_tweaks_spellcheck")
 @pytest.mark.usefixtures("with_plugins", "with_request_context")
 class TestDidYouMeanSnippet:
     def test_empty_without_data(self):
         assert not tk.render("search_tweaks/did_you_mean.html").strip()
 
     def test_with_query(self, monkeypatch):
         expected = "hello"
@@ -37,17 +31,15 @@
         helper.assert_called()
         link = snippet.select_one("a")
         assert link.text.strip() == expected
         assert "q=" + expected in link["href"]
 
 
 @pytest.mark.ckanext_search_tweaks_modified_schema
-@pytest.mark.ckan_config(
-    "ckan.plugins", "search_tweaks search_tweaks_spellcheck"
-)
+@pytest.mark.ckan_config("ckan.plugins", "search_tweaks search_tweaks_spellcheck")
 @pytest.mark.usefixtures("with_plugins", "clean_db", "clean_index")
 class TestHelper:
     def test_recommendations(self):
         Dataset(title="Pick this")
         Dataset(notes="Pick this")
         Dataset(title="Do not touch me")
         helper = tk.h.spellcheck_did_you_mean
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext/search_tweaks/tests/test_plugin.py` & `ckanext-search-tweaks-0.5.0/ckanext/search_tweaks/tests/test_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
-import ckan.plugins as p
 import ckan.lib.search.query as query
+import ckan.plugins as p
 
-from ckanext.search_tweaks import CONFIG_PREFER_BOOST
 import ckanext.search_tweaks.plugin as plugin
+from ckanext.search_tweaks import CONFIG_PREFER_BOOST
 
 
 @pytest.mark.usefixtures("with_plugins")
 def test_plugin_loaded():
     assert p.plugin_loaded("search_tweaks")
 
 
@@ -59,70 +59,58 @@
         assert search(q="hello:world")["q"] == "hello:world"
         assert search(q="hello AND world")["q"] == "hello AND world"
 
     @pytest.mark.ckan_config(plugin.CONFIG_FUZZY_KEEP_ORIGINAL, False)
     @pytest.mark.ckan_config(plugin.CONFIG_FUZZY, "on")
     @pytest.mark.parametrize("distance", [1, 2])
     def test_fuzzy_enabled(self, search, distance, ckan_config, monkeypatch):
-        monkeypatch.setitem(
-            ckan_config, plugin.CONFIG_FUZZY_DISTANCE, distance
-        )
+        monkeypatch.setitem(ckan_config, plugin.CONFIG_FUZZY_DISTANCE, distance)
         assert search()["q"] == "*:*"
         assert search(q="hello")["q"] == f"hello~{distance}"
+        assert search(q="hello world")["q"] == f"hello~{distance} world~{distance}"
+        assert search(q="hello:world")["q"] == "hello:world"
         assert (
-            search(q="hello world")["q"]
-            == f"hello~{distance} world~{distance}"
-        )
-        assert search(q="hello:world")["q"] == f"hello:world"
-        assert (
-            search(q="hello AND world")["q"]
-            == f"hello~{distance} AND world~{distance}"
+            search(q="hello AND world")["q"] == f"hello~{distance} AND world~{distance}"
         )
 
     @pytest.mark.ckan_config(plugin.CONFIG_FUZZY, "on")
     @pytest.mark.parametrize("distance", [-10, -1, 0])
     def test_fuzzy_enabled_with_too_low_distance(
         self, search, distance, ckan_config, monkeypatch
     ):
-        monkeypatch.setitem(
-            ckan_config, plugin.CONFIG_FUZZY_DISTANCE, distance
-        )
+        monkeypatch.setitem(ckan_config, plugin.CONFIG_FUZZY_DISTANCE, distance)
         assert search(q="")["q"] == "*:*"
         assert search(q="hello")["q"] == "hello"
         assert search(q="hello world")["q"] == "hello world"
         assert search(q="hello:world")["q"] == "hello:world"
         assert search(q="hello AND world")["q"] == "hello AND world"
 
     @pytest.mark.ckan_config(plugin.CONFIG_FUZZY_KEEP_ORIGINAL, False)
     @pytest.mark.ckan_config(plugin.CONFIG_FUZZY, "on")
     @pytest.mark.parametrize("distance", [3, 20, 111])
     def test_fuzzy_enabled_with_too_high_distance(
         self, search, distance, ckan_config, monkeypatch
     ):
-        monkeypatch.setitem(
-            ckan_config, plugin.CONFIG_FUZZY_DISTANCE, distance
-        )
+        monkeypatch.setitem(ckan_config, plugin.CONFIG_FUZZY_DISTANCE, distance)
         assert search()["q"] == "*:*"
         assert search(q="hello")["q"] == "hello~2"
         assert search(q="hello world")["q"] == "hello~2 world~2"
         assert search(q="hello:world")["q"] == "hello:world"
         assert search(q="hello AND world")["q"] == "hello~2 AND world~2"
 
     @pytest.mark.ckan_config(plugin.CONFIG_FUZZY, "on")
     @pytest.mark.parametrize("distance", [1, 2])
     def test_fuzzy_keep_original_query(
         self, search, distance, ckan_config, monkeypatch
     ):
-        monkeypatch.setitem(
-            ckan_config, plugin.CONFIG_FUZZY_DISTANCE, distance
-        )
+        monkeypatch.setitem(ckan_config, plugin.CONFIG_FUZZY_DISTANCE, distance)
         assert search()["q"] == "*:*"
         assert search(q="hello")["q"] == f"(hello~{distance}) OR (hello)"
         assert (
             search(q="hello world")["q"]
             == f"(hello~{distance} world~{distance}) OR (hello world)"
         )
-        assert search(q="hello:world")["q"] == f"hello:world"
+        assert search(q="hello:world")["q"] == "hello:world"
         assert (
             search(q="hello AND world")["q"]
             == f"(hello~{distance} AND world~{distance}) OR (hello AND world)"
         )
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/PKG-INFO` & `ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-search-tweaks
-Version: 0.4.12
+Version: 0.5.0
 Home-page: https://github.com/DataShades/ckanext-search-tweaks
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/SOURCES.txt` & `ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/ckanext_search_tweaks.egg-info/entry_points.txt` & `ckanext-search-tweaks-0.5.0/ckanext_search_tweaks.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/setup.cfg` & `ckanext-search-tweaks-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-search-tweaks-0.4.12/setup.py` & `ckanext-search-tweaks-0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,113 +1,97 @@
 # -*- coding: utf-8 -*-
 # Always prefer setuptools over distutils
-from setuptools import setup, find_packages
 from codecs import open  # To use a consistent encoding
 from os import path
 
+from setuptools import find_packages, setup
+
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the relevant file
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='''ckanext-search-tweaks''',
-
+    name="""ckanext-search-tweaks""",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='0.4.12',
-
-    description='''''',
+    version="0.5.0",
+    description="""""",
     long_description=long_description,
     long_description_content_type="text/markdown",
-
     # The project's main homepage.
-    url='https://github.com/DataShades/ckanext-search-tweaks',
-
+    url="https://github.com/DataShades/ckanext-search-tweaks",
     # Author details
-    author='''Sergey Motornyuk''',
-    author_email='''sergey.motornyuk@linkdigital.com.au''',
-
+    author="""Sergey Motornyuk""",
+    author_email="""sergey.motornyuk@linkdigital.com.au""",
     # Choose your license
-    license='AGPL',
-
+    license="AGPL",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
         # 3 - Alpha
         # 4 - Beta
         # 5 - Production/Stable
-        'Development Status :: 4 - Beta',
-
+        "Development Status :: 4 - Beta",
         # Pick your license as you wish (should match "license" above)
-        'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
-
+        "License :: OSI Approved ::"
+        + " GNU Affero General Public License v3 or later (AGPLv3+)",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2.7',
+        "Programming Language :: Python :: 2.7",
     ],
-
-
     # What does your project relate to?
-    keywords='''CKAN''',
-
+    keywords="""CKAN""",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
-    packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
-        namespace_packages=['ckanext'],
-
+    packages=find_packages(exclude=["contrib", "docs", "tests*"]),
+    namespace_packages=["ckanext"],
     install_requires=[
-      # CKAN extensions should not list dependencies here, but in a separate
-      # ``requirements.txt`` file.
-      #
-      # http://docs.ckan.org/en/latest/extensions/best-practices.html
-      # add-third-party-libraries-to-requirements-txt
+        # CKAN extensions should not list dependencies here, but in a separate
+        # ``requirements.txt`` file.
+        #
+        # http://docs.ckan.org/en/latest/extensions/best-practices.html
+        # add-third-party-libraries-to-requirements-txt
         "freezegun",
         "typing_extensions",
     ],
     python_requires=">=3.7",
-    extras_require={
-        "advanced-search": []
-    },
+    extras_require={"advanced-search": []},
     # If there are data files included in your packages that need to be
     # installed, specify them here.  If using Python 2.6 or less, then these
     # have to be included in MANIFEST.in as well.
     include_package_data=True,
-    package_data={
-    },
-
+    package_data={},
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages.
     # see http://docs.python.org/3.4/distutils/setupscript.html
     # installing-additional-files
     # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
     data_files=[],
-
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
-    entry_points='''
+    entry_points="""
         [ckan.plugins]
         search_tweaks=ckanext.search_tweaks.plugin:SearchTweaksPlugin
         search_tweaks_query_relevance=ckanext.search_tweaks.query_relevance.plugin:QueryRelevancePlugin
         search_tweaks_field_relevance=ckanext.search_tweaks.field_relevance.plugin:FieldRelevancePlugin
         search_tweaks_spellcheck=ckanext.search_tweaks.spellcheck.plugin:SpellcheckPlugin
         search_tweaks_advanced_search=ckanext.search_tweaks.advanced_search.plugin:AdvancedSearchPlugin
 
         [babel.extractors]
         ckan = ckan.lib.extract:extract_ckan
-    ''',
-
+    """,
     # If you are changing from the default layout of your extension, you may
     # have to change the message extractors, you can read more about babel
     # message extraction at
     # http://babel.pocoo.org/docs/messages/#extraction-method-mapping-and-configuration
     message_extractors={
-        'ckanext': [
-            ('**.py', 'python', None),
-            ('**.js', 'javascript', None),
-            ('**/templates/**.html', 'ckan', None),
+        "ckanext": [
+            ("**.py", "python", None),
+            ("**.js", "javascript", None),
+            ("**/templates/**.html", "ckan", None),
         ],
-    }
+    },
 )
```

