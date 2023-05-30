# Comparing `tmp/curveengine-1.1.1-py3-none-any.whl.zip` & `tmp/curveengine-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14805 bytes, number of entries: 12
+Zip file size: 14710 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      816 b- defN 23-May-23 20:55 curveengine/__init__.py
--rw-rw-rw-  2.0 fat     7953 b- defN 23-May-23 20:55 curveengine/engine.py
+-rw-rw-rw-  2.0 fat     7288 b- defN 23-May-30 15:26 curveengine/engine.py
 -rw-rw-rw-  2.0 fat      272 b- defN 23-May-23 20:55 curveengine/parsing/__init__.py
 -rw-rw-rw-  2.0 fat    34375 b- defN 23-May-30 02:19 curveengine/parsing/checks.py
 -rw-rw-rw-  2.0 fat     3617 b- defN 23-May-23 20:55 curveengine/parsing/enums.py
 -rw-rw-rw-  2.0 fat     4257 b- defN 23-May-23 20:55 curveengine/parsing/others.py
 -rw-rw-rw-  2.0 fat     8004 b- defN 23-May-30 02:12 curveengine/parsing/parsers.py
--rw-rw-rw-  2.0 fat    14022 b- defN 23-May-30 02:14 curveengine/parsing/ratehelpers.py
--rw-rw-rw-  2.0 fat      550 b- defN 23-May-30 02:23 curveengine-1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 02:23 curveengine-1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-30 02:23 curveengine-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      994 b- defN 23-May-30 02:23 curveengine-1.1.1.dist-info/RECORD
-12 files, 74964 bytes uncompressed, 13133 bytes compressed:  82.5%
+-rw-rw-rw-  2.0 fat    14214 b- defN 23-May-30 15:10 curveengine/parsing/ratehelpers.py
+-rw-rw-rw-  2.0 fat      550 b- defN 23-May-30 17:22 curveengine-1.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 17:22 curveengine-1.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-30 17:22 curveengine-1.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      994 b- defN 23-May-30 17:22 curveengine-1.1.2.dist-info/RECORD
+12 files, 74491 bytes uncompressed, 13038 bytes compressed:  82.5%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: curveengine/parsing/parsers.py
 Comment: 
 
 Filename: curveengine/parsing/ratehelpers.py
 Comment: 
 
-Filename: curveengine-1.1.1.dist-info/METADATA
+Filename: curveengine-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: curveengine-1.1.1.dist-info/WHEEL
+Filename: curveengine-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: curveengine-1.1.1.dist-info/top_level.txt
+Filename: curveengine-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: curveengine-1.1.1.dist-info/RECORD
+Filename: curveengine-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## curveengine/engine.py

```diff
@@ -10,27 +10,27 @@
     Class for building curves and indexes from a JSON configuration file.
 
     Parameters
     ----------
     data : dict
         The JSON configuration file as a dictionary.
     curves : dict, optional
-        A dictionary of curves to be populated by the engine. The default is {}.
+        A dictionary of curves to be populated by the engine. The default is None.
     indexes : dict, optional
-        A dictionary of indexes to be populated by the engine. The default is {}.
+        A dictionary of indexes to be populated by the engine. The default is None.
 
     Returns
     -------
     None
     '''
 
-    def __init__(self, data, curves={}, indexes={}):
+    def __init__(self, data, curves=None, indexes=None):
         self.curveHandles = {None: ore.RelinkableYieldTermStructureHandle()}
-        self.curves = curves
-        self.indexes = indexes
+        self.curves = {} if curves is None else curves
+        self.indexes = {} if indexes is None else indexes
         localData = data.copy()
         checkConfiguration(localData)
         self.__initialize(localData)
 
     '''
     Get a curve by name.
 
@@ -121,51 +121,43 @@
         config = data['curveConfig']
         for i, rateHelper in enumerate(config['rateHelpers']):
             helperType = rateHelper['helperType']
             helperConfig = rateHelper['helperConfig']
             if 'discountCurve' not in helperConfig.keys():
                 helperConfig['discountCurve'] = None
             marketConfig = rateHelper['marketConfig']
-            try:
-                if helperType == HelperType.Deposit:
-                    helper = createDepositRateHelper(
-                        helperConfig, marketConfig, self.curveHandles, self.indexes)
-                elif helperType == HelperType.OIS:
-                    helper = createOISRateHelper(
-                        helperConfig, marketConfig, self.curveHandles, self.indexes)
-                elif helperType == HelperType.Swap:
-                    helper = createSwapRateHelper(
-                        helperConfig, marketConfig, self.curveHandles, self.indexes)
-                elif helperType == HelperType.TenorBasis:
-                    helper = createTenorBasisSwapRateHelper(
-                        helperConfig, marketConfig, self.curveHandles, self.indexes)
-                elif helperType == HelperType.Xccy:
-                    helper = createCrossCcyFixFloatSwapRateHelper(
-                        helperConfig, marketConfig, self.curveHandles, self.indexes)
-                elif helperType == HelperType.FxSwap:
-                    helper = createFxSwapRateHelper(
-                        helperConfig, marketConfig, self.curveHandles, self.indexes)
-                elif helperType == HelperType.SofrFuture:
-                    helper = createSofrFutureRateHelper(
-                        helperConfig, marketConfig, self.curveHandles, self.indexes)
-                elif helperType == HelperType.XccyBasis:
-                    helper = createCrossCcyBasisSwapRateHelper(
-                        helperConfig, marketConfig, self.curveHandles, self.indexes)
-                elif helperType == HelperType.Bond:
-                    helper = createFixedRateBondRateHelper(
-                        helperConfig, marketConfig, self.curveHandles, self.indexes)
-                else:
-                    raise Exception(
-                        'Unknown rate helper type: {}'.format(helperType))
-            except KeyError as e:
-                raise KeyError('Failed to create rate helper {helper}/{i} at curve {curveName}: Key not found: {error} '.format(
-                    helper=helperType, curveName=data['curveName'], error=e, i=i))
-            except Exception as e:
-                raise Exception('Failed to create rate helper {helper}/{i} at curve {curveName}: {error} '.format(
-                    helper=helperType, curveName=data['curveName'], error=e, i=i))
+        
+            if helperType == HelperType.Deposit:
+                helper = createDepositRateHelper(
+                    helperConfig, marketConfig, self.curveHandles, self.indexes)
+            elif helperType == HelperType.OIS:
+                helper = createOISRateHelper(
+                    helperConfig, marketConfig, self.curveHandles, self.indexes)
+            elif helperType == HelperType.Swap:
+                helper = createSwapRateHelper(
+                    helperConfig, marketConfig, self.curveHandles, self.indexes)
+            elif helperType == HelperType.TenorBasis:
+                helper = createTenorBasisSwapRateHelper(
+                    helperConfig, marketConfig, self.curveHandles, self.indexes)
+            elif helperType == HelperType.Xccy:
+                helper = createCrossCcyFixFloatSwapRateHelper(
+                    helperConfig, marketConfig, self.curveHandles, self.indexes)
+            elif helperType == HelperType.FxSwap:
+                helper = createFxSwapRateHelper(
+                    helperConfig, marketConfig, self.curveHandles, self.indexes)
+            elif helperType == HelperType.SofrFuture:
+                helper = createSofrFutureRateHelper(
+                    helperConfig, marketConfig, self.curveHandles, self.indexes)
+            elif helperType == HelperType.XccyBasis:
+                helper = createCrossCcyBasisSwapRateHelper(
+                    helperConfig, marketConfig, self.curveHandles, self.indexes)
+            elif helperType == HelperType.Bond:
+                helper = createFixedRateBondRateHelper(
+                    helperConfig, marketConfig, self.curveHandles, self.indexes)
+          
             rateHelpers.append(helper)
 
         refDate = ore.Settings.instance().evaluationDate
         dayCounter = config['dayCounter']
 
         curve = ore.PiecewiseLogLinearDiscount(
             refDate, rateHelpers, dayCounter)
```

## curveengine/parsing/ratehelpers.py

```diff
@@ -1,25 +1,25 @@
 from .parsers import *
 from .others import *
 
 
-def createOISRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createOISRateHelper(helperConfig: dict, marketConfig: dict, curveHandles: dict, indexes: dict, *args, **kwargs):
     """
     Create an OIS rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
 
     marketConfig : dict
         The market configuration for the helper
 
-    curves : dict
-        The curves
+    curveHandles : dict
+        The curveHandles
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.OISRateHelper
         The rate helper
@@ -36,15 +36,15 @@
     endOfMonth = helperConfig['endOfMonth']
     paymentLag = helperConfig['paymentLag']
     fixedLegFrequency = helperConfig['fixedLegFrequency']
     fwdStart = helperConfig['fwdStart']
     index = indexes[helperConfig['index']]
 
     rate = marketConfig['rate']['value']
-    discountCurve = curves[helperConfig['discountCurve']]
+    discountCurve = curveHandles[helperConfig['discountCurve']]
 
     rate = ore.QuoteHandle(ore.SimpleQuote(rate))
     helper = ore.OISRateHelper(settlementDays, tenor, rate, index, discountCurve, endOfMonth,
                                paymentLag, businessDayConvention, fixedLegFrequency, calendar, fwdStart)
     return helper
 
 
@@ -78,28 +78,28 @@
 
     rate = ore.QuoteHandle(ore.SimpleQuote(marketConfig['rate']['value']))
     helper = ore.DepositRateHelper(rate, tenor, settlementDays, calendar,
                                    convention, endOfMonth, dayCounter)
     return helper
 
 
-def createFixedRateBondRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createFixedRateBondRateHelper(helperConfig: dict, marketConfig: dict, curveHandles: dict, indexes: dict, *args, **kwargs):
     """
     Create a fixed rate bond helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
 
     marketConfig : dict
         The market configuration for the helper
 
-    curves : dict
-        The curves
+    curveHandles : dict
+        The curveHandles
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.BondHelper
         The rate helper
@@ -168,28 +168,28 @@
         ore.QuoteHandle(ore.SimpleQuote(cleanPrice)),
         fixedRateBond
     )
 
     return bondHelper
 
 
-def createSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createSwapRateHelper(helperConfig: dict, marketConfig: dict, curveHandles: dict, indexes: dict, *args, **kwargs):
     """
     Create a swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
 
     marketConfig : dict
         The market configuration for the helper      
 
-    curves : dict
-        The curves
+    curveHandles : dict
+        The curveHandles
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.SwapRateHelper
         The rate helper
@@ -211,37 +211,37 @@
     rateQuote = ore.QuoteHandle(ore.SimpleQuote(rate))
     spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
 
     # Index
     index = indexes[helperConfig['index']]
 
     # Discounting curve
-    discountCurve = curves[helperConfig['discountCurve']]
+    discountCurve = curveHandles[helperConfig['discountCurve']]
 
     # Swap rate helper
     swapRateHelper = ore.SwapRateHelper(
         rateQuote, tenor, calendar, fixedLegFrequency, convention, dayCounter, index, spreadQuote, fwdStart, discountCurve
     )
     return swapRateHelper
 
 
-def createFxSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createFxSwapRateHelper(helperConfig: dict, marketConfig: dict, curveHandles: dict, indexes: dict, *args, **kwargs):
     """
     Create a fx swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
 
     marketConfig : dict
         The market configuration for the helper
 
-    curves : dict
-        The curves
+    curveHandles : dict
+        The curveHandles
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.FxSwapRateHelper
         The rate helper
@@ -268,15 +268,15 @@
         tenor = ore.Period(days, ore.Days)
 
     # QuoteHandle
     fwdPointQuote = ore.QuoteHandle(ore.SimpleQuote(fxPoints))
     spotFxQuote = ore.QuoteHandle(ore.SimpleQuote(spotFx))
 
     # Discounting curve
-    discountCurve = curves[helperConfig['discountCurve']]
+    discountCurve = curveHandles[helperConfig['discountCurve']]
 
     # FxSwapRateHelper
     fxSwapRateHelper = ore.FxSwapRateHelper(
         fwdPointQuote,
         spotFxQuote,
         tenor,
         fixingDays,
@@ -286,28 +286,28 @@
         baseCurrencyAsCollateral,
         discountCurve,
         calendar
     )
     return fxSwapRateHelper
 
 
-def createSofrFutureRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createSofrFutureRateHelper(helperConfig: dict, marketConfig: dict, curveHandles: dict, indexes: dict, *args, **kwargs):
     """
     Create a sofr future rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
 
     marketConfig : dict
         The market configuration for the helper
 
-    curves : dict
-        The curves
+    curveHandles : dict
+        The curveHandles
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.SofrFutureRateHelper
         The rate helper
@@ -332,28 +332,28 @@
         year,
         frequency,
         convexityQuote
     )
     return sofrFutureRateHelper
 
 
-def createTenorBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createTenorBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curveHandles: dict, indexes: dict, *args, **kwargs):
     """
     Create a tenor basis swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
 
     marketConfig : dict
         The market configuration for the helper
 
-    curves : dict
-        The curves
+    curveHandles : dict
+        The curveHandles
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.TenorBasisSwapHelper
         The rate helper
@@ -370,15 +370,15 @@
     shortIndex = indexes[helperConfig['shortIndex']]
 
     # QuoteHandle
     spread = marketConfig['spread']['value']
     spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
 
     # Discounting curve
-    discountCurve = curves[helperConfig['discountCurve']]
+    discountCurve = curveHandles[helperConfig['discountCurve']]
 
     # TenorBasisSwapHelper
     tenorBasisSwapHelper = ore.TenorBasisSwapHelper(
         spreadQuote,
         tenor,
         longIndex,
         shortIndex,
@@ -387,28 +387,28 @@
         spreadOnShort,
         True
     )
 
     return tenorBasisSwapHelper
 
 
-def createCrossCcyFixFloatSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createCrossCcyFixFloatSwapRateHelper(helperConfig: dict, marketConfig: dict, curveHandles: dict, indexes: dict, *args, **kwargs):
     """
     Create a cross currency fix float swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper        
 
     marketConfig : dict
         The market configuration for the helper
 
-    curves : dict
-        The curves
+    curveHandles : dict
+        The curveHandles
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.CrossCcyFixFloatSwapHelper
         The rate helper
@@ -435,15 +435,15 @@
     spotFxQuote = ore.QuoteHandle(ore.SimpleQuote(spotFx))
     spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
 
     # Index
     index = indexes[helperConfig['index']]
 
     # Discounting curve
-    discountCurve = curves[helperConfig['discountCurve']]
+    discountCurve = curveHandles[helperConfig['discountCurve']]
 
     # CrossCcyFixFloatSwapHelper
     crossCcyFixFloatSwapHelper = ore.CrossCcyFixFloatSwapHelper(
         rateQuote,
         spotFxQuote,
         settlementDays,
         calendar,
@@ -457,30 +457,30 @@
         discountCurve,
         spreadQuote,
         endOfMonth
     )
     return crossCcyFixFloatSwapHelper
 
 
-def createCrossCcyBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+def createCrossCcyBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curveHandles: dict, indexes: dict, *args, **kwargs):
     """
     Create a cross currency basis swap rate helper
 
     Parameters
     ----------
     helperConfig : dict
         The configuration for the helper
 
     marketConfig : dict
         The market configuration for the helper
         - spread : float
             The spread
 
-    curves : dict
-        The curves
+    curveHandles : dict
+        The curveHandles
     indexes : dict
         The indexes
 
     Returns
     -------
     ore.CrossCcyBasisSwapHelper
         The rate helper
@@ -491,17 +491,17 @@
     """
     tenor = helperConfig['tenor']
     calendar = helperConfig['calendar']
     settlementDays = helperConfig['settlementDays']
     endOfMonth = helperConfig['endOfMonth']
     convention = helperConfig['convention']
 
-    # Discout curves
-    flatDiscountCurve = curves[helperConfig['discountCurve']]
-    spreadDiscountCurve = curves[helperConfig['discountCurve']]
+    # Discout curveHandles
+    flatDiscountCurve = curveHandles[helperConfig['discountCurve']]
+    spreadDiscountCurve = curveHandles[helperConfig['discountCurve']]
 
     # Index
     flatIndex = indexes[helperConfig['flatIndex']]
     spreadIndex = indexes[helperConfig['spreadIndex']]
 
     # QuoteHandle
     spread = marketConfig['spread']['value']
```

## Comparing `curveengine-1.1.1.dist-info/METADATA` & `curveengine-1.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curveengine
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple curve bootstraping tool based on ORE/QuantLib
 Author: Jose Melo
 Author-email: jmelo@live.cl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Requires-Dist: open-source-risk-engine
```

## Comparing `curveengine-1.1.1.dist-info/RECORD` & `curveengine-1.1.2.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 curveengine/__init__.py,sha256=fG7Ka2v7aTn4pF7lI0zG-neRIZUS8vm6EyF0cxUrCHo,816
-curveengine/engine.py,sha256=ivxgjZjGf8S9UzSaOg9ZJX6Mj-jMVHDQAP24TlcLsZE,7953
+curveengine/engine.py,sha256=HF2MJXybiGHLNIv1OHcfcYdDzlrrsrGCL7tZJF-lVoI,7288
 curveengine/parsing/__init__.py,sha256=jiYxFpB8cxfRiLTIomE7LguueKAKylTb2vrbrj8j1RU,272
 curveengine/parsing/checks.py,sha256=pJfMKomtCgJEbfUuAQGUNG2O4ErWSTfBR3is-04sMX8,34375
 curveengine/parsing/enums.py,sha256=nYlnk3PCV4Jax0Tu68Sh-qpBRR3DWFGXX0W3wI9n0xY,3617
 curveengine/parsing/others.py,sha256=2vNml3mjqUnX9D5Yyce9Y15sWv5JmC8RyS4D0EJH4mI,4257
 curveengine/parsing/parsers.py,sha256=61tqPjHveE6Duu1UJjROWwLlk8sFd_UEpjiVbpdj8pc,8004
-curveengine/parsing/ratehelpers.py,sha256=JBZLC0f634GGF-3MAU6f7u3jO4OSvN8Rcf__Wwn04fA,14022
-curveengine-1.1.1.dist-info/METADATA,sha256=iRO33oBEoHZurvJB1PIbaYJ8YsOyVZ0WU_BhaTgl_Nk,550
-curveengine-1.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-curveengine-1.1.1.dist-info/top_level.txt,sha256=LK8Ltzj4yLB5cfrjUzMY4Uokv2JNYXqgbUzChD4c92c,12
-curveengine-1.1.1.dist-info/RECORD,,
+curveengine/parsing/ratehelpers.py,sha256=uphByfYCN0na5CzTg4IMerTSKFF3j9kHrxjNNcAKGgc,14214
+curveengine-1.1.2.dist-info/METADATA,sha256=CFLhjwMaEz8Vy9shWRLWPs9O_X6-3VlX3PhhlLv2apI,550
+curveengine-1.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+curveengine-1.1.2.dist-info/top_level.txt,sha256=LK8Ltzj4yLB5cfrjUzMY4Uokv2JNYXqgbUzChD4c92c,12
+curveengine-1.1.2.dist-info/RECORD,,
```

