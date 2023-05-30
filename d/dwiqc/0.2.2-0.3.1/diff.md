# Comparing `tmp/dwiqc-0.2.2-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.3.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,24 @@
-Zip file size: 22458 bytes, number of entries: 21
+Zip file size: 24105 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-May-19 16:11 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-26 13:38 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-30 14:45 dwiqc/__version__.py
 -rw-r--r--  2.0 unx      283 b- defN 23-May-25 14:54 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-19 16:11 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-May-25 14:45 dwiqc/cli/get.py
--rw-r--r--  2.0 unx     5731 b- defN 23-May-26 13:28 dwiqc/cli/process.py
+-rw-r--r--  2.0 unx     5610 b- defN 23-May-26 13:48 dwiqc/cli/process.py
+-rw-r--r--  2.0 unx     3722 b- defN 23-May-26 16:03 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-19 16:11 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-19 16:11 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:11 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-19 16:11 dwiqc/tasks/__init__.py
--rw-r--r--  2.0 unx     8664 b- defN 23-May-23 14:22 dwiqc/tasks/prequal.py
--rw-r--r--  2.0 unx     4209 b- defN 23-May-22 17:12 dwiqc/tasks/prequal_EQ.py
+-rw-r--r--  2.0 unx     8810 b- defN 23-May-30 15:45 dwiqc/tasks/prequal.py
+-rw-r--r--  2.0 unx     4480 b- defN 23-May-30 14:45 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6064 b- defN 23-May-26 13:26 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3782 b- defN 23-May-19 16:11 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    16212 b- defN 23-May-26 11:38 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     3889 b- defN 23-May-26 13:39 dwiqc-0.2.2.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      432 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1640 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/RECORD
-21 files, 62172 bytes uncompressed, 19820 bytes compressed:  68.1%
+-rwxr-xr-x  2.0 unx     5765 b- defN 23-May-30 15:46 dwiqc-0.3.1.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      432 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1716 b- defN 23-May-30 15:46 dwiqc-0.3.1.dist-info/RECORD
+22 files, 68142 bytes uncompressed, 21353 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: dwiqc/cli/get.py
 Comment: 
 
 Filename: dwiqc/cli/process.py
 Comment: 
 
+Filename: dwiqc/cli/tandem.py
+Comment: 
+
 Filename: dwiqc/config/__init__.py
 Comment: 
 
 Filename: dwiqc/config/dwiqc.yaml
 Comment: 
 
 Filename: dwiqc/state/__init__.py
@@ -39,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.2.2.data/scripts/dwiQC.py
+Filename: dwiqc-0.3.1.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.2.2.dist-info/LICENSE
+Filename: dwiqc-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.2.2.dist-info/METADATA
+Filename: dwiqc-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.2.2.dist-info/WHEEL
+Filename: dwiqc-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.2.2.dist-info/top_level.txt
+Filename: dwiqc-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.2.2.dist-info/RECORD
+Filename: dwiqc-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.2.2'
+__version__ = '0.3.1'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/cli/process.py

```diff
@@ -46,19 +46,16 @@
     # grab the dwi and json files using pybids and os
 
     dwi_file = os.path.basename(layout.get(subject=args.sub, extension='.nii.gz', suffix='dwi', run=args.run, return_type='filename').pop())
 
     json_file = os.path.basename(layout.get(subject=args.sub, extension='.json', suffix='dwi', run=args.run, return_type='filename').pop())
 
     basename = os.path.splitext(json_file)[0]
-
-    # ⬇️ not sure what to do with these... will come back here.
    
     #logger.debug('DWI raw: %s', raw)
-    #logger.debug('T1vnav sourcedata: %s', source)
 
 
     # prequal job
     prequal_outdir = None
     if 'prequal' in args.sub_tasks:
         logger.debug('building prequal task')
         prequal_outdir = os.path.join(args.bids_dir, 'derivatives', 'dwiqc-prequal', f'sub-{args.sub}', f'ses-{args.ses}', basename, 'OUTPUTS')
@@ -122,16 +119,14 @@
 
     if not args.artifacts_dir:
         args.artifacts_dir = os.path.join(
             args.bids_dir,
             'xnat-artifacts'
         )
 
-
-
     # build data to upload to xnat
     R = Report(args.bids_dir, args.sub, args.ses, args.run)
     logger.info('building xnat artifacts to %s', args.artifacts_dir)
     R.build_assessment(args.artifacts_dir)
 
     # upload data to xnat over rest api
     if args.xnat_upload:
@@ -172,7 +167,8 @@
 
 def copy_qsiprep_output(args, qsiprep_outdir):
     final_qsiprep_outdir = os.path.join(args.bids_dir, 'derivatives', 'dwiqc-qsiprep', f'sub-{args.sub}', f'ses-{args.ses}', basename, 'qsiprep_output')
     shutil.copytree(qsiprep_outdir, final_qsiprep_outdir)
 
 
 
+
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## dwiqc/tasks/prequal.py

```diff
@@ -6,19 +6,23 @@
 import logging
 from bids import BIDSLayout
 import sys
 import json
 import dwiqc.tasks as tasks
 import shutil
 from executors.models import Job
+sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
+from env_modules_python import module
 
 
 logger = logging.getLogger(__name__)
 
 
+module('load', 'cuda/9.1.85-fasrc01')
+
 # pull in some parameters from the BaseTask class in the __init__.py directory
 
 class Task(tasks.BaseTask):
 	def __init__(self, sub, ses, run, bids, outdir, tempdir=None, pipenv=None):
 		self._sub = sub
 		self._ses = ses
 		self._run = run
@@ -332,7 +336,8 @@
 
 
 class DWISpecError(Exception):
 	pass
 
 
 
+
```

## dwiqc/tasks/prequal_EQ.py

```diff
@@ -86,14 +86,15 @@
 		else:
 			logging.error('eddy quad threw an error. exiting.')
 			sys.exit()
 
 		eddy_results_dir = f'{self._outdir}/EDDY/eddy_results.qc'
 
 		self.parse_json(eddy_results_dir)
+		self.extract_b0_vol()
 
 
 	def parse_json(self, eddy_dir):
 		logging.info('parsing qc.json file.')
 		with open(f'{eddy_dir}/qc.json', 'r') as file:
 			data = json.load(file)
 
@@ -151,7 +152,14 @@
 		## Write out all these values to json file
 
 
 		with open('eddy_metrics.json', 'w') as outfile:
 			json.dump(metrics_dict, outfile, indent=1)
 
 		logging.info('successfully parsed json and wrote out results to eddy_metrics.json')
+
+
+	def extract_b0_vol(self)
+		os.chdir(f"{self._outdir}/PREPROCESSED")
+		extract_command = "fslselectvols -i dwmri.nii.gz -o b0_volume --vols=0"
+		proc1 = subprocess.Popen(extract_command, shell=True, stdout=subprocess.PIPE)
+		proc1.communicate()
```

## Comparing `dwiqc-0.2.2.data/scripts/dwiQC.py` & `dwiqc-0.3.1.data/scripts/dwiQC.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     parser.add_argument('-v', '--verbose', action='store_true',
         help='Enable verbose logging')
     parser.add_argument('-c', '--config', default=config.default(),
         help='dwiQC configuration file')
     parser.add_argument('--insecure', action='store_true',
         help='Disable SSL certificate verification')
     subparsers = parser.add_subparsers(help='sub-command help')
+    
     # get mode
     parser_get = subparsers.add_parser('get', help='get -h')
     parser_get.add_argument('--label', required=True,
         help='XNAT MR Session name')
     parser_get.add_argument('--project',
         help='XNAT Project name')
     parser_get.add_argument('--bids-dir', required=True,
@@ -77,14 +78,51 @@
         help='XNAT password')
     parser_process.add_argument('--artifacts-dir',
         help='Location for generated assessors and resources')
     parser_process.add_argument('--xnat-upload', action='store_true',
         help='Upload results to XNAT over REST API')
     parser_process.set_defaults(func=cli.process.do)
 
+    # tandem mode
+    parser_tandem = subparsers.add_parser('tandem', help='tandem -h')
+    parser_tandem.add_argument('--label', required=True,
+        help='XNAT MR Session name')
+    parser_tandem.add_argument('--project',
+        help='XNAT Project name')
+    parser_tandem.add_argument('--bids-dir', required=True,
+        help='Output BIDS directory')
+    parser_tandem.add_argument('--run', default=1, type=int,
+        help='BIDS run')
+    parser_tandem.add_argument('--partition', default='default',
+        help='Job scheduler partition')
+    parser_tandem.add_argument('--scheduler', default=None,
+        help='Choose a specific job scheduler')
+    parser_tandem.add_argument('--rate-limit', type=int, default=None, 
+        help='Rate limit the number of tasks executed in parallel (1=serial)')
+    parser_tandem.add_argument('--dry-run', action='store_true',
+        help='Do not execute any jobs')
+    parser_tandem.add_argument('--sub-tasks', nargs='+', default=['morph', 'mriqc', 'vnav'],
+        help='Run only certain sub tasks')
+    parser_tandem.add_argument('--fs-license',
+        help='Base64 encoded FreeSurfer license')
+    parser_tandem.add_argument('--mock-fs', action='store_true',
+        help='Extract mocked FreeSurfer data for testing')
+    parser_tandem.add_argument('--xnat-alias',
+        help='YAXIL authentication alias')
+    parser_tandem.add_argument('--xnat-host',
+        help='XNAT host')
+    parser_tandem.add_argument('--xnat-user',
+        help='XNAT username')
+    parser_tandem.add_argument('--xnat-pass',
+        help='XNAT password')
+    parser_tandem.add_argument('--artifacts-dir',
+        help='Location for generated assessors and resources')
+    parser_tandem.add_argument('--xnat-upload', action='store_true',
+        help='Upload results to XNAT over REST API')
+    parser_tandem.set_defaults(func=cli.tandem.do)
     args = parser.parse_args()
 
 
     configure_logging(args.verbose)
     logger.info('Welcome to dwiQC version %s', dwiqc.version())
 
     # fire parser_*.set_defaults(func=<function>)
@@ -100,7 +138,8 @@
         datefmt='%Y-%m-%d %H:%M:%S'
     )
 
 if __name__ == '__main__':
    main()
 
 
+
```

## Comparing `dwiqc-0.2.2.dist-info/LICENSE` & `dwiqc-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.2.2.dist-info/RECORD` & `dwiqc-0.3.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=JG0S942mJGhbQCQIJBp9bR8VWELpRCcBPOGM97kE3SY,247
+dwiqc/__version__.py,sha256=MP_XhyztqRDYi-3-mBwJfNK9vFv5Jaoje1D8omvEWlE,247
 dwiqc/browser/__init__.py,sha256=MlUOz0v7bA_dtQyXX27WF0dzyGGo4xkEEt2PT2B0_aQ,283
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
-dwiqc/cli/process.py,sha256=WlCWyY-zd3lnOwbgeZ6wPPGNv5ZAetn_X4Id2QieEJs,5731
+dwiqc/cli/process.py,sha256=CT0xW2qSRlGcpQDUumFnqGSMvH9zFHU7Y2rELBS9-jQ,5610
+dwiqc/cli/tandem.py,sha256=_lSryhvKIzRRdnBnwfKPdfSBV98JwDfz6lzbqETQ3rw,3722
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
-dwiqc/tasks/prequal.py,sha256=GagoXzYhHaWV2uEfcadsc-85ij71hxP3YnZDANMO2UY,8664
-dwiqc/tasks/prequal_EQ.py,sha256=PWmlo8u_D5qM1lyXdmT7iq865JL6xoPM0JHGEwzRnes,4209
+dwiqc/tasks/prequal.py,sha256=5ztmuvWk2xUqgVUkyl1EWmxb84nmDA61ii1ST0XqCh8,8810
+dwiqc/tasks/prequal_EQ.py,sha256=rGVMhN2gKScq0LTPshexzwiAfnuCaLAJEkqzyYQNKMw,4480
 dwiqc/tasks/qsiprep.py,sha256=h4xFJ3dPYPCkelHAtrpGZx47P938dQDOmSeT5JEC__0,6064
 dwiqc/tasks/qsiprep_EQ.py,sha256=JWildptHsuyJVj7ZYMFlWWYvsAIszJpWk1a0m05JM-Q,3782
 dwiqc/xnat/__init__.py,sha256=4-tJIvDSzSiek-aNwRwvKTQ19_xhEwsF-7ty9czWwec,16212
-dwiqc-0.2.2.data/scripts/dwiQC.py,sha256=D6ZRhtwJAl0gYODeWhrT4fl7tZtnul0iXrMRyrHxIfE,3889
-dwiqc-0.2.2.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.2.2.dist-info/METADATA,sha256=0u518gvez7WYjpQV8nqj2Kok481T8p3De0wlHECj2lI,432
-dwiqc-0.2.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.2.2.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.2.2.dist-info/RECORD,,
+dwiqc-0.3.1.data/scripts/dwiQC.py,sha256=0SqQiNyS6ZJmVISRgLuBpP0wFmwsvuXS22-7_Q7dpDo,5765
+dwiqc-0.3.1.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.3.1.dist-info/METADATA,sha256=c8CeMp7if_xjZoM9KyJqE4Jfu51TBTfI8d5mGGZKEfc,432
+dwiqc-0.3.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.3.1.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.3.1.dist-info/RECORD,,
```

