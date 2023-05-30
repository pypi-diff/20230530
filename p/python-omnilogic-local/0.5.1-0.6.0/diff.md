# Comparing `tmp/python_omnilogic_local-0.5.1.tar.gz` & `tmp/python_omnilogic_local-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.5.1.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.6.0.tar", max compression
```

## Comparing `python_omnilogic_local-0.5.1.tar` & `python_omnilogic_local-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1696 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/__init__.py
--rw-r--r--   0        0        0    21453 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3921 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     8079 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9803 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0    10166 2023-05-30 19:43:26.954636 python_omnilogic_local-0.5.1/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6470 2023-05-30 19:43:26.958636 python_omnilogic_local-0.5.1/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-30 19:43:26.958636 python_omnilogic_local-0.5.1/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-30 19:43:27.826640 python_omnilogic_local-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/__init__.py
+-rw-r--r--   0        0        0    21453 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3921 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0      164 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     8352 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9962 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0    10189 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6325 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-30 20:29:07.371425 python_omnilogic_local-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.6.0/PKG-INFO
```

### Comparing `python_omnilogic_local-0.5.1/README.md` & `python_omnilogic_local-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.5.1/pyomnilogic_local/api.py` & `python_omnilogic_local-0.6.0/pyomnilogic_local/api.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.5.1/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.6.0/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.5.1/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.6.0/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.5.1/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.6.0/pyomnilogic_local/models/mspconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
 import logging
 import sys
 from typing import Any, Literal, TypeAlias
 
-from ..types import OmniParsingException
-
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
-
 from pydantic import BaseModel, Field, ValidationError
 from xmltodict import parse as xml_parse
 
+from ..exceptions import OmniParsingException
 from ..types import (
     BodyOfWaterType,
     ColorLogicLightType,
+    ColorLogicShow,
     FilterType,
     HeaterType,
     OmniType,
     PumpFunction,
     PumpType,
     RelayFunction,
     RelayType,
@@ -139,14 +138,19 @@
         self.heater_equipment = [MSPHeaterEquip.parse_obj(equip) for equip in heater_equip_data[OmniType.HEATER_EQUIP]]
 
 
 class MSPColorLogicLight(OmniBase):
     omni_type: OmniType = OmniType.CL_LIGHT
     type: ColorLogicLightType | str = Field(alias="Type")
     v2_active: Literal["yes", "no"] | None = Field(alias="V2-Active")
+    effects: list[ColorLogicShow] | None
+
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+        self.effects = list(ColorLogicShow) if self.v2_active == "yes" else [show for show in ColorLogicShow if show.value <= 16]
 
 
 class MSPBoW(OmniBase):
     _sub_devices = {"filter", "relay", "heater", "sensor", "colorlogic_light"}
 
     omni_type: OmniType = OmniType.BOW
     type: BodyOfWaterType | str = Field(alias="Type")
```

### Comparing `python_omnilogic_local-0.5.1/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.6.0/pyomnilogic_local/models/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from typing import Any, SupportsInt, TypeAlias, TypeVar, cast, overload
 
 from pydantic import BaseModel, Field, ValidationError
 from xmltodict import parse as xml_parse
 
+from ..exceptions import OmniParsingException
 from ..types import (
     BackyardState,
     ChlorinatorOperatingMode,
     ColorLogicBrightness,
     ColorLogicPowerState,
     ColorLogicShow,
     ColorLogicSpeed,
     FilterState,
     FilterValvePosition,
     FilterWhyOn,
     HeaterMode,
     HeaterState,
-    OmniParsingException,
     OmniType,
     PumpState,
     RelayState,
     ValveActuatorState,
 )
 
 # Example telemetry XML data:
@@ -43,16 +43,17 @@
 
 class TelemetryBackyard(BaseModel):
     omni_type: OmniType = OmniType.BACKYARD
     system_id: int = Field(alias="@systemId")
     status_version: int = Field(alias="@statusVersion")
     air_temp: int = Field(alias="@airTemp")
     state: BackyardState | int = Field(alias="@state")
-    config_checksum: int = Field(alias="@ConfigChksum")
-    msp_version: str = Field(alias="@mspVersion")
+    # The below two fields are only available for telemetry with a status_version >= 11
+    config_checksum: int | None = Field(alias="@ConfigChksum")
+    msp_version: str | None = Field(alias="@mspVersion")
 
 
 class TelemetryBoW(BaseModel):
     omni_type: OmniType = OmniType.BOW
     system_id: int = Field(alias="@systemId")
     water_temp: int = Field(alias="@waterTemp")
     flow: int = Field(alias="@flow")
@@ -111,15 +112,15 @@
     maintain_for: int = Field(alias="@maintainFor")
 
 
 class TelemetryPump(BaseModel):
     omni_type: OmniType = OmniType.PUMP
     system_id: int = Field(alias="@systemId")
     state: PumpState | int = Field(alias="@pumpState")
-    speed: int = Field(alias="@pummpSpeed")
+    speed: int = Field(alias="@pumpSpeed")
     last_speed: int = Field(alias="@lastSpeed")
     why_on: int = Field(alias="@whyOn")
 
 
 class TelemetryRelay(BaseModel):
     omni_type: OmniType = OmniType.RELAY
     system_id: int = Field(alias="@systemId")
@@ -221,14 +222,15 @@
                 OmniType.CL_LIGHT,
                 OmniType.FILTER,
                 OmniType.GROUP,
                 OmniType.HEATER,
                 OmniType.PUMP,
                 OmniType.RELAY,
                 OmniType.VALVE_ACTUATOR,
+                OmniType.VIRT_HEATER,
             ),
         )
         try:
             return Telemetry.parse_obj(data["STATUS"])
         except ValidationError as exc:
             raise OmniParsingException(f"Failed to parse Telemetry: {exc}") from exc
```

### Comparing `python_omnilogic_local-0.5.1/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.6.0/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.5.1/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.6.0/pyomnilogic_local/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import time
 from typing import Any, cast
 import xml.etree.ElementTree as ET
 import zlib
 
 from typing_extensions import Self
 
+from .exceptions import OmniTimeoutException
 from .models.leadmessage import LeadMessage
-from .types import ClientType, MessageType, OmniTimeoutException
+from .types import ClientType, MessageType
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class OmniLogicMessage:
     header_format = "!LQ4sLBBBB"
     id: int
```

### Comparing `python_omnilogic_local-0.5.1/pyomnilogic_local/types.py` & `python_omnilogic_local-0.6.0/pyomnilogic_local/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     SANGRIA = 10
     TWILIGHT = 11
     TRANQUILITY = 12
     GEMSTONE = 13
     USA = 14
     MARDI_GRAS = 15
     COOL_CABARET = 16
-    #### THESE SHOW IN THE APP AFTER SETTING, BUT MAY NOT MATCH ALL LIGHTS
+    #### The below options only work on lights that support OmniDirect / V2-Active in MSPConfig
     YELLOW = 17
     ORANGE = 18
     GOLD = 19
     MINT = 20
     TEAL = 21
     BURNT_ORANGE = 22
     PURE_WHITE = 23
@@ -296,19 +296,7 @@
     NO_UNITS = "UNITS_NO_UNITS"
     ACTIVE_INACTIVE = "UNITS_ACTIVE_INACTIVE"
 
 
 class ValveActuatorState(PrettyEnum):
     OFF = 0
     ON = 1
-
-
-class OmniLogicException(Exception):
-    pass
-
-
-class OmniTimeoutException(OmniLogicException):
-    pass
-
-
-class OmniParsingException(OmniLogicException):
-    pass
```

### Comparing `python_omnilogic_local-0.5.1/pyproject.toml` & `python_omnilogic_local-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.5.1"
+version = "0.6.0"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.5.1/PKG-INFO` & `python_omnilogic_local-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.5.1
+Version: 0.6.0
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.5.1 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.6.0 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

