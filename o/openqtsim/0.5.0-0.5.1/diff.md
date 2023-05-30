# Comparing `tmp/OpenQTSim-0.5.0.tar.gz` & `tmp/openqtsim-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\OpenQTSim-0.5.0.tar", last modified: Wed Mar 11 23:08:49 2020, max compression
+gzip compressed data, was "openqtsim-0.5.1.tar", last modified: Tue May 30 13:07:28 2023, max compression
```

## Comparing `OpenQTSim-0.5.0.tar` & `openqtsim-0.5.1.tar`

### file list

```diff
@@ -1,69 +1,44 @@
-drwxrwxrwx   0        0        0        0 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/
--rw-rw-rw-   0        0        0      548 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     4084 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      539 2020-03-11 21:04:55.000000 OpenQTSim-0.5.0/HISTORY.rst
--rw-rw-rw-   0        0        0      273 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/OpenQTSim.egg-info/
--rw-rw-rw-   0        0        0     2778 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/OpenQTSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1906 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/OpenQTSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/OpenQTSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-02-02 12:47:04.000000 OpenQTSim-0.5.0/OpenQTSim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       82 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/OpenQTSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/OpenQTSim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2778 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1718 2020-03-11 22:18:59.000000 OpenQTSim-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/docs/
--rw-rw-rw-   0        0        0    37421 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/OpenQTSim.png
-drwxrwxrwx   0        0        0        0 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/docs/api/
--rw-rw-rw-   0        0        0       68 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/api/modules.rst
--rw-rw-rw-   0        0        0      986 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/api/queueing.rst
--rw-rw-rw-   0        0        0       43 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     5090 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/history.rst
--rw-rw-rw-   0        0        0      795 2020-02-03 14:21:33.000000 OpenQTSim-0.5.0/docs/index.rst
--rw-rw-rw-   0        0        0     1314 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/installation.rst
--rw-rw-rw-   0        0        0       74 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/docs/license.rst
--rw-rw-rw-   0        0        0     1355 2020-02-04 20:53:29.000000 OpenQTSim-0.5.0/docs/openqtsim.rst
-drwxrwxrwx   0        0        0        0 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/openqtsim/
--rw-rw-rw-   0        0        0      409 2020-03-11 21:06:05.000000 OpenQTSim-0.5.0/openqtsim/__init__.py
--rw-rw-rw-   0        0        0      737 2020-03-11 17:52:26.000000 OpenQTSim-0.5.0/openqtsim/arrival_process.py
--rw-rw-rw-   0        0        0     2415 2020-03-11 18:00:38.000000 OpenQTSim-0.5.0/openqtsim/customer.py
--rw-rw-rw-   0        0        0     4075 2020-03-11 19:44:05.000000 OpenQTSim-0.5.0/openqtsim/mm1.py
--rw-rw-rw-   0        0        0      973 2020-03-11 12:43:10.000000 OpenQTSim-0.5.0/openqtsim/mt_engine.py
--rw-rw-rw-   0        0        0    12912 2020-03-11 17:52:26.000000 OpenQTSim-0.5.0/openqtsim/queue.py
--rw-rw-rw-   0        0        0      746 2020-03-11 17:52:26.000000 OpenQTSim-0.5.0/openqtsim/service_process.py
--rw-rw-rw-   0        0        0     9566 2020-03-11 19:39:43.000000 OpenQTSim-0.5.0/openqtsim/simulation.py
--rw-rw-rw-   0        0        0     1230 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1945 2020-03-11 23:08:27.000000 OpenQTSim-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/tests/
--rw-rw-rw-   0        0        0    53248 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/.coverage
--rw-rw-rw-   0        0        0        0 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2020-02-02 12:46:31.000000 OpenQTSim-0.5.0/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2020-03-11 23:08:49.000000 OpenQTSim-0.5.0/tests/htmlcov/
--rw-rw-rw-   0        0        0     2299 2020-02-02 13:16:58.000000 OpenQTSim-0.5.0/tests/htmlcov/__init___py.html
--rw-rw-rw-   0        0        0     6014 2020-03-11 16:54:37.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim___init___py.html
--rw-rw-rw-   0        0        0     8723 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim_arrival_process_py.html
--rw-rw-rw-   0        0        0    23954 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim_customer_py.html
--rw-rw-rw-   0        0        0    72249 2020-02-02 13:17:22.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim_lookup_tables_py.html
--rw-rw-rw-   0        0        0    34822 2020-03-11 16:54:37.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim_mm1_py.html
--rw-rw-rw-   0        0        0    10822 2020-03-11 16:54:37.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim_mt_engine_py.html
--rw-rw-rw-   0        0        0   110777 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim_queue_py.html
--rw-rw-rw-   0        0        0     8781 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim_service_process_py.html
--rw-rw-rw-   0        0        0    80115 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim_simulation_py.html
--rw-rw-rw-   0        0        0    12391 2020-03-11 16:54:37.000000 OpenQTSim-0.5.0/tests/htmlcov/_checkouts_github_OpenQTSim_openqtsim_tables_py.html
--rw-rw-rw-   0        0        0     2299 2020-02-02 13:16:58.000000 OpenQTSim-0.5.0/tests/htmlcov/conftest_py.html
--rw-rw-rw-   0        0        0    18515 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/coverage_html.js
--rw-rw-rw-   0        0        0     6632 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/index.html
--rw-rw-rw-   0        0        0      731 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/jquery.ba-throttle-debounce.min.js
--rw-rw-rw-   0        0        0     3065 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/jquery.hotkeys.js
--rw-rw-rw-   0        0        0     1502 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/jquery.isonscreen.js
--rw-rw-rw-   0        0        0    95785 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/jquery.min.js
--rw-rw-rw-   0        0        0    12795 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/jquery.tablesorter.min.js
--rw-rw-rw-   0        0        0      112 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/keybd_closed.png
--rw-rw-rw-   0        0        0      112 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/keybd_open.png
--rw-rw-rw-   0        0        0     3437 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/status.json
--rw-rw-rw-   0        0        0     7025 2020-03-11 18:16:59.000000 OpenQTSim-0.5.0/tests/htmlcov/style.css
--rw-rw-rw-   0        0        0     8635 2020-03-11 16:54:37.000000 OpenQTSim-0.5.0/tests/htmlcov/test_basics_py.html
--rw-rw-rw-   0        0        0      589 2020-02-04 20:52:40.000000 OpenQTSim-0.5.0/tests/test_basics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:07:28.312132 openqtsim-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-30 13:07:10.000000 openqtsim-0.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-30 13:07:10.000000 openqtsim-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-30 13:07:10.000000 openqtsim-0.5.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-30 13:07:10.000000 openqtsim-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-30 13:07:10.000000 openqtsim-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-30 13:07:28.312132 openqtsim-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-30 13:07:10.000000 openqtsim-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:07:28.312132 openqtsim-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    37421 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/OpenQTSim.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:07:28.312132 openqtsim-0.5.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/api/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-30 13:07:10.000000 openqtsim-0.5.1/docs/openqtsim.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:07:28.312132 openqtsim-0.5.1/openqtsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-30 13:07:10.000000 openqtsim-0.5.1/openqtsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-30 13:07:10.000000 openqtsim-0.5.1/openqtsim/arrival_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-30 13:07:10.000000 openqtsim-0.5.1/openqtsim/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-30 13:07:10.000000 openqtsim-0.5.1/openqtsim/mm1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-30 13:07:10.000000 openqtsim-0.5.1/openqtsim/mt_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-05-30 13:07:10.000000 openqtsim-0.5.1/openqtsim/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-30 13:07:10.000000 openqtsim-0.5.1/openqtsim/service_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-05-30 13:07:10.000000 openqtsim-0.5.1/openqtsim/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:07:28.312132 openqtsim-0.5.1/openqtsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-30 13:07:28.000000 openqtsim-0.5.1/openqtsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 13:07:28.000000 openqtsim-0.5.1/openqtsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:07:28.000000 openqtsim-0.5.1/openqtsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:07:28.000000 openqtsim-0.5.1/openqtsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 13:07:28.000000 openqtsim-0.5.1/openqtsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 13:07:28.000000 openqtsim-0.5.1/openqtsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-30 13:07:28.316132 openqtsim-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-30 13:07:10.000000 openqtsim-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:07:28.312132 openqtsim-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:07:10.000000 openqtsim-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:07:10.000000 openqtsim-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-30 13:07:10.000000 openqtsim-0.5.1/tests/test_basics.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `OpenQTSim-0.5.0/CONTRIBUTING.rst` & `openqtsim-0.5.1/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-.. highlight:: shell
-
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every little bit
-helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/TUDelft-CITG/OpenQTSim/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
-wanted" is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "enhancement"
-and "help wanted" is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-OpenQTSim could always use more documentation, whether as part of the
-official OpenQTSim docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/TUDelft-CITG/OpenQTSim/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `OpenQTSim` for local development.
-
-1. Fork the `OpenQTSim` repository on GitHub.
-
-
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/OpenQTSim.git
-
-
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv openqtsim
-    $ cd openqtsim/
-    $ python setup.py develop
-
-
-4. Create a branch for local development::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-
-   Now you can make your changes locally.
-
-
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
-
-    $ flake8 openqtsim tests
-    $ python setup.py test or py.test
-    $ tox
-
-
-   To get flake8 and tox, just pip install them into your virtualenv.
-
-
-6. The style of OpenQTSim is according to Black. Format your code using 
-   Black with the following lines of code::
-
-    $ black openqtsim
-    $ black tests
-
-
-   You can install black using pip.
-
-
-7. Commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-
-
-8. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 3.4, 3.5 and 3.6, and for PyPy. Check
-   CircleCI and make sure that the tests pass for all supported Python versions.
-
-Tips
-----
-
-To run a subset of tests::
-
-$ py.test tests.test_openqtsim
-
-To make the documentation pages::
-
-$ make docs # for linux/osx
-
-For windows::
-
-$ del docs\openqtsim.rst
-$ del docs\modules.rst
-$ sphinx-apidoc -o docs/ openqtsim
-$ cd docs
-$ make html
-$ start explorer _build\html\index.html
-
-
-Deploying
----------
-
-A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in HISTORY.rst).
-Then run::
-
-$ bumpversion patch # possible: major / minor / patch
-$ git push
-$ git push --tags
-
-Travis will then deploy to PyPI if tests pass.
+.. highlight:: shell
+
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every little bit
+helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/TUDelft-CITG/OpenQTSim/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+wanted" is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "enhancement"
+and "help wanted" is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+OpenQTSim could always use more documentation, whether as part of the
+official OpenQTSim docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/TUDelft-CITG/OpenQTSim/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `OpenQTSim` for local development.
+
+1. Fork the `OpenQTSim` repository on GitHub.
+
+
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/OpenQTSim.git
+
+
+3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+
+    $ mkvirtualenv openqtsim
+    $ cd openqtsim/
+    $ python setup.py develop
+
+
+4. Create a branch for local development::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+
+   Now you can make your changes locally.
+
+
+5. When you're done making changes, check that your changes pass flake8 and the
+   tests, including testing other Python versions with tox::
+
+    $ flake8 openqtsim tests
+    $ python setup.py test or py.test
+    $ tox
+
+
+   To get flake8 and tox, just pip install them into your virtualenv.
+
+
+6. The style of OpenQTSim is according to Black. Format your code using 
+   Black with the following lines of code::
+
+    $ black openqtsim
+    $ black tests
+
+
+   You can install black using pip.
+
+
+7. Commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+    $ git push origin name-of-your-bugfix-or-feature
+
+
+8. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the list in README.rst.
+3. The pull request should work for Python 3.4, 3.5 and 3.6, and for PyPy. Check
+   CircleCI and make sure that the tests pass for all supported Python versions.
+
+Tips
+----
+
+To run a subset of tests::
+
+$ py.test tests.test_openqtsim
+
+To make the documentation pages::
+
+$ make docs # for linux/osx
+
+For windows::
+
+$ del docs\openqtsim.rst
+$ del docs\modules.rst
+$ sphinx-apidoc -o docs/ openqtsim
+$ cd docs
+$ make html
+$ start explorer _build\html\index.html
+
+
+Deploying
+---------
+
+A reminder for the maintainers on how to deploy.
+Make sure all your changes are committed (including an entry in HISTORY.rst).
+Then run::
+
+$ bumpversion patch # possible: major / minor / patch
+$ git push
+$ git push --tags
+
+Travis will then deploy to PyPI if tests pass.
```

### Comparing `OpenQTSim-0.5.0/OpenQTSim.egg-info/PKG-INFO` & `openqtsim-0.5.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-Metadata-Version: 2.1
-Name: OpenQTSim
-Version: 0.5.0
-Summary: OpenQTSim facilitates discrete event simulation of queues with a Kendall notation.
-Home-page: https://github.com/TUDelft-CITG/OpenQTSim
-Author: Mark van Koningsveld and Joris den Uijl
-Author-email: m.vankoningsveld@tudelft.nl
-License: mit
-Description: [ ![Documentation](https://img.shields.io/badge/sphinx-documentation-informational.svg)](https://openqtsim.readthedocs.io)
-        [ ![License: MIT](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/TUDelft-CITG/OpenQTSim/blob/master/LICENSE.txt)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3706929.svg)](https://doi.org/10.5281/zenodo.3706929)
-        
-        [![CircleCI](https://circleci.com/gh/TUDelft-CITG/OpenQTSim.svg?style=svg&circle-token=fe7b8b4d1c30d69ef17df79ebd9e81c3e4823b7e)](https://circleci.com/gh/TUDelft-CITG/OpenQTSim)
-        
-        
-        # OpenQTSim
-        
-        **Open** source **Q**ueueing **T**heory **Sim**ulation - Simulation package that facilitates discrete event simulation of queues with a Kendall notation.
-        
-        Documentation can be found [here](https://openqtsim.readthedocs.io).
-        
-        ## Installation
-        
-        To install OpenQTSim, run this command in your terminal:
-        
-        ``` bash
-        pip install openqtsim
-        ```
-        
-        This is the preferred method to install OpenQTSim, as it will always install the most recent stable release.
-        
-        If you don not have [pip](https://pip.pypa.io) installed, this [Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) can guide you through the process.
-        
-        You can read the [documentation](https://openqtsim.readthedocs.io/en/latest/installation.html) for other installation methods.
-        
-        ## Examples
-        
-        The benefit of OpenQTSim is the generic set-up. This set-up allows the simulation of a range of queues with a Kendall notation. A number of examples are presented in a seperate [Jupyter Notebook repository](https://github.com/TUDelft-CITG/OpenQTSim-Notebooks). Information on how to use the notebooks is presented in that repository as well.
-        
-Keywords: Queueing Theory
-Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
+Metadata-Version: 2.1
+Name: openqtsim
+Version: 0.5.1
+Summary: OpenQTSim facilitates discrete event simulation of queues with a Kendall notation.
+Home-page: https://github.com/TUDelft-CITG/OpenQTSim
+Author: Mark van Koningsveld and Joris den Uijl
+Author-email: m.vankoningsveld@tudelft.nl
+License: mit
+Keywords: Queueing Theory
+Platform: any
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+[ ![Documentation](https://img.shields.io/badge/sphinx-documentation-informational.svg)](https://openqtsim.readthedocs.io)
+[ ![License: MIT](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/TUDelft-CITG/OpenQTSim/blob/master/LICENSE.txt)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3706929.svg)](https://doi.org/10.5281/zenodo.3706929)
+
+[![CircleCI](https://circleci.com/gh/TUDelft-CITG/OpenQTSim.svg?style=svg&circle-token=fe7b8b4d1c30d69ef17df79ebd9e81c3e4823b7e)](https://circleci.com/gh/TUDelft-CITG/OpenQTSim)
+
+
+# OpenQTSim
+
+**Open** source **Q**ueueing **T**heory **Sim**ulation - Simulation package that facilitates discrete event simulation of queues with a Kendall notation.
+
+Documentation can be found [here](https://openqtsim.readthedocs.io).
+
+## Installation
+
+To install OpenQTSim, run this command in your terminal:
+
+``` bash
+pip install openqtsim
+```
+
+This is the preferred method to install OpenQTSim, as it will always install the most recent stable release.
+
+If you don not have [pip](https://pip.pypa.io) installed, this [Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) can guide you through the process.
+
+You can read the [documentation](https://openqtsim.readthedocs.io/en/latest/installation.html) for other installation methods.
+
+## Examples
+
+The benefit of OpenQTSim is the generic set-up. This set-up allows the simulation of a range of queues with a Kendall notation. A number of examples are presented in a seperate [Jupyter Notebook repository](https://github.com/TUDelft-CITG/OpenQTSim-Notebooks). Information on how to use the notebooks is presented in that repository as well.
```

### Comparing `OpenQTSim-0.5.0/PKG-INFO` & `openqtsim-0.5.1/openqtsim.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-Metadata-Version: 2.1
-Name: OpenQTSim
-Version: 0.5.0
-Summary: OpenQTSim facilitates discrete event simulation of queues with a Kendall notation.
-Home-page: https://github.com/TUDelft-CITG/OpenQTSim
-Author: Mark van Koningsveld and Joris den Uijl
-Author-email: m.vankoningsveld@tudelft.nl
-License: mit
-Description: [ ![Documentation](https://img.shields.io/badge/sphinx-documentation-informational.svg)](https://openqtsim.readthedocs.io)
-        [ ![License: MIT](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/TUDelft-CITG/OpenQTSim/blob/master/LICENSE.txt)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3706929.svg)](https://doi.org/10.5281/zenodo.3706929)
-        
-        [![CircleCI](https://circleci.com/gh/TUDelft-CITG/OpenQTSim.svg?style=svg&circle-token=fe7b8b4d1c30d69ef17df79ebd9e81c3e4823b7e)](https://circleci.com/gh/TUDelft-CITG/OpenQTSim)
-        
-        
-        # OpenQTSim
-        
-        **Open** source **Q**ueueing **T**heory **Sim**ulation - Simulation package that facilitates discrete event simulation of queues with a Kendall notation.
-        
-        Documentation can be found [here](https://openqtsim.readthedocs.io).
-        
-        ## Installation
-        
-        To install OpenQTSim, run this command in your terminal:
-        
-        ``` bash
-        pip install openqtsim
-        ```
-        
-        This is the preferred method to install OpenQTSim, as it will always install the most recent stable release.
-        
-        If you don not have [pip](https://pip.pypa.io) installed, this [Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) can guide you through the process.
-        
-        You can read the [documentation](https://openqtsim.readthedocs.io/en/latest/installation.html) for other installation methods.
-        
-        ## Examples
-        
-        The benefit of OpenQTSim is the generic set-up. This set-up allows the simulation of a range of queues with a Kendall notation. A number of examples are presented in a seperate [Jupyter Notebook repository](https://github.com/TUDelft-CITG/OpenQTSim-Notebooks). Information on how to use the notebooks is presented in that repository as well.
-        
-Keywords: Queueing Theory
-Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
+Metadata-Version: 2.1
+Name: openqtsim
+Version: 0.5.1
+Summary: OpenQTSim facilitates discrete event simulation of queues with a Kendall notation.
+Home-page: https://github.com/TUDelft-CITG/OpenQTSim
+Author: Mark van Koningsveld and Joris den Uijl
+Author-email: m.vankoningsveld@tudelft.nl
+License: mit
+Keywords: Queueing Theory
+Platform: any
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+[ ![Documentation](https://img.shields.io/badge/sphinx-documentation-informational.svg)](https://openqtsim.readthedocs.io)
+[ ![License: MIT](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/TUDelft-CITG/OpenQTSim/blob/master/LICENSE.txt)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3706929.svg)](https://doi.org/10.5281/zenodo.3706929)
+
+[![CircleCI](https://circleci.com/gh/TUDelft-CITG/OpenQTSim.svg?style=svg&circle-token=fe7b8b4d1c30d69ef17df79ebd9e81c3e4823b7e)](https://circleci.com/gh/TUDelft-CITG/OpenQTSim)
+
+
+# OpenQTSim
+
+**Open** source **Q**ueueing **T**heory **Sim**ulation - Simulation package that facilitates discrete event simulation of queues with a Kendall notation.
+
+Documentation can be found [here](https://openqtsim.readthedocs.io).
+
+## Installation
+
+To install OpenQTSim, run this command in your terminal:
+
+``` bash
+pip install openqtsim
+```
+
+This is the preferred method to install OpenQTSim, as it will always install the most recent stable release.
+
+If you don not have [pip](https://pip.pypa.io) installed, this [Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) can guide you through the process.
+
+You can read the [documentation](https://openqtsim.readthedocs.io/en/latest/installation.html) for other installation methods.
+
+## Examples
+
+The benefit of OpenQTSim is the generic set-up. This set-up allows the simulation of a range of queues with a Kendall notation. A number of examples are presented in a seperate [Jupyter Notebook repository](https://github.com/TUDelft-CITG/OpenQTSim-Notebooks). Information on how to use the notebooks is presented in that repository as well.
```

### Comparing `OpenQTSim-0.5.0/README.md` & `openqtsim-0.5.1/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-[ ![Documentation](https://img.shields.io/badge/sphinx-documentation-informational.svg)](https://openqtsim.readthedocs.io)
-[ ![License: MIT](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/TUDelft-CITG/OpenQTSim/blob/master/LICENSE.txt)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3706929.svg)](https://doi.org/10.5281/zenodo.3706929)
-
-[![CircleCI](https://circleci.com/gh/TUDelft-CITG/OpenQTSim.svg?style=svg&circle-token=fe7b8b4d1c30d69ef17df79ebd9e81c3e4823b7e)](https://circleci.com/gh/TUDelft-CITG/OpenQTSim)
-
-
-# OpenQTSim
-
-**Open** source **Q**ueueing **T**heory **Sim**ulation - Simulation package that facilitates discrete event simulation of queues with a Kendall notation.
-
-Documentation can be found [here](https://openqtsim.readthedocs.io).
-
-## Installation
-
-To install OpenQTSim, run this command in your terminal:
-
-``` bash
-pip install openqtsim
-```
-
-This is the preferred method to install OpenQTSim, as it will always install the most recent stable release.
-
-If you don not have [pip](https://pip.pypa.io) installed, this [Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) can guide you through the process.
-
-You can read the [documentation](https://openqtsim.readthedocs.io/en/latest/installation.html) for other installation methods.
-
-## Examples
-
-The benefit of OpenQTSim is the generic set-up. This set-up allows the simulation of a range of queues with a Kendall notation. A number of examples are presented in a seperate [Jupyter Notebook repository](https://github.com/TUDelft-CITG/OpenQTSim-Notebooks). Information on how to use the notebooks is presented in that repository as well.
+[ ![Documentation](https://img.shields.io/badge/sphinx-documentation-informational.svg)](https://openqtsim.readthedocs.io)
+[ ![License: MIT](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/TUDelft-CITG/OpenQTSim/blob/master/LICENSE.txt)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3706929.svg)](https://doi.org/10.5281/zenodo.3706929)
+
+[![CircleCI](https://circleci.com/gh/TUDelft-CITG/OpenQTSim.svg?style=svg&circle-token=fe7b8b4d1c30d69ef17df79ebd9e81c3e4823b7e)](https://circleci.com/gh/TUDelft-CITG/OpenQTSim)
+
+
+# OpenQTSim
+
+**Open** source **Q**ueueing **T**heory **Sim**ulation - Simulation package that facilitates discrete event simulation of queues with a Kendall notation.
+
+Documentation can be found [here](https://openqtsim.readthedocs.io).
+
+## Installation
+
+To install OpenQTSim, run this command in your terminal:
+
+``` bash
+pip install openqtsim
+```
+
+This is the preferred method to install OpenQTSim, as it will always install the most recent stable release.
+
+If you don not have [pip](https://pip.pypa.io) installed, this [Python installation guide](http://docs.python-guide.org/en/latest/starting/installation/) can guide you through the process.
+
+You can read the [documentation](https://openqtsim.readthedocs.io/en/latest/installation.html) for other installation methods.
+
+## Examples
+
+The benefit of OpenQTSim is the generic set-up. This set-up allows the simulation of a range of queues with a Kendall notation. A number of examples are presented in a seperate [Jupyter Notebook repository](https://github.com/TUDelft-CITG/OpenQTSim-Notebooks). Information on how to use the notebooks is presented in that repository as well.
```

### Comparing `OpenQTSim-0.5.0/docs/OpenQTSim.png` & `openqtsim-0.5.1/docs/OpenQTSim.png`

 * *Files identical despite different names*

### Comparing `OpenQTSim-0.5.0/docs/conf.py` & `openqtsim-0.5.1/docs/conf.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# openqtsim documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
-#
-import os
-import sys
-sys.path.insert(0, os.path.abspath('..'))
-
-import openqtsim
-
-# -- General configuration ---------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-#
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
-
-# The master toctree document.
-master_doc = 'index'
-
-# General information about the project.
-project = u'OpenQTSim'
-copyright = u"2020, TU Delft"
-author = u"Mark van Koningsveld, Joris den Uijl"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = openqtsim.__version__
-# The full version, including alpha/beta/rc tags.
-release = openqtsim.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = None
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-
-# -- Options for HTML output -------------------------------------------
-
-# Add a logo
-html_logo = "OpenQTSim.png"
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = "sphinx_rtd_theme"
-
-
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_theme_options = {}
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-
-# -- Options for HTMLHelp output ---------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'openqtsimdoc'
-
-
-# -- Options for LaTeX output ------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
-latex_documents = [
-    (master_doc, 'openqtsim.tex',
-     u'OpenQTSim Documentation',
-     u'Mark van Koningsveld, Joris den Uijl', 'manual'),
-]
-
-
-# -- Options for manual page output ------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'openqtsim',
-     u'OpenQTSim Documentation',
-     [author], 1)
-]
-
-
-# -- Options for Texinfo output ----------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (master_doc, 'openqtsim',
-     u'OpenQTSim Documentation',
-     author,
-     'openqtsim',
-     'One line description of project.',
-     'Miscellaneous'),
-]
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+#
+# openqtsim documentation build configuration file, created by
+# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# If extensions (or modules to document with autodoc) are in another
+# directory, add these directories to sys.path here. If the directory is
+# relative to the documentation root, use os.path.abspath to make it
+# absolute, like shown here.
+#
+import os
+import sys
+sys.path.insert(0, os.path.abspath('..'))
+
+import openqtsim
+
+# -- General configuration ---------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+#
+# source_suffix = ['.rst', '.md']
+source_suffix = '.rst'
+
+# The master toctree document.
+master_doc = 'index'
+
+# General information about the project.
+project = u'OpenQTSim'
+copyright = u"2020, TU Delft"
+author = u"Mark van Koningsveld, Joris den Uijl"
+
+# The version info for the project you're documenting, acts as replacement
+# for |version| and |release|, also used in various other places throughout
+# the built documents.
+#
+# The short X.Y version.
+version = openqtsim.__version__
+# The full version, including alpha/beta/rc tags.
+release = openqtsim.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = None
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+
+# -- Options for HTML output -------------------------------------------
+
+# Add a logo
+html_logo = "OpenQTSim.png"
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = "sphinx_rtd_theme"
+
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_theme_options = {}
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ['_static']
+
+
+# -- Options for HTMLHelp output ---------------------------------------
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = 'openqtsimdoc'
+
+
+# -- Options for LaTeX output ------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass
+# [howto, manual, or own class]).
+latex_documents = [
+    (master_doc, 'openqtsim.tex',
+     u'OpenQTSim Documentation',
+     u'Mark van Koningsveld, Joris den Uijl', 'manual'),
+]
+
+
+# -- Options for manual page output ------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [
+    (master_doc, 'openqtsim',
+     u'OpenQTSim Documentation',
+     [author], 1)
+]
+
+
+# -- Options for Texinfo output ----------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (master_doc, 'openqtsim',
+     u'OpenQTSim Documentation',
+     author,
+     'openqtsim',
+     'One line description of project.',
+     'Miscellaneous'),
+]
```

### Comparing `OpenQTSim-0.5.0/docs/openqtsim.rst` & `openqtsim-0.5.1/docs/openqtsim.rst`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-=========
-OpenQTSim
-=========
-
-This page lists all functions and classes available in the OpenQTSim modules. For examples on how to use these submodules please check out the Examples page, information on installing OpenQTSim can be found on the Installation page.
-
-Submodules
-----------
-
-The main components are the Model module and the Core module. All of their components are listed below. 
-
-openqtsim\.arrival_process module
-----------------------------------
-
-.. automodule:: openqtsim.arrival_process
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-openqtsim\.customer module
-----------------------------------
-
-.. automodule:: openqtsim.customer
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-openqtsim\.queue module
----------------------------------
-
-.. automodule:: openqtsim.queue
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-openqtsim\.service_process module
-----------------------------------
-
-.. automodule:: openqtsim.service_process
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-openqtsim\.simulation module
-----------------------------------
-
-.. automodule:: openqtsim.simulation
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-Module contents
----------------
-
-.. automodule:: openqtsim
-   :members:
-   :undoc-members:
-   :show-inheritance:
+=========
+OpenQTSim
+=========
+
+This page lists all functions and classes available in the OpenQTSim modules. For examples on how to use these submodules please check out the Examples page, information on installing OpenQTSim can be found on the Installation page.
+
+Submodules
+----------
+
+The main components are the Model module and the Core module. All of their components are listed below. 
+
+openqtsim\.arrival_process module
+----------------------------------
+
+.. automodule:: openqtsim.arrival_process
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+openqtsim\.customer module
+----------------------------------
+
+.. automodule:: openqtsim.customer
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+openqtsim\.queue module
+---------------------------------
+
+.. automodule:: openqtsim.queue
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+openqtsim\.service_process module
+----------------------------------
+
+.. automodule:: openqtsim.service_process
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+openqtsim\.simulation module
+----------------------------------
+
+.. automodule:: openqtsim.simulation
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+Module contents
+---------------
+
+.. automodule:: openqtsim
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `OpenQTSim-0.5.0/openqtsim/arrival_process.py` & `openqtsim-0.5.1/openqtsim/service_process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-
-
-class ArrivalProcess:
-    """
-    Arrival process class for use in the OpenQTSim package
-    """
-
-    def __init__(self, symbol='M', arr_rate=8):
-        """
-        symbol: symbol of the process (M, E_k, etc.)
-        arr_rate: arrivals per hour
-        """
-
-        self.symbol = symbol
-        self.arr_rate = arr_rate
-
-    def get_IAT(self, customer_nr=[]):
-        """
-        Return the inter arrival time based on the inter arrival time distribution or deterministic list
-        """
-
-        if self.symbol == "M" or self.symbol == "E2":
-            return self.arrival_distribution.rvs()
-
-        elif self.symbol == "D":
-            return self.arrival_distribution.loc[customer_nr, ['IAT']].item()
+
+
+class ServiceProcess:
+    """
+    Server process class for use in the OpenQTSim package
+    """
+
+    def __init__(self, symbol='M', srv_rate=9):
+        """
+        symbol: symbol of the process (M, E_k, etc.)
+        srv_rate: services per hour
+        """
+
+        self.symbol = symbol
+        self.srv_rate = srv_rate
+
+    def get_ST(self, server, customer_nr=[]):
+        """
+        Return the inter arrival time based on the inter arrival time distribution or deterministic list
+        """
+
+        if self.symbol == "M" or self.symbol[0] == "E":
+            return server.service_distribution.rvs()
+
+        elif self.symbol == "D":
+            return server.service_distribution.loc[customer_nr, ['ST']].item()
```

### Comparing `OpenQTSim-0.5.0/openqtsim/customer.py` & `openqtsim-0.5.1/openqtsim/customer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,75 @@
-
-
-class Customer:
-    """
-    Customer class for use in the OpenQTSim package
-    """
-
-    def __init__(self, Env, Sim):
-        """
-        Initialization
-        """
-
-        # self.arrival = arrival
-        self.Env = Env
-        self.Sim = Sim
-
-        Sim.customer_nr += 1
-        self.customer_nr = Sim.customer_nr
-
-    def move(self, IAT, AT):
-        """"
-        Method to move Customer through the system
-        """
-
-        # request access to server
-        self.Sim.c_s += 1
-        self.Sim.c_q += 1
-        t_req = AT
-        c_s_req = self.Sim.c_s
-        c_q_req = self.Sim.c_q
-
-        server = yield self.Env.servers.get()
-
-        self.Sim.c_q -= 1
-        t_yield = self.Env.now - self.Env.epoch
-        c_s_yield = self.Sim.c_s
-        c_q_yield = self.Sim.c_q
-
-        if t_req != t_yield:  # only log when someone is actually waiting to be served
-            self.Sim.log_system_state(t_req, c_s_req, c_q_req)
-            self.Sim.log_system_state(t_yield, c_s_yield, c_q_yield)
-        else:  # otherwise log the yield moment
-            self.Sim.log_system_state(t_yield, c_s_yield, c_q_yield)
-
-        # register if the server was idle
-        ITS = self.Env.now - self.Env.server_info[server.id]['last_active']
-
-        # register which server was used
-        s_id = server.id
-
-        # determine TSB
-        TSB = self.Env.now - self.Env.epoch
-
-        # get ST
-        # ST = server.service_distribution.rvs()
-        ST = self.Sim.queue.S.get_ST(server, customer_nr=self.customer_nr)
-        # server.service_distribution.rvs()
-
-        # move time ST forward
-        yield self.Env.timeout(ST)
-
-        # determine TSE
-        TSE = self.Env.now - self.Env.epoch
-
-        self.Sim.c_s -= 1
-        if self.Sim.c_q == 0:
-            self.Sim.log_system_state(TSE, self.Sim.c_s, self.Sim.c_q)
-        # Todo: when a customer leaves the system while somebody is still in the queue, you get a double logging
-        #  (check how this works for more than 1 server)
-
-        # update server_info when server was last active
-        self.Env.server_info.update({server.id: {'last_active': self.Env.now}})
-
-        # release server when done
-        yield self.Env.servers.put(server)
-
-        # add customer info to log
-        self.Sim.log_customer_state(self.customer_nr, IAT, AT, ST, TSB, TSE, ITS, s_id)
+
+
+class Customer:
+    """
+    Customer class for use in the OpenQTSim package
+    """
+
+    def __init__(self, Env, Sim):
+        """
+        Initialization
+        """
+
+        # self.arrival = arrival
+        self.Env = Env
+        self.Sim = Sim
+
+        Sim.customer_nr += 1
+        self.customer_nr = Sim.customer_nr
+
+    def move(self, IAT, AT):
+        """"
+        Method to move Customer through the system
+        """
+        # request access to server
+        self.Sim.c_s += 1
+        self.Sim.c_q += 1
+        t_req = AT
+        c_s_req = self.Sim.c_s
+        c_q_req = self.Sim.c_q
+
+        server = yield self.Env.servers.get()
+
+        self.Sim.c_q -= 1
+        t_yield = self.Env.now - self.Env.epoch
+        c_s_yield = self.Sim.c_s
+        c_q_yield = self.Sim.c_q
+
+        if t_req != t_yield:  # only log when someone is actually waiting to be served
+            self.Sim.log_system_state(t_req, c_s_req, c_q_req)
+            self.Sim.log_system_state(t_yield, c_s_yield, c_q_yield)
+        else:  # otherwise log the yield moment
+            self.Sim.log_system_state(t_yield, c_s_yield, c_q_yield)
+
+        # register if the server was idle
+        ITS = self.Env.now - self.Env.server_info[server.id]['last_active']
+
+        # register which server was used
+        s_id = server.id
+
+        # determine TSB
+        TSB = self.Env.now - self.Env.epoch
+
+        # get ST
+        ST = self.Sim.queue.S.get_ST(server, customer_nr=self.customer_nr)
+
+        # move time ST forward
+        yield self.Env.timeout(ST)
+
+        # determine TSE
+        TSE = self.Env.now - self.Env.epoch
+
+        self.Sim.c_s -= 1
+        if self.Sim.c_q == 0:
+            self.Sim.log_system_state(TSE, self.Sim.c_s, self.Sim.c_q)
+        # Todo: when a customer leaves the system while somebody is still in the queue, you get a double logging
+        #  (check how this works for more than 1 server)
+
+        # update server_info when server was last active
+        self.Env.server_info.update({server.id: {'last_active': self.Env.now}})
+
+        # release server when done
+        yield self.Env.servers.put(server)
+
+        # add customer info to log
+        self.Sim.log_customer_state(self.customer_nr, IAT, AT, ST, TSB, TSE, ITS, s_id)
```

### Comparing `OpenQTSim-0.5.0/openqtsim/mm1.py` & `openqtsim-0.5.1/openqtsim/mm1.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-from scipy import stats
-import numpy as np
-import pandas as pd
-
-
-class MM1:
-    """
-    A simple simulation method for MM1 queues
-    - MM1.get_IAT_and_ST: generates lists of IAT's and ST's drawn from exponential distributions
-    - MM1.calculate: values for AT, TSB, TSE, TCSS, TCWG and ITS are calculated per arrival
-    - MM1.get_stats: print basic statistics based on the simulation results
-    """
-    def __init__(self, lam, mu, nr_arr, seed=None):
-        """
-        Initialization the basic time unit is hours.
-        """
-
-        # todo: consider to remove seed
-        self.lam = lam  # arrivals per hour
-        self.mu = mu  # departures per hour
-        self.nr_arr = nr_arr  # nr of customers
-
-        np.random.seed(seed)
-
-    def get_IAT_and_ST(self):  # generate list of inter arrival times
-        """
-        Generate lists of IAT's and ST's drawn from exponential distributions.
-        """
-
-        rv_iat = stats.expon(scale=1 / self.lam)
-        rv_st = stats.expon(scale=1 / self.mu)
-
-        # generate list of inter arrival times
-        IAT = rv_iat.rvs(self.nr_arr)
-
-        # generate list of service times
-        ST = rv_st.rvs(self.nr_arr)
-
-        return IAT, ST
-
-    def calculate(self, IAT, ST):
-        """
-        Values for AT, TSB, TSE, TCSS, TCWG and ITS are calculated per arrival
-        """
-
-        df_cust = pd.DataFrame()
-        AT = []
-        TSB = []
-        TSE = []
-        TCSS = []
-        TCWQ = []
-        ITS = []
-
-        for i in range(len(IAT)):
-            # AT
-            if i == 0:
-                AT.append(IAT[i])  # time starts at 0 and the first arrival arrives at 0 + IAT
-            else:
-                AT.append(AT[i - 1] + IAT[i])  # next arrivals start at the previous arrival AT[i-1] + IAT
-
-            # TSB
-            if i == 0:
-                TSB.append(AT[i])  # first arrival the queue is empty so service begins as soon as customer arrives
-            else:
-                TSB.append(np.max([AT[i], TSE[i - 1]]))
-
-            # TSE
-            TSE.append(TSB[i] + ST[i])  # moment service begins plus service time
-
-            # TCSS
-            TCSS.append(TSE[i] - AT[i])  # moment of arrival until service ends
-
-            # TCWQ
-            TCWQ.append(TSB[i] - AT[i])  # moment of arrival until service begins
-
-            # ITS
-            if i == 0:
-                ITS.append(IAT[i])  # the server will start idle until the first arrival
-            else:
-                ITS.append(np.max([AT[i] - TSE[i - 1], 0]))
-
-        # Add lists to dataframe
-        df_cust["IAT"] = IAT
-        df_cust["ST"] = ST
-        df_cust["AT"] = AT
-        df_cust["TSB"] = TSB
-        df_cust["TSE"] = TSE
-        df_cust["TCSS"] = TCSS
-        df_cust["TCWQ"] = TCWQ
-        df_cust["ITS"] = ITS
-
-        return df_cust
-
-    def get_stats(self, df_cust):
-        """
-        Generate lists of IAT's and ST's drawn from exponential distributions.
-        """
-
-        value = np.mean(df_cust["TCWQ"]) / np.mean(df_cust["ST"])
-        print('Waiting time over service time: {:.4f}'.format(value))
-        print('')
-
-        value = (df_cust["TSE"].iloc[-1] - np.sum(df_cust["ITS"])) / df_cust["TSE"].iloc[-1]
-        print('Rho: system utilisation: {:.4f}'.format(value))
-        print('')
-
-        value = np.sum(df_cust["ITS"]) / df_cust["TSE"].iloc[-1]
-        print('P_0: probability nobody in the system: {:.4f}'.format(value))
-
-        value = np.mean(df_cust["TCSS"])
-        print('W_s: the long term average time spent in the system: {:.4f}'.format(value))
-
-        value = np.mean(df_cust["TCWQ"])
-        print('W_q: the long term average time spent in the queue: {:.4f}'.format(value))
-
-        value = df_cust["AT"].iloc[-1]/(len(df_cust["ST"])-1)
-        print('IAT: average inter arrival time: {:.4f}'.format(value))
-
-        value = np.sum(df_cust["ST"])/(len(df_cust["ST"]))
-        print('ST: average service time: {:.4f}'.format(value))
-        print('')
+from scipy import stats
+import numpy as np
+import pandas as pd
+
+
+class MM1:
+    """
+    A simple simulation method for MM1 queues
+    - MM1.get_IAT_and_ST: generates lists of IAT's and ST's drawn from exponential distributions
+    - MM1.calculate: values for AT, TSB, TSE, TCSS, TCWG and ITS are calculated per arrival
+    - MM1.get_stats: print basic statistics based on the simulation results
+    """
+    def __init__(self, lam, mu, nr_arr, seed=None):
+        """
+        Initialization the basic time unit is hours.
+        """
+
+        # todo: consider to remove seed
+        self.lam = lam  # arrivals per hour
+        self.mu = mu  # departures per hour
+        self.nr_arr = nr_arr  # nr of customers
+
+        np.random.seed(seed)
+
+    def get_IAT_and_ST(self):  # generate list of inter arrival times
+        """
+        Generate lists of IAT's and ST's drawn from exponential distributions.
+        """
+
+        rv_iat = stats.expon(scale=1 / self.lam)
+        rv_st = stats.expon(scale=1 / self.mu)
+
+        # generate list of inter arrival times
+        IAT = rv_iat.rvs(self.nr_arr)
+
+        # generate list of service times
+        ST = rv_st.rvs(self.nr_arr)
+
+        return IAT, ST
+
+    def calculate(self, IAT, ST):
+        """
+        Values for AT, TSB, TSE, TCSS, TCWG and ITS are calculated per arrival
+        """
+
+        df_cust = pd.DataFrame()
+        AT = []
+        TSB = []
+        TSE = []
+        TCSS = []
+        TCWQ = []
+        ITS = []
+
+        for i in range(len(IAT)):
+            # AT
+            if i == 0:
+                AT.append(IAT[i])  # time starts at 0 and the first arrival arrives at 0 + IAT
+            else:
+                AT.append(AT[i - 1] + IAT[i])  # next arrivals start at the previous arrival AT[i-1] + IAT
+
+            # TSB
+            if i == 0:
+                TSB.append(AT[i])  # first arrival the queue is empty so service begins as soon as customer arrives
+            else:
+                TSB.append(np.max([AT[i], TSE[i - 1]]))
+
+            # TSE
+            TSE.append(TSB[i] + ST[i])  # moment service begins plus service time
+
+            # TCSS
+            TCSS.append(TSE[i] - AT[i])  # moment of arrival until service ends
+
+            # TCWQ
+            TCWQ.append(TSB[i] - AT[i])  # moment of arrival until service begins
+
+            # ITS
+            if i == 0:
+                ITS.append(IAT[i])  # the server will start idle until the first arrival
+            else:
+                ITS.append(np.max([AT[i] - TSE[i - 1], 0]))
+
+        # Add lists to dataframe
+        df_cust["IAT"] = IAT
+        df_cust["ST"] = ST
+        df_cust["AT"] = AT
+        df_cust["TSB"] = TSB
+        df_cust["TSE"] = TSE
+        df_cust["TCSS"] = TCSS
+        df_cust["TCWQ"] = TCWQ
+        df_cust["ITS"] = ITS
+
+        return df_cust
+
+    def get_stats(self, df_cust):
+        """
+        Generate lists of IAT's and ST's drawn from exponential distributions.
+        """
+
+        value = np.mean(df_cust["TCWQ"]) / np.mean(df_cust["ST"])
+        print('Waiting time over service time: {:.4f}'.format(value))
+        print('')
+
+        value = (df_cust["TSE"].iloc[-1] - np.sum(df_cust["ITS"])) / df_cust["TSE"].iloc[-1]
+        print('Rho: system utilisation: {:.4f}'.format(value))
+        print('')
+
+        value = np.sum(df_cust["ITS"]) / df_cust["TSE"].iloc[-1]
+        print('P_0: probability nobody in the system: {:.4f}'.format(value))
+
+        value = np.mean(df_cust["TCSS"])
+        print('W_s: the long term average time spent in the system: {:.4f}'.format(value))
+
+        value = np.mean(df_cust["TCWQ"])
+        print('W_q: the long term average time spent in the queue: {:.4f}'.format(value))
+
+        value = df_cust["AT"].iloc[-1]/(len(df_cust["ST"])-1)
+        print('IAT: average inter arrival time: {:.4f}'.format(value))
+
+        value = np.sum(df_cust["ST"])/(len(df_cust["ST"]))
+        print('ST: average service time: {:.4f}'.format(value))
+        print('')
```

### Comparing `OpenQTSim-0.5.0/openqtsim/mt_engine.py` & `openqtsim-0.5.1/openqtsim/mt_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import openqtsim
-import pandas as pd
 import numpy as np
 from collections import namedtuple
 
-Task = namedtuple('Task','A, S, c, nr_arr, lam, mu')
+Task = namedtuple('Task', 'A, S, c, nr_arr, lam, mu')
+
 
 def worker(task:Task):
     # calculate the appropriate service rate per server
     srv_rate = task.mu/task.c
 
     # create Arrival and Service processes and specify the number of servers
     A = openqtsim.ArrivalProcess(task.A, arr_rate=task.lam)
@@ -24,8 +24,7 @@
     # retrieve the logs (df1: customer log, df2: system log)
     df1, df2 = sim.return_log()
 
     # use the customer log to determine the average waiting time as a factor of service time 
     factor = np.mean(df1["TCWQ"]) / np.mean(df1["ST"])
 
     return factor
-
```

### Comparing `OpenQTSim-0.5.0/openqtsim/queue.py` & `openqtsim-0.5.1/openqtsim/queue.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-import numpy as np
-import pandas as pd
-
-from openqtsim.customer import Customer
-from openqtsim.arrival_process import ArrivalProcess
-from openqtsim.service_process import ServiceProcess
-
-
-class Queue:
-    """
-    Queueing class based on Kendall's notation, in which:
-    - A is the arrival process
-    - S is the service time distribution
-    - c is the number of servers
-    - K is the number of places in the system
-    - N is the calling population
-    - D is the queue discipline
-    """
-
-    def __init__(self, A=ArrivalProcess(), S=ServiceProcess(), c=1, K=np.inf, N=np.inf, D="FIFO"):
-        """
-        The first six inputs are the typical Kendall inputs. Without inputs the queue object returns an M/M/1 object as
-        default
-        """
-
-        self.A = A
-        self.S = S
-        self.c = c
-        self.K = K
-        self.N = N
-        self.D = D
-
-    def populate(self, Env, Sim):
-        """
-        While the simulation time does not exceed the maximum duration, generate customers
-        according to the distribution of the arrival process to populate the queue
-        """
-
-        # Simulation stops either when max arrivals (max_arr) is reached or the tolerance limits are achieved
-        while Sim.customer_nr < Sim.max_arr:
-
-            # Draw IAT from distribution, move time forward and register arrival time (AT)
-            IAT = Sim.queue.A.get_IAT(Sim.customer_nr)
-
-            yield Env.timeout(IAT)
-
-            # determine AT
-            AT = Env.now - Env.epoch
-
-            # Create a customer
-            customer_new = Customer(Env, Sim)  # init: +1 for the next customer
-
-            # Make the customer go through the system
-            Env.process(customer_new.move(IAT, AT))
-
-    @property
-    def kendall_notation(self):
-        """
-        Return queue name according to the Kendall notation.
-        """
-
-        return "{}/{}/{}/{}/{}/{}".format(
-            self.A.symbol, self.S.symbol, str(self.c), str(self.K), str(self.N), self.D
-        )
-
-    def occupancy_to_waitingfactor(self, utilisation=.3, nr_of_servers_to_chk=4, poly_order=6):
-        """
-        Waiting time factor (E2/E2/n or M/E2/n) queueing theory using 6th order polynomial regression)
-        """
-
-        kendall = "{}/{}/{}".format(self.A.symbol, self.S.symbol, str(self.c))
-
-        if kendall[0:4] == 'M/M/':
-            # Create dataframe with data from Groenveld (2007) - Table I (M/M/n)
-            # See also PIANC 2014 Table 6.2
-            utilisations = np.array([.1, .2, .3, .4, .5, .6, .7, .8, .9])
-            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
-            data = np.array([
-                [0.1111, 0.0101, 0.0014, 0.0002, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
-                [0.2500, 0.0417, 0.0103, 0.0030, 0.0010, 0.0003, 0.0001, 0.0000, 0.0000, 0.0000],
-                [0.4286, 0.0989, 0.0333, 0.0132, 0.0058, 0.0027, 0.0013, 0.0006, 0.0003, 0.0002],
-                [0.6667, 0.1905, 0.0784, 0.0378, 0.0199, 0.0111, 0.0064, 0.0039, 0.0024, 0.0015],
-                [1.0000, 0.3333, 0.1579, 0.0870, 0.0521, 0.0330, 0.0218, 0.0148, 0.0102, 0.0072],
-                [1.5000, 0.5625, 0.2956, 0.1794, 0.1181, 0.0819, 0.0589, 0.0436, 0.0330, 0.0253],
-                [2.3333, 0.9608, 0.5470, 0.3572, 0.2519, 0.1867, 0.1432, 0.1128, 0.0906, 0.0739],
-                [4.0000, 1.7778, 1.0787, 0.7455, 0.5541, 0.4315, 0.3471, 0.2860, 0.2401, 0.2046],
-                [9.0000, 4.2632, 2.7235, 1.9693, 1.5250, 1.2335, 1.0285, 0.8769, 0.7606, 0.6687]])
-
-        elif kendall[0:6] == 'E2/E2/':
-            # Create dataframe with data from Groenveld (2007) - Table V (E2/E2/n)
-            # See also PIANC 2014 Table 6.2
-            utilisations = np.array([.1, .2, .3, .4, .5, .6, .7, .8, .9])
-            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
-            data = np.array([
-                [0.0166, 0.0006, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
-                [0.0604, 0.0065, 0.0011, 0.0002, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
-                [0.1310, 0.0235, 0.0062, 0.0019, 0.0007, 0.0002, 0.0001, 0.0000, 0.0000, 0.0000],
-                [0.2355, 0.0576, 0.0205, 0.0085, 0.0039, 0.0019, 0.0009, 0.0005, 0.0003, 0.0001],
-                [0.3904, 0.1181, 0.0512, 0.0532, 0.0142, 0.0082, 0.0050, 0.0031, 0.0020, 0.0013],
-                [0.6306, 0.2222, 0.1103, 0.0639, 0.0400, 0.0265, 0.0182, 0.0128, 0.0093, 0.0069],
-                [1.0391, 0.4125, 0.2275, 0.1441, 0.0988, 0.0712, 0.0532, 0.0407, 0.0319, 0.0258],
-                [1.8653, 0.8300, 0.4600, 0.3300, 0.2300, 0.1900, 0.1400, 0.1200, 0.0900, 0.0900],
-                [4.3590, 2.0000, 1.2000, 0.9200, 0.6500, 0.5700, 0.4400, 0.4000, 0.3200, 0.3000]
-            ])
-
-        elif kendall[0:5] == 'M/E2/n':
-            # Create dataframe with data from Groenveld (2007) - Table IV (M/E2/n)
-            # See also PIANC 2014 Table 6.1
-            utilisations = np.array([.1, .15, .2, .25, .3, .35, .4, .45, .5, .55, .6, .65, .7, .75, .8, .85, .9])
-            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14])
-            data = np.array([
-                [0.08, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.13, 0.02, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.19, 0.03, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.25, 0.05, 0.02, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.32, 0.08, 0.03, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.40, 0.11, 0.04, 0.02, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.50, 0.15, 0.06, 0.03, 0.02, 0.01, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.60, 0.20, 0.08, 0.05, 0.03, 0.02, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.75, 0.26, 0.12, 0.07, 0.04, 0.03, 0.02, 0.01, 0.01, 0.01, 0.00, 0.00, 0.00, 0.00],
-                [0.91, 0.33, 0.16, 0.10, 0.06, 0.04, 0.03, 0.02, 0.02, 0.01, 0.01, 0.01, 0.00, 0.00],
-                [1.13, 0.43, 0.23, 0.14, 0.09, 0.06, 0.05, 0.03, 0.03, 0.02, 0.02, 0.01, 0.01, 0.01],
-                [1.38, 0.55, 0.30, 0.19, 0.12, 0.09, 0.07, 0.05, 0.04, 0.03, 0.03, 0.02, 0.02, 0.02],
-                [1.75, 0.73, 0.42, 0.27, 0.19, 0.14, 0.11, 0.09, 0.07, 0.06, 0.05, 0.04, 0.03, 0.03],
-                [2.22, 0.96, 0.59, 0.39, 0.28, 0.21, 0.17, 0.14, 0.12, 0.10, 0.08, 0.07, 0.06, 0.05],
-                [3.00, 1.34, 0.82, 0.57, 0.42, 0.33, 0.27, 0.22, 0.18, 0.16, 0.13, 0.11, 0.10, 0.09],
-                [4.50, 2.00, 1.34, 0.90, 0.70, 0.54, 0.46, 0.39, 0.34, 0.30, 0.26, 0.23, 0.20, 0.18],
-                [6.75, 3.14, 2.01, 1.45, 1.12, 0.91, 0.76, 0.65, 0.56, 0.50, 0.45, 0.40, 0.36, 0.33]
-            ])
-
-        df = pd.DataFrame(data, index=utilisations, columns=nr_of_servers)
-
-        # Create a 6th order polynomial fit through the data (for nr_of_stations_chk)
-        target = df.loc[:, nr_of_servers_to_chk];
-        p_p = np.polyfit(target.index, target.values, poly_order)
-
-        waiting_factor = np.polyval(p_p, utilisation)
-        # todo: when the nr of servers > 10 the waiting factor should be set to inf (definitively more equipment needed)
-
-        # Return waiting factor
-        return waiting_factor
-
-    def waitingfactor_to_occupancy(self, factor=.3, nr_of_servers_to_chk=4, poly_order=6):
-        """
-        Waiting time factor (E2/E2/n or M/E2/n) queueing theory using 6th order polynomial regression)
-        """
-
-        kendall = "{}/{}/{}".format(self.A.symbol, self.S.symbol, str(self.c))
-
-        if kendall[0:4] == 'M/M/':
-            # Create dataframe with data from Groenveld (2007) - Table I (M/M/n)
-            # See also PIANC 2014 Table 6.2
-            utilisations = np.array([.1, .2, .3, .4, .5, .6, .7, .8, .9])
-            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
-            data = np.array([
-                [0.1111, 0.0101, 0.0014, 0.0002, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
-                [0.2500, 0.0417, 0.0103, 0.0030, 0.0010, 0.0003, 0.0001, 0.0000, 0.0000, 0.0000],
-                [0.4286, 0.0989, 0.0333, 0.0132, 0.0058, 0.0027, 0.0013, 0.0006, 0.0003, 0.0002],
-                [0.6667, 0.1905, 0.0784, 0.0378, 0.0199, 0.0111, 0.0064, 0.0039, 0.0024, 0.0015],
-                [1.0000, 0.3333, 0.1579, 0.0870, 0.0521, 0.0330, 0.0218, 0.0148, 0.0102, 0.0072],
-                [1.5000, 0.5625, 0.2956, 0.1794, 0.1181, 0.0819, 0.0589, 0.0436, 0.0330, 0.0253],
-                [2.3333, 0.9608, 0.5470, 0.3572, 0.2519, 0.1867, 0.1432, 0.1128, 0.0906, 0.0739],
-                [4.0000, 1.7778, 1.0787, 0.7455, 0.5541, 0.4315, 0.3471, 0.2860, 0.2401, 0.2046],
-                [9.0000, 4.2632, 2.7235, 1.9693, 1.5250, 1.2335, 1.0285, 0.8769, 0.7606, 0.6687]])
-
-        elif kendall[0:6] == 'E2/E2/':
-            # Create dataframe with data from Groenveld (2007) - Table V (E2/E2/n)
-            # See also PIANC 2014 Table 6.2
-            utilisations = np.array([.1, .2, .3, .4, .5, .6, .7, .8, .9])
-            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
-            data = np.array([
-                [0.0166, 0.0006, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
-                [0.0604, 0.0065, 0.0011, 0.0002, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
-                [0.1310, 0.0235, 0.0062, 0.0019, 0.0007, 0.0002, 0.0001, 0.0000, 0.0000, 0.0000],
-                [0.2355, 0.0576, 0.0205, 0.0085, 0.0039, 0.0019, 0.0009, 0.0005, 0.0003, 0.0001],
-                [0.3904, 0.1181, 0.0512, 0.0532, 0.0142, 0.0082, 0.0050, 0.0031, 0.0020, 0.0013],
-                [0.6306, 0.2222, 0.1103, 0.0639, 0.0400, 0.0265, 0.0182, 0.0128, 0.0093, 0.0069],
-                [1.0391, 0.4125, 0.2275, 0.1441, 0.0988, 0.0712, 0.0532, 0.0407, 0.0319, 0.0258],
-                [1.8653, 0.8300, 0.4600, 0.3300, 0.2300, 0.1900, 0.1400, 0.1200, 0.0900, 0.0900],
-                [4.3590, 2.0000, 1.2000, 0.9200, 0.6500, 0.5700, 0.4400, 0.4000, 0.3200, 0.3000]
-            ])
-
-        elif kendall[0:5] == 'M/E2/n':
-            # Create dataframe with data from Groenveld (2007) - Table IV (M/E2/n)
-            # See also PIANC 2014 Table 6.1
-            utilisations = np.array([.1, .15, .2, .25, .3, .35, .4, .45, .5, .55, .6, .65, .7, .75, .8, .85, .9])
-            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14])
-            data = np.array([
-                [0.08, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.13, 0.02, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.19, 0.03, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.25, 0.05, 0.02, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.32, 0.08, 0.03, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.40, 0.11, 0.04, 0.02, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.50, 0.15, 0.06, 0.03, 0.02, 0.01, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.60, 0.20, 0.08, 0.05, 0.03, 0.02, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
-                [0.75, 0.26, 0.12, 0.07, 0.04, 0.03, 0.02, 0.01, 0.01, 0.01, 0.00, 0.00, 0.00, 0.00],
-                [0.91, 0.33, 0.16, 0.10, 0.06, 0.04, 0.03, 0.02, 0.02, 0.01, 0.01, 0.01, 0.00, 0.00],
-                [1.13, 0.43, 0.23, 0.14, 0.09, 0.06, 0.05, 0.03, 0.03, 0.02, 0.02, 0.01, 0.01, 0.01],
-                [1.38, 0.55, 0.30, 0.19, 0.12, 0.09, 0.07, 0.05, 0.04, 0.03, 0.03, 0.02, 0.02, 0.02],
-                [1.75, 0.73, 0.42, 0.27, 0.19, 0.14, 0.11, 0.09, 0.07, 0.06, 0.05, 0.04, 0.03, 0.03],
-                [2.22, 0.96, 0.59, 0.39, 0.28, 0.21, 0.17, 0.14, 0.12, 0.10, 0.08, 0.07, 0.06, 0.05],
-                [3.00, 1.34, 0.82, 0.57, 0.42, 0.33, 0.27, 0.22, 0.18, 0.16, 0.13, 0.11, 0.10, 0.09],
-                [4.50, 2.00, 1.34, 0.90, 0.70, 0.54, 0.46, 0.39, 0.34, 0.30, 0.26, 0.23, 0.20, 0.18],
-                [6.75, 3.14, 2.01, 1.45, 1.12, 0.91, 0.76, 0.65, 0.56, 0.50, 0.45, 0.40, 0.36, 0.33]
-            ])
-
-        df = pd.DataFrame(data, index=utilisations, columns=nr_of_servers)
-
-        # Create a 6th order polynomial fit through the data (for nr_of_stations_chk)
-        target = df.loc[:, nr_of_servers_to_chk]
-        p_p = np.polyfit(target.values, target.index, poly_order)
-
-        occupancy = np.polyval(p_p, factor)
-
-        # Return occupancy
-        return occupancy
+import numpy as np
+import pandas as pd
+
+from openqtsim.customer import Customer
+from openqtsim.arrival_process import ArrivalProcess
+from openqtsim.service_process import ServiceProcess
+
+
+class Queue:
+    """
+    Queueing class based on Kendall's notation, in which:
+    - A is the arrival process
+    - S is the service time distribution
+    - c is the number of servers
+    - K is the number of places in the system
+    - N is the calling population
+    - D is the queue discipline
+    """
+
+    def __init__(self, A=ArrivalProcess(), S=ServiceProcess(), c=1, K=np.inf, N=np.inf, D="FIFO"):
+        """
+        The first six inputs are the typical Kendall inputs. Without inputs the queue object returns an M/M/1 object as
+        default
+        """
+
+        self.A = A
+        self.S = S
+        self.c = c
+        self.K = K
+        self.N = N
+        self.D = D
+
+    def populate(self, Env, Sim):
+        """
+        While the simulation time does not exceed the maximum duration, generate customers
+        according to the distribution of the arrival process to populate the queue
+        """
+
+        # Simulation stops either when max arrivals (max_arr) is reached or the tolerance limits are achieved
+        while Sim.customer_nr < Sim.max_arr:
+
+            # Draw IAT from distribution, move time forward and register arrival time (AT)
+            IAT = Sim.queue.A.get_IAT(Sim.customer_nr)
+
+            yield Env.timeout(IAT)
+
+            # determine AT
+            AT = Env.now - Env.epoch
+
+            # Create a customer
+            customer_new = Customer(Env, Sim)  # init: +1 for the next customer
+
+            # Make the customer go through the system
+            Env.process(customer_new.move(IAT, AT))
+
+    @property
+    def kendall_notation(self):
+        """
+        Return queue name according to the Kendall notation.
+        """
+
+        return "{}/{}/{}/{}/{}/{}".format(
+            self.A.symbol, self.S.symbol, str(self.c), str(self.K), str(self.N), self.D
+        )
+
+    def occupancy_to_waitingfactor(self, utilisation=.3, nr_of_servers_to_chk=4, poly_order=6):
+        """
+        Waiting time factor (E2/E2/n or M/E2/n) queueing theory using 6th order polynomial regression)
+        """
+
+        kendall = "{}/{}/{}".format(self.A.symbol, self.S.symbol, str(self.c))
+
+        if kendall[0:4] == 'M/M/':
+            # Create dataframe with data from Groenveld (2007) - Table I (M/M/n)
+            # See also PIANC 2014 Table 6.2
+            utilisations = np.array([.1, .2, .3, .4, .5, .6, .7, .8, .9])
+            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
+            data = np.array([
+                [0.1111, 0.0101, 0.0014, 0.0002, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
+                [0.2500, 0.0417, 0.0103, 0.0030, 0.0010, 0.0003, 0.0001, 0.0000, 0.0000, 0.0000],
+                [0.4286, 0.0989, 0.0333, 0.0132, 0.0058, 0.0027, 0.0013, 0.0006, 0.0003, 0.0002],
+                [0.6667, 0.1905, 0.0784, 0.0378, 0.0199, 0.0111, 0.0064, 0.0039, 0.0024, 0.0015],
+                [1.0000, 0.3333, 0.1579, 0.0870, 0.0521, 0.0330, 0.0218, 0.0148, 0.0102, 0.0072],
+                [1.5000, 0.5625, 0.2956, 0.1794, 0.1181, 0.0819, 0.0589, 0.0436, 0.0330, 0.0253],
+                [2.3333, 0.9608, 0.5470, 0.3572, 0.2519, 0.1867, 0.1432, 0.1128, 0.0906, 0.0739],
+                [4.0000, 1.7778, 1.0787, 0.7455, 0.5541, 0.4315, 0.3471, 0.2860, 0.2401, 0.2046],
+                [9.0000, 4.2632, 2.7235, 1.9693, 1.5250, 1.2335, 1.0285, 0.8769, 0.7606, 0.6687]])
+
+        elif kendall[0:6] == 'E2/E2/':
+            # Create dataframe with data from Groenveld (2007) - Table V (E2/E2/n)
+            # See also PIANC 2014 Table 6.2
+            utilisations = np.array([.1, .2, .3, .4, .5, .6, .7, .8, .9])
+            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
+            data = np.array([
+                [0.0166, 0.0006, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
+                [0.0604, 0.0065, 0.0011, 0.0002, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
+                [0.1310, 0.0235, 0.0062, 0.0019, 0.0007, 0.0002, 0.0001, 0.0000, 0.0000, 0.0000],
+                [0.2355, 0.0576, 0.0205, 0.0085, 0.0039, 0.0019, 0.0009, 0.0005, 0.0003, 0.0001],
+                [0.3904, 0.1181, 0.0512, 0.0532, 0.0142, 0.0082, 0.0050, 0.0031, 0.0020, 0.0013],
+                [0.6306, 0.2222, 0.1103, 0.0639, 0.0400, 0.0265, 0.0182, 0.0128, 0.0093, 0.0069],
+                [1.0391, 0.4125, 0.2275, 0.1441, 0.0988, 0.0712, 0.0532, 0.0407, 0.0319, 0.0258],
+                [1.8653, 0.8300, 0.4600, 0.3300, 0.2300, 0.1900, 0.1400, 0.1200, 0.0900, 0.0900],
+                [4.3590, 2.0000, 1.2000, 0.9200, 0.6500, 0.5700, 0.4400, 0.4000, 0.3200, 0.3000]
+            ])
+
+        elif kendall[0:5] == 'M/E2/n':
+            # Create dataframe with data from Groenveld (2007) - Table IV (M/E2/n)
+            # See also PIANC 2014 Table 6.1
+            utilisations = np.array([.1, .15, .2, .25, .3, .35, .4, .45, .5, .55, .6, .65, .7, .75, .8, .85, .9])
+            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14])
+            data = np.array([
+                [0.08, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.13, 0.02, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.19, 0.03, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.25, 0.05, 0.02, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.32, 0.08, 0.03, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.40, 0.11, 0.04, 0.02, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.50, 0.15, 0.06, 0.03, 0.02, 0.01, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.60, 0.20, 0.08, 0.05, 0.03, 0.02, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.75, 0.26, 0.12, 0.07, 0.04, 0.03, 0.02, 0.01, 0.01, 0.01, 0.00, 0.00, 0.00, 0.00],
+                [0.91, 0.33, 0.16, 0.10, 0.06, 0.04, 0.03, 0.02, 0.02, 0.01, 0.01, 0.01, 0.00, 0.00],
+                [1.13, 0.43, 0.23, 0.14, 0.09, 0.06, 0.05, 0.03, 0.03, 0.02, 0.02, 0.01, 0.01, 0.01],
+                [1.38, 0.55, 0.30, 0.19, 0.12, 0.09, 0.07, 0.05, 0.04, 0.03, 0.03, 0.02, 0.02, 0.02],
+                [1.75, 0.73, 0.42, 0.27, 0.19, 0.14, 0.11, 0.09, 0.07, 0.06, 0.05, 0.04, 0.03, 0.03],
+                [2.22, 0.96, 0.59, 0.39, 0.28, 0.21, 0.17, 0.14, 0.12, 0.10, 0.08, 0.07, 0.06, 0.05],
+                [3.00, 1.34, 0.82, 0.57, 0.42, 0.33, 0.27, 0.22, 0.18, 0.16, 0.13, 0.11, 0.10, 0.09],
+                [4.50, 2.00, 1.34, 0.90, 0.70, 0.54, 0.46, 0.39, 0.34, 0.30, 0.26, 0.23, 0.20, 0.18],
+                [6.75, 3.14, 2.01, 1.45, 1.12, 0.91, 0.76, 0.65, 0.56, 0.50, 0.45, 0.40, 0.36, 0.33]
+            ])
+
+        df = pd.DataFrame(data, index=utilisations, columns=nr_of_servers)
+
+        # Create a 6th order polynomial fit through the data (for nr_of_stations_chk)
+        target = df.loc[:, nr_of_servers_to_chk];
+        p_p = np.polyfit(target.index, target.values, poly_order)
+
+        waiting_factor = np.polyval(p_p, utilisation)
+        # todo: when the nr of servers > 10 the waiting factor should be set to inf (definitively more equipment needed)
+
+        # Return waiting factor
+        return waiting_factor
+
+    def waitingfactor_to_occupancy(self, factor=.3, nr_of_servers_to_chk=4, poly_order=6):
+        """
+        Waiting time factor (E2/E2/n or M/E2/n) queueing theory using 6th order polynomial regression)
+        """
+
+        kendall = "{}/{}/{}".format(self.A.symbol, self.S.symbol, str(self.c))
+
+        if kendall[0:4] == 'M/M/':
+            # Create dataframe with data from Groenveld (2007) - Table I (M/M/n)
+            # See also PIANC 2014 Table 6.2
+            utilisations = np.array([.1, .2, .3, .4, .5, .6, .7, .8, .9])
+            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
+            data = np.array([
+                [0.1111, 0.0101, 0.0014, 0.0002, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
+                [0.2500, 0.0417, 0.0103, 0.0030, 0.0010, 0.0003, 0.0001, 0.0000, 0.0000, 0.0000],
+                [0.4286, 0.0989, 0.0333, 0.0132, 0.0058, 0.0027, 0.0013, 0.0006, 0.0003, 0.0002],
+                [0.6667, 0.1905, 0.0784, 0.0378, 0.0199, 0.0111, 0.0064, 0.0039, 0.0024, 0.0015],
+                [1.0000, 0.3333, 0.1579, 0.0870, 0.0521, 0.0330, 0.0218, 0.0148, 0.0102, 0.0072],
+                [1.5000, 0.5625, 0.2956, 0.1794, 0.1181, 0.0819, 0.0589, 0.0436, 0.0330, 0.0253],
+                [2.3333, 0.9608, 0.5470, 0.3572, 0.2519, 0.1867, 0.1432, 0.1128, 0.0906, 0.0739],
+                [4.0000, 1.7778, 1.0787, 0.7455, 0.5541, 0.4315, 0.3471, 0.2860, 0.2401, 0.2046],
+                [9.0000, 4.2632, 2.7235, 1.9693, 1.5250, 1.2335, 1.0285, 0.8769, 0.7606, 0.6687]])
+
+        elif kendall[0:6] == 'E2/E2/':
+            # Create dataframe with data from Groenveld (2007) - Table V (E2/E2/n)
+            # See also PIANC 2014 Table 6.2
+            utilisations = np.array([.1, .2, .3, .4, .5, .6, .7, .8, .9])
+            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
+            data = np.array([
+                [0.0166, 0.0006, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
+                [0.0604, 0.0065, 0.0011, 0.0002, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000, 0.0000],
+                [0.1310, 0.0235, 0.0062, 0.0019, 0.0007, 0.0002, 0.0001, 0.0000, 0.0000, 0.0000],
+                [0.2355, 0.0576, 0.0205, 0.0085, 0.0039, 0.0019, 0.0009, 0.0005, 0.0003, 0.0001],
+                [0.3904, 0.1181, 0.0512, 0.0532, 0.0142, 0.0082, 0.0050, 0.0031, 0.0020, 0.0013],
+                [0.6306, 0.2222, 0.1103, 0.0639, 0.0400, 0.0265, 0.0182, 0.0128, 0.0093, 0.0069],
+                [1.0391, 0.4125, 0.2275, 0.1441, 0.0988, 0.0712, 0.0532, 0.0407, 0.0319, 0.0258],
+                [1.8653, 0.8300, 0.4600, 0.3300, 0.2300, 0.1900, 0.1400, 0.1200, 0.0900, 0.0900],
+                [4.3590, 2.0000, 1.2000, 0.9200, 0.6500, 0.5700, 0.4400, 0.4000, 0.3200, 0.3000]
+            ])
+
+        elif kendall[0:5] == 'M/E2/n':
+            # Create dataframe with data from Groenveld (2007) - Table IV (M/E2/n)
+            # See also PIANC 2014 Table 6.1
+            utilisations = np.array([.1, .15, .2, .25, .3, .35, .4, .45, .5, .55, .6, .65, .7, .75, .8, .85, .9])
+            nr_of_servers = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14])
+            data = np.array([
+                [0.08, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.13, 0.02, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.19, 0.03, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.25, 0.05, 0.02, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.32, 0.08, 0.03, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.40, 0.11, 0.04, 0.02, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.50, 0.15, 0.06, 0.03, 0.02, 0.01, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.60, 0.20, 0.08, 0.05, 0.03, 0.02, 0.01, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
+                [0.75, 0.26, 0.12, 0.07, 0.04, 0.03, 0.02, 0.01, 0.01, 0.01, 0.00, 0.00, 0.00, 0.00],
+                [0.91, 0.33, 0.16, 0.10, 0.06, 0.04, 0.03, 0.02, 0.02, 0.01, 0.01, 0.01, 0.00, 0.00],
+                [1.13, 0.43, 0.23, 0.14, 0.09, 0.06, 0.05, 0.03, 0.03, 0.02, 0.02, 0.01, 0.01, 0.01],
+                [1.38, 0.55, 0.30, 0.19, 0.12, 0.09, 0.07, 0.05, 0.04, 0.03, 0.03, 0.02, 0.02, 0.02],
+                [1.75, 0.73, 0.42, 0.27, 0.19, 0.14, 0.11, 0.09, 0.07, 0.06, 0.05, 0.04, 0.03, 0.03],
+                [2.22, 0.96, 0.59, 0.39, 0.28, 0.21, 0.17, 0.14, 0.12, 0.10, 0.08, 0.07, 0.06, 0.05],
+                [3.00, 1.34, 0.82, 0.57, 0.42, 0.33, 0.27, 0.22, 0.18, 0.16, 0.13, 0.11, 0.10, 0.09],
+                [4.50, 2.00, 1.34, 0.90, 0.70, 0.54, 0.46, 0.39, 0.34, 0.30, 0.26, 0.23, 0.20, 0.18],
+                [6.75, 3.14, 2.01, 1.45, 1.12, 0.91, 0.76, 0.65, 0.56, 0.50, 0.45, 0.40, 0.36, 0.33]
+            ])
+
+        df = pd.DataFrame(data, index=utilisations, columns=nr_of_servers)
+
+        # Create a 6th order polynomial fit through the data (for nr_of_stations_chk)
+        target = df.loc[:, nr_of_servers_to_chk]
+        p_p = np.polyfit(target.values, target.index, poly_order)
+
+        occupancy = np.polyval(p_p, factor)
+
+        # Return occupancy
+        return occupancy
```

### Comparing `OpenQTSim-0.5.0/openqtsim/service_process.py` & `openqtsim-0.5.1/openqtsim/arrival_process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-
-
-class ServiceProcess:
-    """
-    Server process class for use in the OpenQTSim package
-    """
-
-    def __init__(self, symbol='M', srv_rate=9):
-        """
-        symbol: symbol of the process (M, E_k, etc.)
-        srv_rate: services per hour
-        """
-
-        self.symbol = symbol
-        self.srv_rate = srv_rate
-
-    def get_ST(self, server, customer_nr=[]):
-        """
-        Return the inter arrival time based on the inter arrival time distribution or deterministic list
-        """
-
-        if self.symbol == "M" or self.symbol == "E2":
-            return server.service_distribution.rvs()
-
-        elif self.symbol == "D":
-            return server.service_distribution.loc[customer_nr, ['ST']].item()
+
+
+class ArrivalProcess:
+    """
+    Arrival process class for use in the OpenQTSim package
+    """
+
+    def __init__(self, symbol='M', arr_rate=8):
+        """
+        symbol: symbol of the process (M, E_k, etc.)
+        arr_rate: arrivals per hour
+        """
+
+        self.symbol = symbol
+        self.arr_rate = arr_rate
+
+    def get_IAT(self, customer_nr=[]):
+        """
+        Return the inter arrival time based on the inter arrival time distribution or deterministic list
+        """
+
+        if self.symbol == "M" or self.symbol[0] == "E":
+            return self.arrival_distribution.rvs()
+
+        elif self.symbol == "D":
+            return self.arrival_distribution.loc[customer_nr, ['IAT']].item()
```

### Comparing `OpenQTSim-0.5.0/setup.cfg` & `openqtsim-0.5.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,73 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 204f 7065 6e51 5453 696d 0d0a 6465   = OpenQTSim..de
-00000020: 7363 7269 7074 696f 6e20 3d20 5468 6973  scription = This
-00000030: 2070 6163 6b61 6765 2066 6163 696c 6974   package facilit
-00000040: 6174 6573 2064 6973 6372 6574 6520 6576  ates discrete ev
-00000050: 656e 7420 7369 6d75 6c61 7469 6f6e 206f  ent simulation o
-00000060: 6620 7175 6575 6573 2077 6974 6820 6120  f queues with a 
-00000070: 4b65 6e64 616c 6c20 6e6f 7461 7469 6f6e  Kendall notation
-00000080: 2e0d 0a61 7574 686f 7220 3d20 4d61 726b  ...author = Mark
-00000090: 2076 616e 204b 6f6e 696e 6773 7665 6c64   van Koningsveld
-000000a0: 2061 6e64 204a 6f72 6973 2064 656e 2055   and Joris den U
-000000b0: 696a 6c0d 0a61 7574 686f 722d 656d 6169  ijl..author-emai
-000000c0: 6c20 3d20 6d2e 7661 6e6b 6f6e 696e 6773  l = m.vankonings
-000000d0: 7665 6c64 4074 7564 656c 6674 2e6e 6c0d  veld@tudelft.nl.
-000000e0: 0a6c 6963 656e 7365 203d 206d 6974 0d0a  .license = mit..
-000000f0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000100: 7468 7562 2e63 6f6d 2f54 5544 656c 6674  thub.com/TUDelft
-00000110: 2d43 4954 472f 4f70 656e 5154 5369 6d0d  -CITG/OpenQTSim.
-00000120: 0a6c 6f6e 672d 6465 7363 7269 7074 696f  .long-descriptio
-00000130: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-00000140: 2e6d 640d 0a70 6c61 7466 6f72 6d73 203d  .md..platforms =
-00000150: 2061 6e79 0d0a 636c 6173 7369 6669 6572   any..classifier
-00000160: 7320 3d20 0d0a 090d 0a09 4465 7665 6c6f  s = ......Develo
-00000170: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-00000180: 3420 2d20 4265 7461 0d0a 090d 0a09 5072  4 - Beta......Pr
-00000190: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001a0: 6765 203a 3a20 5079 7468 6f6e 0d0a 0d0a  ge :: Python....
-000001b0: 5b6f 7074 696f 6e73 5d0d 0a7a 6970 5f73  [options]..zip_s
-000001c0: 6166 6520 3d20 4661 6c73 650d 0a70 6163  afe = False..pac
-000001d0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
-000001e0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-000001f0: 6174 6120 3d20 5472 7565 0d0a 7365 7475  ata = True..setu
-00000200: 705f 7265 7175 6972 6573 203d 2070 7973  p_requires = pys
-00000210: 6361 6666 6f6c 643e 3d33 2e31 6130 2c3c  caffold>=3.1a0,<
-00000220: 332e 3261 300d 0a69 6e73 7461 6c6c 5f72  3.2a0..install_r
-00000230: 6571 7569 7265 7320 3d20 0d0a 0973 696d  equires = ...sim
-00000240: 7079 0d0a 096e 756d 7079 0d0a 0970 616e  py...numpy...pan
-00000250: 6461 730d 0a09 7363 6970 790d 0a09 7079  das...scipy...py
-00000260: 7363 6166 666f 6c64 0d0a 0973 7068 696e  scaffold...sphin
-00000270: 780d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  x....[options.pa
-00000280: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000290: 6572 6520 3d20 6f70 656e 7174 7369 6d0d  ere = openqtsim.
-000002a0: 0a0d 0a5b 6f70 7469 6f6e 732e 6578 7472  ...[options.extr
-000002b0: 6173 5f72 6571 7569 7265 5d0d 0a74 6573  as_require]..tes
-000002c0: 7469 6e67 203d 200d 0a09 7079 7465 7374  ting = ...pytest
-000002d0: 0d0a 0970 7974 6573 742d 636f 760d 0a0d  ...pytest-cov...
-000002e0: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-000002f0: 706f 696e 7473 5d0d 0a0d 0a5b 746f 6f6c  points]....[tool
-00000300: 3a70 7974 6573 745d 0d0a 6164 646f 7074  :pytest]..addopt
-00000310: 7320 3d20 0d0a 092d 2d63 6f76 202d 2d63  s = ...--cov --c
-00000320: 6f76 2d72 6570 6f72 7420 7465 726d 2d6d  ov-report term-m
-00000330: 6973 7369 6e67 202d 2d63 6f76 2d72 6570  issing --cov-rep
-00000340: 6f72 7420 6874 6d6c 0d0a 092d 2d76 6572  ort html...--ver
-00000350: 626f 7365 0d0a 6e6f 7265 6375 7273 6564  bose..norecursed
-00000360: 6972 7320 3d20 0d0a 0964 6973 740d 0a09  irs = ...dist...
-00000370: 6275 696c 640d 0a09 2e74 6f78 0d0a 092e  build....tox....
-00000380: 6567 6773 0d0a 7465 7374 7061 7468 7320  eggs..testpaths 
-00000390: 3d20 7465 7374 730d 0a0d 0a5b 616c 6961  = tests....[alia
-000003a0: 7365 735d 0d0a 646f 6373 203d 2062 7569  ses]..docs = bui
-000003b0: 6c64 5f73 7068 696e 780d 0a74 6573 7420  ld_sphinx..test 
-000003c0: 3d20 7079 7465 7374 0d0a 0d0a 5b62 6469  = pytest....[bdi
-000003d0: 7374 5f77 6865 656c 5d0d 0a75 6e69 7665  st_wheel]..unive
-000003e0: 7273 616c 203d 2031 0d0a 0d0a 5b62 7569  rsal = 1....[bui
-000003f0: 6c64 5f73 7068 696e 785d 0d0a 736f 7572  ld_sphinx]..sour
-00000400: 6365 5f64 6972 203d 2064 6f63 730d 0a62  ce_dir = docs..b
-00000410: 7569 6c64 5f64 6972 203d 2064 6f63 732f  uild_dir = docs/
-00000420: 5f62 7569 6c64 0d0a 0d0a 5b64 6576 7069  _build....[devpi
-00000430: 3a75 706c 6f61 645d 0d0a 6e6f 2d76 6373  :upload]..no-vcs
-00000440: 203d 2031 0d0a 666f 726d 6174 7320 3d20   = 1..formats = 
-00000450: 6264 6973 745f 7768 6565 6c0d 0a0d 0a5b  bdist_wheel....[
-00000460: 666c 616b 6538 5d0d 0a65 7863 6c75 6465  flake8]..exclude
-00000470: 203d 200d 0a09 2e74 6f78 0d0a 0962 7569   = ....tox...bui
-00000480: 6c64 0d0a 0964 6973 740d 0a09 2e65 6767  ld...dist....egg
-00000490: 730d 0a09 646f 6373 2f63 6f6e 662e 7079  s...docs/conf.py
-000004a0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000004b0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000004c0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 4f70 656e 5154 5369 6d0a 6465 7363  = OpenQTSim.desc
+00000020: 7269 7074 696f 6e20 3d20 5468 6973 2070  ription = This p
+00000030: 6163 6b61 6765 2066 6163 696c 6974 6174  ackage facilitat
+00000040: 6573 2064 6973 6372 6574 6520 6576 656e  es discrete even
+00000050: 7420 7369 6d75 6c61 7469 6f6e 206f 6620  t simulation of 
+00000060: 7175 6575 6573 2077 6974 6820 6120 4b65  queues with a Ke
+00000070: 6e64 616c 6c20 6e6f 7461 7469 6f6e 2e0a  ndall notation..
+00000080: 6175 7468 6f72 203d 204d 6172 6b20 7661  author = Mark va
+00000090: 6e20 4b6f 6e69 6e67 7376 656c 6420 616e  n Koningsveld an
+000000a0: 6420 4a6f 7269 7320 6465 6e20 5569 6a6c  d Joris den Uijl
+000000b0: 0a61 7574 686f 722d 656d 6169 6c20 3d20  .author-email = 
+000000c0: 6d2e 7661 6e6b 6f6e 696e 6773 7665 6c64  m.vankoningsveld
+000000d0: 4074 7564 656c 6674 2e6e 6c0a 6c69 6365  @tudelft.nl.lice
+000000e0: 6e73 6520 3d20 6d69 740a 7572 6c20 3d20  nse = mit.url = 
+000000f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000100: 6f6d 2f54 5544 656c 6674 2d43 4954 472f  om/TUDelft-CITG/
+00000110: 4f70 656e 5154 5369 6d0a 6c6f 6e67 2d64  OpenQTSim.long-d
+00000120: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+00000130: 653a 2052 4541 444d 452e 6d64 0a70 6c61  e: README.md.pla
+00000140: 7466 6f72 6d73 203d 2061 6e79 0a63 6c61  tforms = any.cla
+00000150: 7373 6966 6965 7273 203d 200a 090a 0944  ssifiers = ....D
+00000160: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
+00000170: 7320 3a3a 2034 202d 2042 6574 610a 090a  s :: 4 - Beta...
+00000180: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000190: 6775 6167 6520 3a3a 2050 7974 686f 6e0a  guage :: Python.
+000001a0: 0a5b 6f70 7469 6f6e 735d 0a7a 6970 5f73  .[options].zip_s
+000001b0: 6166 6520 3d20 4661 6c73 650a 7061 636b  afe = False.pack
+000001c0: 6167 6573 203d 2066 696e 643a 0a69 6e63  ages = find:.inc
+000001d0: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+000001e0: 6120 3d20 5472 7565 0a73 6574 7570 5f72  a = True.setup_r
+000001f0: 6571 7569 7265 7320 3d20 7079 7363 6166  equires = pyscaf
+00000200: 666f 6c64 3e3d 332e 3161 302c 3c33 2e32  fold>=3.1a0,<3.2
+00000210: 6130 0a69 6e73 7461 6c6c 5f72 6571 7569  a0.install_requi
+00000220: 7265 7320 3d20 0a09 7369 6d70 790a 096e  res = ..simpy..n
+00000230: 756d 7079 0a09 7061 6e64 6173 0a09 7363  umpy..pandas..sc
+00000240: 6970 790a 0970 7973 6361 6666 6f6c 640a  ipy..pyscaffold.
+00000250: 0973 7068 696e 780a 0a5b 6f70 7469 6f6e  .sphinx..[option
+00000260: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000270: 0a77 6865 7265 203d 206f 7065 6e71 7473  .where = openqts
+00000280: 696d 0a0a 5b6f 7074 696f 6e73 2e65 7874  im..[options.ext
+00000290: 7261 735f 7265 7175 6972 655d 0a74 6573  ras_require].tes
+000002a0: 7469 6e67 203d 200a 0970 7974 6573 740a  ting = ..pytest.
+000002b0: 0970 7974 6573 742d 636f 760a 0a5b 6f70  .pytest-cov..[op
+000002c0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+000002d0: 7473 5d0a 0a5b 746f 6f6c 3a70 7974 6573  ts]..[tool:pytes
+000002e0: 745d 0a61 6464 6f70 7473 203d 200a 092d  t].addopts = ..-
+000002f0: 2d63 6f76 202d 2d63 6f76 2d72 6570 6f72  -cov --cov-repor
+00000300: 7420 7465 726d 2d6d 6973 7369 6e67 202d  t term-missing -
+00000310: 2d63 6f76 2d72 6570 6f72 7420 6874 6d6c  -cov-report html
+00000320: 0a09 2d2d 7665 7262 6f73 650a 6e6f 7265  ..--verbose.nore
+00000330: 6375 7273 6564 6972 7320 3d20 0a09 6469  cursedirs = ..di
+00000340: 7374 0a09 6275 696c 640a 092e 746f 780a  st..build...tox.
+00000350: 092e 6567 6773 0a74 6573 7470 6174 6873  ..eggs.testpaths
+00000360: 203d 2074 6573 7473 0a0a 5b61 6c69 6173   = tests..[alias
+00000370: 6573 5d0a 646f 6373 203d 2062 7569 6c64  es].docs = build
+00000380: 5f73 7068 696e 780a 7465 7374 203d 2070  _sphinx.test = p
+00000390: 7974 6573 740a 0a5b 6264 6973 745f 7768  ytest..[bdist_wh
+000003a0: 6565 6c5d 0a75 6e69 7665 7273 616c 203d  eel].universal =
+000003b0: 2031 0a0a 5b62 7569 6c64 5f73 7068 696e   1..[build_sphin
+000003c0: 785d 0a73 6f75 7263 655f 6469 7220 3d20  x].source_dir = 
+000003d0: 646f 6373 0a62 7569 6c64 5f64 6972 203d  docs.build_dir =
+000003e0: 2064 6f63 732f 5f62 7569 6c64 0a0a 5b64   docs/_build..[d
+000003f0: 6576 7069 3a75 706c 6f61 645d 0a6e 6f2d  evpi:upload].no-
+00000400: 7663 7320 3d20 310a 666f 726d 6174 7320  vcs = 1.formats 
+00000410: 3d20 6264 6973 745f 7768 6565 6c0a 0a5b  = bdist_wheel..[
+00000420: 666c 616b 6538 5d0a 6578 636c 7564 6520  flake8].exclude 
+00000430: 3d20 0a09 2e74 6f78 0a09 6275 696c 640a  = ...tox..build.
+00000440: 0964 6973 740a 092e 6567 6773 0a09 646f  .dist...eggs..do
+00000450: 6373 2f63 6f6e 662e 7079 0a0a 5b65 6767  cs/conf.py..[egg
+00000460: 5f69 6e66 6f5d 0a74 6167 5f62 7569 6c64  _info].tag_build
+00000470: 203d 200a 7461 675f 6461 7465 203d 2030   = .tag_date = 0
+00000480: 0a0a                                     ..
```

