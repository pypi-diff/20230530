# Comparing `tmp/emotional-0.2.1.tar.gz` & `tmp/emotional-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotional-0.2.1.tar", last modified: Sat May 27 23:26:59 2023, max compression
+gzip compressed data, was "emotional-0.3.0.tar", last modified: Tue May 30 16:28:29 2023, max compression
```

## Comparing `emotional-0.2.1.tar` & `emotional-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1064 2022-09-16 23:07:01.534539 emotional-0.2.1/LICENSE
--rw-r--r--   0        0        0     2826 2023-05-26 13:49:15.611433 emotional-0.2.1/README.md
--rw-r--r--   0        0        0       98 2023-05-27 03:08:22.776955 emotional-0.2.1/emotional/__init__.py
--rw-r--r--   0        0        0      368 2023-05-27 02:52:07.423635 emotional-0.2.1/emotional/_compat.py
--rw-r--r--   0        0        0       26 2022-09-16 23:25:13.176855 emotional-0.2.1/emotional/_version.py
--rw-r--r--   0        0        0      534 2022-12-14 23:26:05.855303 emotional-0.2.1/emotional/changelog.py
--rw-r--r--   0        0        0     4867 2023-05-27 22:42:43.823053 emotional-0.2.1/emotional/config.py
--rw-r--r--   0        0        0     2864 2023-05-27 22:47:44.207044 emotional-0.2.1/emotional/defaults.py
--rw-r--r--   0        0        0     1476 2022-10-15 12:56:13.266978 emotional-0.2.1/emotional/github.py
--rw-r--r--   0        0        0     1644 2022-10-15 12:56:13.253645 emotional-0.2.1/emotional/gitlab.py
--rw-r--r--   0        0        0     1154 2022-10-15 12:56:13.246978 emotional-0.2.1/emotional/jira.py
--rw-r--r--   0        0        0     8199 2023-05-27 23:13:14.873415 emotional-0.2.1/emotional/plugin.py
--rw-r--r--   0        0        0     1038 2023-05-27 02:17:11.627205 emotional-0.2.1/emotional/templates/changelog.md.jinja
--rw-r--r--   0        0        0      679 2022-09-30 23:32:44.967373 emotional-0.2.1/emotional/templates/example.jinja
--rw-r--r--   0        0        0     1285 2022-09-29 23:33:47.497768 emotional-0.2.1/emotional/templates/info.md.jinja
--rw-r--r--   0        0        0      492 2023-05-27 03:38:07.830591 emotional-0.2.1/emotional/utils.py
--rw-r--r--   0        0        0     3155 2023-05-27 23:26:59.415051 emotional-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-19 23:34:18.625328 emotional-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1760 2023-05-26 13:49:14.058121 emotional-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     2326 2023-05-26 23:19:31.330807 emotional-0.2.1/tests/fixtures/changelogs/default.md
--rw-r--r--   0        0        0     2322 2023-05-27 02:17:11.627205 emotional-0.2.1/tests/fixtures/changelogs/group_by_scope.md
--rw-r--r--   0        0        0     2326 2023-05-27 02:17:11.627205 emotional-0.2.1/tests/fixtures/changelogs/release_emoji.md
--rw-r--r--   0        0        0     2585 2023-05-27 23:13:14.806748 emotional-0.2.1/tests/test_bump.py
--rw-r--r--   0        0        0    20365 2023-05-27 03:02:52.106089 emotional-0.2.1/tests/test_changelog.py
--rw-r--r--   0        0        0     5595 2023-05-27 03:43:41.674835 emotional-0.2.1/tests/test_commit.py
--rw-r--r--   0        0        0     1381 2022-12-18 16:24:15.888821 emotional-0.2.1/tests/test_config.py
--rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.885488 emotional-0.2.1/tests/test_github.py
--rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.888821 emotional-0.2.1/tests/test_gitlab.py
--rw-r--r--   0        0        0     2588 2022-12-18 16:24:15.888821 emotional-0.2.1/tests/test_jira.py
--rw-r--r--   0        0        0      644 2023-05-27 03:02:52.109422 emotional-0.2.1/tests/test_plugin.py
--rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 emotional-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-09-16 23:07:01.534539 emotional-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2981 2023-05-29 23:31:26.683409 emotional-0.3.0/README.md
+-rw-r--r--   0        0        0       98 2023-05-27 03:08:22.776955 emotional-0.3.0/emotional/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-27 02:52:07.423635 emotional-0.3.0/emotional/_compat.py
+-rw-r--r--   0        0        0       26 2022-09-16 23:25:13.176855 emotional-0.3.0/emotional/_version.py
+-rw-r--r--   0        0        0      534 2022-12-14 23:26:05.855303 emotional-0.3.0/emotional/changelog.py
+-rw-r--r--   0        0        0     5016 2023-05-29 23:31:26.683409 emotional-0.3.0/emotional/config.py
+-rw-r--r--   0        0        0     2864 2023-05-27 22:47:44.207044 emotional-0.3.0/emotional/defaults.py
+-rw-r--r--   0        0        0     1476 2022-10-15 12:56:13.266978 emotional-0.3.0/emotional/github.py
+-rw-r--r--   0        0        0     1644 2022-10-15 12:56:13.253645 emotional-0.3.0/emotional/gitlab.py
+-rw-r--r--   0        0        0     1154 2022-10-15 12:56:13.246978 emotional-0.3.0/emotional/jira.py
+-rw-r--r--   0        0        0     8199 2023-05-27 23:13:14.873415 emotional-0.3.0/emotional/plugin.py
+-rw-r--r--   0        0        0     1290 2023-05-29 23:31:26.683409 emotional-0.3.0/emotional/templates/changelog.md.jinja
+-rw-r--r--   0        0        0      679 2022-09-30 23:32:44.967373 emotional-0.3.0/emotional/templates/example.jinja
+-rw-r--r--   0        0        0     1285 2023-05-29 23:36:13.810761 emotional-0.3.0/emotional/templates/info.md.jinja
+-rw-r--r--   0        0        0      492 2023-05-27 03:38:07.830591 emotional-0.3.0/emotional/utils.py
+-rw-r--r--   0        0        0     3155 2023-05-30 16:28:29.450905 emotional-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-19 23:34:18.625328 emotional-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1760 2023-05-26 13:49:14.058121 emotional-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     2326 2023-05-26 23:19:31.330807 emotional-0.3.0/tests/fixtures/changelogs/default.md
+-rw-r--r--   0        0        0     2322 2023-05-27 02:17:11.627205 emotional-0.3.0/tests/fixtures/changelogs/group_by_scope.md
+-rw-r--r--   0        0        0     2326 2023-05-29 23:19:47.101655 emotional-0.3.0/tests/fixtures/changelogs/order_by_scope.md
+-rw-r--r--   0        0        0     2326 2023-05-27 02:17:11.627205 emotional-0.3.0/tests/fixtures/changelogs/release_emoji.md
+-rw-r--r--   0        0        0     2585 2023-05-27 23:13:14.806748 emotional-0.3.0/tests/test_bump.py
+-rw-r--r--   0        0        0    20509 2023-05-29 23:35:29.773993 emotional-0.3.0/tests/test_changelog.py
+-rw-r--r--   0        0        0     5595 2023-05-27 03:43:41.674835 emotional-0.3.0/tests/test_commit.py
+-rw-r--r--   0        0        0     1381 2022-12-18 16:24:15.888821 emotional-0.3.0/tests/test_config.py
+-rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.885488 emotional-0.3.0/tests/test_github.py
+-rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.888821 emotional-0.3.0/tests/test_gitlab.py
+-rw-r--r--   0        0        0     2588 2022-12-18 16:24:15.888821 emotional-0.3.0/tests/test_jira.py
+-rw-r--r--   0        0        0      644 2023-05-27 03:02:52.109422 emotional-0.3.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 emotional-0.3.0/PKG-INFO
```

### Comparing `emotional-0.2.1/LICENSE` & `emotional-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/README.md` & `emotional-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,23 @@
 
 As a starter, remember that all [Commitizen configuration][commitizen-config]
 is available.
 
 ### Changelog
 
 By default, changes by types are kept in order of commit and ignore the scope for ordering.
-You can however force scope to be sorted first by setting `group_by_scope`:
+You can however force scope to be sorted first by setting `order_by_scope`:
+
+```toml
+[tool.commitizen]
+name = "emotional"
+order_by_scope = true
+```
+
+You can also group changes into subsections by scope by setting `group_by_scope`:
 
 ```toml
 [tool.commitizen]
 name = "emotional"
 group_by_scope = true
 ```
```

### Comparing `emotional-0.2.1/emotional/changelog.py` & `emotional-0.3.0/emotional/changelog.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/emotional/config.py` & `emotional-0.3.0/emotional/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     github: str | None
 
     gitlab: str | None
 
     jira_url: str | None
     jira_prefixes: list[str] | None
 
+    order_by_scope: bool | None
     group_by_scope: bool | None
 
     release_emoji: str | None
 
 
 @dataclass
 class EmotionalConfig:
@@ -160,13 +161,17 @@
         return self.settings.get("jira_prefixes", [])
 
     @property
     def incremental(self) -> bool:
         return "--incremental" in sys.argv
 
     @property
+    def order_by_scope(self) -> bool:
+        return self.settings.get("order_by_scope") or False
+
+    @property
     def group_by_scope(self) -> bool:
-        return self.settings.get("group_by_scope", False)
+        return self.settings.get("group_by_scope") or False
 
     @property
     def release_emoji(self) -> str:
-        return self.settings.get("release_emoji", defaults.RELEASE_EMOJI)
+        return self.settings.get("release_emoji") or defaults.RELEASE_EMOJI
```

### Comparing `emotional-0.2.1/emotional/defaults.py` & `emotional-0.3.0/emotional/defaults.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/emotional/github.py` & `emotional-0.3.0/emotional/github.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/emotional/gitlab.py` & `emotional-0.3.0/emotional/gitlab.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/emotional/jira.py` & `emotional-0.3.0/emotional/jira.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/emotional/plugin.py` & `emotional-0.3.0/emotional/plugin.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/emotional/templates/changelog.md.jinja` & `emotional-0.3.0/emotional/templates/changelog.md.jinja`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,22 @@
 
 {% macro render_change(change, scope=True) -%}
 {%- if change.message %}
 - {% if scope and change.scope %}**{{ change.scope }}**: {% endif %}{{ change.message }}
 {%- endif %}
 {% endmacro %}
 
-{% if config.group_by_scope %}
+{% if config.order_by_scope %}
+{% for change in changes|rejectattr("scope", "none")|sort(attribute="scope",) %}
+{{ render_change(change) }}
+{% endfor %}
+{% for change in changes|selectattr("scope", "none") %}
+{{ render_change(change) }}
+{% endfor %}
+{% elif config.group_by_scope %}
 {% set ns = namespace(no_scope=false) %}
 {% for change in changes|selectattr("scope", "none") %}
 {{ render_change(change) }}
 {% if loop.last %}{% set ns.no_scope=true %}{% endif %}
 {% endfor %}
 {% for scope, changes in changes|rejectattr("scope", "none")|groupby("scope") -%}
 {% if ns.no_scope +%}
```

### Comparing `emotional-0.2.1/emotional/templates/example.jinja` & `emotional-0.3.0/emotional/templates/example.jinja`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/emotional/templates/info.md.jinja` & `emotional-0.3.0/emotional/templates/info.md.jinja`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/pyproject.toml` & `emotional-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dependencies = [
     "commitizen>=3.0",
     "typing-extensions>=4.4.0; python_version<'3.10'",
 ]
 dynamic = []
 requires-python = ">=3.7"
 readme = "README.md"
-version = "0.2.1"
+version = "0.3.0"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points."commitizen.plugin"]
 emotional = "emotional.plugin:Emotional"
```

### Comparing `emotional-0.2.1/tests/conftest.py` & `emotional-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/fixtures/changelogs/default.md` & `emotional-0.3.0/tests/fixtures/changelogs/default.md`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/fixtures/changelogs/group_by_scope.md` & `emotional-0.3.0/tests/fixtures/changelogs/group_by_scope.md`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/fixtures/changelogs/release_emoji.md` & `emotional-0.3.0/tests/fixtures/changelogs/release_emoji.md`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/test_bump.py` & `emotional-0.3.0/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/test_changelog.py` & `emotional-0.3.0/tests/test_changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,14 +544,19 @@
     return assertion
 
 
 def test_render_changelog_with_default_settings(assert_changelog):
     assert_changelog("default")
 
 
+@pytest.mark.settings(order_by_scope=True)
+def test_render_changelog_order_by_scope(assert_changelog):
+    assert_changelog("order_by_scope")
+
+
 @pytest.mark.settings(group_by_scope=True)
 def test_render_changelog_group_by_scope(assert_changelog):
     assert_changelog("group_by_scope")
 
 
 @pytest.mark.settings(release_emoji="🎉")
 def test_render_changelog_release_emoji(assert_changelog):
```

### Comparing `emotional-0.2.1/tests/test_commit.py` & `emotional-0.3.0/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/test_config.py` & `emotional-0.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/test_github.py` & `emotional-0.3.0/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/test_gitlab.py` & `emotional-0.3.0/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/test_jira.py` & `emotional-0.3.0/tests/test_jira.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/tests/test_plugin.py` & `emotional-0.3.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `emotional-0.2.1/PKG-INFO` & `emotional-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotional
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Commitizen plugin for conventional commit with emojis and integrations
 Author-Email: Axel H. <noirbizarre@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Requires-Dist: commitizen>=3.0
 Requires-Dist: typing-extensions>=4.4.0; python_version < "3.10"
 Description-Content-Type: text/markdown
@@ -35,15 +35,23 @@
 
 As a starter, remember that all [Commitizen configuration][commitizen-config]
 is available.
 
 ### Changelog
 
 By default, changes by types are kept in order of commit and ignore the scope for ordering.
-You can however force scope to be sorted first by setting `group_by_scope`:
+You can however force scope to be sorted first by setting `order_by_scope`:
+
+```toml
+[tool.commitizen]
+name = "emotional"
+order_by_scope = true
+```
+
+You can also group changes into subsections by scope by setting `group_by_scope`:
 
 ```toml
 [tool.commitizen]
 name = "emotional"
 group_by_scope = true
 ```
```

