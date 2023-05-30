# Comparing `tmp/ilcdlib-0.3.0.tar.gz` & `tmp/ilcdlib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-0.3.0.tar", max compression
+gzip compressed data, was "ilcdlib-0.4.0.tar", max compression
```

## Comparing `ilcdlib-0.3.0.tar` & `ilcdlib-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0    11357 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/LICENSE
--rw-r--r--   0        0        0     4949 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/README.md
--rw-r--r--   0        0        0     3341 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    12504 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0     1334 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     1474 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     5329 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     6330 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     5749 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     4890 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3650 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3774 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0      837 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0     6967 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2023-05-29 13:06:56.643687 ilcdlib-0.3.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     2415 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     1152 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     1014 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     2832 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    17577 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0      837 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1900 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1894 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1732 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7086 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     4728 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1705 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1294 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1206 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     1712 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2382 2023-05-29 13:06:56.647687 ilcdlib-0.3.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 ilcdlib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4949 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/README.md
+-rw-r--r--   0        0        0     3341 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    12504 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0     1334 2023-05-30 11:22:19.974514 ilcdlib-0.4.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     1474 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     5369 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     7981 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     5749 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3650 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3774 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0     8220 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     2596 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     1329 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     1185 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3328 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    19409 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1900 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1899 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1212 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     1737 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7086 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     4728 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1705 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1206 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     1712 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2382 2023-05-30 11:22:19.978514 ilcdlib-0.4.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 ilcdlib-0.4.0/PKG-INFO
```

### Comparing `ilcdlib-0.3.0/LICENSE` & `ilcdlib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/README.md` & `ilcdlib-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/pyproject.toml` & `ilcdlib-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "0.3.0"
+version = "0.4.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
@@ -21,15 +21,15 @@
 
 [tool.poetry.scripts]
 ilcdtool = { callable = "ilcdlib:cli.entrypoint", extras = ["cli"] }
 
 [tool.poetry.dependencies]
 python = "^3.11"
 urllib3 = { version = ">=1.26.16,<2.0.0" }
-openepd = { version = ">=0.3.0,<1.0.0" }
+openepd = { version = ">=0.4.0,<1.0.0" }
 
 # Optional dependencies
 lxml = { version = "~=4.9.2", optional = true }
 cli-rack = { version = ">=1.0.6", optional = true }
 
 [tool.poetry.dev-dependencies]
 # Unit tests
@@ -57,15 +57,15 @@
 types-urllib3 = ">=1.26.2"
 
 [tool.poetry.extras]
 lxml = ["lxml"]
 cli = ["cli-rack"]
 
 [tool.commitizen]
-version = "0.3.0"
+version = "0.4.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/ilcdlib/__version__.py",
 ]
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/__init__.py` & `ilcdlib-0.4.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/__main__.py` & `ilcdlib-0.4.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/__version__.py` & `ilcdlib-0.4.0/src/ilcdlib/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.3.0"
+VERSION = "0.4.0"
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/cli.py` & `ilcdlib-0.4.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/common.py` & `ilcdlib-0.4.0/src/ilcdlib/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/const.py` & `ilcdlib-0.4.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-0.4.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/dto.py` & `ilcdlib-0.4.0/src/ilcdlib/dto.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-0.4.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/entity/contact.py` & `ilcdlib-0.4.0/src/ilcdlib/entity/contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 
     def to_openepd_org(self, lang: LangDef, base_url: str | None = None) -> Org:
         """Convert this data set to an OpenEPD org object."""
         open_epd_contact = Contact.construct(
             email=self.get_email(),
             phone=cleanup_phone(self.get_phone()),
             website=self.get_website(),
+            address=self.get_address(),
         )
         return Org.construct(
             name=self.get_name(lang),
             web_domain=domain_from_url(self.get_website()),
             contacts=open_epd_contact if open_epd_contact.has_values() else None,
             attachments=create_openepd_attachments(self.get_own_reference(), base_url),
         )
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/entity/flow.py` & `ilcdlib-0.4.0/src/ilcdlib/entity/flow.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,51 +19,59 @@
 #
 from dataclasses import dataclass
 from typing import Optional, Type
 
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader
 from ilcdlib.entity.material import MatMlReader
 from ilcdlib.entity.unit import IlcdUnitGroupReader
+from ilcdlib.mapping.properties import PropertiesUUIDMapper, default_properties_uuid_mapper
 from ilcdlib.type import LangDef
 from ilcdlib.utils import none_throws
 from ilcdlib.xml_parser import T_ET
 
 
 class IlcdFlowPropertyReader(IlcdXmlReader):
     """Read an ILCD Flow Property XML file."""
 
     def __init__(
         self,
         element: T_ET.Element,
         data_provider: BaseIlcdMediumSpecificReader,
         *,
         unit_group_reader_cls: Type[IlcdUnitGroupReader] = IlcdUnitGroupReader,
+        property_uuid_mapper: PropertiesUUIDMapper = default_properties_uuid_mapper,
     ):
         super().__init__(data_provider)
         self._entity = element
         self.unit_group_reader_cls = unit_group_reader_cls
+        self.property_uuid_mapper = property_uuid_mapper
 
     def get_uuid(self) -> str:
         """Get the UUID of the entity described by this data set."""
         return none_throws(
             self._get_text(self._entity, ("fp:flowPropertiesInformation", "fp:dataSetInformation", "common:UUID"))
         )
 
     def get_version(self) -> str | None:
         """Get the version of the entity described by this data set."""
         return self._get_text(
             self._entity,
             ("fp:flowPropertiesInformation", "fp:publicationAndOwnership", "common:dataSetVersion"),
         )
 
-    def get_name(self, lang: LangDef) -> str | None:
+    def get_name(self, lang: LangDef, use_mapper: bool = True) -> str | None:
         """Get the name of the entity described by this data set."""
-        return self._get_localized_text(
+        name = self._get_localized_text(
             self._entity, ("fp:flowPropertiesInformation", "fp:dataSetInformation", "common:name"), lang
         )
+        if use_mapper:
+            mapped_name = self.property_uuid_mapper.map(self.get_uuid(), name if name else "")
+            return mapped_name if mapped_name is not None else None
+        else:
+            return name
 
     def get_unit_group_reader(self) -> IlcdUnitGroupReader | None:
         """Get the reader for the unit group."""
         element = self._get_external_tree(
             self._entity,
             ("fp:flowPropertiesInformation", "fp:quantitativeReference", "fp:referenceToReferenceUnitGroup"),
         )
@@ -160,7 +168,34 @@
             if flow_prop_el is None:
                 return None
             return IlcdFlowPropertyDto(
                 dataset_reader=self.flow_property_reader_cls(flow_prop_el, self.data_provider),
                 mean_value=self._get_float(element, ("flow:meanValue",)),
             )
         return None
+
+    def get_flow_other_properties(self, include_ref_flow_prop: bool = False) -> list[IlcdFlowPropertyDto]:
+        """Get the reader for the other flow properties."""
+        reference_flow_property_id = self.get_ref_to_reference_flow_prop() if include_ref_flow_prop else None
+        flow_elements = self._get_all_els(
+            self._entity,
+            (
+                "flow:flowProperties",
+                "flow:flowProperty",
+            ),
+        )
+        result: list[IlcdFlowPropertyDto] = []
+        for e in flow_elements:
+            if reference_flow_property_id is not None and e.attrib["dataSetInternalID"] == str(
+                reference_flow_property_id
+            ):
+                continue
+            flow_prop_el = self._get_external_tree(e, ("flow:referenceToFlowPropertyDataSet",))
+            if flow_prop_el is None:
+                continue
+            result.append(
+                IlcdFlowPropertyDto(
+                    dataset_reader=self.flow_property_reader_cls(flow_prop_el, self.data_provider),
+                    mean_value=self._get_float(e, ("flow:meanValue",)),
+                )
+            )
+        return result
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-0.4.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/entity/material.py` & `ilcdlib-0.4.0/src/ilcdlib/entity/material.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,23 +95,33 @@
                 continue
             prop_meta = self.xml_parser.get_el(self._entity, f"mm:Metadata/mm:PropertyDetails[@id='{prop_ref}']")
             if prop_meta is None:
                 continue
             prop_name = self.xml_parser.get_el_text(prop_meta, "mm:Name")
             if prop_name is None:
                 continue
+            prop_name = prop_name.lower()
             units_obj = self.xml_parser.get_el(prop_meta, "mm:Units")
             if units_obj is None:
                 continue
-            unit = units_obj.attrib.get("name") if units_obj.attrib else None
+            unit = self.__map_unit_name(units_obj.attrib.get("name")) if units_obj.attrib else None
             result.properties[prop_name] = MatMlMaterialProperty(
                 value=prop_value, data_format=prop_format, unit=unit, internal_id=prop_ref  # type: ignore
             )
         return result
 
+    def __map_unit_name(self, unit_name: str | None) -> str | None:
+        if unit_name is None:
+            return None
+        match unit_name.strip():
+            case "-":
+                return None
+            case _:
+                return unit_name
+
     def __parse_prop_data(
         self, prop_data
     ) -> tuple[Literal["float", "integer", "string", "exponential", "mixed"], str | int | float | None]:
         prop_format = prop_data.attrib.get("format") if prop_data is not None else None
         prop_value_raw = prop_data.text if prop_data is not None else None
         match prop_format:
             case "float":
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-0.4.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/entity/unit.py` & `ilcdlib-0.4.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-0.4.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/epd/cli.py` & `ilcdlib-0.4.0/src/ilcdlib/epd/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -95,41 +95,68 @@
             required=False,
             default=False,
         )
         parser.add_argument(
             "doc",
             metavar="doc",
             type=str,
+            nargs="+",
             help="Reference to the input document. Can be a file path or URL "
             "depending on supported converter capabilities.",
         )
 
     def handle(self, args: argparse.Namespace):
         in_format: str = args.in_format
         out_format: str = args.out_format
-        doc_ref: str = args.doc
+        doc_refs: list[str] = args.doc
         lang: str | None = args.lang
         dialect: str | None = args.dialect
         save: bool = args.save
         extract_pdf: bool = args.extract_pdf
         if in_format.lower() != "ilcd+epd":
             CLI.fail(f"Input format {in_format} is not supported.", 1)
         if out_format.lower() != "openepd":
             CLI.fail(f"Output format {out_format} is not supported.", 1)
         if in_format.lower() == out_format.lower():
             CLI.fail(f"Input format {in_format} and output format {out_format} are the same.", 1)
         if extract_pdf and not save:
             CLI.fail("Extracting PDF requires saving the input document. Consider adding -s flag", 1)
-        # if not doc_ref.endswith(".zip"):
-        #     CLI.fail(f"Input document {doc_ref} is not a zip file.", 2)
         epd_reader_factory = EpdReaderFactory()
         if dialect is not None and not epd_reader_factory.is_dialect_supported(dialect):
             CLI.fail(f"Dialect {dialect} is not supported.", 3)
+        for doc in doc_refs:
+            self.process_single_doc(
+                doc,
+                epd_reader_factory,
+                dialect=dialect,
+                extract_pdf=extract_pdf,
+                in_format=in_format,
+                lang=lang,
+                out_format=out_format,
+                save=save,
+            )
+
+    def process_single_doc(
+        self,
+        doc_ref: str,
+        epd_reader_factory: EpdReaderFactory,
+        *,
+        dialect: str | None,
+        in_format: str,
+        out_format: str,
+        lang: str | None = None,
+        extract_pdf: bool = False,
+        save: bool = False,
+    ) -> None:
         CLI.print_info(f"Converting document {doc_ref} from {in_format} to {out_format}.")
-        reader_cls = epd_reader_factory.get_reader_class(dialect)
+        reader_cls, dialect = (
+            (epd_reader_factory.get_reader_class(dialect), dialect)
+            if dialect
+            else epd_reader_factory.autodiscover_by_url(doc_ref)
+        )
         CLI.print_info("Effective dialect: " + (dialect if dialect is not None else "Generic"))
         medium = Soda4LcaZipReader(doc_ref) if doc_ref.startswith("http") else ZipIlcdReader(Path(doc_ref))
         epd_reader = reader_cls(None, None, medium)
         supported_langs = epd_reader.get_supported_langs()
         if len(supported_langs) == 0:
             CLI.fail(f"Input document {doc_ref} Doesn't seem to be correct. No language information detected.", 4)
         prioritize_english = False
@@ -142,15 +169,16 @@
                 f"Supported languages are: {supported_langs}",
                 4,
             )
         lang_list = [lang, None]
         if prioritize_english:
             lang_list.insert(0, "en")
         CLI.print_info("Language priority: " + ",".join([x if x is not None else "any other" for x in lang_list]))
-        open_epd = epd_reader.to_openepd_epd(lang_list)
+        base_url = self.__extract_base_url(doc_ref)
+        open_epd = epd_reader.to_openepd_epd(lang_list, base_url=base_url)
         CLI.print_data(open_epd.json(indent=2, exclude_none=True, exclude_unset=True))
         if save:
             self.save_results(epd_reader, open_epd, extract_pdf=extract_pdf)
 
     def save_results(self, epd_reader: IlcdEpdReader, result: Epd, *, extract_pdf: bool = False):
         output_dir = Path(epd_reader.get_uuid())
         ensure_dir(output_dir)
@@ -160,7 +188,19 @@
             epd_reader.data_provider.save_to(output_dir / "ilcd_epd.zip")
         if extract_pdf:
             pdf_stream = epd_reader.get_epd_document_stream()
             if pdf_stream is not None:
                 with open(output_dir / "original.pdf", "wb") as f:
                     f.write(pdf_stream.read())
         CLI.print_info("Output saved to " + str(output_dir.absolute()))
+
+    def __extract_base_url(self, doc_ref: str) -> str | None:
+        if doc_ref.startswith("http"):
+            if "/datasetdetail/" in doc_ref:
+                return doc_ref.split("/datasetdetail/", 1)[0]
+            elif "/resource/" in doc_ref:
+                return doc_ref.split("/resource/", 1)[0]
+            elif "/showProcess.xhtml" in doc_ref:
+                return doc_ref.split("/showProcess.xhtml", 1)[0]
+            return None
+        else:
+            return None
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-0.4.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-0.4.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,19 @@
             try:
                 date_str = descr.split(self._TIME_REPR_DESC_DELIMITER)[0].strip().rsplit(" ", 1)[-1].strip()
                 return datetime.date.fromisoformat(date_str)
             except Exception:
                 pass
         return super().get_date_published()
 
+    @classmethod
+    def is_known_url(cls, url: str) -> bool:
+        """Return whether the URL recognized as a known Environdec URL."""
+        return "environdec" in url.lower()
+
     def __get_time_repr_description(self) -> str | None:
         return self._get_localized_text(
             self.epd_el_tree,
             (
                 "process:processInformation",
                 "process:time",
                 "common:timeRepresentativenessDescription",
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-0.4.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,7 +22,12 @@
 
 class IndataIlcdXmlEpdReader(IlcdEpdReader):
     """Reader for EPDs in the Indata specific ILCD XML format."""
 
     def post_init(self):
         """Configure Indata specific settings."""
         self.xml_parser.xml_ns["epd2019"] = "http://www.indata.network/EPD/2019"
+
+    @classmethod
+    def is_known_url(cls, url: str) -> bool:
+        """Return whether the URL recognized as a known Environdec URL."""
+        return "indata" in url.lower()
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-0.4.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 #
 from ilcdlib.epd.reader import IlcdEpdReader
 
 
 class OekobauDatIlcdXmlEpdReader(IlcdEpdReader):
     """Reader for EPDs in the Oekobau.DAT specific ILCD XML format."""
 
-    pass
+    @classmethod
+    def is_known_url(cls, url: str) -> bool:
+        """Return whether the URL recognized as a known Environdec URL."""
+        return "oekobaudat" in url.lower()
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/epd/factory.py` & `ilcdlib-0.4.0/src/ilcdlib/epd/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,7 +66,21 @@
         """
         if dialect is None:
             return self.DEFAULT_READER_CLASS
         dialect = dialect.lower()
         if dialect not in self.__DIALECTS:
             raise ValueError(f"Unknown dialect: {dialect}.")
         return self.__DIALECTS[dialect]
+
+    def autodiscover_by_url(self, url: str) -> tuple[Type[IlcdEpdReader], str]:
+        """
+        Return the reader class for the dialect.
+
+        If nothing recognized, return the default reader class.
+
+        @:return tuple of reader class and dialect name
+        """
+        if url.startswith("http"):
+            for name, cls in self.__DIALECTS.items():
+                if cls.is_known_url(url):
+                    return cls, name
+        return self.DEFAULT_READER_CLASS, "default"
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/epd/reader.py` & `ilcdlib-0.4.0/src/ilcdlib/epd/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
 from typing import IO, Sequence, Type
 
-from openepd.model.common import Amount
+from openepd.model.common import Amount, Measurement
 from openepd.model.epd import Epd
 from openepd.model.lcia import ImpactSet
 from openepd.model.specs import Specs
 
 from ilcdlib import const
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdEdpSupportReader
 from ilcdlib.const import IlcdDatasetType
@@ -293,14 +293,35 @@
         if product_flow_dto is None or product_flow_dto.flow_dataset_reader is None:
             return None
         material_reader = product_flow_dto.flow_dataset_reader.get_material_reader()
         if material_reader is None:
             return None
         return material_reader.get_material()
 
+    def get_product_flow_properties(self, include_ref_flow_prop: bool = False) -> dict[str, Measurement]:
+        """Return product flow properties other than reference property."""
+        exchange_dto = self.get_product_flow()
+        if exchange_dto is None:
+            return {}
+        reference_flow_properties = none_throws(exchange_dto.flow_dataset_reader).get_flow_other_properties(
+            include_ref_flow_prop
+        )
+        result = {}
+        for rfp in reference_flow_properties:
+            unit_group_reader = rfp.dataset_reader.get_unit_group_reader()
+            unit = unit_group_reader.get_reference_unit() if unit_group_reader is not None else None
+            if unit is None:
+                continue
+            amount = (exchange_dto.mean_value or 1.0) * (rfp.mean_value or 1.0) * unit.mean_value
+            prop_name = rfp.dataset_reader.get_name(["en", None])
+            if prop_name is None:
+                continue
+            result[prop_name.lower()] = Measurement(mean=amount, unit=unit.name)
+        return result
+
     def get_product_flow(self) -> IlcdExchangeDto | None:
         """Return the product flow (includes mean value and ilcd flow reader)."""
         ref_id = self.get_ref_to_product_flow_dataset()
         if ref_id is None:
             return None
         exchange_element = self._get_el(
             self.epd_el_tree,
@@ -366,35 +387,45 @@
                 result["IBU"] = " >> ".join([none_throws(x.name) for x in class_defs])
             if len(class_defs) > 0:
                 result[const.ILCD_IDENTIFICATION[0]] = (
                     (class_defs[-1].id or "") + " " + " / ".join([none_throws(x.name) for x in class_defs])
                 ).strip()
         return result
 
-    def to_openepd_epd(self, lang: LangDef, base_url: str | None = None) -> Epd:
+    def to_openepd_epd(self, lang: LangDef, base_url: str | None = None) -> Epd:  # NOSONAR
         """Return the EPD as OpenEPD object."""
         lang_code = lang if isinstance(lang, str) else None
         if isinstance(lang, Sequence):
             lang_code = lang[0] if len(lang) > 0 else None
         manufacturer_reader = self.get_manufacturer_reader()
-        manufacturer = manufacturer_reader.to_openepd_org(lang) if manufacturer_reader else None
+        manufacturer = manufacturer_reader.to_openepd_org(lang, base_url) if manufacturer_reader else None
         program_operator_reader = self.get_program_operator_reader()
-        program_operator = program_operator_reader.to_openepd_org(lang) if program_operator_reader else None
+        program_operator = program_operator_reader.to_openepd_org(lang, base_url) if program_operator_reader else None
         external_verifier_reader = self.get_external_verifier_reader()
-        external_verifier = external_verifier_reader.to_openepd_org(lang) if external_verifier_reader else None
+        external_verifier = (
+            external_verifier_reader.to_openepd_org(lang, base_url) if external_verifier_reader else None
+        )
         pcr_reader = self.get_pcr_reader()
-        pcr = pcr_reader.to_openepd_pcr(lang) if pcr_reader else None
+        pcr = pcr_reader.to_openepd_pcr(lang, base_url) if pcr_reader else None
         declared_unit = self.get_declared_unit()
         quantitative_props = self.get_quantitative_product_props_str(lang)
         product_name = self.get_product_name(lang)
         if product_name and quantitative_props:
             product_name += "; " + quantitative_props
         material_properties = self.get_material_properties()
+        other_product_props = self.get_product_flow_properties()
+        product_properties = {}
         if material_properties:
-            specs = Specs(ext=create_ext({n: v.to_unit_string() for n, v in material_properties.properties.items()}))
+            product_properties.update({n: v.to_unit_string() for n, v in material_properties.properties.items()})
+        if other_product_props:
+            product_properties.update(
+                {n: (str(v.mean) + " " + v.unit if v.unit else "").strip() for n, v in other_product_props.items()}
+            )
+        if product_properties:
+            specs = Specs(ext=create_ext(product_properties))
         else:
             specs = Specs()
         return Epd.construct(
             doctype="openEPD",
             language=lang_code,
             attachments=create_openepd_attachments(self.get_own_reference(), base_url),
             name=product_name,
@@ -407,7 +438,17 @@
             product_class=self._product_classes_to_openepd(self.get_product_classes()),
             third_party_verifier=external_verifier,
             pcr=pcr,
             declared_unit=declared_unit,
             impacts=self.get_lcia_results(),
             specs=specs,
         )
+
+    @classmethod
+    def is_known_url(cls, url: str) -> bool:
+        """
+        Return whether the URL recognized by this particular reader.
+
+        This method should be overriden by the dialect and return true if the input URL is know url for this dialect.
+        """
+
+        return False
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-0.4.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/mapping/common.py` & `ilcdlib-0.4.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-0.4.0/src/ilcdlib/mapping/impacts.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from ilcdlib.mapping.common import SimpleDataMapper
 
 
-class ImpactsUUIDToOpenIdMapper(SimpleDataMapper):
+class ImpactsUUIDToOpenIdMapper(SimpleDataMapper[str]):
     """Map ILCD UUIDs to openEPD impact names."""
 
     DATABASE = {
         "77e416eb-a363-4258-a04e-171d843a6460": "gwp",
         "6a37f984-a4b3-458a-a20a-64418c145fa2": "gwp",
         "5f635281-343e-44fb-83df-1971b155e6b6": "gwp-fossil",
         "2356e1ab-0185-4db5-86e5-16de51c7485c": "gwp-biogenic",
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/mapping/units.py` & `ilcdlib-0.4.0/src/ilcdlib/mapping/units.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from ilcdlib.mapping.common import SimpleDataMapper
 
 
-class UnitsUUIDMapper(SimpleDataMapper):
+class UnitsUUIDMapper(SimpleDataMapper[str]):
     """A data mapper that maps units ILCD UUIDs to their symbols."""
 
     DATABASE = {
         "c20a03d7-bd90-4569-bc94-66cfd364dfc8": "m2",
         # Impact units
         "93a60a57-a3c8-11da-a746-0800200c9a66": "MJ",
         "6ae2df01-888e-46c8-b17d-49fa3869b476": "m3AWARE",
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-0.4.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/medium/archive.py` & `ilcdlib-0.4.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-0.4.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/reference_data.py` & `ilcdlib-0.4.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-0.4.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-0.4.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-0.4.0/src/ilcdlib/sanitizing/phone.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import re
 
-PHONE_REGEX = re.compile(r"\+?[\d\s\-()]+", re.IGNORECASE)
+PHONE_REGEX = re.compile(r"[+\d\s\-()]+", re.IGNORECASE)
 
 
 def cleanup_phone(phone: str | None) -> str | None:
     """
     Try to perform cleanup of the given phone number.
 
     E.g. if the input is `Tel: +49 (0) 123 456 789 blah`, the output will be ``+49 (0) 123 456 789``.
     """
     if phone is None:
         return None
-    for m in PHONE_REGEX.findall(phone):
+    for m in sorted(PHONE_REGEX.findall(phone), key=lambda x: len(x), reverse=True):
         if len(m.strip()) > 0:
             return m.strip()
     return phone
```

### Comparing `ilcdlib-0.3.0/src/ilcdlib/type.py` & `ilcdlib-0.4.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/utils.py` & `ilcdlib-0.4.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/src/ilcdlib/xml_parser.py` & `ilcdlib-0.4.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.3.0/PKG-INFO` & `ilcdlib-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 0.3.0
+Version: 0.4.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: cli
 Provides-Extra: lxml
 Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml"
-Requires-Dist: openepd (>=0.3.0,<1.0.0)
+Requires-Dist: openepd (>=0.4.0,<1.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/cchangelabs/ilcdlib
 Description-Content-Type: text/markdown
 
 # ILCD Lib
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 0.3.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 0.4.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: support@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Provides-Extra: cli
 Provides-Extra: lxml Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml" Requires-Dist: openepd
-(>=0.3.0,<1.0.0) Requires-Dist: urllib3 (>=1.26.16,<2.0.0) Project-URL:
+(>=0.4.0,<1.0.0) Requires-Dist: urllib3 (>=1.26.16,<2.0.0) Project-URL:
 Repository, https://github.com/cchangelabs/ilcdlib Description-Content-Type:
 text/markdown # ILCD Lib
      [https://img.shields.io/pypi/l/ilcdlib?style=for-the-badge] [https://
      img.shields.io/pypi/pyversions/ilcdlib?style=for-the-badge] [https://
  img.shields.io/badge/Code%20Style-black-black?style=for-the-badge] [https://
   img.shields.io/pypi/v/ilcdlib?style=for-the-badge] [https://img.shields.io/
                      pypi/dm/ilcdlib?style=for-the-badge]
```

