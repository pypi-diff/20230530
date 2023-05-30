# Comparing `tmp/spei_python-0.5.37.tar.gz` & `tmp/spei_python-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spei_python-0.5.37.tar", max compression
+gzip compressed data, was "spei_python-0.7.0.tar", max compression
```

## Comparing `spei_python-0.5.37.tar` & `spei_python-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.5.37/README.md
--rw-r--r--   0        0        0      859 2023-05-11 17:12:03.608832 spei_python-0.5.37/pyproject.toml
--rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.5.37/spei/__init__.py
--rw-r--r--   0        0        0     2739 2023-05-11 17:06:18.833865 spei_python-0.5.37/spei/client.py
--rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.5.37/spei/resources/__init__.py
--rw-r--r--   0        0        0     3962 2023-03-13 22:05:56.750212 spei_python-0.5.37/spei/resources/ordenes.py
--rw-r--r--   0        0        0     1703 2023-03-13 21:54:51.240999 spei_python-0.5.37/spei/types.py
--rw-r--r--   0        0        0     2289 2023-03-13 22:05:00.658624 spei_python-0.5.37/spei/utils.py
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 spei_python-0.5.37/PKG-INFO
+-rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.7.0/README.md
+-rw-r--r--   0        0        0      856 2023-05-30 01:04:48.825748 spei_python-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.7.0/spei/__init__.py
+-rw-r--r--   0        0        0     2733 2023-05-30 00:46:55.019167 spei_python-0.7.0/spei/client.py
+-rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.7.0/spei/resources/__init__.py
+-rw-r--r--   0        0        0     4559 2023-05-30 00:59:08.634556 spei_python-0.7.0/spei/resources/ordenes.py
+-rw-r--r--   0        0        0     1791 2023-05-30 00:27:21.381550 spei_python-0.7.0/spei/types.py
+-rw-r--r--   0        0        0     2272 2023-05-30 01:00:59.645173 spei_python-0.7.0/spei/utils.py
+-rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 spei_python-0.7.0/setup.py
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 spei_python-0.7.0/PKG-INFO
```

### Comparing `spei_python-0.5.37/README.md` & `spei_python-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.37/pyproject.toml` & `spei_python-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spei-python"
-version = "0.5.37"
+version = "0.7.0"
 description = ""
 authors = ["gonz <gonzasestopal@gmail.com>"]
 readme = "README.md"
 packages = [{include = "spei"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
@@ -27,14 +27,13 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.37"
+version = "0.7.0"
 tag_format = "v$version"
 bump_message = "bump: Semantic Release Bot: Release Version: $new_version 🤖🚀 [skip ci]"
 version_files = [
     "pyproject.toml:version",
 ]
-
```

### Comparing `spei_python-0.5.37/spei/client.py` & `spei_python-0.7.0/spei/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def registra_orden(self, orden_data, orden_cls=Orden, respuesta_cls=Respuesta):
         checksum = self.generate_checksum(orden_data)
         orden = orden_cls(op_firma_dig=checksum, **orden_data)
         soap_request = self._build_request(orden.build_xml())
         response = self.session.post(data=etree.tostring(soap_request), url=self.host)
         response.raise_for_status()
-        respuesta = respuesta_cls.parse_respuesta(response.text)
+        respuesta = respuesta_cls.parse_xml(response.text)
         logger.info(respuesta)
         return respuesta
 
     def _build_request(self, mensaje_xml):
         namespaces_uris = {
             'soapenv': SOAP_NS,
             'prax': PRAXIS_NS,
```

### Comparing `spei_python-0.5.37/spei/resources/ordenes.py` & `spei_python-0.7.0/spei/resources/ordenes.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         raise ValueError('must be in YYYYMMDD format')
 
     def build_xml(self):
         mensaje = etree.Element('mensaje', categoria=self.categoria)
         orden_pago = etree.SubElement(mensaje, 'ordenpago')
 
-        for element, value in self.dict(exclude_none=True, exclude={'categoria', 'op_ord_clave'}).items():  # noqa: WPS110, E501
+        for element, value in self.dict(exclude_none=True, exclude={'categoria', 'op_ord_clave'}).items():  # noqa: WPS110, WPS221, E501
             if element in self.__fields__:
                 if element == 'op_firma_dig':
                     subelement = etree.SubElement(orden_pago, 'opFirmaDig')
                     subelement.text = str(value)
                     continue
                 upper_camel_case_element = to_upper_camel_case(element)
                 subelement = etree.SubElement(orden_pago, upper_camel_case_element)
@@ -80,15 +80,15 @@
 
     @classmethod
     def parse_xml(cls, orden_xml):
         orden = etree.fromstring(orden_xml)  # noqa: S320
         body = orden.find('{http://schemas.xmlsoap.org/soap/envelope/}Body')
         orden_pago = body.find('{http://www.praxis.com.mx/}ordenpago')
 
-        mensaje_xml = etree.fromstring(orden_pago.text)
+        mensaje_xml = etree.fromstring(orden_pago.text)  # noqa: S320
         orden = mensaje_xml.find('ordenpago')
 
         orden_data = {
             'categoria': mensaje_xml.attrib['categoria'],
         }
 
         for element in orden.getchildren():
@@ -96,30 +96,44 @@
             if tag in cls.__fields__:
                 orden_data[tag] = element.text
 
         return cls(**orden_data)
 
 
 class Respuesta(BaseModel):
+    categoria: types.CategoriaOrdenPago
+
     id: str
     fecha_oper: int
     err_codigo: int
     err_descripcion: str
 
-    @classmethod
-    def parse_respuesta(cls, respuesta_xml):
-        response = None
+    def build_xml(self):
+        mensaje = etree.Element('mensaje', categoria=self.categoria)
+        orden_pago = etree.SubElement(mensaje, 'respuesta')
 
-        mensaje = etree.fromstring(respuesta_xml)  # noqa: S320
-        for element in mensaje.getchildren():
+        for element, value in self.dict().items():  # noqa: WPS110
+            if element in self.__fields__:
+                upper_camel_case_element = to_upper_camel_case(element)
+                subelement = etree.SubElement(orden_pago, upper_camel_case_element)
+                subelement.text = str(value)
+
+        return mensaje
+
+    @classmethod
+    def parse_xml(cls, respuesta_xml):
+        respuesta = etree.fromstring(respuesta_xml)  # noqa: S320
+        for element in respuesta.getchildren():
             response = element.find('{http://www.praxis.com.mx/}respuesta')
 
-        response = etree.fromstring(bytes(response.text, encoding='cp850'))  # noqa: S320, E501
+        mensaje_xml = etree.fromstring(bytes(response.text, encoding='cp850'))   # noqa: S320, E501
+        respuesta = mensaje_xml.find('respuesta')
 
-        respuesta = response.find('respuesta')
+        respuesta_data = {
+            'categoria': mensaje_xml.attrib['categoria'],
+        }
 
-        respuesta_data = {}
-        for element in respuesta.getchildren():  # noqa: WPS440
-            tag = to_snake_case(element.tag)
-            respuesta_data[tag] = element.text
+        for sub_element in respuesta.getchildren():
+            tag = to_snake_case(sub_element.tag)
+            respuesta_data[tag] = sub_element.text
 
         return cls(**respuesta_data)
```

### Comparing `spei_python-0.5.37/spei/types.py` & `spei_python-0.7.0/spei/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 class CategoriaOrdenPago(str, Enum):
     cargar_odp = 'CARGAR_ODP'
     cargar_odp_respuesta = 'CARGAR_ODP_RESPUESTA'
     odps_liquidadas_cargos = 'ODPS_LIQUIDADAS_CARGOS'
     odps_liquidadas_cargos_respuesta = 'ODPS_LIQUIDADAS_CARGOS_RESPUESTA'
     odps_liquidadas_abonos = 'ODPS_LIQUIDADAS_ABONOS'
-    odps_liquidadas_abonos_respuesta = 'ODPS_LIQUIDADAS_ABONOS'
+    odps_liquidadas_abonos_respuesta = 'ODPS_LIQUIDADAS_ABONOS_RESPUESTA'
     odps_canceladas_local = 'ODPS_CANCELADAS_LOCAL'
     odps_canceladas_local_respuesta = 'ODPS_CANCELADAS_LOCAL_RESPUESTA'
     odps_canceladas_x_banxico = 'ODPS_CANCELADAS_X_BANXICO'
     odps_canceladas_x_banxico_respuesta = 'ODPS_CANCELADAS_X_BANXICO_RESPUESTA'
 
 
 class EstadoOrdenPago(str, Enum):
@@ -64,7 +64,12 @@
     cei = '7'
     hsbc = '8'
     htvf = '9'
     dtp = '10'
     ifai = '13'
     swift = '17'
     nomina = '18'
+
+
+class CodigoError(str, Enum):
+    exitoso = 0
+    categoria_incorrecta = -1
```

### Comparing `spei_python-0.5.37/spei/utils.py` & `spei_python-0.7.0/spei/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 def to_upper_camel_case(string):
     temp = string.split('_')
     new_string = [ele.title() for ele in temp]
     return ''.join(new_string)
 
 
 def to_snake_case(string):
-    return re.sub(r'(.)([A-Z0-9])', r'\1_\2', str(string)).lower()  # noqa: WPS360
+    return re.sub('(.)([A-Z0-9])', r'\1_\2', str(string)).lower()
```

### Comparing `spei_python-0.5.37/PKG-INFO` & `spei_python-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei-python
-Version: 0.5.37
+Version: 0.7.0
 Summary: 
 Author: gonz
 Author-email: gonzasestopal@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

