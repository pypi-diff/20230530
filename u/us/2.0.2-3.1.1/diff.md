# Comparing `tmp/us-2.0.2.tar.gz` & `tmp/us-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/us-2.0.2.tar", last modified: Wed Apr 29 05:11:44 2020, max compression
+gzip compressed data, was "us-3.1.1.tar", last modified: Tue May 30 19:13:11 2023, max compression
```

## Comparing `us-2.0.2.tar` & `us-3.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2020-04-29 05:11:44.626249 us-2.0.2/
--rw-r--r--   0 jeremy     (501) staff       (20)     1514 2019-11-27 05:28:15.000000 us-2.0.2/LICENSE
--rw-r--r--   0 jeremy     (501) staff       (20)       22 2019-11-27 06:39:59.000000 us-2.0.2/MANIFEST.in
--rw-r--r--   0 jeremy     (501) staff       (20)    10057 2020-04-29 05:11:44.625898 us-2.0.2/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)     7219 2020-04-29 04:44:32.000000 us-2.0.2/README.rst
--rw-r--r--   0 jeremy     (501) staff       (20)       38 2020-04-29 05:11:44.626408 us-2.0.2/setup.cfg
--rw-r--r--   0 jeremy     (501) staff       (20)      802 2020-04-29 04:59:47.000000 us-2.0.2/setup.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2020-04-29 05:11:44.620967 us-2.0.2/us/
--rw-r--r--   0 jeremy     (501) staff       (20)      195 2020-04-29 04:27:20.000000 us-2.0.2/us/__init__.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2020-04-29 05:11:44.624353 us-2.0.2/us/cli/
--rw-r--r--   0 jeremy     (501) staff       (20)        0 2019-11-27 05:28:15.000000 us-2.0.2/us/cli/__init__.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1340 2020-04-23 05:50:58.000000 us-2.0.2/us/cli/states.py
--rw-r--r--   0 jeremy     (501) staff       (20)    31350 2020-04-29 04:45:07.000000 us-2.0.2/us/states.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2020-04-29 05:11:44.625189 us-2.0.2/us/tests/
--rw-r--r--   0 jeremy     (501) staff       (20)        0 2019-11-27 06:20:25.000000 us-2.0.2/us/tests/__init__.py
--rw-r--r--   0 jeremy     (501) staff       (20)     3496 2020-04-29 04:39:37.000000 us-2.0.2/us/tests/test_us.py
--rw-r--r--   0 jeremy     (501) staff       (20)       74 2020-04-18 18:29:18.000000 us-2.0.2/us/unitedstatesofamerica.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2020-04-29 05:11:44.623629 us-2.0.2/us.egg-info/
--rw-r--r--   0 jeremy     (501) staff       (20)    10057 2020-04-29 05:11:44.000000 us-2.0.2/us.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)      330 2020-04-29 05:11:44.000000 us-2.0.2/us.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        1 2020-04-29 05:11:44.000000 us-2.0.2/us.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       47 2020-04-29 05:11:44.000000 us-2.0.2/us.egg-info/entry_points.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       17 2020-04-29 05:11:44.000000 us-2.0.2/us.egg-info/requires.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        3 2020-04-29 05:11:44.000000 us-2.0.2/us.egg-info/top_level.txt
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-30 19:13:11.735077 us-3.1.1/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1514 2019-11-27 05:28:15.000000 us-3.1.1/LICENSE
+-rw-r--r--   0 jeremy     (501) staff       (20)       22 2019-11-27 06:39:59.000000 us-3.1.1/MANIFEST.in
+-rw-r--r--   0 jeremy     (501) staff       (20)     8513 2023-05-30 19:13:11.734571 us-3.1.1/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)     7948 2023-05-30 17:33:10.000000 us-3.1.1/README.rst
+-rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-05-30 19:13:11.735190 us-3.1.1/setup.cfg
+-rw-r--r--   0 jeremy     (501) staff       (20)      903 2023-05-30 17:33:10.000000 us-3.1.1/setup.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-30 19:13:11.728783 us-3.1.1/us/
+-rw-r--r--   0 jeremy     (501) staff       (20)      251 2023-05-30 17:33:10.000000 us-3.1.1/us/__init__.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-30 19:13:11.732822 us-3.1.1/us/cli/
+-rw-r--r--   0 jeremy     (501) staff       (20)        0 2019-11-27 05:28:15.000000 us-3.1.1/us/cli/__init__.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1337 2023-05-30 17:33:10.000000 us-3.1.1/us/cli/states.py
+-rw-r--r--   0 jeremy     (501) staff       (20)    31970 2023-05-30 17:33:10.000000 us-3.1.1/us/states.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-30 19:13:11.733772 us-3.1.1/us/tests/
+-rw-r--r--   0 jeremy     (501) staff       (20)        0 2020-04-29 20:26:59.000000 us-3.1.1/us/tests/__init__.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     3500 2023-05-30 17:33:10.000000 us-3.1.1/us/tests/test_us.py
+-rw-r--r--   0 jeremy     (501) staff       (20)       74 2020-04-18 18:29:18.000000 us-3.1.1/us/unitedstatesofamerica.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-30 19:13:11.732002 us-3.1.1/us.egg-info/
+-rw-r--r--   0 jeremy     (501) staff       (20)     8513 2023-05-30 19:13:11.000000 us-3.1.1/us.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)      330 2023-05-30 19:13:11.000000 us-3.1.1/us.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-05-30 19:13:11.000000 us-3.1.1/us.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       46 2023-05-30 19:13:11.000000 us-3.1.1/us.egg-info/entry_points.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       18 2023-05-30 19:13:11.000000 us-3.1.1/us.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        3 2023-05-30 19:13:11.000000 us-3.1.1/us.egg-info/top_level.txt
```

### Comparing `us-2.0.2/LICENSE` & `us-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `us-2.0.2/README.rst` & `us-3.1.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -32,48 +32,53 @@
 
 Easy access to state information: ::
 
     >>> import us
     >>> us.states.MD
     <State:Maryland>
     >>> us.states.MD.fips
-    u'24'
+    '24'
     >>> us.states.MD.name
-    u'Maryland'
+    'Maryland'
     >>> us.states.MD.is_contiguous
     True
 
 Includes territories too: ::
 
     >>> us.states.VI.name
-    u'Virgin Islands'
+    'Virgin Islands'
     >>> us.states.VI.is_territory
     True
     >>> us.states.MD.is_territory
     False
 
 List of all (actual) states: ::
 
     >>> us.states.STATES
-    [<State:Alabama>, <State:Alaska>, <State:Arizona>, <State:Arkansas>,...
+    [<State:Alabama>, <State:Alaska>, <State:Arizona>, <State:Arkansas>, ...
     >>> us.states.TERRITORIES
-    [<State:American Samoa>, <State:Guam>, <State:Northern Mariana Islands>,...
+    [<State:American Samoa>, <State:Guam>, <State:Northern Mariana Islands>, ...
 
 And the whole shebang, if you want it: ::
 
     >>> us.states.STATES_AND_TERRITORIES
-    [<State:Alabama>, <State:Alaska>, <State:American Samoa>,...
+    [<State:Alabama>, <State:Alaska>, <State:American Samoa>, ...
 
 For convenience, `STATES`, `TERRITORIES`, and `STATES_AND_TERRITORIES` can be
 accessed directly from the `us` module: ::
 
     >>> us.states.STATES
-    [<State:Alabama>, <State:Alaska>, <State:Arizona>, <State:Arkansas>,...
+    [<State:Alabama>, <State:Alaska>, <State:Arizona>, <State:Arkansas>, ...
     >>> us.STATES
-    [<State:Alabama>, <State:Alaska>, <State:Arizona>, <State:Arkansas>,...
+    [<State:Alabama>, <State:Alaska>, <State:Arizona>, <State:Arkansas>, ...
+
+Some states like to be fancy and call themselves commonwealths: ::
+
+    >>> us.states.COMMONWEALTHS
+    [<State:Kentucky>, <State:Massachusetts>, <State:Pennsylvania>, <State:Virginia>]
 
 There's also a list of obsolete territories: ::
 
     >>> us.states.OBSOLETE
     [<State:Dakota>, <State:Orleans>, <State:Philippine Islands>]
 
 The state lookup method allows matching by FIPS code, abbreviation, and name: ::
@@ -87,68 +92,82 @@
     >>> us.states.lookup('maryland')
     <State:Maryland>
 
 Get useful information: ::
 
     >>> state = us.states.lookup('maryland')
     >>> state.abbr
-    u'MD'
+    'MD'
 
 
 And for those days that you just can't remember how to spell Mississippi,
 we've got phonetic name matching too: ::
 
     >>> us.states.lookup('misisipi')
     <State:Mississippi>
 
 
 Shapefiles
 ----------
 
-You want shapefiles too? Gotcha covered.
+You want shapefiles too? As long as you want 2010 shapefiles, we've gotcha covered.
 
 ::
 
-    >>> shpurls = us.states.MD.shapefile_urls()
-    >>> for region, url in shpurls.items():
-    ...   print "%s: %s" % (region, url)
-    ...
-    county: http://www2.census.gov/geo/tiger/TIGER2010/COUNTY/2010/tl_2010_24_county10.zip
-    state: http://www2.census.gov/geo/tiger/TIGER2010/STATE/2010/tl_2010_24_state10.zip
-    cd: http://www2.census.gov/geo/tiger/TIGER2010/CD/111/tl_2010_24_cd111.zip
-    zcta: http://www2.census.gov/geo/tiger/TIGER2010/ZCTA5/2010/tl_2010_24_zcta510.zip
-    tract: http://www2.census.gov/geo/tiger/TIGER2010/TRACT/2010/tl_2010_24_tract10.zip
+    >>> urls = us.states.MD.shapefile_urls()
+    >>> sorted(urls.keys())
+    ['block', 'blockgroup', 'cd', 'county', 'state', 'tract', 'zcta']
+    >>> urls['block']
+    'https://www2.census.gov/geo/tiger/TIGER2010/TABBLOCK/2010/tl_2010_24_tabblock10.zip'
 
 The `shapefile_urls()` method on the State object generates shapefile URLs for
 the following regions:
 
-* state
+* block
+* blockgroup
+* census tract (tract)
+* congressional district (cd)
 * county
-* congressional district
+* state
 * zcta
-* census tract
-
-If you know what region you want, you can explicitly request it: ::
-
-    >>> us.states.MD.shapefile_urls('county')
-    u'http://www2.census.gov/geo/tiger/TIGER2010/COUNTY/2010/tl_2010_24_county10.zip'
 
 
 Mappings
 --------
 
 Mappings between various state attributes are a common need. The `mapping()`
 method will generate a lookup between two specified fields.
 
 ::
 
     >>> us.states.mapping('fips', 'abbr')
-    {u'30': u'MT', u'54': u'WV', u'42': u'PA', u'48': u'TX', u'45': u'SC',...
+    {'01': 'AL', '02': 'AK', '04': 'AZ', '05': 'AR', '06': 'CA', ...
     >>> us.states.mapping('abbr', 'name')
-    {u'WA': u'Washington', u'VA': u'Virginia', u'DE': u'Delaware',...
+    {'AL': 'Alabama', 'AK': 'Alaska', 'AZ': 'Arizona', 'AR': 'Arkansas', ...
+
+This method uses `us.STATES_AND_TERRITORIES` as the default list of states
+it will create a mapping for, but this can be overridden by passing an
+additional states argument: ::
+
+    >>> us.states.mapping('fips', 'abbr', states=[us.states.DC])
+    {'11': 'DC'}
+
+
+DC should be granted statehood
+------------------------------
+
+Washington, DC does not appear in `us.STATES` or any of the
+related state lists, but is often treated as a state in practice and
+should be granted statehood anyway. DC can be automatically included in these
+lists by setting a `DC_STATEHOOD` environment variable to any truthy value
+before importing this package.
+
+::
+
+    DC_STATEHOOD=1
 
 
 CLI
 ----
 
 When you need to know state information RIGHT AWAY, there's the *states* script.
 
@@ -160,60 +179,75 @@
 
       FIPS code: 24
 
       other attributes:
         ap_abbr: Md.
         capital: Annapolis
         capital_tz: America/New_York
+        is_contiguous: True
+        is_continental: True
         is_obsolete: False
         name_metaphone: MRLNT
         statehood_year: 1788
         time_zones: America/New_York
 
       shapefiles:
-        blockgroup: http://www2.census.gov/geo/tiger/TIGER2010/BG/2010/tl_2010_24_bg10.zip
-        cd: http://www2.census.gov/geo/tiger/TIGER2010/CD/111/tl_2010_24_cd111.zip
-        county: http://www2.census.gov/geo/tiger/TIGER2010/COUNTY/2010/tl_2010_24_county10.zip
-        state: http://www2.census.gov/geo/tiger/TIGER2010/STATE/2010/tl_2010_24_state10.zip
-        tract: http://www2.census.gov/geo/tiger/TIGER2010/TRACT/2010/tl_2010_24_tract10.zip
-        zcta: http://www2.census.gov/geo/tiger/TIGER2010/ZCTA5/2010/tl_2010_24_zcta510.zip
-        block: http://www2.census.gov/geo/tiger/TIGER2010/TABBLOCK/2010/tl_2010_24_tabblock10.zip
+        tract: https://www2.census.gov/geo/tiger/TIGER2010/TRACT/2010/tl_2010_24_tract10.zip
+        cd: https://www2.census.gov/geo/tiger/TIGER2010/CD/111/tl_2010_24_cd111.zip
+        county: https://www2.census.gov/geo/tiger/TIGER2010/COUNTY/2010/tl_2010_24_county10.zip
+        state: https://www2.census.gov/geo/tiger/TIGER2010/STATE/2010/tl_2010_24_state10.zip
+        zcta: https://www2.census.gov/geo/tiger/TIGER2010/ZCTA5/2010/tl_2010_24_zcta510.zip
+        block: https://www2.census.gov/geo/tiger/TIGER2010/TABBLOCK/2010/tl_2010_24_tabblock10.zip
+        blockgroup: https://www2.census.gov/geo/tiger/TIGER2010/BG/2010/tl_2010_24_bg10.zip
 
 
 Running Tests
 -------------
 
-CircleCI is set up to automatically run unit tests against any new commits to
-the repo. To run these tests yourself in a standardized, Dockerized
-environment, install
-`the CircleCI CLI <https://circleci.com/docs/2.0/local-cli/>`_, and then
-execute the tests with: ::
-
-    circleci local execute --job build
-
-Alternatively, you can run tests against only your current version of Python,
-using: ::
+GitHub Actions are set up to automatically run unit tests against any new
+commits to the repo. To run these tests yourself: ::
 
-    pytest tests
+    pipenv install --dev
+    pipenv run pytest
 
 
 Changelog
 ---------
 
+3.1.1
+~~~~~
+* add support for Python 3.11
+* upgrade to jellyfish 0.11.2
+
+
+3.0.0
+~~~~~
+
+* upgrade to jellyfish 0.7.2
+* drop support for Python 2.7
+* add us.states.COMMONWEALTHS list of states that call themselves commonwealths 🎩
+* add DC to STATES, STATES_AND_TERRITORIES, STATES_CONTIGUOUS, or STATES_CONTINENTAL when DC_STATEHOOD environment variable is set
+* remove `region` parameter from `shapefile_urls()` method
+* `mapping()` no longer includes obsolete states
+* added type annotations
+
+
 2.0.2
 ~~~~~
 
 * restore DC in lookup() and mapping()
 
+
 2.0.1
 ~~~~~
 
 * fix Python 2.7 tests that ran with Python 3
 * revert to jellyfish 0.6.1 to support Python 2.7
 
+
 2.0.0
 ~~~~~
 
 * add support for Python 3.7 and 3.8
 * remove support for Python 3.4 and 3.5
 * remove pickled objects and database in favor of pure Python code
 * upgrade jellyfish to 0.7.2 to fix metaphone bug
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `us-2.0.2/setup.py` & `us-3.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from setuptools import setup, find_packages
 
 long_description = open("README.rst").read()
 
 setup(
     name="us",
-    version="2.0.2",
+    version="3.1.1",
     author="Jeremy Carbaugh",
     author_email="jeremy@jcarbaugh.com",
     url="https://github.com/unitedstates/python-us",
     description="US state meta information and other fun stuff",
     long_description=long_description,
     license="BSD",
     packages=find_packages(),
     include_package_data=True,
-    install_requires=["jellyfish==0.6.1"],
+    install_requires=["jellyfish==0.11.2"],
     entry_points={"console_scripts": ["states = us.cli.states:main"]},
     platforms=["any"],
     classifiers=[
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `us-2.0.2/us/cli/states.py` & `us-3.1.1/us/cli/states.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 import us
 
 
 def main():
-
     import argparse
 
     parser = argparse.ArgumentParser(description="Lookup state information")
     parser.add_argument(
         "query", metavar="QUERY", nargs=1, help="name, abbreviation, or FIPS code"
     )
 
@@ -15,15 +14,14 @@
 
     state = us.states.lookup(args.query[0])
 
     if not state:
         sys.stdout.write("Sorry, couldn't find a matching state.\n")
 
     else:
-
         data = state.__dict__.copy()
 
         region = "territory" if data.pop("is_territory") else "state"
 
         sys.stdout.write("\n")
         sys.stdout.write(
             "*** The great %s of %s (%s) ***\n\n"
@@ -32,15 +30,14 @@
 
         sys.stdout.write("  FIPS code: %s\n" % data.pop("fips"))
 
         sys.stdout.write("\n")
         sys.stdout.write("  other attributes:\n")
 
         for key in sorted(data.keys()):
-
             val = data[key]
 
             if isinstance(val, (list, tuple)):
                 val = ", ".join(val)
 
             sys.stdout.write("    %s: %s\n" % (key, val))
```

### Comparing `us-2.0.2/us/states.py` & `us-3.1.1/us/states.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,123 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
-import itertools
+import os
 import re
+from typing import Any, Dict, Iterable, List, Optional
+from urllib.parse import urljoin
 
-import jellyfish
+import jellyfish  # type: ignore
 
 FIPS_RE = re.compile(r"^\d{2}$")
 ABBR_RE = re.compile(r"^[a-zA-Z]{2}$")
 
+DC_STATEHOOD = bool(os.environ.get("DC_STATEHOOD"))
 
-_lookup_cache = {}
 
+_lookup_cache: Dict[str, "State"] = {}
+
+
+class State:
+    abbr: str
+    ap_abbr: Optional[str]
+    capital: Optional[str]
+    capital_tz: Optional[str]
+    fips: Optional[str]
+    is_territory: bool
+    is_obsolete: bool
+    is_contiguous: bool
+    is_continental: bool
+    name: str
+    name_metaphone: str
+    statehood_year: Optional[int]
+    time_zones: List[str]
 
-class State(object):
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
-            self.__dict__[k] = v
+            setattr(self, k, v)
 
-    def __repr__(self):
-        return "<State:%s>" % self.name
+    def __repr__(self) -> str:
+        return f"<State:{self.name}>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
-    def shapefile_urls(self, region=None):
+    def shapefile_urls(self) -> Optional[Dict[str, str]]:
+        """Shapefiles are available directly from the US Census Bureau:
+        https://www.census.gov/cgi-bin/geo/shapefiles/index.php
+        """
+
+        fips = self.fips
 
-        if not self.fips:
-            return {}
+        if not fips:
+            return None
 
-        base_url = "https://www2.census.gov/geo/tiger/TIGER2010"
+        base = "https://www2.census.gov/geo/tiger/TIGER2010/"
         urls = {
-            "tract": "{0}/TRACT/2010/tl_2010_{1}_tract10.zip".format(
-                base_url, self.fips
-            ),
-            "cd": "{0}/CD/111/tl_2010_{1}_cd111.zip".format(base_url, self.fips),
-            "county": "{0}/COUNTY/2010/tl_2010_{1}_county10.zip".format(
-                base_url, self.fips
-            ),
-            "state": "{0}/STATE/2010/tl_2010_{1}_state10.zip".format(
-                base_url, self.fips
-            ),
-            "zcta": "{0}/ZCTA5/2010/tl_2010_{1}_zcta510.zip".format(
-                base_url, self.fips
-            ),
-            "block": "{0}/TABBLOCK/2010/tl_2010_{1}_tabblock10.zip".format(
-                base_url, self.fips
-            ),
-            "blockgroup": "{0}/BG/2010/tl_2010_{1}_bg10.zip".format(
-                base_url, self.fips
-            ),
+            "tract": urljoin(base, f"TRACT/2010/tl_2010_{fips}_tract10.zip"),
+            "cd": urljoin(base, f"CD/111/tl_2010_{fips}_cd111.zip"),
+            "county": urljoin(base, f"COUNTY/2010/tl_2010_{fips}_county10.zip"),
+            "state": urljoin(base, f"STATE/2010/tl_2010_{fips}_state10.zip"),
+            "zcta": urljoin(base, f"ZCTA5/2010/tl_2010_{fips}_zcta510.zip"),
+            "block": urljoin(base, f"TABBLOCK/2010/tl_2010_{fips}_tabblock10.zip"),
+            "blockgroup": urljoin(base, f"BG/2010/tl_2010_{fips}_bg10.zip"),
         }
 
-        if region and region in urls:
-            return urls[region]
-
         return urls
 
 
-def lookup(val, field=None, use_cache=True):
-    """ Semi-fuzzy state lookup. This method will make a best effort
-        attempt at finding the state based on the lookup value provided.
-
-          * two digits will search for FIPS code
-          * two letters will search for state abbreviation
-          * anything else will try to match the metaphone of state names
-
-        Metaphone is used to allow for incorrect, but phonetically accurate,
-        spelling of state names.
-
-        Exact matches can be done on any attribute on State objects by passing
-        the `field` argument. This skips the fuzzy-ish matching and does an
-        exact, case-sensitive comparison against the specified field.
+def lookup(val, field: Optional[str] = None, use_cache: bool = True) -> Optional[State]:
+    """Semi-fuzzy state lookup. This method will make a best effort
+    attempt at finding the state based on the lookup value provided.
+
+      * two digits will search for FIPS code
+      * two letters will search for state abbreviation
+      * anything else will try to match the metaphone of state names
+
+    Metaphone is used to allow for incorrect, but phonetically accurate,
+    spelling of state names.
+
+    Exact matches can be done on any attribute on State objects by passing
+    the `field` argument. This skips the fuzzy-ish matching and does an
+    exact, case-sensitive comparison against the specified field.
 
-        This method caches non-None results, but can the cache can be bypassed
-        with the `use_cache=False` argument.
+    This method caches non-None results, but can the cache can be bypassed
+    with the `use_cache=False` argument.
     """
 
+    matched_state = None
+
     if field is None:
         if FIPS_RE.match(val):
             field = "fips"
         elif ABBR_RE.match(val):
             val = val.upper()
             field = "abbr"
         else:
             val = jellyfish.metaphone(val)
             field = "name_metaphone"
 
     # see if result is in cache
-    cache_key = "%s:%s" % (field, val)
+    cache_key = f"{field}:{val}"
     if use_cache and cache_key in _lookup_cache:
-        return _lookup_cache[cache_key]
+        matched_state = _lookup_cache[cache_key]
 
-    for state in itertools.chain(STATES_AND_TERRITORIES, [DC], OBSOLETE):
+    for state in STATES_AND_TERRITORIES:
         if val == getattr(state, field):
-            _lookup_cache[cache_key] = state
-            return state
+            matched_state = state
+            if use_cache:
+                _lookup_cache[cache_key] = state
 
+    return matched_state
 
-def mapping(from_field, to_field, states=None):
+
+def mapping(
+    from_field: str, to_field: str, states: Optional[Iterable[State]] = None
+) -> Dict[Any, Any]:
     if states is None:
-        states = itertools.chain(STATES_AND_TERRITORIES, [DC], OBSOLETE)
-    return dict((getattr(s, from_field), getattr(s, to_field)) for s in states)
+        states = STATES_AND_TERRITORIES
+    return {getattr(s, from_field): getattr(s, to_field) for s in states}
 
 
 AL = State(
     **{
         "fips": "01",
         "name": "Alabama",
         "abbr": "AL",
@@ -1244,17 +1257,17 @@
         "ap_abbr": "Wyo.",
         "time_zones": ["America/Denver"],
         "name_metaphone": "YMNK",
     }
 )
 
 
-OBSOLETE = [DK, OL, PI]
-TERRITORIES = [AS, GU, MP, PR, VI]
-STATES = [
+OBSOLETE: List[State] = [DK, OL, PI]
+TERRITORIES: List[State] = [AS, GU, MP, PR, VI]
+STATES: List[State] = [
     AL,
     AK,
     AZ,
     AR,
     CA,
     CO,
     CT,
@@ -1298,15 +1311,15 @@
     VT,
     VA,
     WA,
     WV,
     WI,
     WY,
 ]
-STATES_CONTIGUOUS = [
+STATES_CONTIGUOUS: List[State] = [
     AL,
     AZ,
     AR,
     CA,
     CO,
     CT,
     DE,
@@ -1348,15 +1361,15 @@
     VT,
     VA,
     WA,
     WV,
     WI,
     WY,
 ]
-STATES_CONTINENTAL = [
+STATES_CONTINENTAL: List[State] = [
     AL,
     AK,
     AZ,
     AR,
     CA,
     CO,
     CT,
@@ -1399,8 +1412,17 @@
     VT,
     VA,
     WA,
     WV,
     WI,
     WY,
 ]
-STATES_AND_TERRITORIES = STATES + TERRITORIES
+
+STATES_AND_TERRITORIES: List[State] = STATES + TERRITORIES
+
+COMMONWEALTHS: List[State] = [KY, MA, PA, VA]
+
+if DC_STATEHOOD:
+    STATES.append(DC)
+    STATES_AND_TERRITORIES.append(DC)
+    STATES_CONTIGUOUS.append(DC)
+    STATES_CONTINENTAL.append(DC)
```

### Comparing `us-2.0.2/us/tests/test_us.py` & `us-3.1.1/us/tests/test_us.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from __future__ import unicode_literals
 from itertools import chain
 
-import jellyfish
-import pytest
+import jellyfish  # type: ignore
+import pytest  # type: ignore
 import pytz
 
 import us
 
 
 # attribute
 
@@ -67,15 +66,15 @@
 def test_name_lookup():
     for state in us.STATES:
         assert us.states.lookup(state.name) == state
 
 
 def test_obsolete_lookup():
     for state in us.OBSOLETE:
-        assert us.states.lookup(state.name) == state
+        assert us.states.lookup(state.name) is None
 
 
 # test metaphone
 
 
 def test_jellyfish_metaphone():
     for state in chain(us.STATES_AND_TERRITORIES, us.OBSOLETE):
@@ -91,15 +90,22 @@
         (s.abbr, s.fips) for s in states
     )
 
 
 def test_obsolete_mapping():
     mapping = us.states.mapping("abbr", "fips")
     for state in us.states.OBSOLETE:
-        assert state.abbr in mapping
+        assert state.abbr not in mapping
+
+
+def test_custom_mapping():
+    mapping = us.states.mapping("abbr", "fips", states=[us.states.DC, us.states.MD])
+    assert len(mapping) == 2
+    assert "DC" in mapping
+    assert "MD" in mapping
 
 
 # known bugs
 
 
 def test_kentucky_uppercase():
     assert us.states.lookup("kentucky") == us.states.KY
@@ -109,28 +115,25 @@
 def test_wayoming():
     assert us.states.lookup("Wyoming") == us.states.WY
     assert us.states.lookup("Wayoming") is None
 
 
 def test_dc():
     assert us.states.DC not in us.STATES
-    assert us.states.lookup("DC") == us.states.DC
-    assert us.states.lookup("District of Columbia") == us.states.DC
-    assert "DC" in us.states.mapping("abbr", "name")
 
 
 # shapefiles
 
 
 @pytest.mark.skip
 def test_head():
     import requests
 
     for state in us.STATES_AND_TERRITORIES:
-        for region, url in state.shapefile_urls().items():
+        for url in state.shapefile_urls().values():
             resp = requests.head(url)
             assert resp.status_code == 200
 
 
 # counts
 
 
@@ -143,14 +146,14 @@
 
 
 def test_territories():
     assert len(us.TERRITORIES) == 5
 
 
 def test_contiguous():
-    # Lower 48 + DC
+    # Lower 48
     assert len(us.STATES_CONTIGUOUS) == 48
 
 
 def test_continental():
-    # Lower 48 + DC + Alaska
+    # Lower 48 + Alaska
     assert len(us.STATES_CONTINENTAL) == 49
```

