# Comparing `tmp/pautobot-0.0.5.tar.gz` & `tmp/pautobot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pautobot-0.0.5.tar", last modified: Mon May 29 19:20:52 2023, max compression
+gzip compressed data, was "pautobot-0.0.6.tar", last modified: Tue May 30 01:50:54 2023, max compression
```

## Comparing `pautobot-0.0.5.tar` & `pautobot-0.0.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.800531 pautobot-0.0.5/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       71 2023-05-29 18:54:55.000000 pautobot-0.0.5/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-29 19:20:52.800382 pautobot-0.0.5/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1518 2023-05-29 19:20:36.000000 pautobot-0.0.5/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.794236 pautobot-0.0.5/pautobot/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-05-29 14:28:20.000000 pautobot-0.0.5/pautobot/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1517 2023-05-29 19:17:04.000000 pautobot-0.0.5/pautobot/app.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)       47 2023-05-29 19:18:36.000000 pautobot-0.0.5/pautobot/app_info.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      418 2023-05-29 18:58:38.000000 pautobot-0.0.5/pautobot/constants.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5057 2023-05-29 18:38:03.000000 pautobot-0.0.5/pautobot/engine.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      243 2023-05-29 16:06:06.000000 pautobot-0.0.5/pautobot/example.env
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.795725 pautobot-0.0.5/pautobot/frontend-dist/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4096 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/404.html
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.792008 pautobot-0.0.5/pautobot/frontend-dist/_next/
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.792346 pautobot-0.0.5/pautobot/frontend-dist/_next/static/
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.796011 pautobot-0.0.5/pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      282 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/_buildManifest.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)       77 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/_ssgManifest.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.796711 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/
--rw-r--r--   0 vietanhdev   (501) staff       (20)   141052 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    95653 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.797072 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      727 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)      247 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26587 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/index-62fdb7c7217c2fea.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    91460 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1430 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.797216 pautobot-0.0.5/pautobot/frontend-dist/_next/static/css/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    32027 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/css/a4a6346dff75e1d3.css
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.800207 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8852 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8972 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8992 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3528 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3492 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9012 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9392 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3572 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9564 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10728 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9276 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9004 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10656 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9144 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8828 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9036 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10428 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3488 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3576 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9604 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10632 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3516 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10840 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10808 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
--rw-rw-r--   0 vietanhdev   (501) staff       (20)    15406 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/favicon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9488 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/index.html
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2925 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/loading.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26848 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/pautobot.png
--rwxr-xr-x   0 vietanhdev   (501) staff       (20)     6468 2023-05-29 16:52:48.000000 pautobot-0.0.5/pautobot/ingest.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)       72 2023-05-29 14:44:03.000000 pautobot-0.0.5/pautobot/models.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2437 2023-05-29 19:13:47.000000 pautobot-0.0.5/pautobot/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.795052 pautobot-0.0.5/pautobot.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2940 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      248 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        9 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      266 2023-05-29 14:25:31.000000 pautobot-0.0.5/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-05-29 19:20:52.800568 pautobot-0.0.5/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2436 2023-05-29 19:08:44.000000 pautobot-0.0.5/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.035944 pautobot-0.0.6/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       71 2023-05-29 18:54:55.000000 pautobot-0.0.6/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-30 01:50:54.035774 pautobot-0.0.6/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1518 2023-05-29 19:20:36.000000 pautobot-0.0.6/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.028181 pautobot-0.0.6/pautobot/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-05-29 14:28:20.000000 pautobot-0.0.6/pautobot/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1579 2023-05-30 01:37:08.000000 pautobot-0.0.6/pautobot/app.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       47 2023-05-30 01:49:59.000000 pautobot-0.0.6/pautobot/app_info.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      418 2023-05-29 18:58:38.000000 pautobot-0.0.6/pautobot/constants.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5976 2023-05-30 01:39:50.000000 pautobot-0.0.6/pautobot/engine.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      243 2023-05-29 16:06:06.000000 pautobot-0.0.6/pautobot/example.env
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.029665 pautobot-0.0.6/pautobot/frontend-dist/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4096 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/404.html
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.025577 pautobot-0.0.6/pautobot/frontend-dist/_next/
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.025910 pautobot-0.0.6/pautobot/frontend-dist/_next/static/
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.030210 pautobot-0.0.6/pautobot/frontend-dist/_next/static/LGBTTPTxeYzvA3cKI-195/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      282 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/LGBTTPTxeYzvA3cKI-195/_buildManifest.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       77 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/LGBTTPTxeYzvA3cKI-195/_ssgManifest.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.031304 pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   141052 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    95653 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.031786 pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/pages/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      727 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      247 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26515 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/pages/index-07647c380718ba41.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    91460 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1430 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.031947 pautobot-0.0.6/pautobot/frontend-dist/_next/static/css/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    32128 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/css/e5e3a6d239ad5709.css
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.035524 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8852 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8972 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8992 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3528 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3492 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9012 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9392 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3572 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9564 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10728 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9276 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9004 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10656 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9144 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8828 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9036 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10428 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3488 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3576 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9604 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10632 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3516 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10840 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10808 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
+-rw-rw-r--   0 vietanhdev   (501) staff       (20)    15406 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/favicon.ico
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9353 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/index.html
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2925 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/loading.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26848 2023-05-30 01:50:50.000000 pautobot-0.0.6/pautobot/frontend-dist/pautobot.png
+-rwxr-xr-x   0 vietanhdev   (501) staff       (20)     6468 2023-05-29 16:52:48.000000 pautobot-0.0.6/pautobot/ingest.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-30 01:30:40.000000 pautobot-0.0.6/pautobot/models.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2437 2023-05-29 19:13:47.000000 pautobot-0.0.6/pautobot/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-30 01:50:54.028945 pautobot-0.0.6/pautobot.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-30 01:50:54.000000 pautobot-0.0.6/pautobot.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2940 2023-05-30 01:50:54.000000 pautobot-0.0.6/pautobot.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-05-30 01:50:54.000000 pautobot-0.0.6/pautobot.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-30 01:50:54.000000 pautobot-0.0.6/pautobot.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      248 2023-05-30 01:50:54.000000 pautobot-0.0.6/pautobot.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        9 2023-05-30 01:50:54.000000 pautobot-0.0.6/pautobot.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      266 2023-05-29 14:25:31.000000 pautobot-0.0.6/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-05-30 01:50:54.035993 pautobot-0.0.6/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2436 2023-05-29 19:08:44.000000 pautobot-0.0.6/setup.py
```

### Comparing `pautobot-0.0.5/PKG-INFO` & `pautobot-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pautobot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Private AutoGPT Robot - Your private task assistant with GPT!
 Home-page: https://github.com/vietanhdev/pautobot
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: Apache License 2.0
 Keywords: Personal Assistant,Automation,GPT,LLM,PrivateGPT
 Classifier: Natural Language :: English
```

### Comparing `pautobot-0.0.5/README.md` & `pautobot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/app.py` & `pautobot-0.0.6/pautobot/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,35 +15,36 @@
 def main():
     init_env_file()
     download_model_if_needed()
     static_folder = "pautobot-data/frontend-dist"
     extract_frontend_dist(static_folder)
 
     # PautoBot engine
-    engine = PautoBotEngine(mode=BotMode.CHAT)
+    engine = PautoBotEngine(mode=BotMode.QA)
 
     # Backend app
     app = FastAPI()
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["*"],
         allow_methods=["*"],
         allow_headers=["*"],
     )
 
     @app.post("/api/ask")
     async def ask(query: Query, background_tasks: BackgroundTasks):
+        engine.check_query(query.mode, query.query)
         if engine.current_answer["status"] == BotStatus.THINKING:
             raise Exception("I am still thinking! Please wait.")
         engine.current_answer = {
             "status": BotStatus.THINKING,
             "answer": "",
             "docs": [],
         }
-        background_tasks.add_task(engine.query, query.query)
+        background_tasks.add_task(engine.query, query.mode, query.query)
         return {"message": "Query received"}
 
     @app.get("/api/get_answer")
     async def get_answer():
         return engine.get_answer()
 
     app.mount(
```

### Comparing `pautobot-0.0.5/pautobot/engine.py` & `pautobot-0.0.6/pautobot/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             "status": BotStatus.READY,
             "answer": "",
             "docs": [],
         }
         self.answer_q = queue.Queue()
 
         embeddings_model_name = os.environ.get("EMBEDDINGS_MODEL_NAME")
-        persist_directory = os.environ.get("PERSIST_DIRECTORY")
+        self.persist_directory = os.environ.get("PERSIST_DIRECTORY")
         model_path = os.environ.get("MODEL_PATH")
         model_n_ctx = os.environ.get("MODEL_N_CTX")
         target_source_chunks = int(os.environ.get("TARGET_SOURCE_CHUNKS", 4))
 
         # Prepare the LLM
         if self.model_type == "LlamaCpp":
             self.llm = LlamaCpp(
@@ -66,47 +66,59 @@
             )
         else:
             print(f"Model {model_type} not supported!")
             exit(1)
 
         # Prepare the retriever
         self.qa_instance = None
+        self.qa_instance_error = None
         if mode == BotMode.CHAT:
             return
         try:
             embeddings = HuggingFaceEmbeddings(
                 model_name=embeddings_model_name
             )
             db = Chroma(
-                persist_directory=persist_directory,
+                persist_directory=self.persist_directory,
                 embedding_function=embeddings,
                 client_settings=CHROMA_SETTINGS,
             )
             retriever = db.as_retriever(
                 search_kwargs={"k": target_source_chunks}
             )
             self.qa_instance = RetrievalQA.from_chain_type(
                 llm=self.llm,
                 chain_type="stuff",
                 retriever=retriever,
                 return_source_documents=True,
             )
-            self.mode = BotMode.QA
         except Exception as e:
             print(f"Error while initializing retriever: {e}")
             print("Switching to chat mode...")
-            self.mode = BotMode.CHAT
+            self.qa_instance_error = f"Error while initializing retriever! Please prepare your documents in `{self.persist_directory}` and run: python -m pautobot.ingest"
 
-    def query(self, query):
+    def check_query(self, mode, query):
+        if mode == BotMode.QA and self.mode == BotMode.CHAT:
+            raise Exception("PautobotEngine was initialized in chat mode! Please restart with QA mode.")
+        elif mode == BotMode.QA and self.qa_instance is None:
+            raise Exception(self.qa_instance_error)
+
+    def query(self, mode, query):
+        self.check_query(mode, query)
+        if mode is None:
+            mode = self.mode
+        if mode == BotMode.QA and self.qa_instance is None:
+            print(self.qa_instance_error)
+            mode = BotMode.CHAT
         self.current_answer = {
             "status": BotStatus.THINKING,
             "answer": "",
             "docs": [],
         }
-        if self.mode == BotMode.QA:
+        if mode == BotMode.QA:
             try:
                 print("Received query: ", query)
                 print("Thinking...")
                 res = self.qa_instance(query)
                 answer, docs = (
                     res["result"],
                     res["source_documents"],
@@ -122,17 +134,20 @@
                 self.current_answer = {
                     "status": BotStatus.READY,
                     "answer": answer,
                     "docs": doc_json,
                 }
             except Exception as e:
                 print("Error during thinking: ", e)
+                answer = "Error during thinking! Please try again."
+                if "Index not found" in str(e):
+                    answer = f"Index not found! Please prepare your documents in `{self.persist_directory}` and run: python -m pautobot.ingest"
                 self.current_answer = {
                     "status": BotStatus.READY,
-                    "answer": "Error during thinking! Please try again.",
+                    "answer": answer,
                     "docs": None,
                 }
         else:
             try:
                 print("Received query: ", query)
                 print("Thinking...")
                 answer = self.llm(query)
```

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/404.html` & `pautobot-0.0.6/pautobot/frontend-dist/404.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/a4a6346dff75e1d3.css" as="style"/><link rel="stylesheet" href="/_next/static/css/a4a6346dff75e1d3.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/Dl9fVCNsnbVyvPy7nTli-/_buildManifest.js" defer=""></script><script src="/_next/static/Dl9fVCNsnbVyvPy7nTli-/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"Dl9fVCNsnbVyvPy7nTli-","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/e5e3a6d239ad5709.css" as="style"/><link rel="stylesheet" href="/_next/static/css/e5e3a6d239ad5709.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/LGBTTPTxeYzvA3cKI-195/_buildManifest.js" defer=""></script><script src="/_next/static/LGBTTPTxeYzvA3cKI-195/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"LGBTTPTxeYzvA3cKI-195","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/index-62fdb7c7217c2fea.js` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/pages/index-07647c380718ba41.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -109,15 +109,15 @@
             };
             let c = e => "number" == typeof e && !isNaN(e),
                 d = e => "string" == typeof e,
                 u = e => "function" == typeof e,
                 m = e => d(e) || u(e) ? e : null,
                 g = e => (0, a.isValidElement)(e) || d(e) || u(e) || c(e);
 
-            function p(e) {
+            function f(e) {
                 let {
                     enter: t,
                     exit: n,
                     appendPosition: r = !1,
                     collapse: s = !0,
                     collapseDuration: o = 300
                 } = e;
@@ -125,20 +125,20 @@
                     let {
                         children: l,
                         position: i,
                         preventExitTransition: c,
                         done: d,
                         nodeRef: u,
                         isIn: m
-                    } = e, g = r ? `${t}--${i}` : t, p = r ? `${n}--${i}` : n, f = (0, a.useRef)(0);
+                    } = e, g = r ? `${t}--${i}` : t, f = r ? `${n}--${i}` : n, p = (0, a.useRef)(0);
                     return (0, a.useLayoutEffect)(() => {
                         let e = u.current,
                             t = g.split(" "),
                             n = r => {
-                                r.target === u.current && (e.dispatchEvent(new Event("d")), e.removeEventListener("animationend", n), e.removeEventListener("animationcancel", n), 0 === f.current && "animationcancel" !== r.type && e.classList.remove(...t))
+                                r.target === u.current && (e.dispatchEvent(new Event("d")), e.removeEventListener("animationend", n), e.removeEventListener("animationcancel", n), 0 === p.current && "animationcancel" !== r.type && e.classList.remove(...t))
                             };
                         e.classList.add(...t), e.addEventListener("animationend", n), e.addEventListener("animationcancel", n)
                     }, []), (0, a.useEffect)(() => {
                         let e = u.current,
                             t = () => {
                                 e.removeEventListener("animationend", t), s ? function(e, t, n) {
                                     void 0 === n && (n = 300);
@@ -149,20 +149,20 @@
                                     requestAnimationFrame(() => {
                                         a.minHeight = "initial", a.height = r + "px", a.transition = `all ${n}ms`, requestAnimationFrame(() => {
                                             a.height = "0", a.padding = "0", a.margin = "0", setTimeout(t, n)
                                         })
                                     })
                                 }(e, d, o) : d()
                             };
-                        m || (c ? t() : (f.current = 1, e.className += ` ${p}`, e.addEventListener("animationend", t)))
+                        m || (c ? t() : (p.current = 1, e.className += ` ${f}`, e.addEventListener("animationend", t)))
                     }, [m]), a.createElement(a.Fragment, null, l)
                 }
             }
 
-            function f(e, t) {
+            function p(e, t) {
                 return null != e ? {
                     content: e.content,
                     containerId: e.props.containerId,
                     id: e.props.toastId,
                     theme: e.props.theme,
                     type: e.props.type,
                     data: e.props.data || {},
@@ -273,55 +273,55 @@
                     viewBox: "0 0 14 16"
                 }, a.createElement("path", {
                     fillRule: "evenodd",
                     d: "M7.71 8.23l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75L1 11.98l3.75-3.75L1 4.48 2.48 3l3.75 3.75L9.98 3l1.48 1.48-3.75 3.75z"
                 })))
             }
 
-            function w(e) {
+            function E(e) {
                 let {
                     delay: t,
                     isRunning: n,
                     closeToast: r,
                     type: s = "default",
                     hide: o,
                     className: l,
                     style: c,
                     controlledProgress: d,
                     progress: m,
                     rtl: g,
-                    isIn: p,
-                    theme: f
+                    isIn: f,
+                    theme: p
                 } = e, h = o || d && 0 === m, y = {
                     ...c,
                     animationDuration: `${t}ms`,
                     animationPlayState: n ? "running" : "paused",
                     opacity: h ? 0 : 1
                 };
                 d && (y.transform = `scaleX(${m})`);
-                let x = i("Toastify__progress-bar", d ? "Toastify__progress-bar--controlled" : "Toastify__progress-bar--animated", `Toastify__progress-bar-theme--${f}`, `Toastify__progress-bar--${s}`, {
+                let x = i("Toastify__progress-bar", d ? "Toastify__progress-bar--controlled" : "Toastify__progress-bar--animated", `Toastify__progress-bar-theme--${p}`, `Toastify__progress-bar--${s}`, {
                         "Toastify__progress-bar--rtl": g
                     }),
                     v = u(l) ? l({
                         rtl: g,
                         type: s,
                         defaultClassName: x
                     }) : i(x, l);
                 return a.createElement("div", {
                     role: "progressbar",
                     "aria-hidden": h ? "true" : "false",
                     "aria-label": "notification timer",
                     className: v,
                     style: y,
                     [d && m >= 1 ? "onTransitionEnd" : "onAnimationEnd"]: d && m < 1 ? null : () => {
-                        p && r()
+                        f && r()
                     }
                 })
             }
-            let E = e => {
+            let w = e => {
                     let {
                         isRunning: t,
                         preventExitTransition: n,
                         toastRef: r,
                         eventHandlers: s
                     } = function(e) {
                         let [t, n] = (0, a.useState)(!1), [r, s] = (0, a.useState)(!1), o = (0, a.useRef)(null), l = (0, a.useRef)({
@@ -335,20 +335,20 @@
                             boundingRect: null,
                             didMove: !1
                         }).current, i = (0, a.useRef)(e), {
                             autoClose: c,
                             pauseOnHover: d,
                             closeToast: m,
                             onClick: g,
-                            closeOnClick: p
+                            closeOnClick: f
                         } = e;
 
-                        function f(t) {
+                        function p(t) {
                             if (e.draggable) {
-                                "touchstart" === t.nativeEvent.type && t.nativeEvent.preventDefault(), l.didMove = !1, document.addEventListener("mousemove", T), document.addEventListener("mouseup", w), document.addEventListener("touchmove", T), document.addEventListener("touchend", w);
+                                "touchstart" === t.nativeEvent.type && t.nativeEvent.preventDefault(), l.didMove = !1, document.addEventListener("mousemove", T), document.addEventListener("mouseup", E), document.addEventListener("touchmove", T), document.addEventListener("touchend", E);
                                 let n = o.current;
                                 l.canCloseOnClick = !0, l.canDrag = !0, l.boundingRect = n.getBoundingClientRect(), n.style.transition = "", l.x = v(t.nativeEvent), l.y = b(t.nativeEvent), "x" === e.draggableDirection ? (l.start = l.x, l.removalDistance = n.offsetWidth * (e.draggablePercent / 100)) : (l.start = l.y, l.removalDistance = n.offsetHeight * (80 === e.draggablePercent ? 1.5 * e.draggablePercent : e.draggablePercent / 100))
                             }
                         }
 
                         function h(t) {
                             if (l.boundingRect) {
@@ -371,16 +371,16 @@
                         }
 
                         function T(n) {
                             let r = o.current;
                             l.canDrag && r && (l.didMove = !0, t && x(), l.x = v(n), l.y = b(n), l.delta = "x" === e.draggableDirection ? l.x - l.start : l.y - l.start, l.start !== l.x && (l.canCloseOnClick = !1), r.style.transform = `translate${e.draggableDirection}(${l.delta}px)`, r.style.opacity = "" + (1 - Math.abs(l.delta / l.removalDistance)))
                         }
 
-                        function w() {
-                            document.removeEventListener("mousemove", T), document.removeEventListener("mouseup", w), document.removeEventListener("touchmove", T), document.removeEventListener("touchend", w);
+                        function E() {
+                            document.removeEventListener("mousemove", T), document.removeEventListener("mouseup", E), document.removeEventListener("touchmove", T), document.removeEventListener("touchend", E);
                             let t = o.current;
                             if (l.canDrag && l.didMove && t) {
                                 if (l.canDrag = !1, Math.abs(l.delta) > l.removalDistance) return s(!0), void e.closeToast();
                                 t.style.transition = "transform 0.2s, opacity 0.2s", t.style.transform = `translate${e.draggableDirection}(0)`, t.style.opacity = "1"
                             }
                         }(0, a.useEffect)(() => {
                             i.current = e
@@ -388,106 +388,106 @@
                             once: !0
                         }), u(e.onOpen) && e.onOpen((0, a.isValidElement)(e.children) && e.children.props), () => {
                             let e = i.current;
                             u(e.onClose) && e.onClose((0, a.isValidElement)(e.children) && e.children.props)
                         }), []), (0, a.useEffect)(() => (e.pauseOnFocusLoss && (document.hasFocus() || x(), window.addEventListener("focus", y), window.addEventListener("blur", x)), () => {
                             e.pauseOnFocusLoss && (window.removeEventListener("focus", y), window.removeEventListener("blur", x))
                         }), [e.pauseOnFocusLoss]);
-                        let E = {
-                            onMouseDown: f,
-                            onTouchStart: f,
+                        let w = {
+                            onMouseDown: p,
+                            onTouchStart: p,
                             onMouseUp: h,
                             onTouchEnd: h
                         };
-                        return c && d && (E.onMouseEnter = x, E.onMouseLeave = y), p && (E.onClick = e => {
+                        return c && d && (w.onMouseEnter = x, w.onMouseLeave = y), f && (w.onClick = e => {
                             g && g(e), l.canCloseOnClick && m()
                         }), {
                             playToast: y,
                             pauseToast: x,
                             isRunning: t,
                             preventExitTransition: r,
                             toastRef: o,
-                            eventHandlers: E
+                            eventHandlers: w
                         }
                     }(e), {
                         closeButton: o,
                         children: l,
                         autoClose: c,
                         onClick: d,
                         type: m,
                         hideProgressBar: g,
-                        closeToast: p,
-                        transition: f,
+                        closeToast: f,
+                        transition: p,
                         position: h,
                         className: y,
                         style: x,
-                        bodyClassName: E,
+                        bodyClassName: w,
                         bodyStyle: N,
                         progressClassName: j,
                         progressStyle: k,
                         updateId: C,
                         role: _,
                         progress: I,
                         rtl: L,
                         toastId: O,
-                        deleteToast: M,
-                        isIn: P,
+                        deleteToast: P,
+                        isIn: M,
                         isLoading: R,
                         iconOut: D,
-                        closeOnClick: z,
+                        closeOnClick: A,
                         theme: B
-                    } = e, A = i("Toastify__toast", `Toastify__toast-theme--${B}`, `Toastify__toast--${m}`, {
+                    } = e, z = i("Toastify__toast", `Toastify__toast-theme--${B}`, `Toastify__toast--${m}`, {
                         "Toastify__toast--rtl": L
                     }, {
-                        "Toastify__toast--close-on-click": z
+                        "Toastify__toast--close-on-click": A
                     }), S = u(y) ? y({
                         rtl: L,
                         position: h,
                         type: m,
-                        defaultClassName: A
-                    }) : i(A, y), $ = !!I || !c, F = {
-                        closeToast: p,
+                        defaultClassName: z
+                    }) : i(z, y), $ = !!I || !c, H = {
+                        closeToast: f,
                         type: m,
                         theme: B
-                    }, H = null;
-                    return !1 === o || (H = u(o) ? o(F) : (0, a.isValidElement)(o) ? (0, a.cloneElement)(o, F) : T(F)), a.createElement(f, {
-                        isIn: P,
-                        done: M,
+                    }, F = null;
+                    return !1 === o || (F = u(o) ? o(H) : (0, a.isValidElement)(o) ? (0, a.cloneElement)(o, H) : T(H)), a.createElement(p, {
+                        isIn: M,
+                        done: P,
                         position: h,
                         preventExitTransition: n,
                         nodeRef: r
                     }, a.createElement("div", {
                         id: O,
                         onClick: d,
                         className: S,
                         ...s,
                         style: x,
                         ref: r
                     }, a.createElement("div", {
-                        ...P && {
+                        ...M && {
                             role: _
                         },
-                        className: u(E) ? E({
+                        className: u(w) ? w({
                             type: m
-                        }) : i("Toastify__toast-body", E),
+                        }) : i("Toastify__toast-body", w),
                         style: N
                     }, null != D && a.createElement("div", {
                         className: i("Toastify__toast-icon", {
                             "Toastify--animate-icon Toastify__zoom-enter": !R
                         })
-                    }, D), a.createElement("div", null, l)), H, a.createElement(w, {
+                    }, D), a.createElement("div", null, l)), F, a.createElement(E, {
                         ...C && !$ ? {
                             key: `pb-${C}`
                         } : {},
                         rtl: L,
                         theme: B,
                         delay: c,
                         isRunning: t,
-                        isIn: P,
-                        closeToast: p,
+                        isIn: M,
+                        closeToast: f,
                         hide: g,
                         type: m,
                         style: k,
                         className: j,
                         controlledProgress: $,
                         progress: I || 0
                     })))
@@ -495,16 +495,16 @@
                 N = function(e, t) {
                     return void 0 === t && (t = !1), {
                         enter: `Toastify--animate Toastify__${e}-enter`,
                         exit: `Toastify--animate Toastify__${e}-exit`,
                         appendPosition: t
                     }
                 },
-                j = p(N("bounce", !0)),
-                k = (p(N("slide", !0)), p(N("zoom")), p(N("flip")), (0, a.forwardRef)((e, t) => {
+                j = f(N("bounce", !0)),
+                k = (f(N("slide", !0)), f(N("zoom")), f(N("flip")), (0, a.forwardRef)((e, t) => {
                     let {
                         getToastToRender: n,
                         containerRef: r,
                         isToastActive: s
                     } = function(e) {
                         let [, t] = (0, a.useReducer)(e => e + 1, 0), [n, r] = (0, a.useState)([]), s = (0, a.useRef)(null), o = (0, a.useRef)(new Map).current, l = e => -1 !== n.indexOf(e), i = (0, a.useRef)({
                             toastKey: 1,
@@ -513,15 +513,15 @@
                             queue: [],
                             props: e,
                             containerId: null,
                             isToastActive: l,
                             getToast: e => o.get(e)
                         }).current;
 
-                        function p(e) {
+                        function f(e) {
                             let {
                                 containerId: t
                             } = e, {
                                 limit: n
                             } = i.props;
                             !n || t && i.containerId !== t || (i.count -= i.queue.length, i.queue = [])
                         }
@@ -538,50 +538,50 @@
                             } = i.queue.shift();
                             T(e, t, n)
                         }
 
                         function b(e, n) {
                             var r, l;
                             let {
-                                delay: p,
+                                delay: f,
                                 staleId: b,
-                                ...w
+                                ...E
                             } = n;
-                            if (!g(e) || !s.current || i.props.enableMultiContainer && w.containerId !== i.props.containerId || o.has(w.toastId) && null == w.updateId) return;
+                            if (!g(e) || !s.current || i.props.enableMultiContainer && E.containerId !== i.props.containerId || o.has(E.toastId) && null == E.updateId) return;
                             let {
-                                toastId: E,
+                                toastId: w,
                                 updateId: N,
                                 data: j
-                            } = w, {
+                            } = E, {
                                 props: k
-                            } = i, C = () => y(E), _ = null == N;
+                            } = i, C = () => y(w), _ = null == N;
                             _ && i.count++;
                             let I = {
                                 ...k,
                                 style: k.toastStyle,
                                 key: i.toastKey++,
-                                ...Object.fromEntries(Object.entries(w).filter(e => {
+                                ...Object.fromEntries(Object.entries(E).filter(e => {
                                     let [t, n] = e;
                                     return null != n
                                 })),
-                                toastId: E,
+                                toastId: w,
                                 updateId: N,
                                 data: j,
                                 closeToast: C,
                                 isIn: !1,
-                                className: m(w.className || k.toastClassName),
-                                bodyClassName: m(w.bodyClassName || k.bodyClassName),
-                                progressClassName: m(w.progressClassName || k.progressClassName),
-                                autoClose: !w.isLoading && (r = w.autoClose, l = k.autoClose, !1 === r || c(r) && r > 0 ? r : l),
+                                className: m(E.className || k.toastClassName),
+                                bodyClassName: m(E.bodyClassName || k.bodyClassName),
+                                progressClassName: m(E.progressClassName || k.progressClassName),
+                                autoClose: !E.isLoading && (r = E.autoClose, l = k.autoClose, !1 === r || c(r) && r > 0 ? r : l),
                                 deleteToast() {
-                                    let e = f(o.get(E), "removed");
-                                    o.delete(E), h.emit(4, e);
+                                    let e = p(o.get(w), "removed");
+                                    o.delete(w), h.emit(4, e);
                                     let n = i.queue.length;
-                                    if (i.count = null == E ? i.count - i.displayedToast : i.count - 1, i.count < 0 && (i.count = 0), n > 0) {
-                                        let e = null == E ? i.props.limit : 1;
+                                    if (i.count = null == w ? i.count - i.displayedToast : i.count - 1, i.count < 0 && (i.count = 0), n > 0) {
+                                        let e = null == w ? i.props.limit : 1;
                                         if (1 === n || 1 === e) i.displayedToast++, v();
                                         else {
                                             let t = e > n ? n : e;
                                             i.displayedToast = t;
                                             for (let e = 0; e < t; e++) v()
                                         }
                                     } else t()
@@ -594,45 +594,45 @@
                                     isLoading: r,
                                     icon: s
                                 } = e, o = null, l = {
                                     theme: t,
                                     type: n
                                 };
                                 return !1 === s || (u(s) ? o = s(l) : (0, a.isValidElement)(s) ? o = (0, a.cloneElement)(s, l) : d(s) || c(s) ? o = s : r ? o = x.spinner() : n in x && (o = x[n](l))), o
-                            }(I), u(w.onOpen) && (I.onOpen = w.onOpen), u(w.onClose) && (I.onClose = w.onClose), I.closeButton = k.closeButton, !1 === w.closeButton || g(w.closeButton) ? I.closeButton = w.closeButton : !0 === w.closeButton && (I.closeButton = !g(k.closeButton) || k.closeButton);
+                            }(I), u(E.onOpen) && (I.onOpen = E.onOpen), u(E.onClose) && (I.onClose = E.onClose), I.closeButton = k.closeButton, !1 === E.closeButton || g(E.closeButton) ? I.closeButton = E.closeButton : !0 === E.closeButton && (I.closeButton = !g(k.closeButton) || k.closeButton);
                             let L = e;
                             (0, a.isValidElement)(e) && !d(e.type) ? L = (0, a.cloneElement)(e, {
                                 closeToast: C,
                                 toastProps: I,
                                 data: j
                             }) : u(e) && (L = e({
                                 closeToast: C,
                                 toastProps: I,
                                 data: j
                             })), k.limit && k.limit > 0 && i.count > k.limit && _ ? i.queue.push({
                                 toastContent: L,
                                 toastProps: I,
                                 staleId: b
-                            }) : c(p) ? setTimeout(() => {
+                            }) : c(f) ? setTimeout(() => {
                                 T(L, I, b)
-                            }, p) : T(L, I, b)
+                            }, f) : T(L, I, b)
                         }
 
                         function T(e, t, n) {
                             let {
                                 toastId: a
                             } = t;
                             n && o.delete(n);
                             let s = {
                                 content: e,
                                 props: t
                             };
-                            o.set(a, s), r(e => [...e, a].filter(e => e !== n)), h.emit(4, f(s, null == s.props.updateId ? "added" : "updated"))
+                            o.set(a, s), r(e => [...e, a].filter(e => e !== n)), h.emit(4, p(s, null == s.props.updateId ? "added" : "updated"))
                         }
-                        return (0, a.useEffect)(() => (i.containerId = e.containerId, h.cancelEmit(3).on(0, b).on(1, e => s.current && y(e)).on(5, p).emit(2, i), () => {
+                        return (0, a.useEffect)(() => (i.containerId = e.containerId, h.cancelEmit(3).on(0, b).on(1, e => s.current && y(e)).on(5, f).emit(2, i), () => {
                             o.clear(), h.emit(3, i)
                         }), []), (0, a.useEffect)(() => {
                             i.props = e, i.isToastActive = l, i.displayedToast = n.length
                         }), {
                             getToastToRender: function(t) {
                                 let n = new Map,
                                     r = Array.from(o.values());
@@ -645,15 +645,15 @@
                             },
                             containerRef: s,
                             isToastActive: l
                         }
                     }(e), {
                         className: o,
                         style: l,
-                        rtl: p,
+                        rtl: f,
                         containerId: y
                     } = e;
                     return (0, a.useEffect)(() => {
                         t && (t.current = r.current)
                     }, []), a.createElement("div", {
                         ref: r,
                         className: "Toastify",
@@ -664,30 +664,30 @@
                         } : {
                             ...l,
                             pointerEvents: "none"
                         };
                         return a.createElement("div", {
                             className: function(e) {
                                 let t = i("Toastify__toast-container", `Toastify__toast-container--${e}`, {
-                                    "Toastify__toast-container--rtl": p
+                                    "Toastify__toast-container--rtl": f
                                 });
                                 return u(o) ? o({
                                     position: e,
-                                    rtl: p,
+                                    rtl: f,
                                     defaultClassName: t
                                 }) : i(t, m(o))
                             }(e),
                             style: n,
                             key: `container-${e}`
                         }, t.map((e, n) => {
                             let {
                                 content: r,
                                 props: o
                             } = e;
-                            return a.createElement(E, {
+                            return a.createElement(w, {
                                 ...o,
                                 isIn: s(o.toastId),
                                 style: {
                                     ...o.style,
                                     "--nth": n + 1,
                                     "--len": t.length
                                 },
@@ -717,28 +717,28 @@
             function O(e, t) {
                 return _.size > 0 ? h.emit(0, e, t) : I.push({
                     content: e,
                     options: t
                 }), t.toastId
             }
 
-            function M(e, t) {
+            function P(e, t) {
                 return {
                     ...t,
                     type: t && t.type || e,
                     toastId: t && (d(t.toastId) || c(t.toastId)) ? t.toastId : "" + L++
                 }
             }
 
-            function P(e) {
-                return (t, n) => O(t, M(e, n))
+            function M(e) {
+                return (t, n) => O(t, P(e, n))
             }
 
             function R(e, t) {
-                return O(e, M("default", t))
+                return O(e, P("default", t))
             }
 
             function D() {
                 return (0, r.jsx)("div", {
                     className: "border-b border-gray-200 dark:border-gray-700 mb-6",
                     children: (0, r.jsxs)("ul", {
                         className: "flex flex-wrap text-sm font-md text-center text-gray-500 dark:text-gray-400",
@@ -777,15 +777,15 @@
                                 }), "Manage Knowledge DB"]
                             })
                         })]
                     })
                 })
             }
 
-            function z() {
+            function A() {
                 return (0, r.jsx)(r.Fragment, {
                     children: (0, r.jsxs)("div", {
                         className: "py-4 px-4",
                         children: [(0, r.jsxs)("div", {
                             align: "center",
                             className: "mb-4",
                             children: [(0, r.jsx)("img", {
@@ -804,56 +804,49 @@
                     })
                 })
             }
 
             function B(e) {
                 let {
                     onSubmitMessage: t
-                } = e, [n, s] = (0, a.useState)("");
+                } = e, [n, s] = (0, a.useState)("CHAT"), [o, l] = (0, a.useState)("");
                 return (0, r.jsx)(r.Fragment, {
                     children: (0, r.jsxs)("form", {
                         className: "w-full px-2",
                         children: [(0, r.jsx)("label", {
                             htmlFor: "chat",
                             className: "sr-only",
                             children: "Your message"
                         }), (0, r.jsxs)("div", {
-                            className: "flex items-center bg-gray-300 px-2 pt-4 rounded-t-2xl overflow-hidden pb-8",
-                            children: [(0, r.jsxs)("button", {
-                                type: "button",
-                                className: "inline-flex justify-center p-2 text-gray-500 rounded-lg cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600",
-                                children: [(0, r.jsx)("svg", {
-                                    "aria-hidden": "true",
-                                    className: "w-8 h-8",
-                                    fill: "currentColor",
-                                    viewBox: "0 0 20 20",
-                                    xmlns: "http://www.w3.org/2000/svg",
-                                    children: (0, r.jsx)("path", {
-                                        fillRule: "evenodd",
-                                        d: "M4 3a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V5a2 2 0 00-2-2H4zm12 12H4l4-8 3 6 2-4 3 6z",
-                                        clipRule: "evenodd"
-                                    })
-                                }), (0, r.jsx)("span", {
-                                    className: "sr-only",
-                                    children: "Upload image"
+                            className: "flex items-center bg-gray-300 pt-4 rounded-t-2xl overflow-hidden pb-8",
+                            children: [(0, r.jsxs)("select", {
+                                class: "text-lg bg-gray-50 border border-gray-300 text-gray-900 py-3 rounded-l-2xl ml-4 focus:ring-gray-500 focus:border-gray-500 block w-[200px] px-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500",
+                                defaultValue: "CHAT",
+                                onChange: e => s(e.target.value),
+                                children: [(0, r.jsx)("option", {
+                                    value: "CHAT",
+                                    children: "Chat"
+                                }), (0, r.jsx)("option", {
+                                    value: "QA",
+                                    children: "Chat + Q&A"
                                 })]
                             }), (0, r.jsx)("textarea", {
-                                rows: "2",
-                                className: "block mx-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-2xl border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500",
+                                rows: "1",
+                                className: "block mr-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-r-2xl border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500",
                                 placeholder: "What are you thinking about?...",
-                                value: n,
-                                onChange: e => s(e.target.value),
+                                value: o,
+                                onChange: e => l(e.target.value),
                                 onKeyDown: e => {
-                                    "Enter" === e.key && !e.shiftKey && (e.preventDefault(), n && (t(n), s("")))
+                                    "Enter" === e.key && !e.shiftKey && (e.preventDefault(), o && (t(n, o), l("")))
                                 }
                             }), (0, r.jsxs)("button", {
                                 type: "submit",
                                 className: "inline-flex justify-center p-2 text-gray-600 rounded-full cursor-pointer hover:bg-blue-100 dark:text-gray-500 dark:hover:bg-gray-600",
                                 onClick: e => {
-                                    e.preventDefault(), n && (t(n), s(""))
+                                    e.preventDefault(), o && (t(n, o), l(""))
                                 },
                                 children: [(0, r.jsx)("svg", {
                                     "aria-hidden": "true",
                                     className: "w-8 h-8 rotate-90",
                                     fill: "currentColor",
                                     viewBox: "0 0 20 20",
                                     xmlns: "http://www.w3.org/2000/svg",
@@ -866,45 +859,46 @@
                                 })]
                             })]
                         })]
                     })
                 })
             }
 
-            function A() {
+            function z() {
                 let [e, t] = (0, a.useState)([]), [n, s] = (0, a.useState)(!1), o = (0, a.useRef)(null);
                 (0, a.useEffect)(() => {
                     let e = localStorage.getItem("messages");
                     if (!e) return;
                     let n = JSON.parse(e);
                     n && n.length > 0 && "Thinking..." === n[n.length - 1].answer && n.pop(), t(n)
                 }, []);
                 let l = e => {
                         localStorage.setItem("messages", JSON.stringify(e))
                     },
-                    i = r => {
+                    i = (r, a) => {
                         if (n) {
                             R.warning("I am thinking about previous question! Please wait...");
                             return
                         }
                         s(!0);
-                        let a = [...e, {
-                            query: r
+                        let i = [...e, {
+                            query: a
                         }, {
                             answer: "Thinking..."
                         }];
-                        t(a), l(a), setTimeout(() => {
+                        t(i), l(i), setTimeout(() => {
                             o.current.scrollTop = o.current.scrollHeight
                         }, 500), fetch("/api/ask", {
                             method: "POST",
                             headers: {
                                 "Content-Type": "application/json"
                             },
                             body: JSON.stringify({
-                                query: r
+                                mode: r,
+                                query: a
                             })
                         }).then(async e => {
                             let n = await e.json();
                             if (!e.ok) {
                                 let t = n && n.message || e.status;
                                 return Promise.reject(t)
                             }
@@ -916,25 +910,25 @@
                                     }
                                 }).then(async e => {
                                     let n = await e.json();
                                     if (!e.ok) {
                                         let t = n && n.message || e.status;
                                         return Promise.reject(t)
                                     }
-                                    "THINKING" == n.status && n.answer ? (a.pop(), t(a = [...a, {
+                                    "THINKING" == n.status && n.answer ? (i.pop(), t(i = [...i, {
                                         answer: n.answer,
                                         docs: null
-                                    }]), l(a), setTimeout(() => {
+                                    }]), l(i), setTimeout(() => {
                                         o.current.scrollIntoView({
                                             behavior: "smooth"
                                         })
-                                    }, 500)) : "READY" == n.status && (clearInterval(r), a.pop(), t(a = [...a, {
+                                    }, 500)) : "READY" == n.status && (clearInterval(r), i.pop(), t(i = [...i, {
                                         answer: n.answer,
                                         docs: n.docs
-                                    }]), l(a), setTimeout(() => {
+                                    }]), l(i), setTimeout(() => {
                                         o.current.scrollIntoView({
                                             behavior: "smooth"
                                         })
                                     }, 500), s(!1))
                                 })
                             }, 2e3)
                         }).catch(e => {
@@ -997,38 +991,38 @@
                                 }), (0, r.jsx)("div", {
                                     ref: o
                                 })]
                             })
                         }), (0, r.jsx)("div", {
                             className: "fixed left-[400px] right-0 bottom-0",
                             children: (0, r.jsx)(B, {
-                                onSubmitMessage: e => {
-                                    i(e)
+                                onSubmitMessage: (e, t) => {
+                                    i(e, t)
                                 }
                             })
                         })]
                     })
                 })
             }
 
             function S() {
                 return (0, r.jsx)(r.Fragment, {
                     children: (0, r.jsxs)("div", {
                         className: "relative w-full h-full",
                         children: [(0, r.jsx)("div", {
                             className: "bg-gray-200 shadow-md fixed w-[400px] h-full top-0",
-                            children: (0, r.jsx)(z, {})
+                            children: (0, r.jsx)(A, {})
                         }), (0, r.jsxs)("div", {
                             className: "h-full fixed left-[400px] right-0 top-0 bottom-0 overflow-auto",
-                            children: [(0, r.jsx)(A, {}), (0, r.jsx)(k, {})]
+                            children: [(0, r.jsx)(z, {}), (0, r.jsx)(k, {})]
                         })]
                     })
                 })
             }
-            R.loading = (e, t) => O(e, M("default", {
+            R.loading = (e, t) => O(e, P("default", {
                 isLoading: !0,
                 autoClose: !1,
                 closeOnClick: !1,
                 closeButton: !1,
                 draggable: !1,
                 ...t
             })), R.promise = function(e, t, n) {
@@ -1065,15 +1059,15 @@
                         }) : R(o.render, {
                             ...s,
                             ...o
                         }), a
                     },
                     c = u(e) ? e() : e;
                 return c.then(e => i("success", o, e)).catch(e => i("error", s, e)), c
-            }, R.success = P("success"), R.info = P("info"), R.error = P("error"), R.warning = P("warning"), R.warn = R.warning, R.dark = (e, t) => O(e, M("default", {
+            }, R.success = M("success"), R.info = M("info"), R.error = M("error"), R.warning = M("warning"), R.warn = R.warning, R.dark = (e, t) => O(e, P("default", {
                 theme: "dark",
                 ...t
             })), R.dismiss = e => {
                 _.size > 0 ? h.emit(1, e) : I = I.filter(t => null != e && t.options.toastId !== e)
             }, R.clearWaitingQueue = function(e) {
                 return void 0 === e && (e = {}), h.emit(5, e)
             }, R.isActive = e => {
```

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/css/a4a6346dff75e1d3.css` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/css/e5e3a6d239ad5709.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 /*
 ! tailwindcss v3.3.2 | MIT License | https://tailwindcss.com
-*/*,:after,:before{box-sizing:border-box;border:0 solid #e5e7eb}:after,:before{--tw-content:""}html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-feature-settings:normal;font-variation-settings:normal}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}.fixed{position:fixed}.relative{position:relative}.bottom-0{bottom:0}.left-\[400px\]{left:400px}.right-0{right:0}.top-0{top:0}.mx-2{margin-left:.5rem;margin-right:.5rem}.mx-4{margin-left:1rem;margin-right:1rem}.mx-auto{margin-left:auto;margin-right:auto}.mb-2{margin-bottom:.5rem}.mb-3{margin-bottom:.75rem}.mb-4{margin-bottom:1rem}.mb-6{margin-bottom:1.5rem}.mb-\[150px\]{margin-bottom:150px}.ml-2{margin-left:.5rem}.mr-2{margin-right:.5rem}.mr-3{margin-right:.75rem}.mt-2{margin-top:.5rem}.mt-3{margin-top:.75rem}.block{display:block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.hidden{display:none}.h-10{height:2.5rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-64{height:16rem}.h-8{height:2rem}.h-auto{height:auto}.h-full{height:100%}.w-10{width:2.5rem}.w-12{width:3rem}.w-4{width:1rem}.w-5{width:1.25rem}.w-8{width:2rem}.w-\[400px\]{width:400px}.w-full{width:100%}.max-w-\[600px\]{max-width:600px}.flex-grow{flex-grow:1}.rotate-90{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@keyframes spin{to{transform:rotate(1turn)}}.animate-spin{animation:spin 1s linear infinite}.cursor-pointer{cursor:pointer}.list-inside{list-style-position:inside}.list-disc{list-style-type:disc}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.justify-start{justify-content:flex-start}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.rounded-2xl{border-radius:1rem}.rounded-full{border-radius:9999px}.rounded-lg{border-radius:.5rem}.rounded-t-2xl{border-top-left-radius:1rem;border-top-right-radius:1rem}.rounded-t-lg{border-top-left-radius:.5rem;border-top-right-radius:.5rem}.border{border-width:1px}.border-2{border-width:2px}.border-b{border-bottom-width:1px}.border-b-2{border-bottom-width:2px}.border-dashed{border-style:dashed}.border-blue-600{--tw-border-opacity:1;border-color:rgb(37 99 235/var(--tw-border-opacity))}.border-gray-200{--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}.border-gray-300{--tw-border-opacity:1;border-color:rgb(209 213 219/var(--tw-border-opacity))}.border-transparent{border-color:transparent}.bg-gray-100{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.bg-gray-200{--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.bg-gray-300{--tw-bg-opacity:1;background-color:rgb(209 213 219/var(--tw-bg-opacity))}.bg-gray-50{--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity))}.bg-gray-800{--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}.p-2{padding:.5rem}.p-2\.5{padding:.625rem}.p-3{padding:.75rem}.p-4{padding:1rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.py-2{padding-top:.5rem;padding-bottom:.5rem}.py-2\.5{padding-top:.625rem;padding-bottom:.625rem}.py-4{padding-top:1rem;padding-bottom:1rem}.pb-6{padding-bottom:1.5rem}.pb-8{padding-bottom:2rem}.pt-20{padding-top:5rem}.pt-4{padding-top:1rem}.pt-5{padding-top:1.25rem}.pt-6{padding-top:1.5rem}.text-center{text-align:center}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-4xl{font-size:2.25rem;line-height:2.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.font-semibold{font-weight:600}.text-black{--tw-text-opacity:1;color:rgb(0 0 0/var(--tw-text-opacity))}.text-blue-500{--tw-text-opacity:1;color:rgb(59 130 246/var(--tw-text-opacity))}.text-blue-600{--tw-text-opacity:1;color:rgb(37 99 235/var(--tw-text-opacity))}.text-gray-200{--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.text-gray-500{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.text-gray-600{--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}.text-gray-700{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.text-gray-900{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.shadow-md{--tw-shadow:0 4px 6px -1px rgba(0,0,0,.1),0 2px 4px -2px rgba(0,0,0,.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color),0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.hover\:border-gray-300:hover{--tw-border-opacity:1;border-color:rgb(209 213 219/var(--tw-border-opacity))}.hover\:bg-blue-100:hover{--tw-bg-opacity:1;background-color:rgb(219 234 254/var(--tw-bg-opacity))}.hover\:bg-gray-100:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.hover\:bg-gray-900:hover{--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.hover\:text-gray-600:hover{--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}.hover\:text-gray-900:hover{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity))}.focus\:border-blue-500:focus{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.focus\:border-gray-500:focus{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.focus\:outline-none:focus{outline:2px solid transparent;outline-offset:2px}.focus\:ring-4:focus{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(4px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus\:ring-blue-500:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(59 130 246/var(--tw-ring-opacity))}.focus\:ring-gray-300:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(209 213 219/var(--tw-ring-opacity))}.focus\:ring-gray-500:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(107 114 128/var(--tw-ring-opacity))}.group:hover .group-hover\:text-blue-500{--tw-text-opacity:1;color:rgb(59 130 246/var(--tw-text-opacity))}.group:hover .group-hover\:text-gray-500{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}@media (prefers-color-scheme:dark){.dark\:border-blue-500{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.dark\:border-gray-600{--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}.dark\:border-gray-700{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.dark\:bg-gray-700{--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.dark\:bg-gray-800{--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}.dark\:text-blue-500{--tw-text-opacity:1;color:rgb(59 130 246/var(--tw-text-opacity))}.dark\:text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.dark\:text-gray-500{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.dark\:text-gray-600{--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}.dark\:text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.dark\:placeholder-gray-400::-moz-placeholder{--tw-placeholder-opacity:1;color:rgb(156 163 175/var(--tw-placeholder-opacity))}.dark\:placeholder-gray-400::placeholder{--tw-placeholder-opacity:1;color:rgb(156 163 175/var(--tw-placeholder-opacity))}.dark\:hover\:border-gray-500:hover{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.dark\:hover\:bg-gray-600:hover{--tw-bg-opacity:1;background-color:rgb(75 85 99/var(--tw-bg-opacity))}.dark\:hover\:bg-gray-700:hover{--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.dark\:hover\:text-gray-300:hover{--tw-text-opacity:1;color:rgb(209 213 219/var(--tw-text-opacity))}.dark\:hover\:text-white:hover{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.dark\:focus\:border-blue-500:focus{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.dark\:focus\:border-gray-500:focus{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.dark\:focus\:ring-blue-500:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(59 130 246/var(--tw-ring-opacity))}.dark\:focus\:ring-gray-500:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(107 114 128/var(--tw-ring-opacity))}.dark\:focus\:ring-gray-700:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(55 65 81/var(--tw-ring-opacity))}.group:hover .dark\:group-hover\:text-gray-300{--tw-text-opacity:1;color:rgb(209 213 219/var(--tw-text-opacity))}}@media (min-width:640px){.sm\:py-4{padding-top:1rem;padding-bottom:1rem}}@media (min-width:768px){.md\:px-5{padding-left:1.25rem;padding-right:1.25rem}}:root{--toastify-color-light:#fff;--toastify-color-dark:#121212;--toastify-color-info:#3498db;--toastify-color-success:#07bc0c;--toastify-color-warning:#f1c40f;--toastify-color-error:#e74c3c;--toastify-color-transparent:hsla(0,0%,100%,.7);--toastify-icon-color-info:var(--toastify-color-info);--toastify-icon-color-success:var(--toastify-color-success);--toastify-icon-color-warning:var(--toastify-color-warning);--toastify-icon-color-error:var(--toastify-color-error);--toastify-toast-width:320px;--toastify-toast-background:#fff;--toastify-toast-min-height:64px;--toastify-toast-max-height:800px;--toastify-font-family:sans-serif;--toastify-z-index:9999;--toastify-text-color-light:#757575;--toastify-text-color-dark:#fff;--toastify-text-color-info:#fff;--toastify-text-color-success:#fff;--toastify-text-color-warning:#fff;--toastify-text-color-error:#fff;--toastify-spinner-color:#616161;--toastify-spinner-color-empty-area:#e0e0e0;--toastify-color-progress-light:linear-gradient(90deg,#4cd964,#5ac8fa,#007aff,#34aadc,#5856d6,#ff2d55);--toastify-color-progress-dark:#bb86fc;--toastify-color-progress-info:var(--toastify-color-info);--toastify-color-progress-success:var(--toastify-color-success);--toastify-color-progress-warning:var(--toastify-color-warning);--toastify-color-progress-error:var(--toastify-color-error)}.Toastify__toast-container{z-index:var(--toastify-z-index);-webkit-transform:translateZ(var(--toastify-z-index));position:fixed;padding:4px;width:var(--toastify-toast-width);box-sizing:border-box;color:#fff}.Toastify__toast-container--top-left{top:1em;left:1em}.Toastify__toast-container--top-center{top:1em;left:50%;transform:translateX(-50%)}.Toastify__toast-container--top-right{top:1em;right:1em}.Toastify__toast-container--bottom-left{bottom:1em;left:1em}.Toastify__toast-container--bottom-center{bottom:1em;left:50%;transform:translateX(-50%)}.Toastify__toast-container--bottom-right{bottom:1em;right:1em}@media only screen and (max-width:480px){.Toastify__toast-container{width:100vw;padding:0;left:0;margin:0}.Toastify__toast-container--top-center,.Toastify__toast-container--top-left,.Toastify__toast-container--top-right{top:0;transform:translateX(0)}.Toastify__toast-container--bottom-center,.Toastify__toast-container--bottom-left,.Toastify__toast-container--bottom-right{bottom:0;transform:translateX(0)}.Toastify__toast-container--rtl{right:0;left:auto}}.Toastify__toast{position:relative;min-height:var(--toastify-toast-min-height);box-sizing:border-box;margin-bottom:1rem;padding:8px;border-radius:4px;box-shadow:0 1px 10px 0 rgba(0,0,0,.1),0 2px 15px 0 rgba(0,0,0,.05);display:flex;justify-content:space-between;max-height:var(--toastify-toast-max-height);overflow:hidden;font-family:var(--toastify-font-family);cursor:default;direction:ltr;z-index:0}.Toastify__toast--rtl{direction:rtl}.Toastify__toast--close-on-click{cursor:pointer}.Toastify__toast-body{margin:auto 0;flex:1 1 auto;padding:6px;display:flex;align-items:center}.Toastify__toast-body>div:last-child{word-break:break-word;flex:1}.Toastify__toast-icon{-webkit-margin-end:10px;margin-inline-end:10px;width:20px;flex-shrink:0;display:flex}.Toastify--animate{animation-fill-mode:both;animation-duration:.7s}.Toastify--animate-icon{animation-fill-mode:both;animation-duration:.3s}@media only screen and (max-width:480px){.Toastify__toast{margin-bottom:0;border-radius:0}}.Toastify__toast-theme--dark{background:var(--toastify-color-dark);color:var(--toastify-text-color-dark)}.Toastify__toast-theme--colored.Toastify__toast--default,.Toastify__toast-theme--light{background:var(--toastify-color-light);color:var(--toastify-text-color-light)}.Toastify__toast-theme--colored.Toastify__toast--info{color:var(--toastify-text-color-info);background:var(--toastify-color-info)}.Toastify__toast-theme--colored.Toastify__toast--success{color:var(--toastify-text-color-success);background:var(--toastify-color-success)}.Toastify__toast-theme--colored.Toastify__toast--warning{color:var(--toastify-text-color-warning);background:var(--toastify-color-warning)}.Toastify__toast-theme--colored.Toastify__toast--error{color:var(--toastify-text-color-error);background:var(--toastify-color-error)}.Toastify__progress-bar-theme--light{background:var(--toastify-color-progress-light)}.Toastify__progress-bar-theme--dark{background:var(--toastify-color-progress-dark)}.Toastify__progress-bar--info{background:var(--toastify-color-progress-info)}.Toastify__progress-bar--success{background:var(--toastify-color-progress-success)}.Toastify__progress-bar--warning{background:var(--toastify-color-progress-warning)}.Toastify__progress-bar--error{background:var(--toastify-color-progress-error)}.Toastify__progress-bar-theme--colored.Toastify__progress-bar--error,.Toastify__progress-bar-theme--colored.Toastify__progress-bar--info,.Toastify__progress-bar-theme--colored.Toastify__progress-bar--success,.Toastify__progress-bar-theme--colored.Toastify__progress-bar--warning{background:var(--toastify-color-transparent)}.Toastify__close-button{color:#fff;background:transparent;outline:none;border:none;padding:0;cursor:pointer;opacity:.7;transition:.3s ease;align-self:flex-start}.Toastify__close-button--light{color:#000;opacity:.3}.Toastify__close-button>svg{fill:currentColor;height:16px;width:14px}.Toastify__close-button:focus,.Toastify__close-button:hover{opacity:1}@keyframes Toastify__trackProgress{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.Toastify__progress-bar{position:absolute;bottom:0;left:0;width:100%;height:5px;z-index:var(--toastify-z-index);opacity:.7;transform-origin:left}.Toastify__progress-bar--animated{animation:Toastify__trackProgress linear 1 forwards}.Toastify__progress-bar--controlled{transition:transform .2s}.Toastify__progress-bar--rtl{right:0;left:auto;transform-origin:right}.Toastify__spinner{width:20px;height:20px;box-sizing:border-box;border:2px solid;border-radius:100%;border-color:var(--toastify-spinner-color-empty-area);border-right-color:var(--toastify-spinner-color);animation:Toastify__spin .65s linear infinite}@keyframes Toastify__bounceInRight{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(3000px,0,0)}60%{opacity:1;transform:translate3d(-25px,0,0)}75%{transform:translate3d(10px,0,0)}90%{transform:translate3d(-5px,0,0)}to{transform:none}}@keyframes Toastify__bounceOutRight{20%{opacity:1;transform:translate3d(-20px,0,0)}to{opacity:0;transform:translate3d(2000px,0,0)}}@keyframes Toastify__bounceInLeft{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(-3000px,0,0)}60%{opacity:1;transform:translate3d(25px,0,0)}75%{transform:translate3d(-10px,0,0)}90%{transform:translate3d(5px,0,0)}to{transform:none}}@keyframes Toastify__bounceOutLeft{20%{opacity:1;transform:translate3d(20px,0,0)}to{opacity:0;transform:translate3d(-2000px,0,0)}}@keyframes Toastify__bounceInUp{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(0,3000px,0)}60%{opacity:1;transform:translate3d(0,-20px,0)}75%{transform:translate3d(0,10px,0)}90%{transform:translate3d(0,-5px,0)}to{transform:translateZ(0)}}@keyframes Toastify__bounceOutUp{20%{transform:translate3d(0,-10px,0)}40%,45%{opacity:1;transform:translate3d(0,20px,0)}to{opacity:0;transform:translate3d(0,-2000px,0)}}@keyframes Toastify__bounceInDown{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(0,-3000px,0)}60%{opacity:1;transform:translate3d(0,25px,0)}75%{transform:translate3d(0,-10px,0)}90%{transform:translate3d(0,5px,0)}to{transform:none}}@keyframes Toastify__bounceOutDown{20%{transform:translate3d(0,10px,0)}40%,45%{opacity:1;transform:translate3d(0,-20px,0)}to{opacity:0;transform:translate3d(0,2000px,0)}}.Toastify__bounce-enter--bottom-left,.Toastify__bounce-enter--top-left{animation-name:Toastify__bounceInLeft}.Toastify__bounce-enter--bottom-right,.Toastify__bounce-enter--top-right{animation-name:Toastify__bounceInRight}.Toastify__bounce-enter--top-center{animation-name:Toastify__bounceInDown}.Toastify__bounce-enter--bottom-center{animation-name:Toastify__bounceInUp}.Toastify__bounce-exit--bottom-left,.Toastify__bounce-exit--top-left{animation-name:Toastify__bounceOutLeft}.Toastify__bounce-exit--bottom-right,.Toastify__bounce-exit--top-right{animation-name:Toastify__bounceOutRight}.Toastify__bounce-exit--top-center{animation-name:Toastify__bounceOutUp}.Toastify__bounce-exit--bottom-center{animation-name:Toastify__bounceOutDown}@keyframes Toastify__zoomIn{0%{opacity:0;transform:scale3d(.3,.3,.3)}50%{opacity:1}}@keyframes Toastify__zoomOut{0%{opacity:1}50%{opacity:0;transform:scale3d(.3,.3,.3)}to{opacity:0}}.Toastify__zoom-enter{animation-name:Toastify__zoomIn}.Toastify__zoom-exit{animation-name:Toastify__zoomOut}@keyframes Toastify__flipIn{0%{transform:perspective(400px) rotateX(90deg);animation-timing-function:ease-in;opacity:0}40%{transform:perspective(400px) rotateX(-20deg);animation-timing-function:ease-in}60%{transform:perspective(400px) rotateX(10deg);opacity:1}80%{transform:perspective(400px) rotateX(-5deg)}to{transform:perspective(400px)}}@keyframes Toastify__flipOut{0%{transform:perspective(400px)}30%{transform:perspective(400px) rotateX(-20deg);opacity:1}to{transform:perspective(400px) rotateX(90deg);opacity:0}}.Toastify__flip-enter{animation-name:Toastify__flipIn}.Toastify__flip-exit{animation-name:Toastify__flipOut}@keyframes Toastify__slideInRight{0%{transform:translate3d(110%,0,0);visibility:visible}to{transform:translateZ(0)}}@keyframes Toastify__slideInLeft{0%{transform:translate3d(-110%,0,0);visibility:visible}to{transform:translateZ(0)}}@keyframes Toastify__slideInUp{0%{transform:translate3d(0,110%,0);visibility:visible}to{transform:translateZ(0)}}@keyframes Toastify__slideInDown{0%{transform:translate3d(0,-110%,0);visibility:visible}to{transform:translateZ(0)}}@keyframes Toastify__slideOutRight{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(110%,0,0)}}@keyframes Toastify__slideOutLeft{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(-110%,0,0)}}@keyframes Toastify__slideOutDown{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(0,500px,0)}}@keyframes Toastify__slideOutUp{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(0,-500px,0)}}.Toastify__slide-enter--bottom-left,.Toastify__slide-enter--top-left{animation-name:Toastify__slideInLeft}.Toastify__slide-enter--bottom-right,.Toastify__slide-enter--top-right{animation-name:Toastify__slideInRight}.Toastify__slide-enter--top-center{animation-name:Toastify__slideInDown}.Toastify__slide-enter--bottom-center{animation-name:Toastify__slideInUp}.Toastify__slide-exit--bottom-left,.Toastify__slide-exit--top-left{animation-name:Toastify__slideOutLeft}.Toastify__slide-exit--bottom-right,.Toastify__slide-exit--top-right{animation-name:Toastify__slideOutRight}.Toastify__slide-exit--top-center{animation-name:Toastify__slideOutUp}.Toastify__slide-exit--bottom-center{animation-name:Toastify__slideOutDown}@keyframes Toastify__spin{0%{transform:rotate(0deg)}to{transform:rotate(1turn)}}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:200;font-display:swap;src:url(/_next/static/media/03a2ebda46411260-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:200;font-display:swap;src:url(/_next/static/media/4ab03c045edad786-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:200;font-display:swap;src:url(/_next/static/media/9d76af61a4574a5c-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:200;font-display:swap;src:url(/_next/static/media/c5fea7478aa47814-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:300;font-display:swap;src:url(/_next/static/media/560bcc4e09749527-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:300;font-display:swap;src:url(/_next/static/media/d77e36fa1e563bf0-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:300;font-display:swap;src:url(/_next/static/media/51fbb2aa5ef2b5cf-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:300;font-display:swap;src:url(/_next/static/media/7da2a3ff16027414-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:400;font-display:swap;src:url(/_next/static/media/2cffe11a47028c14-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:400;font-display:swap;src:url(/_next/static/media/4cf1eda6528c4545-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:400;font-display:swap;src:url(/_next/static/media/037c6ceced78c87a-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:400;font-display:swap;src:url(/_next/static/media/f1520da2fce335b3-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:500;font-display:swap;src:url(/_next/static/media/723f3c07bb1fbaab-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:500;font-display:swap;src:url(/_next/static/media/6cb9e821df97febd-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:500;font-display:swap;src:url(/_next/static/media/a8c682a8f4ee9d69-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:500;font-display:swap;src:url(/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:600;font-display:swap;src:url(/_next/static/media/f1144ac8e703eb32-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:600;font-display:swap;src:url(/_next/static/media/efe191cf7953ff64-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:600;font-display:swap;src:url(/_next/static/media/9b206b5a69aba6d3-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:600;font-display:swap;src:url(/_next/static/media/f6441c9c7c6cedc3-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:700;font-display:swap;src:url(/_next/static/media/84c22514fc6f1667-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:700;font-display:swap;src:url(/_next/static/media/f5ea4559b0835633-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:700;font-display:swap;src:url(/_next/static/media/8bbb723f6276338f-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:700;font-display:swap;src:url(/_next/static/media/996798fe8aee0dc3-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_Fallback_57cb44;src:local("Arial");ascent-override:96.17%;descent-override:24.04%;line-gap-override:0.00%;size-adjust:103.99%}.__className_57cb44{font-family:__Bai_Jamjuree_57cb44,__Bai_Jamjuree_Fallback_57cb44;font-style:normal}
+*/*,:after,:before{box-sizing:border-box;border:0 solid #e5e7eb}:after,:before{--tw-content:""}html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-feature-settings:normal;font-variation-settings:normal}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}.fixed{position:fixed}.relative{position:relative}.bottom-0{bottom:0}.left-\[400px\]{left:400px}.right-0{right:0}.top-0{top:0}.mx-2{margin-left:.5rem;margin-right:.5rem}.mx-4{margin-left:1rem;margin-right:1rem}.mx-auto{margin-left:auto;margin-right:auto}.mb-2{margin-bottom:.5rem}.mb-3{margin-bottom:.75rem}.mb-4{margin-bottom:1rem}.mb-6{margin-bottom:1.5rem}.mb-\[150px\]{margin-bottom:150px}.ml-2{margin-left:.5rem}.ml-4{margin-left:1rem}.mr-2{margin-right:.5rem}.mr-3{margin-right:.75rem}.mr-4{margin-right:1rem}.mt-2{margin-top:.5rem}.mt-3{margin-top:.75rem}.block{display:block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.hidden{display:none}.h-10{height:2.5rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-64{height:16rem}.h-8{height:2rem}.h-auto{height:auto}.h-full{height:100%}.w-10{width:2.5rem}.w-12{width:3rem}.w-4{width:1rem}.w-5{width:1.25rem}.w-8{width:2rem}.w-\[200px\]{width:200px}.w-\[400px\]{width:400px}.w-full{width:100%}.max-w-\[600px\]{max-width:600px}.flex-grow{flex-grow:1}.rotate-90{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@keyframes spin{to{transform:rotate(1turn)}}.animate-spin{animation:spin 1s linear infinite}.cursor-pointer{cursor:pointer}.list-inside{list-style-position:inside}.list-disc{list-style-type:disc}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.justify-start{justify-content:flex-start}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.rounded-full{border-radius:9999px}.rounded-lg{border-radius:.5rem}.rounded-l-2xl{border-top-left-radius:1rem;border-bottom-left-radius:1rem}.rounded-r-2xl{border-top-right-radius:1rem;border-bottom-right-radius:1rem}.rounded-t-2xl{border-top-left-radius:1rem;border-top-right-radius:1rem}.rounded-t-lg{border-top-left-radius:.5rem;border-top-right-radius:.5rem}.border{border-width:1px}.border-2{border-width:2px}.border-b{border-bottom-width:1px}.border-b-2{border-bottom-width:2px}.border-dashed{border-style:dashed}.border-blue-600{--tw-border-opacity:1;border-color:rgb(37 99 235/var(--tw-border-opacity))}.border-gray-200{--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}.border-gray-300{--tw-border-opacity:1;border-color:rgb(209 213 219/var(--tw-border-opacity))}.border-transparent{border-color:transparent}.bg-gray-100{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.bg-gray-200{--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.bg-gray-300{--tw-bg-opacity:1;background-color:rgb(209 213 219/var(--tw-bg-opacity))}.bg-gray-50{--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity))}.bg-gray-800{--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}.p-2{padding:.5rem}.p-2\.5{padding:.625rem}.p-3{padding:.75rem}.p-4{padding:1rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-2\.5{padding-left:.625rem;padding-right:.625rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.py-2{padding-top:.5rem;padding-bottom:.5rem}.py-2\.5{padding-top:.625rem;padding-bottom:.625rem}.py-3{padding-top:.75rem;padding-bottom:.75rem}.py-4{padding-top:1rem;padding-bottom:1rem}.pb-6{padding-bottom:1.5rem}.pb-8{padding-bottom:2rem}.pt-20{padding-top:5rem}.pt-4{padding-top:1rem}.pt-5{padding-top:1.25rem}.pt-6{padding-top:1.5rem}.text-center{text-align:center}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-4xl{font-size:2.25rem;line-height:2.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.font-semibold{font-weight:600}.text-black{--tw-text-opacity:1;color:rgb(0 0 0/var(--tw-text-opacity))}.text-blue-500{--tw-text-opacity:1;color:rgb(59 130 246/var(--tw-text-opacity))}.text-blue-600{--tw-text-opacity:1;color:rgb(37 99 235/var(--tw-text-opacity))}.text-gray-200{--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.text-gray-500{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.text-gray-600{--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}.text-gray-700{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.text-gray-900{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.shadow-md{--tw-shadow:0 4px 6px -1px rgba(0,0,0,.1),0 2px 4px -2px rgba(0,0,0,.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color),0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.hover\:border-gray-300:hover{--tw-border-opacity:1;border-color:rgb(209 213 219/var(--tw-border-opacity))}.hover\:bg-blue-100:hover{--tw-bg-opacity:1;background-color:rgb(219 234 254/var(--tw-bg-opacity))}.hover\:bg-gray-100:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.hover\:bg-gray-900:hover{--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.hover\:text-gray-600:hover{--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}.focus\:border-blue-500:focus{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.focus\:border-gray-500:focus{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.focus\:outline-none:focus{outline:2px solid transparent;outline-offset:2px}.focus\:ring-4:focus{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(4px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus\:ring-blue-500:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(59 130 246/var(--tw-ring-opacity))}.focus\:ring-gray-300:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(209 213 219/var(--tw-ring-opacity))}.focus\:ring-gray-500:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(107 114 128/var(--tw-ring-opacity))}.group:hover .group-hover\:text-blue-500{--tw-text-opacity:1;color:rgb(59 130 246/var(--tw-text-opacity))}.group:hover .group-hover\:text-gray-500{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}@media (prefers-color-scheme:dark){.dark\:border-blue-500{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.dark\:border-gray-600{--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}.dark\:border-gray-700{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.dark\:bg-gray-700{--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.dark\:bg-gray-800{--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}.dark\:text-blue-500{--tw-text-opacity:1;color:rgb(59 130 246/var(--tw-text-opacity))}.dark\:text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.dark\:text-gray-500{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.dark\:text-gray-600{--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}.dark\:text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.dark\:placeholder-gray-400::-moz-placeholder{--tw-placeholder-opacity:1;color:rgb(156 163 175/var(--tw-placeholder-opacity))}.dark\:placeholder-gray-400::placeholder{--tw-placeholder-opacity:1;color:rgb(156 163 175/var(--tw-placeholder-opacity))}.dark\:hover\:border-gray-500:hover{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.dark\:hover\:bg-gray-600:hover{--tw-bg-opacity:1;background-color:rgb(75 85 99/var(--tw-bg-opacity))}.dark\:hover\:bg-gray-700:hover{--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.dark\:hover\:text-gray-300:hover{--tw-text-opacity:1;color:rgb(209 213 219/var(--tw-text-opacity))}.dark\:focus\:border-blue-500:focus{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.dark\:focus\:border-gray-500:focus{--tw-border-opacity:1;border-color:rgb(107 114 128/var(--tw-border-opacity))}.dark\:focus\:ring-blue-500:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(59 130 246/var(--tw-ring-opacity))}.dark\:focus\:ring-gray-500:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(107 114 128/var(--tw-ring-opacity))}.dark\:focus\:ring-gray-700:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(55 65 81/var(--tw-ring-opacity))}.group:hover .dark\:group-hover\:text-gray-300{--tw-text-opacity:1;color:rgb(209 213 219/var(--tw-text-opacity))}}@media (min-width:640px){.sm\:py-4{padding-top:1rem;padding-bottom:1rem}}@media (min-width:768px){.md\:px-5{padding-left:1.25rem;padding-right:1.25rem}}:root{--toastify-color-light:#fff;--toastify-color-dark:#121212;--toastify-color-info:#3498db;--toastify-color-success:#07bc0c;--toastify-color-warning:#f1c40f;--toastify-color-error:#e74c3c;--toastify-color-transparent:hsla(0,0%,100%,.7);--toastify-icon-color-info:var(--toastify-color-info);--toastify-icon-color-success:var(--toastify-color-success);--toastify-icon-color-warning:var(--toastify-color-warning);--toastify-icon-color-error:var(--toastify-color-error);--toastify-toast-width:320px;--toastify-toast-background:#fff;--toastify-toast-min-height:64px;--toastify-toast-max-height:800px;--toastify-font-family:sans-serif;--toastify-z-index:9999;--toastify-text-color-light:#757575;--toastify-text-color-dark:#fff;--toastify-text-color-info:#fff;--toastify-text-color-success:#fff;--toastify-text-color-warning:#fff;--toastify-text-color-error:#fff;--toastify-spinner-color:#616161;--toastify-spinner-color-empty-area:#e0e0e0;--toastify-color-progress-light:linear-gradient(90deg,#4cd964,#5ac8fa,#007aff,#34aadc,#5856d6,#ff2d55);--toastify-color-progress-dark:#bb86fc;--toastify-color-progress-info:var(--toastify-color-info);--toastify-color-progress-success:var(--toastify-color-success);--toastify-color-progress-warning:var(--toastify-color-warning);--toastify-color-progress-error:var(--toastify-color-error)}.Toastify__toast-container{z-index:var(--toastify-z-index);-webkit-transform:translateZ(var(--toastify-z-index));position:fixed;padding:4px;width:var(--toastify-toast-width);box-sizing:border-box;color:#fff}.Toastify__toast-container--top-left{top:1em;left:1em}.Toastify__toast-container--top-center{top:1em;left:50%;transform:translateX(-50%)}.Toastify__toast-container--top-right{top:1em;right:1em}.Toastify__toast-container--bottom-left{bottom:1em;left:1em}.Toastify__toast-container--bottom-center{bottom:1em;left:50%;transform:translateX(-50%)}.Toastify__toast-container--bottom-right{bottom:1em;right:1em}@media only screen and (max-width:480px){.Toastify__toast-container{width:100vw;padding:0;left:0;margin:0}.Toastify__toast-container--top-center,.Toastify__toast-container--top-left,.Toastify__toast-container--top-right{top:0;transform:translateX(0)}.Toastify__toast-container--bottom-center,.Toastify__toast-container--bottom-left,.Toastify__toast-container--bottom-right{bottom:0;transform:translateX(0)}.Toastify__toast-container--rtl{right:0;left:auto}}.Toastify__toast{position:relative;min-height:var(--toastify-toast-min-height);box-sizing:border-box;margin-bottom:1rem;padding:8px;border-radius:4px;box-shadow:0 1px 10px 0 rgba(0,0,0,.1),0 2px 15px 0 rgba(0,0,0,.05);display:flex;justify-content:space-between;max-height:var(--toastify-toast-max-height);overflow:hidden;font-family:var(--toastify-font-family);cursor:default;direction:ltr;z-index:0}.Toastify__toast--rtl{direction:rtl}.Toastify__toast--close-on-click{cursor:pointer}.Toastify__toast-body{margin:auto 0;flex:1 1 auto;padding:6px;display:flex;align-items:center}.Toastify__toast-body>div:last-child{word-break:break-word;flex:1}.Toastify__toast-icon{-webkit-margin-end:10px;margin-inline-end:10px;width:20px;flex-shrink:0;display:flex}.Toastify--animate{animation-fill-mode:both;animation-duration:.7s}.Toastify--animate-icon{animation-fill-mode:both;animation-duration:.3s}@media only screen and (max-width:480px){.Toastify__toast{margin-bottom:0;border-radius:0}}.Toastify__toast-theme--dark{background:var(--toastify-color-dark);color:var(--toastify-text-color-dark)}.Toastify__toast-theme--colored.Toastify__toast--default,.Toastify__toast-theme--light{background:var(--toastify-color-light);color:var(--toastify-text-color-light)}.Toastify__toast-theme--colored.Toastify__toast--info{color:var(--toastify-text-color-info);background:var(--toastify-color-info)}.Toastify__toast-theme--colored.Toastify__toast--success{color:var(--toastify-text-color-success);background:var(--toastify-color-success)}.Toastify__toast-theme--colored.Toastify__toast--warning{color:var(--toastify-text-color-warning);background:var(--toastify-color-warning)}.Toastify__toast-theme--colored.Toastify__toast--error{color:var(--toastify-text-color-error);background:var(--toastify-color-error)}.Toastify__progress-bar-theme--light{background:var(--toastify-color-progress-light)}.Toastify__progress-bar-theme--dark{background:var(--toastify-color-progress-dark)}.Toastify__progress-bar--info{background:var(--toastify-color-progress-info)}.Toastify__progress-bar--success{background:var(--toastify-color-progress-success)}.Toastify__progress-bar--warning{background:var(--toastify-color-progress-warning)}.Toastify__progress-bar--error{background:var(--toastify-color-progress-error)}.Toastify__progress-bar-theme--colored.Toastify__progress-bar--error,.Toastify__progress-bar-theme--colored.Toastify__progress-bar--info,.Toastify__progress-bar-theme--colored.Toastify__progress-bar--success,.Toastify__progress-bar-theme--colored.Toastify__progress-bar--warning{background:var(--toastify-color-transparent)}.Toastify__close-button{color:#fff;background:transparent;outline:none;border:none;padding:0;cursor:pointer;opacity:.7;transition:.3s ease;align-self:flex-start}.Toastify__close-button--light{color:#000;opacity:.3}.Toastify__close-button>svg{fill:currentColor;height:16px;width:14px}.Toastify__close-button:focus,.Toastify__close-button:hover{opacity:1}@keyframes Toastify__trackProgress{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.Toastify__progress-bar{position:absolute;bottom:0;left:0;width:100%;height:5px;z-index:var(--toastify-z-index);opacity:.7;transform-origin:left}.Toastify__progress-bar--animated{animation:Toastify__trackProgress linear 1 forwards}.Toastify__progress-bar--controlled{transition:transform .2s}.Toastify__progress-bar--rtl{right:0;left:auto;transform-origin:right}.Toastify__spinner{width:20px;height:20px;box-sizing:border-box;border:2px solid;border-radius:100%;border-color:var(--toastify-spinner-color-empty-area);border-right-color:var(--toastify-spinner-color);animation:Toastify__spin .65s linear infinite}@keyframes Toastify__bounceInRight{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(3000px,0,0)}60%{opacity:1;transform:translate3d(-25px,0,0)}75%{transform:translate3d(10px,0,0)}90%{transform:translate3d(-5px,0,0)}to{transform:none}}@keyframes Toastify__bounceOutRight{20%{opacity:1;transform:translate3d(-20px,0,0)}to{opacity:0;transform:translate3d(2000px,0,0)}}@keyframes Toastify__bounceInLeft{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(-3000px,0,0)}60%{opacity:1;transform:translate3d(25px,0,0)}75%{transform:translate3d(-10px,0,0)}90%{transform:translate3d(5px,0,0)}to{transform:none}}@keyframes Toastify__bounceOutLeft{20%{opacity:1;transform:translate3d(20px,0,0)}to{opacity:0;transform:translate3d(-2000px,0,0)}}@keyframes Toastify__bounceInUp{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(0,3000px,0)}60%{opacity:1;transform:translate3d(0,-20px,0)}75%{transform:translate3d(0,10px,0)}90%{transform:translate3d(0,-5px,0)}to{transform:translateZ(0)}}@keyframes Toastify__bounceOutUp{20%{transform:translate3d(0,-10px,0)}40%,45%{opacity:1;transform:translate3d(0,20px,0)}to{opacity:0;transform:translate3d(0,-2000px,0)}}@keyframes Toastify__bounceInDown{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(0,-3000px,0)}60%{opacity:1;transform:translate3d(0,25px,0)}75%{transform:translate3d(0,-10px,0)}90%{transform:translate3d(0,5px,0)}to{transform:none}}@keyframes Toastify__bounceOutDown{20%{transform:translate3d(0,10px,0)}40%,45%{opacity:1;transform:translate3d(0,-20px,0)}to{opacity:0;transform:translate3d(0,2000px,0)}}.Toastify__bounce-enter--bottom-left,.Toastify__bounce-enter--top-left{animation-name:Toastify__bounceInLeft}.Toastify__bounce-enter--bottom-right,.Toastify__bounce-enter--top-right{animation-name:Toastify__bounceInRight}.Toastify__bounce-enter--top-center{animation-name:Toastify__bounceInDown}.Toastify__bounce-enter--bottom-center{animation-name:Toastify__bounceInUp}.Toastify__bounce-exit--bottom-left,.Toastify__bounce-exit--top-left{animation-name:Toastify__bounceOutLeft}.Toastify__bounce-exit--bottom-right,.Toastify__bounce-exit--top-right{animation-name:Toastify__bounceOutRight}.Toastify__bounce-exit--top-center{animation-name:Toastify__bounceOutUp}.Toastify__bounce-exit--bottom-center{animation-name:Toastify__bounceOutDown}@keyframes Toastify__zoomIn{0%{opacity:0;transform:scale3d(.3,.3,.3)}50%{opacity:1}}@keyframes Toastify__zoomOut{0%{opacity:1}50%{opacity:0;transform:scale3d(.3,.3,.3)}to{opacity:0}}.Toastify__zoom-enter{animation-name:Toastify__zoomIn}.Toastify__zoom-exit{animation-name:Toastify__zoomOut}@keyframes Toastify__flipIn{0%{transform:perspective(400px) rotateX(90deg);animation-timing-function:ease-in;opacity:0}40%{transform:perspective(400px) rotateX(-20deg);animation-timing-function:ease-in}60%{transform:perspective(400px) rotateX(10deg);opacity:1}80%{transform:perspective(400px) rotateX(-5deg)}to{transform:perspective(400px)}}@keyframes Toastify__flipOut{0%{transform:perspective(400px)}30%{transform:perspective(400px) rotateX(-20deg);opacity:1}to{transform:perspective(400px) rotateX(90deg);opacity:0}}.Toastify__flip-enter{animation-name:Toastify__flipIn}.Toastify__flip-exit{animation-name:Toastify__flipOut}@keyframes Toastify__slideInRight{0%{transform:translate3d(110%,0,0);visibility:visible}to{transform:translateZ(0)}}@keyframes Toastify__slideInLeft{0%{transform:translate3d(-110%,0,0);visibility:visible}to{transform:translateZ(0)}}@keyframes Toastify__slideInUp{0%{transform:translate3d(0,110%,0);visibility:visible}to{transform:translateZ(0)}}@keyframes Toastify__slideInDown{0%{transform:translate3d(0,-110%,0);visibility:visible}to{transform:translateZ(0)}}@keyframes Toastify__slideOutRight{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(110%,0,0)}}@keyframes Toastify__slideOutLeft{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(-110%,0,0)}}@keyframes Toastify__slideOutDown{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(0,500px,0)}}@keyframes Toastify__slideOutUp{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(0,-500px,0)}}.Toastify__slide-enter--bottom-left,.Toastify__slide-enter--top-left{animation-name:Toastify__slideInLeft}.Toastify__slide-enter--bottom-right,.Toastify__slide-enter--top-right{animation-name:Toastify__slideInRight}.Toastify__slide-enter--top-center{animation-name:Toastify__slideInDown}.Toastify__slide-enter--bottom-center{animation-name:Toastify__slideInUp}.Toastify__slide-exit--bottom-left,.Toastify__slide-exit--top-left{animation-name:Toastify__slideOutLeft}.Toastify__slide-exit--bottom-right,.Toastify__slide-exit--top-right{animation-name:Toastify__slideOutRight}.Toastify__slide-exit--top-center{animation-name:Toastify__slideOutUp}.Toastify__slide-exit--bottom-center{animation-name:Toastify__slideOutDown}@keyframes Toastify__spin{0%{transform:rotate(0deg)}to{transform:rotate(1turn)}}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:200;font-display:swap;src:url(/_next/static/media/03a2ebda46411260-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:200;font-display:swap;src:url(/_next/static/media/4ab03c045edad786-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:200;font-display:swap;src:url(/_next/static/media/9d76af61a4574a5c-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:200;font-display:swap;src:url(/_next/static/media/c5fea7478aa47814-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:300;font-display:swap;src:url(/_next/static/media/560bcc4e09749527-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:300;font-display:swap;src:url(/_next/static/media/d77e36fa1e563bf0-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:300;font-display:swap;src:url(/_next/static/media/51fbb2aa5ef2b5cf-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:300;font-display:swap;src:url(/_next/static/media/7da2a3ff16027414-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:400;font-display:swap;src:url(/_next/static/media/2cffe11a47028c14-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:400;font-display:swap;src:url(/_next/static/media/4cf1eda6528c4545-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:400;font-display:swap;src:url(/_next/static/media/037c6ceced78c87a-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:400;font-display:swap;src:url(/_next/static/media/f1520da2fce335b3-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:500;font-display:swap;src:url(/_next/static/media/723f3c07bb1fbaab-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:500;font-display:swap;src:url(/_next/static/media/6cb9e821df97febd-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:500;font-display:swap;src:url(/_next/static/media/a8c682a8f4ee9d69-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:500;font-display:swap;src:url(/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:600;font-display:swap;src:url(/_next/static/media/f1144ac8e703eb32-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:600;font-display:swap;src:url(/_next/static/media/efe191cf7953ff64-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:600;font-display:swap;src:url(/_next/static/media/9b206b5a69aba6d3-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:600;font-display:swap;src:url(/_next/static/media/f6441c9c7c6cedc3-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:700;font-display:swap;src:url(/_next/static/media/84c22514fc6f1667-s.woff2) format("woff2");unicode-range:U+0e01-0e5b,U+200c-200d,U+25cc}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:700;font-display:swap;src:url(/_next/static/media/f5ea4559b0835633-s.p.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:700;font-display:swap;src:url(/_next/static/media/8bbb723f6276338f-s.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__Bai_Jamjuree_57cb44;font-style:normal;font-weight:700;font-display:swap;src:url(/_next/static/media/996798fe8aee0dc3-s.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__Bai_Jamjuree_Fallback_57cb44;src:local("Arial");ascent-override:96.17%;descent-override:24.04%;line-gap-override:0.00%;size-adjust:103.99%}.__className_57cb44{font-family:__Bai_Jamjuree_57cb44,__Bai_Jamjuree_Fallback_57cb44;font-style:normal}
```

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2` & `pautobot-0.0.6/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/favicon.ico` & `pautobot-0.0.6/pautobot/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/index.html` & `pautobot-0.0.6/pautobot/frontend-dist/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/a4a6346dff75e1d3.css" as="style"/><link rel="stylesheet" href="/_next/static/css/a4a6346dff75e1d3.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/index-62fdb7c7217c2fea.js" defer=""></script><script src="/_next/static/Dl9fVCNsnbVyvPy7nTli-/_buildManifest.js" defer=""></script><script src="/_next/static/Dl9fVCNsnbVyvPy7nTli-/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div class="relative w-full h-full"><div class="bg-gray-200 shadow-md fixed w-[400px] h-full top-0"><div class="py-4 px-4"><div align="center" class="mb-4"><img alt="PAutoBot" class="w-12 h-auto mx-auto mb-2" src="/pautobot.png"/><h1 align="center" class="text-3xl font-semibold">🔥 PⒶutoBot 🔥</h1><p align="center">Your private task assistant with GPT</p></div><div class="border-b border-gray-200 dark:border-gray-700 mb-6"><ul class="flex flex-wrap text-sm font-md text-center text-gray-500 dark:text-gray-400"><li class="mr-2"><div class="inline-flex p-4 text-blue-600 border-b-2 border-blue-600 rounded-t-lg active dark:text-blue-500 dark:border-blue-500 group"><svg class="w-5 h-5 mr-2 text-blue-600 group-hover:text-blue-500 dark:text-blue-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path fill-rule="evenodd" d="M4.848 2.771A49.144 49.144 0 0112 2.25c2.43 0 4.817.178 7.152.52 1.978.292 3.348 2.024 3.348 3.97v6.02c0 1.946-1.37 3.678-3.348 3.97a48.901 48.901 0 01-3.476.383.39.39 0 00-.297.17l-2.755 4.133a.75.75 0 01-1.248 0l-2.755-4.133a.39.39 0 00-.297-.17 48.9 48.9 0 01-3.476-.384c-1.978-.29-3.348-2.024-3.348-3.97V6.741c0-1.946 1.37-3.68 3.348-3.97zM6.75 8.25a.75.75 0 01.75-.75h9a.75.75 0 010 1.5h-9a.75.75 0 01-.75-.75zm.75 2.25a.75.75 0 000 1.5H12a.75.75 0 000-1.5H7.5z" clip-rule="evenodd"></path></svg>Query</div></li><li class="mr-2"><div class="inline-flex p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300 group"><svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-400 group-hover:text-gray-500 dark:text-gray-500 dark:group-hover:text-gray-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M5 3a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2V5a2 2 0 00-2-2H5zM5 11a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 00-2-2H5zM11 5a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V5zM11 13a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"></path></svg>Manage Knowledge DB</div></li></ul></div><div class="flex"><select class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" disabled=""><option value="GPT4All" selected="">GPT4All</option><option value="LlamaCpp">LlamaCpp</option></select></div><div class="pt-6"><div class="flex items-center justify-center w-full"><label for="dropzone-file" class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 dark:hover:bg-bray-800 dark:bg-gray-700 hover:bg-gray-100 dark:border-gray-600 dark:hover:border-gray-500 dark:hover:bg-gray-600 p-3"><div class="flex flex-col items-center justify-center pt-5 pb-6"><svg aria-hidden="true" class="w-10 h-10 mb-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"></path></svg><p class="mb-2 text-sm text-gray-500 dark:text-gray-400"><span class="font-semibold">Click to upload</span> or drag and drop</p><p class="text-xs text-gray-500 dark:text-gray-400">CSV, DOCX, DOC, ENEX, EML, EPUB, HTML, MD, MSG, ODT, PDF, PPTX, PPT, TXT, images, zip, and more</p></div><input id="dropzone-file" type="file" class="hidden"/></label></div></div><div class="mt-3"><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Upload File</button><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Clear History</button></div></div></div><div class="h-full fixed left-[400px] right-0 top-0 bottom-0 overflow-auto"><div class="flex flex-col w-full"><div class="mx-2 md:px-5 sm:py-4 flex-grow mb-[150px]"><div class="text-black"><div class="text-center pt-20"><h1 class="text-4xl mb-4">Hello World!</h1><h3 class="text-2xl text-gray-500 max-w-[600px] mx-auto">We are in the mission of building an all-in-one task assistant with PrivateGPT!</h3></div><div></div></div></div><div class="fixed left-[400px] right-0 bottom-0"><form class="w-full px-2"><label for="chat" class="sr-only">Your message</label><div class="flex items-center bg-gray-300 px-2 pt-4 rounded-t-2xl overflow-hidden pb-8"><button type="button" class="inline-flex justify-center p-2 text-gray-500 rounded-lg cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4 3a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V5a2 2 0 00-2-2H4zm12 12H4l4-8 3 6 2-4 3 6z" clip-rule="evenodd"></path></svg><span class="sr-only">Upload image</span></button><textarea rows="2" class="block mx-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-2xl border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500" placeholder="What are you thinking about?..."></textarea><button type="submit" class="inline-flex justify-center p-2 text-gray-600 rounded-full cursor-pointer hover:bg-blue-100 dark:text-gray-500 dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8 rotate-90" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M10.894 2.553a1 1 0 00-1.788 0l-7 14a1 1 0 001.169 1.409l5-1.429A1 1 0 009 15.571V11a1 1 0 112 0v4.571a1 1 0 00.725.962l5 1.428a1 1 0 001.17-1.408l-7-14z"></path></svg><span class="sr-only">Send message</span></button></div></form></div></div><div class="Toastify"></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"Dl9fVCNsnbVyvPy7nTli-","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/e5e3a6d239ad5709.css" as="style"/><link rel="stylesheet" href="/_next/static/css/e5e3a6d239ad5709.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/index-07647c380718ba41.js" defer=""></script><script src="/_next/static/LGBTTPTxeYzvA3cKI-195/_buildManifest.js" defer=""></script><script src="/_next/static/LGBTTPTxeYzvA3cKI-195/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div class="relative w-full h-full"><div class="bg-gray-200 shadow-md fixed w-[400px] h-full top-0"><div class="py-4 px-4"><div align="center" class="mb-4"><img alt="PAutoBot" class="w-12 h-auto mx-auto mb-2" src="/pautobot.png"/><h1 align="center" class="text-3xl font-semibold">🔥 PⒶutoBot 🔥</h1><p align="center">Your private task assistant with GPT</p></div><div class="border-b border-gray-200 dark:border-gray-700 mb-6"><ul class="flex flex-wrap text-sm font-md text-center text-gray-500 dark:text-gray-400"><li class="mr-2"><div class="inline-flex p-4 text-blue-600 border-b-2 border-blue-600 rounded-t-lg active dark:text-blue-500 dark:border-blue-500 group"><svg class="w-5 h-5 mr-2 text-blue-600 group-hover:text-blue-500 dark:text-blue-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path fill-rule="evenodd" d="M4.848 2.771A49.144 49.144 0 0112 2.25c2.43 0 4.817.178 7.152.52 1.978.292 3.348 2.024 3.348 3.97v6.02c0 1.946-1.37 3.678-3.348 3.97a48.901 48.901 0 01-3.476.383.39.39 0 00-.297.17l-2.755 4.133a.75.75 0 01-1.248 0l-2.755-4.133a.39.39 0 00-.297-.17 48.9 48.9 0 01-3.476-.384c-1.978-.29-3.348-2.024-3.348-3.97V6.741c0-1.946 1.37-3.68 3.348-3.97zM6.75 8.25a.75.75 0 01.75-.75h9a.75.75 0 010 1.5h-9a.75.75 0 01-.75-.75zm.75 2.25a.75.75 0 000 1.5H12a.75.75 0 000-1.5H7.5z" clip-rule="evenodd"></path></svg>Query</div></li><li class="mr-2"><div class="inline-flex p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300 group"><svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-400 group-hover:text-gray-500 dark:text-gray-500 dark:group-hover:text-gray-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M5 3a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2V5a2 2 0 00-2-2H5zM5 11a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 00-2-2H5zM11 5a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V5zM11 13a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"></path></svg>Manage Knowledge DB</div></li></ul></div><div class="flex"><select class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" disabled=""><option value="GPT4All" selected="">GPT4All</option><option value="LlamaCpp">LlamaCpp</option></select></div><div class="pt-6"><div class="flex items-center justify-center w-full"><label for="dropzone-file" class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 dark:hover:bg-bray-800 dark:bg-gray-700 hover:bg-gray-100 dark:border-gray-600 dark:hover:border-gray-500 dark:hover:bg-gray-600 p-3"><div class="flex flex-col items-center justify-center pt-5 pb-6"><svg aria-hidden="true" class="w-10 h-10 mb-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"></path></svg><p class="mb-2 text-sm text-gray-500 dark:text-gray-400"><span class="font-semibold">Click to upload</span> or drag and drop</p><p class="text-xs text-gray-500 dark:text-gray-400">CSV, DOCX, DOC, ENEX, EML, EPUB, HTML, MD, MSG, ODT, PDF, PPTX, PPT, TXT, images, zip, and more</p></div><input id="dropzone-file" type="file" class="hidden"/></label></div></div><div class="mt-3"><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Upload File</button><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Clear History</button></div></div></div><div class="h-full fixed left-[400px] right-0 top-0 bottom-0 overflow-auto"><div class="flex flex-col w-full"><div class="mx-2 md:px-5 sm:py-4 flex-grow mb-[150px]"><div class="text-black"><div class="text-center pt-20"><h1 class="text-4xl mb-4">Hello World!</h1><h3 class="text-2xl text-gray-500 max-w-[600px] mx-auto">We are in the mission of building an all-in-one task assistant with PrivateGPT!</h3></div><div></div></div></div><div class="fixed left-[400px] right-0 bottom-0"><form class="w-full px-2"><label for="chat" class="sr-only">Your message</label><div class="flex items-center bg-gray-300 pt-4 rounded-t-2xl overflow-hidden pb-8"><select class="text-lg bg-gray-50 border border-gray-300 text-gray-900 py-3 rounded-l-2xl ml-4 focus:ring-gray-500 focus:border-gray-500 block w-[200px] px-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500"><option value="CHAT" selected="">Chat</option><option value="QA">Chat + Q&amp;A</option></select><textarea rows="1" class="block mr-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-r-2xl border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500" placeholder="What are you thinking about?..."></textarea><button type="submit" class="inline-flex justify-center p-2 text-gray-600 rounded-full cursor-pointer hover:bg-blue-100 dark:text-gray-500 dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8 rotate-90" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M10.894 2.553a1 1 0 00-1.788 0l-7 14a1 1 0 001.169 1.409l5-1.429A1 1 0 009 15.571V11a1 1 0 112 0v4.571a1 1 0 00.725.962l5 1.428a1 1 0 001.17-1.408l-7-14z"></path></svg><span class="sr-only">Send message</span></button></div></form></div></div><div class="Toastify"></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"LGBTTPTxeYzvA3cKI-195","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/loading.svg` & `pautobot-0.0.6/pautobot/frontend-dist/loading.svg`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/frontend-dist/pautobot.png` & `pautobot-0.0.6/pautobot/frontend-dist/pautobot.png`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/ingest.py` & `pautobot-0.0.6/pautobot/ingest.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot/utils.py` & `pautobot-0.0.6/pautobot/utils.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.5/pautobot.egg-info/PKG-INFO` & `pautobot-0.0.6/pautobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pautobot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Private AutoGPT Robot - Your private task assistant with GPT!
 Home-page: https://github.com/vietanhdev/pautobot
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: Apache License 2.0
 Keywords: Personal Assistant,Automation,GPT,LLM,PrivateGPT
 Classifier: Natural Language :: English
```

### Comparing `pautobot-0.0.5/pautobot.egg-info/SOURCES.txt` & `pautobot-0.0.6/pautobot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 pautobot.egg-info/requires.txt
 pautobot.egg-info/top_level.txt
 pautobot/frontend-dist/404.html
 pautobot/frontend-dist/favicon.ico
 pautobot/frontend-dist/index.html
 pautobot/frontend-dist/loading.svg
 pautobot/frontend-dist/pautobot.png
-pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/_buildManifest.js
-pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/_ssgManifest.js
+pautobot/frontend-dist/_next/static/LGBTTPTxeYzvA3cKI-195/_buildManifest.js
+pautobot/frontend-dist/_next/static/LGBTTPTxeYzvA3cKI-195/_ssgManifest.js
 pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
 pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
 pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
 pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
 pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
 pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
-pautobot/frontend-dist/_next/static/chunks/pages/index-62fdb7c7217c2fea.js
-pautobot/frontend-dist/_next/static/css/a4a6346dff75e1d3.css
+pautobot/frontend-dist/_next/static/chunks/pages/index-07647c380718ba41.js
+pautobot/frontend-dist/_next/static/css/e5e3a6d239ad5709.css
 pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2
 pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2
 pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2
 pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2
 pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2
 pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2
 pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2
```

### Comparing `pautobot-0.0.5/setup.py` & `pautobot-0.0.6/setup.py`

 * *Files identical despite different names*

