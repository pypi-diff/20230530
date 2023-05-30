# Comparing `tmp/debloat-1.3.2.2.tar.gz` & `tmp/debloat-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.3.2.2.tar", last modified: Mon May  8 11:40:06 2023, max compression
+gzip compressed data, was "debloat-1.4.0.tar", last modified: Tue May 30 12:17:38 2023, max compression
```

## Comparing `debloat-1.3.2.2.tar` & `debloat-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 11:40:06.836589 debloat-1.3.2.2/
--rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.3.2.2/LICENSE
--rw-rw-rw-   0        0        0     7407 2023-05-08 11:40:06.836589 debloat-1.3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     6851 2023-04-19 22:52:19.000000 debloat-1.3.2.2/README.md
--rw-rw-rw-   0        0        0      790 2023-05-08 11:36:50.000000 debloat-1.3.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      166 2023-05-08 11:40:06.838089 debloat-1.3.2.2/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.3.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:40:06.791591 debloat-1.3.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 11:40:06.808590 debloat-1.3.2.2/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-04-20 03:26:52.000000 debloat-1.3.2.2/src/debloat/__init__.py
--rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.3.2.2/src/debloat/auxiliary.py
--rw-rw-rw-   0        0        0     3835 2023-04-20 03:29:34.000000 debloat-1.3.2.2/src/debloat/gui.py
--rw-rw-rw-   0        0        0     1564 2023-05-05 02:45:32.000000 debloat-1.3.2.2/src/debloat/main.py
--rw-rw-rw-   0        0        0    19515 2023-05-08 11:29:58.000000 debloat-1.3.2.2/src/debloat/processor.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:40:06.835589 debloat-1.3.2.2/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     7407 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 11:40:06.000000 debloat-1.3.2.2/src/debloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.258473 debloat-1.4.0/
+-rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     7405 2023-05-30 12:17:38.258973 debloat-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6851 2023-04-19 22:52:19.000000 debloat-1.4.0/README.md
+-rw-rw-rw-   0        0        0      788 2023-05-30 12:15:47.000000 debloat-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      166 2023-05-30 12:17:38.264474 debloat-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.199962 debloat-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.219466 debloat-1.4.0/src/debloat/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:13:11.000000 debloat-1.4.0/src/debloat/__init__.py
+-rw-rw-rw-   0        0        0     1102 2023-05-09 12:20:28.000000 debloat-1.4.0/src/debloat/archive_processor.py
+-rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.4.0/src/debloat/auxiliary.py
+-rw-rw-rw-   0        0        0     3835 2023-04-20 03:29:34.000000 debloat-1.4.0/src/debloat/gui.py
+-rw-rw-rw-   0        0        0     1679 2023-05-30 12:10:27.000000 debloat-1.4.0/src/debloat/main.py
+-rw-rw-rw-   0        0        0     2536 2023-05-23 11:34:28.000000 debloat-1.4.0/src/debloat/pkreader.py
+-rw-rw-rw-   0        0        0    25547 2023-05-30 12:09:28.000000 debloat-1.4.0/src/debloat/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.256971 debloat-1.4.0/src/debloat/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-24 09:41:28.000000 debloat-1.4.0/src/debloat/tests/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-05-25 09:39:42.000000 debloat-1.4.0/src/debloat/tests/debloat_test.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.253971 debloat-1.4.0/src/debloat.egg-info/
+-rw-rw-rw-   0        0        0     7405 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.3.2.2/LICENSE` & `debloat-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `debloat-1.3.2.2/PKG-INFO` & `debloat-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.3.2.2
+Version: 1.4.0
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `debloat-1.3.2.2/README.md` & `debloat-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `debloat-1.3.2.2/src/debloat/gui.py` & `debloat-1.4.0/src/debloat/gui.py`

 * *Files identical despite different names*

### Comparing `debloat-1.3.2.2/src/debloat/main.py` & `debloat-1.4.0/src/debloat/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     out_path = args.output
 
     if not out_path:
         out_path = file_path.parent \
             / f"{file_path.stem}_patched{file_path.suffix}"
 
     try:
-        pe = pefile.PE(file_path)
+        with open(file_path, "rb") as bloated_file:
+            pe_data = bloated_file.read()
+        pe = pefile.PE(data=pe_data, fast_load=True)
     except Exception:
         print('''
 Provided file is not an executable! Please try again with an executable. 
 Maybe it needs unzipped?'''
               )
         return 1
```

### Comparing `debloat-1.3.2.2/src/debloat/processor.py` & `debloat-1.4.0/src/debloat/processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,59 @@
-"""This file handles the processing of binaries and helper methods."""
+"""
+This file handles the processing of binaries and helper methods.
+
+Three methods are from https://github.com/binref/refinery 
+Copyright 2019 Jesko Hüttenhain used under the 3-Clause BSD License 
+The methods are:
+refinery_strip()
+adjust_offsets()
+refinery_trim_resources()
+The RSRC Class is also from refinery.
+"""
 import re
 from typing import Tuple, Optional, Any, Callable
 import pefile
+import binascii
+import zlib
+from pefile import Structure, SectionStructure, DIRECTORY_ENTRY
+from typing import Generator, Iterable, Optional
+
+_KB = 1000
+_MB = _KB * _KB
 
 PACKER = {
     1 : "Nullsoft"
 }
+import enum
 
+class RSRC(enum.IntEnum):
+    CURSOR        = 0x01  # noqa
+    BITMAP        = 0x02  # noqa
+    ICON          = 0x03  # noqa
+    MENU          = 0x04  # noqa
+    DIALOG        = 0x05  # noqa
+    STRING        = 0x06  # noqa
+    FONTDIR       = 0x07  # noqa
+    FONT          = 0x08  # noqa
+    ACCELERATOR   = 0x09  # noqa
+    RCDATA        = 0x0A  # noqa
+    MESSAGETABLE  = 0x0B  # noqa
+    ICON_GROUP    = 0x0E  # noqa
+    VERSION       = 0x10  # noqa
+    DLGINCLUDE    = 0x11  # noqa
+    PLUGPLAY      = 0x13  # noqa
+    VXD           = 0x14  # noqa
+    ANICURSOR     = 0x15  # noqa
+    ANIICON       = 0x16  # noqa
+    HTML          = 0x17  # noqa
+    MANIFEST      = 0x18  # noqa
+
+    def __str__(self):
+        return self.name
+        
 def readable_size(value: int) -> str:
     '''Return bytes in human readable format.'''
     if value <= 1024:
         return '%s bytes' % value
     elif value < 1024 * 1024:
         return '%.1f KB' % (float(value) / 1024.0)
     elif value < 1024 * 1024 * 1024:
@@ -24,16 +67,16 @@
     '''Writes the patched file to disk.
     
     Keyword Arguments:
     out_path -- the path and file name to write
     pe -- the pefile that is being processed
     end_of_real_data -- an int indicating the size of bytes to write'''
     with open(out_path, 'wb') as writer:
-        writer.write(pe.write()[:end_of_real_data])
-        final_filesize = len(pe.write()[:end_of_real_data])
+        writer.write(pe.write())
+        final_filesize = len(pe.write())
         return final_filesize, out_path
 
 def handle_signature_abnormality(signature_address: int,
                                 signature_size: int, 
                                 beginning_file_size: int) -> bool:
     '''Remove all bytes after a PE signature'''
     # If the signature_address is 0, there was no original signature.
@@ -69,271 +112,435 @@
     last_section = None
     for section in pe.sections:
         if last_section is None \
                         or section.PointerToRawData > last_section.PointerToRawData:
             last_section = section
     return last_section
 
-def remove_signature(pe: pefile.PE) -> Tuple[int, int]:
+def get_signature_info(pe: pefile.PE) -> Tuple[int, int]:
     '''Remove PE signature and update header.''' 
     signature_address = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress
     signature_size = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size
     pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress = 0
     pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size = 0
+    
     return signature_address, signature_size
 
-def remove_resources(pe: pefile.PE, biggest_section: pefile.SectionStructure) -> Tuple[pefile.PE, int]:
-    # This method removed PE resources but not .NET Resources.
-    # PE resources are in the .rcsc section of the binary; 
-    # .NET are in the .text section.
-    # The following nonsense was determined to be the best way
-    # to iterate through resources and find the offending ones.
-    end_of_real_data = len([pe.write()])
-    entry_list = pe.DIRECTORY_ENTRY_RESOURCE.entries
-    for resource_type in pe.DIRECTORY_ENTRY_RESOURCE.entries:
-        if hasattr(resource_type, 'directory'):
-            for resource_id in resource_type.directory.entries:
-                if hasattr(resource_id, 'directory'):
-                    for resource_lang in resource_id.directory.entries:
-                        if hasattr(resource_lang, 'data'):
-                            if resource_lang.data.struct.Size > 50000:
-                                ## If the resource is bloated, remove it with pop
-                                ## then subtract the size from the end_of_real_data variable
-                                resource_type.directory.entries.pop()
-                                end_of_real_data -= resource_lang.data.struct.Size
-                                pe.OPTIONAL_HEADER.DATA_DIRECTORY[2].Size -= resource_lang.data.struct.Size 
-                                pe.sections[pe.sections.index(biggest_section)].SizeOfRawData -= resource_lang.data.struct.Size
-                                pe.sections[pe.sections.index(biggest_section)].Misc_VirtualSize -= resource_lang.data.struct.Size
-                                pe.sections[pe.sections.index(biggest_section)].section_max_addr -= resource_lang.data.struct.Size
-        pe.DIRECTORY_ENTRY_RESOURCE.entries[entry_list.index(resource_type)] = resource_type
-    return pe, end_of_real_data
 
-def check_section_entropy(pe: pefile.PE, end_of_real_data, 
+def adjust_offsets(pe: pefile.PE, gap_offset: int, gap_size: int):
+    base = pe.OPTIONAL_HEADER.ImageBase
+    alignment = pe.OPTIONAL_HEADER.FileAlignment
+    rva_offset = pe.get_rva_from_offset(gap_offset)
+    tva_offset = rva_offset + base
+
+    section = pe.get_section_by_offset(gap_offset)
+    new_section_size = section.SizeOfRawData - gap_size
+    if new_section_size % alignment != 0:
+        raise RuntimeError(
+            F'trimming 0x{gap_size:X} bytes from section {(section.Name)} of size 0x{section.SizeOfRawData:X} '
+            F'violates required section alignment of 0x{alignment:X} bytes')
+    inside_section_offset = gap_offset - section.PointerToRawData
+    if inside_section_offset > new_section_size:
+        overlap = inside_section_offset - new_section_size
+        raise RuntimeError(F'trimming from section {(section.Name)}; data extends {overlap} beyond section')
+
+    rva_lbound = section.VirtualAddress
+    rva_ubound = section.VirtualAddress + section.Misc_VirtualSize - 1
+    tva_lbound = rva_lbound + base
+    tva_ubound = rva_ubound + base
+
+    def adjust_attributes_of_structure(
+        structure: Structure,
+        threshold: int,
+        lbound: Optional[int],
+        ubound: Optional[int],
+        attributes: Iterable[str]
+    ):
+        for attribute in attributes:
+            old_value = getattr(structure, attribute, 0)
+            if old_value <= threshold:
+                continue
+            if lbound is not None and old_value < lbound:
+                continue
+            if ubound is not None and old_value > ubound:
+                continue
+            new_value = old_value - gap_size
+            if new_value < 0:
+                raise RuntimeError(F'adjusting attribute {attribute} of {structure.name} would result in negative value: {new_value}')
+            setattr(structure, attribute, new_value)
+
+    it: Iterable[Structure] = iter(pe.__structures__)
+
+    for structure in it:
+        old_offset = structure.get_file_offset()
+        new_offset = old_offset - gap_offset
+
+        if old_offset > gap_offset:
+            if isinstance(structure, SectionStructure) and new_offset % alignment != 0:
+                raise RuntimeError(
+                    F'section {(structure.Name)} would be moved to offset 0x{new_offset:X}, '
+                    F'violating section alignment value 0x{alignment:X}.')
+            if old_offset < gap_offset + gap_size:
+                raise RuntimeError(
+                    F'structure starts inside removed region: {structure}')
+            structure.set_file_offset(new_offset)
+
+        adjust_attributes_of_structure(structure, rva_offset, rva_lbound, rva_ubound, (
+            'OffsetToData',
+            'AddressOfData',
+            'VirtualAddress',
+            'AddressOfNames',
+            'AddressOfNameOrdinals',
+            'AddressOfFunctions',
+            'AddressOfEntryPoint',
+            'AddressOfRawData',
+            'BaseOfCode',
+            'BaseOfData',
+        ))
+        adjust_attributes_of_structure(structure, tva_offset, tva_lbound, tva_ubound, (
+            'StartAddressOfRawData',
+            'EndAddressOfRawData',
+            'AddressOfIndex',
+            'AddressOfCallBacks',
+        ))
+        adjust_attributes_of_structure(structure, gap_offset, None, None, (
+            'OffsetModuleName',
+            'PointerToRawData',
+        ))
+        
+        for attribute in (
+            'CvHeaderOffset',
+            'OffsetIn2Qwords',
+            'OffsetInQwords',
+            'Offset',
+            'OffsetLow',
+            'OffsetHigh'
+        ):
+            if not hasattr(structure, attribute):
+                continue
+
+    section.SizeOfRawData = new_section_size
+    return pe
+    
+
+
+def refinery_strip(pe: pefile.PE, data: memoryview, block_size=_MB) -> int:
+    threshold = 2
+    alignment = pe.OPTIONAL_HEADER.FileAlignment
+    data_overhang = len(data) % alignment
+    result = data_overhang
+
+    if not data:
+        return 0
+    
+    if 0 < threshold < 1:
+        def compression_ratio(offset: int):
+            ratio = len(zlib.compress(data[:offset], level=1))
+            return ratio
+        upper = len(data)
+        lower = result
+        if compression_ratio(upper) <= threshold:
+            while block_size < upper - lower:
+                pivot = (lower + upper) // 2
+                ratio = compression_ratio(pivot)
+                if ratio > threshold:
+                    lower = pivot + 1
+                    continue
+                upper = pivot
+                if abs(ratio - threshold) < 1e-10:
+                    break
+        result = upper
+
+    match = re.search(B'(?s).(?=\\x%02x+$)' % data[result - 1], data[:result])
+    if match is not None:
+        cutoff = match.start() - 1
+        length = result - cutoff
+        if length > block_size:
+            result = cutoff
+
+    result = max(result, data_overhang)
+
+    result = result + (data_overhang - result) % alignment
+
+    while result > len(data):
+        result -= alignment
+
+    return result
+
+
+def refinery_trim_resources(pe: pefile.PE, pe_data: bytearray) -> int:
+    size_limit = 50000
+    size_removed = 0
+
+    def find_bloated_resources(pe: pefile.PE, directory, level: int = 0, *path) -> Generator[Structure, None, None]:
+        for entry in directory.entries:
+            name = getattr(entry, 'name')
+            numeric_id = getattr(entry, 'id')
+            if not name:
+                if level == 0 and numeric_id in iter(RSRC):
+                    name = RSRC(entry.id)
+                elif numeric_id is not None:
+                    name = str(numeric_id)
+            name = name and str(name) or '?'
+            if entry.struct.DataIsDirectory:
+                yield from find_bloated_resources(pe, entry.directory, level + 1, *path, name)
+                continue
+            struct: Structure = entry.data.struct
+            name = '/'.join((*path, name))
+            if struct.Size <= size_limit:
+                continue
+            yield name, struct
+    
+    RSRC_INDEX = DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_RESOURCE']
+    pe.parse_data_directories(directories=[RSRC_INDEX])
+
+    try:
+        resources = pe.DIRECTORY_ENTRY_RESOURCE
+    except AttributeError:
+        return 0
+    for name, resource in find_bloated_resources(pe, resources):
+        offset = pe.get_offset_from_rva(resource.OffsetToData)
+        old_size = resource.Size
+        new_size = refinery_strip(pe, memoryview(pe_data)[offset:offset + old_size])
+        gap_size = old_size - new_size
+        gap_offset = offset + new_size
+        if gap_size <= 0:
+            continue
+        resource.Size = new_size
+        adjust_offsets(pe, gap_offset, gap_size)
+        size_removed += gap_size
+        pe_data[gap_offset:gap_offset + gap_size] = []
+
+    pe.OPTIONAL_HEADER.DATA_DIRECTORY[RSRC_INDEX].Size -= size_removed
+    return size_removed
+        
+    
+
+def remove_resources(pe: pefile.PE, pe_data: bytearray) -> Tuple[bytearray, int]:
+    trimmed = refinery_trim_resources(pe, pe_data)
+    return trimmed
+
+def check_section_compression(pe: pefile.PE, pe_data: bytearray, end_of_real_data, 
                           log_message: Callable[[str], None]) -> Tuple[pefile.PE, int, str]:
         biggest_section = None
+        biggest_uncompressed = int
         result = ""
         for section in pe.sections:
             section_name = section.Name.decode()
-            section_entropy = section.get_entropy()
+            compressed_section_size = len(zlib.compress(
+                pe.write()[section.PointerToRawData: 
+                           (section.PointerToRawData + section.SizeOfRawData)]))
+            uncompressed_section_size = section.SizeOfRawData
+            section_compression_ratio = uncompressed_section_size / compressed_section_size * 100
             log_message("Section: "  + section_name, end="\t", flush=True)
-            log_message(" Entropy: " + str(round(section_entropy, 4)), end="\t",flush=True) 
+            log_message(" Compression Ratio: " + str(round(section_compression_ratio, 2)) +"%", end="\t",flush=True) 
             log_message("Size of section: " + readable_size(section.SizeOfRawData) +".",flush=True)
-            # The use cases covered by this section are at the end of 
-            # the binary. In my experience, the bloated sections are 
-            # usually at the end unless they are bloat from .NET Resources.
-            if section_entropy < 0.09 and section.SizeOfRawData > 100000:
-                log_message('''
-Entropy of section is exteremely low. This is indicative of a bloated section. 
-Removing bloated section... 
-''', end="", flush=True)
-                # Get the size of the section.
-                section_end = section.PointerToRawData + section.SizeOfRawData
-                # If the entropy is simply 0.00, there is no data to be 
-                # missed, we won't waste CPU and just drop the whole thing.
-                delta_last_non_junk = 0
-                if section_entropy == 0.00:
-                    # To play it safe, we will leave 100 bytes in the 
-                    # section. And thus mark the end of the binary as 
-                    # the beginning of the last section + 100.
-                    section_bytes_to_remove = section.SizeOfRawData - 100
-                    end_of_real_data = section.PointerToRawData + 100
-                # If the section has low entropy we'll try to determine
-                #  how much is junk.
-                else:
-                    section_data = pe.write()[section.PointerToRawData:section_end]
-                    section_end = section.PointerToRawData + section.SizeOfRawData
-                    backward_section_data = section_data[::-1]
-                    # TODO: refactor junk matching from overlay dynamic 
-                    # trim.
-                    junk_match = re.search(rb"(..)\1{20,}", backward_section_data[:200])
-                    if not junk_match:
-                        for i in range(20):
-                            junk_regex = rb"^(..{" + bytes(str(i), "utf-8") + rb"})\1{2,}"
-                            multibyte_junk_regex = re.search(junk_regex,
-                                                            backward_section_data[:200])
-                            if multibyte_junk_regex:
-                                # Having found the pattern, we can make the regex efficient
-                                # by targeting the pattern using the "targeted_regex"
-                                targeted_regex = rb"(" + multibyte_junk_regex.string + rb")\1{2,}"
-                                multibyte_junk_regex = re.search(targeted_regex,
-                                                                backward_section_data)
-                                junk_to_remove = multibyte_junk_regex.end(0)
-                                delta_last_non_junk = end_of_real_data - junk_to_remove
-                                break
-
-                    else:
-                        targeted_regex = rb""+ junk_match.string + rb"{1,}"
-                        targeted_junk_match = re.search(targeted_regex, backward_section_data)
-                        junk_to_remove = targeted_junk_match.end(0)
-                        if junk_to_remove < end_of_real_data / 2:
-                            chunk_start = targeted_junk_match.end(0)
-                            chunk_end = chunk_start
-                            while end_of_real_data > chunk_end:
-                                chunk_end = chunk_start + 200
-                                repeated_junk_match = re.search(rb'(..)\1{20,}', 
-                                                                backward_section_data[chunk_start:chunk_end])
-                                if repeated_junk_match:
-                                    chunk_start += repeated_junk_match.end(0)
-                                else:
-                                    break
-                            junk_to_remove = chunk_start
-                        delta_last_non_junk = len(backward_section_data) - junk_to_remove
-                section_bytes_to_remove = end_of_real_data \
-                    - (section.PointerToRawData + delta_last_non_junk + 1)
-                end_of_real_data = section.PointerToRawData + delta_last_non_junk + 1
-                # This will update the last section header, SizeOfRawData, SizeOfImage.
-                section.Misc_VirtualSize -= section_bytes_to_remove
-                section.SizeOfRawData -= section_bytes_to_remove
-                pe.OPTIONAL_HEADER.SizeOfImage -= section_bytes_to_remove
-                log_message("Bloated section reduced.")
-                return pe, end_of_real_data, result
-            # Handle specific bloated sections
             if biggest_section == None:
                 biggest_section = section
+                biggest_uncompressed = section_compression_ratio
             elif section.SizeOfRawData > biggest_section.SizeOfRawData:
                 biggest_section = section
+                biggest_uncompressed = section_compression_ratio
+        # Handle specific bloated sections
         if biggest_section.Name.decode() == ".rsrc\x00\x00\x00":
             # Get biggest resource or resources and drop them from the 
             # Resource table
             # TODO: recalculate PE header in situations where the 
             # resource is not at the end of an executable.
             # TODO: Handle other tomfoolery required when resource 
             # is not at end of executable.
             log_message('''
-Bloat was located in the resource section. Removing bloat.. \n
+Bloat was located in the resource section. Removing bloat.. 
 ''')
-            pe, end_of_real_data = remove_resources(pe, biggest_section)
-            return pe, end_of_real_data, result
+            
+            bytes_removed = remove_resources(pe, pe_data)
+            end_of_real_data =- bytes_removed
+            return end_of_real_data, result
         elif biggest_section.Name.decode() == ".text\x00\x00\x00":
             # Data stored in the .text section is often a .NET Resource. The following checks
             # to confirm it is .NET and then drops the resources.
             if pe.OPTIONAL_HEADER.DATA_DIRECTORY[14].Size:
                 log_message('''
 Bloat was detected in the text section. Bloat is likely in a .NET Resource 
-This use case cannot be processed at this time.\n
-''')
-            return pe, end_of_real_data, result
+This use case cannot be processed at this time. ''')
+            return end_of_real_data, result
+                
+        # The use cases covered by this section are at the end of 
+        # the binary. In my experience, the bloated sections are 
+        # usually at the end unless they are bloat from .NET Resources.
+        if biggest_uncompressed > 3000:
+            log_message('''
+The compression ratio is indicative of a bloated section.
+''', end="", flush=True)
+            # Get the size of the section.
+            section_end = section.PointerToRawData + section.SizeOfRawData
+            original_section_size = section.SizeOfRawData
+            section_data = pe_data[section.PointerToRawData:section_end]
+            delta_last_non_junk = trim_junk(section_data, original_section_size)
+            pe_data[section.PointerToRawData + delta_last_non_junk:section_end] = []
+            section_bytes_to_remove = original_section_size - delta_last_non_junk
+            end_of_real_data =  end_of_real_data - section_bytes_to_remove
+            # This will update the last section header, SizeOfRawData, SizeOfImage.
+            pe.sections[pe.sections.index(biggest_section)].section_max_addr -= section_bytes_to_remove
+            pe.sections[pe.sections.index(biggest_section)].SizeOfRawData -= section_bytes_to_remove
+            #pe.sections[pe.sections.index(biggest_section)].Misc_VirtualSize -= section_bytes_to_remove
+            #pe.OPTIONAL_HEADER.SizeOfImage -= section_bytes_to_remove
+            log_message("Bloated section reduced.")
+            return end_of_real_data, result
+            
+       
         
-def trim_junk(pe: pefile.PE, end_of_real_data) -> int:
+def trim_junk(bloated_content: bytes, original_size_with_junk: int) -> int:
     ''' Attempt multiple methods or removing junk from overlay.'''
-    backwards_overlay = pe.get_overlay()[::-1]
+    backward_bloated_content = bloated_content[::-1]
     # Regex Explained:
     # Match raw bytes that are repeated more than 20 times at the end
-    # of a binary. Trims 1 repeating byte.
-    delta_last_non_junk = end_of_real_data
+    # of a binary. 
+    delta_last_non_junk = original_size_with_junk
+    # First Method: Trims 1 repeating byte.
     # Check against 200 bytes, if successful, calculate full match.
-    junk_match = re.search(rb'^(..)\1{20,}', backwards_overlay[:200])
-    # If "not junk_match" check for junk larger than 1 byte
+    junk_match = re.search(rb'^(..)\1{20,}', backward_bloated_content[:600])
+    # Second Method: If "not junk_match" check for junk larger than 1 repeating byte
     if not junk_match:
         # Brute force check: check to see if there are 1-20 bytes
         # being repeated and feed the number into the regex
-        for i in range(20):
+        for i in range(300):
             # Regex Explained:
             # Starting at the end of the PE, check for repeated bytes.
             # This indicates junk bytes in the overlay. Match that set
             # of repeated bytes 1 or more times. 
             junk_regex = rb"^(..{" + bytes(str(i), "utf-8") + rb"})\1{2,}"
-            multibyte_junk_regex = re.search(junk_regex, backwards_overlay[:200])
+            multibyte_junk_regex = re.search(junk_regex, backward_bloated_content[:1000])
             if multibyte_junk_regex:
                 # Having found the pattern, we can make the regex efficient
                 # by targeting the pattern using the "targeted_regex"
-                targeted_regex = rb"(" + multibyte_junk_regex.string + rb")\1{2,}"
-                multibyte_junk_regex = re.search(targeted_regex, backwards_overlay)
-                junk_to_remove = multibyte_junk_regex.end(0)
-                delta_last_non_junk = end_of_real_data - junk_to_remove
+                targeted_regex = rb"(" + binascii.hexlify(multibyte_junk_regex.group(1)) + rb")\1{1,}"
+                chunk_start = 0
+                chunk_end = chunk_start
+                while original_size_with_junk > chunk_end:
+                    chunk_end = chunk_start + 1000
+                    targeted_multibyte_junk_regex = re.search(targeted_regex, 
+                                                              binascii.hexlify(backward_bloated_content[chunk_start:chunk_end]))
+                    if targeted_multibyte_junk_regex:
+                        chunk_start += targeted_multibyte_junk_regex.end(0)
+                        unmatched_portion = 1000 - targeted_multibyte_junk_regex.end(0)
+                    else:
+                        # If the targeted_multibyte_junk_regex does not
+                        # return anything, that indicates the previous loop
+                        # had content which did not match. We'll use that
+                        # to help ensure we do not remove too much of the file. 
+                        chunk_start += unmatched_portion 
+                        break
                 break
-    # Junk was identified. New end_of_real_data is assigned and returned.
+                # It was determined that data cannot be removed any more
+                # from the chunk_start. But the value of chunk_start
+                # now tells us how much data we can safely remove.
+        junk_to_remove = chunk_start  
+        #junk_to_remove = int(junk_to_remove)
+        delta_last_non_junk -= junk_to_remove
+    # Third Method: check for a series of one repeated byte. 
+    # Junk was identified. A new size is assigned and returned.
     else:
-        targeted_regex = rb""+ junk_match.string + rb"{1,}"
-        targeted_junk_match = re.search(targeted_regex, backwards_overlay)
+        targeted_regex = rb""+ binascii.hexlify(junk_match.string) + rb"{1,}"
+        targeted_junk_match = re.search(targeted_regex, binascii.hexlify(backward_bloated_content))
         junk_to_remove = targeted_junk_match.end(0)
         # If the trimming did not remove more than half of the bytes then
         # this suggests the attacker may have put a random series of
         # repeated bytes. These will be removed by loading the overlay
         # 200 bytes at a time and removing parts which repeat for more
         # than 20 bytes.
-        if junk_to_remove < end_of_real_data / 2:
+        if junk_to_remove < original_size_with_junk / 2:
             chunk_start = targeted_junk_match.end(0)
             chunk_end = chunk_start
-            while end_of_real_data > chunk_end:
+            while original_size_with_junk > chunk_end:
                 chunk_end = chunk_start + 200
                 repeated_junk_match = re.search(rb'(..)\1{20,}', 
-                                                backwards_overlay[chunk_start:chunk_end])
+                                                binascii.hexlify(backward_bloated_content[chunk_start:chunk_end]))
                 if repeated_junk_match:
                     chunk_start += repeated_junk_match.end(0)
+                    unmatched_portion = 200 - repeated_junk_match.end(0)
                 else:
+                    chunk_start += unmatched_portion
                     break
-            junk_to_remove = chunk_start
-        delta_last_non_junk = end_of_real_data - junk_to_remove
-    return delta_last_non_junk
+            junk_to_remove = chunk_start 
+        else:
+            junk_to_remove = int(junk_to_remove / 2)
+        delta_last_non_junk -= junk_to_remove
+    return delta_last_non_junk  
 
 def process_pe(pe: pefile.PE, out_path: str, unsafe_processing: bool,
                log_message: Callable[[str], None]) -> None:
     '''Prepare PE, perform checks, remote junk, write patched binary.'''
     beginning_file_size = len(pe.write())
     # We are using the variable "end_of_real_data" and are reassigning 
     # the value based on our analysis.We are assigning it now in case 
     # we are unable to reduce the binary size for any reason.
     end_of_real_data = beginning_file_size
+    pe_data = bytearray(pe.__data__)
     # Remove Signature and modify size of Optional Header Security entry.
-    signature_address, signature_size = remove_signature(pe)
+    signature_address, signature_size = get_signature_info(pe)
+    pe_data[signature_address:signature_address + signature_size] = []
     signature_abnormality = handle_signature_abnormality(signature_address, 
                                                         signature_size, 
                                                         beginning_file_size)
     if signature_abnormality:
         log_message('''
 We detected data after the signature. This is abnormal. Removing signature and extra data...''')
         end_of_real_data = signature_address
+        pe_data = pe_data[:end_of_real_data]
     # Handle Overlays: this includes packers and overlays which are completely junk
     elif pe.get_overlay_data_start_offset() and signature_size < len(pe.get_overlay()):
         log_message("An overlay was detected. Checking for known packer.")
         packer_idenfitied = check_for_packer(pe)
         if packer_idenfitied:
             log_message("Packer identified: " + PACKER[packer_idenfitied])
             if PACKER[1]:
                 log_message('''
 The original file cannot be debloated. It must be unpacked with a tool such as UniExtract2.
                 ''')
         else:
             log_message("Packer not identified. Attempting dynamic trim...")
-            end_of_real_data = trim_junk(pe, end_of_real_data)
+            last_section = find_last_section(pe)
+            overlay = pe_data[last_section.PointerToRawData + last_section.SizeOfRawData:]
+            end_of_real_data = trim_junk(overlay, end_of_real_data)
+            pe_data = pe_data[:end_of_real_data]
             if end_of_real_data == beginning_file_size:
                 if unsafe_processing is True:
                     log_message("""
 "Unsafe" switch detected. Running unsafe debloat technique:\n
 This is the last resort of removing the whole overlay: this works in some 
 cases, but can remove critical content. 
 If file is a Nullsoft executable, but was not detected, the original file can 
 be unpacked with the tool "UniExtract2".
                     """)
                     last_section = find_last_section(pe)
                     end_of_real_data = last_section.PointerToRawData + last_section.SizeOfRawData 
                 else:
                     log_message("""
 Overlay was unable to be trimmed. Try unpacking with UniExtract2 or re-running 
-Debloat without the "--unsafe" parameter."""
+Debloat with the "--unsafe" parameter."""
                                 )
     # Handle bloated sections
     # TODO: break up into functions
     else:
         # In order to solve some use cases, we will find the biggest section 
         # within the binary.
-        pe, end_of_real_data, result = check_section_entropy(pe, 
+        end_of_real_data, result = check_section_compression(pe, pe_data,
                                                              end_of_real_data, 
                                                              log_message=log_message)
         log_message(result)
     # All processing is done. Report results.
     if end_of_real_data == beginning_file_size:
-        log_message("""
-No automated method for reducing the size worked. Please consider sharing the
+        log_message("""No automated method for reducing the size worked. Please consider sharing the
 sample for additional analysis.
 Email: Squiblydoo@pm.me
 Twitter: @SquiblydooBlog.
                     """)
     else:
+        pe.__data__ =pe_data
         final_filesize, new_pe_name = write_patched_file(out_path,
                                                          pe, 
                                                          end_of_real_data)
         reduction_calculation = round(((beginning_file_size \
                                         - final_filesize) \
                                         / beginning_file_size) * 100, 2)
         log_message("Beginning File size: " \
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `debloat-1.3.2.2/src/debloat.egg-info/PKG-INFO` & `debloat-1.4.0/src/debloat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.3.2.2
+Version: 1.4.0
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

