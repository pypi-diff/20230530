# Comparing `tmp/spm12-2.0.0-py2.py3-none-any.whl.zip` & `tmp/spm12-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 11480 bytes, number of entries: 17
--rw-r--r--  2.0 unx      382 b- defN 22-Aug-06 08:57 spm12/__init__.py
--rw-r--r--  2.0 unx      137 b- defN 22-Aug-06 08:57 spm12/__main__.py
--rw-r--r--  2.0 unx       22 b- defN 22-Aug-06 08:57 spm12/_dist_ver.py
--rw-r--r--  2.0 unx      776 b- defN 22-Aug-06 08:57 spm12/amypad_coreg.m
--rw-r--r--  2.0 unx      186 b- defN 22-Aug-06 08:57 spm12/amypad_coreg_modify_affine.m
--rw-r--r--  2.0 unx      368 b- defN 22-Aug-06 08:57 spm12/amypad_normw.m
--rw-r--r--  2.0 unx      641 b- defN 22-Aug-06 08:57 spm12/amypad_resample.m
--rw-r--r--  2.0 unx     1792 b- defN 22-Aug-06 08:57 spm12/amypad_seg.m
--rw-r--r--  2.0 unx      551 b- defN 22-Aug-06 08:57 spm12/cli.py
--rw-r--r--  2.0 unx    13791 b- defN 22-Aug-06 08:57 spm12/regseg.py
--rw-r--r--  2.0 unx     1955 b- defN 22-Aug-06 08:57 spm12/utils.py
--rw-r--r--  2.0 unx      550 b- defN 22-Aug-06 08:57 spm12-2.0.0.dist-info/LICENCE.md
--rw-r--r--  2.0 unx     3616 b- defN 22-Aug-06 08:57 spm12-2.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Aug-06 08:57 spm12-2.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 22-Aug-06 08:57 spm12-2.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Aug-06 08:57 spm12-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1298 b- defN 22-Aug-06 08:57 spm12-2.0.0.dist-info/RECORD
-17 files, 26222 bytes uncompressed, 9370 bytes compressed:  64.3%
+Zip file size: 13488 bytes, number of entries: 19
+-rw-r--r--  2.0 unx       49 b- defN 23-May-30 19:17 examples/.gitignore
+-rw-r--r--  2.0 unx     2982 b- defN 23-May-30 19:17 examples/demo.ipynb
+-rw-r--r--  2.0 unx      412 b- defN 23-May-30 19:17 spm12/__init__.py
+-rw-r--r--  2.0 unx      136 b- defN 23-May-30 19:17 spm12/__main__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-May-30 19:17 spm12/_dist_ver.py
+-rw-r--r--  2.0 unx      776 b- defN 23-May-30 19:17 spm12/amypad_coreg.m
+-rw-r--r--  2.0 unx      186 b- defN 23-May-30 19:17 spm12/amypad_coreg_modify_affine.m
+-rw-r--r--  2.0 unx      421 b- defN 23-May-30 19:17 spm12/amypad_normw.m
+-rw-r--r--  2.0 unx      641 b- defN 23-May-30 19:17 spm12/amypad_resample.m
+-rw-r--r--  2.0 unx     1792 b- defN 23-May-30 19:17 spm12/amypad_seg.m
+-rw-r--r--  2.0 unx      540 b- defN 23-May-30 19:17 spm12/cli.py
+-rw-r--r--  2.0 unx    14056 b- defN 23-May-30 19:17 spm12/regseg.py
+-rw-r--r--  2.0 unx     2675 b- defN 23-May-30 19:17 spm12/utils.py
+-rw-r--r--  2.0 unx      553 b- defN 23-May-30 19:17 spm12-2.1.0.dist-info/LICENCE.md
+-rw-r--r--  2.0 unx     3554 b- defN 23-May-30 19:17 spm12-2.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 19:17 spm12-2.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-May-30 19:17 spm12-2.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-May-30 19:17 spm12-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1448 b- defN 23-May-30 19:17 spm12-2.1.0.dist-info/RECORD
+19 files, 30396 bytes uncompressed, 11150 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,7 +1,13 @@
+Filename: examples/.gitignore
+Comment: 
+
+Filename: examples/demo.ipynb
+Comment: 
+
 Filename: spm12/__init__.py
 Comment: 
 
 Filename: spm12/__main__.py
 Comment: 
 
 Filename: spm12/_dist_ver.py
@@ -27,26 +33,26 @@
 
 Filename: spm12/regseg.py
 Comment: 
 
 Filename: spm12/utils.py
 Comment: 
 
-Filename: spm12-2.0.0.dist-info/LICENCE.md
+Filename: spm12-2.1.0.dist-info/LICENCE.md
 Comment: 
 
-Filename: spm12-2.0.0.dist-info/METADATA
+Filename: spm12-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: spm12-2.0.0.dist-info/WHEEL
+Filename: spm12-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: spm12-2.0.0.dist-info/entry_points.txt
+Filename: spm12-2.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: spm12-2.0.0.dist-info/top_level.txt
+Filename: spm12-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: spm12-2.0.0.dist-info/RECORD
+Filename: spm12-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spm12/__init__.py

```diff
@@ -1,9 +1,9 @@
-from .regseg import *  # NOQA
-from .utils import *  # NOQA
+from .regseg import *  # NOQA, yapf: disable
+from .utils import *  # NOQA, yapf: disable
 
 # version detector. Precedence: installed dist, git, 'UNKNOWN'
 try:
     from ._dist_ver import __version__
 except ImportError:
     try:
         from setuptools_scm import get_version
```

## spm12/__main__.py

```diff
@@ -1,7 +1,7 @@
 #!/usr/bin/env python
 import sys
 
 from .cli import main
 
-if __name__ == "__main__":  # pragma: no cover
+if __name__ == "__main__": # pragma: no cover
     sys.exit(main(sys.argv[1:]))
```

## spm12/_dist_ver.py

```diff
@@ -1 +1 @@
-__version__ = '2.0.0'
+__version__ = '2.1.0'
```

## spm12/amypad_normw.m

```diff
@@ -1,11 +1,13 @@
 function out = amypad_normw(def_file, flist4norm, voxsz, intrp, bbox)
     job.subj.def = {def_file};
     job.subj.resample = flist4norm;
     %job.woptions.bb = [NaN, NaN, NaN; NaN, NaN, NaN];
     job.woptions.bb = bbox;
-    job.woptions.vox = [voxsz, voxsz, voxsz];
+    job.woptions.vox = voxsz; %[voxsz, voxsz, voxsz];
     job.woptions.interp = intrp;
     job.woptions.prefix = 'w';
+
+    addpath(fullfile(spm('Dir'),'config'));
     spm_run_norm(job);
     out=0;
 end
```

## spm12/cli.py

```diff
@@ -12,9 +12,9 @@
 from .utils import ensure_spm
 
 
 def main(argv=None):
     logging.basicConfig(level=logging.DEBUG, format="%(levelname)s:%(funcName)s:%(message)s")
     args = argopt(__doc__).parse_args(argv)
     ensure_spm(cache=args.cache, version=args.spm_version)
-    print("SPM{v} is successfully installed".format(v=args.spm_version))
+    print(f"SPM{args.spm_version} is successfully installed")
     return 0
```

## spm12/regseg.py

```diff
@@ -1,12 +1,13 @@
 import errno
 import logging
 import os
 import re
 import shutil
+from numbers import Number
 from pathlib import PurePath
 from textwrap import dedent
 
 import numpy as np
 import scipy.ndimage as ndi
 from miutil import create_dir, hasext
 from miutil.imio import nii
@@ -30,28 +31,27 @@
     """
     glob with regular expressions
     """
     return (os.path.join(pth, f) for f in os.listdir(pth) if re.match(pttrn, f))
 
 
 def fwhm2sig(fwhm, voxsize=2.0):
-    return fwhm / (voxsize * (8 * np.log(2)) ** 0.5)
+    return fwhm / (voxsize * (8 * np.log(2))**0.5)
 
 
 def smoothim(fim, fwhm=4, fout=""):
     """
     Smooth image using Gaussian filter with FWHM given as an option.
     """
     imd = nii.getnii(fim, output="all")
-    imsmo = ndi.filters.gaussian_filter(
-        imd["im"], fwhm2sig(fwhm, voxsize=imd["voxsize"]), mode="constant"
-    )
+    imsmo = ndi.filters.gaussian_filter(imd["im"], fwhm2sig(fwhm, voxsize=imd["voxsize"]),
+                                        mode="constant")
     if not fout:
         f = nii.file_parts(fim)
-        fout = os.path.join(f[0], "{}_smo{}{}".format(f[1], str(fwhm).replace(".", "-"), f[2]))
+        fout = os.path.join(f[0], f"{f[1]}_smo{str(fwhm).replace('.', '-')}{f[2]}")
     nii.array2nii(
         imsmo,
         imd["affine"],
         fout,
         trnsp=(
             imd["transpose"].index(0),
             imd["transpose"].index(1),
@@ -71,39 +71,36 @@
         niidct = nii.getnii(fnii, output="all")
     elif isinstance(fnii, dict) and "hdr" in fnii:
         niidct = fnii
     else:
         raise ValueError("incorrect input NIfTI file/dictionary")
 
     dim = niidct["hdr"]["dim"]
-    corners = np.array(
-        [
-            [1, 1, 1, 1],
-            [1, 1, dim[3], 1],
-            [1, dim[2], 1, 1],
-            [1, dim[2], dim[3], 1],
-            [dim[1], 1, 1, 1],
-            [dim[1], 1, dim[3], 1],
-            [dim[1], dim[2], 1, 1],
-            [dim[1], dim[2], dim[3], 1],
-        ]
-    )
+    corners = np.array([[1, 1, 1, 1], [1, 1, dim[3], 1], [1, dim[2], 1, 1], [1, dim[2], dim[3], 1],
+                        [dim[1], 1, 1, 1], [dim[1], 1, dim[3], 1], [dim[1], dim[2], 1, 1],
+                        [dim[1], dim[2], dim[3], 1]])
 
     XYZ = np.dot(niidct["affine"][:3, :], corners.T)
 
     # FIXME: weird correction for SPM bounding box (??)
     crr = np.dot(niidct["affine"][:3, :3], [1, 1, 1])
 
     # bounding box as matrix
     bbox = np.concatenate((np.min(XYZ, axis=1) - crr, np.max(XYZ, axis=1) - crr))
     bbox.shape = (2, 3)
 
     return bbox
 
 
+def mat2array(matlab_mat):
+    if hasattr(matlab_mat, '_data'): # matlab<R2022a
+        return np.array(matlab_mat._data).reshape(matlab_mat.size, order='F')
+    return np.array(matlab_mat)
+
+
 def coreg_spm(
     imref,
     imflo,
     matlab_eng_name="",
     fwhm_ref=0,
     fwhm_flo=0,
     outpath="",
@@ -130,31 +127,22 @@
       fwhm_ref: FWHM of the smoothing kernel for the reference image
       fwhm_flo: FWHM of the smoothing kernel for the reference image
       modify_nii: modifies the affine of the NIfTI file of the floating
         image according to the rigid body transformation.
     """
     out = {}  # output dictionary
     sep = sep or [4, 2]
+
     tol = tol or [
-        0.0200,
-        0.0200,
-        0.0200,
-        0.0010,
-        0.0010,
-        0.0010,
-        0.0100,
-        0.0100,
-        0.0100,
-        0.0010,
-        0.0010,
-        0.0010,
-    ]
+        0.0200, 0.0200, 0.0200, 0.0010, 0.0010, 0.0010, 0.0100, 0.0100, 0.0100, 0.0010, 0.0010,
+        0.0010]
+
     fwhm = fwhm or [7, 7]
     params = params or [0, 0, 0, 0, 0, 0]
-    eng = ensure_spm(matlab_eng_name)  # get_matlab
+    eng = ensure_spm(matlab_eng_name) # get_matlab
 
     if not outpath and fname_aff and "/" in fname_aff:
         opth = os.path.dirname(fname_aff) or os.path.dirname(imflo)
         fname_aff = os.path.basename(fname_aff)
     else:
         opth = outpath or os.path.dirname(imflo)
     log.debug("output path:%s", opth)
@@ -169,18 +157,15 @@
         shutil.copyfile(imref, imrefu)
 
     if fwhm_ref > 0:
         smodct = smoothim(imrefu, fwhm_ref)
         # delete the previous version (non-smoothed)
         os.remove(imrefu)
         imrefu = smodct["fim"]
-
-        log.info(
-            "smoothed the reference image with FWHM={} and saved to\n{}".format(fwhm_ref, imrefu)
-        )
+        log.info("smoothed the reference image with FWHM=%r and saved to\n%r", fwhm_ref, imrefu)
 
     # floating
     if hasext(imflo, "gz"):
         imflou = nii.nii_ugzip(imflo, outpath=opth)
     else:
         fnm = nii.file_parts(imflo)[1] + "_copy.nii"
         imflou = os.path.join(opth, fnm)
@@ -193,17 +178,15 @@
             os.remove(imflou)
         else:
             # save the uncompressed and unsmoothed version
             imflou_ = imflou
 
         imflou = smodct["fim"]
 
-        log.info(
-            "smoothed the floating image with FWHM={} and saved to\n{}".format(fwhm_flo, imflou)
-        )
+        log.info("smoothed the floating image with FWHM=%r and saved to\n%r", fwhm_flo, imflou)
 
     # run the MATLAB SPM registration
     import matlab as ml
 
     Mm, xm = eng.amypad_coreg(
         imrefu,
         imflou,
@@ -219,19 +202,18 @@
 
     # modify the affine of the floating image (as usually done in SPM)
     if modify_nii:
         eng.amypad_coreg_modify_affine(imflou_, Mm)
         out["freg"] = imflou_
 
     # get the affine matrix
-    M = np.array(Mm._data.tolist())
-    M = M.reshape(4, 4).T
+    M = mat2array(Mm)
 
     # get the translation and rotation parameters in a vector
-    x = np.array(xm._data.tolist())
+    x = mat2array(xm)
 
     # delete the uncompressed files
     if del_uncmpr:
         os.remove(imrefu)
         os.remove(imflou)
 
     create_dir(os.path.join(opth, "affine-spm"))
@@ -288,24 +270,24 @@
     prefix="r_",
     pickname="ref",
     del_ref_uncmpr=False,
     del_flo_uncmpr=False,
     del_out_uncmpr=False,
 ):
     log.debug(
-        dedent(
-            """\
+        dedent("""\
         ======================================================================
          S P M  inputs:
-         > ref:' {}
-         > flo:' {}
-        ======================================================================"""
-        ).format(imref, imflo)
+         > ref:' %r
+         > flo:' %r
+        ======================================================================"""),
+        imref,
+        imflo,
     )
-    eng = ensure_spm(matlab_eng_name)  # get_matlab
+    eng = ensure_spm(matlab_eng_name) # get_matlab
 
     if not outpath and fimout:
         opth = os.path.dirname(fimout) or os.path.dirname(imflo)
     else:
         opth = outpath or os.path.dirname(imflo)
     log.debug("output path:%s", opth)
     create_dir(opth)
@@ -381,19 +363,15 @@
             "affine_flo-" + nii.file_parts(imflo)[1] + fcomment + ".nii.gz",
         )
     # change the file name
     os.rename(fim + ".gz", fout)
 
     if fwhm > 0:
         smodct = smoothim(fout, fwhm)
-        log.info(
-            "smoothed the resampled image with FWHM={} and saved to\n{}".format(
-                fwhm, smodct["fim"]
-            )
-        )
+        log.info("smoothed the resampled image with FWHM=%r and saved to\n%r", fwhm, smodct["fim"])
 
     return fout
 
 
 def seg_spm(
     f_mri,
     spm_path=None,
@@ -414,19 +392,19 @@
       matlab_eng_name: name of the Python engine for Matlab.
       outpath: output folder path for the normalisation file output
       store_nat_*: stores native space segmentation output for either
         grey matter, white matter or CSF
       sotre_fwd/inv: stores forward/inverse normalisation definitions
       visual: shows the Matlab window progress
     """
-    out = {}  # output dictionary
-    # get Matlab engine or use the provided one
-    eng = ensure_spm(matlab_eng_name)
+    out = {}                          # output dictionary
+    eng = ensure_spm(matlab_eng_name) # get Matlab engine or use the provided one
     if not spm_path:
         spm_path = spm_dir()
+
     # run SPM normalisation/segmentation
     param, invdef, fordef = eng.amypad_seg(
         f_mri,
         str(spm_path),
         float(store_nat_gm),
         float(store_nat_wm),
         float(store_nat_csf),
@@ -436,15 +414,16 @@
         nargout=3,
     )
     if outpath is not None:
         create_dir(outpath)
         out["param"] = move_files(param, outpath)
         out["invdef"] = move_files(invdef, outpath)
         out["fordef"] = move_files(fordef, outpath)
-        # go through tissue types and move them to the output folder
+
+        # move each tissue type to the output folder
         for c in glob_match(r"c\d*", os.path.dirname(param)):
             nm = os.path.basename(c)[:2]
             out[nm] = move_files(c, outpath)
     else:
         out["param"] = param
         out["invdef"] = invdef
         out["fordef"] = fordef
@@ -475,23 +454,32 @@
     elif isinstance(bbox, np.ndarray) and bbox.shape == (2, 3):
         bb = ml.double(bbox.tolist())
     elif isinstance(bbox, list) and len(bbox) == 2:
         bb = ml.double(bbox)
     else:
         raise ValueError("unrecognised format for bounding box")
 
-    eng = ensure_spm(matlab_eng_name)  # get_matlab
-    eng.amypad_normw(f_def, files4norm, float(voxsz), float(intrp), bb)
-    out = []  # output list
+    if isinstance(voxsz, Number):
+        voxsz = ml.double([voxsz] * 3)
+    elif isinstance(voxsz, (np.ndarray, list)):
+        if len(voxsz) != 3:
+            raise ValueError(f"voxel size ({voxsz}) should be scalar or 3-vector")
+        voxsz = ml.double(np.float64(voxsz))
+    else:
+        raise ValueError(f"voxel size ({voxsz}) should be scalar or 3-vector")
+
+    eng = ensure_spm(matlab_eng_name) # get_matlab
+    eng.amypad_normw(f_def, files4norm, voxsz, float(intrp), bb)
+    out = []                          # output list
+
     if outpath is not None:
         create_dir(outpath)
         for f in files4norm:
             fpth = f.split(",")[0]
             out.append(
                 move_files(
                     os.path.join(os.path.dirname(fpth), "w" + os.path.basename(fpth)),
                     outpath,
-                )
-            )
+                ))
     else:
         out.append("w" + os.path.basename(f.split(",")[0]))
     return out
```

## spm12/utils.py

```diff
@@ -1,63 +1,79 @@
 import logging
 from functools import lru_cache, wraps
-from os import path
+from os import fspath, path
 from textwrap import dedent
 
 from miutil.fdio import extractall
 from miutil.mlab import get_engine
 from miutil.web import urlopen_cached
-from pkg_resources import resource_filename
 
-__all__ = ["ensure_spm", "get_matlab", "spm_dir"]
-PATH_M = resource_filename(__name__, "")
+try:          # py<3.9
+    import importlib_resources as resources
+except ImportError:
+    from importlib import resources
+
+__all__ = ["ensure_spm", "get_matlab", "spm_dir", "spm_dir_eng"]
+PATH_M = fspath(resources.files("spm12").resolve())
 log = logging.getLogger(__name__)
 
 
-@lru_cache()
 def get_matlab(name=None):
     eng = get_engine(name=name)
     log.debug("adding wrappers (%s) to MATLAB path", PATH_M)
     eng.addpath(PATH_M, nargout=0)
     return eng
 
 
 def spm_dir(cache="~/.spm12", version=12):
+    """Internal SPM12 directory"""
     cache = path.expanduser(cache)
     if str(version) != "12":
         raise NotImplementedError
     return path.join(cache, "spm12")
 
 
+def spm_dir_eng(name=None, cache="~/.spm12", version=12):
+    """
+    Computed SPM12 directory.
+    Uses matlab to find SPM12 directly,
+    so may prefer user-installed version to the internal `spm_dir`.
+    """
+    eng = ensure_spm(name=name, cache=cache, version=version)
+    return path.dirname(eng.which("spm_jobman"))
+
+
 @lru_cache()
 @wraps(get_matlab)
 def ensure_spm(name=None, cache="~/.spm12", version=12):
     eng = get_matlab(name)
     cache = path.expanduser(cache)
     addpath = spm_dir(cache=cache, version=version)
     if path.exists(addpath):
         eng.addpath(addpath)
     if not eng.exist("spm_jobman"):
         log.warning("MATLAB could not find SPM.")
         try:
             log.info("Downloading to %s", cache)
             with urlopen_cached(
-                "https://www.fil.ion.ucl.ac.uk/spm/download/restricted/eldorado/spm12.zip",
-                cache,
+                    "https://www.fil.ion.ucl.ac.uk/spm/download/restricted/eldorado/spm12.zip",
+                    cache,
             ) as fd:
                 extractall(fd, cache)
             eng.addpath(addpath)
             if not eng.exist("spm_jobman"):
                 raise RuntimeError("MATLAB could not find SPM.")
             log.info("Installed")
-        except:  # NOQA: E722,B001
+        except:                # NOQA: E722,B001
             raise ImportError(
-                dedent(
-                    """\
+                dedent("""\
                 MATLAB could not find SPM.
                 Please follow installation instructions at
                 https://en.wikibooks.org/wiki/SPM/Download
                 Make sure to add SPM to MATLAB's path using `startup.m`
-                """
-                )
-            )
+                """))
+
+    found = eng.which("spm_jobman")
+    if path.realpath(path.dirname(found)) != path.realpath(addpath):
+        log.warning(f"Internal ({addpath}) does not match detected ({found}) SPM12.\n"
+                    "This means `spm_dir()` is likely to fail - use `spm_dir_eng()` instead.")
     return eng
```

## Comparing `spm12-2.0.0.dist-info/LICENCE.md` & `spm12-2.1.0.dist-info/LICENCE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2020 AMYPAD
+Copyright 2020-23 AMYPAD
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this project except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

## Comparing `spm12-2.0.0.dist-info/METADATA` & `spm12-2.1.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,53 @@
 Metadata-Version: 2.1
 Name: spm12
-Version: 2.0.0
+Version: 2.1.0
 Summary: Statistical Parametric Mapping
-Home-page: https://github.com/AMYPAD/SPM12
-Maintainer: Casper da Costa-Luis
-Maintainer-email: casper.dcl@physics.org
-License: Apache 2.0
-Project-URL: Changelog, https://github.com/AMYPAD/SPM12/releases
-Project-URL: Documentation, https://github.com/AMYPAD/SPM12/#SPM12
-Project-URL: Upstream Project, https://www.fil.ion.ucl.ac.uk/spm
+Maintainer-email: Casper da Costa-Luis <casper.dcl@physics.org>
+License: Apache-2.0
+Project-URL: documentation, https://github.com/AMYPAD/SPM12/#SPM12
+Project-URL: repository, https://github.com/AMYPAD/SPM12
+Project-URL: changelog, https://github.com/AMYPAD/SPM12/releases
+Project-URL: upstream-project, https://www.fil.ion.ucl.ac.uk/spm
 Keywords: fMRI,PET,SPECT,EEG,MEG
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Other Scripting Engines
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Installation/Setup
-Provides: spm12
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENCE.md
 Requires-Dist: argopt
-Requires-Dist: miutil[nii,web] (>=0.7.2)
-Requires-Dist: setuptools
+Requires-Dist: miutil[nii,web] (>=0.12.0)
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: importlib-resources ; python_version < "3.9"
 Provides-Extra: demo
 Requires-Dist: miutil[plot] (>=0.3.0) ; extra == 'demo'
 Requires-Dist: matplotlib ; extra == 'demo'
 Provides-Extra: dev
-Requires-Dist: pre-commit ; extra == 'dev'
-Requires-Dist: twine ; extra == 'dev'
-Requires-Dist: wheel ; extra == 'dev'
-Requires-Dist: pytest ; extra == 'dev'
+Requires-Dist: pytest (>=6) ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
 Requires-Dist: pytest-timeout ; extra == 'dev'
 Requires-Dist: pytest-xdist ; extra == 'dev'
-Requires-Dist: codecov ; extra == 'dev'
 
 SPM12
 =====
 
 |Version| |Py-Versions| |Tests| |Coverage| |DOI| |LICENCE|
 
 Thin Python wrappers around `Statistical Parametric Mapping <https://www.fil.ion.ucl.ac.uk/spm>`_.
@@ -79,17 +73,16 @@
 
 
 Contributing
 ------------
 
 See `CONTRIBUTING.md <https://github.com/AMYPAD/SPM12/blob/master/CONTRIBUTING.md>`_.
 
-
 .. |PET-MR Coregistration| image:: https://raw.githubusercontent.com/AMYPAD/images/master/spm12/pet_mr_coreg.png
-.. |Tests| image:: https://img.shields.io/github/workflow/status/AMYPAD/SPM12/Test?logo=GitHub
+.. |Tests| image:: https://img.shields.io/github/actions/workflow/status/AMYPAD/SPM12/test.yml?branch=master&logo=GitHub
    :target: https://github.com/AMYPAD/SPM12/actions
 .. |Coverage| image:: https://codecov.io/gh/AMYPAD/SPM12/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/AMYPAD/SPM12
 .. |Version| image:: https://img.shields.io/pypi/v/spm12.svg?logo=python&logoColor=white
    :target: https://github.com/AMYPAD/SPM12/releases
 .. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/spm12.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/spm12
```

## Comparing `spm12-2.0.0.dist-info/RECORD` & `spm12-2.1.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-spm12/__init__.py,sha256=Tq48sTZpJmUNx7D6ckLVfIJT24f6P_CQ1vU4ZDg9pu4,382
-spm12/__main__.py,sha256=BuuN_ZIxBZcdvg8wt2ZvdIZueVaXyJWpA1IIZi-74Is,137
-spm12/_dist_ver.py,sha256=hwOJuFUEKtsgiOt4l6op9s-hviovM6TK1uCdtRNWY4E,22
+examples/.gitignore,sha256=EMiOSbZgGk3pq6vm0ZoPBxgkgQmaQNlNGYUwy673cis,49
+examples/demo.ipynb,sha256=Pxpk1owEAu_T6oNwjLAKfi7ZVss3Baf4Sf4UepEo9Z0,2982
+spm12/__init__.py,sha256=vv-iogI_KS6Nx3wqf85_U0GoxEeAVEeoVHwPjc33Tao,412
+spm12/__main__.py,sha256=BQhjKDjUxrc-wcT5a7zn0re4kX9ZE94tqc6MlyfZrCM,136
+spm12/_dist_ver.py,sha256=LbU43-7hsLmdXWI0wTAl3y6D3Tr7CbJiDOLXwl7clj8,22
 spm12/amypad_coreg.m,sha256=OQipnQFpeT0lMMMPMbXy_NRBbh0G1tAT5_0Ul1prGVg,776
 spm12/amypad_coreg_modify_affine.m,sha256=3cf6pKtb5HU082UqziLxQnHGa-Z_SSi6IdObMQPgJNY,186
-spm12/amypad_normw.m,sha256=Zh3DMvEQcuT4pGBj8rWMEe0xB15GjbRJd0EKSqFySwQ,368
+spm12/amypad_normw.m,sha256=XKWT1LhPsZooE1nSCFW8OUwzWZqzM7cihf-DHhlut4c,421
 spm12/amypad_resample.m,sha256=Snmtg6541js52Fc8ASJrA9yQxsLpJhWHMCuF54xgyw0,641
 spm12/amypad_seg.m,sha256=h16FGQTZx8oUD0Os1Ux95F6q8Ar752FQfqW_MePNwtA,1792
-spm12/cli.py,sha256=lQ1H-htP_DUrY05Eq46M7LxOdNk6DRPyt1tL8cCTMV0,551
-spm12/regseg.py,sha256=0lShkdCyrKee-FD30Tpqd10wIMD3PUcahXEl31RaxWc,13791
-spm12/utils.py,sha256=mRbiHNfqQdwd0ltay9A0n1TZJ4SixrRQ0gwz9OHkZUw,1955
-spm12-2.0.0.dist-info/LICENCE.md,sha256=TzsQFOqgBCdjDy7PkwtmP-jGs6V2sYZ0KIyCpsWBBnQ,550
-spm12-2.0.0.dist-info/METADATA,sha256=n37MtY3N3onQjeDShoTqPfwEfeCBlo0aiNiRxD8KJaU,3616
-spm12-2.0.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-spm12-2.0.0.dist-info/entry_points.txt,sha256=QchkM9vFZxYhd5u4W9_THAjq98GIFPhO6gGmv-5O-0s,41
-spm12-2.0.0.dist-info/top_level.txt,sha256=T8iVTXHUwKi7ZV3HDqKqGKTPUXffKgcFnuDARyP95nU,6
-spm12-2.0.0.dist-info/RECORD,,
+spm12/cli.py,sha256=OblCFA-ZMHzNRLuB3Y_w8bsSlBv-9U5RMnT3KMEhfbg,540
+spm12/regseg.py,sha256=KLN-Kkl0YstDRiedsqLAKjgLkTZ-r8ohnOVpTVYigzo,14056
+spm12/utils.py,sha256=9-_HF0VE2pgbcZfoGNpVR1pJrfKERIxwNW2kFrpGOkM,2675
+spm12-2.1.0.dist-info/LICENCE.md,sha256=VuhEbQOH7mj1ll9Nhfp2F1dEY8gtQZvPkWpsdSOvqSo,553
+spm12-2.1.0.dist-info/METADATA,sha256=z7Z8tZ19roxRtuWJfxbBmN6fKpDfqw5oB7IfXFxD8sI,3554
+spm12-2.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spm12-2.1.0.dist-info/entry_points.txt,sha256=QchkM9vFZxYhd5u4W9_THAjq98GIFPhO6gGmv-5O-0s,41
+spm12-2.1.0.dist-info/top_level.txt,sha256=SDcw0wfgSfrD-bRUnLRzcwWcq5caq0DczzJ45HcMHD4,20
+spm12-2.1.0.dist-info/RECORD,,
```

