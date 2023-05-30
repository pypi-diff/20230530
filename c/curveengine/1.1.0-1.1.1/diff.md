# Comparing `tmp/curveengine-1.1.0-py3-none-any.whl.zip` & `tmp/curveengine-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14635 bytes, number of entries: 12
--rw-r--r--  2.0 unx      803 b- defN 23-May-23 01:29 curveengine/__init__.py
--rw-r--r--  2.0 unx     7755 b- defN 23-May-23 01:06 curveengine/engine.py
--rw-r--r--  2.0 unx      266 b- defN 23-May-23 01:18 curveengine/parsing/__init__.py
--rw-r--r--  2.0 unx    32971 b- defN 23-May-23 02:53 curveengine/parsing/checks.py
--rw-r--r--  2.0 unx     3462 b- defN 23-May-22 02:32 curveengine/parsing/enums.py
--rw-r--r--  2.0 unx     4115 b- defN 23-May-23 01:00 curveengine/parsing/others.py
--rw-r--r--  2.0 unx     7673 b- defN 23-May-23 01:01 curveengine/parsing/parsers.py
--rw-r--r--  2.0 unx    13513 b- defN 23-May-23 03:29 curveengine/parsing/ratehelpers.py
--rw-r--r--  2.0 unx      532 b- defN 23-May-23 03:30 curveengine-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 03:30 curveengine-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-23 03:30 curveengine-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      994 b- defN 23-May-23 03:30 curveengine-1.1.0.dist-info/RECORD
-12 files, 72188 bytes uncompressed, 12963 bytes compressed:  82.0%
+Zip file size: 14805 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      816 b- defN 23-May-23 20:55 curveengine/__init__.py
+-rw-rw-rw-  2.0 fat     7953 b- defN 23-May-23 20:55 curveengine/engine.py
+-rw-rw-rw-  2.0 fat      272 b- defN 23-May-23 20:55 curveengine/parsing/__init__.py
+-rw-rw-rw-  2.0 fat    34375 b- defN 23-May-30 02:19 curveengine/parsing/checks.py
+-rw-rw-rw-  2.0 fat     3617 b- defN 23-May-23 20:55 curveengine/parsing/enums.py
+-rw-rw-rw-  2.0 fat     4257 b- defN 23-May-23 20:55 curveengine/parsing/others.py
+-rw-rw-rw-  2.0 fat     8004 b- defN 23-May-30 02:12 curveengine/parsing/parsers.py
+-rw-rw-rw-  2.0 fat    14022 b- defN 23-May-30 02:14 curveengine/parsing/ratehelpers.py
+-rw-rw-rw-  2.0 fat      550 b- defN 23-May-30 02:23 curveengine-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 02:23 curveengine-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-30 02:23 curveengine-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      994 b- defN 23-May-30 02:23 curveengine-1.1.1.dist-info/RECORD
+12 files, 74964 bytes uncompressed, 13133 bytes compressed:  82.5%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: curveengine/parsing/parsers.py
 Comment: 
 
 Filename: curveengine/parsing/ratehelpers.py
 Comment: 
 
-Filename: curveengine-1.1.0.dist-info/METADATA
+Filename: curveengine-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: curveengine-1.1.0.dist-info/WHEEL
+Filename: curveengine-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: curveengine-1.1.0.dist-info/top_level.txt
+Filename: curveengine-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: curveengine-1.1.0.dist-info/RECORD
+Filename: curveengine-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## curveengine/__init__.py

 * *Ordering differences only*

```diff
@@ -1,14 +1,14 @@
-'''
-    The CurveEngine package is intended to be used to build curves and indexes from a JSON configuration file, using as backend QuantLib and QuantExt.
-    The main class is CurveEngine and has two methods: getCurve and getIndex. The first one returns a curve by name, 
-    the second one returns an index by name. 
-    
-    The class is initialized by the __initialize method, which is called by the constructor. 
-    The __initialize method is the one that actually builds the curves and indexes. 
-    
-    The constructor also takes two optional parameters: curves and indexes. These are dictionaries that can be used to populate the
-    curves and indexes of the engine. This is useful when the engine is used to build multiple
-    curves and indexes from other builds.
-'''
-
+'''
+    The CurveEngine package is intended to be used to build curves and indexes from a JSON configuration file, using as backend QuantLib and QuantExt.
+    The main class is CurveEngine and has two methods: getCurve and getIndex. The first one returns a curve by name, 
+    the second one returns an index by name. 
+    
+    The class is initialized by the __initialize method, which is called by the constructor. 
+    The __initialize method is the one that actually builds the curves and indexes. 
+    
+    The constructor also takes two optional parameters: curves and indexes. These are dictionaries that can be used to populate the
+    curves and indexes of the engine. This is useful when the engine is used to build multiple
+    curves and indexes from other builds.
+'''
+
 from .engine import *
```

## curveengine/engine.py

 * *Ordering differences only*

```diff
@@ -1,198 +1,198 @@
-from .parsing.parsers import *
-from .parsing.enums import *
-from .parsing.others import *
-from .parsing.ratehelpers import *
-from .parsing.checks import *
-
-
-class CurveEngine:
-    '''
-    Class for building curves and indexes from a JSON configuration file.
-
-    Parameters
-    ----------
-    data : dict
-        The JSON configuration file as a dictionary.
-    curves : dict, optional
-        A dictionary of curves to be populated by the engine. The default is {}.
-    indexes : dict, optional
-        A dictionary of indexes to be populated by the engine. The default is {}.
-
-    Returns
-    -------
-    None
-    '''
-
-    def __init__(self, data, curves={}, indexes={}):
-        self.curveHandles = {None: ore.RelinkableYieldTermStructureHandle()}
-        self.curves = curves
-        self.indexes = indexes
-        localData = data.copy()
-        checkConfiguration(localData)
-        self.__initialize(localData)
-
-    '''
-    Get a curve by name.
-
-    Parameters
-    ----------
-    curveName : str
-        The name of the curve to get.
-
-    Returns
-    -------
-    ore.YieldTermStructure
-        The curve with the given name.
-    '''
-
-    def getCurve(self, curveName):
-        return self.curves[curveName]
-
-    '''
-    Get an index by name.
-
-    Parameters
-    ----------
-    indexName : str
-        The name of the index to get.
-
-    Returns
-    -------
-    ore.IborIndex or ore.OvernightIndex
-        The index with the given name.
-    '''
-
-    def getIndex(self, indexName):
-        return self.indexes[indexName]
-
-    def __initialize(self, data):
-        refDate = parseDate(data['refDate'])
-        ore.Settings.instance().evaluationDate = refDate
-
-        tmpData = {}
-        for curve in data['curves']:
-            curveName = curve['curveName']
-            tmpData[curveName] = curve
-
-        dependencies = getDependencyList(data)
-        sortedList = topologicalSort(dependencies)
-        for curveName in sortedList:
-            parsed = parse(**tmpData[curveName])
-            if curveName not in self.indexes.keys():
-                self.__buildIndexes(parsed)
-            if curveName not in self.curves.keys():
-                self.__buildCurve(parsed)
-
-    def __buildIndexes(self, data):
-        name = data['curveName']
-        config = data['curveIndex']
-        indexType = config['indexType']
-        handle = ore.RelinkableYieldTermStructureHandle()
-        self.curveHandles[name] = handle
-        if indexType == IndexType.IborIndex:
-            index = createIborIndex(name, config, handle)
-        elif indexType == IndexType.OvernightIndex:
-            index = createOvernightIndex(name, config, handle)
-        else:
-            raise Exception(
-                'Unknown index type: {}'.format(indexType))
-        self.indexes[name] = index
-
-    def __buildCurve(self, data):
-        curveName = data['curveName']
-        config = data['curveConfig']
-        if config['curveType'] == CurveType.Piecewise:
-            curve = self.__buildPiecewiseCurve(data)
-        elif config['curveType'] == CurveType.Discount:
-            curve = self.__buildDiscountingCurve(data)
-        elif config['curveType'] == CurveType.FlatForward:
-            curve = self.__buildFlatForwardCurve(data)
-        else:
-            raise Exception(
-                'Unknown curve type: {}'.format(config['curveType']))
-
-        self.curveHandles[curveName].linkTo(curve)
-        self.indexes[curveName] = self.indexes[curveName].clone(
-            self.curveHandles[curveName])
-        self.curves[curveName] = curve
-
-    def __buildPiecewiseCurve(self, data):
-        rateHelpers = []
-        config = data['curveConfig']
-        for i, rateHelper in enumerate(config['rateHelpers']):
-            helperType = rateHelper['helperType']
-            helperConfig = rateHelper['helperConfig']
-            if 'discountCurve' not in helperConfig.keys():
-                helperConfig['discountCurve'] = None
-            marketConfig = rateHelper['marketConfig']
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
-            rateHelpers.append(helper)
-
-        refDate = ore.Settings.instance().evaluationDate
-        dayCounter = config['dayCounter']
-
-        curve = ore.PiecewiseLogLinearDiscount(
-            refDate, rateHelpers, dayCounter)
-        if 'enableExtrapolation' in config.keys():
-            if config['enableExtrapolation']:
-                curve.enableExtrapolation()
-
-        return curve
-
-    def __buildDiscountingCurve(self, data):
-        config = data['curveConfig']
-        dates = [node['date'] for node in config['nodes']]
-        dfs = [node['value'] for node in config['nodes']]
-        dayCounter = config['dayCounter']
-        if dates[0] != ore.Settings.instance().evaluationDate:
-            raise Exception(
-                'Failed to create curve {}: first date in discount curve must be the evaluation date'.format(data['curveName']))
-
-        if dfs[0] != 1.0:
-            raise Exception(
-                'Failed to create curve {}: first discount factor in discount curve must be 1.0'.format(data['curveName']))
-
-        curve = ore.DiscountCurve(dates, dfs, dayCounter)
-        if 'enableExtrapolation' in config.keys():
-            if config['enableExtrapolation']:
-                curve.enableExtrapolation()
-        return curve
-
-    def __buildFlatForwardCurve(self, data):
-        raise NotImplementedError("Flat forward curve not implemented yet")
+from .parsing.parsers import *
+from .parsing.enums import *
+from .parsing.others import *
+from .parsing.ratehelpers import *
+from .parsing.checks import *
+
+
+class CurveEngine:
+    '''
+    Class for building curves and indexes from a JSON configuration file.
+
+    Parameters
+    ----------
+    data : dict
+        The JSON configuration file as a dictionary.
+    curves : dict, optional
+        A dictionary of curves to be populated by the engine. The default is {}.
+    indexes : dict, optional
+        A dictionary of indexes to be populated by the engine. The default is {}.
+
+    Returns
+    -------
+    None
+    '''
+
+    def __init__(self, data, curves={}, indexes={}):
+        self.curveHandles = {None: ore.RelinkableYieldTermStructureHandle()}
+        self.curves = curves
+        self.indexes = indexes
+        localData = data.copy()
+        checkConfiguration(localData)
+        self.__initialize(localData)
+
+    '''
+    Get a curve by name.
+
+    Parameters
+    ----------
+    curveName : str
+        The name of the curve to get.
+
+    Returns
+    -------
+    ore.YieldTermStructure
+        The curve with the given name.
+    '''
+
+    def getCurve(self, curveName):
+        return self.curves[curveName]
+
+    '''
+    Get an index by name.
+
+    Parameters
+    ----------
+    indexName : str
+        The name of the index to get.
+
+    Returns
+    -------
+    ore.IborIndex or ore.OvernightIndex
+        The index with the given name.
+    '''
+
+    def getIndex(self, indexName):
+        return self.indexes[indexName]
+
+    def __initialize(self, data):
+        refDate = parseDate(data['refDate'])
+        ore.Settings.instance().evaluationDate = refDate
+
+        tmpData = {}
+        for curve in data['curves']:
+            curveName = curve['curveName']
+            tmpData[curveName] = curve
+
+        dependencies = getDependencyList(data)
+        sortedList = topologicalSort(dependencies)
+        for curveName in sortedList:
+            parsed = parse(**tmpData[curveName])
+            if curveName not in self.indexes.keys():
+                self.__buildIndexes(parsed)
+            if curveName not in self.curves.keys():
+                self.__buildCurve(parsed)
+
+    def __buildIndexes(self, data):
+        name = data['curveName']
+        config = data['curveIndex']
+        indexType = config['indexType']
+        handle = ore.RelinkableYieldTermStructureHandle()
+        self.curveHandles[name] = handle
+        if indexType == IndexType.IborIndex:
+            index = createIborIndex(name, config, handle)
+        elif indexType == IndexType.OvernightIndex:
+            index = createOvernightIndex(name, config, handle)
+        else:
+            raise Exception(
+                'Unknown index type: {}'.format(indexType))
+        self.indexes[name] = index
+
+    def __buildCurve(self, data):
+        curveName = data['curveName']
+        config = data['curveConfig']
+        if config['curveType'] == CurveType.Piecewise:
+            curve = self.__buildPiecewiseCurve(data)
+        elif config['curveType'] == CurveType.Discount:
+            curve = self.__buildDiscountingCurve(data)
+        elif config['curveType'] == CurveType.FlatForward:
+            curve = self.__buildFlatForwardCurve(data)
+        else:
+            raise Exception(
+                'Unknown curve type: {}'.format(config['curveType']))
+
+        self.curveHandles[curveName].linkTo(curve)
+        self.indexes[curveName] = self.indexes[curveName].clone(
+            self.curveHandles[curveName])
+        self.curves[curveName] = curve
+
+    def __buildPiecewiseCurve(self, data):
+        rateHelpers = []
+        config = data['curveConfig']
+        for i, rateHelper in enumerate(config['rateHelpers']):
+            helperType = rateHelper['helperType']
+            helperConfig = rateHelper['helperConfig']
+            if 'discountCurve' not in helperConfig.keys():
+                helperConfig['discountCurve'] = None
+            marketConfig = rateHelper['marketConfig']
+            try:
+                if helperType == HelperType.Deposit:
+                    helper = createDepositRateHelper(
+                        helperConfig, marketConfig, self.curveHandles, self.indexes)
+                elif helperType == HelperType.OIS:
+                    helper = createOISRateHelper(
+                        helperConfig, marketConfig, self.curveHandles, self.indexes)
+                elif helperType == HelperType.Swap:
+                    helper = createSwapRateHelper(
+                        helperConfig, marketConfig, self.curveHandles, self.indexes)
+                elif helperType == HelperType.TenorBasis:
+                    helper = createTenorBasisSwapRateHelper(
+                        helperConfig, marketConfig, self.curveHandles, self.indexes)
+                elif helperType == HelperType.Xccy:
+                    helper = createCrossCcyFixFloatSwapRateHelper(
+                        helperConfig, marketConfig, self.curveHandles, self.indexes)
+                elif helperType == HelperType.FxSwap:
+                    helper = createFxSwapRateHelper(
+                        helperConfig, marketConfig, self.curveHandles, self.indexes)
+                elif helperType == HelperType.SofrFuture:
+                    helper = createSofrFutureRateHelper(
+                        helperConfig, marketConfig, self.curveHandles, self.indexes)
+                elif helperType == HelperType.XccyBasis:
+                    helper = createCrossCcyBasisSwapRateHelper(
+                        helperConfig, marketConfig, self.curveHandles, self.indexes)
+                elif helperType == HelperType.Bond:
+                    helper = createFixedRateBondRateHelper(
+                        helperConfig, marketConfig, self.curveHandles, self.indexes)
+                else:
+                    raise Exception(
+                        'Unknown rate helper type: {}'.format(helperType))
+            except KeyError as e:
+                raise KeyError('Failed to create rate helper {helper}/{i} at curve {curveName}: Key not found: {error} '.format(
+                    helper=helperType, curveName=data['curveName'], error=e, i=i))
+            except Exception as e:
+                raise Exception('Failed to create rate helper {helper}/{i} at curve {curveName}: {error} '.format(
+                    helper=helperType, curveName=data['curveName'], error=e, i=i))
+            rateHelpers.append(helper)
+
+        refDate = ore.Settings.instance().evaluationDate
+        dayCounter = config['dayCounter']
+
+        curve = ore.PiecewiseLogLinearDiscount(
+            refDate, rateHelpers, dayCounter)
+        if 'enableExtrapolation' in config.keys():
+            if config['enableExtrapolation']:
+                curve.enableExtrapolation()
+
+        return curve
+
+    def __buildDiscountingCurve(self, data):
+        config = data['curveConfig']
+        dates = [node['date'] for node in config['nodes']]
+        dfs = [node['value'] for node in config['nodes']]
+        dayCounter = config['dayCounter']
+        if dates[0] != ore.Settings.instance().evaluationDate:
+            raise Exception(
+                'Failed to create curve {}: first date in discount curve must be the evaluation date'.format(data['curveName']))
+
+        if dfs[0] != 1.0:
+            raise Exception(
+                'Failed to create curve {}: first discount factor in discount curve must be 1.0'.format(data['curveName']))
+
+        curve = ore.DiscountCurve(dates, dfs, dayCounter)
+        if 'enableExtrapolation' in config.keys():
+            if config['enableExtrapolation']:
+                curve.enableExtrapolation()
+        return curve
+
+    def __buildFlatForwardCurve(self, data):
+        raise NotImplementedError("Flat forward curve not implemented yet")
```

## curveengine/parsing/__init__.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-'''
-    Parsing and checking functions. The main goal of this methods is to validate that the input JSON 
-    file is correct and can be used to build curves and indexes. The functions are called by the 
-    CurveEngine class, but are available for other uses.
-
-'''
+'''
+    Parsing and checking functions. The main goal of this methods is to validate that the input JSON 
+    file is correct and can be used to build curves and indexes. The functions are called by the 
+    CurveEngine class, but are available for other uses.
+
+'''
```

## curveengine/parsing/checks.py

```diff
@@ -1,1313 +1,1313 @@
-import re
-from functools import partial
-from .enums import *
-
-'''
-Example of a basic structure of the curve request:
-{
-    "refDate": "2020-01-01",
-    "curves": [
-        {
-            "curveName": "PiecewiseCurveExample",
-            "curveConfig": {
-                "curveType": "Piecewise",                
-                "dayCounter": "Actual360",
-                "enableExtrapolation": True,
-                "rateHelpers": [
-                    {                        
-                        "helperConfig": {
-                            ...
-                        },
-                        "marketConfig": {
-                            ...
-                        },
-                    }
-                ]
-            },
-            "curveIndex":{
-                ...
-            }
-        },
-        {
-            "curveName": "DiscountCurveExample",
-            "curveConfig": {
-                "curveType": "Discount",
-                "dayCounter": "Actual360",
-                "enableExtrapolation": True,
-                "nodes": [
-                    {
-                        "date": "2020-01-01",
-                        "discount": 0.01
-                    },
-                    {
-                        "date": "2020-02-01",
-                        "discount": 0.02
-                    }
-                ]
-            },
-            "curveIndex":{
-                ...
-            }
-        }
-    ]
-}
-'''
-
-
-class ConfigurationError(Exception):
-    '''
-    Exception raised when the request is invalid
-    '''
-
-    def __init__(self, message):
-        self.message = message
-
-
-class RateIndexError(ConfigurationError):
-    '''
-    Exception raised when the index is invalid
-    '''
-
-    def __init__(self, message):
-        self.message = message
-
-
-class RateHelperConfigurationError(ConfigurationError):
-    '''
-    Exception raised when the rate helper is invalid
-    '''
-
-    def __init__(self, message):
-        self.message = message
-
-
-class MarketConfigurationError(ConfigurationError):
-    '''
-    Exception raised when the market configuration is invalid
-    '''
-
-    def __init__(self, message):
-        self.message = message
-
-
-## Check available enums and possible instances#
-
-
-def checkDate(value) -> None:
-    '''
-    Check if the date is valid
-
-    Parameters
-    ----------
-    value: str
-        The date
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the date is invalid
-    '''
-    if not re.match(r'^\d{4}-\d{2}-\d{2}$', value):
-        raise ValueError(f'{value} is not a valid date')
-
-
-def checkIsInEnum(value: str, enum: list) -> None:
-    '''
-    Check if the value is in the enum
-
-    Parameters
-    ----------
-    value: str
-        The value to check
-    enum: list
-        The enum
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the value is not in the enum
-    '''
-    if value not in enum:
-        raise ValueError(f'{value} is not in {enum}')
-
-
-def checkDayCounter(value) -> None:
-    '''
-    Check if the day counter is valid
-
-    Parameters
-    ----------
-    value: str
-        The day counter. It must match the DayCounter enum.
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the day counter is invalid
-
-    Also see
-    --------
-    checkIsInEnum
-    DayCounter
-
-    '''
-    checkIsInEnum(value, DayCounter.__members__)
-
-
-def checkFrequency(value) -> None:
-    '''
-    Check if the frequency is valid
-
-    Parameters
-    ----------
-    value: str
-        The frequency, matching the Frequency enum.
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the frequency is invalid
-
-    Also see
-    --------
-    checkIsInEnum
-    Frequency
-    '''
-    checkIsInEnum(value, Frequency.__members__)
-
-
-def checkCompounding(value) -> None:
-    '''
-    Check if the compounding is valid
-
-    Parameters
-    ----------
-    value: str
-        The compounding, matching the Compounding enum.
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the compounding is invalid
-
-    Also see
-    --------
-    checkIsInEnum
-    Compounding
-    '''
-    checkIsInEnum(value, Compounding.__members__)
-
-
-def checkConvention(value) -> None:
-    '''
-    Check if the convention is valid
-
-    Parameters
-    ----------
-    value: str
-        The convention, matching the Convention enum.
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the convention is invalid
-
-    Also see
-    --------
-    checkIsInEnum
-    Convention
-    '''
-    checkIsInEnum(value, Convention.__members__)
-
-
-def checkCalendar(value) -> None:
-    '''
-    Check if the calendar is valid
-
-    Parameters
-    ----------
-    value: str
-        The calendar, matching the Calendar enum.
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the calendar is invalid
-
-    Also see
-    --------
-    checkIsInEnum
-    Calendar
-    '''
-    checkIsInEnum(value, Calendar.__members__)
-
-
-def checkCurrency(value) -> None:
-    '''
-    Check if the currency is valid
-
-    Parameters
-    ----------
-    value: str
-        The currency, matching the Currency enum.
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the currency is invalid
-
-    Also see
-    --------
-    checkIsInEnum
-    Currency
-    '''
-    checkIsInEnum(value, Currency.__members__)
-
-
-def checkDateGenerationRule(value) -> None:
-    '''
-    Check if the date generation rule is valid
-
-    Parameters
-    ----------
-    value: str
-        The date generation rule, matching the DateGenerationRule enum.
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the date generation rule is invalid
-
-    Also see
-    --------
-    checkIsInEnum
-    DateGenerationRule
-    '''
-    checkIsInEnum(value, DateGenerationRule.__members__)
-
-
-def checkTenor(tenor: str) -> None:
-    '''
-    Check if the tenor is valid
-
-    Parameters
-    ----------
-    tenor: str
-        The tenor, it can be a number followed by D, W, M or Y
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ConfigurationError
-        If the tenor is invalid
-    '''
-    regex = r'^(\d+[DWMY])+$'
-    if not re.match(regex, tenor):
-        raise ValueError(f'The tenor {tenor} is invalid')
-
-
-def checkDictStructure(input: dict, reference: dict) -> None:
-    for key in reference.keys():
-        if key not in input.keys():
-            raise KeyError(
-                f'The required key "{key}" is missing.')
-    for key in input.keys():
-        if key in reference.keys():
-            reference[key](input[key])
-
-
-def checkInstance(value: any, type: type) -> None:
-    '''
-    Check if the value is an instance of the type
-
-    Parameters
-    ----------
-    value: any
-        The value to check
-    type: type
-        The type to check
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValueError
-        If the value is not an instance of the type
-    '''
-
-    if not isinstance(value, type):
-        raise ValueError(f'The value {value} is not an instance of {type}.')
-
-
-## Rate helpers checks ##
-
-def checkOISRateHelper(data: dict) -> None:
-    '''
-    Check if the OIS rate helper is valid
-
-    Parameters
-    ----------
-    data: dict
-        The OIS rate helper
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    RateHelperConfigurationError
-        If the rate helper is invalid
-
-    Details
-    -------
-    The OIS rate helper should have the following example structure:
-    ```
-    "helperConfig": {
-                        "tenor": "1W",
-                        "dayCounter": "Actual360",
-                        "calendar": "NullCalendar",
-                        "convention": "Following",
-                        "endOfMonth": True,
-                        "frequency": "Annual",
-                        "settlementDays": 2,
-                        "paymentLag": 2,
-                        "telescopicValueDates": True,
-                        "index": "SOFR",
-                        "fixedLegFrequency": "Semiannual",
-                        "fwdStart": "0D"
-                    }
-    ```
-    '''
-
-    reference = {
-        "tenor": checkTenor,
-        "dayCounter": checkDayCounter,
-        "calendar": checkCalendar,
-        "convention": checkConvention,
-        "endOfMonth": partial(checkInstance, type=bool),
-        "frequency": checkFrequency,
-        "settlementDays": partial(checkInstance, type=int),
-        "paymentLag": partial(checkInstance, type=int),
-        "telescopicValueDates": partial(checkInstance, type=bool),
-        "index": partial(checkInstance, type=str),
-        "fixedLegFrequency": checkFrequency,
-        "fwdStart": checkTenor
-    }
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateHelperConfigurationError('Invalid OIS rate helper') from exc
-
-
-def checkDepositRateHelper(data: dict) -> None:
-    '''
-    Check if the deposit rate helper is valid
-
-    Parameters
-    ----------
-    data: dict
-        The deposit rate helper
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    RateHelperConfigurationError
-        If the rate helper is invalid
-
-    Details
-    -------
-    The deposit rate helper should have the following example structure:
-    ```
-    "helperConfig": {
-                    "dayCounter": "Actual360",
-                    "tenor": "1D",
-                    "calendar": "NullCalendar",
-                    "settlementDays": 0,
-                    "endOfMonth": False,
-                    "convention": "Unadjusted"
-                }
-    ```
-    '''
-    reference = {
-        "dayCounter": checkDayCounter,
-        "tenor": checkTenor,
-        "calendar": checkCalendar,
-        "settlementDays": partial(checkInstance, type=int),
-        "endOfMonth": partial(checkInstance, type=bool),
-        "convention": checkConvention
-    }
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateHelperConfigurationError(
-            'Invalid deposit rate helper') from exc
-
-
-def checkSwapRateHelper(data: dict) -> None:
-    '''
-    Check if the swap rate helper is valid
-
-    Parameters
-    ----------
-    data: dict
-        The swap rate helper
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    RateHelperConfigurationError
-        If the rate helper is invalid
-
-    Details
-    -------
-    The swap rate helper should have the following example structure:
-    ```
-    "helperConfig": {
-                    "tenor": "2Y",
-                    "dayCounter": "Thirty360",
-                    "calendar": "NullCalendar",
-                    "frequency": "Semiannual",
-                    "settlementDays": 2,
-                    "discountCurve": "SOFR",
-                    "index": "LIBOR3M",
-                    "endOfMonth": False,
-                    "convention": "Unadjusted",
-                    "fixedLegFrequency": "Semiannual",
-                    "fwdStart": "0D"
-                }
-    ```
-    '''
-    reference = {
-        "tenor": checkTenor,
-        "dayCounter": checkDayCounter,
-        "calendar": checkCalendar,
-        "frequency": checkFrequency,
-        "settlementDays": partial(checkInstance, type=int),
-        "discountCurve": partial(checkInstance, type=str),
-        "index": partial(checkInstance, type=str),
-        "endOfMonth": partial(checkInstance, type=bool),
-        "convention": checkConvention,
-        "fixedLegFrequency": checkFrequency,
-        "fwdStart": checkTenor
-    }
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateHelperConfigurationError('Invalid swap rate helper') from exc
-
-
-def checkFixedRateBondRateHelper(data: dict) -> None:
-    '''
-    Check if the bond rate helper is valid
-
-    Parameters
-    ----------
-    data: dict
-        The bond rate helper
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    RateHelperConfigurationError
-        If the rate helper is invalid
-
-    Details
-    -------
-    The bond rate helper should have the following example structure:
-    ```
-    "helperConfig": {
-                    "calendar": "NullCalendar",
-                    "convention": "Following",
-                    "settlementDays": 2,
-                    "couponDayCounter": "Actual360",
-                    "couponRate": 0.05,
-                    "frequency": "Annual",
-                    "startDate": "2020-01-01",
-                    "endDate": "2022-01-01",
-                    "tenor": "2Y" # needed if start date and end date are not provided
-                }
-    ```
-    '''
-    reference = {
-        "calendar": checkCalendar,
-        "convention": checkConvention,
-        "settlementDays": partial(checkInstance, type=int),
-        "couponDayCounter": checkDayCounter,
-        "couponRate": partial(checkInstance, type=float),
-        "frequency": checkFrequency,
-    }
-
-    # check if the start date and end date are provided
-    if "startDate" in data or "endDate" in data:
-        reference["startDate"] = checkDate
-        reference["endDate"] = checkDate
-    else:
-        reference["tenor"] = checkTenor
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateHelperConfigurationError('Invalid bond rate helper') from exc
-
-
-def checkFxSwapRateHelper(data: dict) -> None:
-    '''
-    Check if the FX swap rate helper is valid
-
-    Parameters
-    ----------
-    data: dict
-        The FX swap rate helper
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    RateHelperConfigurationError
-        If the rate helper is invalid
-
-    Details
-    -------
-    The FX swap rate helper should have the following example structure:
-    ```
-    "helperConfig": {
-                        "calendar": "NullCalendar",
-                        "fixingDays": 0,
-                        "endOfMonth": False,
-                        "baseCurrencyAsCollateral": False,
-                        "convention": "Following",
-                        "discountCurve": "CLP_COLLUSD",                       
-                        "endDate": "2023-04-09",
-                        "tenor": "1Y", # need if no end date is provided
-                        "settlementDays": 0
-                    }
-    ```
-    '''
-
-    reference = {
-        "calendar": checkCalendar,
-        "fixingDays": partial(checkInstance, type=int),
-        "endOfMonth": partial(checkInstance, type=bool),
-        "baseCurrencyAsCollateral": partial(checkInstance, type=bool),
-        "convention": checkConvention,
-        "discountCurve": partial(checkInstance, type=str),
-        "settlementDays": partial(checkInstance, type=int)
-    }
-
-    # check if the end date is provided
-    if "endDate" in data:
-        reference["endDate"] = checkDate
-    else:
-        reference["tenor"] = checkTenor
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateHelperConfigurationError(
-            'Invalid FX swap rate helper') from exc
-
-
-def checkCrossCcyFixFloatSwapRateHelper(data: dict) -> None:
-    '''
-    Check if the cross currency rate helper is valid
-
-    Parameters
-    ----------
-    data: dict
-        The cross currency rate helper
-
-    Returns
-    -------
-    None
-        no return, raise RateHelperConfigurationError if the request is invalid
-
-    Raises
-    ------
-    RateHelperConfigurationError
-        If the rate helper is invalid
-
-    Details
-    -------
-    The cross currency rate helper should have the following example structure:
-    ```
-    "helperConfig":  {
-                    "tenor": "2Y",
-                    "dayCounter": "Actual360",
-                    "calendar": "NullCalendar",
-                    "convention": "ModifiedFollowing",
-                    "endOfMonth": False,
-                    "settlementDays": 2,
-                    "discountCurve": "CLP_COLLUSD",
-                    "index": "ICP",
-                    "fixedLegCurrency": "CLF",
-                    "fwdStart": "0D",
-                    "fixedLegFrequency": "Semiannual"
-                }
-    ```
-    '''
-
-    reference = {
-        "tenor": checkTenor,
-        "dayCounter": checkDayCounter,
-        "calendar": checkCalendar,
-        "convention": checkConvention,
-        "endOfMonth": partial(checkInstance, type=bool),
-        "settlementDays": partial(checkInstance, type=int),
-        "discountCurve": partial(checkInstance, type=str),
-        "index": partial(checkInstance, type=str),
-        "fixedLegCurrency": partial(checkInstance, type=str),
-        "fwdStart": checkTenor,
-        "fixedLegFrequency": checkFrequency
-    }
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateHelperConfigurationError(
-            'Invalid cross currency rate helper') from exc
-
-
-def checkTenorBasisSwapRateHelper(data: dict) -> None:
-    '''
-    Check if the tenor basis rate helper is valid
-
-    Parameters
-    ----------
-    data: dict
-        The tenor basis rate helper
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    RateHelperConfigurationError
-        If the rate helper is invalid
-
-    Details
-    -------
-    The tenor basis rate helper should have the following example structure:
-    ```
-    "helperConfig": {
-                    "tenor": "3M",
-                    "longIndex": "LIBOR3M",
-                    "shortIndex": "LIBOR1M",
-                    "discountCurve": "SOFR",
-                    "spreadOnShort": True
-                }
-    ```
-    '''
-
-    reference = {
-        "tenor": checkTenor,
-        "longIndex": partial(checkInstance, type=str),
-        "shortIndex": partial(checkInstance, type=str),
-        "discountCurve": partial(checkInstance, type=str),
-        "spreadOnShort": partial(checkInstance, type=bool)
-    }
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateHelperConfigurationError(
-            'Invalid tenor basis rate helper') from exc
-
-
-def checkCrossCcyBasisSwapRateHelper(data: dict) -> None:
-    '''
-    Check if the cross currency basis rate helper is valid
-
-    Parameters
-    ----------
-    data: dict
-        The cross currency basis rate helper
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    RateHelperConfigurationError
-        If the rate helper is invalid
-
-    Details
-    -------
-    The cross currency basis rate helper should have the following example structure:
-    ```
-    "helperConfig": {
-                    "tenor": "3M",
-                    "calendar": "NullCalendar",
-                    "settlementDays": 2,
-                    "endOfMonth": False,
-                    "convention": "ModifiedFollowing",
-                    "flatIndex": "LIBOR3M",
-                    "spreadIndex": "LIBOR1M",
-                    "discountCurve": "SOFR"
-                }
-    ```
-    '''
-
-    reference = {
-        "tenor": checkTenor,
-        "calendar": checkCalendar,
-        "settlementDays": partial(checkInstance, type=int),
-        "endOfMonth": partial(checkInstance, type=bool),
-        "convention": checkConvention,
-        "flatIndex": partial(checkInstance, type=str),
-        "spreadIndex": partial(checkInstance, type=str),
-        "discountCurve": partial(checkInstance, type=str),
-    }
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateHelperConfigurationError(
-            'Invalid cross currency basis rate helper') from exc
-
-
-def checkMarketConfig(data: dict, helperType: HelperType) -> None:
-    '''
-    Check if the market config is valid
-
-    Parameters
-    ----------
-    data: dict
-        The market config
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ConfigurationError
-        If the market config is invalid
-
-    Details
-    -------
-    The market config should have the following example structure:
-    ```
-    "marketConfig": {
-                        "rate": {
-                            "ticker" : "CLP_CU",
-                            "value" : 0.01
-                        },
-                        "spread": {
-                            "ticker" : "CLP_CU",
-                            "value" : 0.01
-                        },
-                        "fxSpot": {
-                            "ticker" : "CLP_CU",
-                            "value" : 0.01
-                        },
-                        "fxPoints": {
-                            "ticker" : "CLP_CU",
-                            "value" : 0.01
-                        }
-                    }
-    ```
-
-    Where each field has at least a value. The ticker is optional.    
-    Each field is dependent on the helper type. The following table shows the required fields for each helper type:
-
-    |Helper type             | Required fields                  |
-    |----------------------- | ---------------------------------|
-    |Deposit                 | rate                             |
-    |Swap                    | rate, spread                     |    
-    |FxSwap                  | fxSpot, fxPoints                 |    
-    |Xccy                    | rate, spread, fxSpot             |
-    |TenorBasis              | spread                           |
-    |XccyBasis               | spread, fxSpot, fxPoints         |
-    |OIS                     | spread                           |
-    |Bond                    | rate                             |
-    '''
-
-    def checkPrice(data: dict) -> None:
-        if not isinstance(data, dict):
-            raise ConfigurationError(
-                'Invalid price, should be a dictionary')
-        if 'value' not in data:
-            raise ConfigurationError(
-                'Invalid price, missing value')
-        if not isinstance(data['value'], float) and not isinstance(data['value'], int):
-            raise ConfigurationError(
-                'Invalid price, value should be a float or int')
-        if 'ticker' in data and not isinstance(data['ticker'], str):
-            raise ConfigurationError(
-                'Invalid price, ticker should be a string')
-
-    reference = {}
-    if helperType == HelperType.Deposit:
-        reference = {
-            "rate": checkPrice
-        }
-    elif helperType == HelperType.Swap:
-        reference = {
-            "rate": checkPrice,
-            "spread": checkPrice
-        }
-    elif helperType == HelperType.FxSwap:
-        reference = {
-            "fxSpot": checkPrice,
-            "fxPoints": checkPrice
-        }
-    elif helperType == HelperType.Xccy:
-        reference = {
-            "rate": checkPrice,
-            "spread": checkPrice,
-            "fxSpot": checkPrice,            
-        }
-    elif helperType == HelperType.TenorBasis:
-        reference = {
-            "spread": checkPrice
-        }
-    elif helperType == HelperType.XccyBasis:
-        reference = {
-            "spread": checkPrice,
-            "fxSpot": checkPrice,
-            "fxPoints": checkPrice
-        }
-    elif helperType == HelperType.OIS:
-        reference = {
-            "spread": checkPrice
-        }
-    elif helperType == HelperType.Bond:
-        reference = {
-            "rate": checkPrice
-        }
-    else:
-        raise ConfigurationError('Invalid helper type')
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise ConfigurationError(
-            'Invalid market config') from exc
-
-
-def checkRateHelper(data: dict, pos: int) -> None:
-    '''
-    Check if the rate helper is valid
-
-    Parameters
-    ----------
-    data: dict
-        The rate helper
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    RateHelperConfigurationError
-        If the rate helper is invalid
-
-    Details
-    -------
-    The rate helper should have the following example structure:
-    ```
-    "rateHelper": {
-                        "helperType": "OIS",
-                        "helperConfig": {
-                           ...
-                        },
-                        "marketConfig": {
-                            ...
-                        }
-                    }
-    ```
-    '''
-
-    reference = {
-        "helperType": partial(checkIsInEnum, enum=[r.value for r in HelperType]),
-    }
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise ConfigurationError(
-            'Invalid rate helper configuration or helper type at pos {}'.format(pos)) from exc
-
-    helperType = HelperType[data['helperType']]
-
-    reference["marketConfig"] = partial(
-        checkMarketConfig, helperType=helperType)
-    if helperType == HelperType.Deposit:
-        reference["helperConfig"] = checkDepositRateHelper
-    elif helperType == HelperType.Swap:
-        reference["helperConfig"] = checkSwapRateHelper
-    elif helperType == HelperType.FxSwap:
-        reference["helperConfig"] = checkFxSwapRateHelper
-    elif helperType == HelperType.Xccy:
-        reference["helperConfig"] = checkCrossCcyFixFloatSwapRateHelper
-    elif helperType == HelperType.TenorBasis:
-        reference["helperConfig"] = checkTenorBasisSwapRateHelper
-    elif helperType == HelperType.XccyBasis:
-        reference["helperConfig"] = checkCrossCcyBasisSwapRateHelper
-    elif helperType == HelperType.OIS:
-        reference["helperConfig"] = checkOISRateHelper
-    elif helperType == HelperType.Bond:
-        reference["helperConfig"] = checkFixedRateBondRateHelper
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateHelperConfigurationError(
-            'Invalid rate helper {} configuration at pos {}'.format(helperType, pos)) from exc
-    
-
-
-## Index checks ##
-
-
-def checkIndex(data: dict) -> None:
-    '''
-    Check if the index is valid
-
-    Parameters
-    ----------
-    data: dict
-        The index
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    RateIndexError
-        If the index is invalid
-
-    Details
-    -------
-    The index should have the following example structure:
-    ```
-    "curveIndex": {
-                "indexType": "IborIndex",
-                "tenor": "6M",
-                "dayCounter": "Actual360",
-                "currency": "CLP",
-                "fixingDays": 0,
-                "calendar": "NullCalendar",
-                "endOfMonth": False,
-                "convention": "Unadjusted"
-            }
-    ```
-    '''
-
-    reference = {
-        "indexType": partial(checkIsInEnum, enum=IndexType.__members__),
-        "tenor": checkTenor,
-        "dayCounter": checkDayCounter,
-        "currency": checkCurrency,
-        "fixingDays": partial(checkInstance, type=int),
-        "calendar": checkCalendar,
-        "endOfMonth": partial(checkInstance, type=bool),
-        "convention": checkConvention
-    }
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise RateIndexError('Invalid index configuration') from exc
-
-
-## Curve checks ##
-
-def checkPiecewiseCurve(data: dict) -> None:
-    '''
-    Check if the piecewise curve is valid
-
-    Parameters
-    ----------
-    data: dict
-        The piecewise curve
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    InvalidCurve
-        If the curve is invalid
-
-    Details
-    -------
-    The piecewise curve should have the following example structure:
-
-    ```
-    "example": {
-            "curveType": "Piecewise",
-            "dayCounter": "Actual360",
-            "enableExtrapolation": True,
-            "rateHelpers": [
-                ...
-            ]
-        }
-    ```
-    '''
-    def checkRateHelperList(l: list) -> None:
-        checkInstance(l, type=list)
-        if len(l) == 0:
-            raise ConfigurationError(
-                'Invalid piecewise curve configuration, rateHelpers should not be empty')
-        for pos, helper in enumerate(l):
-            checkRateHelper(helper, pos)
-
-    reference = {
-        "curveType": partial(checkIsInEnum, enum=[r.value for r in CurveType]),
-        "dayCounter": checkDayCounter,
-        "enableExtrapolation": partial(checkInstance, type=bool),
-        "rateHelpers": checkRateHelperList
-    }
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise ConfigurationError(
-            'Invalid piecewise curve configuration') from exc
-
-
-def checkDiscountCurve(data: dict) -> None:
-    '''
-    Check if the discount curve is valid
-
-    Parameters
-    ----------
-    data: dict
-        The discount curve
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    InvalidCurve
-        If the curve is invalid
-
-    Details
-    -------
-    The discount curve should have the following example structure:
-
-    ```
-    "example": {
-            "curveType": "Discount",
-            "dayCounter": "Actual360",
-            "enableExtrapolation": True,
-            "nodes": [
-                {
-                    "date": "2020-01-01",
-                    "value": 0.99
-                }
-            ]
-        }
-    ```
-    '''
-    def checkNodeList(l: list) -> None:
-        ref = {
-            "date": checkDate,
-            "value": partial(checkInstance, type=float)
-        }
-        checkInstance(l, type=list)
-        if len(l) == 0:
-            raise ConfigurationError(
-                'Invalid discount curve configuration, discountFactors should not be empty')
-        for node in l:
-            checkDictStructure(node, ref)
-
-    reference = {
-        "curveType": partial(checkIsInEnum, enum=[r.value for r in CurveType]),
-        "dayCounter": checkDayCounter,
-        "enableExtrapolation": partial(checkInstance, type=bool),
-        "nodes": checkNodeList
-    }
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise ConfigurationError(
-            'Invalid discount curve configuration') from exc
-
-
-def checkCurve(data: dict, pos: int) -> None:
-    '''
-    Check if the curve is valid
-
-    Parameters
-    ----------
-    data: dict
-        The curve
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ConfigurationError
-        If the curve is invalid
-
-    Details
-    -------
-    The curve should have the following example structure:
-
-    ```
-    "curve": {
-        "curveName": "CLP",
-        "curveConfig": {
-            "curveType": "Piecewise",
-            "dayCounter": "Actual360",
-            "enableExtrapolation": True,
-            "rateHelpers": []   # if curveType is Piecewise, otherwise nodes             
-
-        },
-        "curveIndex": {}
-    }
-    ```
-    '''
-    def checkBaseCurve(dict: dict) -> None:
-        if "curveType" not in dict:
-            raise ConfigurationError(
-                'Invalid curve configuration, curveType should be defined')
-        if dict["curveType"] == CurveType.Piecewise.value:
-            checkPiecewiseCurve(dict)
-        elif dict["curveType"] == CurveType.Discount.value:
-            checkDiscountCurve(dict)
-        else:
-            raise ConfigurationError(
-                'Invalid curve configuration, curveType should be Piecewise or Discount')
-
-    reference = {
-        "curveName": partial(checkInstance, type=str),
-        "curveConfig": checkBaseCurve,
-        "curveIndex": checkIndex
-    }
-
-    try:
-        checkDictStructure(data, reference)
-    except ConfigurationError as exc:
-        raise ConfigurationError(
-            'Invalid curve configuration for {} curve'.format(data['curveName'])) from exc
-    except Exception as exc:
-        raise ConfigurationError('Invalid curve configuration at pos {}'.format(pos)) from exc
-
-
-def checkConfiguration(data: dict) -> None:
-    '''
-    Check if the configuration is valid
-
-    Parameters
-    ----------
-    data: dict
-        The configuration
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ConfigurationError
-        If the configuration is invalid
-
-    Details
-    -------
-    The configuration should have the following example structure:
-
-    ```
-    "configuration": {
-        "refDate": "2020-01-01",
-        "curves": [
-                {
-                    "curveName": "CLP",
-                    "curveConfig": {
-                        "curveType": "Piecewise",
-                        "dayCounter": "Actual360",
-                        "enableExtrapolation": True,
-                        "rateHelpers": [
-                            ...
-                            ]
-                        },
-                    "curveIndex": {
-                        ...
-                    }
-                }
-            ]
-        }        
-    }
-    ```
-    '''
-    def checkCurveList(l: list) -> None:
-        checkInstance(l, type=list)
-        if len(l) == 0:
-            raise ConfigurationError(
-                'Invalid configuration, curves should not be empty')
-        for pos, curve in enumerate(l):
-            checkCurve(curve, pos)
-
-    reference = {
-        "refDate": checkDate,
-        "curves": checkCurveList
-    }
-
-    try:
-        checkDictStructure(data, reference)
-    except Exception as exc:
-        raise ConfigurationError('Invalid configuration') from exc
+import re
+from functools import partial
+from .enums import *
+
+'''
+Example of a basic structure of the curve request:
+{
+    "refDate": "2020-01-01",
+    "curves": [
+        {
+            "curveName": "PiecewiseCurveExample",
+            "curveConfig": {
+                "curveType": "Piecewise",                
+                "dayCounter": "Actual360",
+                "enableExtrapolation": True,
+                "rateHelpers": [
+                    {                        
+                        "helperConfig": {
+                            ...
+                        },
+                        "marketConfig": {
+                            ...
+                        },
+                    }
+                ]
+            },
+            "curveIndex":{
+                ...
+            }
+        },
+        {
+            "curveName": "DiscountCurveExample",
+            "curveConfig": {
+                "curveType": "Discount",
+                "dayCounter": "Actual360",
+                "enableExtrapolation": True,
+                "nodes": [
+                    {
+                        "date": "2020-01-01",
+                        "discount": 0.01
+                    },
+                    {
+                        "date": "2020-02-01",
+                        "discount": 0.02
+                    }
+                ]
+            },
+            "curveIndex":{
+                ...
+            }
+        }
+    ]
+}
+'''
+
+
+class ConfigurationError(Exception):
+    '''
+    Exception raised when the request is invalid
+    '''
+
+    def __init__(self, message):
+        self.message = message
+
+
+class RateIndexError(ConfigurationError):
+    '''
+    Exception raised when the index is invalid
+    '''
+
+    def __init__(self, message):
+        self.message = message
+
+
+class RateHelperConfigurationError(ConfigurationError):
+    '''
+    Exception raised when the rate helper is invalid
+    '''
+
+    def __init__(self, message):
+        self.message = message
+
+
+class MarketConfigurationError(ConfigurationError):
+    '''
+    Exception raised when the market configuration is invalid
+    '''
+
+    def __init__(self, message):
+        self.message = message
+
+
+## Check available enums and possible instances#
+
+
+def checkDate(value) -> None:
+    '''
+    Check if the date is valid
+
+    Parameters
+    ----------
+    value: str
+        The date
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the date is invalid
+    '''
+    if not re.match(r'^\d{4}-\d{2}-\d{2}(T\d{2}:\d{2}:\d{2}(\.\d{1,6})?(Z|[+-]\d{2}:\d{2})?)?$', value):
+        raise ValueError(f'{value} is not a valid date or it does not follow the ISO format.')
+
+
+def checkIsInEnum(value: str, enum: list) -> None:
+    '''
+    Check if the value is in the enum
+
+    Parameters
+    ----------
+    value: str
+        The value to check
+    enum: list
+        The enum
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the value is not in the enum
+    '''
+    if value not in enum:
+        raise ValueError(f'{value} is not in {enum}')
+
+
+def checkDayCounter(value) -> None:
+    '''
+    Check if the day counter is valid
+
+    Parameters
+    ----------
+    value: str
+        The day counter. It must match the DayCounter enum.
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the day counter is invalid
+
+    Also see
+    --------
+    checkIsInEnum
+    DayCounter
+
+    '''
+    checkIsInEnum(value, DayCounter.__members__)
+
+
+def checkFrequency(value) -> None:
+    '''
+    Check if the frequency is valid
+
+    Parameters
+    ----------
+    value: str
+        The frequency, matching the Frequency enum.
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the frequency is invalid
+
+    Also see
+    --------
+    checkIsInEnum
+    Frequency
+    '''
+    checkIsInEnum(value, Frequency.__members__)
+
+
+def checkCompounding(value) -> None:
+    '''
+    Check if the compounding is valid
+
+    Parameters
+    ----------
+    value: str
+        The compounding, matching the Compounding enum.
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the compounding is invalid
+
+    Also see
+    --------
+    checkIsInEnum
+    Compounding
+    '''
+    checkIsInEnum(value, Compounding.__members__)
+
+
+def checkConvention(value) -> None:
+    '''
+    Check if the convention is valid
+
+    Parameters
+    ----------
+    value: str
+        The convention, matching the Convention enum.
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the convention is invalid
+
+    Also see
+    --------
+    checkIsInEnum
+    Convention
+    '''
+    checkIsInEnum(value, Convention.__members__)
+
+
+def checkCalendar(value) -> None:
+    '''
+    Check if the calendar is valid
+
+    Parameters
+    ----------
+    value: str
+        The calendar, matching the Calendar enum.
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the calendar is invalid
+
+    Also see
+    --------
+    checkIsInEnum
+    Calendar
+    '''
+    checkIsInEnum(value, Calendar.__members__)
+
+
+def checkCurrency(value) -> None:
+    '''
+    Check if the currency is valid
+
+    Parameters
+    ----------
+    value: str
+        The currency, matching the Currency enum.
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the currency is invalid
+
+    Also see
+    --------
+    checkIsInEnum
+    Currency
+    '''
+    checkIsInEnum(value, Currency.__members__)
+
+
+def checkDateGenerationRule(value) -> None:
+    '''
+    Check if the date generation rule is valid
+
+    Parameters
+    ----------
+    value: str
+        The date generation rule, matching the DateGenerationRule enum.
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the date generation rule is invalid
+
+    Also see
+    --------
+    checkIsInEnum
+    DateGenerationRule
+    '''
+    checkIsInEnum(value, DateGenerationRule.__members__)
+
+
+def checkTenor(tenor: str) -> None:
+    '''
+    Check if the tenor is valid
+
+    Parameters
+    ----------
+    tenor: str
+        The tenor, it can be a number followed by D, W, M or Y
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ConfigurationError
+        If the tenor is invalid
+    '''
+    regex = r'^(\d+[DWMY])+$'
+    if not re.match(regex, tenor):
+        raise ValueError(f'The tenor {tenor} is invalid')
+
+
+def checkDictStructure(input: dict, reference: dict) -> None:
+    for key in reference.keys():
+        if key not in input.keys():
+            raise KeyError(
+                f'The required key "{key}" is missing.')
+    for key in input.keys():
+        if key in reference.keys():
+            reference[key](input[key])
+
+
+def checkInstance(value: any, type: type) -> None:
+    '''
+    Check if the value is an instance of the type
+
+    Parameters
+    ----------
+    value: any
+        The value to check
+    type: type
+        The type to check
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the value is not an instance of the type
+    '''
+
+    if not isinstance(value, type):
+        raise ValueError(f'The value {value} is not an instance of {type}.')
+
+
+## Rate helpers checks ##
+
+def checkOISRateHelper(data: dict) -> None:
+    '''
+    Check if the OIS rate helper is valid
+
+    Parameters
+    ----------
+    data: dict
+        The OIS rate helper
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    RateHelperConfigurationError
+        If the rate helper is invalid
+
+    Details
+    -------
+    The OIS rate helper should have the following example structure:
+    ```
+    "helperConfig": {
+                        "tenor": "1W",
+                        "dayCounter": "Actual360",
+                        "calendar": "NullCalendar",
+                        "convention": "Following",
+                        "endOfMonth": True,
+                        "frequency": "Annual",
+                        "settlementDays": 2,
+                        "paymentLag": 2,
+                        "telescopicValueDates": True,
+                        "index": "SOFR",
+                        "fixedLegFrequency": "Semiannual",
+                        "fwdStart": "0D"
+                    }
+    ```
+    '''
+
+    reference = {
+        "tenor": checkTenor,
+        "dayCounter": checkDayCounter,
+        "calendar": checkCalendar,
+        "convention": checkConvention,
+        "endOfMonth": partial(checkInstance, type=bool),
+        "frequency": checkFrequency,
+        "settlementDays": partial(checkInstance, type=int),
+        "paymentLag": partial(checkInstance, type=int),
+        "telescopicValueDates": partial(checkInstance, type=bool),
+        "index": partial(checkInstance, type=str),
+        "fixedLegFrequency": checkFrequency,
+        "fwdStart": checkTenor
+    }
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateHelperConfigurationError('Invalid OIS rate helper') from exc
+
+
+def checkDepositRateHelper(data: dict) -> None:
+    '''
+    Check if the deposit rate helper is valid
+
+    Parameters
+    ----------
+    data: dict
+        The deposit rate helper
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    RateHelperConfigurationError
+        If the rate helper is invalid
+
+    Details
+    -------
+    The deposit rate helper should have the following example structure:
+    ```
+    "helperConfig": {
+                    "dayCounter": "Actual360",
+                    "tenor": "1D",
+                    "calendar": "NullCalendar",
+                    "settlementDays": 0,
+                    "endOfMonth": False,
+                    "convention": "Unadjusted"
+                }
+    ```
+    '''
+    reference = {
+        "dayCounter": checkDayCounter,
+        "tenor": checkTenor,
+        "calendar": checkCalendar,
+        "settlementDays": partial(checkInstance, type=int),
+        "endOfMonth": partial(checkInstance, type=bool),
+        "convention": checkConvention
+    }
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateHelperConfigurationError(
+            'Invalid deposit rate helper') from exc
+
+
+def checkSwapRateHelper(data: dict) -> None:
+    '''
+    Check if the swap rate helper is valid
+
+    Parameters
+    ----------
+    data: dict
+        The swap rate helper
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    RateHelperConfigurationError
+        If the rate helper is invalid
+
+    Details
+    -------
+    The swap rate helper should have the following example structure:
+    ```
+    "helperConfig": {
+                    "tenor": "2Y",
+                    "dayCounter": "Thirty360",
+                    "calendar": "NullCalendar",
+                    "frequency": "Semiannual",
+                    "settlementDays": 2,
+                    "discountCurve": "SOFR",
+                    "index": "LIBOR3M",
+                    "endOfMonth": False,
+                    "convention": "Unadjusted",
+                    "fixedLegFrequency": "Semiannual",
+                    "fwdStart": "0D"
+                }
+    ```
+    '''
+    reference = {
+        "tenor": checkTenor,
+        "dayCounter": checkDayCounter,
+        "calendar": checkCalendar,
+        "frequency": checkFrequency,
+        "settlementDays": partial(checkInstance, type=int),
+        "discountCurve": partial(checkInstance, type=str),
+        "index": partial(checkInstance, type=str),
+        "endOfMonth": partial(checkInstance, type=bool),
+        "convention": checkConvention,
+        "fixedLegFrequency": checkFrequency,
+        "fwdStart": checkTenor
+    }
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateHelperConfigurationError('Invalid swap rate helper') from exc
+
+
+def checkFixedRateBondRateHelper(data: dict) -> None:
+    '''
+    Check if the bond rate helper is valid
+
+    Parameters
+    ----------
+    data: dict
+        The bond rate helper
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    RateHelperConfigurationError
+        If the rate helper is invalid
+
+    Details
+    -------
+    The bond rate helper should have the following example structure:
+    ```
+    "helperConfig": {
+                    "calendar": "NullCalendar",
+                    "convention": "Following",
+                    "settlementDays": 2,
+                    "couponDayCounter": "Actual360",
+                    "couponRate": 0.05,
+                    "frequency": "Annual",
+                    "startDate": "2020-01-01",
+                    "endDate": "2022-01-01",
+                    "tenor": "2Y" # needed if start date and end date are not provided
+                }
+    ```
+    '''
+    reference = {
+        "calendar": checkCalendar,
+        "convention": checkConvention,
+        "settlementDays": partial(checkInstance, type=int),
+        "couponDayCounter": checkDayCounter,
+        "couponRate": partial(checkInstance, type=float),
+        "frequency": checkFrequency,
+    }
+
+    # check if the start date and end date are provided
+    if "startDate" in data or "endDate" in data:
+        reference["startDate"] = checkDate
+        reference["endDate"] = checkDate
+    else:
+        reference["tenor"] = checkTenor
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateHelperConfigurationError('Invalid bond rate helper') from exc
+
+
+def checkFxSwapRateHelper(data: dict) -> None:
+    '''
+    Check if the FX swap rate helper is valid
+
+    Parameters
+    ----------
+    data: dict
+        The FX swap rate helper
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    RateHelperConfigurationError
+        If the rate helper is invalid
+
+    Details
+    -------
+    The FX swap rate helper should have the following example structure:
+    ```
+    "helperConfig": {
+                        "calendar": "NullCalendar",
+                        "fixingDays": 0,
+                        "endOfMonth": False,
+                        "baseCurrencyAsCollateral": False,
+                        "convention": "Following",
+                        "discountCurve": "CLP_COLLUSD",                       
+                        "endDate": "2023-04-09",
+                        "tenor": "1Y", # need if no end date is provided
+                        "settlementDays": 0
+                    }
+    ```
+    '''
+
+    reference = {
+        "calendar": checkCalendar,
+        "fixingDays": partial(checkInstance, type=int),
+        "endOfMonth": partial(checkInstance, type=bool),
+        "baseCurrencyAsCollateral": partial(checkInstance, type=bool),
+        "convention": checkConvention,
+        "discountCurve": partial(checkInstance, type=str),
+        "settlementDays": partial(checkInstance, type=int)
+    }
+
+    # check if the end date is provided
+    if "endDate" in data:
+        reference["endDate"] = checkDate
+    else:
+        reference["tenor"] = checkTenor
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateHelperConfigurationError(
+            'Invalid FX swap rate helper') from exc
+
+
+def checkCrossCcyFixFloatSwapRateHelper(data: dict) -> None:
+    '''
+    Check if the cross currency rate helper is valid
+
+    Parameters
+    ----------
+    data: dict
+        The cross currency rate helper
+
+    Returns
+    -------
+    None
+        no return, raise RateHelperConfigurationError if the request is invalid
+
+    Raises
+    ------
+    RateHelperConfigurationError
+        If the rate helper is invalid
+
+    Details
+    -------
+    The cross currency rate helper should have the following example structure:
+    ```
+    "helperConfig":  {
+                    "tenor": "2Y",
+                    "dayCounter": "Actual360",
+                    "calendar": "NullCalendar",
+                    "convention": "ModifiedFollowing",
+                    "endOfMonth": False,
+                    "settlementDays": 2,
+                    "discountCurve": "CLP_COLLUSD",
+                    "index": "ICP",
+                    "fixedLegCurrency": "CLF",
+                    "fwdStart": "0D",
+                    "fixedLegFrequency": "Semiannual"
+                }
+    ```
+    '''
+
+    reference = {
+        "tenor": checkTenor,
+        "dayCounter": checkDayCounter,
+        "calendar": checkCalendar,
+        "convention": checkConvention,
+        "endOfMonth": partial(checkInstance, type=bool),
+        "settlementDays": partial(checkInstance, type=int),
+        "discountCurve": partial(checkInstance, type=str),
+        "index": partial(checkInstance, type=str),
+        "fixedLegCurrency": partial(checkInstance, type=str),
+        "fwdStart": checkTenor,
+        "fixedLegFrequency": checkFrequency
+    }
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateHelperConfigurationError(
+            'Invalid cross currency rate helper') from exc
+
+
+def checkTenorBasisSwapRateHelper(data: dict) -> None:
+    '''
+    Check if the tenor basis rate helper is valid
+
+    Parameters
+    ----------
+    data: dict
+        The tenor basis rate helper
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    RateHelperConfigurationError
+        If the rate helper is invalid
+
+    Details
+    -------
+    The tenor basis rate helper should have the following example structure:
+    ```
+    "helperConfig": {
+                    "tenor": "3M",
+                    "longIndex": "LIBOR3M",
+                    "shortIndex": "LIBOR1M",
+                    "discountCurve": "SOFR",
+                    "spreadOnShort": True
+                }
+    ```
+    '''
+
+    reference = {
+        "tenor": checkTenor,
+        "longIndex": partial(checkInstance, type=str),
+        "shortIndex": partial(checkInstance, type=str),
+        "discountCurve": partial(checkInstance, type=str),
+        "spreadOnShort": partial(checkInstance, type=bool)
+    }
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateHelperConfigurationError(
+            'Invalid tenor basis rate helper') from exc
+
+
+def checkCrossCcyBasisSwapRateHelper(data: dict) -> None:
+    '''
+    Check if the cross currency basis rate helper is valid
+
+    Parameters
+    ----------
+    data: dict
+        The cross currency basis rate helper
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    RateHelperConfigurationError
+        If the rate helper is invalid
+
+    Details
+    -------
+    The cross currency basis rate helper should have the following example structure:
+    ```
+    "helperConfig": {
+                    "tenor": "3M",
+                    "calendar": "NullCalendar",
+                    "settlementDays": 2,
+                    "endOfMonth": False,
+                    "convention": "ModifiedFollowing",
+                    "flatIndex": "LIBOR3M",
+                    "spreadIndex": "LIBOR1M",
+                    "discountCurve": "SOFR"
+                }
+    ```
+    '''
+
+    reference = {
+        "tenor": checkTenor,
+        "calendar": checkCalendar,
+        "settlementDays": partial(checkInstance, type=int),
+        "endOfMonth": partial(checkInstance, type=bool),
+        "convention": checkConvention,
+        "flatIndex": partial(checkInstance, type=str),
+        "spreadIndex": partial(checkInstance, type=str),
+        "discountCurve": partial(checkInstance, type=str),
+    }
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateHelperConfigurationError(
+            'Invalid cross currency basis rate helper') from exc
+
+
+def checkMarketConfig(data: dict, helperType: HelperType) -> None:
+    '''
+    Check if the market config is valid
+
+    Parameters
+    ----------
+    data: dict
+        The market config
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ConfigurationError
+        If the market config is invalid
+
+    Details
+    -------
+    The market config should have the following example structure:
+    ```
+    "marketConfig": {
+                        "rate": {
+                            "ticker" : "CLP_CU",
+                            "value" : 0.01
+                        },
+                        "spread": {
+                            "ticker" : "CLP_CU",
+                            "value" : 0.01
+                        },
+                        "fxSpot": {
+                            "ticker" : "CLP_CU",
+                            "value" : 0.01
+                        },
+                        "fxPoints": {
+                            "ticker" : "CLP_CU",
+                            "value" : 0.01
+                        }
+                    }
+    ```
+
+    Where each field has at least a value. The ticker is optional.    
+    Each field is dependent on the helper type. The following table shows the required fields for each helper type:
+
+    |Helper type             | Required fields                  |
+    |----------------------- | ---------------------------------|
+    |Deposit                 | rate                             |
+    |Swap                    | rate, spread                     |    
+    |FxSwap                  | fxSpot, fxPoints                 |    
+    |Xccy                    | rate, spread, fxSpot             |
+    |TenorBasis              | spread                           |
+    |XccyBasis               | spread, fxSpot, fxPoints         |
+    |OIS                     | spread                           |
+    |Bond                    | rate                             |
+    '''
+
+    def checkPrice(data: dict) -> None:
+        if not isinstance(data, dict):
+            raise ConfigurationError(
+                'Invalid price, should be a dictionary')
+        if 'value' not in data:
+            raise ConfigurationError(
+                'Invalid price, missing value')
+        if not isinstance(data['value'], float) and not isinstance(data['value'], int):
+            raise ConfigurationError(
+                'Invalid price, value should be a float or int')
+        if 'ticker' in data and not isinstance(data['ticker'], str):
+            raise ConfigurationError(
+                'Invalid price, ticker should be a string')
+
+    reference = {}
+    if helperType == HelperType.Deposit:
+        reference = {
+            "rate": checkPrice
+        }
+    elif helperType == HelperType.Swap:
+        reference = {
+            "rate": checkPrice,
+            "spread": checkPrice
+        }
+    elif helperType == HelperType.FxSwap:
+        reference = {
+            "fxSpot": checkPrice,
+            "fxPoints": checkPrice
+        }
+    elif helperType == HelperType.Xccy:
+        reference = {
+            "rate": checkPrice,
+            "spread": checkPrice,
+            "fxSpot": checkPrice,            
+        }
+    elif helperType == HelperType.TenorBasis:
+        reference = {
+            "spread": checkPrice
+        }
+    elif helperType == HelperType.XccyBasis:
+        reference = {
+            "spread": checkPrice,
+            "fxSpot": checkPrice,
+            "fxPoints": checkPrice
+        }
+    elif helperType == HelperType.OIS:
+        reference = {
+            "spread": checkPrice
+        }
+    elif helperType == HelperType.Bond:
+        reference = {
+            "rate": checkPrice
+        }
+    else:
+        raise ConfigurationError('Invalid helper type')
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise ConfigurationError(
+            'Invalid market config') from exc
+
+
+def checkRateHelper(data: dict, pos: int) -> None:
+    '''
+    Check if the rate helper is valid
+
+    Parameters
+    ----------
+    data: dict
+        The rate helper
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    RateHelperConfigurationError
+        If the rate helper is invalid
+
+    Details
+    -------
+    The rate helper should have the following example structure:
+    ```
+    "rateHelper": {
+                        "helperType": "OIS",
+                        "helperConfig": {
+                           ...
+                        },
+                        "marketConfig": {
+                            ...
+                        }
+                    }
+    ```
+    '''
+
+    reference = {
+        "helperType": partial(checkIsInEnum, enum=[r.value for r in HelperType]),
+    }
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise ConfigurationError(
+            'Invalid rate helper configuration or helper type at pos {}'.format(pos)) from exc
+
+    helperType = HelperType[data['helperType']]
+
+    reference["marketConfig"] = partial(
+        checkMarketConfig, helperType=helperType)
+    if helperType == HelperType.Deposit:
+        reference["helperConfig"] = checkDepositRateHelper
+    elif helperType == HelperType.Swap:
+        reference["helperConfig"] = checkSwapRateHelper
+    elif helperType == HelperType.FxSwap:
+        reference["helperConfig"] = checkFxSwapRateHelper
+    elif helperType == HelperType.Xccy:
+        reference["helperConfig"] = checkCrossCcyFixFloatSwapRateHelper
+    elif helperType == HelperType.TenorBasis:
+        reference["helperConfig"] = checkTenorBasisSwapRateHelper
+    elif helperType == HelperType.XccyBasis:
+        reference["helperConfig"] = checkCrossCcyBasisSwapRateHelper
+    elif helperType == HelperType.OIS:
+        reference["helperConfig"] = checkOISRateHelper
+    elif helperType == HelperType.Bond:
+        reference["helperConfig"] = checkFixedRateBondRateHelper
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateHelperConfigurationError(
+            'Invalid rate helper {} configuration at pos {}'.format(helperType, pos)) from exc
+    
+
+
+## Index checks ##
+
+
+def checkIndex(data: dict) -> None:
+    '''
+    Check if the index is valid
+
+    Parameters
+    ----------
+    data: dict
+        The index
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    RateIndexError
+        If the index is invalid
+
+    Details
+    -------
+    The index should have the following example structure:
+    ```
+    "curveIndex": {
+                "indexType": "IborIndex",
+                "tenor": "6M",
+                "dayCounter": "Actual360",
+                "currency": "CLP",
+                "fixingDays": 0,
+                "calendar": "NullCalendar",
+                "endOfMonth": False,
+                "convention": "Unadjusted"
+            }
+    ```
+    '''
+
+    reference = {
+        "indexType": partial(checkIsInEnum, enum=IndexType.__members__),
+        "tenor": checkTenor,
+        "dayCounter": checkDayCounter,
+        "currency": checkCurrency,
+        "fixingDays": partial(checkInstance, type=int),
+        "calendar": checkCalendar,
+        "endOfMonth": partial(checkInstance, type=bool),
+        "convention": checkConvention
+    }
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise RateIndexError('Invalid index configuration') from exc
+
+
+## Curve checks ##
+
+def checkPiecewiseCurve(data: dict) -> None:
+    '''
+    Check if the piecewise curve is valid
+
+    Parameters
+    ----------
+    data: dict
+        The piecewise curve
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    InvalidCurve
+        If the curve is invalid
+
+    Details
+    -------
+    The piecewise curve should have the following example structure:
+
+    ```
+    "example": {
+            "curveType": "Piecewise",
+            "dayCounter": "Actual360",
+            "enableExtrapolation": True,
+            "rateHelpers": [
+                ...
+            ]
+        }
+    ```
+    '''
+    def checkRateHelperList(l: list) -> None:
+        checkInstance(l, type=list)
+        if len(l) == 0:
+            raise ConfigurationError(
+                'Invalid piecewise curve configuration, rateHelpers should not be empty')
+        for pos, helper in enumerate(l):
+            checkRateHelper(helper, pos)
+
+    reference = {
+        "curveType": partial(checkIsInEnum, enum=[r.value for r in CurveType]),
+        "dayCounter": checkDayCounter,
+        "enableExtrapolation": partial(checkInstance, type=bool),
+        "rateHelpers": checkRateHelperList
+    }
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise ConfigurationError(
+            'Invalid piecewise curve configuration') from exc
+
+
+def checkDiscountCurve(data: dict) -> None:
+    '''
+    Check if the discount curve is valid
+
+    Parameters
+    ----------
+    data: dict
+        The discount curve
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    InvalidCurve
+        If the curve is invalid
+
+    Details
+    -------
+    The discount curve should have the following example structure:
+
+    ```
+    "example": {
+            "curveType": "Discount",
+            "dayCounter": "Actual360",
+            "enableExtrapolation": True,
+            "nodes": [
+                {
+                    "date": "2020-01-01",
+                    "value": 0.99
+                }
+            ]
+        }
+    ```
+    '''
+    def checkNodeList(l: list) -> None:
+        ref = {
+            "date": checkDate,
+            "value": partial(checkInstance, type=float)
+        }
+        checkInstance(l, type=list)
+        if len(l) == 0:
+            raise ConfigurationError(
+                'Invalid discount curve configuration, discountFactors should not be empty')
+        for node in l:
+            checkDictStructure(node, ref)
+
+    reference = {
+        "curveType": partial(checkIsInEnum, enum=[r.value for r in CurveType]),
+        "dayCounter": checkDayCounter,
+        "enableExtrapolation": partial(checkInstance, type=bool),
+        "nodes": checkNodeList
+    }
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise ConfigurationError(
+            'Invalid discount curve configuration') from exc
+
+
+def checkCurve(data: dict, pos: int) -> None:
+    '''
+    Check if the curve is valid
+
+    Parameters
+    ----------
+    data: dict
+        The curve
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ConfigurationError
+        If the curve is invalid
+
+    Details
+    -------
+    The curve should have the following example structure:
+
+    ```
+    "curve": {
+        "curveName": "CLP",
+        "curveConfig": {
+            "curveType": "Piecewise",
+            "dayCounter": "Actual360",
+            "enableExtrapolation": True,
+            "rateHelpers": []   # if curveType is Piecewise, otherwise nodes             
+
+        },
+        "curveIndex": {}
+    }
+    ```
+    '''
+    def checkBaseCurve(dict: dict) -> None:
+        if "curveType" not in dict:
+            raise ConfigurationError(
+                'Invalid curve configuration, curveType should be defined')
+        if dict["curveType"] == CurveType.Piecewise.value:
+            checkPiecewiseCurve(dict)
+        elif dict["curveType"] == CurveType.Discount.value:
+            checkDiscountCurve(dict)
+        else:
+            raise ConfigurationError(
+                'Invalid curve configuration, curveType should be Piecewise or Discount')
+
+    reference = {
+        "curveName": partial(checkInstance, type=str),
+        "curveConfig": checkBaseCurve,
+        "curveIndex": checkIndex
+    }
+
+    try:
+        checkDictStructure(data, reference)
+    except ConfigurationError as exc:
+        raise ConfigurationError(
+            'Invalid curve configuration for {} curve'.format(data['curveName'])) from exc
+    except Exception as exc:
+        raise ConfigurationError('Invalid curve configuration at pos {}'.format(pos)) from exc
+
+
+def checkConfiguration(data: dict) -> None:
+    '''
+    Check if the configuration is valid
+
+    Parameters
+    ----------
+    data: dict
+        The configuration
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ConfigurationError
+        If the configuration is invalid
+
+    Details
+    -------
+    The configuration should have the following example structure:
+
+    ```
+    "configuration": {
+        "refDate": "2020-01-01",
+        "curves": [
+                {
+                    "curveName": "CLP",
+                    "curveConfig": {
+                        "curveType": "Piecewise",
+                        "dayCounter": "Actual360",
+                        "enableExtrapolation": True,
+                        "rateHelpers": [
+                            ...
+                            ]
+                        },
+                    "curveIndex": {
+                        ...
+                    }
+                }
+            ]
+        }        
+    }
+    ```
+    '''
+    def checkCurveList(l: list) -> None:
+        checkInstance(l, type=list)
+        if len(l) == 0:
+            raise ConfigurationError(
+                'Invalid configuration, curves should not be empty')
+        for pos, curve in enumerate(l):
+            checkCurve(curve, pos)
+
+    reference = {
+        "refDate": checkDate,
+        "curves": checkCurveList
+    }
+
+    try:
+        checkDictStructure(data, reference)
+    except Exception as exc:
+        raise ConfigurationError('Invalid configuration') from exc
```

## curveengine/parsing/enums.py

 * *Ordering differences only*

```diff
@@ -1,155 +1,155 @@
-from enum import Enum
-import ORE as ore
-
-
-class HelperType(Enum):
-    '''
-    Enum for the type of helper
-    '''
-    Bond = "Bond"
-    Deposit = "Deposit"
-    FxSwap = "FxSwap"
-    OIS = "OIS"
-    SofrFuture = "SofrFuture"
-    Xccy = "Xccy"
-    Swap = "Swap"
-    TenorBasis = "TenorBasis"
-    XccyBasis = "XccyBasis"
-
-
-class CurveType(Enum):
-    '''
-    Enum for the type of curve
-    '''
-    Discount = "Discount"
-    Piecewise = "Piecewise"
-
-
-class IndexType(Enum):
-    '''
-    Enum for the type of index
-    '''
-    OvernightIndex = "OvernightIndex"
-    IborIndex = "IborIndex"
-
-
-class Frequency(Enum):
-    '''
-    Enum for the frequency of the index
-    '''
-    Annual = ore.Annual
-    Semiannual = ore.Semiannual
-    Quarterly = ore.Quarterly
-    Monthly = ore.Monthly
-    Weekly = ore.Weekly
-    Daily = ore.Daily
-    Once = ore.Once
-    Bimonthly = ore.Bimonthly
-    OtherFrequency = ore.OtherFrequency
-    EveryFourthMonth = ore.EveryFourthMonth
-    EveryFourthWeek = ore.EveryFourthWeek
-    Biweekly = ore.Biweekly
-    NoFrequency = ore.NoFrequency
-
-
-class DayCounter(Enum):
-    '''
-    Enum for the day counter of the index
-    '''
-    Actual360 = ore.Actual360()
-    Actual365 = ore.Actual365Fixed()
-    Thirty360 = ore.Thirty360(ore.Thirty360.BondBasis)
-
-
-class Calendar(Enum):
-    '''
-    Enum for the calendar of the index
-    '''
-    NullCalendar = ore.NullCalendar()
-    TARGET = ore.TARGET()
-    UnitedStates = ore.UnitedStates(ore.UnitedStates.NYSE)
-    Chile = ore.Chile()
-    Brazil = ore.Brazil()
-
-
-class Convention(Enum):
-    '''
-    Enum for the convention of the index
-    '''
-    Following = ore.Following
-    ModifiedFollowing = ore.ModifiedFollowing
-    Preceding = ore.Preceding
-    ModifiedPreceding = ore.ModifiedPreceding
-    HalfMonthModifiedFollowing = ore.HalfMonthModifiedFollowing
-    Unadjusted = ore.Unadjusted
-
-
-class Compounding(Enum):
-    '''
-    Enum for the compounding of the index
-    '''
-    Simple = ore.Simple
-    Compounded = ore.Compounded
-    Continuous = ore.Continuous
-    SimpleThenCompounded = ore.SimpleThenCompounded
-
-
-class TimeUnit(Enum):
-    '''
-    Enum for the time unit of the index
-    '''
-    Days = ore.Days
-    Weeks = ore.Weeks
-    Months = ore.Months
-    Years = ore.Years
-
-
-class DateGenerationRule(Enum):
-    '''
-    Enum for the date generation rule of the index
-    '''
-    Backward = ore.DateGeneration.Backward
-    Forward = ore.DateGeneration.Forward
-    Zero = ore.DateGeneration.Zero
-    ThirdWednesday = ore.DateGeneration.ThirdWednesday
-    Twentieth = ore.DateGeneration.Twentieth
-    TwentiethIMM = ore.DateGeneration.TwentiethIMM
-    OldCDS = ore.DateGeneration.OldCDS
-
-
-class Currency(Enum):
-    '''
-    Enum for currencies    
-    '''
-    USD = ore.USDCurrency()
-    EUR = ore.EURCurrency()
-    GBP = ore.GBPCurrency()
-    CHF = ore.CHFCurrency()
-    JPY = ore.JPYCurrency()
-    CLF = ore.CLFCurrency()
-    CLP = ore.CLPCurrency()
-    COP = ore.COPCurrency()
-    BRL = ore.BRLCurrency()
-    MXN = ore.MXNCurrency()
-    AUD = ore.AUDCurrency()
-    NZD = ore.NZDCurrency()
-    SEK = ore.SEKCurrency()
-    PEN = ore.PENCurrency()
-
-
-class Month(Enum):
-    '''
-    Enum for months
-    '''
-    January = ore.January
-    February = ore.February
-    March = ore.March
-    April = ore.April
-    May = ore.May
-    June = ore.June
-    July = ore.July
-    August = ore.August
-    September = ore.September
-    October = ore.October
-    November = ore.November
-    December = ore.December
+from enum import Enum
+import ORE as ore
+
+
+class HelperType(Enum):
+    '''
+    Enum for the type of helper
+    '''
+    Bond = "Bond"
+    Deposit = "Deposit"
+    FxSwap = "FxSwap"
+    OIS = "OIS"
+    SofrFuture = "SofrFuture"
+    Xccy = "Xccy"
+    Swap = "Swap"
+    TenorBasis = "TenorBasis"
+    XccyBasis = "XccyBasis"
+
+
+class CurveType(Enum):
+    '''
+    Enum for the type of curve
+    '''
+    Discount = "Discount"
+    Piecewise = "Piecewise"
+
+
+class IndexType(Enum):
+    '''
+    Enum for the type of index
+    '''
+    OvernightIndex = "OvernightIndex"
+    IborIndex = "IborIndex"
+
+
+class Frequency(Enum):
+    '''
+    Enum for the frequency of the index
+    '''
+    Annual = ore.Annual
+    Semiannual = ore.Semiannual
+    Quarterly = ore.Quarterly
+    Monthly = ore.Monthly
+    Weekly = ore.Weekly
+    Daily = ore.Daily
+    Once = ore.Once
+    Bimonthly = ore.Bimonthly
+    OtherFrequency = ore.OtherFrequency
+    EveryFourthMonth = ore.EveryFourthMonth
+    EveryFourthWeek = ore.EveryFourthWeek
+    Biweekly = ore.Biweekly
+    NoFrequency = ore.NoFrequency
+
+
+class DayCounter(Enum):
+    '''
+    Enum for the day counter of the index
+    '''
+    Actual360 = ore.Actual360()
+    Actual365 = ore.Actual365Fixed()
+    Thirty360 = ore.Thirty360(ore.Thirty360.BondBasis)
+
+
+class Calendar(Enum):
+    '''
+    Enum for the calendar of the index
+    '''
+    NullCalendar = ore.NullCalendar()
+    TARGET = ore.TARGET()
+    UnitedStates = ore.UnitedStates(ore.UnitedStates.NYSE)
+    Chile = ore.Chile()
+    Brazil = ore.Brazil()
+
+
+class Convention(Enum):
+    '''
+    Enum for the convention of the index
+    '''
+    Following = ore.Following
+    ModifiedFollowing = ore.ModifiedFollowing
+    Preceding = ore.Preceding
+    ModifiedPreceding = ore.ModifiedPreceding
+    HalfMonthModifiedFollowing = ore.HalfMonthModifiedFollowing
+    Unadjusted = ore.Unadjusted
+
+
+class Compounding(Enum):
+    '''
+    Enum for the compounding of the index
+    '''
+    Simple = ore.Simple
+    Compounded = ore.Compounded
+    Continuous = ore.Continuous
+    SimpleThenCompounded = ore.SimpleThenCompounded
+
+
+class TimeUnit(Enum):
+    '''
+    Enum for the time unit of the index
+    '''
+    Days = ore.Days
+    Weeks = ore.Weeks
+    Months = ore.Months
+    Years = ore.Years
+
+
+class DateGenerationRule(Enum):
+    '''
+    Enum for the date generation rule of the index
+    '''
+    Backward = ore.DateGeneration.Backward
+    Forward = ore.DateGeneration.Forward
+    Zero = ore.DateGeneration.Zero
+    ThirdWednesday = ore.DateGeneration.ThirdWednesday
+    Twentieth = ore.DateGeneration.Twentieth
+    TwentiethIMM = ore.DateGeneration.TwentiethIMM
+    OldCDS = ore.DateGeneration.OldCDS
+
+
+class Currency(Enum):
+    '''
+    Enum for currencies    
+    '''
+    USD = ore.USDCurrency()
+    EUR = ore.EURCurrency()
+    GBP = ore.GBPCurrency()
+    CHF = ore.CHFCurrency()
+    JPY = ore.JPYCurrency()
+    CLF = ore.CLFCurrency()
+    CLP = ore.CLPCurrency()
+    COP = ore.COPCurrency()
+    BRL = ore.BRLCurrency()
+    MXN = ore.MXNCurrency()
+    AUD = ore.AUDCurrency()
+    NZD = ore.NZDCurrency()
+    SEK = ore.SEKCurrency()
+    PEN = ore.PENCurrency()
+
+
+class Month(Enum):
+    '''
+    Enum for months
+    '''
+    January = ore.January
+    February = ore.February
+    March = ore.March
+    April = ore.April
+    May = ore.May
+    June = ore.June
+    July = ore.July
+    August = ore.August
+    September = ore.September
+    October = ore.October
+    November = ore.November
+    December = ore.December
```

## curveengine/parsing/others.py

 * *Ordering differences only*

```diff
@@ -1,142 +1,142 @@
-from .parsers import *
-from .enums import *
-from collections import deque
-
-
-def createOvernightIndex(name: str, indexConfig: dict, handle: ore.YieldTermStructureHandle):
-    """
-    Create an overnight index
-
-    Parameters
-    ----------
-    name : str
-        Name of the index
-    indexConfig : dict
-        Dictionary containing the index configuration
-    handle : ore.YieldTermStructureHandle
-        Handle to the yield term structure
-
-    Returns
-    -------
-    ore.OvernightIndex
-        Overnight index
-    """
-    dayCounter = indexConfig['dayCounter']
-    currency = indexConfig['currency']
-    calendar = indexConfig['calendar']
-    fixingDays = indexConfig['fixingDays']
-    index = ore.OvernightIndex(
-        name, fixingDays, currency, calendar, dayCounter)
-    return index
-
-
-def createIborIndex(name: str, indexConfig: dict, handle: ore.YieldTermStructureHandle):
-    """
-    Create an ibor index
-
-    Parameters
-    ----------
-    name : str
-        Name of the index
-    indexConfig : dict
-        Dictionary containing the index configuration
-    handle : ore.YieldTermStructureHandle
-        Handle to the yield term structure
-
-    Returns
-    -------
-    ore.IborIndex
-        Ibor index
-    """
-    dayCounter = indexConfig['dayCounter']
-    currency = indexConfig['currency']
-    calendar = indexConfig['calendar']
-    fixingDays = indexConfig['fixingDays']
-    tenor = indexConfig['tenor']
-    endOfMonth = indexConfig['endOfMonth']
-    convention = indexConfig['convention']
-    index = ore.IborIndex(name, tenor, fixingDays, currency,
-                          calendar, convention, endOfMonth, dayCounter)
-    return index
-
-
-def getDependencyList(data: dict) -> dict:
-    """
-    Get the dependency list for the curves.
-
-    Parameters
-    ----------
-    data : dict
-        Dictionary containing the curve data.
-
-    Returns
-    -------
-    dict
-        Dictionary containing the dependency list.
-
-    Notes
-    -----
-    The dependency list is a dictionary with the curve name as key and a set of
-    curve names as value. The set contains the names of the curves that the
-    curve depends on.
-    """
-    # Possible curve related keys
-    pc = ['discountCurve', 'collateralCurve']
-    # Possible index related keys
-    pi = ['index', 'shortIndex', 'longIndex']
-
-    dependencies = {}
-    for curve in data['curves']:
-        curveName = curve['curveName']
-        if curveName not in dependencies.keys():
-            dependencies[curveName] = set()
-
-        curveConfig = curve['curveConfig']
-        curveType = CurveType(curveConfig['curveType'])
-        if curveType == CurveType.Piecewise:
-            for rateHelper in curveConfig['rateHelpers']:
-                helperConfig = rateHelper['helperConfig']
-                for key in pc:
-                    if key in helperConfig:
-                        dependencies[curveName].add(helperConfig[key])
-                    for key in pi:
-                        if key in helperConfig:
-                            dependencies[curveName].add(helperConfig[key])
-    return dependencies
-
-
-def topologicalSort(dependencies):
-    """
-    Sort the dependency list topologically
-
-    Parameters
-    ----------
-    dependencies : dict
-        Dictionary containing the dependency list
-
-    Returns
-    -------
-    list
-        List of curve names sorted topologically
-    """
-    for element, deps in dependencies.items():
-        deps.discard(element)
-
-    # Find elements with no dependencies
-    noDependency = deque([k for k, v in dependencies.items() if not v])
-
-    sortedElements = []
-
-    while noDependency:
-        currentElement = noDependency.popleft()
-        sortedElements.append(currentElement)
-
-        # Remove the current element as a dependency from other elements
-        for element, deps in dependencies.items():
-            if currentElement in deps:
-                deps.remove(currentElement)
-                # If the element now has no dependencies, add it to the queue
-                if not deps and element not in noDependency:
-                    noDependency.append(element)
-
-    return sortedElements
+from .parsers import *
+from .enums import *
+from collections import deque
+
+
+def createOvernightIndex(name: str, indexConfig: dict, handle: ore.YieldTermStructureHandle):
+    """
+    Create an overnight index
+
+    Parameters
+    ----------
+    name : str
+        Name of the index
+    indexConfig : dict
+        Dictionary containing the index configuration
+    handle : ore.YieldTermStructureHandle
+        Handle to the yield term structure
+
+    Returns
+    -------
+    ore.OvernightIndex
+        Overnight index
+    """
+    dayCounter = indexConfig['dayCounter']
+    currency = indexConfig['currency']
+    calendar = indexConfig['calendar']
+    fixingDays = indexConfig['fixingDays']
+    index = ore.OvernightIndex(
+        name, fixingDays, currency, calendar, dayCounter)
+    return index
+
+
+def createIborIndex(name: str, indexConfig: dict, handle: ore.YieldTermStructureHandle):
+    """
+    Create an ibor index
+
+    Parameters
+    ----------
+    name : str
+        Name of the index
+    indexConfig : dict
+        Dictionary containing the index configuration
+    handle : ore.YieldTermStructureHandle
+        Handle to the yield term structure
+
+    Returns
+    -------
+    ore.IborIndex
+        Ibor index
+    """
+    dayCounter = indexConfig['dayCounter']
+    currency = indexConfig['currency']
+    calendar = indexConfig['calendar']
+    fixingDays = indexConfig['fixingDays']
+    tenor = indexConfig['tenor']
+    endOfMonth = indexConfig['endOfMonth']
+    convention = indexConfig['convention']
+    index = ore.IborIndex(name, tenor, fixingDays, currency,
+                          calendar, convention, endOfMonth, dayCounter)
+    return index
+
+
+def getDependencyList(data: dict) -> dict:
+    """
+    Get the dependency list for the curves.
+
+    Parameters
+    ----------
+    data : dict
+        Dictionary containing the curve data.
+
+    Returns
+    -------
+    dict
+        Dictionary containing the dependency list.
+
+    Notes
+    -----
+    The dependency list is a dictionary with the curve name as key and a set of
+    curve names as value. The set contains the names of the curves that the
+    curve depends on.
+    """
+    # Possible curve related keys
+    pc = ['discountCurve', 'collateralCurve']
+    # Possible index related keys
+    pi = ['index', 'shortIndex', 'longIndex']
+
+    dependencies = {}
+    for curve in data['curves']:
+        curveName = curve['curveName']
+        if curveName not in dependencies.keys():
+            dependencies[curveName] = set()
+
+        curveConfig = curve['curveConfig']
+        curveType = CurveType(curveConfig['curveType'])
+        if curveType == CurveType.Piecewise:
+            for rateHelper in curveConfig['rateHelpers']:
+                helperConfig = rateHelper['helperConfig']
+                for key in pc:
+                    if key in helperConfig:
+                        dependencies[curveName].add(helperConfig[key])
+                    for key in pi:
+                        if key in helperConfig:
+                            dependencies[curveName].add(helperConfig[key])
+    return dependencies
+
+
+def topologicalSort(dependencies):
+    """
+    Sort the dependency list topologically
+
+    Parameters
+    ----------
+    dependencies : dict
+        Dictionary containing the dependency list
+
+    Returns
+    -------
+    list
+        List of curve names sorted topologically
+    """
+    for element, deps in dependencies.items():
+        deps.discard(element)
+
+    # Find elements with no dependencies
+    noDependency = deque([k for k, v in dependencies.items() if not v])
+
+    sortedElements = []
+
+    while noDependency:
+        currentElement = noDependency.popleft()
+        sortedElements.append(currentElement)
+
+        # Remove the current element as a dependency from other elements
+        for element, deps in dependencies.items():
+            if currentElement in deps:
+                deps.remove(currentElement)
+                # If the element now has no dependencies, add it to the queue
+                if not deps and element not in noDependency:
+                    noDependency.append(element)
+
+    return sortedElements
```

## curveengine/parsing/parsers.py

```diff
@@ -1,335 +1,337 @@
-import ORE as ore
-from .enums import *
-
-
-def parse(**kwargs):
-    results = {}
-    for key, value in kwargs.items():
-        if key in ['helperConfig', 'curveIndex', 'curveConfig']:
-            results[key] = parse(**value)
-
-        elif key == 'nodes':
-            results[key] = [parseNode(v) for v in value]
-
-        elif key in ['curves', 'rateHelpers']:
-            results[key] = [parse(**v) for v in value]
-
-        elif key in ['date', 'startDate', 'endDate']:
-            results[key] = parseDate(value)
-
-        elif key == 'helperType':
-            results[key] = HelperType(value)
-
-        elif key == 'curveType':
-            results[key] = CurveType(value)
-
-        elif key == 'indexType':
-            results[key] = IndexType(value)
-
-        elif key in ['dayCounter', 'couponDayCounter', 'yieldDayCounter']:
-            results[key] = parseDayCounter(value)
-
-        elif key == 'compounding':
-            results[key] = parseCompounding(value)
-
-        elif key in ['frequency', 'paymentFrequency', 'fixedLegFrequency', 'floatingLegFrequency']:
-            results[key] = parseFrequency(value)
-
-        elif key in ['currency', 'fixedLegCurrency']:
-            results[key] = parseCurrency(value)
-
-        elif key == 'calendar':
-            results[key] = parseCalendar(value)
-
-        elif key == 'convention':
-            results[key] = parseBusinessDayConvention(value)
-
-        elif key in ['tenor', 'fwdStart', 'shortPayTenor']:
-            results[key] = parsePeriod(value)
-
-        elif key in ['endOfMonth', 'telescopicValueDates', 'spreadOnShortIndex', 'baseCurrencyAsCollateral', 'enableExtrapolation']:
-            results[key] = value
-
-        elif key in ['settlementDays', 'paymentLag', 'fixingDays', 'year']:
-            results[key] = value
-
-        elif key in ['discountCurve', 'index', 'shortIndex', 'longIndex', 'curveName']:
-            results[key] = value
-
-        elif key in ['couponRate']:
-            results[key] = value
-
-        elif key == 'month':
-            results[key] = parseMonth(value)
-
-        else:
-            results[key] = value
-
-    return results
-
-
-def parseOREDate(date: ore.Date) -> str:
-    """
-    Parse an ORE date to a string
-
-    Parameters
-    ----------
-    date : ore.Date
-        The ORE date
-
-    Returns
-    -------
-    str
-        The string representation of the date
-    """
-    return '{0}-{1}-{2}'.format(date.year(), date.month(), date.dayOfMonth())
-
-
-def parseNode(node):
-    return {'date': parseDate(node['date']), 'value': node['value']}
-
-
-def createInterestRate(
-        rate: float,
-        dayCount: str,
-        compounding: str,
-        frequency: str) -> ore.InterestRate:
-    return ore.InterestRate(
-        rate,
-        parseDayCounter(dayCount),
-        parseCompounding(compounding),
-        parseFrequency(frequency))
-
-
-def parseCompounding(compounding: str):
-    """
-    Parse a compounding string to an ORE compounding enum
-
-    Parameters
-    ----------
-    compounding : str
-        The compounding string
-
-    Returns
-    -------
-    ore.Compounding
-        The ORE compounding enum
-    """
-    try:
-        value = Compounding[compounding]
-    except KeyError:
-        raise NotImplementedError(
-            'unknown compounding: {0}'.format(compounding))
-    return value.value
-
-
-def parseFrequency(frequency: str):
-    """
-    Parse a frequency string to an ORE frequency enum
-
-    Parameters
-    ----------
-    frequency : str
-        The frequency string
-
-    Returns
-    -------
-    ore.Frequency
-        The ORE frequency enum
-    """
-
-    try:
-        value = Frequency[frequency]
-    except KeyError:
-        raise NotImplementedError('unknown frequency: {0}'.format(frequency))
-    return value.value
-
-
-def parseDayCounter(dayCounter: ore.DayCounter) -> ore.DayCounter:
-    """
-    Parse a day counter string to an ORE day counter enum
-
-    Parameters
-    ----------
-    dayCounter : str
-        The day counter string
-
-    Returns
-    -------
-    ore.DayCounter
-        The ORE day counter enum
-    """
-    try:
-        value = DayCounter[dayCounter]
-    except KeyError:
-        raise NotImplementedError(
-            'unknown day counter: {0}'.format(dayCounter))
-    return value.value
-
-
-def parseCalendar(calendar: str) -> ore.Calendar:
-    """
-    Parse a calendar string to an ORE calendar enum
-
-    Parameters
-    ----------
-    calendar : str
-        The calendar string
-
-    Returns
-    -------
-    ore.Calendar
-        The ORE calendar enum
-    """
-    try:
-        value = Calendar[calendar]
-    except KeyError:
-        raise NotImplementedError('unknown calendar: {0}'.format(calendar))
-    return value.value
-
-
-def parseBusinessDayConvention(businessDayConvention: str):
-    """
-    Parse a business day convention string to an ORE business day convention enum
-
-    Parameters
-    ----------
-    businessDayConvention : str
-        The business day convention string
-
-    Returns
-    -------
-    ore.BusinessDayConvention
-        The ORE business day convention enum
-    """
-
-    try:
-        value = Convention[businessDayConvention]
-    except KeyError:
-        raise NotImplementedError(
-            'unknown business day convention: {0}'.format(businessDayConvention))
-    return value.value
-
-
-def parseTimeUnit(timeUnit: str):
-    """
-    Parse a time unit string to an ORE time unit enum
-
-    Parameters
-    ----------
-    timeUnit : str
-        The time unit string
-
-    Returns
-    -------
-    ore.TimeUnit
-        The ORE time unit enum
-    """
-    try:
-        value = TimeUnit[timeUnit]
-    except KeyError:
-        raise NotImplementedError('unknown time unit: {0}'.format(timeUnit))
-    return value.value
-
-
-def parseDateGenerationRule(dateGenerationRule: str):
-    """
-    Parse a date generation rule string to an ORE date generation rule enum
-
-    Parameters
-    ----------
-    dateGenerationRule : str
-        The date generation rule string
-
-    Returns
-    -------
-    ore.DateGeneration
-        The ORE date generation rule enum
-    """
-    try:
-        value = DateGenerationRule[dateGenerationRule]
-    except KeyError:
-        raise NotImplementedError(
-            'unknown date generation rule: {0}'.format(dateGenerationRule))
-    return value.value
-
-
-def parseDate(date: str) -> ore.Date:
-    """
-    Parse a date string to an ORE date
-
-    Parameters
-    ----------
-    date : str
-        The date string
-
-    Returns
-    -------
-    ore.Date
-        The ORE date
-    """
-
-    if date == 'today':
-        return ore.Date.todaysDate()
-    else:
-        return ore.DateParser.parseFormatted(date, '%Y-%m-%d')
-
-
-def parsePeriod(period: str) -> ore.Period:
-    """
-    Parse a period string to an ORE period
-
-    Parameters
-    ----------
-    period : str
-        The period string
-
-    Returns
-    -------
-    ore.Period
-        The ORE period
-    """
-    tenor = ore.PeriodParser.parse(period)
-    return tenor
-
-
-def parseCurrency(currency: str) -> ore.Currency:
-    """
-    Parse a currency string to an ORE currency
-
-    Parameters
-    ----------
-    currency : str
-        The currency string
-
-    Returns
-    -------
-    ore.Currency
-        The ORE currency
-    """
-    try:
-        value = Currency[currency]
-    except KeyError:
-        raise NotImplementedError('unknown currency: {0}'.format(currency))
-    return value.value
-
-
-def parseMonth(month: str):
-    """
-    Parse a month string to an ORE month enum
-
-    Parameters
-    ----------
-    month : str
-        The month string
-
-    Returns
-    -------
-    ore.Month
-        The ORE month enum
-    """
-    try:
-        value = Month[month]
-    except KeyError:
-        raise NotImplementedError('unknown month: {0}'.format(month))
-    return value.value
+import ORE as ore
+from .enums import *
+
+
+def parse(**kwargs):
+    results = {}
+    for key, value in kwargs.items():
+        if key in ['helperConfig', 'curveIndex', 'curveConfig']:
+            results[key] = parse(**value)
+
+        elif key == 'nodes':
+            results[key] = [parseNode(v) for v in value]
+
+        elif key in ['curves', 'rateHelpers']:
+            results[key] = [parse(**v) for v in value]
+
+        elif key in ['date', 'startDate', 'endDate']:
+            results[key] = parseDate(value)
+
+        elif key == 'helperType':
+            results[key] = HelperType(value)
+
+        elif key == 'curveType':
+            results[key] = CurveType(value)
+
+        elif key == 'indexType':
+            results[key] = IndexType(value)
+
+        elif key in ['dayCounter', 'couponDayCounter', 'yieldDayCounter']:
+            results[key] = parseDayCounter(value)
+
+        elif key == 'compounding':
+            results[key] = parseCompounding(value)
+
+        elif key in ['frequency', 'paymentFrequency', 'fixedLegFrequency', 'floatingLegFrequency']:
+            results[key] = parseFrequency(value)
+
+        elif key in ['currency', 'fixedLegCurrency']:
+            results[key] = parseCurrency(value)
+
+        elif key == 'calendar':
+            results[key] = parseCalendar(value)
+
+        elif key == 'convention':
+            results[key] = parseBusinessDayConvention(value)
+
+        elif key in ['tenor', 'fwdStart', 'shortPayTenor']:
+            results[key] = parsePeriod(value)
+
+        elif key in ['endOfMonth', 'telescopicValueDates', 'spreadOnShortIndex', 'baseCurrencyAsCollateral', 'enableExtrapolation']:
+            results[key] = value
+
+        elif key in ['settlementDays', 'paymentLag', 'fixingDays', 'year']:
+            results[key] = value
+
+        elif key in ['discountCurve', 'index', 'shortIndex', 'longIndex', 'curveName']:
+            results[key] = value
+
+        elif key in ['couponRate']:
+            results[key] = value
+
+        elif key == 'month':
+            results[key] = parseMonth(value)
+
+        else:
+            results[key] = value
+
+    return results
+
+
+def parseOREDate(date: ore.Date) -> str:
+    """
+    Parse an ORE date to a string
+
+    Parameters
+    ----------
+    date : ore.Date
+        The ORE date
+
+    Returns
+    -------
+    str
+        The string representation of the date
+    """
+    return '{0}-{1}-{2}'.format(date.year(), date.month(), date.dayOfMonth())
+
+
+def parseNode(node):
+    return {'date': parseDate(node['date']), 'value': node['value']}
+
+
+def createInterestRate(
+        rate: float,
+        dayCount: str,
+        compounding: str,
+        frequency: str) -> ore.InterestRate:
+    return ore.InterestRate(
+        rate,
+        parseDayCounter(dayCount),
+        parseCompounding(compounding),
+        parseFrequency(frequency))
+
+
+def parseCompounding(compounding: str):
+    """
+    Parse a compounding string to an ORE compounding enum
+
+    Parameters
+    ----------
+    compounding : str
+        The compounding string
+
+    Returns
+    -------
+    ore.Compounding
+        The ORE compounding enum
+    """
+    try:
+        value = Compounding[compounding]
+    except KeyError:
+        raise NotImplementedError(
+            'unknown compounding: {0}'.format(compounding))
+    return value.value
+
+
+def parseFrequency(frequency: str):
+    """
+    Parse a frequency string to an ORE frequency enum
+
+    Parameters
+    ----------
+    frequency : str
+        The frequency string
+
+    Returns
+    -------
+    ore.Frequency
+        The ORE frequency enum
+    """
+
+    try:
+        value = Frequency[frequency]
+    except KeyError:
+        raise NotImplementedError('unknown frequency: {0}'.format(frequency))
+    return value.value
+
+
+def parseDayCounter(dayCounter: ore.DayCounter) -> ore.DayCounter:
+    """
+    Parse a day counter string to an ORE day counter enum
+
+    Parameters
+    ----------
+    dayCounter : str
+        The day counter string
+
+    Returns
+    -------
+    ore.DayCounter
+        The ORE day counter enum
+    """
+    try:
+        value = DayCounter[dayCounter]
+    except KeyError:
+        raise NotImplementedError(
+            'unknown day counter: {0}'.format(dayCounter))
+    return value.value
+
+
+def parseCalendar(calendar: str) -> ore.Calendar:
+    """
+    Parse a calendar string to an ORE calendar enum
+
+    Parameters
+    ----------
+    calendar : str
+        The calendar string
+
+    Returns
+    -------
+    ore.Calendar
+        The ORE calendar enum
+    """
+    try:
+        value = Calendar[calendar]
+    except KeyError:
+        raise NotImplementedError('unknown calendar: {0}'.format(calendar))
+    return value.value
+
+
+def parseBusinessDayConvention(businessDayConvention: str):
+    """
+    Parse a business day convention string to an ORE business day convention enum
+
+    Parameters
+    ----------
+    businessDayConvention : str
+        The business day convention string
+
+    Returns
+    -------
+    ore.BusinessDayConvention
+        The ORE business day convention enum
+    """
+
+    try:
+        value = Convention[businessDayConvention]
+    except KeyError:
+        raise NotImplementedError(
+            'unknown business day convention: {0}'.format(businessDayConvention))
+    return value.value
+
+
+def parseTimeUnit(timeUnit: str):
+    """
+    Parse a time unit string to an ORE time unit enum
+
+    Parameters
+    ----------
+    timeUnit : str
+        The time unit string
+
+    Returns
+    -------
+    ore.TimeUnit
+        The ORE time unit enum
+    """
+    try:
+        value = TimeUnit[timeUnit]
+    except KeyError:
+        raise NotImplementedError('unknown time unit: {0}'.format(timeUnit))
+    return value.value
+
+
+def parseDateGenerationRule(dateGenerationRule: str):
+    """
+    Parse a date generation rule string to an ORE date generation rule enum
+
+    Parameters
+    ----------
+    dateGenerationRule : str
+        The date generation rule string
+
+    Returns
+    -------
+    ore.DateGeneration
+        The ORE date generation rule enum
+    """
+    try:
+        value = DateGenerationRule[dateGenerationRule]
+    except KeyError:
+        raise NotImplementedError(
+            'unknown date generation rule: {0}'.format(dateGenerationRule))
+    return value.value
+
+
+def parseDate(date: str) -> ore.Date:
+    """
+    Parse a date string to an ORE date
+
+    Parameters
+    ----------
+    date : str
+        The date string
+
+    Returns
+    -------
+    ore.Date
+        The ORE date
+    """
+
+    if date == 'today':
+        return ore.Date.todaysDate()
+    else:
+        return ore.DateParser.parseISO(date[0:10])
+
+
+
+def parsePeriod(period: str) -> ore.Period:
+    """
+    Parse a period string to an ORE period
+
+    Parameters
+    ----------
+    period : str
+        The period string
+
+    Returns
+    -------
+    ore.Period
+        The ORE period
+    """
+    
+    tenor = ore.PeriodParser.parse(period)
+    return tenor
+
+
+def parseCurrency(currency: str) -> ore.Currency:
+    """
+    Parse a currency string to an ORE currency
+
+    Parameters
+    ----------
+    currency : str
+        The currency string
+
+    Returns
+    -------
+    ore.Currency
+        The ORE currency
+    """
+    try:
+        value = Currency[currency]
+    except KeyError:
+        raise NotImplementedError('unknown currency: {0}'.format(currency))
+    return value.value
+
+
+def parseMonth(month: str):
+    """
+    Parse a month string to an ORE month enum
+
+    Parameters
+    ----------
+    month : str
+        The month string
+
+    Returns
+    -------
+    ore.Month
+        The ORE month enum
+    """
+    try:
+        value = Month[month]
+    except KeyError:
+        raise NotImplementedError('unknown month: {0}'.format(month))
+    return value.value
```

## curveengine/parsing/ratehelpers.py

```diff
@@ -1,523 +1,523 @@
-from .parsers import *
-from .others import *
-
-
-def createOISRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
-    """
-    Create an OIS rate helper
-
-    Parameters
-    ----------
-    helperConfig : dict
-        The configuration for the helper
-
-    marketConfig : dict
-        The market configuration for the helper
-
-    curves : dict
-        The curves
-    indexes : dict
-        The indexes
-
-    Returns
-    -------
-    ore.OISRateHelper
-        The rate helper
-
-    See Also
-    ----------
-    checkOISRateHelper
-    """
-    tenor = helperConfig['tenor']
-    calendar = helperConfig['calendar']
-    businessDayConvention = helperConfig['convention']
-
-    settlementDays = helperConfig['settlementDays']
-    endOfMonth = helperConfig['endOfMonth']
-    paymentLag = helperConfig['paymentLag']
-    fixedLegFrequency = helperConfig['fixedLegFrequency']
-    fwdStart = helperConfig['fwdStart']
-    index = indexes[helperConfig['index']]
-
-    rate = marketConfig['rate']['value']
-    discountCurve = curves[helperConfig['discountCurve']]
-
-    rate = ore.QuoteHandle(ore.SimpleQuote(rate))
-    helper = ore.OISRateHelper(settlementDays, tenor, rate, index, discountCurve, endOfMonth,
-                               paymentLag, businessDayConvention, fixedLegFrequency, calendar, fwdStart)
-    return helper
-
-
-def createDepositRateHelper(helperConfig: dict, marketConfig: dict, *args, **kwargs):
-    """
-    Create a deposit rate helper
-
-    Parameters
-    ----------
-    helperConfig : dict
-        The configuration for the helper
-       
-    marketConfig : dict
-        The market configuration for the helper
-       
-    Returns
-    -------
-    ore.DepositRateHelper
-        The rate helper
-
-    See Also
-    ----------
-    checkDepositRateHelper
-    """
-    tenor = helperConfig['tenor']
-    settlementDays = helperConfig['settlementDays']
-    calendar = helperConfig['calendar']
-    convention = helperConfig['convention']
-    endOfMonth = helperConfig['endOfMonth']
-    dayCounter = helperConfig['dayCounter']
-
-    rate = ore.QuoteHandle(ore.SimpleQuote(marketConfig['rate']['value']))
-    helper = ore.DepositRateHelper(rate, tenor, settlementDays, calendar,
-                                   convention, endOfMonth, dayCounter)
-    return helper
-
-
-def createFixedRateBondRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
-    """
-    Create a fixed rate bond helper
-
-    Parameters
-    ----------
-    helperConfig : dict
-        The configuration for the helper
-
-    marketConfig : dict
-        The market configuration for the helper
-
-    curves : dict
-        The curves
-    indexes : dict
-        The indexes
-
-    Returns
-    -------
-    ore.BondHelper
-        The rate helper
-
-    See Also
-    ----------
-    checkFixedRateBondRateHelper
-    """
-    calendar = helperConfig['calendar']
-    businessDayConvention = helperConfig['convention']
-    settlementDays = helperConfig['settlementDays']
-    couponDayCounter = helperConfig['couponDayCounter']
-    couponRate = helperConfig['couponRate']
-    frequency = helperConfig['frequency']
-
-    if 'tenor' in helperConfig.keys():
-        tenor = helperConfig['tenor']
-        startDate = ore.Settings.instance().evaluationDate()
-        maturityDate = startDate + ore.Period(tenor)
-    else:
-        startDate = helperConfig['startDate']
-        maturityDate = helperConfig['endDate']
-
-    # Create a schedule
-    schedule = ore.Schedule(
-        startDate,
-        maturityDate,
-        ore.Period(frequency),
-        calendar,
-        businessDayConvention,
-        businessDayConvention,
-        ore.DateGeneration.Backward,
-        False
-    )
-
-    rate = marketConfig['rate']['value']
-    if isinstance(rate, float):
-        rateDayCounter = ore.Actual365Fixed()
-        rateCompounding = ore.Compounded
-        rateFrequency = ore.Annual
-    elif isinstance(rate, ore.InterestRate):
-        rateDayCounter = rate.dayCounter()
-        rateCompounding = rate.compounding()
-        rateFrequency = rate.frequency()
-    else:
-        raise Exception('rate is not a float or an InterestRate')
-
-    # Create a fixed rate bond
-    fixedRateBond = ore.FixedRateBond(
-        settlementDays,
-        100,
-        schedule,
-        [couponRate],
-        couponDayCounter,
-    )
-
-    # Calculate the clean price
-    cleanPrice = fixedRateBond.cleanPrice(
-        rate,
-        rateDayCounter,
-        rateCompounding,
-        rateFrequency)
-
-    # Bond helper
-    bondHelper = ore.BondHelper(
-        ore.QuoteHandle(ore.SimpleQuote(cleanPrice)),
-        fixedRateBond
-    )
-
-    return bondHelper
-
-
-def createSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
-    """
-    Create a swap rate helper
-
-    Parameters
-    ----------
-    helperConfig : dict
-        The configuration for the helper
-
-    marketConfig : dict
-        The market configuration for the helper      
-
-    curves : dict
-        The curves
-    indexes : dict
-        The indexes
-
-    Returns
-    -------
-    ore.SwapRateHelper
-        The rate helper
-
-    See Also
-    ----------
-    checkSwapRateHelper
-    """
-    tenor = helperConfig['tenor']
-    calendar = helperConfig['calendar']
-    convention = helperConfig['convention']
-    fixedLegFrequency = helperConfig['fixedLegFrequency']
-    dayCounter = helperConfig['dayCounter']
-    fwdStart = helperConfig['fwdStart']
-
-    # QuoteHandle
-    rate = marketConfig['rate']['value']
-    spread = marketConfig['spread']['value']
-    rateQuote = ore.QuoteHandle(ore.SimpleQuote(rate))
-    spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
-
-    # Index
-    index = indexes[helperConfig['index']]
-
-    # Discounting curve
-    discountCurve = curves[helperConfig['discountCurve']]
-
-    # Swap rate helper
-    swapRateHelper = ore.SwapRateHelper(
-        rateQuote, tenor, calendar, fixedLegFrequency, convention, dayCounter, index, spreadQuote, fwdStart, discountCurve
-    )
-    return swapRateHelper
-
-
-def createFxSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
-    """
-    Create a fx swap rate helper
-
-    Parameters
-    ----------
-    helperConfig : dict
-        The configuration for the helper
-
-    marketConfig : dict
-        The market configuration for the helper
-
-    curves : dict
-        The curves
-    indexes : dict
-        The indexes
-
-    Returns
-    -------
-    ore.FxSwapRateHelper
-        The rate helper
-
-    See Also
-    ----------
-    checkFxSwapRateHelper
-    """
-    fxPoints = marketConfig['fxPoints']['value']
-    spotFx = marketConfig['fxSpot']['value']
-
-    fixingDays = helperConfig['fixingDays']
-    calendar = helperConfig['calendar']
-    convention = helperConfig['convention']
-    endOfMonth = helperConfig['endOfMonth']
-    baseCurrencyAsCollateral = helperConfig['baseCurrencyAsCollateral']
-
-    if 'tenor' in helperConfig.keys():
-        tenor = helperConfig['tenor']
-    else:
-        startDate = ore.Settings.instance().evaluationDate
-        maturityDate = helperConfig['endDate']
-        days = maturityDate - startDate
-        tenor = ore.Period(days, ore.Days)
-
-    # QuoteHandle
-    fwdPointQuote = ore.QuoteHandle(ore.SimpleQuote(fxPoints))
-    spotFxQuote = ore.QuoteHandle(ore.SimpleQuote(spotFx))
-
-    # Discounting curve
-    discountCurve = curves[helperConfig['discountCurve']]
-
-    # FxSwapRateHelper
-    fxSwapRateHelper = ore.FxSwapRateHelper(
-        fwdPointQuote,
-        spotFxQuote,
-        tenor,
-        fixingDays,
-        calendar,
-        convention,
-        endOfMonth,
-        baseCurrencyAsCollateral,
-        discountCurve,
-        calendar
-    )
-    return fxSwapRateHelper
-
-
-def createSofrFutureRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
-    """
-    Create a sofr future rate helper
-
-    Parameters
-    ----------
-    helperConfig : dict
-        The configuration for the helper
-
-    marketConfig : dict
-        The market configuration for the helper
-
-    curves : dict
-        The curves
-    indexes : dict
-        The indexes
-
-    Returns
-    -------
-    ore.SofrFutureRateHelper
-        The rate helper
-
-    See Also
-    ----------
-    TODO: checkSofrFutureRateHelper
-    """
-    month = helperConfig['month']
-    year = helperConfig['year']
-    frequency = helperConfig['frequency']
-    # QuoteHandle
-    price = marketConfig['price']
-    convexity = marketConfig['convexity']
-    priceQuote = ore.QuoteHandle(ore.SimpleQuote(price))
-    convexityQuote = ore.QuoteHandle(ore.SimpleQuote(convexity))
-
-    # SofrFutureRateHelper
-    sofrFutureRateHelper = ore.SofrFutureRateHelper(
-        priceQuote,
-        month,
-        year,
-        frequency,
-        convexityQuote
-    )
-    return sofrFutureRateHelper
-
-
-def createTenorBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
-    """
-    Create a tenor basis swap rate helper
-
-    Parameters
-    ----------
-    helperConfig : dict
-        The configuration for the helper
-
-    marketConfig : dict
-        The market configuration for the helper
-
-    curves : dict
-        The curves
-    indexes : dict
-        The indexes
-
-    Returns
-    -------
-    ore.TenorBasisSwapHelper
-        The rate helper
-
-    See Also
-    ----------
-    checkTenorBasisRateHelper
-    """
-    tenor = helperConfig['tenor']
-    spreadOnShort = helperConfig['spreadOnShort']
-
-    # Index
-    longIndex = indexes[helperConfig['longIndex']]
-    shortIndex = indexes[helperConfig['shortIndex']]
-
-    # QuoteHandle
-    spread = marketConfig['spread']['value']
-    spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
-
-    # Discounting curve
-    discountCurve = curves[helperConfig['discountCurve']]
-
-    # TenorBasisSwapHelper
-    tenorBasisSwapHelper = ore.TenorBasisSwapHelper(
-        spreadQuote,
-        tenor,
-        longIndex,
-        shortIndex,
-        ore.Period(),
-        discountCurve,
-        spreadOnShort,
-        True
-    )
-
-    return tenorBasisSwapHelper
-
-
-def createCrossCcyFixFloatSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
-    """
-    Create a cross currency fix float swap rate helper
-
-    Parameters
-    ----------
-    helperConfig : dict
-        The configuration for the helper        
-
-    marketConfig : dict
-        The market configuration for the helper
-
-    curves : dict
-        The curves
-    indexes : dict
-        The indexes
-
-    Returns
-    -------
-    ore.CrossCcyFixFloatSwapHelper
-        The rate helper
-
-    See Also
-    ----------
-    checkCrossCcyFixFloatSwapRateHelper
-    """
-    tenor = helperConfig['tenor']
-    dayCounter = helperConfig['dayCounter']
-    settlementDays = helperConfig['settlementDays']
-    endOfMonth = helperConfig['endOfMonth']
-    convention = helperConfig['convention']
-    fixedLegFrequency = helperConfig['fixedLegFrequency']
-    fixedLegCurrency = helperConfig['fixedLegCurrency']
-    calendar = helperConfig['calendar']
-
-    # QuoteHandle
-    rate = marketConfig['rate']['value']
-    spotFx = marketConfig['fxSpot']['value']
-    spread = marketConfig['spread']['value']
-
-    rateQuote = ore.QuoteHandle(ore.SimpleQuote(rate))
-    spotFxQuote = ore.QuoteHandle(ore.SimpleQuote(spotFx))
-    spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
-
-    # Index
-    index = indexes[helperConfig['index']]
-
-    # Discounting curve
-    discountCurve = curves[helperConfig['discountCurve']]
-
-    # CrossCcyFixFloatSwapHelper
-    crossCcyFixFloatSwapHelper = ore.CrossCcyFixFloatSwapHelper(
-        rateQuote,
-        spotFxQuote,
-        settlementDays,
-        calendar,
-        convention,
-        tenor,
-        fixedLegCurrency,
-        fixedLegFrequency,
-        convention,
-        dayCounter,
-        index,
-        discountCurve,
-        spreadQuote,
-        endOfMonth
-    )
-    return crossCcyFixFloatSwapHelper
-
-
-def createCrossCcyBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
-    """
-    Create a cross currency basis swap rate helper
-
-    Parameters
-    ----------
-    helperConfig : dict
-        The configuration for the helper
-
-    marketConfig : dict
-        The market configuration for the helper
-        - spread : float
-            The spread
-
-    curves : dict
-        The curves
-    indexes : dict
-        The indexes
-
-    Returns
-    -------
-    ore.CrossCcyBasisSwapHelper
-        The rate helper
-
-    See Also
-    ----------
-    checkCrossCcyBasisSwapRateHelper
-    """
-    tenor = helperConfig['tenor']
-    calendar = helperConfig['calendar']
-    settlementDays = helperConfig['settlementDays']
-    endOfMonth = helperConfig['endOfMonth']
-    convention = helperConfig['convention']
-
-    # Discout curves
-    flatDiscountCurve = curves[helperConfig['discountCurve']]
-    spreadDiscountCurve = curves[helperConfig['discountCurve']]
-
-    # Index
-    flatIndex = indexes[helperConfig['flatIndex']]
-    spreadIndex = indexes[helperConfig['spreadIndex']]
-
-    # QuoteHandle
-    spread = marketConfig['spread']['value']
-    spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
-
-    # CrossCcyBasisSwapHelper
-    crossCcyBasisSwapHelper = ore.CrossCcyBasisSwapHelper(
-        spreadQuote,
-        tenor,
-        calendar,
-        settlementDays,
-        flatIndex,
-        spreadIndex,
-        flatDiscountCurve,
-        spreadDiscountCurve,
-        endOfMonth,
-        convention
-    )
-    return crossCcyBasisSwapHelper
+from .parsers import *
+from .others import *
+
+
+def createOISRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+    """
+    Create an OIS rate helper
+
+    Parameters
+    ----------
+    helperConfig : dict
+        The configuration for the helper
+
+    marketConfig : dict
+        The market configuration for the helper
+
+    curves : dict
+        The curves
+    indexes : dict
+        The indexes
+
+    Returns
+    -------
+    ore.OISRateHelper
+        The rate helper
+
+    See Also
+    ----------
+    checkOISRateHelper
+    """
+    tenor = helperConfig['tenor']
+    calendar = helperConfig['calendar']
+    businessDayConvention = helperConfig['convention']
+
+    settlementDays = helperConfig['settlementDays']
+    endOfMonth = helperConfig['endOfMonth']
+    paymentLag = helperConfig['paymentLag']
+    fixedLegFrequency = helperConfig['fixedLegFrequency']
+    fwdStart = helperConfig['fwdStart']
+    index = indexes[helperConfig['index']]
+
+    rate = marketConfig['rate']['value']
+    discountCurve = curves[helperConfig['discountCurve']]
+
+    rate = ore.QuoteHandle(ore.SimpleQuote(rate))
+    helper = ore.OISRateHelper(settlementDays, tenor, rate, index, discountCurve, endOfMonth,
+                               paymentLag, businessDayConvention, fixedLegFrequency, calendar, fwdStart)
+    return helper
+
+
+def createDepositRateHelper(helperConfig: dict, marketConfig: dict, *args, **kwargs):
+    """
+    Create a deposit rate helper
+
+    Parameters
+    ----------
+    helperConfig : dict
+        The configuration for the helper
+       
+    marketConfig : dict
+        The market configuration for the helper
+       
+    Returns
+    -------
+    ore.DepositRateHelper
+        The rate helper
+
+    See Also
+    ----------
+    checkDepositRateHelper
+    """
+    tenor = helperConfig['tenor']
+    settlementDays = helperConfig['settlementDays']
+    calendar = helperConfig['calendar']
+    convention = helperConfig['convention']
+    endOfMonth = helperConfig['endOfMonth']
+    dayCounter = helperConfig['dayCounter']
+
+    rate = ore.QuoteHandle(ore.SimpleQuote(marketConfig['rate']['value']))
+    helper = ore.DepositRateHelper(rate, tenor, settlementDays, calendar,
+                                   convention, endOfMonth, dayCounter)
+    return helper
+
+
+def createFixedRateBondRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+    """
+    Create a fixed rate bond helper
+
+    Parameters
+    ----------
+    helperConfig : dict
+        The configuration for the helper
+
+    marketConfig : dict
+        The market configuration for the helper
+
+    curves : dict
+        The curves
+    indexes : dict
+        The indexes
+
+    Returns
+    -------
+    ore.BondHelper
+        The rate helper
+
+    See Also
+    ----------
+    checkFixedRateBondRateHelper
+    """
+    calendar = helperConfig['calendar']
+    businessDayConvention = helperConfig['convention']
+    settlementDays = helperConfig['settlementDays']
+    couponDayCounter = helperConfig['couponDayCounter']
+    couponRate = helperConfig['couponRate']
+    frequency = helperConfig['frequency']
+
+    if 'tenor' in helperConfig.keys():
+        tenor = helperConfig['tenor']
+        startDate = ore.Settings.instance().evaluationDate
+        maturityDate = startDate + tenor
+    else:
+        startDate = helperConfig['startDate']
+        maturityDate = helperConfig['endDate']
+
+    # Create a schedule
+    schedule = ore.Schedule(
+        startDate,
+        maturityDate,
+        ore.Period(frequency),
+        calendar,
+        businessDayConvention,
+        businessDayConvention,
+        ore.DateGeneration.Backward,
+        False
+    )
+
+    rate = marketConfig['rate']['value']
+    if isinstance(rate, float):
+        rateDayCounter = ore.Actual365Fixed()
+        rateCompounding = ore.Compounded
+        rateFrequency = ore.Annual
+    elif isinstance(rate, ore.InterestRate):
+        rateDayCounter = rate.dayCounter()
+        rateCompounding = rate.compounding()
+        rateFrequency = rate.frequency()
+    else:
+        raise Exception('rate is not a float or an InterestRate')
+
+    # Create a fixed rate bond
+    fixedRateBond = ore.FixedRateBond(
+        settlementDays,
+        100,
+        schedule,
+        [couponRate],
+        couponDayCounter,
+    )
+
+    # Calculate the clean price
+    cleanPrice = fixedRateBond.cleanPrice(
+        rate,
+        rateDayCounter,
+        rateCompounding,
+        rateFrequency)
+
+    # Bond helper
+    bondHelper = ore.BondHelper(
+        ore.QuoteHandle(ore.SimpleQuote(cleanPrice)),
+        fixedRateBond
+    )
+
+    return bondHelper
+
+
+def createSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+    """
+    Create a swap rate helper
+
+    Parameters
+    ----------
+    helperConfig : dict
+        The configuration for the helper
+
+    marketConfig : dict
+        The market configuration for the helper      
+
+    curves : dict
+        The curves
+    indexes : dict
+        The indexes
+
+    Returns
+    -------
+    ore.SwapRateHelper
+        The rate helper
+
+    See Also
+    ----------
+    checkSwapRateHelper
+    """
+    tenor = helperConfig['tenor']
+    calendar = helperConfig['calendar']
+    convention = helperConfig['convention']
+    fixedLegFrequency = helperConfig['fixedLegFrequency']
+    dayCounter = helperConfig['dayCounter']
+    fwdStart = helperConfig['fwdStart']
+
+    # QuoteHandle
+    rate = marketConfig['rate']['value']
+    spread = marketConfig['spread']['value']
+    rateQuote = ore.QuoteHandle(ore.SimpleQuote(rate))
+    spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
+
+    # Index
+    index = indexes[helperConfig['index']]
+
+    # Discounting curve
+    discountCurve = curves[helperConfig['discountCurve']]
+
+    # Swap rate helper
+    swapRateHelper = ore.SwapRateHelper(
+        rateQuote, tenor, calendar, fixedLegFrequency, convention, dayCounter, index, spreadQuote, fwdStart, discountCurve
+    )
+    return swapRateHelper
+
+
+def createFxSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+    """
+    Create a fx swap rate helper
+
+    Parameters
+    ----------
+    helperConfig : dict
+        The configuration for the helper
+
+    marketConfig : dict
+        The market configuration for the helper
+
+    curves : dict
+        The curves
+    indexes : dict
+        The indexes
+
+    Returns
+    -------
+    ore.FxSwapRateHelper
+        The rate helper
+
+    See Also
+    ----------
+    checkFxSwapRateHelper
+    """
+    fxPoints = marketConfig['fxPoints']['value']
+    spotFx = marketConfig['fxSpot']['value']
+
+    fixingDays = helperConfig['fixingDays']
+    calendar = helperConfig['calendar']
+    convention = helperConfig['convention']
+    endOfMonth = helperConfig['endOfMonth']
+    baseCurrencyAsCollateral = helperConfig['baseCurrencyAsCollateral']
+
+    if 'tenor' in helperConfig.keys():
+        tenor = helperConfig['tenor']
+    else:
+        startDate = ore.Settings.instance().evaluationDate
+        maturityDate = helperConfig['endDate']
+        days = maturityDate - startDate
+        tenor = ore.Period(days, ore.Days)
+
+    # QuoteHandle
+    fwdPointQuote = ore.QuoteHandle(ore.SimpleQuote(fxPoints))
+    spotFxQuote = ore.QuoteHandle(ore.SimpleQuote(spotFx))
+
+    # Discounting curve
+    discountCurve = curves[helperConfig['discountCurve']]
+
+    # FxSwapRateHelper
+    fxSwapRateHelper = ore.FxSwapRateHelper(
+        fwdPointQuote,
+        spotFxQuote,
+        tenor,
+        fixingDays,
+        calendar,
+        convention,
+        endOfMonth,
+        baseCurrencyAsCollateral,
+        discountCurve,
+        calendar
+    )
+    return fxSwapRateHelper
+
+
+def createSofrFutureRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+    """
+    Create a sofr future rate helper
+
+    Parameters
+    ----------
+    helperConfig : dict
+        The configuration for the helper
+
+    marketConfig : dict
+        The market configuration for the helper
+
+    curves : dict
+        The curves
+    indexes : dict
+        The indexes
+
+    Returns
+    -------
+    ore.SofrFutureRateHelper
+        The rate helper
+
+    See Also
+    ----------
+    TODO: checkSofrFutureRateHelper
+    """
+    month = helperConfig['month']
+    year = helperConfig['year']
+    frequency = helperConfig['frequency']
+    # QuoteHandle
+    price = marketConfig['price']
+    convexity = marketConfig['convexity']
+    priceQuote = ore.QuoteHandle(ore.SimpleQuote(price))
+    convexityQuote = ore.QuoteHandle(ore.SimpleQuote(convexity))
+
+    # SofrFutureRateHelper
+    sofrFutureRateHelper = ore.SofrFutureRateHelper(
+        priceQuote,
+        month,
+        year,
+        frequency,
+        convexityQuote
+    )
+    return sofrFutureRateHelper
+
+
+def createTenorBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+    """
+    Create a tenor basis swap rate helper
+
+    Parameters
+    ----------
+    helperConfig : dict
+        The configuration for the helper
+
+    marketConfig : dict
+        The market configuration for the helper
+
+    curves : dict
+        The curves
+    indexes : dict
+        The indexes
+
+    Returns
+    -------
+    ore.TenorBasisSwapHelper
+        The rate helper
+
+    See Also
+    ----------
+    checkTenorBasisRateHelper
+    """
+    tenor = helperConfig['tenor']
+    spreadOnShort = helperConfig['spreadOnShort']
+
+    # Index
+    longIndex = indexes[helperConfig['longIndex']]
+    shortIndex = indexes[helperConfig['shortIndex']]
+
+    # QuoteHandle
+    spread = marketConfig['spread']['value']
+    spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
+
+    # Discounting curve
+    discountCurve = curves[helperConfig['discountCurve']]
+
+    # TenorBasisSwapHelper
+    tenorBasisSwapHelper = ore.TenorBasisSwapHelper(
+        spreadQuote,
+        tenor,
+        longIndex,
+        shortIndex,
+        ore.Period(),
+        discountCurve,
+        spreadOnShort,
+        True
+    )
+
+    return tenorBasisSwapHelper
+
+
+def createCrossCcyFixFloatSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+    """
+    Create a cross currency fix float swap rate helper
+
+    Parameters
+    ----------
+    helperConfig : dict
+        The configuration for the helper        
+
+    marketConfig : dict
+        The market configuration for the helper
+
+    curves : dict
+        The curves
+    indexes : dict
+        The indexes
+
+    Returns
+    -------
+    ore.CrossCcyFixFloatSwapHelper
+        The rate helper
+
+    See Also
+    ----------
+    checkCrossCcyFixFloatSwapRateHelper
+    """
+    tenor = helperConfig['tenor']
+    dayCounter = helperConfig['dayCounter']
+    settlementDays = helperConfig['settlementDays']
+    endOfMonth = helperConfig['endOfMonth']
+    convention = helperConfig['convention']
+    fixedLegFrequency = helperConfig['fixedLegFrequency']
+    fixedLegCurrency = helperConfig['fixedLegCurrency']
+    calendar = helperConfig['calendar']
+
+    # QuoteHandle
+    rate = marketConfig['rate']['value']
+    spotFx = marketConfig['fxSpot']['value']
+    spread = marketConfig['spread']['value']
+
+    rateQuote = ore.QuoteHandle(ore.SimpleQuote(rate))
+    spotFxQuote = ore.QuoteHandle(ore.SimpleQuote(spotFx))
+    spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
+
+    # Index
+    index = indexes[helperConfig['index']]
+
+    # Discounting curve
+    discountCurve = curves[helperConfig['discountCurve']]
+
+    # CrossCcyFixFloatSwapHelper
+    crossCcyFixFloatSwapHelper = ore.CrossCcyFixFloatSwapHelper(
+        rateQuote,
+        spotFxQuote,
+        settlementDays,
+        calendar,
+        convention,
+        tenor,
+        fixedLegCurrency,
+        fixedLegFrequency,
+        convention,
+        dayCounter,
+        index,
+        discountCurve,
+        spreadQuote,
+        endOfMonth
+    )
+    return crossCcyFixFloatSwapHelper
+
+
+def createCrossCcyBasisSwapRateHelper(helperConfig: dict, marketConfig: dict, curves: dict, indexes: dict, *args, **kwargs):
+    """
+    Create a cross currency basis swap rate helper
+
+    Parameters
+    ----------
+    helperConfig : dict
+        The configuration for the helper
+
+    marketConfig : dict
+        The market configuration for the helper
+        - spread : float
+            The spread
+
+    curves : dict
+        The curves
+    indexes : dict
+        The indexes
+
+    Returns
+    -------
+    ore.CrossCcyBasisSwapHelper
+        The rate helper
+
+    See Also
+    ----------
+    checkCrossCcyBasisSwapRateHelper
+    """
+    tenor = helperConfig['tenor']
+    calendar = helperConfig['calendar']
+    settlementDays = helperConfig['settlementDays']
+    endOfMonth = helperConfig['endOfMonth']
+    convention = helperConfig['convention']
+
+    # Discout curves
+    flatDiscountCurve = curves[helperConfig['discountCurve']]
+    spreadDiscountCurve = curves[helperConfig['discountCurve']]
+
+    # Index
+    flatIndex = indexes[helperConfig['flatIndex']]
+    spreadIndex = indexes[helperConfig['spreadIndex']]
+
+    # QuoteHandle
+    spread = marketConfig['spread']['value']
+    spreadQuote = ore.QuoteHandle(ore.SimpleQuote(spread))
+
+    # CrossCcyBasisSwapHelper
+    crossCcyBasisSwapHelper = ore.CrossCcyBasisSwapHelper(
+        spreadQuote,
+        tenor,
+        calendar,
+        settlementDays,
+        flatIndex,
+        spreadIndex,
+        flatDiscountCurve,
+        spreadDiscountCurve,
+        endOfMonth,
+        convention
+    )
+    return crossCcyBasisSwapHelper
```

## Comparing `curveengine-1.1.0.dist-info/METADATA` & `curveengine-1.1.1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
-Name: curveengine
-Version: 1.1.0
-Summary: A simple curve bootstraping tool based on ORE/QuantLib
-Author: Jose Melo
-Author-email: jmelo@live.cl
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
-Requires-Dist: open-source-risk-engine
-
-# CurveEngine
-
-A simple curve bootstrapping tool. It uses ORE as backend and parses configuration files and transform them into QL/ORE objects.
-
-For examples, visit https://github.com/jmelo11/curveengine
-
+Metadata-Version: 2.1
+Name: curveengine
+Version: 1.1.1
+Summary: A simple curve bootstraping tool based on ORE/QuantLib
+Author: Jose Melo
+Author-email: jmelo@live.cl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Requires-Dist: open-source-risk-engine
+
+# CurveEngine
+
+A simple curve bootstrapping tool. It uses ORE as backend and parses configuration files and transform them into QL/ORE objects.
+
+For examples, visit https://github.com/jmelo11/curveengine
+
```

## Comparing `curveengine-1.1.0.dist-info/RECORD` & `curveengine-1.1.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-curveengine/__init__.py,sha256=95wOEVVHXQrJ8qWI3NUwOou1Lh4zJnueSSLIIGRjPHk,803
-curveengine/engine.py,sha256=XHHYfmaJh_5hdnZhwN9FEgZxoZM_C3jTnMzkk0-Fpeg,7755
-curveengine/parsing/__init__.py,sha256=oMHj2EG6yBaqLIHKgtSYqTMLevQZC7RnDiO-BdfnJyY,266
-curveengine/parsing/checks.py,sha256=Ait6aJlr2c_4T4pBKIQGM8S56_5u6WXsluwzHnbdrNI,32971
-curveengine/parsing/enums.py,sha256=FGf8LCypnqyrnWmmL-iP5qLxuoAfXhTqtPqssa9MGHo,3462
-curveengine/parsing/others.py,sha256=CuIzwnfqlzX5dTT2vLAgzWlMaoqVBNwfxfO3f5FzksM,4115
-curveengine/parsing/parsers.py,sha256=WTbJGNMPQUyWCFubh-WKh7kcNfqfL4k1aVx5PvgpdTc,7673
-curveengine/parsing/ratehelpers.py,sha256=9QwVqsTawsxvTSbjGuZOtuAkbJpa1o99AykOOQtxIW8,13513
-curveengine-1.1.0.dist-info/METADATA,sha256=rZDfuMLyOCSJks0PTNZtAV05F1JwFOj3rX4okSeuaPQ,532
-curveengine-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-curveengine-1.1.0.dist-info/top_level.txt,sha256=LK8Ltzj4yLB5cfrjUzMY4Uokv2JNYXqgbUzChD4c92c,12
-curveengine-1.1.0.dist-info/RECORD,,
+curveengine/__init__.py,sha256=fG7Ka2v7aTn4pF7lI0zG-neRIZUS8vm6EyF0cxUrCHo,816
+curveengine/engine.py,sha256=ivxgjZjGf8S9UzSaOg9ZJX6Mj-jMVHDQAP24TlcLsZE,7953
+curveengine/parsing/__init__.py,sha256=jiYxFpB8cxfRiLTIomE7LguueKAKylTb2vrbrj8j1RU,272
+curveengine/parsing/checks.py,sha256=pJfMKomtCgJEbfUuAQGUNG2O4ErWSTfBR3is-04sMX8,34375
+curveengine/parsing/enums.py,sha256=nYlnk3PCV4Jax0Tu68Sh-qpBRR3DWFGXX0W3wI9n0xY,3617
+curveengine/parsing/others.py,sha256=2vNml3mjqUnX9D5Yyce9Y15sWv5JmC8RyS4D0EJH4mI,4257
+curveengine/parsing/parsers.py,sha256=61tqPjHveE6Duu1UJjROWwLlk8sFd_UEpjiVbpdj8pc,8004
+curveengine/parsing/ratehelpers.py,sha256=JBZLC0f634GGF-3MAU6f7u3jO4OSvN8Rcf__Wwn04fA,14022
+curveengine-1.1.1.dist-info/METADATA,sha256=iRO33oBEoHZurvJB1PIbaYJ8YsOyVZ0WU_BhaTgl_Nk,550
+curveengine-1.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+curveengine-1.1.1.dist-info/top_level.txt,sha256=LK8Ltzj4yLB5cfrjUzMY4Uokv2JNYXqgbUzChD4c92c,12
+curveengine-1.1.1.dist-info/RECORD,,
```

