# Comparing `tmp/visor_gligen-1.3.tar.gz` & `tmp/visor_gligen-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visor_gligen-1.3.tar", last modified: Tue May 30 04:45:12 2023, max compression
+gzip compressed data, was "dist/visor_gligen-1.4.tar", last modified: Tue May 30 04:55:59 2023, max compression
```

## Comparing `visor_gligen-1.3.tar` & `visor_gligen-1.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.646119 visor_gligen-1.3/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       94 2023-05-30 04:45:12.646119 visor_gligen-1.3/PKG-INFO
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6697 2023-05-28 18:35:53.000000 visor_gligen-1.3/README.md
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       38 2023-05-30 04:45:12.646119 visor_gligen-1.3/setup.cfg
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)      338 2023-05-30 04:44:26.000000 visor_gligen-1.3/setup.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.642119 visor_gligen-1.3/visor_gligen/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    36555 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/gligen_inference_box.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6039 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/inpaint_mask_func.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.642119 visor_gligen-1.3/visor_gligen/ldm/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/__init__.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.646119 visor_gligen-1.3/visor_gligen/ldm/models/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/models/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     1364 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/models/autoencoder.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.646119 visor_gligen-1.3/visor_gligen/ldm/models/diffusion/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:18:26.000000 visor_gligen-1.3/visor_gligen/ldm/models/diffusion/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    10302 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/models/diffusion/classifier.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6100 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/models/diffusion/ddim.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2859 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/models/diffusion/ddpm.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     3155 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/models/diffusion/ldm.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     7552 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/models/diffusion/plms.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.646119 visor_gligen-1.3/visor_gligen/ldm/modules/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    10821 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/attention.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.646119 visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:42:02.000000 visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)      564 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/grounding_net_example.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2317 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/keypoint_grounding_net.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    33435 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    15183 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     1785 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/text_grounding_net.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2742 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/text_image_grounding_net.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     9747 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/util.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.646119 visor_gligen-1.3/visor_gligen/ldm/modules/distributions/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:42:05.000000 visor_gligen-1.3/visor_gligen/ldm/modules/distributions/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2970 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/distributions/distributions.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2982 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/ema.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.646119 visor_gligen-1.3/visor_gligen/ldm/modules/encoders/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:42:12.000000 visor_gligen-1.3/visor_gligen/ldm/modules/encoders/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     8860 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/encoders/modules.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     8180 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/encoders/modules_backup.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.646119 visor_gligen-1.3/visor_gligen/ldm/modules/image_degradation/
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)      234 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    25198 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    22238 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/image_degradation/bsrgan_light.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    29024 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/image_degradation/utils_image.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.646119 visor_gligen-1.3/visor_gligen/ldm/modules/losses/
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)       81 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/modules/losses/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     5581 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/losses/contperceptual.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     7941 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/losses/vqperceptual.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    20168 2023-04-16 05:30:27.000000 visor_gligen-1.3/visor_gligen/ldm/modules/x_transformer.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2517 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/ldm/util.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    19659 2023-05-28 18:35:53.000000 visor_gligen-1.3/visor_gligen/trainer.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:45:12.642119 visor_gligen-1.3/visor_gligen.egg-info/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       94 2023-05-30 04:45:12.000000 visor_gligen-1.3/visor_gligen.egg-info/PKG-INFO
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)     1954 2023-05-30 04:45:12.000000 visor_gligen-1.3/visor_gligen.egg-info/SOURCES.txt
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        1 2023-05-30 04:45:12.000000 visor_gligen-1.3/visor_gligen.egg-info/dependency_links.txt
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       92 2023-05-30 04:45:12.000000 visor_gligen-1.3/visor_gligen.egg-info/requires.txt
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       13 2023-05-30 04:45:12.000000 visor_gligen-1.3/visor_gligen.egg-info/top_level.txt
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.678386 visor_gligen-1.4/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       94 2023-05-30 04:55:59.678386 visor_gligen-1.4/PKG-INFO
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6697 2023-05-28 18:35:53.000000 visor_gligen-1.4/README.md
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       38 2023-05-30 04:55:59.678386 visor_gligen-1.4/setup.cfg
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)      338 2023-05-30 04:55:43.000000 visor_gligen-1.4/setup.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.674386 visor_gligen-1.4/visor_gligen/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    14652 2023-05-30 04:54:20.000000 visor_gligen-1.4/visor_gligen/gligen_inference_box.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6039 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/inpaint_mask_func.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.674386 visor_gligen-1.4/visor_gligen/ldm/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/__init__.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.674386 visor_gligen-1.4/visor_gligen/ldm/models/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/models/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     1364 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/models/autoencoder.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.674386 visor_gligen-1.4/visor_gligen/ldm/models/diffusion/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:18:26.000000 visor_gligen-1.4/visor_gligen/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    10302 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/models/diffusion/classifier.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6100 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2859 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/models/diffusion/ddpm.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     3155 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/models/diffusion/ldm.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     7552 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/models/diffusion/plms.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.678386 visor_gligen-1.4/visor_gligen/ldm/modules/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    10821 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/attention.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.678386 visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:42:02.000000 visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)      564 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/grounding_net_example.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2317 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/keypoint_grounding_net.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    33435 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    15183 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     1785 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/text_grounding_net.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2742 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/text_image_grounding_net.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     9747 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/util.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.678386 visor_gligen-1.4/visor_gligen/ldm/modules/distributions/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:42:05.000000 visor_gligen-1.4/visor_gligen/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2970 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2982 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/ema.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.678386 visor_gligen-1.4/visor_gligen/ldm/modules/encoders/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:42:12.000000 visor_gligen-1.4/visor_gligen/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     8860 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/encoders/modules.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     8180 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/encoders/modules_backup.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.678386 visor_gligen-1.4/visor_gligen/ldm/modules/image_degradation/
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)      234 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    25198 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    22238 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/image_degradation/bsrgan_light.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    29024 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/image_degradation/utils_image.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.678386 visor_gligen-1.4/visor_gligen/ldm/modules/losses/
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)       81 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/modules/losses/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     5581 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/losses/contperceptual.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     7941 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/losses/vqperceptual.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    20168 2023-04-16 05:30:27.000000 visor_gligen-1.4/visor_gligen/ldm/modules/x_transformer.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2517 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/ldm/util.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    19659 2023-05-28 18:35:53.000000 visor_gligen-1.4/visor_gligen/trainer.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-30 04:55:59.674386 visor_gligen-1.4/visor_gligen.egg-info/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       94 2023-05-30 04:55:59.000000 visor_gligen-1.4/visor_gligen.egg-info/PKG-INFO
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)     1954 2023-05-30 04:55:59.000000 visor_gligen-1.4/visor_gligen.egg-info/SOURCES.txt
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        1 2023-05-30 04:55:59.000000 visor_gligen-1.4/visor_gligen.egg-info/dependency_links.txt
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       92 2023-05-30 04:55:59.000000 visor_gligen-1.4/visor_gligen.egg-info/requires.txt
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       13 2023-05-30 04:55:59.000000 visor_gligen-1.4/visor_gligen.egg-info/top_level.txt
```

### Comparing `visor_gligen-1.3/README.md` & `visor_gligen-1.4/README.md`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/inpaint_mask_func.py` & `visor_gligen-1.4/visor_gligen/inpaint_mask_func.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/models/autoencoder.py` & `visor_gligen-1.4/visor_gligen/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/models/diffusion/classifier.py` & `visor_gligen-1.4/visor_gligen/ldm/models/diffusion/classifier.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/models/diffusion/ddim.py` & `visor_gligen-1.4/visor_gligen/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/models/diffusion/ddpm.py` & `visor_gligen-1.4/visor_gligen/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/models/diffusion/ldm.py` & `visor_gligen-1.4/visor_gligen/ldm/models/diffusion/ldm.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/models/diffusion/plms.py` & `visor_gligen-1.4/visor_gligen/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/attention.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/grounding_net_example.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/grounding_net_example.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/keypoint_grounding_net.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/keypoint_grounding_net.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/model.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/openaimodel.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/text_grounding_net.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/text_grounding_net.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/text_image_grounding_net.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/text_image_grounding_net.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/diffusionmodules/util.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/distributions/distributions.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/ema.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/encoders/modules.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/encoders/modules_backup.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/encoders/modules_backup.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/image_degradation/bsrgan.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/image_degradation/bsrgan_light.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/image_degradation/utils_image.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/losses/contperceptual.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/losses/contperceptual.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/losses/vqperceptual.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/losses/vqperceptual.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/modules/x_transformer.py` & `visor_gligen-1.4/visor_gligen/ldm/modules/x_transformer.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/ldm/util.py` & `visor_gligen-1.4/visor_gligen/ldm/util.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen/trainer.py` & `visor_gligen-1.4/visor_gligen/trainer.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.3/visor_gligen.egg-info/SOURCES.txt` & `visor_gligen-1.4/visor_gligen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

