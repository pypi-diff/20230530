# Comparing `tmp/dwiqc-0.3.1-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.3.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24105 bytes, number of entries: 22
+Zip file size: 24110 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-May-19 16:11 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-30 14:45 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-30 15:50 dwiqc/__version__.py
 -rw-r--r--  2.0 unx      283 b- defN 23-May-25 14:54 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-19 16:11 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-May-25 14:45 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5610 b- defN 23-May-26 13:48 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     3722 b- defN 23-May-26 16:03 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-19 16:11 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-19 16:11 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:11 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-19 16:11 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx     8810 b- defN 23-May-30 15:45 dwiqc/tasks/prequal.py
--rw-r--r--  2.0 unx     4480 b- defN 23-May-30 14:45 dwiqc/tasks/prequal_EQ.py
+-rw-r--r--  2.0 unx     4483 b- defN 23-May-30 15:50 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6064 b- defN 23-May-26 13:26 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3782 b- defN 23-May-19 16:11 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    16212 b- defN 23-May-26 11:38 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5765 b- defN 23-May-30 15:46 dwiqc-0.3.1.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      432 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1716 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/RECORD
-22 files, 68142 bytes uncompressed, 21353 bytes compressed:  68.7%
+-rwxr-xr-x  2.0 unx     5765 b- defN 23-May-30 15:51 dwiqc-0.3.2.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-30 15:52 dwiqc-0.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      432 b- defN 23-May-30 15:52 dwiqc-0.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-30 15:52 dwiqc-0.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-30 15:51 dwiqc-0.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1716 b- defN 23-May-30 15:52 dwiqc-0.3.2.dist-info/RECORD
+22 files, 68145 bytes uncompressed, 21358 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.3.1.data/scripts/dwiQC.py
+Filename: dwiqc-0.3.2.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.3.1.dist-info/LICENSE
+Filename: dwiqc-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.3.1.dist-info/METADATA
+Filename: dwiqc-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.3.1.dist-info/WHEEL
+Filename: dwiqc-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.3.1.dist-info/top_level.txt
+Filename: dwiqc-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.3.1.dist-info/RECORD
+Filename: dwiqc-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/tasks/prequal_EQ.py

```diff
@@ -86,14 +86,15 @@
 		else:
 			logging.error('eddy quad threw an error. exiting.')
 			sys.exit()
 
 		eddy_results_dir = f'{self._outdir}/EDDY/eddy_results.qc'
 
 		self.parse_json(eddy_results_dir)
+
 		self.extract_b0_vol()
 
 
 	def parse_json(self, eddy_dir):
 		logging.info('parsing qc.json file.')
 		with open(f'{eddy_dir}/qc.json', 'r') as file:
 			data = json.load(file)
@@ -153,13 +154,14 @@
 
 
 		with open('eddy_metrics.json', 'w') as outfile:
 			json.dump(metrics_dict, outfile, indent=1)
 
 		logging.info('successfully parsed json and wrote out results to eddy_metrics.json')
 
-
-	def extract_b0_vol(self)
+	def extract_b0_vol(self):
 		os.chdir(f"{self._outdir}/PREPROCESSED")
 		extract_command = "fslselectvols -i dwmri.nii.gz -o b0_volume --vols=0"
 		proc1 = subprocess.Popen(extract_command, shell=True, stdout=subprocess.PIPE)
 		proc1.communicate()
+
+
```

## Comparing `dwiqc-0.3.1.data/scripts/dwiQC.py` & `dwiqc-0.3.2.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.3.1.dist-info/LICENSE` & `dwiqc-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.3.1.dist-info/RECORD` & `dwiqc-0.3.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=MP_XhyztqRDYi-3-mBwJfNK9vFv5Jaoje1D8omvEWlE,247
+dwiqc/__version__.py,sha256=b89qqQFDNCj7_2lbaopqcr6yjN3RxcMtSf9TI8TeZH8,247
 dwiqc/browser/__init__.py,sha256=MlUOz0v7bA_dtQyXX27WF0dzyGGo4xkEEt2PT2B0_aQ,283
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=CT0xW2qSRlGcpQDUumFnqGSMvH9zFHU7Y2rELBS9-jQ,5610
 dwiqc/cli/tandem.py,sha256=_lSryhvKIzRRdnBnwfKPdfSBV98JwDfz6lzbqETQ3rw,3722
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=5ztmuvWk2xUqgVUkyl1EWmxb84nmDA61ii1ST0XqCh8,8810
-dwiqc/tasks/prequal_EQ.py,sha256=rGVMhN2gKScq0LTPshexzwiAfnuCaLAJEkqzyYQNKMw,4480
+dwiqc/tasks/prequal_EQ.py,sha256=cV3V6WP1_YHLz5dtwWGxS_HPdtbqnra2xT64-_TEdj0,4483
 dwiqc/tasks/qsiprep.py,sha256=h4xFJ3dPYPCkelHAtrpGZx47P938dQDOmSeT5JEC__0,6064
 dwiqc/tasks/qsiprep_EQ.py,sha256=JWildptHsuyJVj7ZYMFlWWYvsAIszJpWk1a0m05JM-Q,3782
 dwiqc/xnat/__init__.py,sha256=4-tJIvDSzSiek-aNwRwvKTQ19_xhEwsF-7ty9czWwec,16212
-dwiqc-0.3.1.data/scripts/dwiQC.py,sha256=0SqQiNyS6ZJmVISRgLuBpP0wFmwsvuXS22-7_Q7dpDo,5765
-dwiqc-0.3.1.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.3.1.dist-info/METADATA,sha256=c8CeMp7if_xjZoM9KyJqE4Jfu51TBTfI8d5mGGZKEfc,432
-dwiqc-0.3.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.3.1.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.3.1.dist-info/RECORD,,
+dwiqc-0.3.2.data/scripts/dwiQC.py,sha256=0SqQiNyS6ZJmVISRgLuBpP0wFmwsvuXS22-7_Q7dpDo,5765
+dwiqc-0.3.2.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.3.2.dist-info/METADATA,sha256=a1vMj1_DssBwHgZkOAMa-FaZ0TZmKqWs6SHtDZP-_G8,432
+dwiqc-0.3.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.3.2.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.3.2.dist-info/RECORD,,
```

