# Comparing `tmp/life-model-0.1.2.tar.gz` & `tmp/life-model-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "life-model-0.1.2.tar", last modified: Sun Oct 30 06:26:02 2022, max compression
+gzip compressed data, was "life-model-0.1.3.tar", last modified: Tue May 30 06:38:42 2023, max compression
```

## Comparing `life-model-0.1.2.tar` & `life-model-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2022-10-30 06:26:02.167184 life-model-0.1.2/
--rw-r--r--   0 spencer    (501) staff       (20)      896 2022-10-14 05:03:19.000000 life-model-0.1.2/INSTALL.rst
--rw-r--r--   0 spencer    (501) staff       (20)     1073 2022-02-06 12:42:06.000000 life-model-0.1.2/LICENSE
--rw-r--r--   0 spencer    (501) staff       (20)       95 2022-10-30 06:18:28.000000 life-model-0.1.2/MANIFEST.in
--rw-r--r--   0 spencer    (501) staff       (20)     1106 2022-10-30 06:26:02.164098 life-model-0.1.2/PKG-INFO
--rw-r--r--   0 spencer    (501) staff       (20)       49 2022-02-06 13:20:46.000000 life-model-0.1.2/README.rst
--rw-r--r--   0 spencer    (501) staff       (20)        5 2022-10-30 06:25:40.000000 life-model-0.1.2/VERSION
--rw-r--r--   0 spencer    (501) staff       (20)       31 2022-10-16 02:48:44.000000 life-model-0.1.2/requirements.txt
--rw-r--r--   0 spencer    (501) staff       (20)       38 2022-10-30 06:26:02.167634 life-model-0.1.2/setup.cfg
--rw-r--r--   0 spencer    (501) staff       (20)     2158 2022-10-30 06:18:55.000000 life-model-0.1.2/setup.py
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2022-10-30 06:26:02.108727 life-model-0.1.2/src/
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2022-10-30 06:26:02.133944 life-model-0.1.2/src/life_model/
--rw-r--r--   0 spencer    (501) staff       (20)        0 2022-02-06 14:16:49.000000 life-model-0.1.2/src/life_model/__init__.py
--rw-r--r--   0 spencer    (501) staff       (20)     1067 2022-10-14 05:03:19.000000 life-model-0.1.2/src/life_model/__main__.py
--rw-r--r--   0 spencer    (501) staff       (20)       99 2022-10-30 06:26:01.000000 life-model-0.1.2/src/life_model/__meta__.py
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2022-10-30 06:26:02.150599 life-model-0.1.2/src/life_model/account/
--rw-r--r--   0 spencer    (501) staff       (20)        0 2022-02-06 13:16:54.000000 life-model-0.1.2/src/life_model/account/__init__.py
--rw-r--r--   0 spencer    (501) staff       (20)     1857 2022-10-14 05:19:34.000000 life-model-0.1.2/src/life_model/account/bank.py
--rw-r--r--   0 spencer    (501) staff       (20)     4200 2022-10-14 05:27:26.000000 life-model-0.1.2/src/life_model/account/job401k.py
--rw-r--r--   0 spencer    (501) staff       (20)     4818 2022-10-16 01:46:40.000000 life-model-0.1.2/src/life_model/basemodel.py
--rw-r--r--   0 spencer    (501) staff       (20)     4158 2022-10-15 20:35:27.000000 life-model-0.1.2/src/life_model/family.py
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2022-10-30 06:26:02.160379 life-model-0.1.2/src/life_model/housing/
--rw-r--r--   0 spencer    (501) staff       (20)        0 2022-10-30 06:00:01.000000 life-model-0.1.2/src/life_model/housing/__init__.py
--rw-r--r--   0 spencer    (501) staff       (20)     1004 2022-10-14 05:29:57.000000 life-model-0.1.2/src/life_model/housing/apartment.py
--rw-r--r--   0 spencer    (501) staff       (20)     6378 2022-10-14 05:40:48.000000 life-model-0.1.2/src/life_model/housing/home.py
--rw-r--r--   0 spencer    (501) staff       (20)     3611 2022-10-15 20:33:26.000000 life-model-0.1.2/src/life_model/job.py
--rw-r--r--   0 spencer    (501) staff       (20)     1581 2022-10-15 20:58:10.000000 life-model-0.1.2/src/life_model/lifeevents.py
--rw-r--r--   0 spencer    (501) staff       (20)     1377 2022-02-12 21:05:17.000000 life-model-0.1.2/src/life_model/limits.py
--rw-r--r--   0 spencer    (501) staff       (20)     8342 2022-10-16 02:14:32.000000 life-model-0.1.2/src/life_model/person.py
--rw-r--r--   0 spencer    (501) staff       (20)     2759 2022-10-16 01:36:41.000000 life-model-0.1.2/src/life_model/simulation.py
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2022-10-30 06:26:02.163188 life-model-0.1.2/src/life_model/tax/
--rw-r--r--   0 spencer    (501) staff       (20)        0 2022-02-06 13:41:30.000000 life-model-0.1.2/src/life_model/tax/__init__.py
--rw-r--r--   0 spencer    (501) staff       (20)     1552 2022-10-15 20:17:41.000000 life-model-0.1.2/src/life_model/tax/federal.py
-drwxr-xr-x   0 spencer    (501) staff       (20)        0 2022-10-30 06:26:02.146479 life-model-0.1.2/src/life_model.egg-info/
--rw-r--r--   0 spencer    (501) staff       (20)     1106 2022-10-30 06:26:02.000000 life-model-0.1.2/src/life_model.egg-info/PKG-INFO
--rw-r--r--   0 spencer    (501) staff       (20)      829 2022-10-30 06:26:02.000000 life-model-0.1.2/src/life_model.egg-info/SOURCES.txt
--rw-r--r--   0 spencer    (501) staff       (20)        1 2022-10-30 06:26:02.000000 life-model-0.1.2/src/life_model.egg-info/dependency_links.txt
--rw-r--r--   0 spencer    (501) staff       (20)        1 2022-10-30 06:26:02.000000 life-model-0.1.2/src/life_model.egg-info/not-zip-safe
--rw-r--r--   0 spencer    (501) staff       (20)       18 2022-10-30 06:26:02.000000 life-model-0.1.2/src/life_model.egg-info/requires.txt
--rw-r--r--   0 spencer    (501) staff       (20)       11 2022-10-30 06:26:02.000000 life-model-0.1.2/src/life_model.egg-info/top_level.txt
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-30 06:38:42.156741 life-model-0.1.3/
+-rw-r--r--   0 spencer    (501) staff       (20)      896 2022-10-14 05:03:19.000000 life-model-0.1.3/INSTALL.rst
+-rw-r--r--   0 spencer    (501) staff       (20)     1073 2022-02-06 12:42:06.000000 life-model-0.1.3/LICENSE
+-rw-r--r--   0 spencer    (501) staff       (20)       95 2022-10-30 06:18:28.000000 life-model-0.1.3/MANIFEST.in
+-rw-r--r--   0 spencer    (501) staff       (20)     1088 2023-05-30 06:38:42.155842 life-model-0.1.3/PKG-INFO
+-rw-r--r--   0 spencer    (501) staff       (20)       49 2022-02-06 13:20:46.000000 life-model-0.1.3/README.rst
+-rw-r--r--   0 spencer    (501) staff       (20)        6 2023-05-30 06:38:36.000000 life-model-0.1.3/VERSION
+-rw-r--r--   0 spencer    (501) staff       (20)       43 2023-05-29 19:31:46.000000 life-model-0.1.3/requirements.txt
+-rw-r--r--   0 spencer    (501) staff       (20)       38 2023-05-30 06:38:42.156961 life-model-0.1.3/setup.cfg
+-rw-r--r--   0 spencer    (501) staff       (20)     2158 2022-10-30 06:18:55.000000 life-model-0.1.3/setup.py
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-30 06:38:41.979434 life-model-0.1.3/src/
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-30 06:38:42.123270 life-model-0.1.3/src/life_model/
+-rw-r--r--   0 spencer    (501) staff       (20)        0 2022-02-06 14:16:49.000000 life-model-0.1.3/src/life_model/__init__.py
+-rw-r--r--   0 spencer    (501) staff       (20)     1217 2022-11-23 18:38:21.000000 life-model-0.1.3/src/life_model/__main__.py
+-rw-r--r--   0 spencer    (501) staff       (20)       99 2023-05-30 06:38:41.000000 life-model-0.1.3/src/life_model/__meta__.py
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-30 06:38:42.143180 life-model-0.1.3/src/life_model/account/
+-rw-r--r--   0 spencer    (501) staff       (20)        0 2022-02-06 13:16:54.000000 life-model-0.1.3/src/life_model/account/__init__.py
+-rw-r--r--   0 spencer    (501) staff       (20)     2011 2023-04-26 03:05:29.000000 life-model-0.1.3/src/life_model/account/bank.py
+-rw-r--r--   0 spencer    (501) staff       (20)     4656 2023-05-30 01:40:01.000000 life-model-0.1.3/src/life_model/account/job401k.py
+-rw-r--r--   0 spencer    (501) staff       (20)     4752 2023-02-25 21:12:51.000000 life-model-0.1.3/src/life_model/family.py
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-30 06:38:42.151235 life-model-0.1.3/src/life_model/housing/
+-rw-r--r--   0 spencer    (501) staff       (20)        0 2022-10-30 06:00:01.000000 life-model-0.1.3/src/life_model/housing/__init__.py
+-rw-r--r--   0 spencer    (501) staff       (20)     1150 2023-02-25 21:12:51.000000 life-model-0.1.3/src/life_model/housing/apartment.py
+-rw-r--r--   0 spencer    (501) staff       (20)     6903 2023-02-25 21:12:51.000000 life-model-0.1.3/src/life_model/housing/home.py
+-rw-r--r--   0 spencer    (501) staff       (20)     4416 2023-05-30 02:07:23.000000 life-model-0.1.3/src/life_model/job.py
+-rw-r--r--   0 spencer    (501) staff       (20)     1769 2023-02-25 21:12:51.000000 life-model-0.1.3/src/life_model/lifeevents.py
+-rw-r--r--   0 spencer    (501) staff       (20)     1550 2022-12-12 23:54:07.000000 life-model-0.1.3/src/life_model/limits.py
+-rw-r--r--   0 spencer    (501) staff       (20)    11084 2023-05-30 06:11:38.000000 life-model-0.1.3/src/life_model/model.py
+-rw-r--r--   0 spencer    (501) staff       (20)    11265 2023-05-30 03:47:41.000000 life-model-0.1.3/src/life_model/person.py
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-30 06:38:42.154475 life-model-0.1.3/src/life_model/tax/
+-rw-r--r--   0 spencer    (501) staff       (20)        0 2022-02-06 13:41:30.000000 life-model-0.1.3/src/life_model/tax/__init__.py
+-rw-r--r--   0 spencer    (501) staff       (20)     1981 2023-05-30 04:29:40.000000 life-model-0.1.3/src/life_model/tax/federal.py
+drwxr-xr-x   0 spencer    (501) staff       (20)        0 2023-05-30 06:38:42.137284 life-model-0.1.3/src/life_model.egg-info/
+-rw-r--r--   0 spencer    (501) staff       (20)     1088 2023-05-30 06:38:41.000000 life-model-0.1.3/src/life_model.egg-info/PKG-INFO
+-rw-r--r--   0 spencer    (501) staff       (20)      796 2023-05-30 06:38:41.000000 life-model-0.1.3/src/life_model.egg-info/SOURCES.txt
+-rw-r--r--   0 spencer    (501) staff       (20)        1 2023-05-30 06:38:41.000000 life-model-0.1.3/src/life_model.egg-info/dependency_links.txt
+-rw-r--r--   0 spencer    (501) staff       (20)        1 2022-10-30 06:26:02.000000 life-model-0.1.3/src/life_model.egg-info/not-zip-safe
+-rw-r--r--   0 spencer    (501) staff       (20)       18 2023-05-30 06:38:41.000000 life-model-0.1.3/src/life_model.egg-info/requires.txt
+-rw-r--r--   0 spencer    (501) staff       (20)       11 2023-05-30 06:38:41.000000 life-model-0.1.3/src/life_model.egg-info/top_level.txt
```

### Comparing `life-model-0.1.2/INSTALL.rst` & `life-model-0.1.3/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `life-model-0.1.2/LICENSE` & `life-model-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `life-model-0.1.2/PKG-INFO` & `life-model-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: life-model
-Version: 0.1.2
+Version: 0.1.3
 Summary: Modeling life events and how they impact finances
 Home-page: https://github.com/sw23/life-model
 Author: Spencer Williams
 Author-email: sw23@users.noreply.github.com
-License: UNKNOWN
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
@@ -22,8 +21,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Modeling life events and how they impact finances
-
```

### Comparing `life-model-0.1.2/setup.py` & `life-model-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `life-model-0.1.2/src/life_model/__main__.py` & `life-model-0.1.3/src/life_model/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+# Copyright 2022 Spencer Williams
+#
+# Use of this source code is governed by an MIT license:
+# https://github.com/sw23/life-model/blob/main/LICENSE
+
 import argparse
 from datetime import date
-from life_model import __version__, Family, Person
+
+from life_model import Family, Person, __version__
 
 
 def get_parser():
     """
     Creates a new argument parser.
     """
     parser = argparse.ArgumentParser('life-model')
```

### Comparing `life-model-0.1.2/src/life_model/account/bank.py` & `life-model-0.1.3/src/life_model/account/bank.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-from ..basemodel import BaseModel, compound_interest
+# Copyright 2022 Spencer Williams
+#
+# Use of this source code is governed by an MIT license:
+# https://github.com/sw23/life-model/blob/main/LICENSE
 
+from ..model import LifeModelAgent, compound_interest
+from ..person import Person
 
-class BankAccount(BaseModel):
-    def __init__(self, owner, company, type='Bank', balance=0, interest_rate=0):
+
+class BankAccount(LifeModelAgent):
+    def __init__(self, owner: Person, company: str, type: str = 'Bank', balance: int = 0, interest_rate: float = 0):
         """Class modeling bank accounds
 
         Args:
             owner (Person): Person that owns the Bank Account.
             company (Company): Company at which the bank account belongs.
             type (str, optional): Type of account. Defaults to 'Bank'.
             balance (int, optional): Balance of account. Defaults to 0.
             interest_rate (float, optional): Interest rate. Defaults to 0.
         """
-        self.simulation = owner.simulation
+        super().__init__(owner.model)
         self.owner = owner
         self.company = company
         self.type = type
         self.balance = balance
         self.interest_rate = interest_rate
         self.compound_rate = 12  # Monthly - TODO - make configurable
 
@@ -25,16 +31,15 @@
         self.stat_useable_balance = 0
 
         owner.bank_accounts.append(self)
 
     def _repr_html_(self):
         return f"{self.type} account at {self.company} balance: ${self.balance:,}"
 
-    def advance_year(self, objects=None):
-        super().advance_year(objects)
+    def step(self):
         interest = compound_interest(self.balance, self.interest_rate, self.compound_rate)
         self.balance += interest
 
         self.stat_total_interest += interest
         self.stat_balance_history.append(self.balance)
         self.stat_useable_balance = self.balance
```

### Comparing `life-model-0.1.2/src/life_model/account/job401k.py` & `life-model-0.1.3/src/life_model/account/job401k.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,38 @@
-from ..basemodel import BaseModel, continous_interest
+# Copyright 2022 Spencer Williams
+#
+# Use of this source code is governed by an MIT license:
+# https://github.com/sw23/life-model/blob/main/LICENSE
+
+from typing import Optional, TYPE_CHECKING
+from ..model import LifeModelAgent, continous_interest
 from ..limits import federal_retirement_age, required_min_distrib
 
+if TYPE_CHECKING:
+    from ..job import Job
+
 
-class Job401kAccount(BaseModel):
-    def __init__(self, job,
-                 pretax_balance=0, pretax_contrib_percent=0,
-                 roth_balance=0, roth_contrib_percent=0,
-                 average_growth=0, company_match_percent=0):
+class Job401kAccount(LifeModelAgent):
+    def __init__(self, job: 'Job',
+                 pretax_balance: float = 0, pretax_contrib_percent: float = 0,
+                 roth_balance: float = 0, roth_contrib_percent: float = 0,
+                 average_growth: float = 0, company_match_percent: float = 0):
         """401k Account
 
         Args:
             job (Job): Job offering the 401k plan.
             pretax_balance (float, optional): Initial pre-tax balance of account. Defaults to 0.
             pretax_contrib_percent (float, optional): Pre-tax contribution percentage. Defaults to 0.
             roth_balance (float, optional): Initial roth balance of account. Defaults to 0.
             roth_contrib_percent (float, optional): Roth contribution percentage. Defaults to 0.
             average_growth (float, optional): Average account growth every year. Defaults to 0.
             company_match_percent (float, optional): Percentage that company matches contributions. Defaults to 0.
         """
-        self.simulation = job.simulation
-        self.job = job
+        super().__init__(job.model)
+        self.job: Optional['Job'] = job
         self.owner = job.owner
         self.pretax_balance = pretax_balance
         self.pretax_contrib_percent = pretax_contrib_percent
         self.roth_balance = roth_balance
         self.roth_contrib_percent = roth_contrib_percent
         self.average_growth = average_growth
         self.company_match_percent = company_match_percent
@@ -31,66 +40,68 @@
         self.stat_balance_history = []
         self.stat_useable_balance = 0
         self.stat_required_min_distrib = 0
         self.stat_401k_balance = 0
 
         job.retirement_account = self
 
-    def pretax_contrib(self, salary):
+    def pretax_contrib(self, salary: float):
         return salary * (self.pretax_contrib_percent / 100)
 
-    def roth_contrib(self, salary):
+    def roth_contrib(self, salary: float):
         return salary * (self.roth_contrib_percent / 100)
 
-    def company_match(self, contribution):
+    def company_match(self, contribution: float):
         return contribution * (self.company_match_percent / 100)
 
     @property
     def balance(self):
         return self.pretax_balance + self.roth_balance
 
     def _repr_html_(self):
-        return f"401k at {self.job.company} balance: ${self.balance:,}"
+        company = self.job.company if self.job is not None else "<None>"
+        return f"401k at {company} balance: ${self.balance:,}"
 
-    def advance_year(self, objects=None):
-        super().advance_year(objects)
-        # Note: Contributions are handled by job, after this is called
+    # Using pre_step() so taxable_income will be set before person's step() is called
+    def pre_step(self):
+        # Note: Contributions are handled by job, after this is called.
         # This isn't 100% accurate since contributions aren't included in the
-        # growth, which is a little pessimistic but that should be fine
+        # growth, which is a little pessimistic but that should be fine.
+
         self.pretax_balance += continous_interest(self.pretax_balance, self.average_growth)
         self.roth_balance += continous_interest(self.roth_balance, self.average_growth)
 
         self.stat_balance_history.append(self.balance)
         if (self.owner.age > federal_retirement_age()):
             self.stat_useable_balance = self.balance
 
         # Required minimum distributions
         # - Based on the owner's age, force withdraw the required minium
         required_min_dist_amount = self.deduct_pretax(required_min_distrib(self.owner.age, self.pretax_balance))
-        self.owner.bank_accounts[0].balance += required_min_dist_amount
+        self.owner.deposit_into_bank_account(required_min_dist_amount)
         self.owner.taxable_income += required_min_dist_amount
 
         self.stat_required_min_distrib = required_min_dist_amount
         self.stat_401k_balance = self.balance
 
-    def deduct_pretax(self, amount):
+    def deduct_pretax(self, amount: float):
         """Deduct from pre-tax balance
 
         Args:
             amount (float): Amount to deduct.
 
         Returns:
             float: Amount deducted. Will not be less than the account balance.
         """
         # TODO - Need to figure out where early penalties and limits are applied
         amount_deducted = min(self.pretax_balance, amount)
         self.pretax_balance -= amount_deducted
         return amount_deducted
 
-    def deduct_roth(self, amount):
+    def deduct_roth(self, amount: float) -> float:
         """Deduct from roth balance
 
         Args:
             amount (float): Amount to deduct.
 
         Returns:
             float: Amount deducted. Will not be less than the account balance.
```

### Comparing `life-model-0.1.2/src/life_model/family.py` & `life-model-0.1.3/src/life_model/family.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,93 @@
-from .basemodel import BaseModel
+# Copyright 2022 Spencer Williams
+#
+# Use of this source code is governed by an MIT license:
+# https://github.com/sw23/life-model/blob/main/LICENSE
+
 from .tax.federal import FilingStatus, federal_income_tax, max_tax_rate
+from .model import LifeModelAgent, LifeModel
 
 
-class Family(BaseModel):
-    def __init__(self, simulation, *args):
+class Family(LifeModelAgent):
+    def __init__(self, model: LifeModel, *args):
         """Family
 
         Args:
-            simulation (Simulation): Simulation.
+            model (LifeModel): LifeModel.
             args (Person): Family members.
         """
-        self.simulation = simulation
-        self.simulation.top_level_models.append(self)
+        super().__init__(model)
         self.members = list(args)
 
     @property
-    def bank_account_balance(self):
+    def bank_account_balance(self) -> float:
         return sum(x.bank_account_balance for x in self.members)
 
     @property
-    def debt(self):
+    def debt(self) -> float:
         return sum(x.debt for x in self.members)
 
     @property
-    def filing_status(self):
+    def filing_status(self) -> FilingStatus:
         # TODO - Currently using the first member's filing status for the whole family
         return self.members[0].filing_status
 
     @property
-    def combined_spending(self):
+    def combined_spending(self) -> float:
         return sum(x.spending.base for x in self.members)
 
     @property
-    def combined_taxable_income(self):
+    def combined_taxable_income(self) -> float:
         return sum(x.taxable_income for x in self.members)
 
     def __getitem__(self, key):
         matches = {x.name: x for x in self.members}
         return matches[key]
 
     def _repr_html_(self):
         return '<b>Family:</b><ul>' + ''.join(f"<li>{x._repr_html_()}</li>" for x in self.members) + '</ul>'
 
-    def withdraw_from_pretax_401ks(self, amount):
+    def withdraw_from_pretax_401ks(self, amount: float) -> float:
         for member in self.members:
             if (amount == 0):
                 break
             amount -= member.withdraw_from_pretax_401ks(amount)
         return amount
 
-    def pay_bills(self, spending_balance):
+    def pay_bills(self, spending_balance: float) -> float:
+        """Pay bills for the year.
+
+        Args:
+            spending_balance (float): Amount of spending left to pay.
+
+        Returns:
+            float: Balance remaining after paying bills.
+        """
         for member in self.members:
             if (spending_balance == 0):
                 return 0
             spending_balance = member.pay_bills(spending_balance)
         return spending_balance
 
-    def get_federal_taxes_due(self, additional_income=0):
+    def get_federal_taxes_due(self, additional_income: float = 0) -> float:
+        """Get federal taxes due for the year.
+
+        Args:
+            additional_income (float, optional): Additional income to include in calculation. Defaults to 0.
+
+        Returns:
+            float: Federal taxes due.
+        """
         income_amount = self.combined_taxable_income + additional_income
         if self.filing_status == FilingStatus.MARRIED_FILING_JOINTLY:
             return federal_income_tax(income_amount, self.filing_status)
         else:
             raise NotImplementedError(f"Unsupported filing status: {self.filing_status}")
 
-    def advance_year(self, objects=None):
-        super().advance_year(objects)
+    def step(self):
 
         # Pay off spending, taxes, and debts for the year
         # - People filing MFJ is handled individually here, single is handled in family
         if self.filing_status == FilingStatus.MARRIED_FILING_JOINTLY:
             # 1. See what amount needs to come from pre-tax 401k
             #    - RMDs are handled before this by moving the RMD from 401k to bank account
             # 2. Withdraw that amount plus max tax rate to cover taxes
```

### Comparing `life-model-0.1.2/src/life_model/housing/apartment.py` & `life-model-0.1.3/src/life_model/housing/apartment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-from ..basemodel import BaseModel
+# Copyright 2022 Spencer Williams
+#
+# Use of this source code is governed by an MIT license:
+# https://github.com/sw23/life-model/blob/main/LICENSE
 
+from ..person import Person
+from ..model import LifeModelAgent
 
-class Apartment(BaseModel):
-    def __init__(self, person, name, monthly_rent, yearly_increase=5):
+
+class Apartment(LifeModelAgent):
+    def __init__(self, person: Person, name: str, monthly_rent: float, yearly_increase: float = 5):
         """Apartment
 
         Args:
             person (Person): Primary resident or person paying apartment rent.
             name (string): Apartment Name.
             monthly_rent (float): Amount of rent charged monthly.
             yearly_increase (float, optional): Percentage of rent increase every year. Defaults to 5.
         """
-        self.simulation = person.simulation
+        super().__init__(person.model)
         self.name = name
         self.monthly_rent = monthly_rent
         self.yearly_increase = yearly_increase
         person.apartments.append(self)
 
     @property
     def yearly_rent(self):
         return self.monthly_rent * 12
 
     def _repr_html_(self):
         return f"{self.name}, monthly rent ${self.monthly_rent:,}"
 
-    def advance_year(self, objects=None):
-        super().advance_year(objects)
-
+    def step(self):
         self.monthly_rent += self.monthly_rent * (self.yearly_increase / 100)
```

### Comparing `life-model-0.1.2/src/life_model/housing/home.py` & `life-model-0.1.3/src/life_model/housing/home.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,101 +1,110 @@
-from ..basemodel import BaseModel
+# Copyright 2022 Spencer Williams
+#
+# Use of this source code is governed by an MIT license:
+# https://github.com/sw23/life-model/blob/main/LICENSE
+
+from typing import Optional
+from ..person import Person
+from ..model import LifeModelAgent, LifeModel
 
 
-class Home(BaseModel):
-    def __init__(self, person, name, purchase_price, value_yearly_increase,
-                 down_payment, mortgage, expenses):
+class Home(LifeModelAgent):
+    def __init__(self, person: Person, name: str, purchase_price: float, value_yearly_increase: float,
+                 down_payment: float, mortgage: 'Mortgage', expenses: 'HomeExpenses'):
         """Home
 
         Args:
             person (Person): Primary resident or person that pays the bills.
             name (string): Name of the house or neighborhood.
             purchase_price (float): Purchase price of the home.
             value_yearly_increase (float): Percentage of yearly home value appreciation.
             down_payment (float): Amount of down payment.
             mortgage (Mortgage): Mortgage associated with the home.
             expenses (HomeExpenses): Home expenses associated with the home.
         """
-        self.simulation = person.simulation
+        super().__init__(person.model)
         self.name = name
         self.purchase_price = purchase_price
         self.value_yearly_increase = value_yearly_increase
         self.down_payment = down_payment
         self.mortgage = mortgage
         self.expenses = expenses
         self.expenses.home = self
-        self.home_value = self.purchase_price
+        self.home_value: float = self.purchase_price
         person.homes.append(self)
 
     @property
-    def yearly_expenses_due(self):
+    def yearly_expenses_due(self) -> float:
         return self.expenses.get_yearly_spending() + self.mortgage.get_payment_due_for_year()
 
-    def make_yearly_payment(self, yearly_payment=None, extra_to_principal=0):
+    def make_yearly_payment(self, yearly_payment: Optional[float] = None, extra_to_principal: float = 0):
         if yearly_payment is None:
             yearly_payment = self.yearly_expenses_due
         base_mortgage_payment = yearly_payment - self.expenses.get_yearly_spending()
         self.mortgage.make_yearly_payment(base_mortgage_payment, extra_to_principal)
         return yearly_payment + extra_to_principal
 
     def _repr_html_(self):
         return f"{self.name}, purchase price ${self.purchase_price:,}, " \
                + f"monthly mortgage ${self.mortgage.monthly_payment:,}"
 
-    def advance_year(self, objects=None):
-        super().advance_year(objects)
+    def step(self):
         self.home_value += self.home_value * (self.value_yearly_increase / 100)
 
 
-class HomeExpenses(BaseModel):
-    def __init__(self, property_tax_percent, home_insurance_percent,
-                 maintenance_amount, maintenance_increase,
-                 improvement_amount, improvement_increase,
-                 hoa_amount, hoa_increase):
+class HomeExpenses(LifeModelAgent):
+    def __init__(self, model: LifeModel,
+                 property_tax_percent: float, home_insurance_percent: float,
+                 maintenance_amount: float, maintenance_increase: float,
+                 improvement_amount: float, improvement_increase: float,
+                 hoa_amount: float, hoa_increase: float):
         """Home Expenses
 
         Args:
             property_tax_percent (float): Property tax percentage paid yearly based on home value.
             home_insurance_percent (float): Yearly home insurance cost as percentage of home value.
             maintenance_amount (float): Yearly cost of home maintenance.
             maintenance_increase (float): Yearly percentage increase of maintenance costs.
             improvement_amount (float): Yearly cost of improvements.
             improvement_increase (float): Yearly percentage increase of improvment costs.
             hoa_amount (float): Yearly HOA dues.
             hoa_increase (float): Yearly percentage incresae of HOA dues.
         """
+        super().__init__(model)
         self.property_tax_percent = property_tax_percent
         self.home_insurance_percent = home_insurance_percent
         self.maintenance_amount = maintenance_amount
         self.maintenance_increase = maintenance_increase
         self.improvement_amount = improvement_amount
         self.improvement_increase = improvement_increase
         self.hoa_amount = hoa_amount
         self.hoa_increase = hoa_increase
-        self.home = None
+        self.home: Optional[Home] = None
 
     def get_yearly_spending(self):
-        spending_amount = self.home.home_value * (self.property_tax_percent / 100)
-        spending_amount += self.home.home_value * (self.home_insurance_percent / 100)
+        spending_amount = 0
+        if self.home is not None:
+            spending_amount += self.home.home_value * (self.property_tax_percent / 100)
+            spending_amount += self.home.home_value * (self.home_insurance_percent / 100)
         spending_amount += self.maintenance_amount + self.improvement_amount + self.hoa_amount
         return spending_amount
 
-    def advance_year(self, objects=None):
-        super().advance_year(objects)
+    def step(self):
         self.maintenance_amount += self.maintenance_amount * (self.maintenance_increase / 100)
         self.improvement_amount += self.improvement_amount * (self.improvement_increase / 100)
         self.hoa_amount += self.hoa_amount * (self.hoa_increase / 100)
 
 
 # https://www.nerdwallet.com/mortgages/mortgage-calculator/calculate-mortgage-payment
 # https://www.valuepenguin.com/mortgages/mortgage-payments-calculator
 # https://www.investopedia.com/calculate-principal-and-interest-5211981
 class Mortgage:
-    def __init__(self, loan_amount, start_date, length_years, yearly_interest_rate,
-                 principal=None, monthly_payment=None):
+    def __init__(self, loan_amount: float, start_date: float, length_years: int, yearly_interest_rate: float,
+                 principal: Optional[float] = None, monthly_payment: Optional[float] = None):
         """Mortgage
 
         Args:
             loan_amount (float): Amount of loan.
             start_date (float): Starting year of loan.
             length_years (int): Length of years of loan (e.g. 30, 15)
             yearly_interest_rate (float): Yearly interest rate
@@ -111,28 +120,28 @@
         self.monthly_payment = monthly_payment or self.get_monthly_payment()
         self.yearly_payment = self.monthly_payment * 12
 
         self.stat_principal_payment_history = []
         self.stat_interest_payment_history = []
         self.stat_principal_balance_history = []
 
-    def get_monthly_payment(self):
+    def get_monthly_payment(self) -> float:
         p = self.loan_amount
         i = self.yearly_interest_rate / (100 * 12)
         n = self.length_years * 12
         return p * (i * ((1 + i) ** n)) / (((1 + i) ** n) - 1)
 
-    def get_payment_due_for_year(self):
+    def get_payment_due_for_year(self) -> float:
         return min(self.yearly_payment,
                    self.principal + (self.principal * (self.yearly_interest_rate / 100)))
 
-    def get_interest_for_year(self):
+    def get_interest_for_year(self) -> float:
         return self.principal * (self.yearly_interest_rate / 100)
 
-    def make_yearly_payment(self, yearly_payment, extra_to_principal=0):
+    def make_yearly_payment(self, yearly_payment: float, extra_to_principal: float = 0):
         interest_amount = self.get_interest_for_year()
         principal_amount = (yearly_payment - interest_amount) + extra_to_principal
         self.principal -= principal_amount
 
         self.stat_principal_payment_history.append(principal_amount)
         self.stat_interest_payment_history.append(interest_amount)
         self.stat_principal_balance_history.append(self.principal)
```

### Comparing `life-model-0.1.2/src/life_model/limits.py` & `life-model-0.1.3/src/life_model/limits.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+# Copyright 2022 Spencer Williams
+#
+# Use of this source code is governed by an MIT license:
+# https://github.com/sw23/life-model/blob/main/LICENSE
 
-def job_401k_contrib_limit(age):
+def job_401k_contrib_limit(age) -> int:
     return 20500 + (0 if (age < 50) else 6500)
 
 
-def federal_retirement_age():
+def federal_retirement_age() -> float:
     return 59.5
 
 
 # The table below is taken from the IRS website:
 # https://www.irs.gov/pub/irs-tege/uniform_rmd_wksht.pdf
 # Last accessed: 2/12/22
 rmd_distribution_period = [
@@ -57,14 +61,14 @@
     [112, 2.6],
     [113, 2.4],
     [114, 2.1],
     [115, 1.9],
 ]
 
 
-def required_min_distrib(age, balance):
+def required_min_distrib(age, balance) -> float:
     if age < rmd_distribution_period[0][0]:
         return 0
     elif age > rmd_distribution_period[-1][0]:
         return balance / rmd_distribution_period[-1][1]
     else:
         return balance / [x[1] for x in rmd_distribution_period if x[0] == age][0]
```

### Comparing `life-model-0.1.2/src/life_model.egg-info/PKG-INFO` & `life-model-0.1.3/src/life_model.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: life-model
-Version: 0.1.2
+Version: 0.1.3
 Summary: Modeling life events and how they impact finances
 Home-page: https://github.com/sw23/life-model
 Author: Spencer Williams
 Author-email: sw23@users.noreply.github.com
-License: UNKNOWN
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
@@ -22,8 +21,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Modeling life events and how they impact finances
-
```

### Comparing `life-model-0.1.2/src/life_model.egg-info/SOURCES.txt` & `life-model-0.1.3/src/life_model.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 README.rst
 VERSION
 requirements.txt
 setup.py
 src/life_model/__init__.py
 src/life_model/__main__.py
 src/life_model/__meta__.py
-src/life_model/basemodel.py
 src/life_model/family.py
 src/life_model/job.py
 src/life_model/lifeevents.py
 src/life_model/limits.py
+src/life_model/model.py
 src/life_model/person.py
-src/life_model/simulation.py
 src/life_model.egg-info/PKG-INFO
 src/life_model.egg-info/SOURCES.txt
 src/life_model.egg-info/dependency_links.txt
 src/life_model.egg-info/not-zip-safe
 src/life_model.egg-info/requires.txt
 src/life_model.egg-info/top_level.txt
 src/life_model/account/__init__.py
```

