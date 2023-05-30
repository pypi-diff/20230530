# Comparing `tmp/unstructured_inference-0.5.0.tar.gz` & `tmp/unstructured_inference-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.5.0.tar", last modified: Thu May 18 20:00:21 2023, max compression
+gzip compressed data, was "unstructured_inference-0.5.1.tar", last modified: Tue May 30 21:18:31 2023, max compression
```

## Comparing `unstructured_inference-0.5.0.tar` & `unstructured_inference-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.175327 unstructured_inference-0.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.175327 unstructured_inference-0.5.0/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.179327 unstructured_inference-0.5.0/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/detectron2onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/unstructured_inference/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/patches/pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.179327 unstructured_inference-0.5.0/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.426563 unstructured_inference-0.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.430563 unstructured_inference-0.5.1/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.430563 unstructured_inference-0.5.1/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/detectron2onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.430563 unstructured_inference-0.5.1/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.5.0/PKG-INFO` & `unstructured_inference-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.5.0
+Version: 0.5.1
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.0/README.md` & `unstructured_inference-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/setup.py` & `unstructured_inference-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/inference/elements.py` & `unstructured_inference-0.5.1/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/inference/layout.py` & `unstructured_inference-0.5.1/unstructured_inference/inference/layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 )
 from unstructured_inference.inference.layoutelement import LayoutElement
 from unstructured_inference.inference.ordering import order_layout
 from unstructured_inference.logger import logger
 from unstructured_inference.models.base import get_model
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 from unstructured_inference.patches.pdfminer import parse_keyword
+from unstructured_inference.visualize import draw_bbox
 
 # NOTE(alan): Patching this to fix a bug in pdfminer.six. Submitted this PR into pdfminer.six to fix
 # the bug: https://github.com/pdfminer/pdfminer.six/pull/885
 psparser.PSBaseParser._parse_keyword = parse_keyword  # type: ignore
 
 import pdfplumber  # noqa
 
@@ -72,19 +73,20 @@
         if len(layouts) > len(images):
             raise RuntimeError(
                 "Some images were not loaded. Check that poppler is installed and in your $PATH."
             )
         pages: List[PageLayout] = list()
         if fixed_layouts is None:
             fixed_layouts = [None for _ in layouts]
-        for image, layout, fixed_layout in zip(images, layouts, fixed_layouts):
+        for i, (image, layout, fixed_layout) in enumerate(zip(images, layouts, fixed_layouts)):
             # NOTE(robinson) - In the future, maybe we detect the page number and default
             # to the index if it is not detected
             page = PageLayout.from_image(
                 image,
+                number=i + 1,
                 model=model,
                 layout=layout,
                 ocr_strategy=ocr_strategy,
                 ocr_languages=ocr_languages,
                 fixed_layout=fixed_layout,
                 extract_tables=extract_tables,
             )
@@ -187,28 +189,44 @@
 
     def _get_image_array(self) -> Union[np.ndarray, None]:
         """Converts the raw image into a numpy array."""
         if self.image_array is None:
             self.image_array = np.array(self.image)
         return self.image_array
 
+    def annotate(self, colors: Optional[Union[List[str], str]] = None) -> Image.Image:
+        """Annotates the elements on the page image."""
+        if colors is None:
+            colors = ["red" for _ in self.elements]
+        if isinstance(colors, str):
+            colors = [colors]
+        # If there aren't enough colors, just cycle through the colors a few times
+        if len(colors) < len(self.elements):
+            n_copies = (len(self.elements) // len(colors)) + 1
+            colors = colors * n_copies
+        img = self.image.copy()
+        for el, color in zip(self.elements, colors):
+            img = draw_bbox(img, el, color=color)
+        return img
+
     @classmethod
     def from_image(
         cls,
         image,
+        number=1,
         model: Optional[UnstructuredModel] = None,
         layout: Optional[List[TextRegion]] = None,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
         extract_tables: bool = False,
         fixed_layout: Optional[List[TextRegion]] = None,
     ):
         """Creates a PageLayout from an already-loaded PIL Image."""
         page = cls(
-            number=0,
+            number=number,
             image=image,
             layout=layout,
             model=model,
             ocr_strategy=ocr_strategy,
             ocr_languages=ocr_languages,
             extract_tables=extract_tables,
         )
```

### Comparing `unstructured_inference-0.5.0/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.5.1/unstructured_inference/inference/layoutelement.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/models/base.py` & `unstructured_inference-0.5.1/unstructured_inference/models/base.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.5.1/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/models/detectron2onnx.py` & `unstructured_inference-0.5.1/unstructured_inference/models/detectron2onnx.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,19 @@
     required_h = 1035
 
     def predict(self, image: Image.Image) -> List[LayoutElement]:
         """Makes a prediction using detectron2 model."""
         super().predict(image)
 
         prepared_input = self.preprocess(image)
-        bboxes, labels, confidence_scores, _ = self.model.run(None, prepared_input)
+        try:
+            bboxes, labels, confidence_scores, _ = self.model.run(None, prepared_input)
+        except onnxruntime.capi.onnxruntime_pybind11_state.RuntimeException:
+            logger.error("Something happened while inferencing page")
+            return []
         input_w, input_h = image.size
         regions = self.postprocess(bboxes, labels, confidence_scores, input_w, input_h)
 
         return regions
 
     def initialize(
         self,
```

### Comparing `unstructured_inference-0.5.0/unstructured_inference/models/donut.py` & `unstructured_inference-0.5.1/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.5.1/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/models/tables.py` & `unstructured_inference-0.5.1/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.5.1/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.5.1/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/models/yolox.py` & `unstructured_inference-0.5.1/unstructured_inference/models/yolox.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from huggingface_hub import hf_hub_download
 import numpy as np
 import onnxruntime
 from typing import List
 
 from unstructured_inference.inference.layoutelement import LayoutElement
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
-from unstructured_inference.visualize import draw_bounding_boxes
+from unstructured_inference.visualize import draw_yolox_bounding_boxes
 from unstructured_inference.utils import LazyDict, LazyEvaluateInfo
 
 YOLOX_LABEL_MAP = {
     0: "Caption",
     1: "Footnote",
     2: "Formula",
     3: "List-item",
@@ -114,15 +114,15 @@
         return page_layout
 
     def annotate_image(self, image_fn, dets, out_fn):
         """Draw bounding boxes and prediction metadata."""
         origin_img = np.array(Image.open(image_fn))
         final_boxes, final_scores, final_cls_inds = dets[:, :4], dets[:, 4], dets[:, 5]
 
-        annotated_image = draw_bounding_boxes(
+        annotated_image = draw_yolox_bounding_boxes(
             origin_img,
             final_boxes,
             final_scores,
             final_cls_inds,
             conf=0.3,
             class_names=self.layout_classes,
         )
```

### Comparing `unstructured_inference-0.5.0/unstructured_inference/patches/pdfminer.py` & `unstructured_inference-0.5.1/unstructured_inference/patches/pdfminer.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference/utils.py` & `unstructured_inference-0.5.1/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.0/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.5.1/unstructured_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.5.0
+Version: 0.5.1
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.0/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.5.1/unstructured_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

