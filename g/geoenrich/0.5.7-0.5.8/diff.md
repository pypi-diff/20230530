# Comparing `tmp/geoenrich-0.5.7.tar.gz` & `tmp/geoenrich-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoenrich-0.5.7.tar", last modified: Tue Mar 21 05:16:04 2023, max compression
+gzip compressed data, was "geoenrich-0.5.8.tar", last modified: Tue May 30 10:35:01 2023, max compression
```

## Comparing `geoenrich-0.5.7.tar` & `geoenrich-0.5.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 gaetan    (1000) root         (0)        0 2023-03-21 05:16:04.179788 geoenrich-0.5.7/
--rwxrwxrwx   0 gaetan    (1000) root         (0)    35150 2022-04-01 07:24:14.000000 geoenrich-0.5.7/LICENSE
--rwxrwxrwx   0 gaetan    (1000) root         (0)      180 2023-03-21 05:15:47.000000 geoenrich-0.5.7/MANIFEST.in
--rwxrwxrwx   0 gaetan    (1000) root         (0)     4526 2023-03-21 05:16:04.179906 geoenrich-0.5.7/PKG-INFO
--rwxrwxrwx   0 gaetan    (1000) root         (0)     3365 2023-03-21 05:15:47.000000 geoenrich-0.5.7/README.md
-drwxrwxrwx   0 gaetan    (1000) root         (0)        0 2023-03-21 05:16:04.174894 geoenrich-0.5.7/geoenrich/
--rwxrwxrwx   0 gaetan    (1000) root         (0)        0 2022-04-01 07:24:14.000000 geoenrich-0.5.7/geoenrich/__init__.py
--rwxrwxrwx   0 gaetan    (1000) root         (0)      703 2022-07-12 08:05:03.000000 geoenrich-0.5.7/geoenrich/credentials_example.py
-drwxrwxrwx   0 gaetan    (1000) root         (0)        0 2023-03-21 05:16:04.179489 geoenrich-0.5.7/geoenrich/data/
--rwxrwxrwx   0 gaetan    (1000) root         (0)   354142 2022-04-13 11:03:20.000000 geoenrich-0.5.7/geoenrich/data/AcDigitifera.zip
--rwxrwxrwx   0 gaetan    (1000) root         (0)      204 2022-05-20 08:08:28.000000 geoenrich-0.5.7/geoenrich/data/areas.csv
--rwxrwxrwx   0 gaetan    (1000) root         (0)     6652 2022-12-01 11:09:26.000000 geoenrich-0.5.7/geoenrich/data/catalog.csv
--rwxrwxrwx   0 gaetan    (1000) root         (0)    10015 2023-01-10 07:53:06.000000 geoenrich-0.5.7/geoenrich/dataloader.py
--rwxrwxrwx   0 gaetan    (1000) root         (0)    38871 2023-01-10 07:53:06.000000 geoenrich-0.5.7/geoenrich/enrichment.py
--rwxrwxrwx   0 gaetan    (1000) root         (0)    30319 2023-03-09 06:49:52.000000 geoenrich-0.5.7/geoenrich/exports.py
--rwxrwxrwx   0 gaetan    (1000) root         (0)    15880 2023-03-21 05:15:47.000000 geoenrich-0.5.7/geoenrich/satellite.py
-drwxrwxrwx   0 gaetan    (1000) root         (0)        0 2023-03-21 05:16:04.176555 geoenrich-0.5.7/geoenrich.egg-info/
--rwxrwxrwx   0 gaetan    (1000) root         (0)     4526 2023-03-21 05:16:04.000000 geoenrich-0.5.7/geoenrich.egg-info/PKG-INFO
--rwxrwxrwx   0 gaetan    (1000) root         (0)      449 2023-03-21 05:16:04.000000 geoenrich-0.5.7/geoenrich.egg-info/SOURCES.txt
--rwxrwxrwx   0 gaetan    (1000) root         (0)        1 2023-03-21 05:16:04.000000 geoenrich-0.5.7/geoenrich.egg-info/dependency_links.txt
--rwxrwxrwx   0 gaetan    (1000) root         (0)      148 2023-03-21 05:16:04.000000 geoenrich-0.5.7/geoenrich.egg-info/requires.txt
--rwxrwxrwx   0 gaetan    (1000) root         (0)       10 2023-03-21 05:16:04.000000 geoenrich-0.5.7/geoenrich.egg-info/top_level.txt
--rwxrwxrwx   0 gaetan    (1000) root         (0)       85 2022-04-01 07:24:14.000000 geoenrich-0.5.7/pyproject.toml
--rwxrwxrwx   0 gaetan    (1000) root         (0)     1332 2023-03-21 05:16:04.180375 geoenrich-0.5.7/setup.cfg
+drwxrwxrwx   0 gaetan    (1000) root         (0)        0 2023-05-30 10:35:01.964421 geoenrich-0.5.8/
+-rwxrwxrwx   0 gaetan    (1000) root         (0)    35150 2022-04-01 07:24:14.000000 geoenrich-0.5.8/LICENSE
+-rwxrwxrwx   0 gaetan    (1000) root         (0)      180 2023-03-21 05:15:47.000000 geoenrich-0.5.8/MANIFEST.in
+-rwxrwxrwx   0 gaetan    (1000) root         (0)     4526 2023-05-30 10:35:01.964542 geoenrich-0.5.8/PKG-INFO
+-rwxrwxrwx   0 gaetan    (1000) root         (0)     3365 2023-05-10 05:20:42.000000 geoenrich-0.5.8/README.md
+drwxrwxrwx   0 gaetan    (1000) root         (0)        0 2023-05-30 10:35:01.957238 geoenrich-0.5.8/geoenrich/
+-rwxrwxrwx   0 gaetan    (1000) root         (0)        0 2022-04-01 07:24:14.000000 geoenrich-0.5.8/geoenrich/__init__.py
+-rwxrwxrwx   0 gaetan    (1000) root         (0)      703 2022-07-12 08:05:03.000000 geoenrich-0.5.8/geoenrich/credentials_example.py
+drwxrwxrwx   0 gaetan    (1000) root         (0)        0 2023-05-30 10:35:01.963899 geoenrich-0.5.8/geoenrich/data/
+-rwxrwxrwx   0 gaetan    (1000) root         (0)   354142 2022-04-13 11:03:20.000000 geoenrich-0.5.8/geoenrich/data/AcDigitifera.zip
+-rwxrwxrwx   0 gaetan    (1000) root         (0)      204 2022-05-20 08:08:28.000000 geoenrich-0.5.8/geoenrich/data/areas.csv
+-rwxrwxrwx   0 gaetan    (1000) root         (0)     6483 2023-05-16 12:11:06.000000 geoenrich-0.5.8/geoenrich/data/catalog.csv
+-rwxrwxrwx   0 gaetan    (1000) root         (0)     9814 2023-05-10 05:52:25.000000 geoenrich-0.5.8/geoenrich/dataloader.py
+-rwxrwxrwx   0 gaetan    (1000) root         (0)    38811 2023-05-10 06:17:06.000000 geoenrich-0.5.8/geoenrich/enrichment.py
+-rwxrwxrwx   0 gaetan    (1000) root         (0)    30306 2023-04-03 05:46:35.000000 geoenrich-0.5.8/geoenrich/exports.py
+-rwxrwxrwx   0 gaetan    (1000) root         (0)    15880 2023-03-21 05:15:47.000000 geoenrich-0.5.8/geoenrich/satellite.py
+drwxrwxrwx   0 gaetan    (1000) root         (0)        0 2023-05-30 10:35:01.960143 geoenrich-0.5.8/geoenrich.egg-info/
+-rwxrwxrwx   0 gaetan    (1000) root         (0)     4526 2023-05-30 10:35:01.000000 geoenrich-0.5.8/geoenrich.egg-info/PKG-INFO
+-rwxrwxrwx   0 gaetan    (1000) root         (0)      449 2023-05-30 10:35:01.000000 geoenrich-0.5.8/geoenrich.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gaetan    (1000) root         (0)        1 2023-05-30 10:35:01.000000 geoenrich-0.5.8/geoenrich.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gaetan    (1000) root         (0)      155 2023-05-30 10:35:01.000000 geoenrich-0.5.8/geoenrich.egg-info/requires.txt
+-rwxrwxrwx   0 gaetan    (1000) root         (0)       10 2023-05-30 10:35:01.000000 geoenrich-0.5.8/geoenrich.egg-info/top_level.txt
+-rwxrwxrwx   0 gaetan    (1000) root         (0)       85 2022-04-01 07:24:14.000000 geoenrich-0.5.8/pyproject.toml
+-rwxrwxrwx   0 gaetan    (1000) root         (0)     1339 2023-05-30 10:35:01.964991 geoenrich-0.5.8/setup.cfg
```

### Comparing `geoenrich-0.5.7/LICENSE` & `geoenrich-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `geoenrich-0.5.7/PKG-INFO` & `geoenrich-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoenrich
-Version: 0.5.7
+Version: 0.5.8
 Summary: A package to enrich your geo-referenced data (e.g. species occurrences) with environmental data.
 Author: Gaétan Morand (UMR Marbec)
 Author-email: gaetan.morand@ird.fr
 Project-URL: Tutorial, https://geoenrich.readthedocs.io/en/latest/tutorial.html
 Project-URL: Documentation, https://geoenrich.readthedocs.io
 Project-URL: Code, https://github.com/morand-g/geoenrich
 Project-URL: Bug Tracker, https://github.com/morand-g/geoenrich/issues
@@ -14,19 +14,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# **geoenrich 0.5.7**
+# **geoenrich 0.5.8**
 
 [![Read the Docs](https://img.shields.io/readthedocs/geoenrich)](https://geoenrich.readthedocs.io/en/latest/)
 [![License](https://img.shields.io/github/license/morand-g/geoenrich?color=green)](https://github.com/morand-g/geoenrich/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/geoenrich?color=green)](https://pypi.org/project/geoenrich/)
 [![Python versions](https://img.shields.io/pypi/pyversions/geoenrich)](https://www.python.org/downloads/)
 [![Last commit](https://img.shields.io/github/last-commit/morand-g/geoenrich)](https://github.com/morand-g/geoenrich/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6458090.svg)](https://doi.org/10.5281/zenodo.6458090)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: geoenrich Version: 0.5.7 Summary: A package to
+Metadata-Version: 2.1 Name: geoenrich Version: 0.5.8 Summary: A package to
 enrich your geo-referenced data (e.g. species occurrences) with environmental
 data. Author: GaÃ©tan Morand (UMR Marbec) Author-email: gaetan.morand@ird.fr
 Project-URL: Tutorial, https://geoenrich.readthedocs.io/en/latest/tutorial.html
 Project-URL: Documentation, https://geoenrich.readthedocs.io Project-URL: Code,
 https://github.com/morand-g/geoenrich Project-URL: Bug Tracker, https://
 github.com/morand-g/geoenrich/issues Classifier: Programming Language :: Python
 :: 3 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Classifier: Natural Language :: English Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
 Bio-Informatics Classifier: Topic :: Scientific/Engineering :: Atmospheric
 Science Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE # **geoenrich 0.5.7** [![Read the Docs](https://img.shields.io/
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE # **geoenrich 0.5.8** [![Read the Docs](https://img.shields.io/
 readthedocs/geoenrich)](https://geoenrich.readthedocs.io/en/latest/) [!
 [License](https://img.shields.io/github/license/morand-g/
 geoenrich?color=green)](https://github.com/morand-g/geoenrich/blob/main/
 LICENSE) [![PyPI](https://img.shields.io/pypi/v/geoenrich?color=green)](https:/
 /pypi.org/project/geoenrich/) [![Python versions](https://img.shields.io/pypi/
 pyversions/geoenrich)](https://www.python.org/downloads/) [![Last commit]
 (https://img.shields.io/github/last-commit/morand-g/geoenrich)](https://
```

### Comparing `geoenrich-0.5.7/README.md` & `geoenrich-0.5.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# **geoenrich 0.5.7**
+# **geoenrich 0.5.8**
 
 [![Read the Docs](https://img.shields.io/readthedocs/geoenrich)](https://geoenrich.readthedocs.io/en/latest/)
 [![License](https://img.shields.io/github/license/morand-g/geoenrich?color=green)](https://github.com/morand-g/geoenrich/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/geoenrich?color=green)](https://pypi.org/project/geoenrich/)
 [![Python versions](https://img.shields.io/pypi/pyversions/geoenrich)](https://www.python.org/downloads/)
 [![Last commit](https://img.shields.io/github/last-commit/morand-g/geoenrich)](https://github.com/morand-g/geoenrich/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6458090.svg)](https://doi.org/10.5281/zenodo.6458090)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# **geoenrich 0.5.7** [![Read the Docs](https://img.shields.io/readthedocs/
+# **geoenrich 0.5.8** [![Read the Docs](https://img.shields.io/readthedocs/
 geoenrich)](https://geoenrich.readthedocs.io/en/latest/) [![License](https://
 img.shields.io/github/license/morand-g/geoenrich?color=green)](https://
 github.com/morand-g/geoenrich/blob/main/LICENSE) [![PyPI](https://
 img.shields.io/pypi/v/geoenrich?color=green)](https://pypi.org/project/
 geoenrich/) [![Python versions](https://img.shields.io/pypi/pyversions/
 geoenrich)](https://www.python.org/downloads/) [![Last commit](https://
 img.shields.io/github/last-commit/morand-g/geoenrich)](https://github.com/
```

### Comparing `geoenrich-0.5.7/geoenrich/credentials_example.py` & `geoenrich-0.5.8/geoenrich/credentials_example.py`

 * *Files identical despite different names*

### Comparing `geoenrich-0.5.7/geoenrich/data/AcDigitifera.zip` & `geoenrich-0.5.8/geoenrich/data/AcDigitifera.zip`

 * *Files identical despite different names*

### Comparing `geoenrich-0.5.7/geoenrich/data/catalog.csv` & `geoenrich-0.5.8/geoenrich/data/catalog.csv`

 * *Files 9% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 mixed-layer-thickness,Copernicus,0.25°,7d,1993-01-01 - ongoing,surface,https://nrt.cmems-du.eu/thredds/dodsC/dataset-armor-3d-rep-weekly,mlotst
 nanophytoplankton,Copernicus,4km,1m,1997-09-04 - ongoing,surface,https://my.cmems-du.eu/thredds/dodsC/cmems_obs-oc_glo_bgc-plankton_my_l4-multi-4km_P1M,NANO
 ocean-heat-content,NOAA,1°,3m,1955-01-01 - ongoing,surface,https://www.ncei.noaa.gov/thredds-ocean/dodsC/woa/heat_content/heat_content/heat_content_anomaly_0-700_seasonal.nc,h18_hc
 organic-carbon3d,Copernicus,0.25°,7d,1998-01-01 - ongoing,36 levels,https://my.cmems-du.eu/thredds/dodsC/cmems_obs_glo_bgc3d_rep_weekly,poc
 oxygen,Copernicus,0.25°,1d,1993-01-01 - 2020-12-31,75 levels,https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_bgc_my_0.25_P1D-m,o2
 oxygen2,Copernicus,0.25°,1d,2019-05-04 - ongoing,50 levels,https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-bio-001-028-daily,o2
 ph,Copernicus,0.25°,1m,1993-01-01 - 2020-12-31,75 levels,https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_bgc_my_0.25_P1M-m,ph
+ph2,Copernicus,0.25°,1d,2019-05-04 - ongoing,50 levels,https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-bio-001-028-daily,ph
 picophytoplankton,Copernicus,4km,1m,1997-09-04 - ongoing,surface,https://my.cmems-du.eu/thredds/dodsC/cmems_obs-oc_glo_bgc-plankton_my_l4-multi-4km_P1M,PICO
 primary-production,Copernicus,4km,1m,1997-09-04 - ongoing,surface,https://my.cmems-du.eu/thredds/dodsC/cmems_obs-oc_glo_bgc-pp_my_l4-multi-4km_P1M,PP
 prochlorophytes,Copernicus,4km,1m,1997-09-04 - ongoing,surface,https://my.cmems-du.eu/thredds/dodsC/cmems_obs-oc_glo_bgc-plankton_my_l4-multi-4km_P1M,PROCHLO
 prokaryotes,Copernicus,4km,1m,1997-09-04 - ongoing,surface,https://my.cmems-du.eu/thredds/dodsC/cmems_obs-oc_glo_bgc-plankton_my_l4-multi-4km_P1M,PROKAR
 salinity,SMOS+Aquarius,0.25°,7d,2011-09-01 - 2021-09-08,surface,[FillMismatch]https://thredds.jpl.nasa.gov/thredds/dodsC/SalinityDensity/OISSS_L4_multimission_7day_v1.nc,sss
 salinity3d,Copernicus,0.25°,7d,1993-01-01 - ongoing,50 levels,https://nrt.cmems-du.eu/thredds/dodsC/dataset-armor-3d-rep-weekly,so
 sla,Copernicus,0.25°,1d,1993-01-01 - 2019-12-31,surface,https://my.cmems-du.eu/thredds/dodsC/cmems_obs-sl_glo_phy-ssh_my_allsat-l4-duacs-0.25deg_P1D,sla
 sla2,Copernicus,0.25°,1d,2019-12-01 - ongoing,surface,https://nrt.cmems-du.eu/thredds/dodsC/dataset-duacs-nrt-global-merged-allsat-phy-l4,sla
 sst,Copernicus,0.05°,1d,1981-10-01 - ongoing,surface,https://my.cmems-du.eu/thredds/dodsC/METOFFICE-GLO-SST-L4-REP-OBS-SST,analysed_sst
-sst-mur,MUR-SST,0.01°,1d,2002-06-02 - ongoing,surface,https://thredds.jpl.nasa.gov/thredds/dodsC/OceanTemperature/MUR-JPL-L4-GLOB-v4.1.nc,analysed_sst
-sst-mur25,MUR-SST,0.25°,1d,2002-06-02 - ongoing,surface,https://thredds.jpl.nasa.gov/thredds/dodsC/OceanTemperature/MUR25-JPL-L4-GLOB-v04.2.nc,analysed_sst
 surface-current-u,Copernicus,0.25°,3h,1993-10-01 - ongoing,"surface, 15m",https://my.cmems-du.eu/thredds/dodsC/dataset-uv-rep-hourly,uo
 surface-current-v,Copernicus,0.25°,3h,1993-10-01 - ongoing,"surface, 15m",https://my.cmems-du.eu/thredds/dodsC/dataset-uv-rep-hourly,vo
 surface-wind-u,CCMP,0.25°,6h,1987-07-02 - 2011-12-31,surface,http://apdrc.soest.hawaii.edu:80/dods/public_data/satellite_product/CCMP/6hourly_v2,uwnd
 surface-wind-v,CCMP,0.25°,6h,1987-07-02 - 2011-12-31,surface,http://apdrc.soest.hawaii.edu:80/dods/public_data/satellite_product/CCMP/6hourly_v2,vwnd
 temperature3d,Copernicus,0.25°,7d,1993-01-01 - ongoing,50 levels,https://nrt.cmems-du.eu/thredds/dodsC/dataset-armor-3d-rep-weekly,to
 wave-height,Copernicus,2°,1d,2002-01-01 - ongoing,surface,https://my.cmems-du.eu/thredds/dodsC/cmems_obs-wave_glo_phy-swh_my_multi-l4-2deg_P1D,VAVH_INST
 wind-u,Copernicus,0.125°,1h,2020-07-01 – ongoing,surface,https://nrt.cmems-du.eu/thredds/dodsC/cmems_obs-wind_glo_phy_nrt_l4_0.125deg_PT1H,eastward_wind
```

### Comparing `geoenrich-0.5.7/geoenrich/dataloader.py` & `geoenrich-0.5.8/geoenrich/dataloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     idf = rawdf[rawdf['basisOfRecord'].isin(['HUMAN_OBSERVATION', 'MACHINE_OBSERVATION', 'OCCURRENCE'])]
 
     # Convert Lat/Long to GEOS POINT
     idf['geometry'] = gpd.points_from_xy(idf['decimalLongitude'], idf['decimalLatitude'], idf['depth'],crs="EPSG:4326")
 
     # Remove rows with no event date
     idf['eventDate'] = pd.to_datetime(idf['eventDate'], errors = 'coerce')
-    df = idf[idf['eventDate'].notna()]
+    df = idf.dropna(subset = ['eventDate'])
 
     if len(df) > max_number:
         df = df.sample(max_number)
         print('Selected {} random occurrences from the dataset'.format(max_number))
 
     # Convert to GeoDataFrame & standardize Date
     geodf = gpd.GeoDataFrame(df[['id', 'geometry', 'eventDate']])
@@ -227,16 +227,15 @@
     if len(rawdf) != len(idf):
         print('Dropped {} rows with missing coordinates'.format(len(rawdf) - len(idf)))
     
     # Convert Lat/Long to GEOS POINT
     idf['geometry'] = gpd.points_from_xy(idf[lon_col], idf[lat_col], crs=crs)
 
     # Remove rows with no event date
-    idf['eventDate'] = pd.to_datetime(idf[date_col], errors = 'coerce', format = date_format,
-                                    infer_datetime_format = True)
+    idf['eventDate'] = pd.to_datetime(idf[date_col], errors = 'coerce', format = date_format)
     df = idf.dropna(subset = ['eventDate'])
 
     if len(idf) != len(df):
         print('Dropped {} rows with missing or badly formated dates'.format(len(idf) - len(df)))
 
     # Convert to GeoDataFrame
     geodf = gpd.GeoDataFrame(df[['geometry', 'eventDate']])
@@ -267,18 +266,16 @@
 
     rawdf = pd.read_csv(path, index_col = 'id', parse_dates = ['date_min', 'date_max'],
                 infer_datetime_format = True, *args, **kwargs)
     rawdf.index.rename('id', inplace=True)
     idf = pd.DataFrame()
 
     if 'date_min' in rawdf.columns:
-        idf['mint'] = pd.to_datetime(rawdf['date_min'], errors = 'coerce', format = date_format,
-                                        infer_datetime_format = True)
-        idf['maxt'] = pd.to_datetime(rawdf['date_max'], errors = 'coerce', format = date_format,
-                                        infer_datetime_format = True)
+        idf['mint'] = pd.to_datetime(rawdf['date_min'], errors = 'coerce', format = date_format)
+        idf['maxt'] = pd.to_datetime(rawdf['date_max'], errors = 'coerce', format = date_format)
 
     idf['minx'], idf['maxx'] = rawdf['longitude_min'], rawdf['longitude_max']
     idf['miny'], idf['maxy'] = rawdf['latitude_min'], rawdf['latitude_max']
 
     df = idf.dropna()
     if len(idf) != len(df):
         print('Dropped {} rows with missing or badly formated coordinates'.format(len(idf) - len(df)))
```

### Comparing `geoenrich-0.5.7/geoenrich/enrichment.py` & `geoenrich-0.5.8/geoenrich/enrichment.py`

 * *Files 1% similar despite different names*

```diff
@@ -760,20 +760,20 @@
         enrichment_metadata = json.load(f)
     input_type = enrichment_metadata['input_type']
 
     filepath = Path(biodiv_path, dataset_ref + '.csv')
 
 
     if input_type == 'occurrence':
-        df = pd.read_csv(str(filepath), parse_dates = ['eventDate'], infer_datetime_format = True, index_col = 'id')
+        df = pd.read_csv(str(filepath), parse_dates = ['eventDate'], index_col = 'id')
         df['geometry'] = df['geometry'].apply(wkt.loads)
         df = gpd.GeoDataFrame(df, crs = 'epsg:4326')
 
     else:
-        df = pd.read_csv(str(filepath), parse_dates = ['mint', 'maxt'], infer_datetime_format = True, index_col = 'id')
+        df = pd.read_csv(str(filepath), parse_dates = ['mint', 'maxt'], index_col = 'id')
 
     if not(mute):
         print('{} {}s were loaded from enrichment file'.format(len(df), input_type))
     
     return(df, enrichment_metadata)
```

### Comparing `geoenrich-0.5.7/geoenrich/exports.py` & `geoenrich-0.5.8/geoenrich/exports.py`

 * *Files 2% similar despite different names*

```diff
@@ -661,25 +661,25 @@
             print(f'Raster saved at {im_path}')
 
         else:
 
             print('Abort. Array is smaller than 2x2 pixels.')
 
 
-def collate_npy(ds_ref, data_path, output_res = 32, sample = None, dimension3 = {'surface-current-u': 2}):
+def collate_npy(ds_ref, data_path, output_res = 32, slice = None, dimension3 = {'surface-current-u': 2}):
 
     """
     Export a 3D numpy array with all layers for each occurrence of a dataset.
     WARNING: the dimension3 dictionary must be provided if some variables have a time or depth dimension.
 
     Args:
         ds_ref (str): The enrichment file name (e.g. gbif_taxonKey).
         data_path (str): path where numpy files will be saved.
         output_res (int) : output data resolution along lat and lon axes.
-        sample (int): if not None, only process a random sample of the dataset (N=*sample*)
+        slice (list[int]): if not None, only process the given slice of the dataset.
         dimension3: provides the expected 3rd dimension length (time dimension * depth dimension) for each variable where it is larger than 1.
 
     Returns:
         None
     """
 
     folderpath = data_path / (ds_ref + '-npy')
@@ -705,18 +705,18 @@
         serial_dict[en['id']]['var_source'] = var_source
         serial_dict[en['id']]['dimdict'], serial_dict[en['id']]['var'] = get_metadata(ds, var_source['varname'])
         serial_dict[en['id']]['ds'] = ds
 
 
     # Define ids to be exported
 
-    if sample is None:
+    if slice is None:
         ids = df.index
     else:
-        ids = random.sample(list(df.index), sample)
+        ids = list(df.index)[slice[0]:slice[1]]
 
 
     # Export np arrays for each occurrence
 
     for occ_id in tqdm(ids):
         all_bands = []
         for en in enrichments:
```

### Comparing `geoenrich-0.5.7/geoenrich/satellite.py` & `geoenrich-0.5.8/geoenrich/satellite.py`

 * *Files identical despite different names*

### Comparing `geoenrich-0.5.7/geoenrich.egg-info/PKG-INFO` & `geoenrich-0.5.8/geoenrich.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoenrich
-Version: 0.5.7
+Version: 0.5.8
 Summary: A package to enrich your geo-referenced data (e.g. species occurrences) with environmental data.
 Author: Gaétan Morand (UMR Marbec)
 Author-email: gaetan.morand@ird.fr
 Project-URL: Tutorial, https://geoenrich.readthedocs.io/en/latest/tutorial.html
 Project-URL: Documentation, https://geoenrich.readthedocs.io
 Project-URL: Code, https://github.com/morand-g/geoenrich
 Project-URL: Bug Tracker, https://github.com/morand-g/geoenrich/issues
@@ -14,19 +14,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# **geoenrich 0.5.7**
+# **geoenrich 0.5.8**
 
 [![Read the Docs](https://img.shields.io/readthedocs/geoenrich)](https://geoenrich.readthedocs.io/en/latest/)
 [![License](https://img.shields.io/github/license/morand-g/geoenrich?color=green)](https://github.com/morand-g/geoenrich/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/geoenrich?color=green)](https://pypi.org/project/geoenrich/)
 [![Python versions](https://img.shields.io/pypi/pyversions/geoenrich)](https://www.python.org/downloads/)
 [![Last commit](https://img.shields.io/github/last-commit/morand-g/geoenrich)](https://github.com/morand-g/geoenrich/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6458090.svg)](https://doi.org/10.5281/zenodo.6458090)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: geoenrich Version: 0.5.7 Summary: A package to
+Metadata-Version: 2.1 Name: geoenrich Version: 0.5.8 Summary: A package to
 enrich your geo-referenced data (e.g. species occurrences) with environmental
 data. Author: GaÃ©tan Morand (UMR Marbec) Author-email: gaetan.morand@ird.fr
 Project-URL: Tutorial, https://geoenrich.readthedocs.io/en/latest/tutorial.html
 Project-URL: Documentation, https://geoenrich.readthedocs.io Project-URL: Code,
 https://github.com/morand-g/geoenrich Project-URL: Bug Tracker, https://
 github.com/morand-g/geoenrich/issues Classifier: Programming Language :: Python
 :: 3 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Classifier: Natural Language :: English Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
 Bio-Informatics Classifier: Topic :: Scientific/Engineering :: Atmospheric
 Science Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE # **geoenrich 0.5.7** [![Read the Docs](https://img.shields.io/
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE # **geoenrich 0.5.8** [![Read the Docs](https://img.shields.io/
 readthedocs/geoenrich)](https://geoenrich.readthedocs.io/en/latest/) [!
 [License](https://img.shields.io/github/license/morand-g/
 geoenrich?color=green)](https://github.com/morand-g/geoenrich/blob/main/
 LICENSE) [![PyPI](https://img.shields.io/pypi/v/geoenrich?color=green)](https:/
 /pypi.org/project/geoenrich/) [![Python versions](https://img.shields.io/pypi/
 pyversions/geoenrich)](https://www.python.org/downloads/) [![Last commit]
 (https://img.shields.io/github/last-commit/morand-g/geoenrich)](https://
```

### Comparing `geoenrich-0.5.7/setup.cfg` & `geoenrich-0.5.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geoenrich
-version = 0.5.7
+version = 0.5.8
 author = Gaétan Morand (UMR Marbec)
 author_email = gaetan.morand@ird.fr
 description = A package to enrich your geo-referenced data (e.g. species occurrences) with environmental data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Tutorial = https://geoenrich.readthedocs.io/en/latest/tutorial.html
@@ -22,26 +22,26 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Atmospheric Science
 	Topic :: Scientific/Engineering :: Information Analysis
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	numpy
-	pandas
+	pandas>=2.0.0
 	geopandas
 	netCDF4==1.5.8
 	python-dwca-reader
 	tqdm
 	opencv-python
 	pathlib
 	rasterio
-	pygbif==0.6.1
+	pygbif>=0.6.1
 	matplotlib
 	appdirs
 	geojson_rewind
 	geomet
 
 [egg_info]
 tag_build =
```

