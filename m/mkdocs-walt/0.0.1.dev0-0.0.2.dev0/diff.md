# Comparing `tmp/mkdocs-walt-0.0.1.dev0.tar.gz` & `tmp/mkdocs-walt-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-walt-0.0.1.dev0.tar", last modified: Tue May 30 02:15:26 2023, max compression
+gzip compressed data, was "mkdocs-walt-0.0.2.dev0.tar", last modified: Tue May 30 20:24:13 2023, max compression
```

## Comparing `mkdocs-walt-0.0.1.dev0.tar` & `mkdocs-walt-0.0.2.dev0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 02:15:26.780032 mkdocs-walt-0.0.1.dev0/
--rw-r--r--   0 sue        (501) staff       (20)      139 2023-05-29 21:22:40.000000 mkdocs-walt-0.0.1.dev0/MANIFEST.in
--rw-r--r--   0 sue        (501) staff       (20)      601 2023-05-30 02:15:26.779926 mkdocs-walt-0.0.1.dev0/PKG-INFO
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 02:15:26.779330 mkdocs-walt-0.0.1.dev0/mkdocs_walt.egg-info/
--rw-r--r--   0 sue        (501) staff       (20)      601 2023-05-30 02:15:26.000000 mkdocs-walt-0.0.1.dev0/mkdocs_walt.egg-info/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      329 2023-05-30 02:15:26.000000 mkdocs-walt-0.0.1.dev0/mkdocs_walt.egg-info/SOURCES.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-30 02:15:26.000000 mkdocs-walt-0.0.1.dev0/mkdocs_walt.egg-info/dependency_links.txt
--rw-r--r--   0 sue        (501) staff       (20)       28 2023-05-30 02:15:26.000000 mkdocs-walt-0.0.1.dev0/mkdocs_walt.egg-info/entry_points.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 21:29:31.000000 mkdocs-walt-0.0.1.dev0/mkdocs_walt.egg-info/not-zip-safe
--rw-r--r--   0 sue        (501) staff       (20)        7 2023-05-30 02:15:26.000000 mkdocs-walt-0.0.1.dev0/mkdocs_walt.egg-info/requires.txt
--rw-r--r--   0 sue        (501) staff       (20)        5 2023-05-30 02:15:26.000000 mkdocs-walt-0.0.1.dev0/mkdocs_walt.egg-info/top_level.txt
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-30 02:15:26.780066 mkdocs-walt-0.0.1.dev0/setup.cfg
--rw-r--r--   0 sue        (501) staff       (20)      970 2023-05-30 02:15:09.000000 mkdocs-walt-0.0.1.dev0/setup.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 02:15:26.779783 mkdocs-walt-0.0.1.dev0/walt/
--rw-r--r--   0 sue        (501) staff       (20)       29 2023-05-29 21:22:32.000000 mkdocs-walt-0.0.1.dev0/walt/__init__.py
--rw-r--r--   0 sue        (501) staff       (20)     1878 2023-05-30 01:56:13.000000 mkdocs-walt-0.0.1.dev0/walt/base.html
--rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-30 01:55:40.000000 mkdocs-walt-0.0.1.dev0/walt/main.html
--rw-r--r--   0 sue        (501) staff       (20)     3433 2023-05-30 01:57:17.000000 mkdocs-walt-0.0.1.dev0/walt/styles.css
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 20:24:13.981025 mkdocs-walt-0.0.2.dev0/
+-rw-r--r--   0 sue        (501) staff       (20)      139 2023-05-29 21:22:40.000000 mkdocs-walt-0.0.2.dev0/MANIFEST.in
+-rw-r--r--   0 sue        (501) staff       (20)      877 2023-05-30 20:24:13.980893 mkdocs-walt-0.0.2.dev0/PKG-INFO
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 20:24:13.980001 mkdocs-walt-0.0.2.dev0/mkdocs_walt.egg-info/
+-rw-r--r--   0 sue        (501) staff       (20)      877 2023-05-30 20:24:13.000000 mkdocs-walt-0.0.2.dev0/mkdocs_walt.egg-info/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)      344 2023-05-30 20:24:13.000000 mkdocs-walt-0.0.2.dev0/mkdocs_walt.egg-info/SOURCES.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-30 20:24:13.000000 mkdocs-walt-0.0.2.dev0/mkdocs_walt.egg-info/dependency_links.txt
+-rw-r--r--   0 sue        (501) staff       (20)       28 2023-05-30 20:24:13.000000 mkdocs-walt-0.0.2.dev0/mkdocs_walt.egg-info/entry_points.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 21:29:31.000000 mkdocs-walt-0.0.2.dev0/mkdocs_walt.egg-info/not-zip-safe
+-rw-r--r--   0 sue        (501) staff       (20)        7 2023-05-30 20:24:13.000000 mkdocs-walt-0.0.2.dev0/mkdocs_walt.egg-info/requires.txt
+-rw-r--r--   0 sue        (501) staff       (20)        5 2023-05-30 20:24:13.000000 mkdocs-walt-0.0.2.dev0/mkdocs_walt.egg-info/top_level.txt
+-rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-30 20:24:13.981062 mkdocs-walt-0.0.2.dev0/setup.cfg
+-rw-r--r--   0 sue        (501) staff       (20)     1246 2023-05-30 18:34:29.000000 mkdocs-walt-0.0.2.dev0/setup.py
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 20:24:13.980715 mkdocs-walt-0.0.2.dev0/walt/
+-rw-r--r--   0 sue        (501) staff       (20)       29 2023-05-29 21:22:32.000000 mkdocs-walt-0.0.2.dev0/walt/__init__.py
+-rw-r--r--   0 sue        (501) staff       (20)     2035 2023-05-30 17:08:24.000000 mkdocs-walt-0.0.2.dev0/walt/base.html
+-rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-30 01:55:40.000000 mkdocs-walt-0.0.2.dev0/walt/main.html
+-rw-r--r--   0 sue        (501) staff       (20)     5628 2023-05-30 19:55:41.000000 mkdocs-walt-0.0.2.dev0/walt/styles.css
+-rw-r--r--   0 sue        (501) staff       (20)      423 2023-05-30 20:14:49.000000 mkdocs-walt-0.0.2.dev0/walt/writ.html
```

### Comparing `mkdocs-walt-0.0.1.dev0/setup.py` & `mkdocs-walt-0.0.2.dev0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1-dev'
+VERSION = '0.0.2-dev'
 
 LONG_DESCRIPTION = '''
-# mkdocs-walt: a mininal documentation theme for MkDocs
+# mkdocs-walt: a minimal documentation theme for MkDocs
+
+Walt is a minimal documentation theme that is best suited for single page websites.
 
 ## Installation
 
 ```sh
 pip install mkdocs-walt
 ```
 
@@ -18,14 +20,20 @@
 
 ```yaml
 theme:
   name: walt
 ```
 
 See the [full usage example](https://github.com/codesue/walt/examples/mkdocs-walt).
+
+## Acknowledgements
+
+Walt uses [writ.css](https://github.com/programble/writ/tree/master) for styles
+and [Catppuccin](https://github.com/catppuccin/catppuccin) for dark mode
+color palettes.
 '''
 
 setup(
     name='mkdocs-walt',
     version=VERSION,
     author='Suzen Fylke',
     author_email='codesue@users.noreply.github.com',
```

### Comparing `mkdocs-walt-0.0.1.dev0/walt/base.html` & `mkdocs-walt-0.0.2.dev0/walt/base.html`

 * *Files 7% similar despite different names*

```diff
@@ -29,18 +29,25 @@
 
     {%- block extrahead %} {% endblock %}
   </head>
   <body>
     <a href="#skip" class="visually-hidden">Skip to main content</a>
     {%- block header %}
     {%- endblock %}
+    {%- block main %}
     <main id="skip">
       {{ page.content }}
     </main>
+    {%- endblock %}
     {%- block footer %}
+    <footer>
+      {%- if config.copyright %}
+      <p>{{ config.copyright }}</p>
+      {%- endif %}
+    </footer>
     {%- endblock %}
 
     {%- block scripts %}
     {% for path in config.extra_javascript %}
     <script src="{{ path|url }}"></script>
     {% endfor %}
     {%- endblock %}
```

#### html2text {}

```diff
@@ -8,11 +8,14 @@
 {% endif %}
 
 
  {%- endblock %} {%- block styles %}
 css"|url }}"> {% for path in config.extra_css %}
  {% endfor %} {%- endblock %} {%- block libs %} {%- endblock %} {%- block
 extrahead %} {% endblock %}
-Skip_to_main_content {%- block header %} {%- endblock %}  {{ page.content }}
-{%- block footer %} {%- endblock %} {%- block scripts %} {% for path in
+Skip_to_main_content {%- block header %} {%- endblock %} {%- block main %}  {
+{ page.content }}  {%- endblock %} {%- block footer %}  {%- if config.copyright
+%}
+{{ config.copyright }}
+{%- endif %}  {%- endblock %} {%- block scripts %} {% for path in
 config.extra_javascript %}
  {% endfor %} {%- endblock %}
```

