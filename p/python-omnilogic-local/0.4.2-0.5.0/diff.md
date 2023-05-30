# Comparing `tmp/python_omnilogic_local-0.4.2.tar.gz` & `tmp/python_omnilogic_local-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.4.2.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.5.0.tar", max compression
```

## Comparing `python_omnilogic_local-0.4.2.tar` & `python_omnilogic_local-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1696 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/README.md
--rw-r--r--   0        0        0        0 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    21535 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3921 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     7871 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9619 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     9040 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6304 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-29 20:55:49.086857 python_omnilogic_local-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/__init__.py
+-rw-r--r--   0        0        0    21453 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3921 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     8079 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9803 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0    10157 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6470 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-30 19:13:13.639070 python_omnilogic_local-0.5.0/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-30 19:13:14.531076 python_omnilogic_local-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.5.0/PKG-INFO
```

### Comparing `python_omnilogic_local-0.4.2/README.md` & `python_omnilogic_local-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.2/pyomnilogic_local/api.py` & `python_omnilogic_local-0.5.0/pyomnilogic_local/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,17 +50,17 @@
         """
         loop = asyncio.get_running_loop()
         transport, protocol = await loop.create_datagram_endpoint(OmniLogicProtocol, remote_addr=(self.controller_ip, self.controller_port))
 
         resp: str | None = None
         try:
             if need_response:
-                resp = await asyncio.wait_for(protocol.send_and_receive(message_type, message), self.response_timeout)
+                resp = await protocol.send_and_receive(message_type, message)
             else:
-                await asyncio.wait_for(protocol.send_message(message_type, message), self.response_timeout)
+                await protocol.send_message(message_type, message)
         finally:
             transport.close()
 
         return resp
 
     async def async_get_alarm_list(self) -> str:
         """Retrieve a list of alarms from the Omni.
```

### Comparing `python_omnilogic_local-0.4.2/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.5.0/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.2/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.5.0/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.2/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.5.0/pyomnilogic_local/models/mspconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import logging
 import sys
 from typing import Any, Literal, TypeAlias
 
+from ..types import OmniParsingException
+
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, ValidationError
 from xmltodict import parse as xml_parse
 
 from ..types import (
     BodyOfWaterType,
     ColorLogicLightType,
     FilterType,
     HeaterType,
@@ -205,8 +207,11 @@
                 OmniType.GROUPS,
                 OmniType.HEATER_EQUIP,
                 OmniType.RELAY,
                 OmniType.SENSOR,
                 OmniType.SCHE,
             ),
         )
-        return MSPConfig.parse_obj(data["MSPConfig"])
+        try:
+            return MSPConfig.parse_obj(data["MSPConfig"])
+        except ValidationError as exc:
+            raise OmniParsingException(f"Failed to parse MSP Configuration: {exc}") from exc
```

### Comparing `python_omnilogic_local-0.4.2/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.5.0/pyomnilogic_local/models/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
 from typing import Any, SupportsInt, TypeAlias, TypeVar, cast, overload
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, ValidationError
 from xmltodict import parse as xml_parse
 
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
+    OmniParsingException,
     OmniType,
     PumpState,
     RelayState,
     ValveActuatorState,
 )
 
 # Example telemetry XML data:
@@ -222,15 +223,18 @@
                 OmniType.GROUP,
                 OmniType.HEATER,
                 OmniType.PUMP,
                 OmniType.RELAY,
                 OmniType.VALVE_ACTUATOR,
             ),
         )
-        return Telemetry.parse_obj(data["STATUS"])
+        try:
+            return Telemetry.parse_obj(data["STATUS"])
+        except ValidationError as exc:
+            raise OmniParsingException(f"Failed to parse Telemetry: {exc}") from exc
 
     def get_telem_by_systemid(self, system_id: int) -> TelemetryType | None:
         for field_name, value in self:
             if field_name == "version" or value is None:
                 continue
             if isinstance(value, list):
                 for model in value:
```

### Comparing `python_omnilogic_local-0.4.2/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.5.0/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.2/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.5.0/pyomnilogic_local/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from typing import Any, cast
 import xml.etree.ElementTree as ET
 import zlib
 
 from typing_extensions import Self
 
 from .models.leadmessage import LeadMessage
-from .types import ClientType, MessageType
+from .types import ClientType, MessageType, OmniTimeoutException
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class OmniLogicMessage:
     header_format = "!LQ4sLBBBB"
     id: int
     type: MessageType
     payload: bytes
     client_type: ClientType = ClientType.SIMPLE
     version: str = "1.19"
     timestamp: int | None
-    reserved_1: int
-    compressed: int
-    reserved_2: int
+    reserved_1: int = 0
+    compressed: int = 0
+    reserved_2: int = 0
 
     def __init__(self, msg_id: int, msg_type: MessageType, payload: str | None = None, version: str = "1.19") -> None:
         self.id = msg_id
         self.type = msg_type
         # If we are speaking the XML API, it seems like we need client_type 0, otherwise we need client_type 1
         self.client_type = ClientType.XML if payload is not None else ClientType.SIMPLE
         # The Hayward API terminates it's messages with a null character
@@ -48,14 +48,19 @@
             self.client_type.value,  # Client type
             0,  # reserved
             0,  # compressed
             0,  # reserved
         )
         return header + self.payload
 
+    def __repr__(self) -> str:
+        if self.compressed or self.type is MessageType.MSP_BLOCKMESSAGE:
+            return f"ID: {self.id}, Type: {self.type}, Compressed: {self.compressed}"
+        return f"ID: {self.id}, Type: {self.type}, Compressed: {self.compressed}, Body: {self.payload[:-1].decode('utf-8')}"
+
     @classmethod
     def from_bytes(cls, data: bytes) -> Self:
         # split the header and data
         header = data[0:24]
         rdata: bytes = data[24:]
 
         msg_id, tstamp, vers, msg_type, client_type, res1, compressed, res2 = struct.unpack(cls.header_format, header)
@@ -69,31 +74,32 @@
         message.payload = rdata
 
         return message
 
 
 class OmniLogicProtocol(asyncio.DatagramProtocol):
     transport: asyncio.DatagramTransport
+    # The omni will re-transmit a packet every 2 seconds if it does not receive an ACK.  We pad that just a touch to be safe
+    _omni_retransmit_time = 2.1
+    # The omni will re-transmit 5 times (a total of 6 attempts including the initial) if it does not receive an ACK
+    _omni_retransmit_count = 5
 
     def __init__(self) -> None:
         self.data_queue = asyncio.Queue[OmniLogicMessage]()
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         self.transport = cast(asyncio.DatagramTransport, transport)
 
     def connection_lost(self, exc: Exception | None) -> None:
         if exc:
             raise exc
 
     def datagram_received(self, data: bytes, addr: tuple[str | Any, int]) -> None:
         message = OmniLogicMessage.from_bytes(data)
-        if message.compressed:
-            _LOGGER.debug("Received compressed message ID: %s, Type: %s", message.id, message.type)
-        else:
-            _LOGGER.debug("Received Message ID: %s, Type: %s", message.id, message.type)
+        _LOGGER.debug("Received Message %s", str(message))
         self.data_queue.put_nowait(message)
 
     def error_received(self, exc: Exception) -> None:
         raise exc
 
     async def _wait_for_ack(self, ack_id: int) -> None:
         message = await self.data_queue.get()
@@ -111,44 +117,46 @@
                 _LOGGER.debug("Omni has sent a new message, continuing on with the communication")
                 await self.data_queue.put(message)
                 break
             # In theory, we should never get to this spot, but it's mostly here to cause the code to wait forever so that asyncio will
             # eventually time out waiting for it, that way we can deal with the dropped packets
             message = await self.data_queue.get()
 
-    async def _ensure_sent(self, message: OmniLogicMessage) -> None:
-        delivered = False
-        while not delivered:
+    async def _ensure_sent(self, message: OmniLogicMessage, max_attempts: int = 5) -> None:
+        for attempt in range(0, max_attempts):
             self.transport.sendto(bytes(message))
 
             # If the message that we just sent is an ACK, we do not need to wait to receive an ACK, we are done
             if message.type in [MessageType.XML_ACK, MessageType.ACK]:
                 return
 
             # Wait for a bit to either receive an ACK for our message, otherwise, we retry delivery
             try:
                 await asyncio.wait_for(self._wait_for_ack(message.id), 0.25)
-                delivered = True
-            except TimeoutError:
-                _LOGGER.debug("ACK not received, re-attempting delivery")
+                return
+            except TimeoutError as exc:
+                if attempt < 4:
+                    _LOGGER.debug("ACK not received, re-attempting delivery")
+                else:
+                    raise OmniTimeoutException("Failed to receive acknowledgement of command, max retries exceeded") from exc
 
     async def send_and_receive(self, msg_type: MessageType, payload: str | None, msg_id: int | None = None) -> str:
         await self.send_message(msg_type, payload, msg_id)
         return await self._receive_file()
 
     # Send a message that you do NOT need a response to
     async def send_message(self, msg_type: MessageType, payload: str | None, msg_id: int | None = None) -> None:
         # If we aren't sending a specific msg_id, lets randomize it
         if not msg_id:
             msg_id = random.randrange(2**32)
 
-        _LOGGER.debug("Sending Message ID: %s, Message Type: %s, Request Body: %s", msg_id, msg_type.name, payload)
-
         message = OmniLogicMessage(msg_id, msg_type, payload)
 
+        _LOGGER.debug("Sending Message %s", str(message))
+
         await self._ensure_sent(message)
 
     async def _send_ack(self, msg_id: int) -> None:
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "Ack"
 
@@ -166,25 +174,35 @@
 
         await self._send_ack(message.id)
 
         # If the response is too large, the controller will send a LeadMessage indicating how many follow-up messages will be sent
         if message.type == MessageType.MSP_LEADMESSAGE:
             leadmsg = LeadMessage.from_orm(ET.fromstring(message.payload[:-1]))
 
+            _LOGGER.debug("Will receive %s blockmessages", leadmsg.msg_block_count)
+
             # Wait for the block data data
             retval: bytes = b""
             # If we received a LeadMessage, continue to receive messages until we have all of our data
             # Fragments of data may arrive out of order, so we store them in a buffer as they arrive and sort them after
             data_fragments: dict[int, bytes] = {}
             while len(data_fragments) < leadmsg.msg_block_count:
-                resp = await self.data_queue.get()
+                # We need to wait long enough for the Omni to get through all of it's retries before we bail out.
+                try:
+                    resp = await asyncio.wait_for(self.data_queue.get(), self._omni_retransmit_time * self._omni_retransmit_count)
+                except TimeoutError as exc:
+                    raise OmniTimeoutException from exc
+
                 # We only want to collect blockmessages here
                 if resp.type is not MessageType.MSP_BLOCKMESSAGE:
+                    _LOGGER.debug("Received a message other than a blockmessage: %s", resp.type)
                     continue
+
                 await self._send_ack(resp.id)
+
                 # remove an 8 byte header to get to the payload data
                 data_fragments[resp.id] = resp.payload[8:]
 
             # Reassemble the fragmets in order
             for _, data in sorted(data_fragments.items()):
                 retval += data
```

### Comparing `python_omnilogic_local-0.4.2/pyomnilogic_local/types.py` & `python_omnilogic_local-0.5.0/pyomnilogic_local/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -296,7 +296,19 @@
     NO_UNITS = "UNITS_NO_UNITS"
     ACTIVE_INACTIVE = "UNITS_ACTIVE_INACTIVE"
 
 
 class ValveActuatorState(PrettyEnum):
     OFF = 0
     ON = 1
+
+
+class OmniLogicException(Exception):
+    pass
+
+
+class OmniTimeoutException(OmniLogicException):
+    pass
+
+
+class OmniParsingException(OmniLogicException):
+    pass
```

### Comparing `python_omnilogic_local-0.4.2/pyproject.toml` & `python_omnilogic_local-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.4.2"
+version = "0.5.0"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.4.2/PKG-INFO` & `python_omnilogic_local-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.4.2
+Version: 0.5.0
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
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.4.2 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.5.0 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

