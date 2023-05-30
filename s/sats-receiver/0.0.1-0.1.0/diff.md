# Comparing `tmp/sats_receiver-0.0.1.tar.gz` & `tmp/sats_receiver-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sats_receiver-0.0.1.tar", last modified: Tue May 30 17:12:58 2023, max compression
+gzip compressed data, was "sats_receiver-0.1.0.tar", last modified: Tue Jan 17 16:15:05 2023, max compression
```

## Comparing `sats_receiver-0.0.1.tar` & `sats_receiver-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:58.689360 sats_receiver-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-05-30 17:12:58.689360 sats_receiver-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:58.685360 sats_receiver-0.0.1/sats_receiver/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/async_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:58.689360 sats_receiver-0.0.1/sats_receiver/gr_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/gr_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/gr_modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/gr_modules/demodulators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:58.689360 sats_receiver-0.0.1/sats_receiver/gr_modules/epb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/gr_modules/epb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/gr_modules/epb/sstv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/gr_modules/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/gr_modules/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/librtlsdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/observer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:58.689360 sats_receiver-0.0.1/sats_receiver/systems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/systems/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/systems/sstv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/tle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/sats_receiver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:58.685360 sats_receiver-0.0.1/sats_receiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-05-30 17:12:58.000000 sats_receiver-0.0.1/sats_receiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-30 17:12:58.000000 sats_receiver-0.0.1/sats_receiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:12:58.000000 sats_receiver-0.0.1/sats_receiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 17:12:58.000000 sats_receiver-0.0.1/sats_receiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 17:12:58.000000 sats_receiver-0.0.1/sats_receiver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 17:12:58.689360 sats_receiver-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:58.689360 sats_receiver-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/tests/test_async_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/tests/test_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-30 17:12:46.000000 sats_receiver-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:15:05.329370 sats_receiver-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-01-17 16:15:05.329370 sats_receiver-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:15:05.325370 sats_receiver-0.1.0/sats_receiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1675 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/async_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:15:05.325370 sats_receiver-0.1.0/sats_receiver/gr_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/gr_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/gr_modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/gr_modules/demodulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/gr_modules/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/gr_modules/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/librtlsdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/observer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:15:05.329370 sats_receiver-0.1.0/sats_receiver/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/systems/apt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/tle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/sats_receiver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:15:05.325370 sats_receiver-0.1.0/sats_receiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-01-17 16:15:05.000000 sats_receiver-0.1.0/sats_receiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-01-17 16:15:05.000000 sats_receiver-0.1.0/sats_receiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 16:15:05.000000 sats_receiver-0.1.0/sats_receiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-17 16:15:05.000000 sats_receiver-0.1.0/sats_receiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-17 16:15:05.000000 sats_receiver-0.1.0/sats_receiver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 16:15:05.329370 sats_receiver-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-01-17 16:14:53.000000 sats_receiver-0.1.0/setup.py
```

### Comparing `sats_receiver-0.0.1/LICENSE` & `sats_receiver-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.0.1/PKG-INFO` & `sats_receiver-0.1.0/sats_receiver.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sats_receiver
-Version: 0.0.1
+Name: sats-receiver
+Version: 0.1.0
 Summary: Satellites data receiver based on GNU Radio
 Home-page: https://github.com/baskiton/sats-receiver
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baskiton/sats-receiver/issues
 Classifier: License :: OSI Approved :: MIT License
@@ -12,112 +12,86 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sats Receiver
-[![PyPI](https://img.shields.io/pypi/v/sats-receiver?logo=python&logoColor=white)][pypi_proj]
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/sats-receiver?logo=python&logoColor=white)][pypi_proj]
-[![PyPI - License](https://img.shields.io/pypi/l/sats-receiver?logo=open-source-initiative&logoColor=white)][license]  
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/tests.yml?label=tests&logo=github)][tests]
-[![Codecov branch](https://img.shields.io/codecov/c/gh/baskiton/sats-receiver/dev?logo=codecov)][codecov]
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/pypi-upload.yml?label=upload&logo=github)][upload]
-
-[pypi_proj]: https://pypi.org/project/sats-receiver/
-[license]: https://github.com/baskiton/sats-receiver/blob/main/LICENSE
-[tests]: https://github.com/baskiton/sats-receiver/actions/workflows/tests.yml
-[codecov]: https://app.codecov.io/gh/baskiton/sats-receiver
-[upload]: https://github.com/baskiton/sats-receiver/actions/workflows/pypi-upload.yml
+[![PyPI](https://img.shields.io/pypi/v/sats_receiver?logo=python&logoColor=white)][pypi_proj]
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/sats_receiver?logo=python&logoColor=white)][pypi_proj]
+[![PyPI - License](https://img.shields.io/pypi/l/sats_receiver?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/sats-receiver/blob/main/LICENSE)
+[![upload](https://img.shields.io/github/actions/workflow/status/baskiton/sats_receiver/pypi-upload.yml?label=upload&logo=github)](https://github.com/baskiton/sats-receiver/actions/workflows/pypi-upload.yml)
+
+[pypi_proj]: https://pypi.org/project/sats_receiver/
 
 Satellites data receiver based on GNURadio
 
 <!-- TOC -->
 * [About](#About)
 * [Requirements](#Requirements)
 * [Installation](#Installation)
-  * [Linux](#Linux)
-  * [Windows](#Windows)
 * [Usage](#Usage)
 * [Configure](#Configure)
   * [observer](#observer)
   * [tle](#tle)
   * [receivers](#receivers)
     * [sats](#sats)
       * [frequencies](#frequencies)
         * [modulations](#modulations)
         * [decoders](#decoders)
 * [Map Shapes](#Map-Shapes)
   * [shapes](#shapes)
   * [points](#points)
 <!-- TOC -->
 
-
-
 ### About
 This program is written to automate the process of receiving signals from
 various orbiting satellites on your SDR. The basis for digital signal
 processing is GNU Radio - a free software development toolkit that provides
 signal processing blocks to implement software-defined radios and
 signal-processing systems. [[wikipedia](https://en.wikipedia.org/wiki/GNU_Radio)]  
 For example, this program is perfect for receiving weather
 satellites like NOAA (image below).  
 If you have ideas or knowledge on how to improve this project, feel free to submit issues or pull requests.
 
-![](doc/NOAA-15_2023-05-11_03-30-41,734229_map.jpg "NOAA-15")
+![](doc/NOAA-19_2023-01-12_04-24-35,752471_map.jpg "NOAA-19")
 
 
 ### Requirements
 The program has only been tested on Linux. Work on Windows is not guaranteed!
 * Python>=3.10 (or lower, see below)
 * GNURadio>=3.10 (or lower if gr-soapy installed); GUI-modules is not required
 * librtlsdr (if you use RTL-SDR)
 
 ### Installation
-First [install gnuradio](https://wiki.gnuradio.org/index.php?title=InstallingGR)
-
-#### Linux
-  If you need a virtual environment (recommended), you need to create it
-  with the `--system-site-packages` option
-  ```
-  python3 -m venv --system-site-packages venv
-  source venv/bin/activate
-  pip install sats-receiver
-  ```
-
-#### Windows
-  After install `radioconda`, launch a terminal by running "Conda Prompt"
-  in the "radioconda" directory in the Start menu and type
-  ```
-  pip install sats-receiver
-  ```
+* if you need a virtual environment, you need to create it with the `--system-site-packages` option:  
+  `python3 -m venv --system-site-packages venv`  
+  `source venv/bin/activate`  
+* from source  
+  `git clone https://github.com/baskiton/sats-receiver.git`  
+  `cd sats-receiver`  
+  `pip install -r requirements.txt`  
+* from pip  
+  `pip install sats_receiver`  
 
 ### Usage
-* in Linux if a virtual environment has been created:  
-  `source venv/bin/activate`
-* in Windows launch "Conda Prompt" terminal
-
-`python -u -m sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
+`python3 -m sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
+`sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
 * `config` Config file path. See [Configure](#Configure)
 * `-h, --help` Help message
 * `--log LOG` Logging level, INFO default
-* `--sysu SYSU` System Usages debug info timeout in seconds, 1 hour default
+* `--sysu SYSU` System Usages info timeout in seconds, 1 hour default
 
-For example, simple command line to launch program:  
-`python -u -m sats_receiver /path/to/config.json`  
-You can copy the `default.json` config file from the root of the repository to a
-location of your choice
-
-Program home directory is `~/sats_receiver`  
-Logfile saved to program home directory (`~/sats_receiver/logs`)  
-Tle files stored to program home directory (`~/sats_receiver/tle`)  
+Program home directory is `~/sats_receiver`
+Logfile saved to program home directory (~/sats_receiver/logs)
+Tle files stored to program home directory (~/sats_receiver/tle)
 
 ### Configure
 The configuration file is in JSON format.  
-You can copy the `default.json` file from the root of the repository to a
+You can copy the default.json file from the root of the repository to a
 location of your choice and edit it.
 
 | Field     | Type            | Description                                                |
 |:----------|:----------------|:-----------------------------------------------------------|
 | observer  | Object          | Observer/receiver parameters (see [observer](#observer))   |
 | tle       | Object          | TLE data parameters (see [tle](#tle))                      |
 | receivers | Array of Object | List of receivers parameters (see [receivers](#receivers)) |
@@ -181,59 +155,42 @@
 | freq_correction | Boolean | _Optional._ Correction for basic frequency, Hz. `0` by default                    |
 | mode            | String  | _Optional._ Modulation option (see [modulations](#modulations)). `RAW` by default |
 | decode          | String  | _Optional._ Decoder option (see [decoders](#decoders)). `RAW` by default          |
 | qpsk_baudrate   | Number  | _Required only for **QPSK** mode._ QPSK Baudrate, bps                             |
 | qpsk_excess_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Excess bandwidth. `0.35` by default      |
 | qpsk_ntaps      | Integer | _Optional. Only for **QPSK** mode._ QPSK number of taps. `33` by default          |
 | qpsk_costas_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Costas bandwidth. `0.005` by default     |
-| sstv_wsr        | Number  | _Optional. Only for **SSTV** decoder._ SSTV work samplerate. `16000` by default   |
-| sstv_sync       | Number  | _Optional. Only for **SSTV** decoder._ SSTV syncing. `true` by default            |
 
 
 #### modulations
 * `RAW`
 * `AM`
 * `FM`
 * `WFM`
 * `WFM_STEREO`
 * `QUAD`
 * `QPSK`
 
 #### decoders
 * `RAW` Saved to 2-channel float32 WAV file with `bandwidth` sample rate
 * `RSTREAM` Raw Stream - binary int8. Suitable for further processing, for example, in SatDump
-* `APT` sats-receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
-* `SSTV` SSTV saved to PNG image with EXIF. Supported modes:
-  * `Robot24`
-  * `Robot36`
-  * `Robot72`
-  * `MartinM1`
-  * `MartinM2`
-  * `MartinM3`
-  * `MartinM4`
-  * `PD50`
-  * `PD90`
-  * `PD120`
-  * `PD160`
-  * `PD180`
-  * `PD240`
-  * `PD290`
+* `APT` sats_receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
 * ~~`LRPT`~~ Not implemented yet
 
 
 ### Map Shapes
 Map shapes config file `map_shapes.json` can be found at the root of this repository.
 Shapefiles can be downloaded from [Natural Earth](https://www.naturalearthdata.com/downloads/)
 
-| Field      | Type             | Description                                                                        |
-|:-----------|:-----------------|:-----------------------------------------------------------------------------------|
-| shapes     | Array of Array   | _Optional._ List of shapes data (see [shapes](#shapes))                            |
-| shapes_dir | String           | _Optional. Only when `shapes` specified._ Path to directory contains shapes file   |
-| points     | Object of Object | _Optional._ Additional points to draw on map (see [points](#points))               |
-| line_width | Number           | _Optional._ Overlay lines width, pixels. `1` by default                            |
+| Field      | Type             | Description                                                          |
+|:-----------|:-----------------|:---------------------------------------------------------------------|
+| shapes_dir | String           | Path to directory contains shapes file                               |
+| shapes     | Array of Array   | List of shapes data (see [shapes](#shapes))                          |
+| line_width | Number           | _Optional._ Overlay lines width, pixels. `1` by default              |
+| points     | Object of Object | _Optional._ Additional points to draw on map (see [points](#points)) |
 
 
 #### shapes
 Each shape contain:
 
 | Offset | Field     | Type                       | Description                                                                                                        |
 |:-------|:----------|:---------------------------|:-------------------------------------------------------------------------------------------------------------------|
```

### Comparing `sats_receiver-0.0.1/README.md` & `sats_receiver-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,106 +1,80 @@
 # Sats Receiver
-[![PyPI](https://img.shields.io/pypi/v/sats-receiver?logo=python&logoColor=white)][pypi_proj]
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/sats-receiver?logo=python&logoColor=white)][pypi_proj]
-[![PyPI - License](https://img.shields.io/pypi/l/sats-receiver?logo=open-source-initiative&logoColor=white)][license]  
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/tests.yml?label=tests&logo=github)][tests]
-[![Codecov branch](https://img.shields.io/codecov/c/gh/baskiton/sats-receiver/dev?logo=codecov)][codecov]
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/pypi-upload.yml?label=upload&logo=github)][upload]
-
-[pypi_proj]: https://pypi.org/project/sats-receiver/
-[license]: https://github.com/baskiton/sats-receiver/blob/main/LICENSE
-[tests]: https://github.com/baskiton/sats-receiver/actions/workflows/tests.yml
-[codecov]: https://app.codecov.io/gh/baskiton/sats-receiver
-[upload]: https://github.com/baskiton/sats-receiver/actions/workflows/pypi-upload.yml
+[![PyPI](https://img.shields.io/pypi/v/sats_receiver?logo=python&logoColor=white)][pypi_proj]
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/sats_receiver?logo=python&logoColor=white)][pypi_proj]
+[![PyPI - License](https://img.shields.io/pypi/l/sats_receiver?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/sats-receiver/blob/main/LICENSE)
+[![upload](https://img.shields.io/github/actions/workflow/status/baskiton/sats_receiver/pypi-upload.yml?label=upload&logo=github)](https://github.com/baskiton/sats-receiver/actions/workflows/pypi-upload.yml)
+
+[pypi_proj]: https://pypi.org/project/sats_receiver/
 
 Satellites data receiver based on GNURadio
 
 <!-- TOC -->
 * [About](#About)
 * [Requirements](#Requirements)
 * [Installation](#Installation)
-  * [Linux](#Linux)
-  * [Windows](#Windows)
 * [Usage](#Usage)
 * [Configure](#Configure)
   * [observer](#observer)
   * [tle](#tle)
   * [receivers](#receivers)
     * [sats](#sats)
       * [frequencies](#frequencies)
         * [modulations](#modulations)
         * [decoders](#decoders)
 * [Map Shapes](#Map-Shapes)
   * [shapes](#shapes)
   * [points](#points)
 <!-- TOC -->
 
-
-
 ### About
 This program is written to automate the process of receiving signals from
 various orbiting satellites on your SDR. The basis for digital signal
 processing is GNU Radio - a free software development toolkit that provides
 signal processing blocks to implement software-defined radios and
 signal-processing systems. [[wikipedia](https://en.wikipedia.org/wiki/GNU_Radio)]  
 For example, this program is perfect for receiving weather
 satellites like NOAA (image below).  
 If you have ideas or knowledge on how to improve this project, feel free to submit issues or pull requests.
 
-![](doc/NOAA-15_2023-05-11_03-30-41,734229_map.jpg "NOAA-15")
+![](doc/NOAA-19_2023-01-12_04-24-35,752471_map.jpg "NOAA-19")
 
 
 ### Requirements
 The program has only been tested on Linux. Work on Windows is not guaranteed!
 * Python>=3.10 (or lower, see below)
 * GNURadio>=3.10 (or lower if gr-soapy installed); GUI-modules is not required
 * librtlsdr (if you use RTL-SDR)
 
 ### Installation
-First [install gnuradio](https://wiki.gnuradio.org/index.php?title=InstallingGR)
-
-#### Linux
-  If you need a virtual environment (recommended), you need to create it
-  with the `--system-site-packages` option
-  ```
-  python3 -m venv --system-site-packages venv
-  source venv/bin/activate
-  pip install sats-receiver
-  ```
-
-#### Windows
-  After install `radioconda`, launch a terminal by running "Conda Prompt"
-  in the "radioconda" directory in the Start menu and type
-  ```
-  pip install sats-receiver
-  ```
+* if you need a virtual environment, you need to create it with the `--system-site-packages` option:  
+  `python3 -m venv --system-site-packages venv`  
+  `source venv/bin/activate`  
+* from source  
+  `git clone https://github.com/baskiton/sats-receiver.git`  
+  `cd sats-receiver`  
+  `pip install -r requirements.txt`  
+* from pip  
+  `pip install sats_receiver`  
 
 ### Usage
-* in Linux if a virtual environment has been created:  
-  `source venv/bin/activate`
-* in Windows launch "Conda Prompt" terminal
-
-`python -u -m sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
+`python3 -m sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
+`sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
 * `config` Config file path. See [Configure](#Configure)
 * `-h, --help` Help message
 * `--log LOG` Logging level, INFO default
-* `--sysu SYSU` System Usages debug info timeout in seconds, 1 hour default
+* `--sysu SYSU` System Usages info timeout in seconds, 1 hour default
 
-For example, simple command line to launch program:  
-`python -u -m sats_receiver /path/to/config.json`  
-You can copy the `default.json` config file from the root of the repository to a
-location of your choice
-
-Program home directory is `~/sats_receiver`  
-Logfile saved to program home directory (`~/sats_receiver/logs`)  
-Tle files stored to program home directory (`~/sats_receiver/tle`)  
+Program home directory is `~/sats_receiver`
+Logfile saved to program home directory (~/sats_receiver/logs)
+Tle files stored to program home directory (~/sats_receiver/tle)
 
 ### Configure
 The configuration file is in JSON format.  
-You can copy the `default.json` file from the root of the repository to a
+You can copy the default.json file from the root of the repository to a
 location of your choice and edit it.
 
 | Field     | Type            | Description                                                |
 |:----------|:----------------|:-----------------------------------------------------------|
 | observer  | Object          | Observer/receiver parameters (see [observer](#observer))   |
 | tle       | Object          | TLE data parameters (see [tle](#tle))                      |
 | receivers | Array of Object | List of receivers parameters (see [receivers](#receivers)) |
@@ -164,59 +138,42 @@
 | freq_correction | Boolean | _Optional._ Correction for basic frequency, Hz. `0` by default                    |
 | mode            | String  | _Optional._ Modulation option (see [modulations](#modulations)). `RAW` by default |
 | decode          | String  | _Optional._ Decoder option (see [decoders](#decoders)). `RAW` by default          |
 | qpsk_baudrate   | Number  | _Required only for **QPSK** mode._ QPSK Baudrate, bps                             |
 | qpsk_excess_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Excess bandwidth. `0.35` by default      |
 | qpsk_ntaps      | Integer | _Optional. Only for **QPSK** mode._ QPSK number of taps. `33` by default          |
 | qpsk_costas_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Costas bandwidth. `0.005` by default     |
-| sstv_wsr        | Number  | _Optional. Only for **SSTV** decoder._ SSTV work samplerate. `16000` by default   |
-| sstv_sync       | Number  | _Optional. Only for **SSTV** decoder._ SSTV syncing. `true` by default            |
 
 
 #### modulations
 * `RAW`
 * `AM`
 * `FM`
 * `WFM`
 * `WFM_STEREO`
 * `QUAD`
 * `QPSK`
 
 #### decoders
 * `RAW` Saved to 2-channel float32 WAV file with `bandwidth` sample rate
 * `RSTREAM` Raw Stream - binary int8. Suitable for further processing, for example, in SatDump
-* `APT` sats-receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
-* `SSTV` SSTV saved to PNG image with EXIF. Supported modes:
-  * `Robot24`
-  * `Robot36`
-  * `Robot72`
-  * `MartinM1`
-  * `MartinM2`
-  * `MartinM3`
-  * `MartinM4`
-  * `PD50`
-  * `PD90`
-  * `PD120`
-  * `PD160`
-  * `PD180`
-  * `PD240`
-  * `PD290`
+* `APT` sats_receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
 * ~~`LRPT`~~ Not implemented yet
 
 
 ### Map Shapes
 Map shapes config file `map_shapes.json` can be found at the root of this repository.
 Shapefiles can be downloaded from [Natural Earth](https://www.naturalearthdata.com/downloads/)
 
-| Field      | Type             | Description                                                                        |
-|:-----------|:-----------------|:-----------------------------------------------------------------------------------|
-| shapes     | Array of Array   | _Optional._ List of shapes data (see [shapes](#shapes))                            |
-| shapes_dir | String           | _Optional. Only when `shapes` specified._ Path to directory contains shapes file   |
-| points     | Object of Object | _Optional._ Additional points to draw on map (see [points](#points))               |
-| line_width | Number           | _Optional._ Overlay lines width, pixels. `1` by default                            |
+| Field      | Type             | Description                                                          |
+|:-----------|:-----------------|:---------------------------------------------------------------------|
+| shapes_dir | String           | Path to directory contains shapes file                               |
+| shapes     | Array of Array   | List of shapes data (see [shapes](#shapes))                          |
+| line_width | Number           | _Optional._ Overlay lines width, pixels. `1` by default              |
+| points     | Object of Object | _Optional._ Additional points to draw on map (see [points](#points)) |
 
 
 #### shapes
 Each shape contain:
 
 | Offset | Field     | Type                       | Description                                                                                                        |
 |:-------|:----------|:---------------------------|:-------------------------------------------------------------------------------------------------------------------|
```

### Comparing `sats_receiver-0.0.1/sats_receiver/__main__.py` & `sats_receiver-0.1.0/sats_receiver/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,46 @@
 #!/usr/bin/env -S python -u
 
 import argparse
-import atexit
 import logging
-import logging.handlers
-import multiprocessing as mp
 import pathlib
 
 from sats_receiver import HOMEDIR, LOGSDIR, TLEDIR, RECDIR
-from sats_receiver.async_signal import AsyncSignal
 from sats_receiver.manager import ReceiverManager
-from sats_receiver.utils import SysUsage
+from sats_receiver.async_signal import AsyncSignal
 
 
-def setup_logging(q: mp.Queue, log_lvl: int):
+def setup_logging(log_lvl):
     if not isinstance(log_lvl, int):
         raise ValueError('Invalid log level: %s' % log_lvl)
 
-    logger = logging.getLogger()
-    logger.setLevel(log_lvl)
-    logger.addHandler(logging.handlers.QueueHandler(q))
-    mp.get_logger().setLevel(log_lvl)
-
-    fmt = logging.Formatter('%(asctime)s %(levelname)s: %(name)s: %(message)s')
+    fmt = '%(asctime)s %(levelname)s: %(name)s: %(message)s'
+    logging.basicConfig(level=log_lvl, format=fmt, filename=LOGSDIR / 'sats_receiver.log')
     sh = logging.StreamHandler()
-    sh.setFormatter(fmt)
-    fh = logging.handlers.TimedRotatingFileHandler(LOGSDIR / 'sats_receiver.log', 'midnight')
-    fh.setFormatter(fmt)
-
-    qhl = logging.handlers.QueueListener(q, sh, fh)
-    qhl.start()
-    atexit.register(qhl.stop)
-
-    # PIL logging level
-    pil_logger = logging.getLogger('PIL')
-    pil_logger.setLevel(logging.DEBUG + 2)
+    sh.setFormatter(logging.Formatter(fmt))
+    logging.getLogger().addHandler(sh)
 
 
 if __name__ == '__main__':
     ap = argparse.ArgumentParser()
     ap.add_argument('config', type=pathlib.Path, help='Config file path')
-    ap.add_argument('--log', default='INFO', type=(lambda x: getattr(logging, x.upper(), None)),
-                    help='Logging level, INFO default')
-    ap.add_argument('--sysu', default=SysUsage.DEFAULT_INTV, type=int,
-                    help='System Usages info timeout in seconds, 1 hour default')
+    ap.add_argument('--log', default='INFO', type=(lambda x: getattr(logging, x.upper(), None)), help='Logging level, INFO default')
+    ap.add_argument('--sysu', default=3600, type=int, help='System Usages info timeout in seconds, 1 hour default')
     args = ap.parse_args()
 
     for d in LOGSDIR, TLEDIR, RECDIR:
         if not d.exists():
             d.mkdir(parents=True, exist_ok=True)
 
-    q = mp.Queue()
-    setup_logging(q, args.log)
+    setup_logging(args.log)
 
     logging.info('Hello!')
 
-    asig = AsyncSignal(['SIGABRT', 'SIGHUP', 'SIGINT', 'SIGTERM', 'SIGUSR1', 'SIGUSR2', 'SIGBREAK'])
-    mng = ReceiverManager(q, args.config, args.sysu)
+    asig = AsyncSignal(['SIGABRT', 'SIGHUP', 'SIGINT', 'SIGTERM', 'SIGUSR1', 'SIGUSR2'])
+    mng = ReceiverManager(args.config, args.sysu)
 
     while not mng.action():
         signame = asig.wait(1)
         if signame:
             if 'USR' in signame:
                 # TODO
                 pass
```

### Comparing `sats_receiver-0.0.1/sats_receiver/async_signal.py` & `sats_receiver-0.1.0/sats_receiver/async_signal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-import multiprocessing as mp
+import errno
+import fcntl
 import os
+import select
 import signal
+import time
 
 
 SIG = {}
 for n, v in signal.__dict__.items():
     if n.startswith('SIG') and n.isalnum() and isinstance(v, int):
         SIG[n] = v
         SIG[n[3:]] = v
@@ -20,52 +23,72 @@
         if signals is None:
             signals = ['SIGINT']
 
         for s in signals:
             try:
                 sig = int(s)
             except ValueError:
-                sig = SIG.get(s, -1)
+                sig = SIG[s]
 
-            if not (0 < sig < 256 and sig in SIG):
-                continue
+            assert 0 < sig < 256 and sig in SIG
 
             old = signal.signal(sig, self._handler)
             if old is None:
                 old = signal.SIG_DFL
             self.olds[sig] = old
 
         if self.olds:
             self.pid = os.getpid()
-            self.rd, self.wr = mp.Pipe(False)
+            self.rd, self.wr = os.pipe()
+            self._tune(self.rd)
+            self._tune(self.wr)
 
     def close(self):
         if self.olds:
             for sig, old in self.olds.items():
                 signal.signal(sig, old)
-            self.rd.close()
-            self.wr.close()
+            os.close(self.rd)
+            os.close(self.wr)
         self.olds = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
+    def _tune(self, fd):
+        fcntl.fcntl(fd, fcntl.F_SETFL, fcntl.fcntl(fd, fcntl.F_GETFL) | os.O_NONBLOCK)
+        fcntl.fcntl(fd, fcntl.F_SETFD, fcntl.fcntl(fd, fcntl.F_GETFD) | fcntl.FD_CLOEXEC)
+
     def _handler(self, signum, frame):
         if os.getpid() != self.pid:
             os.kill(self.pid, signum)
         else:
-            self.wr.send(signum)
+            try:
+                os.write(self.wr, chr(signum).encode())
+            except ValueError:
+                pass
 
     def wait(self, t=None):
-        try:
-            x = self.rd.poll(t)
-        except InterruptedError:
-            x = 1
+        if t and t > 0:
+            till = time.monotonic() + t
 
-        if x:
+        while 1:
             try:
-                return SIG[self.rd.recv()]
-            except:
-                return
+                select.select((self.rd,), (), (), t)
+                break
+            except select.error as e:
+                if e[0] == errno.EINTR:
+                    if t and t > 0:
+                        t = till - time.monotonic()
+                        if t <= 0:
+                            break
+                    continue
+                if e[0] == errno.EBADF:
+                    return
+                raise
+
+        try:
+            return SIG[ord(os.read(self.rd, 1))]
+        except:
+            return
```

### Comparing `sats_receiver-0.0.1/sats_receiver/gr_modules/decoders.py` & `sats_receiver-0.1.0/sats_receiver/gr_modules/decoders.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,20 +11,16 @@
 import gnuradio.analog
 import gnuradio.blocks
 import gnuradio.digital
 import gnuradio.fft
 import gnuradio.filter
 import gnuradio.gr
 
-from PIL import ExifTags
-
 from sats_receiver import utils
-from sats_receiver.gr_modules.epb import sstv as sstv_epb
-from sats_receiver.observer import Observer
-from sats_receiver.systems import apt, sstv
+from sats_receiver.systems import apt
 
 
 class Decoder(gr.gr.hier_block2):
     def __init__(self,
                  name: str,
                  sat_name: str,
                  samp_rate: Union[int, float],
@@ -38,15 +34,15 @@
             gr.gr.io_signature(0, 0, 0)
         )
 
         self.now = dt.datetime.fromtimestamp(0)
         self.sat_name = sat_name
         self.samp_rate = samp_rate
         self.out_dir = out_dir
-        self.tmp_file = utils.mktmp(prefix='_'.join(name.lower().split()))
+        self.tmp_file = out_dir / ('_'.join(name.lower().split()) + '.tmp')
         self.base_kw = dict(log=self.log, sat_name=sat_name, out_dir=out_dir)
 
     def start(self):
         self.tmp_file = self.out_dir / ('_'.join([self.t.strftime('%Y%m%d%H%M%S'),
                                                   *self.name().lower().split()]) + '.tmp')
         self.base_kw.update(tmp_file=self.tmp_file)
 
@@ -73,15 +69,15 @@
             2,
             samp_rate,
             gr.blocks.FORMAT_WAV,
             gr.blocks.FORMAT_FLOAT,
             False
         )
         self.wav_sink.close()
-        utils.unlink(self.tmp_file)
+        self.tmp_file.unlink(True)
 
         self.connect(self, self.ctf, self.wav_sink)
         self.connect((self.ctf, 1), (self.wav_sink, 1))
 
     def start(self):
         super(RawDecoder, self).start()
 
@@ -95,35 +91,34 @@
     @staticmethod
     def _raw_finalize(log, sat_name, out_dir, tmp_file, fin_key) -> Optional[tuple[str, str, str, dt.datetime]]:
         log.debug('finalizing...')
 
         d = dt.datetime.fromtimestamp(tmp_file.stat().st_mtime, dateutil.tz.tzutc())
         res_fn = tmp_file.rename(out_dir / d.strftime(f'{sat_name}_%Y-%m-%d_%H-%M-%S_RAW.wav'))
         st = res_fn.stat()
-        log.info('finish: %s (%s)', res_fn, utils.numbi_disp(st.st_size))
+        log.info('finish: %s (%s)', res_fn, utils.numdisp(st.st_size))
 
         return sat_name, fin_key, res_fn, dt.datetime.fromtimestamp(st.st_mtime, dateutil.tz.tzutc())
 
 
 class AptDecoder(Decoder):
     def __init__(self,
                  sat_name: str,
                  samp_rate: Union[int, float],
                  out_dir: pathlib.Path,
                  sat_ephem_tle: Optional[tuple[ephem.EarthSatellite, tuple[str, str, str]]],
                  observer_lonlat: tuple[float, float]):
         name = 'APT Decoder'
         super(AptDecoder, self).__init__(name, sat_name, samp_rate, out_dir)
 
-        pfx = '_'.join(name.lower().split())
-        self.corr_file = utils.mktmp(dir=out_dir, prefix=pfx, suffix='.corr')
-        self.peaks_file = utils.mktmp(dir=out_dir, prefix=pfx, suffix='.peaks')
+        self.corr_file = out_dir / ('_'.join(name.lower().split()) + '.corr')
+        self.peaks_file = out_dir / ('_'.join(name.lower().split()) + '.peaks')
         self.sat_ephem_tle = sat_ephem_tle
         self.observer_lonlat = observer_lonlat
-        self.base_kw.update(sat_tle=sat_ephem_tle[1], observer_lonlat=observer_lonlat)
+        self.base_kw.update(sat_tle=self.sat_ephem_tle[1], observer_lonlat=self.observer_lonlat)
 
         resamp_gcd = math.gcd(samp_rate, apt.Apt.WORK_RATE)
 
         self.frs = gr.blocks.rotator_cc(2 * math.pi * -apt.Apt.CARRIER_FREQ / samp_rate)
         self.rsp = gr.filter.rational_resampler_ccc(
             interpolation=apt.Apt.WORK_RATE // resamp_gcd,
             decimation=samp_rate // resamp_gcd,
@@ -155,21 +150,29 @@
             threshold=0.9,
             threshold_method=gr.digital.THRESHOLD_ABSOLUTE,
         )
         self.ctf_out = gr.blocks.complex_to_float()
         self.ctf_corr = gr.blocks.complex_to_float()
 
         self.out_file_sink = gr.blocks.file_sink(gr.gr.sizeof_float, str(self.tmp_file), False)
+        self.out_file_sink.close()
+        self.tmp_file.unlink(True)
+
         self.out_corr_sink = gr.blocks.file_sink(gr.gr.sizeof_float, str(self.corr_file), False)
+        self.out_corr_sink.close()
+        self.corr_file.unlink(True)
+
         self.peak_detector = gr.blocks.peak_detector2_fb(
             threshold_factor_rise=7,
             look_ahead=apt.Apt.FRAME_WIDTH * apt.Apt.WORK_RATE // apt.Apt.FINAL_RATE,
             alpha=0.001,
         )
         self.out_peaks_sink = gr.blocks.file_sink(gr.gr.sizeof_char, str(self.peaks_file), False)
+        self.out_peaks_sink.close()
+        self.peaks_file.unlink(True)
 
         self.connect(
             self,
             self.frs,
             self.rsp,
             self.lpf,
             self.ctm,
@@ -186,17 +189,14 @@
         )
         self.connect(
             self.ctf_corr,
             self.peak_detector,
             self.out_peaks_sink,
         )
 
-        utils.close(self.out_file_sink, self.out_corr_sink, self.out_peaks_sink)
-        utils.unlink(self.tmp_file, self.corr_file, self.peaks_file)
-
     def start(self):
         super(AptDecoder, self).start()
         self.corr_file = self.out_dir / ('_'.join([self.now.strftime('%Y%m%d%H%M%S'),
                                                    *self.name().lower().split()]) + '.corr.tmp')
         self.peaks_file = self.out_dir / ('_'.join([self.now.strftime('%Y%m%d%H%M%S'),
                                                     *self.name().lower().split()]) + '.peaks.tmp')
         self.base_kw.update(corr_file=self.corr_file, peaks_file=self.peaks_file)
@@ -207,24 +207,24 @@
         self.out_corr_sink.open(str(self.corr_file))
         self.out_corr_sink.set_unbuffered(False)
 
         self.out_peaks_sink.open(str(self.peaks_file))
         self.out_peaks_sink.set_unbuffered(False)
 
     def finalize(self, executor, fin_key: str):
-        self.out_file_sink.do_update()
-        self.out_corr_sink.do_update()
-        self.out_peaks_sink.do_update()
-
-        utils.close(self.out_file_sink, self.out_corr_sink, self.out_peaks_sink)
+        self.out_file_sink.close()
+        self.out_corr_sink.close()
+        self.out_peaks_sink.close()
 
         for p in self.tmp_file, self.corr_file, self.peaks_file:
             if not p.exists():
                 self.log.warning('%s: missing components `%s`', p)
-                utils.unlink(self.tmp_file, self.corr_file, self.peaks_file)
+                self.tmp_file.unlink(True)
+                self.corr_file.unlink(True)
+                self.peaks_file.unlink(True)
                 return
 
         executor.execute(self._apt_finalize, **self.base_kw, fin_key=fin_key)
 
     @staticmethod
     def _apt_finalize(log: logging.Logger,
                       sat_name: str,
@@ -236,21 +236,23 @@
                       out_dir: pathlib.Path,
                       fin_key: str) -> Optional[tuple[str, str, pathlib.Path, dt.datetime]]:
         log.debug('finalizing...')
 
         a = apt.Apt(sat_name, tmp_file, corr_file, peaks_file, sat_tle, observer_lonlat)
         x = a.process()
 
-        utils.unlink(tmp_file, corr_file, peaks_file)
+        tmp_file.unlink(True)
+        corr_file.unlink(True)
+        peaks_file.unlink(True)
 
         if x:
             log.info('finish with error')
         else:
             res_fn, sz = a.to_apt(out_dir)
-            log.info('finish: %s (%s)', res_fn, utils.numbi_disp(sz))
+            log.info('finish: %s (%s)', res_fn, utils.numdisp(sz))
 
             return sat_name, fin_key, res_fn, a.end_time
 
 
 class RawStreamDecoder(Decoder):
     def __init__(self,
                  sat_name: str,
@@ -263,15 +265,15 @@
         self.rail = gr.analog.rail_ff(-1, 1)
         self.ftch = gr.blocks.float_to_char(1, 127)
         # self.fts = gr.blocks.float_to_short(1, 32767)
         # self.stch = gr.blocks.short_to_char(1)
 
         self.out_file_sink = gr.blocks.file_sink(gr.gr.sizeof_char, str(self.tmp_file), False)
         self.out_file_sink.close()
-        utils.unlink(self.tmp_file)
+        self.tmp_file.unlink(True)
 
         self.connect(
             self,
             self.ctf,
             self.rail,
             self.ftch,
             self.out_file_sink,
@@ -280,15 +282,14 @@
     def start(self):
         super(RawStreamDecoder, self).start()
 
         self.out_file_sink.open(str(self.tmp_file))
         self.out_file_sink.set_unbuffered(False)
 
     def finalize(self, executor, fin_key: str):
-        self.out_file_sink.do_update()
         self.out_file_sink.close()
         if self.tmp_file.exists():
             executor.execute(self._raw_stream_finalize, **self.base_kw, fin_key=fin_key)
 
     @staticmethod
     def _raw_stream_finalize(log: logging.Logger,
                              sat_name: str,
@@ -296,15 +297,15 @@
                              tmp_file: pathlib.Path,
                              fin_key: str) -> Optional[tuple[str, str, pathlib.Path, dt.datetime]]:
         log.debug('finalizing...')
 
         d = dt.datetime.fromtimestamp(tmp_file.stat().st_mtime, dateutil.tz.tzutc())
         res_fn = tmp_file.rename(out_dir / d.strftime(f'{sat_name}_%Y-%m-%d_%H-%M-%S_RAW.s'))
         st = res_fn.stat()
-        log.info('finish: %s (%s)', res_fn, utils.numbi_disp(st.st_size))
+        log.info('finish: %s (%s)', res_fn, utils.numdisp(st.st_size))
 
         return sat_name, fin_key, res_fn, dt.datetime.fromtimestamp(st.st_mtime, dateutil.tz.tzutc())
 
 
 class LrptDecoder(RawStreamDecoder):
     def __init__(self,
                  sat_name: str,
@@ -314,125 +315,7 @@
         super(LrptDecoder, self).__init__(sat_name, samp_rate, out_dir, name='LRPT Decoder')
 
     def start(self):
         super(LrptDecoder, self).start()
 
     def finalize(self, executor, fin_key: str):
         super(LrptDecoder, self).finalize(executor, fin_key)
-
-
-class SstvDecoder(Decoder):
-    _FREQ_1 = (1900 - 1200) / 2
-
-    def __init__(self,
-                 sat_name: str,
-                 samp_rate: Union[int, float],
-                 out_dir: pathlib.Path,
-                 observer: Observer,
-                 do_sync=True,
-                 wsr=16000):
-        super(SstvDecoder, self).__init__('SSTV Decoder', sat_name, samp_rate, out_dir)
-
-        self.observer = observer
-        self.do_sync = do_sync
-        self.wsr = wsr
-
-        hdr_pix_width = int(wsr * sstv.Sstv.HDR_PIX_S)
-        hdr = sstv.Sstv.HDR_SYNC_WORD.repeat(hdr_pix_width)
-        resamp_gcd = math.gcd(wsr, samp_rate)
-
-        self.bpf_input = gr.filter.fir_filter_ccc(
-            1,
-            gr.filter.firdes.complex_band_pass(
-                1,          # gain
-                samp_rate,  # sampling_freq
-                900,        # low_cutoff_freq
-                2500,       # high_cutoff_freq
-                200,        # transition_width
-                gr.fft.window.WIN_HAMMING,
-                6.76))
-        self.frs = gr.blocks.rotator_cc(2 * math.pi * -(1900 - self._FREQ_1) / samp_rate)
-        self.quad_demod = gr.analog.quadrature_demod_cf((samp_rate / (2 * math.pi * self._FREQ_1)))
-        self.rsp = gr.filter.rational_resampler_fcc(
-                interpolation=samp_rate // resamp_gcd,
-                decimation=wsr // resamp_gcd,
-                taps=[],
-                fractional_bw=0
-        )
-        self.correllator = gr.digital.corr_est_cc(hdr, hdr_pix_width, 1, 0.4, gr.digital.THRESHOLD_ABSOLUTE)
-        self.ctf_out = gr.blocks.complex_to_float()
-        self.out_add_const = gr.blocks.add_const_ff(450 / self._FREQ_1)
-        self.out_multiply_const = gr.blocks.multiply_const_ff(self._FREQ_1 / (750 + 450))
-        self.ctf_corr = gr.blocks.complex_to_float()
-        self.corr_peak_detector = gr.blocks.peak_detector2_fb(0.1, hdr.size, 0.001)
-        self.sstv_epb = sstv_epb.SstvEpb(wsr, do_sync, self.log, sat_name, out_dir)
-
-        self.connect(
-            self,
-            self.bpf_input,
-            self.frs,
-            self.quad_demod,
-            self.rsp,
-            self.correllator,
-            self.ctf_out,
-            self.out_add_const,
-            self.out_multiply_const,
-            (self.sstv_epb, self.sstv_epb.OUT_IN),
-        )
-        self.connect(
-            (self.correllator, 1),
-            self.ctf_corr,
-            self.corr_peak_detector,
-            (self.sstv_epb, self.sstv_epb.PEAKS_IN),
-        )
-
-        latlonalt = str(observer.lat), str(observer.lon), observer.elev
-        self.base_kw.update(observer_latlonalt=latlonalt)
-
-    def start(self):
-        # super(SstvDecoder, self).start()
-        utils.unlink(self.tmp_file)
-
-    def finalize(self, executor, fin_key: str):
-        self.sstv_epb.stop()
-        sstv_rr: list[sstv.SstvRecognizer] = self.sstv_epb.finalize()
-        executor.execute(self._sstv_finalize, **self.base_kw, sstv_rr=sstv_rr, fin_key=fin_key)
-
-    @staticmethod
-    def _sstv_finalize(log: logging.Logger,
-                       sat_name: str,
-                       out_dir: pathlib.Path,
-                       observer_latlonalt: tuple[str, str, Union[int, float]],
-                       sstv_rr: list[sstv.SstvRecognizer],
-                       fin_key: str) -> tuple[str, str, list[tuple[pathlib.Path, dt.datetime]]]:
-        log.debug('finalizing...')
-
-        observer = ephem.Observer()
-        observer.lat, observer.lon, observer.elev = observer_latlonalt
-        fn_dt = []
-        sz_sum = 0
-        for i in sstv_rr:
-            img = i.get_image()
-            if not img:
-                continue
-
-            log.debug('add GPSInfo EXIF')
-            img = utils.img_add_exif(img, observer=observer)
-            exif = img.getexif()
-
-            sstv_mode = exif.get_ifd(ExifTags.IFD.Exif).get(ExifTags.Base.UserComment, 'SSTV')
-            end_time = exif.get(ExifTags.Base.DateTime)
-            end_time = (dt.datetime.strptime(end_time, '%Y:%m:%d %H:%M:%S')
-                        if end_time
-                        else dt.datetime.utcnow())
-            res_fn = out_dir / end_time.strftime(f'{sat_name}_{sstv_mode}_%Y-%m-%d_%H-%M-%S,%f.png')
-
-            img.save(res_fn, exif=exif)
-
-            fn_dt.append((res_fn, end_time))
-            sz = res_fn.stat().st_size
-            sz_sum += sz
-            log.info('finish: %s (%s)', res_fn, utils.numbi_disp(sz))
-
-        log.info('finish %s images (%s)', len(fn_dt), utils.numbi_disp(sz_sum))
-
-        return sat_name, fin_key, fn_dt
```

### Comparing `sats_receiver-0.0.1/sats_receiver/gr_modules/demodulators.py` & `sats_receiver-0.1.0/sats_receiver/gr_modules/demodulators.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.0.1/sats_receiver/gr_modules/modules.py` & `sats_receiver-0.1.0/sats_receiver/gr_modules/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import gnuradio.analog
 import gnuradio.blocks
 import gnuradio.filter
 import gnuradio.gr
 
 from sats_receiver import utils
 from sats_receiver.gr_modules import decoders, demodulators
-from sats_receiver.observer import Observer
 
 
 class RadioModule(gr.gr.hier_block2):
     def __init__(self,
                  main_tune: Union[int, float],
                  samp_rate: Union[int, float],
                  bandwidth: Union[int, float],
@@ -77,28 +76,25 @@
                         'mode',
                         # 'decode',           # optional
 
                         # 'qpsk_baudrate',    # only in QPSK demode
                         # 'qpsk_excess_bw',   # optional
                         # 'qpsk_ntaps',       # optional
                         # 'qpsk_costas_bw',   # optional
-
-                        # 'sstv_wsr',         # optional, only in SSTV decode
-                        # 'sstv_sync',        # optional, only in SSTV decode
                     ]))
             and (config['mode'] != utils.Mode.QPSK or 'qpsk_baudrate' in config)
         )
 
     def __init__(self,
                  up: 'Satellite',
                  config: Mapping,
                  main_tune: Union[int, float],
                  samp_rate: Union[int, float]):
         f = config.get('freq')
-        self.prefix = f'{self.__class__.__name__}: {up.name}: {f and f": {utils.num_disp(f)}Hz"}'
+        self.prefix = f'{self.__class__.__name__}: {up.name}: {f and f": {utils.numdisp(f)}Hz"}'
 
         if not self._validate_config(config):
             raise ValueError(f'{self.prefix}: Invalid config!')
 
         super(SatRecorder, self).__init__(
             self.prefix,
             gr.gr.io_signature(1, 1, gr.gr.sizeof_gr_complex),
@@ -157,29 +153,26 @@
         elif self.mode == utils.Mode.QUAD:
             self.demodulator = gr.analog.quadrature_demod_cf(1)
 
         elif self.mode == utils.Mode.QPSK:
             self.demodulator = demodulators.QpskDemod(self.bandwidth, self.qpsk_baudrate, self.qpsk_excess_bw, self.qpsk_ntaps, self.qpsk_costas_bw)
 
         if self.decode == utils.Decode.APT:
-            self.decoder = decoders.AptDecoder(up.name, self.bandwidth, up.output_directory, up.sat_ephem_tle, up.observer.lonlat)
+            self.decoder = decoders.AptDecoder(up.name, self.bandwidth, up.output_directory, up.sat_ephem_tle, up.observer_lonlat)
 
         # elif self.decode == Decode.LRPT:
         #     # TODO
         #     # self.decoder =
 
         elif self.decode == utils.Decode.RSTREAM:
             self.decoder = decoders.RawStreamDecoder(up.name, self.bandwidth, up.output_directory)
 
         elif self.decode == utils.Decode.RAW:
             self.decoder = decoders.RawDecoder(up.name, self.bandwidth, up.output_directory)
 
-        elif self.decode == utils.Decode.SSTV:
-            self.decoder = decoders.SstvDecoder(up.name, self.bandwidth, up.output_directory, up.observer, self.sstv_sync, self.sstv_wsr)
-
         self.connect(
             self,
             self.radio,
             *((self.demodulator, self.post_demod) if self.demodulator else tuple()),
             self.decoder,
         )
 
@@ -212,39 +205,31 @@
 
     @property
     def mode(self) -> utils.Mode:
         return utils.Mode(self.config.get('mode', utils.Mode.RAW.value))
 
     @property
     def decode(self) -> utils.Decode:
-        return utils.Decode(self.config.get('decode', utils.Decode.RAW.value))
+        return utils.Decode(self.config.get('decode', utils.Decode.RAW.value)) or utils.Decode.RAW
 
     @property
     def qpsk_baudrate(self) -> Union[int, float]:
         return self.config['qpsk_baudrate']
 
     @property
     def qpsk_excess_bw(self) -> Union[int, float]:
-        return self.config.get('qpsk_excess_bw', 0.35)
+        return self.config.get('qpsk_excess_bw')
 
     @property
     def qpsk_ntaps(self) -> int:
-        return int(self.config.get('qpsk_ntaps'), 33)
-
-    @property
-    def qpsk_costas_bw(self) -> Union[int, float]:
-        return self.config.get('qpsk_costas_bw', 0.005)
-
-    @property
-    def sstv_wsr(self) -> Union[int, float]:
-        return self.config.get('sstv_wsr', 16000)
+        return int(self.config.get('qpsk_ntaps'))
 
     @property
-    def sstv_sync(self) -> bool:
-        return self.config.get('sstv_sync', True)
+    def qpsk_costas_bw(self):
+        return self.config.get('qpsk_costas_bw')
 
 
 class Satellite(gr.gr.hier_block2):
     @staticmethod
     def _validate_config(config: Mapping) -> bool:
         return (
             all(map(lambda x: x in config,
@@ -257,15 +242,15 @@
                     ]))
             and config['frequencies']
         )
 
     def __init__(self,
                  config: Mapping,
                  sat_ephem_tle: Optional[tuple[ephem.EarthSatellite, tuple[str, str, str]]],
-                 observer: Observer,
+                 observer_lonlat: tuple[Union[int, float], Union[int, float]],
                  main_tune: Union[int, float],
                  samp_rate: Union[int, float],
                  output_directory: pathlib.Path,
                  executor):
         n = config.get('name', '')
         self.prefix = f'{self.__class__.__name__}{n and f": {n}"}'
         self.log = logging.getLogger(self.prefix)
@@ -276,15 +261,15 @@
         super(Satellite, self).__init__(
             self.prefix,
             gr.gr.io_signature(1, 1, gr.gr.sizeof_gr_complex),
             gr.gr.io_signature(0, 0, 0)
         )
 
         self.sat_ephem_tle = sat_ephem_tle
-        self.observer = observer
+        self.observer_lonlat = observer_lonlat
         self.executor = executor
         self.config = config
         self.output_directory = output_directory / self.name
         self.output_directory.mkdir(parents=True, exist_ok=True)
         self.events: list[Optional[utils.Event]] = [None, None, None]
         self.recorders = []
```

### Comparing `sats_receiver-0.0.1/sats_receiver/gr_modules/receiver.py` & `sats_receiver-0.1.0/sats_receiver/gr_modules/receiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import gnuradio as gr
 import gnuradio.blocks
 import gnuradio.gr
 import gnuradio.soapy
 
 from sats_receiver.gr_modules import modules
-from sats_receiver.utils import num_disp
 
 try:
     from sats_receiver import librtlsdr
     LIBRTLSDR = None
 except OSError as e:
     LIBRTLSDR = str(e)
 
@@ -125,15 +124,15 @@
 
                 sat_ephem_tle = self.up.tle.get(sat_name)
                 if sat_ephem_tle is None:
                     self.log.info('Sat `%s` not found in TLE. Skip', sat_name)
                     continue
 
                 try:
-                    sat = modules.Satellite(cfg, sat_ephem_tle, self.up.observer, self.tune, self.samp_rate, self.output_directory, self.up.executor)
+                    sat = modules.Satellite(cfg, sat_ephem_tle, self.up.observer.lonlat, self.tune, self.samp_rate, self.output_directory, self.up.executor)
                 except ValueError as e:
                     self.log.warning('%s: %s. Skip', sat_name, e)
                     continue
 
                 if self.calculate_pass(sat):
                     if self.is_runned:
                         self.connect(self.blocks_correctiq, sat)
@@ -219,16 +218,16 @@
         True when at least one satellite recorder is running
         """
 
         return any(x.is_runned for x in self.satellites.values())
 
     def start(self, max_noutput_items=10000000):
         if self.enabled and not self.is_runned:
-            self.log.info('START tune=%sHz samp_rate=%sHz gain=%s biast=%s',
-                          num_disp(self.tune, 3), num_disp(self.samp_rate, 3), self.gain, self.biast)
+            self.log.info('START tune=%s samp_rate=%s gain=%s biast=%s',
+                          self.tune, self.samp_rate, self.gain, self.biast)
 
             self.set_biast(self.biast)
 
             try:
                 self.signal_src = gr.soapy.source(f'driver={self.source}{self.serial and f",serial={self.serial}"}',
                                                   'fc32', 1, '', '', [''], [''])
             except RuntimeError as e:
@@ -346,13 +345,13 @@
     def recalculate_pass(self):
         for sat in self.satellites.values():
             self.up.scheduler.cancel(*sat.events)
             sat.events = [None, None, None]
             self.calculate_pass(sat)
 
     def set_biast(self, v, silent=False):
-        if self.source == 'rtlsdr' and not LIBRTLSDR:
+        if not LIBRTLSDR and self.source == 'rtlsdr':
             try:
                 librtlsdr.set_bt(v, self.serial)
             except librtlsdr.LibRtlSdrError as e:
                 if not silent:
                     self.log.info('change bias-t error: %s', e)
```

### Comparing `sats_receiver-0.0.1/sats_receiver/librtlsdr.py` & `sats_receiver-0.1.0/sats_receiver/librtlsdr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-import sys
-
 from ctypes import CDLL, c_char, c_char_p, c_int, c_uint32, c_void_p, POINTER
 
-
-if sys.platform == 'win32':
-    _lib = CDLL('rtlsdr')
-else:
-    _lib = CDLL('librtlsdr.so.0')
+_lib = CDLL('librtlsdr.so.0')
+rtlsdr_dev_p = c_void_p
 
 
 class LibRtlSdrError(RuntimeError):
     pass
 
 
 class LibUsbError(RuntimeError):
@@ -31,16 +26,14 @@
         -99: 'Other error',
     }
 
     def __init__(self, err_code):
         super(LibUsbError, self).__init__(f'[{err_code}] {self.CODES.get(err_code, -99)}')
 
 
-rtlsdr_dev_p = c_void_p
-
 _f = _lib.rtlsdr_open
 _f.argtypes = POINTER(rtlsdr_dev_p), c_uint32
 _f.restype = c_int
 def rtlsdr_open(idx=0) -> rtlsdr_dev_p:
     dev = rtlsdr_dev_p(None)
     if _lib.rtlsdr_open(dev, idx):
         raise LibRtlSdrError('Could not open RTL-SDR')
```

### Comparing `sats_receiver-0.0.1/sats_receiver/manager.py` & `sats_receiver-0.1.0/sats_receiver/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,135 +1,96 @@
 import atexit
 import datetime as dt
 import json
 import logging
-import logging.handlers
 import multiprocessing as mp
 import pathlib
 import time
+import queue
 
 from typing import Mapping
 
 from sats_receiver.gr_modules.receiver import RecUpdState, SatsReceiver
 from sats_receiver.observer import Observer
 from sats_receiver.tle import Tle
 from sats_receiver.utils import Scheduler, SysUsage
 
 
 class Executor(mp.Process):
-    def __init__(self, q: mp.Queue = None, sysu_intv=SysUsage.DEFAULT_INTV):
-        super().__init__(daemon=False, name=self.__class__.__name__)
+    def __init__(self, sysu_intv=SysUsage.DEFAULT_INTV):
+        self.prefix = self.__class__.__name__
+        self.log = logging.getLogger(self.prefix)
 
-        self.q = q
-        self.sysu_intv = sysu_intv
-        self.rd, self.wr = mp.Pipe(False)
+        super().__init__(daemon=False)
 
-    def _setup_process(self):
-        logger = logging.getLogger()
-        logger.handlers.clear()
-        logger.setLevel(mp.get_logger().level)
-        if self.q is not None:
-            qh = logging.handlers.QueueHandler(self.q)
-            logger.addHandler(qh)
-            # logging.basicConfig(level=mp.get_logger().level, handlers=[qh])
-        self.log = logging.getLogger(self.name)
-        self.sysu = SysUsage(self.name, self.sysu_intv)
-
-    def start(self) -> None:
-        super(Executor, self).start()
-        self.rd.close()
+        self.sysu_intv = sysu_intv
+        self.q = mp.Queue()
 
     def run(self):
-        self._setup_process()
-
         self.log.debug('start')
 
-        try:
-            self.action()
-        except:
-            self.log.exception('Exception:')
-        finally:
-            try:
-                self.stop()
-            except:
-                self.log.exception('stop Exception:')
+        sysu = SysUsage(self.prefix, self.sysu_intv)
 
-        self.log.debug('finish')
-
-    def action(self):
         while 1:
-            self.sysu.collect()
+            sysu.collect()
 
             try:
-                x = self.rd.poll(1)
-            except InterruptedError:
-                x = 1
-            except:
-                continue
-
-            if not x:
+                x = self.q.get(timeout=1)
+            except queue.Empty:
                 continue
 
-            x = self.rd.recv()
-
             if x == '.':
                 break
 
             try:
                 fn, args, kwargs = x
             except ValueError:
                 self.log.error('invalid task: %s', x)
                 continue
 
             if callable(fn):
                 try:
                     x = fn(*args, **kwargs)
                 except Exception:
                     self.log.exception('%s with args=%s kwargs=%s', fn, args, kwargs)
-                    continue
 
-                if x and isinstance(x, tuple):
-                    if len(x) == 4:
-                        sat_name, fin_key, res_filename, end_time = x
-                    elif len(x) == 3:
-                        sat_name, fin_key, fn_dt = x
+                if x and isinstance(x, tuple) and len(x) == 4:
+                    sat_name, fin_key, res_filename, end_time = x
+
+        self.log.debug('finish')
 
     def execute(self, fn, *args, **kwargs):
-        if self.wr:
-            self.wr.send((fn, args, kwargs))
+        self.q.put((fn, args, kwargs))
 
     def stop(self):
-        if self.wr:
-            self.wr.send('.')
-            self.wr.close()
-            self.wr = 0
+        self.q.put('.')
 
 
 class ReceiverManager:
-    def __init__(self, q: mp.Queue, config_filename: pathlib.Path, sysu_intv=SysUsage.DEFAULT_INTV, executor_cls=Executor):
+    def __init__(self, config_filename: pathlib.Path, sysu_intv=SysUsage.DEFAULT_INTV, executor_cls=Executor):
         self.prefix = self.__class__.__name__
         self.log = logging.getLogger(self.prefix)
 
         self.sysu = SysUsage(self.prefix, sysu_intv)
-        self.config_filename = config_filename.expanduser().absolute()
+        self.config_filename = config_filename
         self.config_file_stat = None
         self.config = {}
 
         self.receivers: dict[str, SatsReceiver] = {}
         self.stopped = False
         self.now = dt.datetime.now(dt.timezone.utc)
         self.file_failed_t = 0
 
         if not self.update_config(True, True):
             raise ValueError(f'{self.prefix}: Invalid config!')
 
         self.observer = Observer(self.config['observer'])
         self.tle = Tle(self.config['tle'])
         self.scheduler = Scheduler()
-        self.executor = executor_cls(q, sysu_intv)
+        self.executor = executor_cls(sysu_intv)
         self.executor.start()
         atexit.register(lambda x: (x.stop(), x.join()), self.executor)
 
         for cfg in self.config['receivers']:
             self._add_receiver(cfg)
 
     def _add_receiver(self, cfg: Mapping):
```

### Comparing `sats_receiver-0.0.1/sats_receiver/observer.py` & `sats_receiver-0.1.0/sats_receiver/observer.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.0.1/sats_receiver/systems/apt.py` & `sats_receiver-0.1.0/sats_receiver/systems/apt.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.0.1/sats_receiver/tle.py` & `sats_receiver-0.1.0/sats_receiver/tle.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.0.1/sats_receiver.egg-info/PKG-INFO` & `sats_receiver-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sats-receiver
-Version: 0.0.1
+Name: sats_receiver
+Version: 0.1.0
 Summary: Satellites data receiver based on GNU Radio
 Home-page: https://github.com/baskiton/sats-receiver
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baskiton/sats-receiver/issues
 Classifier: License :: OSI Approved :: MIT License
@@ -12,112 +12,86 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sats Receiver
-[![PyPI](https://img.shields.io/pypi/v/sats-receiver?logo=python&logoColor=white)][pypi_proj]
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/sats-receiver?logo=python&logoColor=white)][pypi_proj]
-[![PyPI - License](https://img.shields.io/pypi/l/sats-receiver?logo=open-source-initiative&logoColor=white)][license]  
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/tests.yml?label=tests&logo=github)][tests]
-[![Codecov branch](https://img.shields.io/codecov/c/gh/baskiton/sats-receiver/dev?logo=codecov)][codecov]
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/pypi-upload.yml?label=upload&logo=github)][upload]
-
-[pypi_proj]: https://pypi.org/project/sats-receiver/
-[license]: https://github.com/baskiton/sats-receiver/blob/main/LICENSE
-[tests]: https://github.com/baskiton/sats-receiver/actions/workflows/tests.yml
-[codecov]: https://app.codecov.io/gh/baskiton/sats-receiver
-[upload]: https://github.com/baskiton/sats-receiver/actions/workflows/pypi-upload.yml
+[![PyPI](https://img.shields.io/pypi/v/sats_receiver?logo=python&logoColor=white)][pypi_proj]
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/sats_receiver?logo=python&logoColor=white)][pypi_proj]
+[![PyPI - License](https://img.shields.io/pypi/l/sats_receiver?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/sats-receiver/blob/main/LICENSE)
+[![upload](https://img.shields.io/github/actions/workflow/status/baskiton/sats_receiver/pypi-upload.yml?label=upload&logo=github)](https://github.com/baskiton/sats-receiver/actions/workflows/pypi-upload.yml)
+
+[pypi_proj]: https://pypi.org/project/sats_receiver/
 
 Satellites data receiver based on GNURadio
 
 <!-- TOC -->
 * [About](#About)
 * [Requirements](#Requirements)
 * [Installation](#Installation)
-  * [Linux](#Linux)
-  * [Windows](#Windows)
 * [Usage](#Usage)
 * [Configure](#Configure)
   * [observer](#observer)
   * [tle](#tle)
   * [receivers](#receivers)
     * [sats](#sats)
       * [frequencies](#frequencies)
         * [modulations](#modulations)
         * [decoders](#decoders)
 * [Map Shapes](#Map-Shapes)
   * [shapes](#shapes)
   * [points](#points)
 <!-- TOC -->
 
-
-
 ### About
 This program is written to automate the process of receiving signals from
 various orbiting satellites on your SDR. The basis for digital signal
 processing is GNU Radio - a free software development toolkit that provides
 signal processing blocks to implement software-defined radios and
 signal-processing systems. [[wikipedia](https://en.wikipedia.org/wiki/GNU_Radio)]  
 For example, this program is perfect for receiving weather
 satellites like NOAA (image below).  
 If you have ideas or knowledge on how to improve this project, feel free to submit issues or pull requests.
 
-![](doc/NOAA-15_2023-05-11_03-30-41,734229_map.jpg "NOAA-15")
+![](doc/NOAA-19_2023-01-12_04-24-35,752471_map.jpg "NOAA-19")
 
 
 ### Requirements
 The program has only been tested on Linux. Work on Windows is not guaranteed!
 * Python>=3.10 (or lower, see below)
 * GNURadio>=3.10 (or lower if gr-soapy installed); GUI-modules is not required
 * librtlsdr (if you use RTL-SDR)
 
 ### Installation
-First [install gnuradio](https://wiki.gnuradio.org/index.php?title=InstallingGR)
-
-#### Linux
-  If you need a virtual environment (recommended), you need to create it
-  with the `--system-site-packages` option
-  ```
-  python3 -m venv --system-site-packages venv
-  source venv/bin/activate
-  pip install sats-receiver
-  ```
-
-#### Windows
-  After install `radioconda`, launch a terminal by running "Conda Prompt"
-  in the "radioconda" directory in the Start menu and type
-  ```
-  pip install sats-receiver
-  ```
+* if you need a virtual environment, you need to create it with the `--system-site-packages` option:  
+  `python3 -m venv --system-site-packages venv`  
+  `source venv/bin/activate`  
+* from source  
+  `git clone https://github.com/baskiton/sats-receiver.git`  
+  `cd sats-receiver`  
+  `pip install -r requirements.txt`  
+* from pip  
+  `pip install sats_receiver`  
 
 ### Usage
-* in Linux if a virtual environment has been created:  
-  `source venv/bin/activate`
-* in Windows launch "Conda Prompt" terminal
-
-`python -u -m sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
+`python3 -m sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
+`sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
 * `config` Config file path. See [Configure](#Configure)
 * `-h, --help` Help message
 * `--log LOG` Logging level, INFO default
-* `--sysu SYSU` System Usages debug info timeout in seconds, 1 hour default
+* `--sysu SYSU` System Usages info timeout in seconds, 1 hour default
 
-For example, simple command line to launch program:  
-`python -u -m sats_receiver /path/to/config.json`  
-You can copy the `default.json` config file from the root of the repository to a
-location of your choice
-
-Program home directory is `~/sats_receiver`  
-Logfile saved to program home directory (`~/sats_receiver/logs`)  
-Tle files stored to program home directory (`~/sats_receiver/tle`)  
+Program home directory is `~/sats_receiver`
+Logfile saved to program home directory (~/sats_receiver/logs)
+Tle files stored to program home directory (~/sats_receiver/tle)
 
 ### Configure
 The configuration file is in JSON format.  
-You can copy the `default.json` file from the root of the repository to a
+You can copy the default.json file from the root of the repository to a
 location of your choice and edit it.
 
 | Field     | Type            | Description                                                |
 |:----------|:----------------|:-----------------------------------------------------------|
 | observer  | Object          | Observer/receiver parameters (see [observer](#observer))   |
 | tle       | Object          | TLE data parameters (see [tle](#tle))                      |
 | receivers | Array of Object | List of receivers parameters (see [receivers](#receivers)) |
@@ -181,59 +155,42 @@
 | freq_correction | Boolean | _Optional._ Correction for basic frequency, Hz. `0` by default                    |
 | mode            | String  | _Optional._ Modulation option (see [modulations](#modulations)). `RAW` by default |
 | decode          | String  | _Optional._ Decoder option (see [decoders](#decoders)). `RAW` by default          |
 | qpsk_baudrate   | Number  | _Required only for **QPSK** mode._ QPSK Baudrate, bps                             |
 | qpsk_excess_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Excess bandwidth. `0.35` by default      |
 | qpsk_ntaps      | Integer | _Optional. Only for **QPSK** mode._ QPSK number of taps. `33` by default          |
 | qpsk_costas_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Costas bandwidth. `0.005` by default     |
-| sstv_wsr        | Number  | _Optional. Only for **SSTV** decoder._ SSTV work samplerate. `16000` by default   |
-| sstv_sync       | Number  | _Optional. Only for **SSTV** decoder._ SSTV syncing. `true` by default            |
 
 
 #### modulations
 * `RAW`
 * `AM`
 * `FM`
 * `WFM`
 * `WFM_STEREO`
 * `QUAD`
 * `QPSK`
 
 #### decoders
 * `RAW` Saved to 2-channel float32 WAV file with `bandwidth` sample rate
 * `RSTREAM` Raw Stream - binary int8. Suitable for further processing, for example, in SatDump
-* `APT` sats-receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
-* `SSTV` SSTV saved to PNG image with EXIF. Supported modes:
-  * `Robot24`
-  * `Robot36`
-  * `Robot72`
-  * `MartinM1`
-  * `MartinM2`
-  * `MartinM3`
-  * `MartinM4`
-  * `PD50`
-  * `PD90`
-  * `PD120`
-  * `PD160`
-  * `PD180`
-  * `PD240`
-  * `PD290`
+* `APT` sats_receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
 * ~~`LRPT`~~ Not implemented yet
 
 
 ### Map Shapes
 Map shapes config file `map_shapes.json` can be found at the root of this repository.
 Shapefiles can be downloaded from [Natural Earth](https://www.naturalearthdata.com/downloads/)
 
-| Field      | Type             | Description                                                                        |
-|:-----------|:-----------------|:-----------------------------------------------------------------------------------|
-| shapes     | Array of Array   | _Optional._ List of shapes data (see [shapes](#shapes))                            |
-| shapes_dir | String           | _Optional. Only when `shapes` specified._ Path to directory contains shapes file   |
-| points     | Object of Object | _Optional._ Additional points to draw on map (see [points](#points))               |
-| line_width | Number           | _Optional._ Overlay lines width, pixels. `1` by default                            |
+| Field      | Type             | Description                                                          |
+|:-----------|:-----------------|:---------------------------------------------------------------------|
+| shapes_dir | String           | Path to directory contains shapes file                               |
+| shapes     | Array of Array   | List of shapes data (see [shapes](#shapes))                          |
+| line_width | Number           | _Optional._ Overlay lines width, pixels. `1` by default              |
+| points     | Object of Object | _Optional._ Additional points to draw on map (see [points](#points)) |
 
 
 #### shapes
 Each shape contain:
 
 | Offset | Field     | Type                       | Description                                                                                                        |
 |:-------|:----------|:---------------------------|:-------------------------------------------------------------------------------------------------------------------|
```

### Comparing `sats_receiver-0.0.1/sats_receiver.egg-info/SOURCES.txt` & `sats_receiver-0.1.0/sats_receiver.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,9 @@
 sats_receiver.egg-info/requires.txt
 sats_receiver.egg-info/top_level.txt
 sats_receiver/gr_modules/__init__.py
 sats_receiver/gr_modules/decoders.py
 sats_receiver/gr_modules/demodulators.py
 sats_receiver/gr_modules/modules.py
 sats_receiver/gr_modules/receiver.py
-sats_receiver/gr_modules/epb/__init__.py
-sats_receiver/gr_modules/epb/sstv.py
 sats_receiver/systems/__init__.py
-sats_receiver/systems/apt.py
-sats_receiver/systems/sstv.py
-tests/__init__.py
-tests/test_async_signal.py
-tests/test_decoders.py
-tests/test_utils.py
+sats_receiver/systems/apt.py
```

