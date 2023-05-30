# Comparing `tmp/up_lpg-0.0.6.4-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/up_lpg-0.0.7-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1190490 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       36 b- defN 23-May-03 12:54 up_lpg/__init__.py
--rw-rw-rw-  2.0 fat    10761 b- defN 23-May-03 12:54 up_lpg/lpg_planner.py
--rw-rw-rw-  2.0 fat  3881596 b- defN 23-May-03 12:54 up_lpg/winlpg.exe
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      336 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      620 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/RECORD
-8 files, 3905021 bytes uncompressed, 1189420 bytes compressed:  69.5%
+Zip file size: 1190477 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       36 b- defN 23-May-30 14:40 up_lpg/__init__.py
+-rw-rw-rw-  2.0 fat    10795 b- defN 23-May-30 14:40 up_lpg/lpg_planner.py
+-rw-rw-rw-  2.0 fat  3881596 b- defN 23-May-30 14:40 up_lpg/winlpg.exe
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      334 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      610 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/RECORD
+8 files, 3905043 bytes uncompressed, 1189427 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: up_lpg/lpg_planner.py
 Comment: 
 
 Filename: up_lpg/winlpg.exe
 Comment: 
 
-Filename: up_lpg-0.0.6.4.dist-info/LICENSE
+Filename: up_lpg-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: up_lpg-0.0.6.4.dist-info/METADATA
+Filename: up_lpg-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: up_lpg-0.0.6.4.dist-info/WHEEL
+Filename: up_lpg-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: up_lpg-0.0.6.4.dist-info/top_level.txt
+Filename: up_lpg-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: up_lpg-0.0.6.4.dist-info/RECORD
+Filename: up_lpg-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## up_lpg/lpg_planner.py

```diff
@@ -6,15 +6,15 @@
 import unified_planning as up
 from fractions import Fraction
 from unified_planning.model import ProblemKind, AbstractProblem
 from unified_planning.plans import PlanKind, Plan
 from unified_planning.engines import PlanGenerationResult, PlanGenerationResultStatus
 from unified_planning.engines import PDDLPlanner, Credits, LogMessage, PlanGenerationResult
 from unified_planning.exceptions import UPException
-from unified_planning.engines.mixins import AnytimePlannerMixin
+from unified_planning.engines.pddl_anytime_planner import PDDLAnytimePlanner
 from unified_planning.engines.mixins.plan_repairer import PlanRepairerMixin
 from typing import Callable, Optional, List, Union, Iterator, IO
 
 credits = Credits('LPG',
                   'UNIBS Team',
                   'ivan.serina@unibs.it',
                   'https://lpg.unibs.it',
@@ -127,25 +127,25 @@
     def supports(problem_kind: 'ProblemKind') -> bool:
         return problem_kind <= LPGEngine.supported_kind()
 
     @staticmethod
     def get_credits(**kwargs) -> Optional['Credits']:
         return credits
 
-class LPGAnytimeEngine(LPGEngine, AnytimePlannerMixin):
+class LPGAnytimeEngine(LPGEngine, PDDLAnytimePlanner):
 
     def __init__(self):
         super().__init__()
         self._options = []
 
     @property
     def name(self) -> str:
         return 'lpg-anytime'
 
-    def _get_cmd(self, domain_filename: str, problem_filename: str, plan_filename: str) -> List[str]:
+    def _get_anytime_cmd(self, domain_filename: str, problem_filename: str, plan_filename: str) -> List[str]:
         base_command = [pkg_resources.resource_filename(__name__, lpg_os[sys.platform]),
         '-o', domain_filename,
         '-f', problem_filename,
         '-n', '1000',
         '-noout'] + self._options
         return base_command
 
@@ -193,15 +193,15 @@
                         self._plan = []
                         self._storing = False
                     elif self._storing and l:
                         self._plan.append(l.split(':')[1].split('[')[0])
 
         def run():
             writer: IO[str] = Writer(output_stream, q, self)
-            res = self._solve(problem, output_stream=writer)
+            res = self._solve(problem, output_stream=writer, anytime=True)
             q.put(res)
 
         try:
             t = threading.Thread(target=run, daemon=True)
             t.start()
             status = PlanGenerationResultStatus.INTERMEDIATE
             while status == PlanGenerationResultStatus.INTERMEDIATE:
```

## Comparing `up_lpg-0.0.6.4.dist-info/LICENSE` & `up_lpg-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

