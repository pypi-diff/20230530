# Comparing `tmp/dwiqc-0.3.4-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.3.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24110 bytes, number of entries: 22
+Zip file size: 24124 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-May-19 16:11 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-30 21:08 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-30 21:16 dwiqc/__version__.py
 -rw-r--r--  2.0 unx      283 b- defN 23-May-25 14:54 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-19 16:11 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-May-25 14:45 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5611 b- defN 23-May-30 21:07 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     3722 b- defN 23-May-26 16:03 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-19 16:11 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-19 16:11 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:11 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-19 16:11 dwiqc/tasks/__init__.py
--rw-r--r--  2.0 unx     8810 b- defN 23-May-30 15:45 dwiqc/tasks/prequal.py
+-rw-r--r--  2.0 unx     8863 b- defN 23-May-30 21:16 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4483 b- defN 23-May-30 15:50 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6064 b- defN 23-May-26 13:26 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-May-30 20:59 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    16297 b- defN 23-May-30 21:00 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5766 b- defN 23-May-30 21:09 dwiqc-0.3.4.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-30 21:09 dwiqc-0.3.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      432 b- defN 23-May-30 21:09 dwiqc-0.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-30 21:09 dwiqc-0.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-30 21:09 dwiqc-0.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1716 b- defN 23-May-30 21:09 dwiqc-0.3.4.dist-info/RECORD
-22 files, 68322 bytes uncompressed, 21358 bytes compressed:  68.7%
+-rwxr-xr-x  2.0 unx     5766 b- defN 23-May-30 21:17 dwiqc-0.3.5.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-30 21:18 dwiqc-0.3.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      432 b- defN 23-May-30 21:18 dwiqc-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-30 21:18 dwiqc-0.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-30 21:17 dwiqc-0.3.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1716 b- defN 23-May-30 21:18 dwiqc-0.3.5.dist-info/RECORD
+22 files, 68375 bytes uncompressed, 21372 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.3.4.data/scripts/dwiQC.py
+Filename: dwiqc-0.3.5.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.3.4.dist-info/LICENSE
+Filename: dwiqc-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.3.4.dist-info/METADATA
+Filename: dwiqc-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.3.4.dist-info/WHEEL
+Filename: dwiqc-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.3.4.dist-info/top_level.txt
+Filename: dwiqc-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.3.4.dist-info/RECORD
+Filename: dwiqc-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.3.4'
+__version__ = '0.3.5'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/tasks/prequal.py

```diff
@@ -29,15 +29,18 @@
 		self._bids = bids
 		self._layout = BIDSLayout(bids)
 		super().__init__(outdir, tempdir, pipenv)
 
 
 	# create an INPUTS dir next to the OUTPUTS dir
 	def copy_inputs(self, inputs_dir):
-		os.makedirs(inputs_dir)
+		try:
+			os.makedirs(inputs_dir)
+		except OSError:
+			os.makedirs(inputs_dir)
 		#layout = BIDSLayout(self._bids) # load the data layout into pybids
 		all_files = self._layout.get(subject=self._sub, session=self._ses, run=self._run, return_type='filename') # get a list of all of the subject's files
 		# copy the all the subject's files into the INPUTS directory
 		for file in all_files:
 			basename = os.path.basename(file)
 			dest = os.path.join(inputs_dir, basename)
 			shutil.copy(file, dest)
```

## Comparing `dwiqc-0.3.4.data/scripts/dwiQC.py` & `dwiqc-0.3.5.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.3.4.dist-info/LICENSE` & `dwiqc-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.3.4.dist-info/RECORD` & `dwiqc-0.3.5.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=2kSKQPPWs7S1mx6VfQWlijKG8_9hv7sGfltlZyVNp44,247
+dwiqc/__version__.py,sha256=xowxeqsz-kOW_Tq15jU92OPOEIkoUOQSWZLTJbO9bxA,247
 dwiqc/browser/__init__.py,sha256=MlUOz0v7bA_dtQyXX27WF0dzyGGo4xkEEt2PT2B0_aQ,283
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=8yu5Mo831gDElFEiEsjNfwc7w5L8A6jymARK-wuFt2U,5611
 dwiqc/cli/tandem.py,sha256=_lSryhvKIzRRdnBnwfKPdfSBV98JwDfz6lzbqETQ3rw,3722
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
-dwiqc/tasks/prequal.py,sha256=5ztmuvWk2xUqgVUkyl1EWmxb84nmDA61ii1ST0XqCh8,8810
+dwiqc/tasks/prequal.py,sha256=MVJuQqx2WkS0IGAhdL8pdcfC8Ka2AtRgSrRXUuACkwo,8863
 dwiqc/tasks/prequal_EQ.py,sha256=cV3V6WP1_YHLz5dtwWGxS_HPdtbqnra2xT64-_TEdj0,4483
 dwiqc/tasks/qsiprep.py,sha256=h4xFJ3dPYPCkelHAtrpGZx47P938dQDOmSeT5JEC__0,6064
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
 dwiqc/xnat/__init__.py,sha256=MA1CB00D6a5z3dHfN0D1TxXpvXmZrj8pqBgGgPdhCmI,16297
-dwiqc-0.3.4.data/scripts/dwiQC.py,sha256=76M57U-wyP0Webb3Q_KiQbK4setkfGpXjhKVFUHu9SY,5766
-dwiqc-0.3.4.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.3.4.dist-info/METADATA,sha256=0QkJvCII5urFi_mlKYyLVj3akFayGhRWYgGTZF9BAaQ,432
-dwiqc-0.3.4.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.3.4.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.3.4.dist-info/RECORD,,
+dwiqc-0.3.5.data/scripts/dwiQC.py,sha256=76M57U-wyP0Webb3Q_KiQbK4setkfGpXjhKVFUHu9SY,5766
+dwiqc-0.3.5.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.3.5.dist-info/METADATA,sha256=-BHwj4_ZGomOGrL_Vo13p9tHj4lBeIe3rjTd6Y4HWXw,432
+dwiqc-0.3.5.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.3.5.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.3.5.dist-info/RECORD,,
```

