# Comparing `tmp/geotexxx-0.0.1.tar.gz` & `tmp/geotexxx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotexxx-0.0.1.tar", last modified: Mon Feb 27 10:14:40 2023, max compression
+gzip compressed data, was "geotexxx-0.1.3.tar", last modified: Tue May 30 09:32:45 2023, max compression
```

## Comparing `geotexxx-0.0.1.tar` & `geotexxx-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 10:14:40.916181 geotexxx-0.0.1/
--rw-rw-rw-   0        0        0    13954 2022-04-20 15:29:56.000000 geotexxx-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3783 2023-02-27 10:14:40.912963 geotexxx-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3525 2023-01-20 11:30:06.000000 geotexxx-0.0.1/README.md
--rw-rw-rw-   0        0        0      405 2023-02-27 10:14:14.000000 geotexxx-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-27 10:14:40.916181 geotexxx-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-27 10:14:40.892067 geotexxx-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-02-27 10:14:40.899057 geotexxx-0.0.1/src/geotexxx/
--rw-rw-rw-   0        0        0        0 2023-02-24 15:44:18.000000 geotexxx-0.0.1/src/geotexxx/__init__.py
--rw-rw-rw-   0        0        0    91544 2023-02-27 08:51:03.000000 geotexxx-0.0.1/src/geotexxx/gefxml_reader.py
-drwxrwxrwx   0        0        0        0 2023-02-27 10:14:40.909967 geotexxx-0.0.1/src/geotexxx.egg-info/
--rw-rw-rw-   0        0        0     3783 2023-02-27 10:14:40.000000 geotexxx-0.0.1/src/geotexxx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-02-27 10:14:40.000000 geotexxx-0.0.1/src/geotexxx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 10:14:40.000000 geotexxx-0.0.1/src/geotexxx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-02-27 10:14:40.000000 geotexxx-0.0.1/src/geotexxx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-27 10:14:40.000000 geotexxx-0.0.1/src/geotexxx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 09:32:45.236550 geotexxx-0.1.3/
+-rw-rw-rw-   0        0        0    13954 2022-04-20 15:29:56.000000 geotexxx-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3831 2023-05-30 09:32:45.235548 geotexxx-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3573 2023-04-04 15:09:05.000000 geotexxx-0.1.3/README.md
+-rw-rw-rw-   0        0        0      405 2023-05-30 09:32:28.000000 geotexxx-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 09:32:45.237552 geotexxx-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 09:32:45.200669 geotexxx-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 09:32:45.213048 geotexxx-0.1.3/src/geotexxx/
+-rw-rw-rw-   0        0        0        0 2023-02-24 15:44:18.000000 geotexxx-0.1.3/src/geotexxx/__init__.py
+-rw-rw-rw-   0        0        0   101264 2023-05-30 09:31:50.000000 geotexxx-0.1.3/src/geotexxx/gefxml_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:32:45.233170 geotexxx-0.1.3/src/geotexxx.egg-info/
+-rw-rw-rw-   0        0        0     3831 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 09:32:45.000000 geotexxx-0.1.3/src/geotexxx.egg-info/top_level.txt
```

### Comparing `geotexxx-0.0.1/LICENSE.txt` & `geotexxx-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geotexxx-0.0.1/PKG-INFO` & `geotexxx-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: geotexxx
-Version: 0.0.1
+Version: 0.1.3
 Summary: Package om geotechnisch grondonderzoek te verwerken
 Author-email: Thomas van der Linden <t.van.der.linden@amsterdam.nl>
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gefxml_reader
 
 Application to read geotechnical CPT and bore data in GEF or BRO XML format
 
 ## Dependecies
 See environment.yml
 
 ## Instruction
 Create an empty object:
+`from geotexxx.gefxml_reader import Cpt, Bore`
 `test = Cpt()` or `test = Bore()`    
 Read in a file:
 `test.load_gef(filename)` or `test.load_xml(filename)`  
 Create a plot in folder ./output
 `test.plot()`  
 
 gui_plot.py provides a point and click interface to make plots of individual files or of all the files in a folder
```

### Comparing `geotexxx-0.0.1/README.md` & `geotexxx-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Application to read geotechnical CPT and bore data in GEF or BRO XML format
 
 ## Dependecies
 See environment.yml
 
 ## Instruction
 Create an empty object:
+`from geotexxx.gefxml_reader import Cpt, Bore`
 `test = Cpt()` or `test = Bore()`    
 Read in a file:
 `test.load_gef(filename)` or `test.load_xml(filename)`  
 Create a plot in folder ./output
 `test.plot()`  
 
 gui_plot.py provides a point and click interface to make plots of individual files or of all the files in a folder
```

### Comparing `geotexxx-0.0.1/src/geotexxx/gefxml_reader.py` & `geotexxx-0.1.3/src/geotexxx/gefxml_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from matplotlib.gridspec import GridSpec
 import matplotlib.pyplot as plt
 from xml.etree.ElementTree import ElementTree
 import xml.etree.ElementTree as ET
 import pyproj
 import ast
 import os
+from datetime import datetime
 
 @dataclass
 class Test():
     def __init__(self):
         self.type = str()
     
     def type_from_gef(self, gefFile, fromFile=True):
@@ -265,14 +266,87 @@
         self.filename = None
         self.companyid = None
         self.projectid = None
         self.projectname = None
         self.filedate = {}
         self.testdate = {}
 
+    def load_son(self, sonFile, checkAddFrictionRatio=False, checkAddDepth=False, fromFile=True):
+        filename_pattern = re.compile(r'(.*[\\/])*(?P<filename>.*)\.')
+        testid_pattern = re.compile(r'Sondering\s*:\s*(?P<testid>.*)\s*')
+        date_pattern = re.compile(r'Datum\s*:\s*(?P<date>[\d-]*)')
+        xy_id_pattern = re.compile(r'')
+        z_id_pattern = re.compile(r'Maaiveld t.o.v. referentievlak\s*:\s*(?P<zid>\d*\.?\d*)\s*[\[\]mM\s]\s*')
+        companyid_pattern = re.compile(r'Bedrijf\s*:\s*(?P<companyid>.*)\s*') 
+        projectid_pattern = re.compile(r'Opdracht\s*:\s*(?P<testid>.*)\s*')
+        data_pattern = re.compile(r'Aantal meetregels\s*(bij deze sondering\.)*\s*(?P<data>[-\d\s\.]+)\s*[-=]*') # TODO: \s*(bij deze sondering\.)?
+
+        if fromFile:
+            with open(sonFile) as f:
+                son_raw = f.read()
+        else:
+            son_raw = sonFile
+
+        try:
+            #TODO: let op, er kunnen meerder sonderingen in een bestand zitten
+            match = re.search(data_pattern, son_raw)
+            data = match.group('data')
+        
+            columns= ['penetrationLength', 'coneResistance', 'localFriction', 'frictionRatio']
+            self.data = pd.read_csv(StringIO(data), sep=' ', skipinitialspace=True, lineterminator='\n', header=None)
+            self.data.columns = [col for i, col in enumerate(columns) if i < len(self.data.columns)]
+            self.data = self.data.astype(float, errors='ignore')
+        except:
+            pass
+
+        try:
+            match = re.search(testid_pattern, son_raw)
+            self.testid = match.group('testid')
+        except:
+            pass
+
+        try:
+            match = re.search(z_id_pattern, son_raw)
+            self.groundlevel = float(match.group('zid'))
+        except:
+            pass
+
+        try:
+            match = re.search(companyid_pattern, son_raw)
+            self.companyid = match.group('zid')
+        except:
+            pass
+
+        try:
+            self.date = {'year': None, 'month': None, 'day': None}
+            match = re.search(date_pattern, son_raw)
+            date = datetime.strptime(match.group('date'), '%Y-%m-%d').date()
+            self.date['year'] = date.year
+            self.date['month'] = date.month
+            self.date['day'] = date.day
+        except:
+            pass
+
+        try:
+            self.date = {'year': None, 'month': None, 'day': None}
+            match = re.search(date_pattern, son_raw)
+            date = datetime.strptime(match.group('date'), '%d-%m-%Y').date()
+            self.date['year'] = date.year
+            self.date['month'] = date.month
+            self.date['day'] = date.day
+        except:
+            pass
+
+
+        if checkAddDepth:
+            self.check_add_depth()
+        if checkAddFrictionRatio:
+            self.check_add_frictionRatio()
+
+
     def load_xml(self, xmlFile, checkAddFrictionRatio=False, checkAddDepth=False, fromFile=True):
 
         # lees een CPT in vanuit een BRO XML
         tree = ElementTree()
         if fromFile:
             # Standaard functionaliteit voor wanneer de XML uit een file wordt gelezen
             tree.parse(xmlFile)
@@ -482,16 +556,16 @@
             42: 'Orientation between X axis inclination and North. See section 3.7 Sept 2006 N'
         }
 
         self.metadata_from_gef(gefFile, fromFile)
 
         data_pattern = re.compile(r'#EOH\s*=\s*(?P<data>(.*\n)*)')
 
-        columnvoid_pattern = re.compile(r'#COLUMNVOID\s*=\s*(?P<columnnr>\d*),\s*(?P<voidvalue>.*)\s*')
-        columninfo_pattern = re.compile(r'#COLUMNINFO\s*=\s*(?P<columnnr>\d*),\s*(?P<unit>.*),\s*(?P<parameter>.*),\s*(?P<quantitynr>\d*)\s*')
+        columnvoid_pattern = re.compile(r'#COLUMNVOID\s*=\s*(?P<columnnr>\d*)\s*,\s*(?P<voidvalue>.*)\s*')
+        columninfo_pattern = re.compile(r'#COLUMNINFO\s*=\s*(?P<columnnr>\d*)\s*,\s*(?P<unit>.*)\s*,\s*(?P<parameter>.*)\s*,\s*(?P<quantitynr>\d*)\s*')
         columnseparator_pattern = re.compile(r'#COLUMNSEPARATOR\s*=\s*(?P<columnseparator>.*)\s*')
         recordseparator_pattern = re.compile(r'#RECORDSEPARATOR\s*=\s*(?P<recordseparator>.*)\s*')
 
         if fromFile:
             with open(gefFile) as f:
                 gef_raw = f.read()
         else:
@@ -838,15 +912,15 @@
         return self.data
 
     def interpret_robertson(self):
         # formula from: Soil Behaviour Type from the CPT: an update 
         # http://www.cpt-robertson.com/PublicationsPDF/2-56%20RobSBT.pdf
 
         # non-normalized soil behaviour types omgezet naar Nederlandse namen
-        # TODO: nummers toevoegen
+        # TODO: SBT-nummers toevoegen
         sbtDict = {
             'veen': 3.6,
             'klei': 2.95,
             'zwakKleiigSilt': 2.6,
             'zwakSiltigZand': 2.05,
             'sterkSiltigZand': 1.31,
             'zand': 0,
@@ -874,23 +948,26 @@
         self.companyid = None
         self.testid = None
         self.easting = None
         self.northing = None
         self.groundlevel = None
         self.srid = None
         self.testid = None
-        self.date = {}
+        self.date = {'year': None, 'month': None, 'day': None}
         self.finaldepth = None
         self.soillayers = {}
         self.analyses = []
+        self.complexAnalyses = {}
         self.metadata = {}
         self.descriptionquality = None
 
     def load_xml(self, xmlFile, fromFile=True):
-
+        
+        complexAnalyses = {}
+        
         # lees een boring in vanuit een BRO XML
         # TODO: werkt nog niet voor IMBRO_A
         if fromFile:
             # Standaard functionaliteit voor wanneer de XML uit een file wordt gelezen
             tree = ElementTree()
             tree.parse(xmlFile)
             root = tree.getroot()
@@ -934,18 +1011,38 @@
                         soillayers.append({re.sub(r'{.*}', '', p.tag) : re.sub(r'\s*', '', p.text) for p in child.iter() if p.text is not None})
                 # zet soillayers om in dataframe om het makkelijker te verwerken
                 self.soillayers[descriptionLocation] = pd.DataFrame(soillayers) 
 
             elif 'boreholeSampleAnalysis' in element.tag:
                 for child in element.iter():
                     if 'investigatedInterval' in child.tag:
-                        self.analyses.append({re.sub(r'{.*}', '', p.tag) : re.sub(r'\s*', '', p.text) for p in child.iter() if p.text is not None})
+                        # dit is een eenvoudige manier om eenvoudige analyses in een tabel te zetten
+                        self.analyses.append({re.sub(r'{.*}', '', p.tag) : re.sub(r'\s*', '', p.text) for p in child.iter() if p.text is not None and p.tag not in ['settlementCharacteristicsDetermination']})
+                        
+                        # de eenvoudige methode werkt niet goed voor complexe proeven met bijvoorbeeld verschillende trappen
+                        for baby in child.iter():
+                            if 'settlementCharacteristicsDetermination' in baby.tag:
+                                sampleNumber = len(complexAnalyses.keys())
+                                complexAnalyses[sampleNumber] = {}
+                                for determination in baby.iter():
+                                    if 'determinationStep' in determination.tag:
+                                        for x in determination.iter():
+                                            if 'stepNumber' in x.tag:
+                                                stepNumber = x.text
+                                        complexAnalyses[sampleNumber][stepNumber] = {re.sub(r'{.*}', '', p.tag) : re.sub(r'\s*', '', p.text) for p in determination.iter() if p.text is not None}
+
                 self.analyses = pd.DataFrame().from_dict(self.analyses)
                 self.analyses = self.analyses.astype(float, errors='ignore')
 
+                for key, values in complexAnalyses.items():
+                    complexAnalysis = pd.DataFrame().from_dict(values)
+                    complexAnalysis = complexAnalysis.astype(float, errors='ignore')
+                    self.complexAnalyses[key] = complexAnalysis
+
+
         self.metadata = {"easting": self.easting, "northing": self.northing, "groundlevel": self.groundlevel, "testid": self.testid, "date": self.date, "finaldepth": self.finaldepth}
 
         for descriptionLocation, soillayers in self.soillayers.items():
             # TODO: mogelijk verwarrend om soillayers en self.soillayers te combineren
             # voeg de componenten toe t.b.v. plot       
             self.soillayers[descriptionLocation] = self.add_components(soillayers)
 
@@ -1029,16 +1126,16 @@
             '7': 'organische stof',
             '8': 'zandmediaan',
             '9': 'grindmediaan'
         }
 
         data_pattern = re.compile(r'#EOH\s*=\s*(?P<data>(.*\n)*)')
 
-        columnvoid_pattern = re.compile(r'#COLUMNVOID\s*=\s*(?P<columnnr>\d*),\s*(?P<voidvalue>.*)\s*')
-        columninfo_pattern = re.compile(r'#COLUMNINFO\s*=\s*(?P<columnnr>\d*),\s*(?P<unit>.*),\s*(?P<parameter>.*),\s*(?P<quantitynr>\d*)\s*')
+        columnvoid_pattern = re.compile(r'#COLUMNVOID\s*=\s*(?P<columnnr>\d*)\s*,\s*(?P<voidvalue>.*)\s*')
+        columninfo_pattern = re.compile(r'#COLUMNINFO\s*=\s*(?P<columnnr>\d*)\s*,\s*(?P<unit>.*)\s*,\s*(?P<parameter>.*)\s*,\s*(?P<quantitynr>\d*)\s*')
         columnseparator_pattern = re.compile(r'#COLUMNSEPARATOR\s*=\s*(?P<columnseparator>.*)\s*')
         recordseparator_pattern = re.compile(r'#RECORDSEPARATOR\s*=\s*(?P<recordseparator>.*)\s*')
 
         self.metadata_from_gef(gefFile)
 
         with open(gefFile) as f:
             gef_raw = f.read()
@@ -1188,119 +1285,217 @@
         materials = {0: 'grind', 1: 'zand', 2: 'klei', 3: 'leem', 4: 'veen', 5: 'silt', 6: 'overig'}
         colorsDict = {0: "orange", 1: "yellow", 2: "green", 3: "", 4: "brown", 5: "grey", 6: "black"} # NEN-EN-ISO 14688-1 style, geen leem
         colorsDictNEN5104 = {0: "grey", 1: "yellow", 2: "steelblue", 3: "yellowgreen", 4: "brown", 5: "", 6: "black"} # NEN5104 style, geen silt
 
         hatchesDict = {0: "ooo", 1: "...", 2: "///", 3:"", 4: "---", 5: "|||", 6: ""} # NEN-EN-ISO 14688-1 style
         hatchesDictNEN5104 = {0: "ooo", 1: "...", 2: "///", 3:"\\\\\\", 4: "---", 5: "|||", 6: ""} # NEN-EN-ISO 14688-1 style
 
+        plotbareData = ['tertiaryConstituent', 'colour', 'dispersedInhomogeneity', 'carbonateContentClass',
+                            'organicMatterContentClass', 'mixed', 'sandMedianClass', 'grainshape', # TODO: sandMedianClass kan ook mooi visueel
+                            'sizeFraction', 'angularity', 'sphericity', 'fineSoilConsistency',
+                            'organicSoilTexture', 'organicSoilConsistency', 'peatTensileStrength', 'waterContent', 'volumetricMassDensity', 
+                            'volumetricMassDensitySolids', 'beginDepth', 'endDepth', 'maximumUndrainedShearStrength']
+
         # als er een veld- en een labbeschrijving is, dan maken we meer kolommen
         nrOfLogs = len(self.soillayers.keys())
 
         # figuur breedte instellen, 6 werkt goed voor alleen een veldbeschrijving
         if nrOfLogs == 1:
             width = 6
+            ncols = 2
             width_ratios = [1, 3] # boorstaat, beschrijving
 
         # in geval van lab is het gecompliceerder
-        # als er alleen veld- en labbeschrijving is, geen testen, dan is self.analyses nog een dict (niet omgezet in DataFrame)
-        elif isinstance(self.analyses, dict):
+        # als er alleen veld- en labbeschrijving is, geen testen, dan is self.analyses niet omgezet in DataFrame
+        if nrOfLogs == 2:
             width = 18
+            ncols = 4
             width_ratios = [1, 3, 0.5, 3]
 
-        # zijn er wel testen, dan alleen de numerieke kolommen selecteren voor plot
-        elif isinstance(self.analyses, pd.DataFrame):
-            # filter alleen de numerieke kolommen
-            self.analyses = self.analyses.apply(lambda x: pd.to_numeric(x.astype(str).str.replace(',',''), errors='coerce')).dropna(axis='columns', how='all')
+        # zijn er wel testen, dan is self.analyses wél een DataFrame
+        if isinstance(self.analyses, pd.DataFrame): 
+            # alleen de numerieke kolommen selecteren voor plot
+            # maak een nieuw dataframe voor de eenvoudige plots (TODO: kan ook gebruikt worden als aparte output)
+            plotTabel = self.analyses.apply(lambda x: pd.to_numeric(x.astype(str).str.replace(',',''), errors='coerce')).dropna(axis='columns', how='all')
+            plotbareData = [data for data in plotbareData if data in plotTabel.columns] # bepaal welke kolommen aanwezig zijn in het dataframe
+            plotTabel = plotTabel[plotbareData] # filter alleen de plotbare data
 
-            width = 24
+            width = 24 # TODO: dynamisch maken afhankelijk van aantal kolommen met data
             # voeg kolommen toe voor de plot van de meetwaarden
-            # beginDepth en endDepth doen niet mee
-            width_ratios = [1, 3, 0.5, 3, 1, 1] # TODO: lengte moet afhankelijk van aantal meetkolommen
-            nrOfLogs += 1 # TODO: waarde moet afhankelijk van aantal meetkolommen
+            nrOfPlotbareData = len([col for col in plotTabel.columns if col in plotbareData]) # voor elke kolom met plotbare data een plot toevoegen
+            ncols += nrOfPlotbareData
+            width_ratios.extend([1] * nrOfPlotbareData) 
+        else:
+            plotTabel = None
 
         # maak een diagram 
-        fig = plt.figure(figsize=(width, max(self.finaldepth + 2, 4.5))) 
-        gs = GridSpec(nrows=2, ncols=2 * nrOfLogs, height_ratios=[self.finaldepth, 2], width_ratios=width_ratios, figure=fig)
+        if self.finaldepth is not None:
+            fig = plt.figure(figsize=(width, max(self.finaldepth + 2, 4.5)))
+            gs = GridSpec(nrows=2, ncols=ncols, height_ratios=[self.finaldepth, 2], width_ratios=width_ratios, figure=fig)
+        else:
+            fig = plt.figure(figsize=(width, 4.5))
+            gs = GridSpec(nrows=2, ncols=ncols, height_ratios=[4.5, 2], width_ratios=width_ratios, figure=fig)
+        
         axes = []
 
         # als er veld- en labbeschrijving is, dan worden deze apart geplot
         for i, [descriptionLocation, soillayers] in enumerate(self.soillayers.items()):
             axes.append(fig.add_subplot(gs[0, i * 2])) # boorstaat 
             axes.append(fig.add_subplot(gs[0, i * 2 + 1], sharey=axes[0])) # toelichting 
         
             # maak een eenvoudige plot van een boring
-            uppers = list(soillayers["upper_NAP"])
-            lowers = list(soillayers["lower_NAP"])
+            if "upper_NAP" in soillayers.columns:
+                uppers = list(soillayers["upper_NAP"])
+                lowers = list(soillayers["lower_NAP"])
+            else:
+                uppers = list(soillayers["upper"])
+                lowers = list(soillayers["lower"])
             components = list(soillayers["components"])
 
             for upper, lower, component in reversed(list(zip(uppers, lowers, components))):
                 left = 0
                 try: # TODO: kan dit beter. Gemaakt vanwege een geval met component = nan (lab boring van Anthony Moddermanstraat)
                     for comp, nr in component.items():
                         barPlot = axes[i * 2].barh(lower, width=comp, left=left, height=upper-lower, color=colorsDict[nr], hatch=hatchesDict[nr], edgecolor="black", align="edge")
                         left += comp
                 except:
                     pass
-
-            axes[i * 2].set_ylim([self.groundlevel - self.finaldepth, self.groundlevel])
+            if self.groundlevel is not None:
+                axes[i * 2].set_ylim([self.groundlevel - self.finaldepth, self.groundlevel])
             axes[i * 2].set_xticks([])
             axes[i * 2].set_ylabel('diepte [m t.o.v. NAP]')
             plt.title(descriptionLocation) 
 
             # voeg de beschrijving toe
             for layer in soillayers.itertuples():
-                y = (getattr(layer, "lower_NAP") + getattr(layer, "upper_NAP")) / 2
+                if "upper_NAP" in soillayers.columns:
+                    y = (getattr(layer, "lower_NAP") + getattr(layer, "upper_NAP")) / 2
+                else:
+                    y = (getattr(layer, "lower") + getattr(layer, "upper")) / 2
                 propertiesText = ""
                 # TODO: deze materialproperty werken niet voor SIKB
-                for materialproperty in ['tertiaryConstituent', 'colour', 'dispersedInhomogeneity', 'carbonateContentClass',
-                                            'organicMatterContentClass', 'mixed', 'sandMedianClass', 'grainshape', # TODO: sandMedianClass kan ook mooi visueel
-                                            'sizeFraction', 'angularity', 'sphericity', 'fineSoilConsistency',
-                                            'organicSoilTexture', 'organicSoilConsistency', 'peatTensileStrength']:
+                for materialproperty in plotbareData:
                     # TODO: dit werkt nog niet goed
                     if materialproperty in soillayers.columns:
                         value = getattr(layer, materialproperty)
                         try:
                             np.isnan(value)
                         except:
                             propertiesText += f', {value}'
-                text = f'{getattr(layer, "soilName")}{propertiesText}'
-                axes[i * 2 + 1].text(0, y, text, wrap=True)
+                if "soilName" in soillayers.columns:
+                    text = f'{getattr(layer, "soilName")}{propertiesText}'
+                    axes[i * 2 + 1].text(0, y, text, wrap=True)
                 # verberg de assen van de beschrijving
                 axes[i * 2 + 1].set_axis_off() 
 
                 plt.title(descriptionLocation)
         
         # als er analyses zijn uitgevoerd, deze ook toevoegen
         # TODO: filteren welke wel / niet of samen
         # TODO: korrelgrootte uit beschrijving toevoegen?
-        if isinstance(self.analyses, pd.DataFrame):
-            averageDepth = self.groundlevel - self.analyses[['beginDepth', 'endDepth']].mean(axis=1)
+        if isinstance(plotTabel, pd.DataFrame):
+            averageDepth = self.groundlevel - plotTabel[['beginDepth', 'endDepth']].mean(axis=1)
             # voeg axes toe voor de plots
             # TODO: dit ook werkend maken voor korrelgrootteverdelingen (zie Vreeswijkpad voor voorbeeldbestanden)
-            for j, col in enumerate([col for col in self.analyses.columns if col not in ['beginDepth', 'endDepth']]):
+            for j, col in enumerate([col for col in plotTabel.columns if col not in ['beginDepth', 'endDepth']]):
                 axes.append(fig.add_subplot(gs[0, i * 2 + 2 + j], sharey=axes[0]))
-                axes[i * 2 + 2 + j].plot(self.analyses[col], averageDepth, '.')
+                axes[i * 2 + 2 + j].plot(plotTabel[col], averageDepth, '.')
                 plt.title(col)
 
         # voeg een stempel toe
         axes.append(fig.add_subplot(gs[1,:])) # stempel
         # verberg de assen van de stempel
         axes[-1].set_axis_off()
         # tekst voor de stempel
+        if not isinstance(self.date, dict):
+            self.date = {'year': None, 'month': None, 'day': None}
         plt.text(0.05, 0.6, f'Boring: {self.testid}\nx-coördinaat: {self.easting}\ny-coördinaat: {self.northing}\nmaaiveld: {self.groundlevel}\nkwaliteit: {self.descriptionquality}\ndatum: {self.date["year"]}-{self.date["month"]}-{self.date["day"]}', fontsize=14, fontweight='bold')
         plt.text(0.05, 0.2, 'Ingenieursbureau Gemeente Amsterdam Vakgroep Geotechniek Python ', fontsize=10)
 
 #        plt.tight_layout() # TODO: werkt niet met text die wrapt
 
         if saveFig:
             plt.savefig(fname=f'{path}/{self.testid}.{outputType}')
             plt.close('all')
 
         return fig
 
+    def plot_samendrukkingsproeven(self, saveFigs=False):
+        figs = []
+        for sampleNumber, complexAnalysis in self.complexAnalyses.items():
+            if self.analyses.loc[sampleNumber, 'analysisType'] == 'zetting':
+                fig = self.plot_samendrukkingsproef(sampleNumber, complexAnalysis, tijdIn='min', saveFig=False, saveData=False)
+                figs.append(fig)
+                if saveFigs:
+                    plt.savefig(f'./samendrukkingsproef_{self.testid}_{sampleNumber}.png')
+                    plt.close('all')
+        return figs
+    
+    def plot_samendrukkingsproef(self, sampleNumber, complexAnalysis, tijdIn='min', saveFig=False, saveData=False):
+        testdf = [] # dataframe om proefresultaten in tabel weg te schrijven
+        # bepaal de monsterhoogte
+        sampleHeight = float(self.analyses.loc[sampleNumber, 'endDepth']) - float(self.analyses.loc[sampleNumber, 'beginDepth'])
+
+        # maak een figuur met boven tijd-zetting en onder belasting-rek
+        fig = plt.figure(figsize=[8, 12]) 
+        gs = GridSpec(nrows=2, ncols=1, figure=fig)
+        ax1 = fig.add_subplot(gs[0, 0])
+        ax2 = fig.add_subplot(gs[1, 0])
+
+        # maak een tijd-zetting plot
+        # voeg de trappen toe aan de plot
+        for stepNumber in complexAnalysis.loc['values'].index:
+            xy = pd.read_csv(StringIO(complexAnalysis.loc['values', stepNumber]), sep=',', lineterminator=';', header=None)
+            # in xml tijd in secondes, omzetten naar minuten of dagen, dat is standaard voor plots
+            if tijdIn == 'min':
+                x = xy[0] / 60
+            elif tijdIn == 'dag':
+                x = xy[0] / 60 / 60 / 24
+            # in xml lineaire rek in %, omzetten naar mm, dat is standaard voor plots. monsterhoogte is in xml in m
+            y = xy[1] / 100 * sampleHeight * 1000
+            ax1.plot(x, y) 
+            xy['stap'] = stepNumber
+            testdf.append(xy)
+
+        # opmaak figuur
+        ax1.invert_yaxis()
+        ax1.set_xlabel(f'Tijd [{tijdIn}]')
+        ax1.set_ylabel('Zetting [mm]')
+        ax1.set_title(f'Tijd-Zetting Boring: {self.testid} Monster: {sampleNumber} Niveau: {float(self.analyses.loc[sampleNumber, "endDepth"]):.2f} - {float(self.analyses.loc[sampleNumber, "beginDepth"]):.2f}')
+
+        # tabel met proefresultaten wegschrijven
+        if saveData:
+            testdf = pd.concat(testdf)
+            testdf.to_csv(f'./tijdzetting_{sampleNumber}.csv', sep=';', decimal=',')
+
+        # maak een belasting-rek plot
+        x, y = [], []
+        # doorloop de stappen
+        for stepNumber in complexAnalysis.loc['values'].index:
+
+            xy = pd.read_csv(StringIO(complexAnalysis.loc['values', stepNumber]), sep=',', lineterminator=';', header=None)
+            # x is de spanning tijdens de trap
+            x.append(float(complexAnalysis.loc['verticalStress', stepNumber]))
+            # y is de rek aan het einde van de trap
+            y.append(float(xy[1].iloc[-1]) / 100) # in xml rek in %, dat omzetten naar een fractie 0-1
+
+        # figuur opmaken
+        ax2.plot(x, y)
+        ax2.set_xscale('log')
+        ax2.set_xlim([1, 1000])
+        ax2.invert_yaxis()
+        ax2.set_xlabel('belasting [kPa]')
+        ax2.set_ylabel('lineaire rek [-]')
+        ax2.set_title(f'Belasting-Rek Boring: {self.testid} Monster: {sampleNumber} Niveau: {float(self.analyses.loc[sampleNumber, "endDepth"]):.2f} - {float(self.analyses.loc[sampleNumber, "beginDepth"]):.2f}')
+
+        if saveFig:
+            plt.savefig(f'./samendrukkingsproef_{self.testid}_{sampleNumber}.png')
+
+        return fig
+
     def from_cpt(self, cpt, interpretationModel='Robertson'):
 
         # maak een object alsof het een boring is
         self.soillayers['cpt']= pd.DataFrame(columns=['geotechnicalSoilName', 'frictionRatio', 'coneResistance', 'upper_NAP', 'lower_NAP'])
         self.soillayers['cpt']['geotechnicalSoilName'] = cpt.data[interpretationModel]
         # TODO frictionRatio en coneResistance horen er eigenlijk niet in thuis, maar zijn handig als referentie
         self.soillayers['cpt'][['frictionRatio', 'coneResistance']] = cpt.data[['frictionRatio', 'coneResistance']]
@@ -1401,15 +1596,15 @@
         return soillayers
 
 @dataclass
 class Multibore():
     def __init__(self):
         self.bores = []
 
-    def load_xml_sikb0101(self, xmlFile, projectName): 
+    def load_xml_sikb0101(self, xmlFile, projectName, saveFiles=True): 
 
         # lees boringen in vanuit een SIKB0101 XML
         # anders dan de BRO komen alle boringen van een project in 1 bestand
         tree = ElementTree()
         tree.parse(xmlFile)
         root = tree.getroot()
 
@@ -1436,15 +1631,14 @@
         geometries = []
         fs = []
         groundlevels = []
         depths = []
         peilbuizen = []
         boorbeschrijvingen = []
         from shapely.geometry import Point
-        import geopandas as gpd
 
 
         for element in root.iter():
             # vul de dictionaries voor de boringen met lagen
             if 'Borehole' in element.tag:
                 for key in element.attrib.keys():
                     if 'id' in key:
@@ -1662,26 +1856,27 @@
         # TODO: de 'urn:imsikb0101:' moeten omgezet worden naar iets anders. ubicode is bijv. VerdachteActiviteit 
         # TODO: de 'urn:imsikb0101:' heel veel domeintabellen moeten nog gedownload
         columnsDict = {
             'Grondsoort': 'Bodemsoort', 
             'GrondsoortMediaan': 'BodemsoortMediaan',
             'ubicode': 'VerdachteActiviteit'}
         properties.rename(columns=columnsDict, inplace=True)
-        
+
         # make een mapje om bestanden per project (invoer XML) weg te schrijven
-        fileName = xmlFile.split('/')[-1].replace('.xml', '')
-        if not os.path.isdir(f'./output/{projectName}'):
-            os.mkdir(f'./output/{projectName}')
-        if not os.path.isdir(f'./output/{projectName}/{fileName}'):
-            os.mkdir(f'./output/{projectName}/{fileName}')
+        if saveFiles:
+            fileName = xmlFile.split('/')[-1].replace('.xml', '')
+            if not os.path.isdir(f'./output/{projectName}'):
+                os.mkdir(f'./output/{projectName}')
+            if not os.path.isdir(f'./output/{projectName}/{fileName}'):
+                os.mkdir(f'./output/{projectName}/{fileName}')
 
         aantal_boringen = len(properties['bore'].unique())
         
         for boreId, boreData in properties.groupby('bore'): 
-            
+
             if type(boreId) != float: # er kan een nan inzitten, dat is data type float
                 try: 
                     print(f'{boreId} van {aantal_boringen} boringen')
 
                     # TODO: zou dit beter zijn als method voor de class Bore?
                     bore = Bore()
                     bore.soillayers = {}
@@ -1689,20 +1884,20 @@
                     layers = {}
                     for layerNr, layerData in boreData.groupby('layer'):
                         layerData = layerData.max(skipna=True)
                         layerData = code2text(layerData)
                         layerData = Bodemsoort2components(layerData)
                         layerData.dropna(inplace=True)
 
-                        if all(param in layerData.index for param in ['upper', 'lower', 'Bodemsoort']): # anders plot het later niet
+                        if all(param in layerData.index for param in ['upper', 'lower', 'Bodemsoort']): # anders plot het later niet of niet goed
                             layers[layerNr] = layerData
                     
                     bore.soillayers['veld'] = pd.DataFrame().from_dict(layers).T
                     bore.soillayers['veld'].rename(columns={'Bodemsoort': 'soilName'}, inplace=True)
-                
+
                     # soms is de lower kleiner dan upper, dat is niet volgens de conventie
                     # dan de kolommen omdraaien
                     if bore.soillayers['veld']['upper'].gt(bore.soillayers['veld']['lower']).all():
                         bore.soillayers['veld'].rename(columns={'upper': 'lower', 'lower': 'upper'}, inplace=True)
 
                     try:
                         bore.testid = boreXYZ[boreId]['name']
@@ -1721,17 +1916,14 @@
                         bore.easting = 0
                         bore.northing = 0                    
 
                     if bore.groundlevel is not None and 'upper' in bore.soillayers['veld'].columns:
                         bore.soillayers['veld']['upper_NAP'] = bore.groundlevel - bore.soillayers['veld']['upper']
                         bore.soillayers['veld']['lower_NAP'] = bore.groundlevel - bore.soillayers['veld']['lower']
                         bore.finaldepth = bore.soillayers['veld']['upper_NAP'].max() - bore.soillayers['veld']['lower_NAP'].min() # lengte van de boring
-                        self.bores.append(bore)
-                    else:
-                        self.bores.append(bore)
 
                     try:
                         onderkant = bore.soillayers['veld']['lower_NAP'].min()
                     except:
                         onderkant = None
                     
                     # check of er een peilbuis aanwezig is
@@ -1739,15 +1931,17 @@
                         peilbuisAanwezig = True
                     else:
                         peilbuisAanwezig = False
 
 
                     # schrijf een csv weg als er lagen in de boorbeschrijving zitten. Als je alles meteen omzet naar een plot, dan crasht het bij grote hoeveelheden boringen
                     if len(bore.soillayers['veld']) > 0:
-                        bore.soillayers['veld'].to_csv(f'./output/{projectName}/{fileName}/{bore.testid}_{boreId}.csv', sep=';')
+                        self.bores.append(bore)
+                        if saveFiles:
+                            bore.soillayers['veld'].to_csv(f'./output/{projectName}/{fileName}/{bore.testid}_{boreId}.csv', sep=';')
                         boorbeschrijving = True
                     else:
                         boorbeschrijving = False
 
                     geometries.append(Point(bore.easting, bore.northing)) 
                     xs.append(bore.easting)
                     ys.append(bore.northing)
@@ -1764,35 +1958,37 @@
         kaart['x'] = xs
         kaart['y'] = ys
         kaart['boring'] = fs
         kaart['maaiveld'] = groundlevels
         kaart['onderkant_NAP'] = depths
         kaart['peilbuis'] = peilbuizen
         kaart['boorbeschrijving'] = boorbeschrijvingen
-        kaart.to_csv(f'./output/{projectName}/{fileName}.csv', sep=';') 
+        if saveFiles: 
+            kaart.to_csv(f'./output/{projectName}/{fileName}.csv', sep=';') 
 
         # maak een geojson voor GIS
         kaart['geometry'] = geometries
-        kaart = gpd.GeoDataFrame(kaart, geometry='geometry').set_crs(epsg=28992)
-        kaart.to_file(f'./output/{projectName}/{fileName}.geojson', driver='GeoJSON') 
+        if saveFiles: 
+            import geopandas as gpd
+            kaart = gpd.GeoDataFrame(kaart, geometry='geometry').set_crs(epsg=28992)
+            kaart.to_file(f'./output/{projectName}/{fileName}.geojson', driver='GeoJSON') 
 
 def code2text(series):
     # functie om codes gebruikt in de XML op te zoeken in de domeintabellen van SIKB
     seriesTranslated = {}
-    for index, value in series.iteritems():
+    for index, value in series.items():
         try:
             # lees de tabel met coderingen in
-            domeintabel = pd.read_excel(f'./sikb_domeintabellen/{index}.xlsx')
+            domeintabel = pd.read_excel(f'./data/raw/sikb_domeintabellen/{index}.xlsx') # TODO: dit moet een relatief pad zijn. Maar welk?
             # maak een dict voor de uitvoering
             translation = {k:v for (k,v) in zip(domeintabel['ID'], domeintabel['Omschrijving'])}
             # zet de codering om in leesbare tekst            
             seriesTranslated[index] = translation[value]
         except:
             seriesTranslated[index] = value
-            pass
 
     seriesTranslated = pd.Series(seriesTranslated)
      
     return seriesTranslated
 
 def Bodemsoort2components(series):
     # functie om de naamgeving gebruikt in SIKB om te zetten in de dictionary met waarden zoals gebruikt voor het plotten van boringen
```

### Comparing `geotexxx-0.0.1/src/geotexxx.egg-info/PKG-INFO` & `geotexxx-0.1.3/src/geotexxx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: geotexxx
-Version: 0.0.1
+Version: 0.1.3
 Summary: Package om geotechnisch grondonderzoek te verwerken
 Author-email: Thomas van der Linden <t.van.der.linden@amsterdam.nl>
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gefxml_reader
 
 Application to read geotechnical CPT and bore data in GEF or BRO XML format
 
 ## Dependecies
 See environment.yml
 
 ## Instruction
 Create an empty object:
+`from geotexxx.gefxml_reader import Cpt, Bore`
 `test = Cpt()` or `test = Bore()`    
 Read in a file:
 `test.load_gef(filename)` or `test.load_xml(filename)`  
 Create a plot in folder ./output
 `test.plot()`  
 
 gui_plot.py provides a point and click interface to make plots of individual files or of all the files in a folder
```

