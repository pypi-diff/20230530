# Comparing `tmp/alacorder-80.8.5.tar.gz` & `tmp/alacorder-80.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.8.5.tar", max compression
+gzip compressed data, was "alacorder-80.8.6.tar", max compression
```

## Comparing `alacorder-80.8.5.tar` & `alacorder-80.8.6.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.5/LICENSE
--rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.5/README.md
--rw-r--r--   0        0        0      746 2023-05-29 15:57:01.593196 alacorder-80.8.5/pyproject.toml
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.5/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.5/src/alacorder/__init__.py
--rw-r--r--   0        0        0   281427 2023-05-29 15:56:03.618301 alacorder-80.8.5/src/alacorder/__main__.py
--rw-r--r--   0        0        0   281427 2023-05-29 15:55:57.780550 alacorder-80.8.5/src/alacorder/alac.py
--rw-r--r--   0        0        0     8286 1970-01-01 00:00:00.000000 alacorder-80.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.6/LICENSE
+-rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.6/README.md
+-rw-r--r--   0        0        0      697 2023-05-30 15:50:27.085894 alacorder-80.8.6/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-29 16:04:40.384447 alacorder-80.8.6/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.6/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.6/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   281467 2023-05-30 15:53:52.895017 alacorder-80.8.6/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   281467 2023-05-30 15:53:43.101038 alacorder-80.8.6/src/alacorder/alac.py
+-rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 alacorder-80.8.6/PKG-INFO
```

### Comparing `alacorder-80.8.5/LICENSE` & `alacorder-80.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.5/README.md` & `alacorder-80.8.6/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.5/pyproject.toml` & `alacorder-80.8.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.8.5"
+version = "80.8.6"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-polars = "^0.17.6"
+polars = "^0.18.0"
 XlsxWriter = "^3.0.9"
 click = "^8.1.3"
 tqdm = "^4.65.0"
 xlsx2csv = "^0.8.1"
 PySimpleGUI = "^4.60.4"
 selenium = "^4.8.3"
 PyMuPDF = "^1.21.1"
 brotli = "^1.0.9"
-pyarrow = {version = "^12.0.0", optional = true}
 
 [[tool.poetry.source]]
 name = "alacorder"
 url = "https://pypi.org/project/alacorder"
 default = false
 secondary = false
```

### Comparing `alacorder-80.8.5/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.8.6/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.5/src/alacorder/__main__.py` & `alacorder-80.8.6/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 ╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
 ╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
 ╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
 (c) 2023 Sam Robson ----------
 
 Dependencies: 
     python 3.9+, brotli ^1.0.9, click ^8.1.3,
-    polars ^0.17.6, PyMuPDF ^1.21.1,
+    polars ^0.18.0, PyMuPDF ^1.21.1,
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.5"
+version = "80.8.6"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1236,18 +1236,18 @@
     names = (
         names.groupby("Name")
         .agg("CaseNumber", "Alias", "DOB")
         .select(
             [
                 pl.lit("").alias("AIS / Unique ID"),
                 pl.col("Name"),
-                pl.col("Alias").arr.get(0),
-                pl.col("DOB").arr.get(0),
-                pl.col("CaseNumber").arr.lengths().alias("CaseCount"),
-                pl.col("CaseNumber").arr.join(", ").alias("Cases"),
+                pl.col("Alias").list.get(0),
+                pl.col("DOB").list.get(0),
+                pl.col("CaseNumber").list.lengths().alias("CaseCount"),
+                pl.col("CaseNumber").list.join(", ").alias("Cases"),
             ]
         )
     )
     names = names.sort("Name")
     names = names.filter(pl.col("Name") != "")
     return names
 
@@ -1267,22 +1267,22 @@
     )
     fch = charges.filter(pl.col("Filing"))
     fch = fch.join(pairs, on="Name", how="outer")
     fch = fch.groupby("AIS / Unique ID").all()
     fch = fch.select(
         [
             pl.col("AIS / Unique ID"),
-            pl.col("CERVDisqCharge").arr.count_match(True).alias("CERVChargesCount"),
+            pl.col("CERVDisqCharge").list.count_match(True).alias("CERVChargesCount"),
             pl.col("PardonDisqCharge")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("PardonToVoteChargesCount"),
             pl.col("PermanentDisqCharge")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("PermanentDisqChargesCount"),
-            pl.col("ChargesSummary").arr.join(", ")
+            pl.col("ChargesSummary").list.join(", ")
             .str.replace_all(r"null,?", "")
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
             .alias("FilingCharges"),
 
         ]
@@ -1290,27 +1290,27 @@
     conv = charges.filter(pl.col("Disposition") & pl.col("Conviction"))
     conv = conv.join(pairs, on="Name", how="outer")
     conv = conv.groupby("AIS / Unique ID").all()
     conv = conv.select(
         [
             pl.col("AIS / Unique ID"),
             pl.col("Conviction")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("ConvictionCount"),
             pl.col("CERVDisqConviction")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("CERVConvictionCount"),
             pl.col("PardonDisqConviction")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("PardonToVoteConvictionCount"),
             pl.col("PermanentDisqConviction")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("PermanentDisqConvictionCount"),
-            pl.col("PaymentToRestore").arr.mean(),
-            pl.col("ChargesSummary").arr.join(", ")
+            pl.col("PaymentToRestore").list.mean(),
+            pl.col("ChargesSummary").list.join(", ")
             .str.replace_all(r"null,?", "")
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
             .alias("Convictions"),
         ]
     )
@@ -1320,30 +1320,30 @@
         | pl.col("PermanentDisqConviction")
     )
     vrr = vrr.join(pairs, on="Name", how="outer")
     vrr = vrr.groupby("AIS / Unique ID").all()
     vrr = vrr.select(
         [
             pl.col("AIS / Unique ID"),
-            pl.col("ChargesSummary").arr.join(", ")
+            pl.col("ChargesSummary").list.join(", ")
             .str.replace_all(r"null,?", "")
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
             .alias("DisqualifyingConvictions")
         ]
     )
     cases = cases.join(pairs, on="Name", how="outer")
     cases = cases.groupby("AIS / Unique ID").all()
     cases = cases.join(vrr, on="AIS / Unique ID", how="outer")
     cases = cases.join(conv, on="AIS / Unique ID", how="outer")
     cases = cases.join(fch, on="AIS / Unique ID", how="outer")
     cases = cases.with_columns(
         [
-            pl.col("CaseNumber").arr.join(", ")            
+            pl.col("CaseNumber").list.join(", ")            
             .str.replace_all(r"null,?", "")
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
             .alias("Cases")
         ]
     )
@@ -1378,18 +1378,18 @@
             .then(None).otherwise(pl.col("PermanentlyDisqualified"))
             .alias("PermanentlyDisqualified"),
         ]
     )
     cases = cases.select(
         [
             pl.col("AIS / Unique ID"),
-            pl.col("Name").arr.first(),
-            pl.col("DOB").arr.first(),
-            pl.col("Race").arr.first(),
-            pl.col("Sex").arr.first(),
+            pl.col("Name").list.first(),
+            pl.col("DOB").list.first(),
+            pl.col("Race").list.first(),
+            pl.col("Sex").list.first(),
             pl.col("PaymentToRestore"),
             pl.col("EligibleToVote"),
             pl.col("NeedsCERV"),
             pl.col("NeedsPardon"),
             pl.col("PermanentlyDisqualified"),
             pl.col("ConvictionCount"),
             pl.col("CERVChargesCount"),
@@ -1453,22 +1453,22 @@
                 r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
             )
             .alias("RE_Charges"),
             pl.col("AllPagesText")
             .str.extract(r"(Total:.+\$[^\n]*)")
             .str.replace_all(r"[^0-9|\.|\s|\$]", "")
             .str.extract_all(r"\s\$\d+\.\d{2}")
-            .arr.get(2)
+            .list.get(2)
             .str.replace_all(r"[^0-9\.]", "")
             .cast(pl.Float64, strict=False)
             .alias("RAWTotalBalance"),
             pl.col("AllPagesText")
             .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
             .str.extract_all(r"\$\d+\.\d{2}")
-            .arr.get(-1)
+            .list.get(-1)
             .str.replace(r"[\$\s]", "")
             .cast(pl.Float64, strict=False)
             .alias("RAWD999"),
         ]
     )
 
     all_charges = all_charges.explode("RE_Charges").select(
@@ -1601,21 +1601,21 @@
             .str.extract(r"(Total:.+\$[^\n]*)")
             .str.replace_all(r"[^0-9|\.|\s|\$]", "")
             .str.extract_all(r"\s\$\d+\.\d{2}")
             .alias("TOTALS"),
             pl.col("AllPagesText")
             .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
             .str.extract_all(r"\$\d+\.\d{2}")
-            .arr.get(-1)
+            .list.get(-1)
             .str.replace(r"[\$\s]", "")
             .cast(pl.Float64, strict=False)
             .alias("D999RAW"),
             pl.col("AllPagesText")
             .str.extract_all(r"(\w{2}\d{12})")
-            .arr.join("/")
+            .list.join("/")
             .alias("RelatedCases"),
             pl.col("AllPagesText")
             .str.extract(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.to_date("%m/%d/%Y", strict=False)
             .alias("FilingDate"),
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)")
@@ -2026,30 +2026,30 @@
         .otherwise(pl.col("DLRAW"))
         .alias("DriverLicenseNo"),
         pl.when(pl.col("SIDRAW") == "AL000000000")
         .then(pl.lit(""))
         .otherwise(pl.col("SIDRAW"))
         .alias("StateID"),
         pl.col("TOTALS")
-        .arr.get(0)
+        .list.get(0)
         .str.replace_all(r"[^0-9\.]", "")
         .cast(pl.Float64, strict=False)
         .alias("TotalAmtDue"),
         pl.col("TOTALS")
-        .arr.get(1)
+        .list.get(1)
         .str.replace_all(r"[^0-9\.]", "")
         .cast(pl.Float64, strict=False)
         .alias("TotalAmtPaid"),
         pl.col("TOTALS")
-        .arr.get(2)
+        .list.get(2)
         .str.replace_all(r"[^0-9\.]", "")
         .cast(pl.Float64, strict=False)
         .alias("TotalBalance"),
         pl.col("TOTALS")
-        .arr.get(3)
+        .list.get(3)
         .str.replace_all(r"[^0-9\.]", "")
         .cast(pl.Float64, strict=False)
         .alias("TotalAmtHold"),
     )
     cases = cases.with_columns(
         pl.when(pl.col("CLEAN_Phone").str.n_chars() < 7)
         .then(None)
@@ -2269,23 +2269,23 @@
             pl.col("Charges").str.contains("GUILTY PLEA").alias("GUILTY_PLEA"),
             pl.col("Charges").str.contains("CONVICTED").alias("CONVICTED"),
         ]
     )
     charges = charges.with_columns(
         [
             pl.when(pl.col("Disposition"))
-            .then(pl.col("Split").arr.get(1))
-            .otherwise(pl.col("Split").arr.get(0).str.slice(9))
+            .then(pl.col("Split").list.get(1))
+            .otherwise(pl.col("Split").list.get(0).str.slice(9))
             .str.replace(r"-   -", "", literal=True)
             .str.replace("1STS", "1ST", literal=True)
             .str.strip()
             .alias("RAWDESC"),
             pl.when(pl.col("Disposition"))
-            .then(pl.col("Split").arr.get(0).str.slice(19))
-            .otherwise(pl.col("Split").arr.get(1))
+            .then(pl.col("Split").list.get(0).str.slice(19))
+            .otherwise(pl.col("Split").list.get(1))
             .str.strip()
             .alias("SEG_2"),
             pl.when(pl.col("Disposition") == True)
             .then(False)
             .otherwise(True)
             .alias("Filing"),
         ]
@@ -2550,22 +2550,22 @@
             .alias("FEE_SEP"),
         ]
     )
     dlog(df.columns, df.shape, cf=debug)
     df = df.with_columns(
         [
             pl.col("CaseNumber"),
-            pl.col("SPACE_SEP").arr.get(0).alias("FeeStatus1"),
-            pl.col("FEE_SEP").arr.get(0).str.replace(r"\$", "").alias("AmtDue"),  # good
+            pl.col("SPACE_SEP").list.get(0).alias("FeeStatus1"),
+            pl.col("FEE_SEP").list.get(0).str.replace(r"\$", "").alias("AmtDue"),  # good
             pl.col("FEE_SEP")
-            .arr.get(1)
+            .list.get(1)
             .str.replace(r"\$", "")
             .alias("AmtPaid"),  # good
-            pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", "").alias("Balance1"),
-            pl.col("SPACE_SEP").arr.get(5).alias("FeeCode"),
+            pl.col("FEE_SEP").list.get(2).str.replace(r"\$", "").alias("Balance1"),
+            pl.col("SPACE_SEP").list.get(5).alias("FeeCode"),
             pl.col("Fees").str.extract(r"(\w00\d)").alias("Payor"),
             pl.col("Fees").str.extract(r"\s(\d\d\d)\s").alias("Payee"),
         ]
     )
     out = df.with_columns(
         [
             pl.col("CaseNumber"),
@@ -2578,19 +2578,19 @@
             .otherwise(pl.col("Balance1").str.replace_all(r"[A-Z]|\$", ""))
             .alias("AmtHold2"),
         ]
     )
     out = out.with_columns(
         pl.col("Fees").str.extract(r'\s(Y|N)\s').alias("AdminFee"),
         pl.when(pl.col("TOT") == True)
-        .then(pl.col("FEE_SEP").arr.get(-1).str.replace(r"\$", ""))
-        .otherwise(pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", ""))
+        .then(pl.col("FEE_SEP").list.get(-1).str.replace(r"\$", ""))
+        .otherwise(pl.col("FEE_SEP").list.get(2).str.replace(r"\$", ""))
         .alias("AmtHold"),
         pl.when(pl.col("TOT") == False)
-        .then(pl.col("SPACE_SEP").arr.get(0))
+        .then(pl.col("SPACE_SEP").list.get(0))
         .otherwise(pl.lit(""))
         .alias("FeeStatus"),
         pl.when(pl.col("TOT") == True)
         .then(pl.lit("Total:"))
         .otherwise(pl.lit(""))
         .alias("Total"),
     )
```

### Comparing `alacorder-80.8.5/src/alacorder/alac.py` & `alacorder-80.8.6/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 ╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
 ╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
 ╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
 (c) 2023 Sam Robson ----------
 
 Dependencies: 
     python 3.9+, brotli ^1.0.9, click ^8.1.3,
-    polars ^0.17.6, PyMuPDF ^1.21.1,
+    polars ^0.18.0, PyMuPDF ^1.21.1,
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.5"
+version = "80.8.6"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1236,18 +1236,18 @@
     names = (
         names.groupby("Name")
         .agg("CaseNumber", "Alias", "DOB")
         .select(
             [
                 pl.lit("").alias("AIS / Unique ID"),
                 pl.col("Name"),
-                pl.col("Alias").arr.get(0),
-                pl.col("DOB").arr.get(0),
-                pl.col("CaseNumber").arr.lengths().alias("CaseCount"),
-                pl.col("CaseNumber").arr.join(", ").alias("Cases"),
+                pl.col("Alias").list.get(0),
+                pl.col("DOB").list.get(0),
+                pl.col("CaseNumber").list.lengths().alias("CaseCount"),
+                pl.col("CaseNumber").list.join(", ").alias("Cases"),
             ]
         )
     )
     names = names.sort("Name")
     names = names.filter(pl.col("Name") != "")
     return names
 
@@ -1267,22 +1267,22 @@
     )
     fch = charges.filter(pl.col("Filing"))
     fch = fch.join(pairs, on="Name", how="outer")
     fch = fch.groupby("AIS / Unique ID").all()
     fch = fch.select(
         [
             pl.col("AIS / Unique ID"),
-            pl.col("CERVDisqCharge").arr.count_match(True).alias("CERVChargesCount"),
+            pl.col("CERVDisqCharge").list.count_match(True).alias("CERVChargesCount"),
             pl.col("PardonDisqCharge")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("PardonToVoteChargesCount"),
             pl.col("PermanentDisqCharge")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("PermanentDisqChargesCount"),
-            pl.col("ChargesSummary").arr.join(", ")
+            pl.col("ChargesSummary").list.join(", ")
             .str.replace_all(r"null,?", "")
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
             .alias("FilingCharges"),
 
         ]
@@ -1290,27 +1290,27 @@
     conv = charges.filter(pl.col("Disposition") & pl.col("Conviction"))
     conv = conv.join(pairs, on="Name", how="outer")
     conv = conv.groupby("AIS / Unique ID").all()
     conv = conv.select(
         [
             pl.col("AIS / Unique ID"),
             pl.col("Conviction")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("ConvictionCount"),
             pl.col("CERVDisqConviction")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("CERVConvictionCount"),
             pl.col("PardonDisqConviction")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("PardonToVoteConvictionCount"),
             pl.col("PermanentDisqConviction")
-            .arr.count_match(True)
+            .list.count_match(True)
             .alias("PermanentDisqConvictionCount"),
-            pl.col("PaymentToRestore").arr.mean(),
-            pl.col("ChargesSummary").arr.join(", ")
+            pl.col("PaymentToRestore").list.mean(),
+            pl.col("ChargesSummary").list.join(", ")
             .str.replace_all(r"null,?", "")
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
             .alias("Convictions"),
         ]
     )
@@ -1320,30 +1320,30 @@
         | pl.col("PermanentDisqConviction")
     )
     vrr = vrr.join(pairs, on="Name", how="outer")
     vrr = vrr.groupby("AIS / Unique ID").all()
     vrr = vrr.select(
         [
             pl.col("AIS / Unique ID"),
-            pl.col("ChargesSummary").arr.join(", ")
+            pl.col("ChargesSummary").list.join(", ")
             .str.replace_all(r"null,?", "")
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
             .alias("DisqualifyingConvictions")
         ]
     )
     cases = cases.join(pairs, on="Name", how="outer")
     cases = cases.groupby("AIS / Unique ID").all()
     cases = cases.join(vrr, on="AIS / Unique ID", how="outer")
     cases = cases.join(conv, on="AIS / Unique ID", how="outer")
     cases = cases.join(fch, on="AIS / Unique ID", how="outer")
     cases = cases.with_columns(
         [
-            pl.col("CaseNumber").arr.join(", ")            
+            pl.col("CaseNumber").list.join(", ")            
             .str.replace_all(r"null,?", "")
             .str.strip()
             .str.replace(r",$", "")
             .str.replace_all(r"\s+", " ")
             .alias("Cases")
         ]
     )
@@ -1378,18 +1378,18 @@
             .then(None).otherwise(pl.col("PermanentlyDisqualified"))
             .alias("PermanentlyDisqualified"),
         ]
     )
     cases = cases.select(
         [
             pl.col("AIS / Unique ID"),
-            pl.col("Name").arr.first(),
-            pl.col("DOB").arr.first(),
-            pl.col("Race").arr.first(),
-            pl.col("Sex").arr.first(),
+            pl.col("Name").list.first(),
+            pl.col("DOB").list.first(),
+            pl.col("Race").list.first(),
+            pl.col("Sex").list.first(),
             pl.col("PaymentToRestore"),
             pl.col("EligibleToVote"),
             pl.col("NeedsCERV"),
             pl.col("NeedsPardon"),
             pl.col("PermanentlyDisqualified"),
             pl.col("ConvictionCount"),
             pl.col("CERVChargesCount"),
@@ -1453,22 +1453,22 @@
                 r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
             )
             .alias("RE_Charges"),
             pl.col("AllPagesText")
             .str.extract(r"(Total:.+\$[^\n]*)")
             .str.replace_all(r"[^0-9|\.|\s|\$]", "")
             .str.extract_all(r"\s\$\d+\.\d{2}")
-            .arr.get(2)
+            .list.get(2)
             .str.replace_all(r"[^0-9\.]", "")
             .cast(pl.Float64, strict=False)
             .alias("RAWTotalBalance"),
             pl.col("AllPagesText")
             .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
             .str.extract_all(r"\$\d+\.\d{2}")
-            .arr.get(-1)
+            .list.get(-1)
             .str.replace(r"[\$\s]", "")
             .cast(pl.Float64, strict=False)
             .alias("RAWD999"),
         ]
     )
 
     all_charges = all_charges.explode("RE_Charges").select(
@@ -1601,21 +1601,21 @@
             .str.extract(r"(Total:.+\$[^\n]*)")
             .str.replace_all(r"[^0-9|\.|\s|\$]", "")
             .str.extract_all(r"\s\$\d+\.\d{2}")
             .alias("TOTALS"),
             pl.col("AllPagesText")
             .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
             .str.extract_all(r"\$\d+\.\d{2}")
-            .arr.get(-1)
+            .list.get(-1)
             .str.replace(r"[\$\s]", "")
             .cast(pl.Float64, strict=False)
             .alias("D999RAW"),
             pl.col("AllPagesText")
             .str.extract_all(r"(\w{2}\d{12})")
-            .arr.join("/")
+            .list.join("/")
             .alias("RelatedCases"),
             pl.col("AllPagesText")
             .str.extract(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.to_date("%m/%d/%Y", strict=False)
             .alias("FilingDate"),
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)")
@@ -2026,30 +2026,30 @@
         .otherwise(pl.col("DLRAW"))
         .alias("DriverLicenseNo"),
         pl.when(pl.col("SIDRAW") == "AL000000000")
         .then(pl.lit(""))
         .otherwise(pl.col("SIDRAW"))
         .alias("StateID"),
         pl.col("TOTALS")
-        .arr.get(0)
+        .list.get(0)
         .str.replace_all(r"[^0-9\.]", "")
         .cast(pl.Float64, strict=False)
         .alias("TotalAmtDue"),
         pl.col("TOTALS")
-        .arr.get(1)
+        .list.get(1)
         .str.replace_all(r"[^0-9\.]", "")
         .cast(pl.Float64, strict=False)
         .alias("TotalAmtPaid"),
         pl.col("TOTALS")
-        .arr.get(2)
+        .list.get(2)
         .str.replace_all(r"[^0-9\.]", "")
         .cast(pl.Float64, strict=False)
         .alias("TotalBalance"),
         pl.col("TOTALS")
-        .arr.get(3)
+        .list.get(3)
         .str.replace_all(r"[^0-9\.]", "")
         .cast(pl.Float64, strict=False)
         .alias("TotalAmtHold"),
     )
     cases = cases.with_columns(
         pl.when(pl.col("CLEAN_Phone").str.n_chars() < 7)
         .then(None)
@@ -2269,23 +2269,23 @@
             pl.col("Charges").str.contains("GUILTY PLEA").alias("GUILTY_PLEA"),
             pl.col("Charges").str.contains("CONVICTED").alias("CONVICTED"),
         ]
     )
     charges = charges.with_columns(
         [
             pl.when(pl.col("Disposition"))
-            .then(pl.col("Split").arr.get(1))
-            .otherwise(pl.col("Split").arr.get(0).str.slice(9))
+            .then(pl.col("Split").list.get(1))
+            .otherwise(pl.col("Split").list.get(0).str.slice(9))
             .str.replace(r"-   -", "", literal=True)
             .str.replace("1STS", "1ST", literal=True)
             .str.strip()
             .alias("RAWDESC"),
             pl.when(pl.col("Disposition"))
-            .then(pl.col("Split").arr.get(0).str.slice(19))
-            .otherwise(pl.col("Split").arr.get(1))
+            .then(pl.col("Split").list.get(0).str.slice(19))
+            .otherwise(pl.col("Split").list.get(1))
             .str.strip()
             .alias("SEG_2"),
             pl.when(pl.col("Disposition") == True)
             .then(False)
             .otherwise(True)
             .alias("Filing"),
         ]
@@ -2550,22 +2550,22 @@
             .alias("FEE_SEP"),
         ]
     )
     dlog(df.columns, df.shape, cf=debug)
     df = df.with_columns(
         [
             pl.col("CaseNumber"),
-            pl.col("SPACE_SEP").arr.get(0).alias("FeeStatus1"),
-            pl.col("FEE_SEP").arr.get(0).str.replace(r"\$", "").alias("AmtDue"),  # good
+            pl.col("SPACE_SEP").list.get(0).alias("FeeStatus1"),
+            pl.col("FEE_SEP").list.get(0).str.replace(r"\$", "").alias("AmtDue"),  # good
             pl.col("FEE_SEP")
-            .arr.get(1)
+            .list.get(1)
             .str.replace(r"\$", "")
             .alias("AmtPaid"),  # good
-            pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", "").alias("Balance1"),
-            pl.col("SPACE_SEP").arr.get(5).alias("FeeCode"),
+            pl.col("FEE_SEP").list.get(2).str.replace(r"\$", "").alias("Balance1"),
+            pl.col("SPACE_SEP").list.get(5).alias("FeeCode"),
             pl.col("Fees").str.extract(r"(\w00\d)").alias("Payor"),
             pl.col("Fees").str.extract(r"\s(\d\d\d)\s").alias("Payee"),
         ]
     )
     out = df.with_columns(
         [
             pl.col("CaseNumber"),
@@ -2578,19 +2578,19 @@
             .otherwise(pl.col("Balance1").str.replace_all(r"[A-Z]|\$", ""))
             .alias("AmtHold2"),
         ]
     )
     out = out.with_columns(
         pl.col("Fees").str.extract(r'\s(Y|N)\s').alias("AdminFee"),
         pl.when(pl.col("TOT") == True)
-        .then(pl.col("FEE_SEP").arr.get(-1).str.replace(r"\$", ""))
-        .otherwise(pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", ""))
+        .then(pl.col("FEE_SEP").list.get(-1).str.replace(r"\$", ""))
+        .otherwise(pl.col("FEE_SEP").list.get(2).str.replace(r"\$", ""))
         .alias("AmtHold"),
         pl.when(pl.col("TOT") == False)
-        .then(pl.col("SPACE_SEP").arr.get(0))
+        .then(pl.col("SPACE_SEP").list.get(0))
         .otherwise(pl.lit(""))
         .alias("FeeStatus"),
         pl.when(pl.col("TOT") == True)
         .then(pl.lit("Total:"))
         .otherwise(pl.lit(""))
         .alias("Total"),
     )
```

### Comparing `alacorder-80.8.5/PKG-INFO` & `alacorder-80.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.8.5
+Version: 80.8.6
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,16 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyMuPDF (>=1.21.1,<2.0.0)
 Requires-Dist: PySimpleGUI (>=4.60.4,<5.0.0)
 Requires-Dist: XlsxWriter (>=3.0.9,<4.0.0)
 Requires-Dist: brotli (>=1.0.9,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: polars (>=0.17.6,<0.18.0)
-Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
+Requires-Dist: polars (>=0.18.0,<0.19.0)
 Requires-Dist: selenium (>=4.8.3,<5.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: xlsx2csv (>=0.8.1,<0.9.0)
 Description-Content-Type: text/markdown
 
 ```
     ___    __                          __
```

