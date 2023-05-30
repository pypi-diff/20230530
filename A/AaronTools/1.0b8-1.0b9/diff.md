# Comparing `tmp/AaronTools-1.0b8.tar.gz` & `tmp/AaronTools-1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AaronTools-1.0b8.tar", last modified: Mon Mar 22 19:09:36 2021, max compression
+gzip compressed data, was "AaronTools-1.0b9.tar", last modified: Tue Apr 20 16:16:33 2021, max compression
```

## Comparing `AaronTools-1.0b8.tar` & `AaronTools-1.0b9.tar`

### file list

```diff
@@ -1,400 +1,1867 @@
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.345226 AaronTools-1.0b8/
--rw-r--r--   0 deo       (1000) users      (985)      145 2021-03-11 23:11:08.000000 AaronTools-1.0b8/.gitignore
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.308559 AaronTools-1.0b8/AaronTools.egg-info/
--rw-r--r--   0 deo       (1000) users      (985)     2430 2021-03-22 19:09:36.000000 AaronTools-1.0b8/AaronTools.egg-info/PKG-INFO
--rw-r--r--   0 deo       (1000) users      (985)     9484 2021-03-22 19:09:36.000000 AaronTools-1.0b8/AaronTools.egg-info/SOURCES.txt
--rw-r--r--   0 deo       (1000) users      (985)        1 2021-03-22 19:09:36.000000 AaronTools-1.0b8/AaronTools.egg-info/dependency_links.txt
--rw-r--r--   0 deo       (1000) users      (985)       38 2021-03-22 19:09:36.000000 AaronTools-1.0b8/AaronTools.egg-info/requires.txt
--rw-r--r--   0 deo       (1000) users      (985)       11 2021-03-22 19:09:36.000000 AaronTools-1.0b8/AaronTools.egg-info/top_level.txt
--rw-r--r--   0 deo       (1000) users      (985)    35149 2020-09-09 16:20:38.000000 AaronTools-1.0b8/LICENSE
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.315226 AaronTools-1.0b8/Ligands/
--rw-r--r--   0 deo       (1000) users      (985)      272 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/ACN.xyz
--rw-r--r--   0 deo       (1000) users      (985)      627 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/AcAc.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2346 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Ad-HC5C.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1071 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/BDA.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1419 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/BPE.xyz
--rw-r--r--   0 deo       (1000) users      (985)      892 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/BPY.xyz
--rw-r--r--   0 deo       (1000) users      (985)      980 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/BenQuin.xyz
--rw-r--r--   0 deo       (1000) users      (985)      822 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/BiOX.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1236 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/BiOx_Me.xyz
--rw-r--r--   0 deo       (1000) users      (985)       96 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/CO.xyz
--rw-r--r--   0 deo       (1000) users      (985)      897 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/COD.xyz
--rw-r--r--   0 deo       (1000) users      (985)      455 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Cp.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1117 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Cp_star.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1156 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/DMBPY.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1243 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/DMP.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1067 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/DMPE.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2961 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/DPEphos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2299 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/DPPE.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2871 2020-11-11 15:56:35.000000 AaronTools-1.0b8/Ligands/DPPF.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2431 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/DPPP.xyz
--rw-r--r--   0 deo       (1000) users      (985)      540 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/EDA.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2077 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/IMes.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1993 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/JoshPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3617 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/KASBAI.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1578 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Mes-NC5C.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2170 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Milstein.xyz
--rw-r--r--   0 deo       (1000) users      (985)      675 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/NBD.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1074 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/PHNNP.xyz
--rw-r--r--   0 deo       (1000) users      (985)      891 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/PIN.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1539 2020-06-24 20:42:33.000000 AaronTools-1.0b8/Ligands/PPh3.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1898 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Paton_DL.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1946 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Paton_EL.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3973 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/PhBP3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      964 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/PymdOx.xyz
--rw-r--r--   0 deo       (1000) users      (985)      867 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/PyrOx.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3445 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R-BINAP.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3905 2019-11-13 15:52:13.000000 AaronTools-1.0b8/Ligands/R-Me-StackPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2079 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R-Ph-BOX.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3309 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R-Ph-Mes-NC5C.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2922 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R-Quinox-AdtBu2.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2607 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R-Quinox-tBu3.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4186 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R-SEGPHOS.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4732 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R-StackPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1995 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R-iPr-PyBOX.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4731 2019-11-13 15:52:13.000000 AaronTools-1.0b8/Ligands/R-pFPh-StackPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R-tBu-BOX.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2695 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-BDPP.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-BPCp.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2651 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-Et-DuPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1947 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-Me-BPE.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2123 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-Me-DuPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1248 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-Me-TBF.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3221 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-Me-iPrPh-NC5C.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2210 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-QuinoxP.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3179 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-iPr-DuPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2695 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RR-norphos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2563 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/RRSS-DuanPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     5009 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/R_temp.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3445 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/S-BINAP.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2915 2019-11-13 15:52:13.000000 AaronTools-1.0b8/Ligands/S-Me-StackPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2079 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/S-Ph-BOX.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3309 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/S-Ph-Mes-NC5C.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3135 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/S-Quinox-AdtBu2.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2607 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/S-Quinox-tBu3.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3178 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/S-SEGPHOS.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3532 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/S-StackPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1995 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/S-iPr-PyBOX.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3531 2019-11-13 15:52:13.000000 AaronTools-1.0b8/Ligands/S-pFPh-StackPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/S-tBu-BOX.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2095 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SL-J212-1.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3047 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SL-J212-2.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2695 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SS-BDPP.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SS-BPCp.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2651 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SS-Et-DuPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1947 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SS-Me-BPE.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2123 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SS-Me-DuPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1248 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SS-Me-TBF.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3221 2019-11-15 16:33:28.000000 AaronTools-1.0b8/Ligands/SS-Me-iPrPh-NC5C.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2210 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SS-QuinoxP.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3179 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SS-iPr-DuPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2695 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SS-norphos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2563 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/SSRR-DuanPhos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1069 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/TACN.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1070 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/TACN_star.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1316 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Tp.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3269 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Xantphos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3661 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/Xphos.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2101 2020-06-24 20:42:33.000000 AaronTools-1.0b8/Ligands/achiral_ligands
--rw-r--r--   0 deo       (1000) users      (985)     1709 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/bi-isoquinoline-NN-dioxide.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3012 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/chiral_ligands
--rw-r--r--   0 deo       (1000) users      (985)     1839 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/dithiolate-4F.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1989 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/iPr-NC3C.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2477 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/iPr-PNPEt.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3491 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/iPrPh-BIP.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2957 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/iPrPh-NC5C.xyz
--rw-r--r--   0 deo       (1000) users      (985)       53 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/organocatalysts
--rw-r--r--   0 deo       (1000) users      (985)     3550 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/squaramide-iPr.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3028 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/squaramide.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3049 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/tBu-PCP.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3181 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Ligands/tBu-PNPPyr.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2430 2021-03-22 19:09:36.345226 AaronTools-1.0b8/PKG-INFO
--rw-r--r--   0 deo       (1000) users      (985)     1272 2021-01-17 15:33:35.000000 AaronTools-1.0b8/README.md
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.315226 AaronTools-1.0b8/Rings/
--rw-r--r--   0 deo       (1000) users      (985)      595 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/benzene.xyz
--rw-r--r--   0 deo       (1000) users      (985)      891 2021-03-11 23:11:08.000000 AaronTools-1.0b8/Rings/cyclohexane.1.xyz
--rw-r--r--   0 deo       (1000) users      (985)      891 2021-03-11 23:11:08.000000 AaronTools-1.0b8/Rings/cyclohexane.xyz
--rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentadiene.1.xyz
--rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentadiene.2.xyz
--rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentadiene.3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentadiene.5.xyz
--rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentadiene.6.xyz
--rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentadiene.7.xyz
--rw-r--r--   0 deo       (1000) users      (985)      730 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentane.1.xyz
--rw-r--r--   0 deo       (1000) users      (985)      730 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentane.2.xyz
--rw-r--r--   0 deo       (1000) users      (985)      730 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentane.3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      730 2020-02-05 23:48:35.000000 AaronTools-1.0b8/Rings/cyclopentane.4.xyz
--rw-r--r--   0 deo       (1000) users      (985)      730 2021-03-11 23:11:08.000000 AaronTools-1.0b8/Rings/cyclopentane.xyz
--rw-r--r--   0 deo       (1000) users      (985)      416 2021-03-11 23:11:08.000000 AaronTools-1.0b8/Rings/m-pyridine.xyz
--rw-r--r--   0 deo       (1000) users      (985)      601 2021-03-11 23:11:08.000000 AaronTools-1.0b8/Rings/m-tetrahydropyran.1.xyz
--rw-r--r--   0 deo       (1000) users      (985)      601 2021-03-11 23:11:08.000000 AaronTools-1.0b8/Rings/m-tetrahydropyran.xyz
--rw-r--r--   0 deo       (1000) users      (985)      416 2021-03-11 23:11:08.000000 AaronTools-1.0b8/Rings/o-pyridine.xyz
--rw-r--r--   0 deo       (1000) users      (985)      602 2021-03-11 23:11:08.000000 AaronTools-1.0b8/Rings/o-tetrahydropyran.1.xyz
--rw-r--r--   0 deo       (1000) users      (985)      602 2021-03-11 23:11:08.000000 AaronTools-1.0b8/Rings/o-tetrahydropyran.xyz
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.318559 AaronTools-1.0b8/Substituents/
--rw-r--r--   0 deo       (1000) users      (985)      649 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/26-F-Ph.xyz
--rw-r--r--   0 deo       (1000) users      (985)      649 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/35-F-Ph.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1112 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/Ad.xyz
--rw-r--r--   0 deo       (1000) users      (985)      145 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/BF2.xyz
--rw-r--r--   0 deo       (1000) users      (985)       53 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/Br.xyz
--rw-r--r--   0 deo       (1000) users      (985)      144 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CCH.xyz
--rw-r--r--   0 deo       (1000) users      (985)      175 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CF3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      188 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CH2Cl.xyz
--rw-r--r--   0 deo       (1000) users      (985)      187 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CH2F.xyz
--rw-r--r--   0 deo       (1000) users      (985)      236 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CH2OH.xyz
--rw-r--r--   0 deo       (1000) users      (985)      185 2020-10-01 20:48:29.000000 AaronTools-1.0b8/Substituents/CH3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      231 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CHCH2.xyz
--rw-r--r--   0 deo       (1000) users      (985)      189 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CHCl2.xyz
--rw-r--r--   0 deo       (1000) users      (985)      187 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CHF2.xyz
--rw-r--r--   0 deo       (1000) users      (985)      146 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CHO.xyz
--rw-r--r--   0 deo       (1000) users      (985)       99 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/CN.xyz
--rw-r--r--   0 deo       (1000) users      (985)      281 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/COCH3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      326 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/COOCH3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      191 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/COOH.xyz
--rw-r--r--   0 deo       (1000) users      (985)       53 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/Cl.xyz
--rw-r--r--   0 deo       (1000) users      (985)      760 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/Cy.xyz
--rw-r--r--   0 deo       (1000) users      (985)      417 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/Et.xyz
--rw-r--r--   0 deo       (1000) users      (985)       54 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/F.xyz
--rw-r--r--   0 deo       (1000) users      (985)       54 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/H.xyz
--rw-r--r--   0 deo       (1000) users      (985)       53 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/I.xyz
--rw-r--r--   0 deo       (1000) users      (985)      185 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/Me.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1191 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/Mes.xyz
--rw-r--r--   0 deo       (1000) users      (985)      416 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/NCH3_2.xyz
--rw-r--r--   0 deo       (1000) users      (985)      146 2019-11-15 16:33:28.000000 AaronTools-1.0b8/Substituents/NH2.xyz
--rw-r--r--   0 deo       (1000) users      (985)      281 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/NHCH3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      191 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/NHOH.xyz
--rw-r--r--   0 deo       (1000) users      (985)      101 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/NO.xyz
--rw-r--r--   0 deo       (1000) users      (985)      146 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/NO2.xyz
--rw-r--r--   0 deo       (1000) users      (985)       52 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/O.xyz
--rw-r--r--   0 deo       (1000) users      (985)      236 2019-11-15 16:33:28.000000 AaronTools-1.0b8/Substituents/OCF3.xyz
--rw-r--r--   0 deo       (1000) users      (985)       99 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/OH.xyz
--rw-r--r--   0 deo       (1000) users      (985)      236 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/OMe.xyz
--rw-r--r--   0 deo       (1000) users      (985)      506 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/Ph.xyz
--rw-r--r--   0 deo       (1000) users      (985)      236 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/SCH3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      101 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/SH.xyz
--rw-r--r--   0 deo       (1000) users      (985)      190 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/SiF3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      190 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/SiH3.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2126 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/SuperMes.xyz
--rw-r--r--   0 deo       (1000) users      (985)      462 2019-05-29 22:58:18.000000 AaronTools-1.0b8/Substituents/iPr.xyz
--rw-r--r--   0 deo       (1000) users      (985)      209 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/subs
--rw-r--r--   0 deo       (1000) users      (985)      596 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/tBu.xyz
--rw-r--r--   0 deo       (1000) users      (985)      325 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/triazole_C.xyz
--rw-r--r--   0 deo       (1000) users      (985)      325 2019-05-08 20:00:01.000000 AaronTools-1.0b8/Substituents/triazole_N.xyz
--rwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-11 23:11:08.000000 AaronTools-1.0b8/__init__.py
--rw-r--r--   0 deo       (1000) users      (985)    22391 2021-03-11 23:11:08.000000 AaronTools-1.0b8/atoms.py
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.321892 AaronTools-1.0b8/bin/
--rwxr-xr-x   0 deo       (1000) users      (985)     4611 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/angle.py
--rwxr-xr-x   0 deo       (1000) users      (985)     4060 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/bond.py
--rwxr-xr-x   0 deo       (1000) users      (985)    10809 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/changeChirality.py
--rwxr-xr-x   0 deo       (1000) users      (985)     4431 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/changeElement.py
--rwxr-xr-x   0 deo       (1000) users      (985)     3338 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/closeRing.py
--rwxr-xr-x   0 deo       (1000) users      (985)     3677 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/coneAngle.py
--rwxr-xr-x   0 deo       (1000) users      (985)     4894 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/dihedral.py
--rwxr-xr-x   0 deo       (1000) users      (985)     1193 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/fetchMolecule.py
--rwxr-xr-x   0 deo       (1000) users      (985)     8029 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/findAtoms.py
--rwxr-xr-x   0 deo       (1000) users      (985)     7235 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/follow.py
--rwxr-xr-x   0 deo       (1000) users      (985)     2708 2021-03-15 19:37:49.000000 AaronTools-1.0b8/bin/grabStatus.py
--rwxr-xr-x   0 deo       (1000) users      (985)     7351 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/grabThermo.py
--rwxr-xr-x   0 deo       (1000) users      (985)     7592 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/interpolate.py
--rwxr-xr-x   0 deo       (1000) users      (985)     3600 2021-03-19 18:30:22.000000 AaronTools-1.0b8/bin/jobSubmit.py
--rwxr-xr-x   0 deo       (1000) users      (985)     1858 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/libaddLigand.py
--rwxr-xr-x   0 deo       (1000) users      (985)     1531 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/libaddRing.py
--rwxr-xr-x   0 deo       (1000) users      (985)     2430 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/libaddSubstituent.py
--rwxr-xr-x   0 deo       (1000) users      (985)     1056 2021-03-19 18:30:22.000000 AaronTools-1.0b8/bin/listChanges.py
--rwxr-xr-x   0 deo       (1000) users      (985)     8397 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/makeConf.py
--rwxr-xr-x   0 deo       (1000) users      (985)    20887 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/makeInput.py
--rwxr-xr-x   0 deo       (1000) users      (985)     6266 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/mapLigand.py
--rwxr-xr-x   0 deo       (1000) users      (985)     2424 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/mirror.py
--rwxr-xr-x   0 deo       (1000) users      (985)     2979 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/parsePDF.py
--rwxr-xr-x   0 deo       (1000) users      (985)     4960 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/percentVolumeBuried.py
--rwxr-xr-x   0 deo       (1000) users      (985)     1884 2020-11-23 17:42:29.000000 AaronTools-1.0b8/bin/printFreq.py
--rwxr-xr-x   0 deo       (1000) users      (985)     4663 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/printFreqBild.py
--rwxr-xr-x   0 deo       (1000) users      (985)     5112 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/printInfo.py
--rwxr-xr-x   0 deo       (1000) users      (985)     1914 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/printXYZ.py
--rwxr-xr-x   0 deo       (1000) users      (985)     2559 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/removeFragment.py
--rwxr-xr-x   0 deo       (1000) users      (985)     5401 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/rmsdAlign.py
--rwxr-xr-x   0 deo       (1000) users      (985)     7310 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/rotate.py
--rwxr-xr-x   0 deo       (1000) users      (985)     8201 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/stericMap.py
--rwxr-xr-x   0 deo       (1000) users      (985)     3735 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/substituentSterimol.py
--rwxr-xr-x   0 deo       (1000) users      (985)     3840 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/substitute.py
--rwxr-xr-x   0 deo       (1000) users      (985)     5402 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/translate.py
--rwxr-xr-x   0 deo       (1000) users      (985)     6920 2021-03-11 23:11:08.000000 AaronTools-1.0b8/bin/unique.py
--rw-r--r--   0 deo       (1000) users      (985)   405624 2019-10-31 21:17:55.000000 AaronTools-1.0b8/calculated_bond_lengths.json
--rw-r--r--   0 deo       (1000) users      (985)    15752 2021-03-15 19:24:53.000000 AaronTools-1.0b8/comp_output.py
--rw-r--r--   0 deo       (1000) users      (985)    29096 2021-03-11 23:11:08.000000 AaronTools-1.0b8/component.py
--rw-r--r--   0 deo       (1000) users      (985)      527 2021-03-19 20:25:16.000000 AaronTools-1.0b8/config.ini
--rw-r--r--   0 deo       (1000) users      (985)    35476 2021-03-19 19:41:18.000000 AaronTools-1.0b8/config.py
--rw-r--r--   0 deo       (1000) users      (985)    24009 2020-11-23 18:30:14.000000 AaronTools-1.0b8/const.py
--rw-r--r--   0 deo       (1000) users      (985)    75609 2021-03-19 18:26:38.000000 AaronTools-1.0b8/fileIO.py
--rw-r--r--   0 deo       (1000) users      (985)    17203 2021-03-11 23:11:08.000000 AaronTools-1.0b8/finders.py
--rw-r--r--   0 deo       (1000) users      (985)   154190 2021-03-19 19:18:42.000000 AaronTools-1.0b8/geometry.py
--rw-r--r--   0 deo       (1000) users      (985)     9754 2021-03-11 23:11:08.000000 AaronTools-1.0b8/job_control.py
--rw-r--r--   0 deo       (1000) users      (985)    13774 2021-03-19 18:26:38.000000 AaronTools-1.0b8/json_extension.py
--rw-r--r--   0 deo       (1000) users      (985)     7607 2020-11-17 21:43:36.000000 AaronTools-1.0b8/new_fileIO.py
--rw-r--r--   0 deo       (1000) users      (985)    12772 2021-03-11 23:11:08.000000 AaronTools-1.0b8/pathway.py
--rw-r--r--   0 deo       (1000) users      (985)     7006 2021-03-11 23:11:08.000000 AaronTools-1.0b8/ring.py
--rw-r--r--   0 deo       (1000) users      (985)       38 2021-03-22 19:09:36.345226 AaronTools-1.0b8/setup.cfg
--rw-r--r--   0 deo       (1000) users      (985)     8613 2021-03-22 19:01:57.000000 AaronTools-1.0b8/setup.py
--rw-r--r--   0 deo       (1000) users      (985)    31028 2021-03-11 23:11:08.000000 AaronTools-1.0b8/substituent.py
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.325226 AaronTools-1.0b8/test/
--rw-r--r--   0 deo       (1000) users      (985)     4814 2020-12-10 18:23:44.000000 AaronTools-1.0b8/test/__init__.py
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.328559 AaronTools-1.0b8/test/ref_files/
--rw-r--r--   0 deo       (1000) users      (985)     2227 2021-03-19 19:31:36.000000 AaronTools-1.0b8/test/ref_files/HOH_init.json
--rw-r--r--   0 deo       (1000) users      (985)     2653 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/atom.json
--rw-r--r--   0 deo       (1000) users      (985)      893 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/benzene_dimer_ref.xyz
--rw-r--r--   0 deo       (1000) users      (985)      403 2021-03-19 19:31:36.000000 AaronTools-1.0b8/test/ref_files/blank_init.json
--rw-r--r--   0 deo       (1000) users      (985)    23638 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/cat.json
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.328559 AaronTools-1.0b8/test/ref_files/change_chirality_cls/
--rw-r--r--   0 deo       (1000) users      (985)      780 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/ref_files/change_chirality_cls/diastereomer-1.xyz
--rw-r--r--   0 deo       (1000) users      (985)      780 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/ref_files/change_chirality_cls/diastereomer-2.xyz
--rw-r--r--   0 deo       (1000) users      (985)      780 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/ref_files/change_chirality_cls/diastereomer-3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      780 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/ref_files/change_chirality_cls/diastereomer-4.xyz
--rw-r--r--   0 deo       (1000) users      (985)      577 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/chlorotoluene_180.xyz
--rw-r--r--   0 deo       (1000) users      (985)      323 2019-05-21 17:47:47.000000 AaronTools-1.0b8/test/ref_files/conf_spec.txt
--rw-r--r--   0 deo       (1000) users      (985)     2668 2021-03-19 18:26:30.000000 AaronTools-1.0b8/test/ref_files/config_HOH_init.json
--rw-r--r--   0 deo       (1000) users      (985)     2387 2021-03-19 18:26:30.000000 AaronTools-1.0b8/test/ref_files/config_blank_init.json
--rw-r--r--   0 deo       (1000) users      (985)     3664 2020-09-09 16:21:22.000000 AaronTools-1.0b8/test/ref_files/detect_components.json
--rw-r--r--   0 deo       (1000) users      (985)     4934 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/file_io_died.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4934 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/file_io_error.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2866 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/file_io_normal.xyz
--rw-r--r--   0 deo       (1000) users      (985)   969249 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/freq.json
--rw-r--r--   0 deo       (1000) users      (985)     2884 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/geometry.json
--rw-r--r--   0 deo       (1000) users      (985)    13081 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/lig.json
--rw-r--r--   0 deo       (1000) users      (985)     1520 2020-11-11 15:57:03.000000 AaronTools-1.0b8/test/ref_files/lig_map_1.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1751 2020-11-11 15:57:03.000000 AaronTools-1.0b8/test/ref_files/lig_map_2.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3191 2020-09-09 16:21:22.000000 AaronTools-1.0b8/test/ref_files/lig_map_3.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2837 2020-09-09 16:21:22.000000 AaronTools-1.0b8/test/ref_files/lig_map_4.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4661 2020-11-11 15:57:03.000000 AaronTools-1.0b8/test/ref_files/lig_map_5.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1600 2020-09-09 16:21:22.000000 AaronTools-1.0b8/test/ref_files/lig_map_6.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2844 2020-06-17 21:16:05.000000 AaronTools-1.0b8/test/ref_files/lig_map_7.xyz
--rw-r--r--   0 deo       (1000) users      (985)  1340368 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/log.json
--rw-r--r--   0 deo       (1000) users      (985)     1262 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/make_conf_1.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1262 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/make_conf_2.xyz
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.328559 AaronTools-1.0b8/test/ref_files/make_conf_cls/
--rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-1.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-2.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-3.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-4.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-5.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-6.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-7.xyz
--rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-8.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1329 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/ref_files/minimize_torsion.xyz
--rw-r--r--   0 deo       (1000) users      (985)      682 2020-02-05 23:48:35.000000 AaronTools-1.0b8/test/ref_files/naphthalene.xyz
--rw-r--r--   0 deo       (1000) users      (985)      171 2020-03-24 19:50:16.000000 AaronTools-1.0b8/test/ref_files/orca_geom.xyz
--rw-r--r--   0 deo       (1000) users      (985)      461 2020-06-24 20:42:33.000000 AaronTools-1.0b8/test/ref_files/psi4_geom.xyz
--rw-r--r--   0 deo       (1000) users      (985)      967 2020-02-05 23:48:35.000000 AaronTools-1.0b8/test/ref_files/pyrene.xyz
--rw-r--r--   0 deo       (1000) users      (985)      342 2021-03-19 18:30:22.000000 AaronTools-1.0b8/test/ref_files/ring_subs_changes.json
--rw-r--r--   0 deo       (1000) users      (985)      275 2021-03-19 18:30:22.000000 AaronTools-1.0b8/test/ref_files/simple_subs_changes.json
--rw-r--r--   0 deo       (1000) users      (985)     1310 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/ref_files/sub.json
--rw-r--r--   0 deo       (1000) users      (985)     2187 2020-05-01 21:49:41.000000 AaronTools-1.0b8/test/ref_files/sub_rotate.xyz
--rw-r--r--   0 deo       (1000) users      (985)      819 2020-02-05 23:48:35.000000 AaronTools-1.0b8/test/ref_files/tetrahydronaphthalene.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2018 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/ref_files/torsion_interpolation.xyz
--rw-r--r--   0 deo       (1000) users      (985)       44 2020-11-17 22:04:01.000000 AaronTools-1.0b8/test/ref_files/vbur.xyz
--rw-r--r--   0 deo       (1000) users      (985)       44 2020-11-17 22:04:01.000000 AaronTools-1.0b8/test/ref_files/vbur2.xyz
--rwxr-xr-x   0 deo       (1000) users      (985)     8141 2020-11-19 16:39:16.000000 AaronTools-1.0b8/test/test_atoms.py
--rwxr-xr-x   0 deo       (1000) users      (985)    27506 2021-03-19 19:20:10.000000 AaronTools-1.0b8/test/test_cls.py
--rwxr-xr-x   0 deo       (1000) users      (985)     2926 2021-03-15 19:24:53.000000 AaronTools-1.0b8/test/test_comp_output.py
--rwxr-xr-x   0 deo       (1000) users      (985)     4128 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/test_component.py
--rwxr-xr-x   0 deo       (1000) users      (985)     3503 2021-03-19 19:40:26.000000 AaronTools-1.0b8/test/test_config.py
--rwxr-xr-x   0 deo       (1000) users      (985)     5086 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/test_fetch.py
--rwxr-xr-x   0 deo       (1000) users      (985)    10630 2021-03-15 19:24:53.000000 AaronTools-1.0b8/test/test_fileIO.py
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.338559 AaronTools-1.0b8/test/test_files/
--rw-r--r--   0 deo       (1000) users      (985)     5549 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/5a-sub1.R.ts1.Cf1.3.com
--rw-r--r--   0 deo       (1000) users      (985)     1694 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/6a2e5am1hex.xyz
--rw-r--r--   0 deo       (1000) users      (985)      281 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/COCH3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      330 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/Et_1-NO2.xyz
--rw-r--r--   0 deo       (1000) users      (985)      134 2021-03-19 18:30:22.000000 AaronTools-1.0b8/test/test_files/HOH.ini
--rw-r--r--   0 deo       (1000) users      (985)      146 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/NO2.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2607 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/R-Quinox-tBu3.xyz
--rw-r--r--   0 deo       (1000) users      (985)      563 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/benzene.xyz
--rw-r--r--   0 deo       (1000) users      (985)      707 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/benzene_1-NO2_4-Cl.can.xyz
--rw-r--r--   0 deo       (1000) users      (985)      463 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/benzene_1-NO2_4-Cl.txt
--rw-r--r--   0 deo       (1000) users      (985)      553 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/benzene_1-NO2_4-Cl.xyz
--rw-r--r--   0 deo       (1000) users      (985)      600 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/benzene_1-OH_4-Cl.xyz
--rw-r--r--   0 deo       (1000) users      (985)      849 2019-05-14 21:55:47.000000 AaronTools-1.0b8/test/test_files/benzene_1-Ph_4-Cl.xyz
--rw-r--r--   0 deo       (1000) users      (985)      479 2019-05-14 20:31:18.000000 AaronTools-1.0b8/test/test_files/benzene_4-Cl.xyz
--rw-r--r--   0 deo       (1000) users      (985)      892 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/test_files/benzene_dimer.xyz
--rw-r--r--   0 deo       (1000) users      (985)        0 2021-03-19 18:30:22.000000 AaronTools-1.0b8/test/test_files/blank.ini
--rw-r--r--   0 deo       (1000) users      (985)      759 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/test_files/bpy.xyz
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.341893 AaronTools-1.0b8/test/test_files/catalysts/
--rw-r--r--   0 deo       (1000) users      (985)     8611 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/catalysts/org_1.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3529 2020-09-09 16:21:22.000000 AaronTools-1.0b8/test/test_files/catalysts/org_tri.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3719 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/catalysts/tm_multi-lig.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3488 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/catalysts/tm_single-lig.xyz
--rw-r--r--   0 deo       (1000) users      (985)      553 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/change_dihedral_0.xyz
--rw-r--r--   0 deo       (1000) users      (985)      844 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/test_files/chiral_centers_1.xyz
--rw-r--r--   0 deo       (1000) users      (985)      844 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/test_files/chiral_centers_2.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1264 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/test_files/chiral_centers_3.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1264 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/test_files/chiral_centers_4.xyz
--rw-r--r--   0 deo       (1000) users      (985)      886 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/test_files/chiral_ring.xyz
--rw-r--r--   0 deo       (1000) users      (985)      781 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/test_files/chiral_ring_mirror.xyz
--rw-r--r--   0 deo       (1000) users      (985)      697 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/test_files/chlorotoluene.xyz
--rw-r--r--   0 deo       (1000) users      (985)    86480 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/died.log
--rw-r--r--   0 deo       (1000) users      (985)     1955 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/test_files/dppe.xyz
--rw-r--r--   0 deo       (1000) users      (985)   723280 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/error.log
--rw-r--r--   0 deo       (1000) users      (985)      161 2021-03-19 18:30:22.000000 AaronTools-1.0b8/test/test_files/for_loop.ini
--rw-r--r--   0 deo       (1000) users      (985)    23661 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/test_files/freq.log
--rw-r--r--   0 deo       (1000) users      (985)    29748 2021-03-15 19:24:53.000000 AaronTools-1.0b8/test/test_files/good.crest
--rw-r--r--   0 deo       (1000) users      (985)     1521 2020-10-20 15:19:52.000000 AaronTools-1.0b8/test/test_files/lig_1.xyz
--rw-r--r--   0 deo       (1000) users      (985)     1521 2020-10-20 15:19:52.000000 AaronTools-1.0b8/test/test_files/lig_2.xyz
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.341893 AaronTools-1.0b8/test/test_files/ligands/
--rw-r--r--   0 deo       (1000) users      (985)      272 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/ligands/ACN.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2607 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/ligands/R-Quinox-tBu3.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/ligands/S-tBu-BOX.xyz
--rw-r--r--   0 deo       (1000) users      (985)     3028 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/ligands/squaramide.xyz
--rw-r--r--   0 deo       (1000) users      (985)  1269480 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/normal.log
--rw-r--r--   0 deo       (1000) users      (985)  3342165 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/opt_constraint.log
--rw-r--r--   0 deo       (1000) users      (985)   895212 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/opt_normal.log
--rw-r--r--   0 deo       (1000) users      (985)   402219 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/opt_running.log
--rw-r--r--   0 deo       (1000) users      (985)    78096 2020-03-24 19:50:16.000000 AaronTools-1.0b8/test/test_files/orca_geom.out
--rw-r--r--   0 deo       (1000) users      (985)      861 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/pentane.xyz
--rw-r--r--   0 deo       (1000) users      (985)    62283 2020-06-24 20:42:33.000000 AaronTools-1.0b8/test/test_files/psi4-test.out
--rw-r--r--   0 deo       (1000) users      (985)      508 2020-06-25 22:10:46.000000 AaronTools-1.0b8/test/test_files/ptco4.xyz
--rw-r--r--   0 deo       (1000) users      (985)      419 2020-06-24 20:44:01.000000 AaronTools-1.0b8/test/test_files/pyridine.xyz
--rw-r--r--   0 deo       (1000) users      (985)       94 2021-03-19 18:30:22.000000 AaronTools-1.0b8/test/test_files/ring_subs.ini
--rw-r--r--   0 deo       (1000) users      (985)       95 2021-03-19 18:30:22.000000 AaronTools-1.0b8/test/test_files/simple_subs.ini
--rw-r--r--   0 deo       (1000) users      (985)   895212 2019-05-08 20:00:01.000000 AaronTools-1.0b8/test/test_files/step3.log
--rw-r--r--   0 deo       (1000) users      (985)       48 2021-03-19 18:26:30.000000 AaronTools-1.0b8/test/test_files/substyle_1.ini
--rw-r--r--   0 deo       (1000) users      (985)      725 2020-06-24 20:42:33.000000 AaronTools-1.0b8/test/test_files/test-route-2.com
--rw-r--r--   0 deo       (1000) users      (985)      729 2020-06-24 20:42:33.000000 AaronTools-1.0b8/test/test_files/test-route.com
--rw-r--r--   0 deo       (1000) users      (985)     2566 2020-06-24 20:42:33.000000 AaronTools-1.0b8/test/test_files/test_rmsd_sort1.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2566 2020-06-24 20:42:33.000000 AaronTools-1.0b8/test/test_files/test_rmsd_sort2.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2451 2019-11-13 15:52:13.000000 AaronTools-1.0b8/test/test_files/torsion-60.xyz
--rw-r--r--   0 deo       (1000) users      (985)     2451 2019-11-13 15:52:13.000000 AaronTools-1.0b8/test/test_files/torsion-90.xyz
--rwxr-xr-x   0 deo       (1000) users      (985)     5536 2020-09-09 16:20:38.000000 AaronTools-1.0b8/test/test_finders.py
--rwxr-xr-x   0 deo       (1000) users      (985)    31781 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/test_geometry.py
--rwxr-xr-x   0 deo       (1000) users      (985)     8540 2020-11-19 16:36:34.000000 AaronTools-1.0b8/test/test_json_extension.py
--rwxr-xr-x   0 deo       (1000) users      (985)     1062 2021-03-11 23:11:08.000000 AaronTools-1.0b8/test/test_pathway.py
--rwxr-xr-x   0 deo       (1000) users      (985)     2257 2020-11-19 16:37:02.000000 AaronTools-1.0b8/test/test_substituent.py
--rwxr-xr-x   0 deo       (1000) users      (985)      984 2020-11-19 15:47:08.000000 AaronTools-1.0b8/test/test_utils.py
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.341893 AaronTools-1.0b8/theory/
--rw-r--r--   0 deo       (1000) users      (985)     2949 2021-03-11 23:11:08.000000 AaronTools-1.0b8/theory/__init__.py
--rw-r--r--   0 deo       (1000) users      (985)    30533 2021-03-19 18:26:38.000000 AaronTools-1.0b8/theory/basis.py
--rw-r--r--   0 deo       (1000) users      (985)     7839 2021-03-11 23:11:08.000000 AaronTools-1.0b8/theory/emp_dispersion.py
--rw-r--r--   0 deo       (1000) users      (985)     9794 2021-03-11 23:11:08.000000 AaronTools-1.0b8/theory/grid.py
--rw-r--r--   0 deo       (1000) users      (985)    14765 2021-03-19 18:26:38.000000 AaronTools-1.0b8/theory/implicit_solvent.py
--rw-r--r--   0 deo       (1000) users      (985)    30248 2021-03-19 18:26:38.000000 AaronTools-1.0b8/theory/job_types.py
--rw-r--r--   0 deo       (1000) users      (985)     3887 2021-03-11 23:11:08.000000 AaronTools-1.0b8/theory/method.py
--rw-r--r--   0 deo       (1000) users      (985)    50947 2021-03-19 18:38:49.000000 AaronTools-1.0b8/theory/theory.py
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.341893 AaronTools-1.0b8/utils/
--rw-r--r--   0 deo       (1000) users      (985)        0 2020-11-18 22:59:34.000000 AaronTools-1.0b8/utils/__init__.py
--rwxr-xr-x   0 deo       (1000) users      (985)     2429 2021-03-11 23:11:08.000000 AaronTools-1.0b8/utils/prime_numbers.py
-drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-03-22 19:09:36.345226 AaronTools-1.0b8/utils/quad_grids/
--rw-r--r--   0 deo       (1000) users      (985)     9240 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leb110.grid
--rw-r--r--   0 deo       (1000) users      (985)   122136 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leb1454.grid
--rw-r--r--   0 deo       (1000) users      (985)    16296 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leb194.grid
--rw-r--r--   0 deo       (1000) users      (985)   170520 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leb2030.grid
--rw-r--r--   0 deo       (1000) users      (985)   226968 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leb2702.grid
--rw-r--r--   0 deo       (1000) users      (985)    25368 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leb302.grid
--rw-r--r--   0 deo       (1000) users      (985)   488040 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leb5810.grid
--rw-r--r--   0 deo       (1000) users      (985)    49560 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leb590.grid
--rw-r--r--   0 deo       (1000) users      (985)    81816 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leb974.grid
--rw-r--r--   0 deo       (1000) users      (985)     7788 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leg127.grid
--rw-r--r--   0 deo       (1000) users      (985)     1066 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leg20.grid
--rw-r--r--   0 deo       (1000) users      (985)     1696 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leg32.grid
--rw-r--r--   0 deo       (1000) users      (985)     3387 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leg64.grid
--rw-r--r--   0 deo       (1000) users      (985)     3957 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leg75.grid
--rw-r--r--   0 deo       (1000) users      (985)     5233 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/Leg99.grid
--rw-r--r--   0 deo       (1000) users      (985)      769 2020-11-17 22:04:01.000000 AaronTools-1.0b8/utils/quad_grids/NOTES
--rw-r--r--   0 deo       (1000) users      (985)    18324 2021-03-11 23:11:08.000000 AaronTools-1.0b8/utils/utils.py
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.751455 AaronTools-1.0b9/
+-rw-r--r--   0 deo       (1000) users      (985)      145 2021-03-11 23:11:08.000000 AaronTools-1.0b9/.gitignore
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.534788 AaronTools-1.0b9/AaronTools.egg-info/
+-rw-r--r--   0 deo       (1000) users      (985)     2430 2021-04-20 16:16:33.000000 AaronTools-1.0b9/AaronTools.egg-info/PKG-INFO
+-rw-r--r--   0 deo       (1000) users      (985)    61201 2021-04-20 16:16:33.000000 AaronTools-1.0b9/AaronTools.egg-info/SOURCES.txt
+-rw-r--r--   0 deo       (1000) users      (985)        1 2021-04-20 16:16:33.000000 AaronTools-1.0b9/AaronTools.egg-info/dependency_links.txt
+-rw-r--r--   0 deo       (1000) users      (985)       38 2021-04-20 16:16:33.000000 AaronTools-1.0b9/AaronTools.egg-info/requires.txt
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-20 16:16:33.000000 AaronTools-1.0b9/AaronTools.egg-info/top_level.txt
+-rw-r--r--   0 deo       (1000) users      (985)    35149 2020-09-09 16:20:38.000000 AaronTools-1.0b9/LICENSE
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.594788 AaronTools-1.0b9/Ligands/
+-rw-r--r--   0 deo       (1000) users      (985)      272 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/ACN.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      627 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/AcAc.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2346 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Ad-HC5C.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1071 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/BDA.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1419 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/BPE.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      892 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/BPY.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      980 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/BenQuin.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      822 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/BiOX.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1236 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/BiOx_Me.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       96 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/CO.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      897 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/COD.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      455 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Cp.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1117 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Cp_star.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1156 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/DMBPY.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1243 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/DMP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1067 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/DMPE.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2961 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/DPEphos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2299 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/DPPE.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2871 2020-11-11 15:56:35.000000 AaronTools-1.0b9/Ligands/DPPF.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2431 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/DPPP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      540 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/EDA.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2077 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/IMes.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1993 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/JoshPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3617 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/KASBAI.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1578 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Mes-NC5C.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2170 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Milstein.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      675 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/NBD.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1074 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/PHNNP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      891 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/PIN.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1539 2020-06-24 20:42:33.000000 AaronTools-1.0b9/Ligands/PPh3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1898 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Paton_DL.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1946 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Paton_EL.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3973 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/PhBP3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      964 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/PymdOx.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      867 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/PyrOx.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3445 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R-BINAP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3905 2019-11-13 15:52:13.000000 AaronTools-1.0b9/Ligands/R-Me-StackPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2079 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R-Ph-BOX.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3309 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R-Ph-Mes-NC5C.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2922 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R-Quinox-AdtBu2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2607 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R-Quinox-tBu3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4186 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R-SEGPHOS.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4732 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R-StackPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1995 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R-iPr-PyBOX.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4731 2019-11-13 15:52:13.000000 AaronTools-1.0b9/Ligands/R-pFPh-StackPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R-tBu-BOX.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2695 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-BDPP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-BPCp.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2651 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-Et-DuPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1947 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-Me-BPE.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2123 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-Me-DuPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1248 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-Me-TBF.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3221 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-Me-iPrPh-NC5C.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2210 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-QuinoxP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3179 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-iPr-DuPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2695 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RR-norphos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2563 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/RRSS-DuanPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     5009 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/R_temp.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3445 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/S-BINAP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2915 2019-11-13 15:52:13.000000 AaronTools-1.0b9/Ligands/S-Me-StackPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2079 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/S-Ph-BOX.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3309 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/S-Ph-Mes-NC5C.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3135 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/S-Quinox-AdtBu2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2607 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/S-Quinox-tBu3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3178 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/S-SEGPHOS.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3532 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/S-StackPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1995 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/S-iPr-PyBOX.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3531 2019-11-13 15:52:13.000000 AaronTools-1.0b9/Ligands/S-pFPh-StackPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/S-tBu-BOX.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2095 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SL-J212-1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3047 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SL-J212-2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2695 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SS-BDPP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SS-BPCp.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2651 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SS-Et-DuPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1947 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SS-Me-BPE.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2123 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SS-Me-DuPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1248 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SS-Me-TBF.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3221 2019-11-15 16:33:28.000000 AaronTools-1.0b9/Ligands/SS-Me-iPrPh-NC5C.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2210 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SS-QuinoxP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3179 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SS-iPr-DuPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2695 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SS-norphos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2563 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/SSRR-DuanPhos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1069 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/TACN.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1070 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/TACN_star.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1316 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Tp.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3269 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Xantphos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3661 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/Xphos.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2101 2020-06-24 20:42:33.000000 AaronTools-1.0b9/Ligands/achiral_ligands
+-rw-r--r--   0 deo       (1000) users      (985)     1709 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/bi-isoquinoline-NN-dioxide.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3012 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/chiral_ligands
+-rw-r--r--   0 deo       (1000) users      (985)     1839 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/dithiolate-4F.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1989 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/iPr-NC3C.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2477 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/iPr-PNPEt.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3491 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/iPrPh-BIP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2957 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/iPrPh-NC5C.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       53 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/organocatalysts
+-rw-r--r--   0 deo       (1000) users      (985)     3550 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/squaramide-iPr.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3028 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/squaramide.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3049 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/tBu-PCP.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3181 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Ligands/tBu-PNPPyr.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2430 2021-04-20 16:16:33.751455 AaronTools-1.0b9/PKG-INFO
+-rw-r--r--   0 deo       (1000) users      (985)     1272 2021-01-17 15:33:35.000000 AaronTools-1.0b9/README.md
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.601455 AaronTools-1.0b9/Rings/
+-rw-r--r--   0 deo       (1000) users      (985)      595 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/benzene.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      891 2021-03-11 23:11:08.000000 AaronTools-1.0b9/Rings/cyclohexane.1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      891 2021-03-11 23:11:08.000000 AaronTools-1.0b9/Rings/cyclohexane.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentadiene.1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentadiene.2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentadiene.3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentadiene.5.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentadiene.6.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      538 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentadiene.7.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      730 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentane.1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      730 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentane.2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      730 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentane.3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      730 2020-02-05 23:48:35.000000 AaronTools-1.0b9/Rings/cyclopentane.4.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      730 2021-03-11 23:11:08.000000 AaronTools-1.0b9/Rings/cyclopentane.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      416 2021-03-11 23:11:08.000000 AaronTools-1.0b9/Rings/m-pyridine.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      601 2021-03-11 23:11:08.000000 AaronTools-1.0b9/Rings/m-tetrahydropyran.1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      601 2021-03-11 23:11:08.000000 AaronTools-1.0b9/Rings/m-tetrahydropyran.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      416 2021-03-11 23:11:08.000000 AaronTools-1.0b9/Rings/o-pyridine.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      602 2021-03-11 23:11:08.000000 AaronTools-1.0b9/Rings/o-tetrahydropyran.1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      602 2021-03-11 23:11:08.000000 AaronTools-1.0b9/Rings/o-tetrahydropyran.xyz
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.611455 AaronTools-1.0b9/Substituents/
+-rw-r--r--   0 deo       (1000) users      (985)      649 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/26-F-Ph.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      649 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/35-F-Ph.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1112 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/Ad.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      145 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/BF2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       53 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/Br.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      144 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CCH.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      175 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CF3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      188 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CH2Cl.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      187 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CH2F.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      236 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CH2OH.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      185 2020-10-01 20:48:29.000000 AaronTools-1.0b9/Substituents/CH3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      231 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CHCH2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      189 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CHCl2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      187 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CHF2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      146 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CHO.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       99 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/CN.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      281 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/COCH3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      196 2021-04-20 16:10:55.000000 AaronTools-1.0b9/Substituents/CONH2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      326 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/COOCH3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      191 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/COOH.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       53 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/Cl.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      760 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/Cy.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      417 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/Et.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       54 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/F.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       54 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/H.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       53 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/I.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      185 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/Me.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1191 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/Mes.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      416 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/NCH3_2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      146 2019-11-15 16:33:28.000000 AaronTools-1.0b9/Substituents/NH2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      281 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/NHCH3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      191 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/NHOH.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      101 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/NO.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      146 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/NO2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       52 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/O.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      236 2019-11-15 16:33:28.000000 AaronTools-1.0b9/Substituents/OCF3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       99 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/OH.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      236 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/OMe.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      270 2021-04-20 16:10:55.000000 AaronTools-1.0b9/Substituents/OPO3H2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      233 2021-04-20 16:10:55.000000 AaronTools-1.0b9/Substituents/PO3H2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      506 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/Ph.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      236 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/SCH3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      101 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/SH.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      190 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/SiF3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      190 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/SiH3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2126 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/SuperMes.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      307 2021-04-20 16:10:55.000000 AaronTools-1.0b9/Substituents/guanidino.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      462 2019-05-29 22:58:18.000000 AaronTools-1.0b9/Substituents/iPr.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      238 2021-04-20 16:10:55.000000 AaronTools-1.0b9/Substituents/subs
+-rw-r--r--   0 deo       (1000) users      (985)      596 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/tBu.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      325 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/triazole_C.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      325 2019-05-08 20:00:01.000000 AaronTools-1.0b9/Substituents/triazole_N.xyz
+-rwxr-xr-x   0 deo       (1000) users      (985)     9071 2021-04-20 16:10:55.000000 AaronTools-1.0b9/__init__.py
+-rw-r--r--   0 deo       (1000) users      (985)    44921 2021-04-14 18:15:22.000000 AaronTools-1.0b9/atoms.py
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.644788 AaronTools-1.0b9/bin/
+-rwxr-xr-x   0 deo       (1000) users      (985)     4712 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/angle.py
+-rw-r--r--   0 deo       (1000) users      (985)     9074 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/averageBuriedVolume.py
+-rw-r--r--   0 deo       (1000) users      (985)     7203 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/averageSterimol.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     4161 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/bond.py
+-rwxr-xr-x   0 deo       (1000) users      (985)    10809 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/changeChirality.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     5234 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/changeElement.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     3393 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/closeRing.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     4315 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/coneAngle.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     4994 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/dihedral.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     1193 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/fetchMolecule.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     8029 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/findAtoms.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     7260 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/follow.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     5981 2021-04-02 20:25:12.000000 AaronTools-1.0b9/bin/getCitations.py
+-rw-r--r--   0 deo       (1000) users      (985)     2946 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/getCoordinationComplexes.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2813 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/grabStatus.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     7350 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/grabThermo.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     7592 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/interpolate.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     3609 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/jobSubmit.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     1858 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/libaddLigand.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     1531 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/libaddRing.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2430 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/libaddSubstituent.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     1056 2021-03-19 18:30:22.000000 AaronTools-1.0b9/bin/listChanges.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     8423 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/makeConf.py
+-rwxr-xr-x   0 deo       (1000) users      (985)    21119 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/makeInput.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     6299 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/mapLigand.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2470 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/mirror.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2979 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/parsePDF.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     5533 2021-04-07 16:19:06.000000 AaronTools-1.0b9/bin/percentVolumeBuried.py
+-rw-r--r--   0 deo       (1000) users      (985)     4499 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/plotIR.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2387 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/printFreq.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     4663 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/printFreqBild.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     5112 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/printInfo.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2192 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/printXYZ.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2605 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/removeFragment.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     5550 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/rmsdAlign.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     7395 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/rotate.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     8689 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/stericMap.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     5045 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/substituentSterimol.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     3929 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/substitute.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     5492 2021-04-20 16:10:55.000000 AaronTools-1.0b9/bin/translate.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     6920 2021-03-11 23:11:08.000000 AaronTools-1.0b9/bin/unique.py
+-rw-r--r--   0 deo       (1000) users      (985)   405624 2019-10-31 21:17:55.000000 AaronTools-1.0b9/calculated_bond_lengths.json
+-rw-r--r--   0 deo       (1000) users      (985)    16616 2021-04-15 14:34:51.000000 AaronTools-1.0b9/comp_output.py
+-rw-r--r--   0 deo       (1000) users      (985)    30095 2021-04-20 16:10:55.000000 AaronTools-1.0b9/component.py
+-rw-r--r--   0 deo       (1000) users      (985)      611 2021-04-20 16:10:55.000000 AaronTools-1.0b9/config.ini
+-rw-r--r--   0 deo       (1000) users      (985)    38417 2021-04-16 18:55:37.000000 AaronTools-1.0b9/config.py
+-rw-r--r--   0 deo       (1000) users      (985)    24198 2021-04-07 16:20:00.000000 AaronTools-1.0b9/const.py
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.531455 AaronTools-1.0b9/coordination_complex/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.444788 AaronTools-1.0b9/coordination_complex/capped octahedral/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.644788 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     2575 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.644788 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)     1259 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.644788 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)(BB)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)(BB)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.644788 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)(BB)(CC)/
+-rw-r--r--   0 deo       (1000) users      (985)      643 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)(BB)(CC)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.644788 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      615 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.644788 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)2(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      307 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)2(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)2(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)3/
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)3/C3_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AA)3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AB)(CD)(EF)/
+-rw-r--r--   0 deo       (1000) users      (985)     5151 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AB)(CD)(EF)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AB)2(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     2519 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AB)2(CD)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AB)2(CD)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AB)3/
+-rw-r--r--   0 deo       (1000) users      (985)      783 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AB)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AB)3/C3_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma(AB)3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1987 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AA)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AA)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      979 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)      447 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     4031 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)     1931 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2c(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     1567 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2c(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2c(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2c(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     3303 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2c(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2c(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.648122 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2c2d/
+-rw-r--r--   0 deo       (1000) users      (985)     2687 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2c2d/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      251 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2c2d/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2cde/
+-rw-r--r--   0 deo       (1000) users      (985)     5711 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2cde/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2b2cde/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2bcd(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     3275 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2bcd(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2bcd(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2bcd(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     6719 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2bcd(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2bcdef/
+-rw-r--r--   0 deo       (1000) users      (985)    11759 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma2bcdef/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      643 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AA)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AA)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      307 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     1343 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      643 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      475 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1063 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2c2/
+-rw-r--r--   0 deo       (1000) users      (985)      783 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2c2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      195 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2c2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2cd/
+-rw-r--r--   0 deo       (1000) users      (985)     1791 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2cd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b2cd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b3c/
+-rw-r--r--   0 deo       (1000) users      (985)      503 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b3c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b3c/C3v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3b3c/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3bc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     1035 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3bc(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3bc(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3bc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     2239 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3bc(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3bcde/
+-rw-r--r--   0 deo       (1000) users      (985)     3919 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma3bcde/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      223 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      531 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b2c/
+-rw-r--r--   0 deo       (1000) users      (985)      363 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b2c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      125 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b2c/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.651455 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b3/
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b3/C3v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4b3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4bcd/
+-rw-r--r--   0 deo       (1000) users      (985)      895 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4bcd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma4bcd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5b2/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5b2/C1_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5b2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5bc/
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5bc/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma5bc/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma6b/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma6b/C3v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma6b/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma7/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Ma7/C3v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     4031 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)     2015 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AA)(BB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)      923 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     8063 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)     3863 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabc(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabcde(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     6719 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabcde(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabcde(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)    13439 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabcde(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabcdefg/
+-rw-r--r--   0 deo       (1000) users      (985)    23519 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped octahedral/Mabcdefg/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.454788 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     4703 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)     2267 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(AB)2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(BB)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     2323 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(BB)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(BB)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(BB)(CC)/
+-rw-r--r--   0 deo       (1000) users      (985)     1091 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(BB)(CC)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)(BB)(CC)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.654789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1147 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)2(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      531 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)2(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)2(BB)/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)2(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)3/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)3/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AA)3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AB)(CD)(EF)/
+-rw-r--r--   0 deo       (1000) users      (985)     9407 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AB)(CD)(EF)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AB)2(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     4675 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AB)2(CD)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AB)2(CD)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AB)3/
+-rw-r--r--   0 deo       (1000) users      (985)     1539 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AB)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma(AB)3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     3499 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1651 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)      783 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)2/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     7055 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)     3387 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AB)2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     2575 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c(AA)/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     5431 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c2d/
+-rw-r--r--   0 deo       (1000) users      (985)     4199 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c2d/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c2d/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2c2d/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2cde/
+-rw-r--r--   0 deo       (1000) users      (985)     8735 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2cde/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2b2cde/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2bcd(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     5375 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2bcd(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2bcd(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.658122 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2bcd(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)    10919 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2bcd(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2bcdef/
+-rw-r--r--   0 deo       (1000) users      (985)    17639 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma2bcdef/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1147 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      503 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)      223 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)2/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     2351 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)     1063 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AB)2/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      783 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2(AA)/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1791 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2c2/
+-rw-r--r--   0 deo       (1000) users      (985)     1287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2c2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2c2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2c2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2cd/
+-rw-r--r--   0 deo       (1000) users      (985)     2855 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2cd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b2cd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b3c/
+-rw-r--r--   0 deo       (1000) users      (985)      895 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b3c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3b3c/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3bc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     1735 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3bc(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3bc(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3bc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     3639 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3bc(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3bcde/
+-rw-r--r--   0 deo       (1000) users      (985)     5879 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma3bcde/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      391 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b(AA)/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      895 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.661455 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b2c/
+-rw-r--r--   0 deo       (1000) users      (985)      643 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b2c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b2c/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b2c/C2v_D.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b2c/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b3/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b3/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b3/C2v_D.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4b3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4bcd/
+-rw-r--r--   0 deo       (1000) users      (985)     1427 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4bcd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma4bcd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5(AA)/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5b2/
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5b2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5b2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5b2/C2v_D.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5b2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5bc/
+-rw-r--r--   0 deo       (1000) users      (985)      251 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5bc/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma5bc/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma6b/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma6b/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma6b/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma6b/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma7/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Ma7/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     7055 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)     3443 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)     1679 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)    14111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)     6971 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabc(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabcde(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)    10919 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabcde(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabcde(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)    21839 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabcde(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabcdefg/
+-rw-r--r--   0 deo       (1000) users      (985)    35279 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/capped trigonal prismatic/Mabcdefg/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.464788 AaronTools-1.0b9/coordination_complex/heptagonal/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)(AB)(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)(AB)2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)(AB)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)(BB)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)(BB)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)(BB)(CC)/
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)(BB)(CC)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.664789 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)2(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)2(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)2(BB)/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)2(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)3/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AA)3/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AB)(CD)(EF)/
+-rw-r--r--   0 deo       (1000) users      (985)      335 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AB)(CD)(EF)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AB)2(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AB)2(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AB)3/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma(AB)3/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AA)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AA)(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AA)2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AA)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      335 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AB)(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AB)2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b(AB)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2c(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2c(AA)/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)      195 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2c(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2c(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      419 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2c(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2c2d/
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2c2d/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)      587 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2c2d/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2cde/
+-rw-r--r--   0 deo       (1000) users      (985)     1259 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2b2cde/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2bcd(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      419 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2bcd(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2bcd(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      839 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2bcd(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2bcdef/
+-rw-r--r--   0 deo       (1000) users      (985)     2519 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma2bcdef/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AA)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AA)(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AA)2/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AB)(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AB)2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3(AB)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2(AA)/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2c2/
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2c2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2c2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2cd/
+-rw-r--r--   0 deo       (1000) users      (985)      419 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b2cd/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b3c/
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3b3c/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3bc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3bc(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3bc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      279 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3bc(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3bcde/
+-rw-r--r--   0 deo       (1000) users      (985)      839 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma3bcde/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.668122 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b(AA)/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b2c/
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b2c/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b2c/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b3/
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b3/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4b3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4bcd/
+-rw-r--r--   0 deo       (1000) users      (985)      209 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma4bcd/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma5(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma5(AA)/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma5(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma5(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma5b2/
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma5b2/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma5bc/
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma5bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma6b/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma6b/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Ma7/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Ma7/D7h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      335 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AA)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AA)(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AA)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      671 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AB)(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      335 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Mabc(AB)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Mabcde(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      839 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Mabcde(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Mabcde(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1679 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Mabcde(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/heptagonal/Mabcdefg/
+-rw-r--r--   0 deo       (1000) users      (985)     5039 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/heptagonal/Mabcdefg/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.478121 AaronTools-1.0b9/coordination_complex/hexagonal/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)(AB)(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)(AB)2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)(AB)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)(BB)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)(BB)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)(BB)(CC)/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)(BB)(CC)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)2(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)2(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)2(BB)/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)3/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AA)3/D3h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AB)(CD)(EF)/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AB)(CD)(EF)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AB)2(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AB)2(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/M(AB)3/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AB)3/C3h_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/M(AB)3/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       35 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AA)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AA)(BB)/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AA)(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AA)2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AA)2/D2h_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AB)(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AB)2/C2h_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       35 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AB)2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2(AA)/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2c2/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2c2/C2h_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2c2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2c2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2cd/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2cd/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2b2cd/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2bc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2bc(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2bc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      143 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2bc(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2bcde/
+-rw-r--r--   0 deo       (1000) users      (985)      359 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma2bcde/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b2c/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b2c/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b2c/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b3/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b3/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b3/Cs_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3b3/D3h_C.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3bcd/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma3bcd/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4(AA)/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4b2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4b2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4b2/D2h_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4bc/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4bc/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma4bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma5b/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma5b/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Ma6/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Ma6/D6h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AA)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       35 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AA)(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AA)2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AA)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      143 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AB)(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AB)2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       59 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mab(AB)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Mabcd(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      143 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mabcd(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Mabcd(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mabcd(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/hexagonal/Mabcdef/
+-rw-r--r--   0 deo       (1000) users      (985)      719 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal/Mabcdef/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.471454 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     1119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      503 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)(BB)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      559 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)(BB)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)(BB)(CC)/
+-rw-r--r--   0 deo       (1000) users      (985)      279 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)(BB)(CC)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      251 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)2(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)2(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)2(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)3/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)3/C3v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AA)3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AB)(CD)(EF)/
+-rw-r--r--   0 deo       (1000) users      (985)     2239 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AB)(CD)(EF)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.671455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AB)2(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     1063 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AB)2(CD)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AB)2(CD)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AB)3/
+-rw-r--r--   0 deo       (1000) users      (985)      307 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AB)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AB)3/C3_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma(AB)3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      923 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      447 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)      195 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AA)2/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     1847 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      839 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AB)2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      783 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1623 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c2d/
+-rw-r--r--   0 deo       (1000) users      (985)     1287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c2d/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c2d/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2c2d/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2cde/
+-rw-r--r--   0 deo       (1000) users      (985)     2855 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2cde/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2b2cde/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2bcd(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     1679 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2bcd(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2bcd(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     3359 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2bcd(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2bcdef/
+-rw-r--r--   0 deo       (1000) users      (985)     5879 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma2bcdef/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      307 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AA)2/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      615 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      251 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AB)2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      223 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.674789 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      503 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2c2/
+-rw-r--r--   0 deo       (1000) users      (985)      335 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2c2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2c2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2c2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2cd/
+-rw-r--r--   0 deo       (1000) users      (985)      895 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2cd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b2cd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b3c/
+-rw-r--r--   0 deo       (1000) users      (985)      251 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b3c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b3c/C3v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3b3c/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3bc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      559 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3bc(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3bc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3bc(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3bcde/
+-rw-r--r--   0 deo       (1000) users      (985)     1959 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma3bcde/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      251 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b2c/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b2c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b2c/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b2c/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b3/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b3/C1_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b3/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b3/C3v_D.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4b3/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4bcd/
+-rw-r--r--   0 deo       (1000) users      (985)      447 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4bcd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma4bcd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5b2/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5b2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5b2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5bc/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5bc/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma5bc/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma6b/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma6b/C6v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma6b/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma7/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Ma7/C6v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1847 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      923 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AA)(BB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)      419 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.678122 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     3695 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)     1763 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabc(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabcde(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     3359 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabcde(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabcde(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     6719 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabcde(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.681455 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabcdefg/
+-rw-r--r--   0 deo       (1000) users      (985)    11759 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/hexagonal pyramidal/Mabcdefg/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.481455 AaronTools-1.0b9/coordination_complex/octahedral/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)(AB)2/C2_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)(BB)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)(BB)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)(BB)(CC)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)(BB)(CC)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)2(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)2(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)2(BB)/C2_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)3/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AA)3/D3_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AB)(CD)(EF)/
+-rw-r--r--   0 deo       (1000) users      (985)      191 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AB)(CD)(EF)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AB)2(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AB)2(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/M(AB)3/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AB)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/M(AB)3/C3_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.684789 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AA)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AA)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AA)(BB)/C2v_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AA)2/C2_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AA)2/D2h_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AB)(CD)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AB)(CD)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AB)2/C2_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AB)2/C2h_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2(AB)2/C2v_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2(AA)/C2v_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2c2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2c2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       35 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2c2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2c2/D2h_C.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2cd/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2cd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2cd/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       35 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2b2cd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2bc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2bc(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2bc(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2bc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2bc(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2bc(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma2bcde/
+-rw-r--r--   0 deo       (1000) users      (985)      143 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2bcde/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       35 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma2bcde/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b2c/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b2c/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b2c/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.688122 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b3/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b3/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma3b3/C3v_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Ma3bcd/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma3bcd/C1_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       35 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma3bcd/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Ma4(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma4(AA)/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Ma4(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma4(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Ma4b2/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma4b2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma4b2/D4h_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Ma4bc/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma4bc/C4v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma4bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Ma5b/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma5b/C4v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Ma6/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Ma6/Oh_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AA)2/C2v_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      239 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AB)2/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mab(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Mabcd(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      143 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mabcd(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Mabcd(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mabcd(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/octahedral/Mabcdef/
+-rw-r--r--   0 deo       (1000) users      (985)      359 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/octahedral/Mabcdef/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.491455 AaronTools-1.0b9/coordination_complex/pentagonal/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AA)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AA)(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AA)2/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       39 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AB)(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AB)2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma(AB)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2b(AA)/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2b(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       29 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2b(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2b2c/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2b2c/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2b2c/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2bcd/
+-rw-r--r--   0 deo       (1000) users      (985)       59 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma2bcd/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma3(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma3(AA)/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma3(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma3(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma3b2/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma3b2/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma3bc/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma3bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma4b/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma4b/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Ma5/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Ma5/D5h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Mabc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       29 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Mabc(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Mabc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       59 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Mabc(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal/Mabcde/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal/Mabcde/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.484788 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     1343 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      615 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(AB)2/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(BB)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      671 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(BB)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(BB)(CC)/
+-rw-r--r--   0 deo       (1000) users      (985)      335 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)(BB)(CC)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      307 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.691455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)2(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)2(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)2(BB)/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)2(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)3/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)3/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AA)3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AB)(CD)(EF)/
+-rw-r--r--   0 deo       (1000) users      (985)     2687 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AB)(CD)(EF)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AB)2(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     1287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AB)2(CD)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AB)2(CD)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AB)3/
+-rw-r--r--   0 deo       (1000) users      (985)      391 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AB)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma(AB)3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      867 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      419 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)2/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)2/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     1791 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AB)(CD)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AB)(CD)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      811 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AB)2/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AB)2/C2v_D.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b(AB)2/Cs_C.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      531 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c(AA)/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c2d/
+-rw-r--r--   0 deo       (1000) users      (985)      671 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c2d/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c2d/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2c2d/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2cde/
+-rw-r--r--   0 deo       (1000) users      (985)     1511 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2cde/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      251 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2b2cde/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2bcd(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     1175 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2bcd(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2bcd(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.694789 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2bcd(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     2435 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2bcd(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2bcd(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2bcdef/
+-rw-r--r--   0 deo       (1000) users      (985)     3359 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2bcdef/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma2bcdef/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      251 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)2/C2_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)2/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      559 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AB)(CD)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AB)(CD)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      223 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AB)2/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AB)2/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3(AB)2/Cs_C.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2(AA)/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      307 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      111 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2c2/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2c2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2c2/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2c2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2cd/
+-rw-r--r--   0 deo       (1000) users      (985)      391 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2cd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      195 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b2cd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b3c/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b3c/C1_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3b3c/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3bc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      335 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3bc(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3bc(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3bc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      755 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3bc(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3bc(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3bcde/
+-rw-r--r--   0 deo       (1000) users      (985)     1007 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3bcde/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma3bcde/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b(AA)/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.698122 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      139 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b2c/
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b2c/C1_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b2c/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       69 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b2c/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b3/
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b3/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4b3/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4bcd/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4bcd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)      125 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma4bcd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5(AA)/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5b2/
+-rw-r--r--   0 deo       (1000) users      (985)       27 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5b2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5b2/Cs_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5b2/D5h_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5bc/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5bc/C5v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       55 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma5bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma6b/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma6b/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma6b/C5v_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma7/
+-rw-r--r--   0 deo       (1000) users      (985)       13 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Ma7/D5h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1847 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      923 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AA)(BB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)      419 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       41 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)     3695 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)     1763 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       83 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabc(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabcde(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)     2519 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabcde(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabcde(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     5039 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabcde(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabcdefg/
+-rw-r--r--   0 deo       (1000) users      (985)     7055 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal bipyramidal/Mabcdefg/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.488121 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)(BB)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      143 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)(BB)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)(BB)(CC)/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)(BB)(CC)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)2(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)2(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)2(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)3/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AA)3/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.701455 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AB)(CD)(EF)/
+-rw-r--r--   0 deo       (1000) users      (985)      575 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AB)(CD)(EF)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AB)2(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      239 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AB)2(CD)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AB)2(CD)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AB)3/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AB)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/M(AB)3/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AA)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AA)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AA)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      383 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      239 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2c2/
+-rw-r--r--   0 deo       (1000) users      (985)      143 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2c2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2c2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2cd/
+-rw-r--r--   0 deo       (1000) users      (985)      383 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2cd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2b2cd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2bc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      263 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2bc(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2bc(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2bc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      575 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2bc(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2bcde/
+-rw-r--r--   0 deo       (1000) users      (985)      863 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma2bcde/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      191 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b2c/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b2c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b2c/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b3/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3b3/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3bcd/
+-rw-r--r--   0 deo       (1000) users      (985)      287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma3bcd/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.704789 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4b2/
+-rw-r--r--   0 deo       (1000) users      (985)       35 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4b2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4bc/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4bc/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma4bc/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma5b/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma5b/C5v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma5b/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma6/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Ma6/C5v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      383 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      191 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AA)(BB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      767 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      335 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mab(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mabcd(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      575 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mabcd(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mabcd(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)     1151 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mabcd(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mabcdef/
+-rw-r--r--   0 deo       (1000) users      (985)     1727 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/pentagonal pyramidal/Mabcdef/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.491455 AaronTools-1.0b9/coordination_complex/seesaw/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/seesaw/M(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       31 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/M(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/seesaw/M(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/M(AA)(BB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.708122 AaronTools-1.0b9/coordination_complex/seesaw/M(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/M(AA)2/C2_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/M(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       63 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/M(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/M(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/M(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       31 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/M(AB)2/C2_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/Ma2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma2(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma2(AA)/C2v_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/Ma2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       31 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/Ma2b2/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma2b2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma2b2/C2v_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/Ma2bc/
+-rw-r--r--   0 deo       (1000) users      (985)       31 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma2bc/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma2bc/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/Ma3b/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma3b/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/Ma4/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Ma4/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/Mab(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       31 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Mab(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Mab(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/Mab(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       79 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Mab(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/seesaw/Mabcd/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/seesaw/Mabcd/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.491455 AaronTools-1.0b9/coordination_complex/square planar/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/M(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/M(AA)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/M(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/M(AA)(BB)/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/M(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/M(AA)2/D2h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/M(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/M(AB)(CD)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/M(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/M(AB)2/C2h_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/M(AB)2/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/Ma2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Ma2(AA)/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/Ma2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Ma2(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/Ma2b2/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Ma2b2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Ma2b2/D2h_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/Ma2bc/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Ma2bc/C2h_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Ma2bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/Ma3b/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Ma3b/C2h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/Ma4/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Ma4/D4h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/Mab(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Mab(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/Mab(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Mab(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square planar/Mabcd/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square planar/Mabcd/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.528121 AaronTools-1.0b9/coordination_complex/square pyramidal/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AA)(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.711455 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AA)2/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       39 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AB)2/C2_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma(AB)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2b(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2b(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       59 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2b(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2b2c/
+-rw-r--r--   0 deo       (1000) users      (985)       39 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2b2c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2b2c/C2v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       29 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2b2c/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2bcd/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2bcd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       29 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma2bcd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3b2/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3b2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3b2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3bc/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3bc/C1_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       29 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma3bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma4b/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma4b/C4v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma4b/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma5/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Ma5/C4v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Mabc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       59 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Mabc(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Mabc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Mabc(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/square pyramidal/Mabcde/
+-rw-r--r--   0 deo       (1000) users      (985)      299 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/square pyramidal/Mabcde/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.528121 AaronTools-1.0b9/coordination_complex/tetrahedral/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AA)(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AA)(BB)/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AA)2/D2d_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/M(AB)2/C2_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma2(AA)/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma2(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma2b2/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma2b2/C2v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma2bc/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma2bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma3b/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma3b/C3v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma4/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/Ma4/Td_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/Mab(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/Mab(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/Mab(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/Mab(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/tetrahedral/Mabcd/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/tetrahedral/Mabcd/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.528121 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       39 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AA)(BB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.714789 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AA)2/C2_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)       79 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       39 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma(AB)2/C2_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       39 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b2c/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b2c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b2c/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2b2c/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2bcd/
+-rw-r--r--   0 deo       (1000) users      (985)       59 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2bcd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       39 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma2bcd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       19 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3b2/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3b2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3b2/Cs_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3b2/D3h_C.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3bc/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3bc/C3v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       29 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma3bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma4b/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma4b/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma4b/C3v_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma5/
+-rw-r--r--   0 deo       (1000) users      (985)        9 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Ma5/D3h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Mabc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       59 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Mabc(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Mabc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Mabc(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Mabcde/
+-rw-r--r--   0 deo       (1000) users      (985)      199 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal bipyramidal/Mabcde/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.531455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      191 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(AB)2/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(BB)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(BB)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(BB)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(BB)(CC)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)(BB)(CC)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)2(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)2(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)2(BB)/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)2(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)3/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)3/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AA)3/D3h_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.718122 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AB)(CD)(EF)/
+-rw-r--r--   0 deo       (1000) users      (985)      383 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AB)(CD)(EF)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AB)2(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      167 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AB)2(CD)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AB)2(CD)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AB)3/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AB)3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AB)3/C3v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/M(AB)3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)(BB)/C1_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)(BB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)2/C2_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)2/C2v_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AA)2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AB)2/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2(AB)2/Cs_C.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2(AA)/C2_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      191 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2c2/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2c2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       71 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2c2/C2_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2c2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2cd/
+-rw-r--r--   0 deo       (1000) users      (985)      335 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2cd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2b2cd/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2bc(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      191 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2bc(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2bc(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2bc(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      431 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2bc(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2bcde/
+-rw-r--r--   0 deo       (1000) users      (985)      719 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma2bcde/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b(AA)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b(AA)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      143 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.721455 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b2c/
+-rw-r--r--   0 deo       (1000) users      (985)       95 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b2c/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b2c/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b3/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b3/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b3/C3v_C.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3b3/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3bcd/
+-rw-r--r--   0 deo       (1000) users      (985)      239 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma3bcd/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4(AA)/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4(AB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4(AB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4b2/
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4b2/C2_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4b2/C2v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4b2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4bc/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4bc/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma4bc/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma5b/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma5b/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma6/
+-rw-r--r--   0 deo       (1000) users      (985)       11 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Ma6/D3h_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AA)(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      287 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AA)(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AA)(BB)/
+-rw-r--r--   0 deo       (1000) users      (985)      119 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AA)(BB)/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AA)(BB)/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AA)2/
+-rw-r--r--   0 deo       (1000) users      (985)       47 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AA)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AA)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AB)(CD)/
+-rw-r--r--   0 deo       (1000) users      (985)      575 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AB)(CD)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AB)2/
+-rw-r--r--   0 deo       (1000) users      (985)      263 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AB)2/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       23 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mab(AB)2/Cs_B.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mabcd(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)      431 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mabcd(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mabcd(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)      863 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mabcd(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mabcdef/
+-rw-r--r--   0 deo       (1000) users      (985)     1439 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal prismatic/Mabcdef/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.531455 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma2(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma2(AA)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma2(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma2(AB)/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma2b2/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma2b2/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma2bc/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma2bc/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma2bc/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma3b/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma3b/C3v_B.csv
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma3b/Cs_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.724789 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma4/
+-rw-r--r--   0 deo       (1000) users      (985)        7 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Ma4/C3v_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.728122 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Mab(AA)/
+-rw-r--r--   0 deo       (1000) users      (985)       15 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Mab(AA)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.728122 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Mab(AB)/
+-rw-r--r--   0 deo       (1000) users      (985)       31 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Mab(AB)/C1_A.csv
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.728122 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Mabcd/
+-rw-r--r--   0 deo       (1000) users      (985)       63 2021-04-07 16:19:06.000000 AaronTools-1.0b9/coordination_complex/trigonal pyramidal/Mabcd/C1_A.csv
+-rw-r--r--   0 deo       (1000) users      (985)    93136 2021-04-20 16:10:55.000000 AaronTools-1.0b9/fileIO.py
+-rw-r--r--   0 deo       (1000) users      (985)    17203 2021-03-30 13:49:47.000000 AaronTools-1.0b9/finders.py
+-rw-r--r--   0 deo       (1000) users      (985)   167133 2021-04-20 16:10:55.000000 AaronTools-1.0b9/geometry.py
+-rw-r--r--   0 deo       (1000) users      (985)     9901 2021-04-20 16:10:55.000000 AaronTools-1.0b9/job_control.py
+-rw-r--r--   0 deo       (1000) users      (985)    13780 2021-04-07 16:19:06.000000 AaronTools-1.0b9/json_extension.py
+-rw-r--r--   0 deo       (1000) users      (985)     7607 2020-11-17 21:43:36.000000 AaronTools-1.0b9/new_fileIO.py
+-rw-r--r--   0 deo       (1000) users      (985)    12772 2021-03-11 23:11:08.000000 AaronTools-1.0b9/pathway.py
+-rw-r--r--   0 deo       (1000) users      (985)     7006 2021-03-11 23:11:08.000000 AaronTools-1.0b9/ring.py
+-rw-r--r--   0 deo       (1000) users      (985)       38 2021-04-20 16:16:33.751455 AaronTools-1.0b9/setup.cfg
+-rw-r--r--   0 deo       (1000) users      (985)     8613 2021-04-20 16:16:28.000000 AaronTools-1.0b9/setup.py
+-rw-r--r--   0 deo       (1000) users      (985)    29628 2021-04-20 16:10:55.000000 AaronTools-1.0b9/substituent.py
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.728122 AaronTools-1.0b9/test/
+-rw-r--r--   0 deo       (1000) users      (985)     5250 2021-04-07 16:15:10.000000 AaronTools-1.0b9/test/__init__.py
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.734789 AaronTools-1.0b9/test/ref_files/
+-rw-r--r--   0 deo       (1000) users      (985)     1905 2021-04-20 15:45:14.000000 AaronTools-1.0b9/test/ref_files/HOH_init.json
+-rw-r--r--   0 deo       (1000) users      (985)     2653 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/atom.json
+-rw-r--r--   0 deo       (1000) users      (985)      893 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/benzene_dimer_ref.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      389 2021-04-20 15:45:14.000000 AaronTools-1.0b9/test/ref_files/blank_init.json
+-rw-r--r--   0 deo       (1000) users      (985)    23638 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/cat.json
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.734789 AaronTools-1.0b9/test/ref_files/change_chirality_cls/
+-rw-r--r--   0 deo       (1000) users      (985)      780 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/ref_files/change_chirality_cls/diastereomer-1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      780 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/ref_files/change_chirality_cls/diastereomer-2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      780 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/ref_files/change_chirality_cls/diastereomer-3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      780 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/ref_files/change_chirality_cls/diastereomer-4.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      577 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/chlorotoluene_180.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      323 2019-05-21 17:47:47.000000 AaronTools-1.0b9/test/ref_files/conf_spec.txt
+-rw-r--r--   0 deo       (1000) users      (985)     2668 2021-03-22 19:17:08.000000 AaronTools-1.0b9/test/ref_files/config_HOH_init.json
+-rw-r--r--   0 deo       (1000) users      (985)     2387 2021-03-22 19:17:08.000000 AaronTools-1.0b9/test/ref_files/config_blank_init.json
+-rw-r--r--   0 deo       (1000) users      (985)     3664 2020-09-09 16:21:22.000000 AaronTools-1.0b9/test/ref_files/detect_components.json
+-rw-r--r--   0 deo       (1000) users      (985)     4934 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/file_io_died.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4934 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/file_io_error.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2866 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/file_io_normal.xyz
+-rw-r--r--   0 deo       (1000) users      (985)   969249 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/freq.json
+-rw-r--r--   0 deo       (1000) users      (985)     2884 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/geometry.json
+-rw-r--r--   0 deo       (1000) users      (985)    13081 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/lig.json
+-rw-r--r--   0 deo       (1000) users      (985)     1520 2020-11-11 15:57:03.000000 AaronTools-1.0b9/test/ref_files/lig_map_1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1751 2020-11-11 15:57:03.000000 AaronTools-1.0b9/test/ref_files/lig_map_2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3191 2020-09-09 16:21:22.000000 AaronTools-1.0b9/test/ref_files/lig_map_3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2837 2020-09-09 16:21:22.000000 AaronTools-1.0b9/test/ref_files/lig_map_4.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4661 2020-11-11 15:57:03.000000 AaronTools-1.0b9/test/ref_files/lig_map_5.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1600 2020-09-09 16:21:22.000000 AaronTools-1.0b9/test/ref_files/lig_map_6.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2844 2020-06-17 21:16:05.000000 AaronTools-1.0b9/test/ref_files/lig_map_7.xyz
+-rw-r--r--   0 deo       (1000) users      (985)  1340368 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/log.json
+-rw-r--r--   0 deo       (1000) users      (985)     1262 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/make_conf_1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1262 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/make_conf_2.xyz
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.734789 AaronTools-1.0b9/test/ref_files/make_conf_cls/
+-rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-4.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-5.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-6.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-7.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     4386 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-8.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1329 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/ref_files/minimize_torsion.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      682 2020-02-05 23:48:35.000000 AaronTools-1.0b9/test/ref_files/naphthalene.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      171 2020-03-24 19:50:16.000000 AaronTools-1.0b9/test/ref_files/orca_geom.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      461 2020-06-24 20:42:33.000000 AaronTools-1.0b9/test/ref_files/psi4_geom.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      967 2020-02-05 23:48:35.000000 AaronTools-1.0b9/test/ref_files/pyrene.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      342 2021-03-19 18:30:22.000000 AaronTools-1.0b9/test/ref_files/ring_subs_changes.json
+-rw-r--r--   0 deo       (1000) users      (985)      275 2021-03-19 18:30:22.000000 AaronTools-1.0b9/test/ref_files/simple_subs_changes.json
+-rw-r--r--   0 deo       (1000) users      (985)     1310 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/ref_files/sub.json
+-rw-r--r--   0 deo       (1000) users      (985)     2187 2020-05-01 21:49:41.000000 AaronTools-1.0b9/test/ref_files/sub_rotate.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      819 2020-02-05 23:48:35.000000 AaronTools-1.0b9/test/ref_files/tetrahydronaphthalene.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2018 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/ref_files/torsion_interpolation.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       44 2020-11-17 22:04:01.000000 AaronTools-1.0b9/test/ref_files/vbur.xyz
+-rw-r--r--   0 deo       (1000) users      (985)       44 2020-11-17 22:04:01.000000 AaronTools-1.0b9/test/ref_files/vbur2.xyz
+-rwxr-xr-x   0 deo       (1000) users      (985)     8162 2021-04-05 20:37:07.000000 AaronTools-1.0b9/test/test_atoms.py
+-rwxr-xr-x   0 deo       (1000) users      (985)    27554 2021-04-07 16:19:06.000000 AaronTools-1.0b9/test/test_cls.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2936 2021-03-30 21:43:50.000000 AaronTools-1.0b9/test/test_comp_output.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     4128 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/test_component.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     3597 2021-04-20 15:54:33.000000 AaronTools-1.0b9/test/test_config.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     5239 2021-04-20 15:58:32.000000 AaronTools-1.0b9/test/test_fetch.py
+-rwxr-xr-x   0 deo       (1000) users      (985)    10647 2021-03-30 21:43:50.000000 AaronTools-1.0b9/test/test_fileIO.py
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.744789 AaronTools-1.0b9/test/test_files/
+-rw-r--r--   0 deo       (1000) users      (985)     5549 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/5a-sub1.R.ts1.Cf1.3.com
+-rw-r--r--   0 deo       (1000) users      (985)     1694 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/6a2e5am1hex.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      281 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/COCH3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      330 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/Et_1-NO2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      134 2021-03-19 18:30:22.000000 AaronTools-1.0b9/test/test_files/HOH.ini
+-rw-r--r--   0 deo       (1000) users      (985)      146 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/NO2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2607 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/R-Quinox-tBu3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      563 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/benzene.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      707 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/benzene_1-NO2_4-Cl.can.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      463 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/benzene_1-NO2_4-Cl.txt
+-rw-r--r--   0 deo       (1000) users      (985)      553 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/benzene_1-NO2_4-Cl.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      600 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/benzene_1-OH_4-Cl.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      849 2019-05-14 21:55:47.000000 AaronTools-1.0b9/test/test_files/benzene_1-Ph_4-Cl.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      479 2019-05-14 20:31:18.000000 AaronTools-1.0b9/test/test_files/benzene_4-Cl.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      892 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/test_files/benzene_dimer.xyz
+-rw-r--r--   0 deo       (1000) users      (985)        0 2021-03-19 18:30:22.000000 AaronTools-1.0b9/test/test_files/blank.ini
+-rw-r--r--   0 deo       (1000) users      (985)      759 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/test_files/bpy.xyz
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.744789 AaronTools-1.0b9/test/test_files/catalysts/
+-rw-r--r--   0 deo       (1000) users      (985)     8611 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/catalysts/org_1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3529 2020-09-09 16:21:22.000000 AaronTools-1.0b9/test/test_files/catalysts/org_tri.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3719 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/catalysts/tm_multi-lig.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3488 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/catalysts/tm_single-lig.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      553 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/change_dihedral_0.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      844 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/test_files/chiral_centers_1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      844 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/test_files/chiral_centers_2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1264 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/test_files/chiral_centers_3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1264 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/test_files/chiral_centers_4.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      886 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/test_files/chiral_ring.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      781 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/test_files/chiral_ring_mirror.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      697 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/test_files/chlorotoluene.xyz
+-rw-r--r--   0 deo       (1000) users      (985)    86480 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/died.log
+-rw-r--r--   0 deo       (1000) users      (985)     1955 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/test_files/dppe.xyz
+-rw-r--r--   0 deo       (1000) users      (985)   723280 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/error.log
+-rw-r--r--   0 deo       (1000) users      (985)      161 2021-03-19 18:30:22.000000 AaronTools-1.0b9/test/test_files/for_loop.ini
+-rw-r--r--   0 deo       (1000) users      (985)    23661 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/test_files/freq.log
+-rw-r--r--   0 deo       (1000) users      (985)    29748 2021-03-15 19:24:53.000000 AaronTools-1.0b9/test/test_files/good.crest
+-rw-r--r--   0 deo       (1000) users      (985)     1521 2020-10-20 15:19:52.000000 AaronTools-1.0b9/test/test_files/lig_1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     1521 2020-10-20 15:19:52.000000 AaronTools-1.0b9/test/test_files/lig_2.xyz
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.744789 AaronTools-1.0b9/test/test_files/ligands/
+-rw-r--r--   0 deo       (1000) users      (985)      272 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/ligands/ACN.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2607 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/ligands/R-Quinox-tBu3.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2255 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/ligands/S-tBu-BOX.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     3028 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/ligands/squaramide.xyz
+-rw-r--r--   0 deo       (1000) users      (985)  1269480 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/normal.log
+-rw-r--r--   0 deo       (1000) users      (985)  3342165 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/opt_constraint.log
+-rw-r--r--   0 deo       (1000) users      (985)   895212 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/opt_normal.log
+-rw-r--r--   0 deo       (1000) users      (985)   402219 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/opt_running.log
+-rw-r--r--   0 deo       (1000) users      (985)    78096 2020-03-24 19:50:16.000000 AaronTools-1.0b9/test/test_files/orca_geom.out
+-rw-r--r--   0 deo       (1000) users      (985)      861 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/pentane.xyz
+-rw-r--r--   0 deo       (1000) users      (985)    62283 2020-06-24 20:42:33.000000 AaronTools-1.0b9/test/test_files/psi4-test.out
+-rw-r--r--   0 deo       (1000) users      (985)      508 2020-06-25 22:10:46.000000 AaronTools-1.0b9/test/test_files/ptco4.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      419 2020-06-24 20:44:01.000000 AaronTools-1.0b9/test/test_files/pyridine.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      107 2021-04-20 15:54:18.000000 AaronTools-1.0b9/test/test_files/ring_subs.ini
+-rw-r--r--   0 deo       (1000) users      (985)       72 2021-04-20 15:52:22.000000 AaronTools-1.0b9/test/test_files/simple_subs.ini
+-rw-r--r--   0 deo       (1000) users      (985)   895212 2019-05-08 20:00:01.000000 AaronTools-1.0b9/test/test_files/step3.log
+-rw-r--r--   0 deo       (1000) users      (985)       48 2021-03-22 19:17:08.000000 AaronTools-1.0b9/test/test_files/substyle_1.ini
+-rw-r--r--   0 deo       (1000) users      (985)      725 2020-06-24 20:42:33.000000 AaronTools-1.0b9/test/test_files/test-route-2.com
+-rw-r--r--   0 deo       (1000) users      (985)      729 2020-06-24 20:42:33.000000 AaronTools-1.0b9/test/test_files/test-route.com
+-rw-r--r--   0 deo       (1000) users      (985)     2566 2020-06-24 20:42:33.000000 AaronTools-1.0b9/test/test_files/test_rmsd_sort1.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2566 2020-06-24 20:42:33.000000 AaronTools-1.0b9/test/test_files/test_rmsd_sort2.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2451 2019-11-13 15:52:13.000000 AaronTools-1.0b9/test/test_files/torsion-60.xyz
+-rw-r--r--   0 deo       (1000) users      (985)     2451 2019-11-13 15:52:13.000000 AaronTools-1.0b9/test/test_files/torsion-90.xyz
+-rw-r--r--   0 deo       (1000) users      (985)      300 2021-04-09 16:07:31.000000 AaronTools-1.0b9/test/test_files/xtb_config.ini
+-rwxr-xr-x   0 deo       (1000) users      (985)     5536 2020-09-09 16:20:38.000000 AaronTools-1.0b9/test/test_finders.py
+-rwxr-xr-x   0 deo       (1000) users      (985)    31781 2021-04-07 16:17:01.000000 AaronTools-1.0b9/test/test_geometry.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     8540 2020-11-19 16:36:34.000000 AaronTools-1.0b9/test/test_json_extension.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     1062 2021-03-11 23:11:08.000000 AaronTools-1.0b9/test/test_pathway.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2257 2020-11-19 16:37:02.000000 AaronTools-1.0b9/test/test_substituent.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     1516 2021-04-20 15:43:57.000000 AaronTools-1.0b9/test/test_theory.py
+-rwxr-xr-x   0 deo       (1000) users      (985)      984 2020-11-19 15:47:08.000000 AaronTools-1.0b9/test/test_utils.py
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.744789 AaronTools-1.0b9/theory/
+-rw-r--r--   0 deo       (1000) users      (985)     2949 2021-04-01 21:51:39.000000 AaronTools-1.0b9/theory/__init__.py
+-rw-r--r--   0 deo       (1000) users      (985)    43293 2021-04-08 14:17:49.000000 AaronTools-1.0b9/theory/basis.py
+-rw-r--r--   0 deo       (1000) users      (985)     7839 2021-03-11 23:11:08.000000 AaronTools-1.0b9/theory/emp_dispersion.py
+-rw-r--r--   0 deo       (1000) users      (985)     9794 2021-03-11 23:11:08.000000 AaronTools-1.0b9/theory/grid.py
+-rw-r--r--   0 deo       (1000) users      (985)    14765 2021-03-22 19:17:08.000000 AaronTools-1.0b9/theory/implicit_solvent.py
+-rw-r--r--   0 deo       (1000) users      (985)    31155 2021-04-09 21:46:50.000000 AaronTools-1.0b9/theory/job_types.py
+-rw-r--r--   0 deo       (1000) users      (985)     6101 2021-04-07 16:19:06.000000 AaronTools-1.0b9/theory/method.py
+-rw-r--r--   0 deo       (1000) users      (985)    59604 2021-04-15 20:12:45.000000 AaronTools-1.0b9/theory/theory.py
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.748122 AaronTools-1.0b9/theory/valid_basis_sets/
+-rw-r--r--   0 deo       (1000) users      (985)     2949 2021-03-29 21:37:44.000000 AaronTools-1.0b9/theory/valid_basis_sets/gaussian.txt
+-rw-r--r--   0 deo       (1000) users      (985)      188 2021-03-29 21:37:44.000000 AaronTools-1.0b9/theory/valid_basis_sets/gaussian_ecp.txt
+-rw-r--r--   0 deo       (1000) users      (985)     4853 2021-03-29 21:37:44.000000 AaronTools-1.0b9/theory/valid_basis_sets/orca.txt
+-rw-r--r--   0 deo       (1000) users      (985)       60 2021-03-29 21:37:44.000000 AaronTools-1.0b9/theory/valid_basis_sets/orca_ecp.txt
+-rw-r--r--   0 deo       (1000) users      (985)     8093 2021-03-29 21:37:44.000000 AaronTools-1.0b9/theory/valid_basis_sets/psi4.txt
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.748122 AaronTools-1.0b9/theory/valid_methods/
+-rw-r--r--   0 deo       (1000) users      (985)     2071 2021-03-29 21:37:44.000000 AaronTools-1.0b9/theory/valid_methods/gaussian.txt
+-rw-r--r--   0 deo       (1000) users      (985)     4296 2021-04-07 16:19:06.000000 AaronTools-1.0b9/theory/valid_methods/orca.txt
+-rw-r--r--   0 deo       (1000) users      (985)     3380 2021-04-07 16:19:06.000000 AaronTools-1.0b9/theory/valid_methods/psi4.txt
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.748122 AaronTools-1.0b9/utils/
+-rw-r--r--   0 deo       (1000) users      (985)        0 2020-11-18 22:59:34.000000 AaronTools-1.0b9/utils/__init__.py
+-rwxr-xr-x   0 deo       (1000) users      (985)     2596 2021-04-20 16:10:55.000000 AaronTools-1.0b9/utils/prime_numbers.py
+drwxr-xr-x   0 deo       (1000) users      (985)        0 2021-04-20 16:16:33.748122 AaronTools-1.0b9/utils/quad_grids/
+-rw-r--r--   0 deo       (1000) users      (985)     9240 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leb110.grid
+-rw-r--r--   0 deo       (1000) users      (985)   122136 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leb1454.grid
+-rw-r--r--   0 deo       (1000) users      (985)    16296 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leb194.grid
+-rw-r--r--   0 deo       (1000) users      (985)   170520 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leb2030.grid
+-rw-r--r--   0 deo       (1000) users      (985)   226968 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leb2702.grid
+-rw-r--r--   0 deo       (1000) users      (985)    25368 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leb302.grid
+-rw-r--r--   0 deo       (1000) users      (985)   488040 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leb5810.grid
+-rw-r--r--   0 deo       (1000) users      (985)    49560 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leb590.grid
+-rw-r--r--   0 deo       (1000) users      (985)    81816 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leb974.grid
+-rw-r--r--   0 deo       (1000) users      (985)     7788 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leg127.grid
+-rw-r--r--   0 deo       (1000) users      (985)     1066 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leg20.grid
+-rw-r--r--   0 deo       (1000) users      (985)     1696 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leg32.grid
+-rw-r--r--   0 deo       (1000) users      (985)     3387 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leg64.grid
+-rw-r--r--   0 deo       (1000) users      (985)     3957 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leg75.grid
+-rw-r--r--   0 deo       (1000) users      (985)     5233 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/Leg99.grid
+-rw-r--r--   0 deo       (1000) users      (985)      769 2020-11-17 22:04:01.000000 AaronTools-1.0b9/utils/quad_grids/NOTES
+-rw-r--r--   0 deo       (1000) users      (985)    20039 2021-04-20 16:11:48.000000 AaronTools-1.0b9/utils/utils.py
```

### Comparing `AaronTools-1.0b8/AaronTools.egg-info/PKG-INFO` & `AaronTools-1.0b9/AaronTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AaronTools
-Version: 1.0b8
+Version: 1.0b9
 Summary: Tools for measuring and manipulating molecular structures
 Home-page: https://github.com/QChASM/AaronTools.py
 Author: QChASM
 Author-email: qchasm@uga.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/QChASM/AaronTools.py/issues
 Project-URL: Source, https://github.com/QChASM/AaronTools.py
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AaronTools Version: 1.0b8 Summary: Tools for
+Metadata-Version: 2.1 Name: AaronTools Version: 1.0b9 Summary: Tools for
 measuring and manipulating molecular structures Home-page: https://github.com/
 QChASM/AaronTools.py Author: QChASM Author-email: qchasm@uga.edu License:
 UNKNOWN Project-URL: Bug Reports, https://github.com/QChASM/AaronTools.py/
 issues Project-URL: Source, https://github.com/QChASM/AaronTools.py
 Description: # AaronTools.py This Python implimentation of AaronTools provides
 a collection of tools for automating routine tasks encountered when running
 quantum chemistry computations. These tools can be used either directly within
```

### Comparing `AaronTools-1.0b8/LICENSE` & `AaronTools-1.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/AcAc.xyz` & `AaronTools-1.0b9/Ligands/AcAc.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/Ad-HC5C.xyz` & `AaronTools-1.0b9/Ligands/Ad-HC5C.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/BDA.xyz` & `AaronTools-1.0b9/Ligands/BDA.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/BPE.xyz` & `AaronTools-1.0b9/Ligands/BPE.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/BPY.xyz` & `AaronTools-1.0b9/Ligands/BPY.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/BenQuin.xyz` & `AaronTools-1.0b9/Ligands/BenQuin.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/BiOX.xyz` & `AaronTools-1.0b9/Ligands/BiOX.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/BiOx_Me.xyz` & `AaronTools-1.0b9/Ligands/BiOx_Me.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/COD.xyz` & `AaronTools-1.0b9/Ligands/COD.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/Cp_star.xyz` & `AaronTools-1.0b9/Ligands/Cp_star.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/DMBPY.xyz` & `AaronTools-1.0b9/Ligands/DMBPY.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/DMP.xyz` & `AaronTools-1.0b9/Ligands/DMP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/DMPE.xyz` & `AaronTools-1.0b9/Ligands/DMPE.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/DPEphos.xyz` & `AaronTools-1.0b9/Ligands/DPEphos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/DPPE.xyz` & `AaronTools-1.0b9/Ligands/DPPE.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/DPPF.xyz` & `AaronTools-1.0b9/Ligands/DPPF.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/DPPP.xyz` & `AaronTools-1.0b9/Ligands/DPPP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/EDA.xyz` & `AaronTools-1.0b9/Ligands/EDA.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/IMes.xyz` & `AaronTools-1.0b9/Ligands/IMes.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/JoshPhos.xyz` & `AaronTools-1.0b9/Ligands/JoshPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/KASBAI.xyz` & `AaronTools-1.0b9/Ligands/KASBAI.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/Mes-NC5C.xyz` & `AaronTools-1.0b9/Ligands/Mes-NC5C.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/Milstein.xyz` & `AaronTools-1.0b9/Ligands/Milstein.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/NBD.xyz` & `AaronTools-1.0b9/Ligands/NBD.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/PHNNP.xyz` & `AaronTools-1.0b9/Ligands/PHNNP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/PIN.xyz` & `AaronTools-1.0b9/Ligands/PIN.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/PPh3.xyz` & `AaronTools-1.0b9/Ligands/PPh3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/Paton_DL.xyz` & `AaronTools-1.0b9/Ligands/Paton_DL.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/Paton_EL.xyz` & `AaronTools-1.0b9/Ligands/Paton_EL.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/PhBP3.xyz` & `AaronTools-1.0b9/Ligands/PhBP3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/PymdOx.xyz` & `AaronTools-1.0b9/Ligands/PymdOx.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/PyrOx.xyz` & `AaronTools-1.0b9/Ligands/PyrOx.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-BINAP.xyz` & `AaronTools-1.0b9/Ligands/R-BINAP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-Me-StackPhos.xyz` & `AaronTools-1.0b9/Ligands/R-Me-StackPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-Ph-BOX.xyz` & `AaronTools-1.0b9/Ligands/R-Ph-BOX.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-Ph-Mes-NC5C.xyz` & `AaronTools-1.0b9/Ligands/R-Ph-Mes-NC5C.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-Quinox-AdtBu2.xyz` & `AaronTools-1.0b9/Ligands/R-Quinox-AdtBu2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-Quinox-tBu3.xyz` & `AaronTools-1.0b9/Ligands/R-Quinox-tBu3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-SEGPHOS.xyz` & `AaronTools-1.0b9/Ligands/R-SEGPHOS.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-StackPhos.xyz` & `AaronTools-1.0b9/Ligands/R-StackPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-iPr-PyBOX.xyz` & `AaronTools-1.0b9/Ligands/R-iPr-PyBOX.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-pFPh-StackPhos.xyz` & `AaronTools-1.0b9/Ligands/R-pFPh-StackPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R-tBu-BOX.xyz` & `AaronTools-1.0b9/Ligands/R-tBu-BOX.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-BDPP.xyz` & `AaronTools-1.0b9/Ligands/RR-BDPP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-BPCp.xyz` & `AaronTools-1.0b9/Ligands/RR-BPCp.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-Et-DuPhos.xyz` & `AaronTools-1.0b9/Ligands/RR-Et-DuPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-Me-BPE.xyz` & `AaronTools-1.0b9/Ligands/RR-Me-BPE.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-Me-DuPhos.xyz` & `AaronTools-1.0b9/Ligands/RR-Me-DuPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-Me-TBF.xyz` & `AaronTools-1.0b9/Ligands/RR-Me-TBF.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-Me-iPrPh-NC5C.xyz` & `AaronTools-1.0b9/Ligands/RR-Me-iPrPh-NC5C.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-QuinoxP.xyz` & `AaronTools-1.0b9/Ligands/RR-QuinoxP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-iPr-DuPhos.xyz` & `AaronTools-1.0b9/Ligands/RR-iPr-DuPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RR-norphos.xyz` & `AaronTools-1.0b9/Ligands/RR-norphos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/RRSS-DuanPhos.xyz` & `AaronTools-1.0b9/Ligands/RRSS-DuanPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/R_temp.xyz` & `AaronTools-1.0b9/Ligands/R_temp.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-BINAP.xyz` & `AaronTools-1.0b9/Ligands/S-BINAP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-Me-StackPhos.xyz` & `AaronTools-1.0b9/Ligands/S-Me-StackPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-Ph-BOX.xyz` & `AaronTools-1.0b9/Ligands/S-Ph-BOX.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-Ph-Mes-NC5C.xyz` & `AaronTools-1.0b9/Ligands/S-Ph-Mes-NC5C.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-Quinox-AdtBu2.xyz` & `AaronTools-1.0b9/Ligands/S-Quinox-AdtBu2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-Quinox-tBu3.xyz` & `AaronTools-1.0b9/Ligands/S-Quinox-tBu3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-SEGPHOS.xyz` & `AaronTools-1.0b9/Ligands/S-SEGPHOS.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-StackPhos.xyz` & `AaronTools-1.0b9/Ligands/S-StackPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-iPr-PyBOX.xyz` & `AaronTools-1.0b9/Ligands/S-iPr-PyBOX.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-pFPh-StackPhos.xyz` & `AaronTools-1.0b9/Ligands/S-pFPh-StackPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/S-tBu-BOX.xyz` & `AaronTools-1.0b9/Ligands/S-tBu-BOX.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SL-J212-1.xyz` & `AaronTools-1.0b9/Ligands/SL-J212-1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SL-J212-2.xyz` & `AaronTools-1.0b9/Ligands/SL-J212-2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-BDPP.xyz` & `AaronTools-1.0b9/Ligands/SS-BDPP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-BPCp.xyz` & `AaronTools-1.0b9/Ligands/SS-BPCp.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-Et-DuPhos.xyz` & `AaronTools-1.0b9/Ligands/SS-Et-DuPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-Me-BPE.xyz` & `AaronTools-1.0b9/Ligands/SS-Me-BPE.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-Me-DuPhos.xyz` & `AaronTools-1.0b9/Ligands/SS-Me-DuPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-Me-TBF.xyz` & `AaronTools-1.0b9/Ligands/SS-Me-TBF.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-Me-iPrPh-NC5C.xyz` & `AaronTools-1.0b9/Ligands/SS-Me-iPrPh-NC5C.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-QuinoxP.xyz` & `AaronTools-1.0b9/Ligands/SS-QuinoxP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-iPr-DuPhos.xyz` & `AaronTools-1.0b9/Ligands/SS-iPr-DuPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SS-norphos.xyz` & `AaronTools-1.0b9/Ligands/SS-norphos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/SSRR-DuanPhos.xyz` & `AaronTools-1.0b9/Ligands/SSRR-DuanPhos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/TACN.xyz` & `AaronTools-1.0b9/Ligands/TACN.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/TACN_star.xyz` & `AaronTools-1.0b9/Ligands/TACN_star.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/Tp.xyz` & `AaronTools-1.0b9/Ligands/Tp.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/Xantphos.xyz` & `AaronTools-1.0b9/Ligands/Xantphos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/Xphos.xyz` & `AaronTools-1.0b9/Ligands/Xphos.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/achiral_ligands` & `AaronTools-1.0b9/Ligands/achiral_ligands`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/bi-isoquinoline-NN-dioxide.xyz` & `AaronTools-1.0b9/Ligands/bi-isoquinoline-NN-dioxide.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/chiral_ligands` & `AaronTools-1.0b9/Ligands/chiral_ligands`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/dithiolate-4F.xyz` & `AaronTools-1.0b9/Ligands/dithiolate-4F.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/iPr-NC3C.xyz` & `AaronTools-1.0b9/Ligands/iPr-NC3C.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/iPr-PNPEt.xyz` & `AaronTools-1.0b9/Ligands/iPr-PNPEt.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/iPrPh-BIP.xyz` & `AaronTools-1.0b9/Ligands/iPrPh-BIP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/iPrPh-NC5C.xyz` & `AaronTools-1.0b9/Ligands/iPrPh-NC5C.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/squaramide-iPr.xyz` & `AaronTools-1.0b9/Ligands/squaramide-iPr.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/squaramide.xyz` & `AaronTools-1.0b9/Ligands/squaramide.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/tBu-PCP.xyz` & `AaronTools-1.0b9/Ligands/tBu-PCP.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Ligands/tBu-PNPPyr.xyz` & `AaronTools-1.0b9/Ligands/tBu-PNPPyr.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/PKG-INFO` & `AaronTools-1.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AaronTools
-Version: 1.0b8
+Version: 1.0b9
 Summary: Tools for measuring and manipulating molecular structures
 Home-page: https://github.com/QChASM/AaronTools.py
 Author: QChASM
 Author-email: qchasm@uga.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/QChASM/AaronTools.py/issues
 Project-URL: Source, https://github.com/QChASM/AaronTools.py
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AaronTools Version: 1.0b8 Summary: Tools for
+Metadata-Version: 2.1 Name: AaronTools Version: 1.0b9 Summary: Tools for
 measuring and manipulating molecular structures Home-page: https://github.com/
 QChASM/AaronTools.py Author: QChASM Author-email: qchasm@uga.edu License:
 UNKNOWN Project-URL: Bug Reports, https://github.com/QChASM/AaronTools.py/
 issues Project-URL: Source, https://github.com/QChASM/AaronTools.py
 Description: # AaronTools.py This Python implimentation of AaronTools provides
 a collection of tools for automating routine tasks encountered when running
 quantum chemistry computations. These tools can be used either directly within
```

### Comparing `AaronTools-1.0b8/README.md` & `AaronTools-1.0b9/README.md`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/benzene.xyz` & `AaronTools-1.0b9/Rings/benzene.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclohexane.1.xyz` & `AaronTools-1.0b9/Rings/cyclohexane.1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclohexane.xyz` & `AaronTools-1.0b9/Rings/cyclohexane.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentadiene.1.xyz` & `AaronTools-1.0b9/Rings/cyclopentadiene.1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentadiene.2.xyz` & `AaronTools-1.0b9/Rings/cyclopentadiene.2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentadiene.3.xyz` & `AaronTools-1.0b9/Rings/cyclopentadiene.3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentadiene.5.xyz` & `AaronTools-1.0b9/Rings/cyclopentadiene.5.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentadiene.6.xyz` & `AaronTools-1.0b9/Rings/cyclopentadiene.6.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentadiene.7.xyz` & `AaronTools-1.0b9/Rings/cyclopentadiene.7.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentane.1.xyz` & `AaronTools-1.0b9/Rings/cyclopentane.1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentane.2.xyz` & `AaronTools-1.0b9/Rings/cyclopentane.2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentane.3.xyz` & `AaronTools-1.0b9/Rings/cyclopentane.3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentane.4.xyz` & `AaronTools-1.0b9/Rings/cyclopentane.4.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/cyclopentane.xyz` & `AaronTools-1.0b9/Rings/cyclopentane.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/m-tetrahydropyran.1.xyz` & `AaronTools-1.0b9/Rings/m-tetrahydropyran.1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/m-tetrahydropyran.xyz` & `AaronTools-1.0b9/Rings/m-tetrahydropyran.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/o-tetrahydropyran.1.xyz` & `AaronTools-1.0b9/Rings/o-tetrahydropyran.1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Rings/o-tetrahydropyran.xyz` & `AaronTools-1.0b9/Rings/o-tetrahydropyran.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Substituents/26-F-Ph.xyz` & `AaronTools-1.0b9/Substituents/26-F-Ph.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Substituents/35-F-Ph.xyz` & `AaronTools-1.0b9/Substituents/35-F-Ph.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Substituents/Ad.xyz` & `AaronTools-1.0b9/Substituents/Ad.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Substituents/Cy.xyz` & `AaronTools-1.0b9/Substituents/Cy.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Substituents/Mes.xyz` & `AaronTools-1.0b9/Substituents/Mes.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Substituents/SuperMes.xyz` & `AaronTools-1.0b9/Substituents/SuperMes.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/Substituents/tBu.xyz` & `AaronTools-1.0b9/Substituents/tBu.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/angle.py` & `AaronTools-1.0b9/bin/angle.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,23 +166,23 @@
 
         out += "%f\n" % val
 
     out = out.rstrip()
 
     if len(args.set_ang) + len(args.change) > 0:
         if args.outfile:
-            geom.write(
-                append=True,
-                outfile=args.outfile.replace("$INFILE", get_filename(f))
-            )
+            outfile = args.outfile
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
+            geom.write(append=True, outfile=outfile)
         else:
             print(geom.write(outfile=False))
 
     if len(args.measure) > 0:
         if not args.outfile:
             print(out)
         else:
-            with open(
-                    args.outfile.replace("$INFILE", get_filename(f)),
-                    "a"
-            ) as f:
-                f.write(out)
+            outfile = args.outfile
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
+            with open(outfile, "a") as f:
+                f.write(out)
```

### Comparing `AaronTools-1.0b8/bin/bond.py` & `AaronTools-1.0b9/bin/bond.py`

 * *Files 9% similar despite different names*

```diff
@@ -141,23 +141,23 @@
         val = a1.dist(a2)
         out += "%f\n" % val
 
     out = out.rstrip()
 
     if len(args.set_ang) + len(args.change) > 0:
         if args.outfile:
-            geom.write(
-                append=True, 
-                outfile=args.outfile.replace("$INFILE", get_filename(f))
-            )
+            outfile = args.outfile
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
+            geom.write(append=True, outfile=outfile)
         else:
             print(geom.write(outfile=False))
 
     if len(args.measure) > 0:
         if not args.outfile:
             print(out)
         else:
-            with open(
-                    args.outfile.replace("$INFILE", get_filename(f)),
-                    "a"
-            ) as f:
+            outfile = args.outfile
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
+            with open(outfile, "a") as f:
                 f.write(out)
```

### Comparing `AaronTools-1.0b8/bin/changeChirality.py` & `AaronTools-1.0b9/bin/changeChirality.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/changeElement.py` & `AaronTools-1.0b9/bin/substituentSterimol.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,152 @@
 #!/usr/bin/env python3
 
-import sys
 import argparse
-from warnings import warn
+import sys
 
-from AaronTools.geometry import Geometry
 from AaronTools.fileIO import FileReader, read_types
-from AaronTools.utils.utils import get_filename
-
-vsepr_choices = [
-    "linear_1",
-    "linear_2",
-    "bent_2_planar",
-    "bent_2_tetrahedral",
-    "trigonal_planar",
-    "bent_3_tetrahedral",
-    "t_shaped",
-    "tetrahedral",
-    "sawhorse",
-    "square_planar",
-    "trigonal_bipyriamidal",
-    "square_pyramidal",
-    "octahedral",
-]
-
-element_parser = argparse.ArgumentParser(
-    description="change an element and/or adjust the VSEPR geometry",
-    formatter_class=argparse.RawTextHelpFormatter
-)
-
-element_parser.add_argument(
-    "infile",
-    metavar="input file",
-    type=str,
-    nargs="*",
-    default=[sys.stdin],
-    help="a coordinate file"
-)
-
-element_parser.add_argument(
-    "-o", "--output",
-    type=str,
-    default=False,
-    required=False,
-    dest="outfile",
-    help="output destination\n" +
-    "$INFILE will be replaced with the name of the input file\n" +
-    "Default: stdout"
-)
-
-element_parser.add_argument(
-    "-if", "--input-format",
-    type=str,
-    default=None,
-    dest="input_format",
-    choices=read_types,
-    help="file format of input - xyz is assumed if input is stdin"
-)
-
-element_parser.add_argument(
-    "-e", "--element",
-    metavar="target=element",
-    type=str,
-    action="append",
-    required=True,
-    dest="targets",
-    help="element to change into"
-)
-
-element_parser.add_argument(
-    "-b", "--fix-bonds",
-    action="store_true",
-    required=False,
-    dest="fix_bonds",
-    help="adjust bond lengths for the new element"
-)
-
-element_parser.add_argument(
-    "-c", "--change-hydrogens",
-    nargs="?",
-    required=False,
-    default=[None],
-    type=int,
-    dest="change_hs",
-    metavar=("N",),
-    help="change the number of hydrogens by the specified amount\n" +
-    "Specify nothing to automatically determine how many hydrogens\n" +
-    "to add or remove. If nothing is specified, the new geometry will\n" +
-    "also be determined automatically."
-)
-
-element_parser.add_argument(
-    "-g", "--geometry",
-    type=str,
-    default=None,
-    dest="geometry",
-    required=False,
-    help="specify the geometry to use with the new element\n" +
-    "if the argument is not supplied, the geometry will remain the same as\n" +
-    "the previous element's, unless necessitated by an increase in hydrogens\n" +
-    "Geometry can be:\n%s" % "".join(
-        s + ", " if (sum(len(x) for x in vsepr_choices[:i])) % 40 < 21 else s + ",\n"
-        for i, s in enumerate(vsepr_choices)
-    ).strip().strip(","),
-)
-
-args = element_parser.parse_args()
-
-fix_bonds = args.fix_bonds
-
-if args.change_hs is None:
-    adjust_structure = True
-    if args.geometry is not None:
-        warn(
-            "a geometry was specified, but geometry is determined automatically\n" +
-            "with the supplied arguments"
-        )
-else:
-    if isinstance(args.change_hs, int):
-        adjust_hs = args.change_hs
-    else:
-        adjust_hs = 0
-
-    new_vsepr = args.geometry.replace("_", " ")
-
-    if adjust_hs == 0 and new_vsepr is None:
-        adjust_structure = False
-    else:
-        adjust_structure = (adjust_hs, new_vsepr)
+from AaronTools.geometry import Geometry
+from AaronTools.substituent import Substituent
 
-for f in args.infile:
-    if isinstance(f, str):
-        if args.input_format is not None:
-            infile = FileReader((f, args.input_format, None))
+def main(argv):
+    sterimol_parser = argparse.ArgumentParser(
+        description="calculate B1-B5, and L sterimol parameters for substituents - see Verloop, A. and Tipker, J. (1976), Use of linear free energy related and other parameters in the study of fungicidal selectivity. Pestic. Sci., 7: 379-390.",
+        formatter_class=argparse.RawTextHelpFormatter
+    )
+    
+    sterimol_parser.add_argument(
+        "infile", metavar="input file",
+        type=str,
+        nargs="*",
+        default=[sys.stdin],
+        help="a coordinate file"
+    )
+    
+    sterimol_parser.add_argument(
+        "-if", "--input-format",
+        type=str,
+        default=None,
+        choices=read_types,
+        dest="input_format",
+        help="file format of input\nxyz is assumed if input is stdin"
+    )
+    
+    sterimol_parser.add_argument(
+        "-s", "--substituent-atom",
+        type=str,
+        required=True,
+        dest="targets",
+        help="substituent atom\n" +
+        "1-indexed position of the starting position of the\n" +
+        "substituent of which you are calculating sterimol\nparameters"
+    )
+    
+    sterimol_parser.add_argument(
+        "-a", "--attached-to",
+        type=str,
+        required=True,
+        dest="avoid",
+        help="non-substituent atom\n" +
+        "1-indexed position of the starting position of the atom\n" +
+        "connected to the substituent of which you are calculating\n" +
+        "sterimol parameters"
+    )
+    
+    sterimol_parser.add_argument(
+        "-r", "--radii",
+        type=str,
+        default="bondi",
+        choices=["bondi", "umn"],
+        dest="radii",
+        help="VDW radii to use in calculation\n" + 
+        "umn: main group vdw radii from J. Phys. Chem. A 2009, 113, 19, 5806–5812\n" +
+        "    (DOI: 10.1021/jp8111556)\n" + 
+        "    transition metals are crystal radii from Batsanov, S.S. Van der Waals\n" +
+        "    Radii of Elements. Inorganic Materials 37, 871–885 (2001).\n" +
+        "    (DOI: 10.1023/A:1011625728803)\n" + 
+        "bondi: radii from J. Phys. Chem. 1964, 68, 3, 441–451 (DOI: 10.1021/j100785a001)\n" +
+        "Default: bondi"
+    )
+    
+    sterimol_parser.add_argument(
+        "-l", "--old-l",
+        action="store_true",
+        required=False,
+        dest="old_L",
+        help="approximate FORTRAN Sterimol method for determining L\n"
+        "This is 0.4 + the ideal bond length for a target-H bond\n"
+        "Default: L value is from VDW radii of target atom to outer\n"
+        "VDW radii of atoms projected onto L-axis"
+    )
+    
+    sterimol_parser.add_argument(
+        "-v", "--vector",
+        action="store_true",
+        required=False,
+        dest="vector",
+        help="print Chimera/ChimeraX bild file for vectors instead of parameter values"
+    )
+    
+    sterimol_parser.add_argument(
+        "-o", "--output",
+        type=str,
+        default=False,
+        required=False,
+        metavar="output destination",
+        dest="outfile",
+        help="output destination\n" +
+        "Default: stdout"
+    )
+    
+    args = sterimol_parser.parse_args(args=argv)
+    
+    s = ""
+    if not args.vector:
+        s += "B1\tB2\tB3\tB4\tB5\tL\tfile\n"
+    
+    for infile in args.infile:
+        if isinstance(infile, str):
+            if args.input_format is not None:
+                f = FileReader((infile, args.input_format, infile))
+            else:
+                f = FileReader(infile)
         else:
-            infile = FileReader(f)
-    else:
-        if args.input_format is not None:
-            infile = FileReader(("from stdin", args.input_format, f))
+            if args.input_format is not None:
+                f = FileReader(("from stdin", args.input_format, infile))
+            else:
+                f = FileReader(("from stdin", "xyz", infile))
+    
+        geom = Geometry(f)
+        target = args.targets
+        avoid = args.avoid
+        end = geom.find(avoid)[0]
+        frag = geom.get_fragment(target, stop=end)
+        sub = Substituent(frag, end=end, detect=False)
+        data = sub.sterimol(return_vector=args.vector, radii=args.radii, old_L=args.old_L)
+        if args.vector:
+            for key, color in zip(
+                    ["B1", "B2", "B3", "B4", "B5", "L"],
+                    ["black", "green", "purple", "orange", "red", "blue"]
+            ):
+                start, end = data[key]
+                s += ".color %s\n" % color
+                s += ".note Sterimol %s\n" % key
+                s += ".arrow %6.3f %6.3f %6.3f   %6.3f %6.3f %6.3f\n" % (*start, *end)
         else:
-            if len(sys.argv) >= 1:
-                infile = FileReader(("from stdin", "xyz", f))
-
-    geom = Geometry(infile)
-
-    target_list = []
-    for sub in args.targets:
-        ndx_targets = sub.split("=")[0]
-        target_list.append(geom.find(ndx_targets))
-
-    for i, target in enumerate(target_list):
-        element = args.targets[i].split("=")[1]
-        # changeElement will only change one at a time
-        for single_target in target:
-            geom.change_element(
-                single_target,
-                element,
-                adjust_bonds=fix_bonds,
-                adjust_hydrogens=adjust_structure
+            s += "%.2f\t%.2f\t%.2f\t%.2f\t%.2f\t%.2f\t%s\n" % (
+                data["B1"],
+                data["B2"],
+                data["B3"],
+                data["B4"],
+                data["B5"],
+                data["L"],
+                infile,
             )
-
-    if args.outfile:
-        geom.write(
-            append=True, 
-            outfile=args.outfile.replace("$INFILE", get_filename(f))
-        )
+    
+    if not args.outfile:
+        print(s)
     else:
-        print(geom.write(outfile=False))
+        with open(args.outfile, "w") as f:
+            f.write(s)
+
+if __name__ == "__main__":
+    main(None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AaronTools-1.0b8/bin/closeRing.py` & `AaronTools-1.0b9/bin/closeRing.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,13 +133,13 @@
                 key,
                 ring_geom,
                 minimize=args.minimize,
                 flip_walk=args.flip,
             )
 
     if args.outfile:
-        geom.write(
-            append=True,
-            outfile=args.outfile.replace("$INFILE", get_filename(infile))
-        )
+        outfile = args.outfile
+        if "$INFILE" in outfile:
+            outfile = outfile.replace("$INFILE", get_filename(infile))
+        geom.write(append=True, outfile=outfile)
     else:
         print(geom.write(outfile=False))
```

### Comparing `AaronTools-1.0b8/bin/dihedral.py` & `AaronTools-1.0b9/bin/dihedral.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,23 +165,23 @@
 
         out += "%f\n" % val
 
     out = out.rstrip()
 
     if len(args.set_ang) + len(args.change) > 0:
         if args.outfile:
-            geom.write(
-                append=True, 
-                outfile=args.outfile.replace("$INFILE", get_filename(f))
-            )
+            outfile = args.outfile
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
+            geom.write(append=True, outfile=outfile)
         else:
             print(geom.write(outfile=False))
 
     if len(args.measure) > 0:
         if not args.outfile:
             print(out)
         else:
-            with open(
-                    args.outfile.replace("$INFILE", get_filename(f)),
-                    "a"
-            ) as f:
-                f.write(out)
+            outfile = args.outfile
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
+            with open(outfile, "a") as f:
+                f.write(out)
```

### Comparing `AaronTools-1.0b8/bin/fetchMolecule.py` & `AaronTools-1.0b9/bin/fetchMolecule.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/findAtoms.py` & `AaronTools-1.0b9/bin/findAtoms.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/follow.py` & `AaronTools-1.0b9/bin/follow.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,13 +244,12 @@
         followed_geom.comment = "following mode %s scaled to displace at most %s" % (
             repr(mode),
             repr(scale[i]),
         )
 
         outfile = outfiles[i]
         if args.outfile:
-            followed_geom.write(
-                append=True,
-                outfile=outfile.replace("$INFILE", get_filename(args.input_file))
-            )
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(args.input_file))
+            followed_geom.write(append=True, outfile=outfile)
         else:
             print(followed_geom.write(outfile=False))
```

### Comparing `AaronTools-1.0b8/bin/grabStatus.py` & `AaronTools-1.0b9/bin/grabStatus.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,42 +59,45 @@
         else:
             stat_parser.print_help()
             raise RuntimeError(
                 "when no input file is given, stdin is read and a format must be specified"
             )
 
     co = CompOutput(infile)
-    if not all(
+    if co.gradient.keys() and (
+        not all(
             x in header_vals for x in co.gradient.keys()
-    ) or not all(
-        x in co.gradient for x in header_vals
+        ) or not all(
+            x in co.gradient for x in header_vals
+        )
     ):
         header_vals = [x for x in sorted(co.gradient.keys())]
         header = "                      Filename    Step  " + "  ".join(
             ["%14s" % crit for crit in header_vals]
         )
         header += "\n"
         s += header
 
     s += "%30s" % f
     s += "%8s" % co.opt_steps
 
-    for crit in header_vals:
-        col = "%.2e/%s" % (
-            float(co.gradient[crit]["value"]), "YES" if co.gradient[crit]["converged"] else "NO"
-        )
-        s += "  %14s" % col
+    if co.gradient.keys():
+        for crit in header_vals:
+            col = "%.2e/%s" % (
+                float(co.gradient[crit]["value"]), "YES" if co.gradient[crit]["converged"] else "NO"
+            )
+            s += "  %14s" % col
 
     if (
             "error" in infile.other and
             infile.other["error"] is not None and
             infile.other["error"] != "UNKNOWN"
     ):
         s += "  %s" % infile.other["error_msg"]
-    elif not header_vals:
+    elif not co.gradient.keys():
         s += "  no progress found"
     elif co.finished:
         s += "  finished"
     else:
         s += "  not finished"
 
     s += "\n"
```

### Comparing `AaronTools-1.0b8/bin/grabThermo.py` & `AaronTools-1.0b9/bin/grabThermo.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,17 +232,18 @@
             [nrg_str] +
             ["%.6f" % x for x in therm] + \
             ["%.6f" % x for x in corrections] + \
             [sp_file if sp_file is not None else f, f]
         )
         output += "\n"
     else:
-        output += "electronic energy of %s = %.6f Eh\n" % (sp_file \
-                if sp_file is not None else f, \
-                nrg)
+        output += "electronic energy of %s = %.6f Eh\n" % (
+            sp_file if sp_file is not None else f, 
+            nrg
+        )
         output += "    E+ZPE             = %.6f Eh  (ZPE = %.6f)\n" % (nrg + co.ZPVE, co.ZPVE)
         output += "thermochemistry from %s at %.2f K:\n" % (f, t)
         output += "    H(RRHO)           = %.6f Eh  (dH = %.6f)\n" % (nrg + dH, dH)
         output += "    G(RRHO)           = %.6f Eh  (dG = %.6f)\n" % (nrg + rrho_dG, rrho_dG)
         output += "  quasi treatments for entropy (w0=%.1f cm^-1):\n" % args.w0
         output += "    G(Quasi-RRHO)     = %.6f Eh  (dG = %.6f)\n" % (nrg + qrrho_dG, qrrho_dG)
         output += "    G(Quasi-harmonic) = %.6f Eh  (dG = %.6f)\n" % (nrg + qharm_dG, qharm_dG)
```

### Comparing `AaronTools-1.0b8/bin/interpolate.py` & `AaronTools-1.0b9/bin/interpolate.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/jobSubmit.py` & `AaronTools-1.0b9/bin/jobSubmit.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from AaronTools.config import Config
 from AaronTools.job_control import SubmitProcess
 
 config = Config(quiet=True)
 
 default_proc = config.getint(
-    "Job", "processors", config.getint("Job", "procs", fallback=4)
+    "Job", "processors", fallback=config.getint("Job", "procs", fallback=4)
 )
 default_mem = config.getint("Job", "memory", fallback=8)
 default_walltime = config.getint("Job", "walltime", fallback=12)
 default_template = config.get("Job", "template", fallback=None)
 
 
 submit_parser = argparse.ArgumentParser(
```

### Comparing `AaronTools-1.0b8/bin/libaddLigand.py` & `AaronTools-1.0b9/bin/libaddLigand.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/libaddRing.py` & `AaronTools-1.0b9/bin/libaddRing.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/libaddSubstituent.py` & `AaronTools-1.0b9/bin/libaddSubstituent.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/listChanges.py` & `AaronTools-1.0b9/bin/listChanges.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/makeConf.py` & `AaronTools-1.0b9/bin/makeConf.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,18 +263,18 @@
                 outfile = os.path.join(
                     os.path.expanduser(args.outfile), "conformer-%i.xyz" % (conf + 1)
                 )
 
             else:
                 outfile = args.outfile.replace("$i", str(conf + 1))
 
-            print_geom.write(
-                outfile=outfile.replace("$INFILE", get_filename(infile)),
-                append="$i" not in args.outfile
-            )
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(infile))
+
+            print_geom.write(outfile=outfile, append="$i" not in args.outfile)
 
 
 if args.outfile is None or args.list_info:
     print(s[:-1])
 
 if skipped > 0:
     print("%i conformers skipped because of clashing substituent(s)" % skipped)
```

### Comparing `AaronTools-1.0b8/bin/makeInput.py` & `AaronTools-1.0b9/bin/makeInput.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 import sys
 from os.path import splitext
 import argparse
+from warnings import warn
 
 from AaronTools.geometry import Geometry
 from AaronTools.fileIO import FileReader, read_types
 from AaronTools.theory import *
 from AaronTools.utils.utils import combine_dicts, get_filename
 
 theory_parser = argparse.ArgumentParser(
@@ -738,24 +739,31 @@
 
     if args.use_prev and "other_kwargs" in infile.other:
         other_kwargs = combine_dicts(other_kwargs, infile.other["other_kwargs"])
 
     other_kwargs = combine_dicts(kwargs, other_kwargs)
 
     if args.outfile:
-        geom.write(
+        outfile = args.outfile
+        if "$INFILE" in outfile:
+            outfile = outfile.replace("$INFILE", get_filename(f))
+        warnings = geom.write(
             append=True,
-            outfile=args.outfile.replace("$INFILE", get_filename(f)),
+            outfile=outfile,
             style=style,
             theory=theory,
+            return_warnings=True,
             **other_kwargs
         )
     else:
-        print(
-            geom.write(
-                append=True,
-                outfile=False,
-                style=style,
-                theory=theory,
-                **other_kwargs
-            )
+        out, warnings = geom.write(
+            append=True,
+            outfile=False,
+            style=style,
+            theory=theory,
+            return_warnings=True,
+            **other_kwargs
         )
+        print(out)
+    
+    for warning in warnings:
+        warn(warning)
```

### Comparing `AaronTools-1.0b8/bin/mapLigand.py` & `AaronTools-1.0b9/bin/mapLigand.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
                     )
 
                 key.extend(cat.components["ligand"][j].key_atoms)
                 j += 1
 
             cat_copy.map_ligand(ligands, key)
 
-            if isinstance(args.outfile, str):
-                outfile = args.outfile.replace("$INFILE", get_filename(infile))
+            if args.outfile:
+                if "$INFILE" in args.outfile:
+                    outfile = args.outfile.replace("$INFILE", get_filename(infile))
                 outfile = outfile.replace("$LIGAND", lig_name)
                 cat_copy.write(append=False, outfile=outfile)
             else:
                 s = cat_copy.write(outfile=False)
                 print(s)
```

### Comparing `AaronTools-1.0b8/bin/mirror.py` & `AaronTools-1.0b9/bin/mirror.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,13 +97,13 @@
             infile = FileReader(("from stdin", "xyz", f))
 
     geom = Geometry(infile)
 
     geom.update_geometry(np.dot(geom.coords, eye))
 
     if args.outfile:
-        geom.write(
-            append=True, 
-            outfile=args.outfile.replace("$INFILE", get_filename(f))
-        )
+        outfile = args.outfile
+        if "$INFILE" in outfile:
+            outfile = outfile.replace("$INFILE", outfile)
+        geom.write(append=True, outfile=outfile)
     else:
         print(geom.write(outfile=False))
```

### Comparing `AaronTools-1.0b8/bin/parsePDF.py` & `AaronTools-1.0b9/bin/parsePDF.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/percentVolumeBuried.py` & `AaronTools-1.0b9/bin/percentVolumeBuried.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from AaronTools.geometry import Geometry
 from AaronTools.fileIO import FileReader, read_types
 from AaronTools.finders import NotAny
 
 
 vbur_parser = argparse.ArgumentParser(
-    description="calculated % volume buried in a sphere around a center atom",
+    description="calculated % volume buried in a sphere around a center atom - see Organometallics 2008, 27, 12, 2679–2681",
     formatter_class=argparse.RawTextHelpFormatter
 )
 
 vbur_parser.add_argument(
     "infile", metavar="input file",
     type=str,
     nargs="*",
@@ -67,15 +67,22 @@
 )
 
 vbur_parser.add_argument(
     "-v", "--vdw-radii",
     default="umn",
     choices=["umn", "bondi"],
     dest="radii",
-    help="VDW radii to use in calculation\nDefault: umn",
+    help="VDW radii to use in calculation\n" + 
+    "umn: main group vdw radii from J. Phys. Chem. A 2009, 113, 19, 5806–5812\n" +
+    "    (DOI: 10.1021/jp8111556)\n" + 
+    "    transition metals are crystal radii from Batsanov, S.S. Van der Waals\n" +
+    "    Radii of Elements. Inorganic Materials 37, 871–885 (2001).\n" +
+    "    (DOI: 10.1023/A:1011625728803)\n" + 
+    "bondi: radii from J. Phys. Chem. 1964, 68, 3, 441–451 (DOI: 10.1021/j100785a001)\n" +
+    "Default: umn",
 )
 
 vbur_parser.add_argument(
     "-s", "--scale",
     default=1.17,
     type=float,
     dest="scale",
@@ -92,25 +99,26 @@
 
 vbur_parser.add_argument(
     "-m", "--method",
     default="Lebedev",
     type=lambda x: x.capitalize() if x.lower() == "lebedev" else x.upper(),
     choices=["MC", "Lebedev"],
     dest="method",
-    help="integration method\nDefault: Lebedev"
+    help="integration method - Monte-Carlo (MC) or Lebedev quadrature (Lebedev)\nDefault: Lebedev"
 )
 
 grid_options = vbur_parser.add_argument_group("Lebedev integration options")
 grid_options.add_argument(
     "-rp", "--radial-points",
     type=int,
     default=20,
     choices=[20, 32, 64, 75, 99, 127],
     dest="rpoints",
-    help="number of radial shells for Lebedev integration\n" +
+    help="number of radial shells for Gauss-Legendre integration\n" +
+    "of the radial component\n" +
     "lower values are faster, but at the cost of accuracy\nDefault: 20"
 )
 
 grid_options.add_argument(
     "-ap", "--angular-points",
     type=int,
     default=1454,
```

### Comparing `AaronTools-1.0b8/bin/printFreq.py` & `AaronTools-1.0b9/bin/printFreq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 #! /usr/bin/env python3
-from AaronTools.comp_output import CompOutput
+from AaronTools.fileIO import FileReader
 
 
 def main(args):
-    comp = CompOutput(args.filename)
-    for i, key in enumerate(sorted(comp.frequency.by_frequency.keys())):
-        if args.type == "neg" and key > 0:
+    fr = FileReader(args.filename, just_geom=False)
+    if args.show:
+        s = "frequency\t"
+        for x in args.show:
+            if x == "vector":
+                continue
+            s += "%s\t" % x
+        print(s)
+    for i, data in enumerate(sorted(fr.other["frequency"].data, key=lambda x: x.frequency)):
+        if args.type == "neg" and data.frequency > 0:
             continue
-        if args.type == "pos" and key < 0:
+        if args.type == "pos" and data.frequency < 0:
             continue
-        if isinstance(args.type, int) and i > args.type:
+        if isinstance(args.type, int) and i + 1 > args.type:
             break
-        val = comp.frequency.by_frequency[key]
-        show = [val[x] for x in args.show if x != "vector"]
-        line = "{:9.4f}\t" + "{}\t" * len(show)
-        print(line.format(key, *show))
+        s = "%9.4f\t" % data.frequency
+        for x in args.show:
+            if x == "vector":
+                continue
+            val = getattr(data, x)
+            if isinstance(val, float):
+                s += "%9.4f\t" % val
+            else:
+                s += "%s\t" % str(val)
+        
+        print(s)
+        
         if "vector" in args.show:
-            print(val["vector"])
+            print(data.vector)
             print()
 
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser(
-        description="Prints frequencies from computational output file"
+        description="Prints frequencies from computational output file",
+        formatter_class=argparse.RawTextHelpFormatter,
     )
     parser.add_argument(
         "filename", help="Completed QM output file with frequency info"
     )
     parser.add_argument(
         "--type",
         "-t",
@@ -38,16 +54,17 @@
         default="all",
     )
     parser.add_argument(
         "--show",
         "-s",
         type=str,
         nargs="*",
-        help="Specify what additional information to show",
-        choices=["intensity", "vector"],
+        help="Specify what additional information to show\n"
+        "Some info may not be available for certain file formats",
+        choices=["intensity", "vector", "forcek", "symmetry"],
         default=[],
     )
     args = parser.parse_args()
     try:
         args.type = int(args.type)
     except ValueError:
         args.type = args.type.lower()
```

### Comparing `AaronTools-1.0b8/bin/printFreqBild.py` & `AaronTools-1.0b9/bin/printFreqBild.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/printInfo.py` & `AaronTools-1.0b9/bin/printInfo.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/bin/printXYZ.py` & `AaronTools-1.0b9/bin/printXYZ.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,20 +39,29 @@
     choices=read_types,
     help="file format of input - xyz is assumed if input is stdin"
 )
 
 xyz_parser.add_argument(
     "-c", "--comment",
     type=str,
-    default="",
+    default=None,
     required=False,
     dest="comment",
     help="comment line"
 )
 
+xyz_parser.add_argument(
+    "-a", "--append",
+    action="store_true",
+    default=False,
+    required=False,
+    dest="append",
+    help="append structures to output file if it already exists\nDefault: false"
+)
+
 args = xyz_parser.parse_args()
 
 for f in args.infile:
     if isinstance(f, str):
         if args.input_format is not None:
             infile = FileReader((f, args.input_format, None))
         else:
@@ -70,11 +79,11 @@
     else:
         geom.comment = f
 
 
     if not args.outfile:
         print(geom.write(outfile=False))
     else:
-        geom.write(
-            append=True,
-            outfile=args.outfile.replace("$INFILE", get_filename(f))
-        )
+        outfile = args.outfile
+        if "$INFILE" in outfile:
+            outfile = outfile.replace("$INFILE", get_filename(f))
+        geom.write(append=args.append, outfile=outfile)
```

### Comparing `AaronTools-1.0b8/bin/removeFragment.py` & `AaronTools-1.0b9/bin/removeFragment.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,13 +91,15 @@
     
     for atom in geom.find(args.target):
         if atom in geom.atoms:
             geom.remove_fragment(atom, avoid=args.avoid, add_H=args.add_H)
             if not args.add_H:
                 geom -= atom
     
-    if isinstance(args.outfile, str):
-        outfile = args.outfile.replace("$INFILE", get_filename(infile))
+    if args.outfile:
+        outfile = args.outfile
+        if "$INFILE" in outfile:
+            outfile = outfile.replace("$INFILE", get_filename(infile))
         geom.write(append=False, outfile=outfile)
     else:
         s = geom.write(outfile=False)
         print(s)
```

### Comparing `AaronTools-1.0b8/bin/rmsdAlign.py` & `AaronTools-1.0b9/bin/rmsdAlign.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,35 +191,35 @@
         sort=args.sort
     )
 
     geom.comment = "rmsd = %f" % rmsd
 
     if not args.value_only and not args.csv:
         if args.outfile:
-            geom.write(
-                append=True,
-                outfile=args.outfile.replace("$INFILE", get_filename(f))
-            )
+            outfile = args.outfile
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
+            geom.write(append=True, outfile=outfile)
         else:
             print(geom.write(outfile=False))
 
     elif args.value_only:
         if args.outfile:
-            with open(
-                    args.outfile.replace("$INFILE", get_filename(f)),
-                    "a"
-            ) as f:
+            outfile = args.outfile
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
+            with open(outfile, "a") as f:
                 f.write("%f\n" % rmsd)
 
         else:
             print("%f" % rmsd)
 
     elif args.csv:
         s = delim.join([ref_geom.name, geom.name, "%f" % rmsd])
         if args.outfile:
-            with open(
-                    args.outfile.replace("$INFILE", get_filename(f)),
-                    "a"
-            ) as f:
+            outfile = args.outfile
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
+            with open(outfile, "a") as f:
                 f.write(s + "\n")
         else:
             print(s)
```

### Comparing `AaronTools-1.0b8/bin/rotate.py` & `AaronTools-1.0b9/bin/rotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 from warnings import warn
 
 import numpy as np
 from AaronTools.fileIO import FileReader, read_types
 from AaronTools.geometry import Geometry
+from AaronTools.utils.utils import get_filename
 
 rotate_parser = argparse.ArgumentParser(
     description="rotate a fragment or molecule's coordinates",
     formatter_class=argparse.RawTextHelpFormatter,
 )
 
 rotate_parser.add_argument(
@@ -260,15 +261,16 @@
 
     rotated_geoms = []
     for i in range(0, args.num):
         geom.rotate(vector, args.angle, targets=targets, center=center)
 
         if args.outfile is not False:
             outfile = args.outfile
-            outfile = outfile.replace("$INFILE", os.path.basename(f))
+            if "$INFILE" in outfile:
+                outfile = outfile.replace("$INFILE", get_filename(f))
             outfile = outfile.replace(
                 "$AXIS", ".".join(["%.3f" % x for x in vector])
             )
             outfile = outfile.replace(
                 "$ANGLE",
                 str.zfill("%.2f" % np.rad2deg(args.angle * (i + 1)), 6),
             )
```

### Comparing `AaronTools-1.0b8/bin/stericMap.py` & `AaronTools-1.0b9/bin/stericMap.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,22 @@
 
 steric_parser.add_argument(
     "-v",
     "--vdw-radii",
     default="umn",
     choices=["umn", "bondi"],
     dest="radii",
-    help="VDW radii to use in calculation\nDefault: umn",
+    help="VDW radii to use in calculation\n" + 
+    "umn: main group vdw radii from J. Phys. Chem. A 2009, 113, 19, 5806–5812\n" +
+    "    (DOI: 10.1021/jp8111556)\n" + 
+    "    transition metals are crystal radii from Batsanov, S.S. Van der Waals\n" +
+    "    Radii of Elements. Inorganic Materials 37, 871–885 (2001).\n" +
+    "    (DOI: 10.1023/A:1011625728803)\n" + 
+    "bondi: radii from J. Phys. Chem. 1964, 68, 3, 441–451 (DOI: 10.1021/j100785a001)\n" +
+    "Default: umn",
 )
 
 steric_parser.add_argument(
     "-r",
     "--radius",
     default=3.5,
     type=float,
@@ -310,11 +317,11 @@
         ax.text(-0.9 * args.radius, +0.9 * args.radius, "%.1f%%" % vbur[1])
         ax.text(-0.9 * args.radius, -0.9 * args.radius, "%.1f%%" % vbur[2])
         ax.text(+0.7 * args.radius, -0.9 * args.radius, "%.1f%%" % vbur[3])
 
     if not args.outfile:
         plt.show()
     else:
-        plt.savefig(
-            args.outfile.replace("$INFILE", get_filename(f)),
-            dpi=500
-        )
+        outfile = args.outfile
+        if "$INFILE" in outfile:
+            outfile = outfile.replace("$INFILE", get_filename(f))
+        plt.savefig(outfile, dpi=500)
```

### Comparing `AaronTools-1.0b8/bin/substitute.py` & `AaronTools-1.0b9/bin/substitute.py`

 * *Files 8% similar despite different names*

```diff
@@ -130,13 +130,16 @@
                 sub = Substituent(sub_name)
 
             # replace old substituent with new substituent
             geom.substitute(sub, target, minimize=args.mini)
             geom.refresh_connected()
 
     if args.outfile:
+        outfile = args.outfile
+        if "INFILE" in outfile:
+            outfile = outfile.replace("$INFILE", get_filename(infile))
         geom.write(
             append=True,
-            outfile=args.outfile.replace("$INFILE", get_filename(infile))
+            outfile=outfile,
         )
     else:
         print(geom.write(outfile=False))
```

### Comparing `AaronTools-1.0b8/bin/translate.py` & `AaronTools-1.0b9/bin/translate.py`

 * *Files 5% similar despite different names*

```diff
@@ -192,13 +192,16 @@
         destination = np.zeros(3)
 
     translate_vector = destination - start
 
     geom.coord_shift(translate_vector, targets=targets)
 
     if args.outfile:
+        outfile = args.outfile
+        if "$INFILE" in outfile:
+            outfile = outfile.replace("$INFILE", get_filename(f))
         geom.write(
             append=True,
-            outfile=args.outfile.replace("$INFILE", get_filename(f))
+            outfile=outfile,
         )
     else:
         print(geom.write(outfile=False))
```

### Comparing `AaronTools-1.0b8/bin/unique.py` & `AaronTools-1.0b9/bin/unique.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/calculated_bond_lengths.json` & `AaronTools-1.0b9/calculated_bond_lengths.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/comp_output.py` & `AaronTools-1.0b9/comp_output.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 #! /usr/bin/env python3
 from collections.abc import MutableSequence
 
 import numpy as np
 
+from AaronTools import addlogger, getlogger
 from AaronTools.atoms import Atom
 from AaronTools.const import PHYSICAL, UNIT
 from AaronTools.fileIO import FileReader
 from AaronTools.geometry import Geometry
 from AaronTools.utils.utils import float_vec, uptri2sym
 
 
-def obj_to_dict(obj, skip_attrs=[]):
+def obj_to_dict(obj, skip_attrs=None):
+    # log = getlogger(level="debug")
+    if skip_attrs is None:
+        skip_attrs = []
+    if isinstance(obj, Geometry):
+        return obj.comment, [str(a) for a in obj]
     rv = {}
     if hasattr(obj, "__dict__"):
         for attr in obj.__dict__:
             if attr in skip_attrs:
                 continue
             val = getattr(obj, attr)
-            if isinstance(val, Geometry):
-                val = list(zip(val.elements, val.coords))
-            elif isinstance(val, MutableSequence):
+            if isinstance(val, MutableSequence):
                 val = [obj_to_dict(v) for v in val]
             else:
                 val = obj_to_dict(val)
-            if isinstance(val, dict):
-                tmp = {}
-                for k, v in val.items():
-                    tmp[str(k)] = v
-                val = tmp
             rv[str(attr)] = val
         return rv
-    else:
-        return obj
+    return obj
 
 
+@addlogger
 class CompOutput:
     """
     Attributes:
         geometry    the last Geometry
         opts        list of Geometry for each optimization steps
         frequency   Frequency object
         archive     a string containing the archive entry
@@ -47,16 +46,18 @@
         error, error_msg, finished,
         gradient, E_ZPVE, ZPVE
     """
 
     QUASI_HARMONIC = "QHARM"
     QUASI_RRHO = "QRRHO"
     RRHO = "RRHO"
+    LOG = None
+    LOGLEVEL = "debug"
 
-    def __init__(self, fname="", get_all=True):
+    def __init__(self, fname="", get_all=True, freq_name=None, conf_name=None):
         self.geometry = None
         self.opts = None
         self.opt_steps = None
         self.frequency = None
         self.archive = None
         self.other = None
         self.conformers = None
@@ -69,14 +70,15 @@
         self.multiplicity, self.charge = (None, None)
 
         self.rotational_temperature = None
         self.rotational_symmetry_number = None
 
         self.error, self.error_msg, self.finished = (None, None, None)
 
+        # these will be pulled out of FileReader.other dict
         keys = [
             "opt_steps",
             "energy",
             "error",
             "error_msg",
             "gradient",
             "finished",
@@ -91,30 +93,38 @@
             "ZPVE",
             "rotational_symmetry_number",
             "enthalpy",
             "archive",
         ]
 
         if isinstance(fname, (str, tuple)) and len(fname) > 0:
-            from_file = FileReader(fname, get_all, just_geom=False)
+            from_file = FileReader(
+                fname,
+                get_all,
+                just_geom=False,
+                freq_name=freq_name,
+                conf_name=conf_name,
+            )
         elif isinstance(fname, FileReader):
             from_file = fname
         else:
             return
 
         if from_file.atoms:
-            self.geometry = Geometry(from_file)
+            self.geometry = Geometry(
+                from_file.atoms, comment=from_file.comment
+            )
         if from_file.all_geom:
             self.opts = []
             for g in from_file.all_geom:
                 self.opts += [Geometry(g[0])]
         if "conformers" in from_file.other:
             self.conformers = []
             for comment, atoms in from_file.other["conformers"]:
-                self.conformers += [Geometry(atoms, comment=comment)]
+                self.conformers.append(Geometry(atoms, comment=comment))
             del from_file.other["conformers"]
 
         for k in keys:
             if k in from_file.other:
                 self.__setattr__(k, from_file.other[k])
                 del from_file.other[k]
         self.other = from_file.other
@@ -125,15 +135,15 @@
         if self.frequency:
             self.grimme_g = self.calc_Grimme_G()
             # recalculate ZPVE b/c our constants and the ones in various programs
             # might be slightly different
             self.ZPVE = self.calc_zpe()
             self.E_ZPVE = self.energy + self.ZPVE
 
-    def to_dict(self, skip_attrs=[]):
+    def to_dict(self, skip_attrs=None):
         return obj_to_dict(self, skip_attrs=skip_attrs)
 
     def get_progress(self):
         rv = ""
         grad = self.gradient
         if not grad:
             rv += "Progress not found"
@@ -152,23 +162,30 @@
         """returns ZPVE correction"""
         hc = PHYSICAL.PLANCK * PHYSICAL.SPEED_OF_LIGHT / UNIT.HART_TO_JOULE
         vib = sum(self.frequency.real_frequencies)
         zpve = 0.5 * hc * vib
         return zpve
 
     def therm_corr(self, temperature=None, v0=100, method="RRHO"):
-        """returns thermal correction to energy, enthalpy correction to energy, and entropy
+        """
+        returns thermal correction to energy, enthalpy correction to energy, and entropy
         for the specified cutoff frequency and temperature
         in that order (Hartrees for corrections, Eh/K for entropy)
 
-        temperature     -   float/None               temperature in K, None will use self.temperature
-        v0              -   float/100                cutoff for quasi G corrections
-        method          -   str/RRHO, QRRHO, QHARM   type of quasi treatment (RRHO  - no quasi treatment
-                                                                              QRRHO - Grimme's quasi-RRHO
-                                                                              QHARM - Truhlar's quasi-harmonic)
+        temperature: float, temperature in K- None will use self.temperature
+        v0: float, cutoff/damping parameter for quasi G corrections
+        method: str - type of quasi treatment:
+                RRHO  - no quasi treatment
+                QRRHO - Grimme's quasi-RRHO
+                see Grimme, S. (2012), Supramolecular Binding Thermodynamics by
+                Dispersion‐Corrected Density Functional Theory. Chem. Eur. J.,
+                18: 9955-9964. (DOI: 10.1002/chem.201200497) for details
+                QHARM - Truhlar's quasi-harmonic
+                see J. Phys. Chem. B 2011, 115, 49, 14556–14562
+                (DOI: 10.1021/jp205508z) for details
         """
         if self.frequency is None:
             msg = "Vibrational frequencies not found, "
             msg += "cannot calculate vibrational entropy."
             raise AttributeError(msg)
 
         rot = [temp for temp in self.rotational_temperature if temp != 0]
@@ -182,21 +199,27 @@
             sigmar = 3
         mult = self.multiplicity
         freqs = np.array(self.frequency.real_frequencies)
 
         vib_unit_convert = (
             PHYSICAL.SPEED_OF_LIGHT * PHYSICAL.PLANCK / PHYSICAL.KB
         )
-        vibtemps = np.array([f_i * vib_unit_convert for f_i in freqs if f_i > 0])
+        vibtemps = np.array(
+            [f_i * vib_unit_convert for f_i in freqs if f_i > 0]
+        )
         if method == "QHARM":
-            harm_vibtemps = np.array([
-                f_i * vib_unit_convert if f_i > v0 else v0 * vib_unit_convert
-                for f_i in freqs
-                if f_i > 0
-            ])
+            harm_vibtemps = np.array(
+                [
+                    f_i * vib_unit_convert
+                    if f_i > v0
+                    else v0 * vib_unit_convert
+                    for f_i in freqs
+                    if f_i > 0
+                ]
+            )
         else:
             harm_vibtemps = vibtemps
 
         Bav = PHYSICAL.PLANCK ** 2 / (24 * np.pi ** 2 * PHYSICAL.KB)
         Bav *= sum([1 / r for r in rot])
 
         # Translational
@@ -232,23 +255,21 @@
             Er = 0
         else:
             Er = len(rot) * PHYSICAL.GAS_CONSTANT * T / 2
 
         # Vibrational
         if method == self.QUASI_HARMONIC:
             Sv = np.sum(
-                harm_vibtemps / (
-                    T * (np.exp(harm_vibtemps / T) - 1)
-                ) - np.log(1 - np.exp(-harm_vibtemps / T))
+                harm_vibtemps / (T * (np.exp(harm_vibtemps / T) - 1))
+                - np.log(1 - np.exp(-harm_vibtemps / T))
             )
         elif method == self.RRHO:
             Sv = np.sum(
-                vibtemps / (
-                    T * (np.exp(vibtemps / T) - 1)
-                ) - np.log(1 - np.exp(-vibtemps / T))
+                vibtemps / (T * (np.exp(vibtemps / T) - 1))
+                - np.log(1 - np.exp(-vibtemps / T))
             )
         elif method == self.QUASI_RRHO:
             mu = PHYSICAL.PLANCK
             mu /= 8 * np.pi ** 2 * freqs * PHYSICAL.SPEED_OF_LIGHT
             mu = mu * Bav / (mu + Bav)
             Sr_eff = 1 / 2 + np.log(
                 np.sqrt(
@@ -260,19 +281,20 @@
                     / PHYSICAL.PLANCK ** 2
                 )
             )
 
             weights = weight = 1 / (1 + (v0 / freqs) ** 4)
 
             Sv = np.sum(
-                weights * (
-                    harm_vibtemps / (
-                        T * (np.exp(harm_vibtemps / T) - 1)
-                    ) - np.log(1 - np.exp(-harm_vibtemps / T))
-                ) + (1 - weights) * Sr_eff
+                weights
+                * (
+                    harm_vibtemps / (T * (np.exp(harm_vibtemps / T) - 1))
+                    - np.log(1 - np.exp(-harm_vibtemps / T))
+                )
+                + (1 - weights) * Sr_eff
             )
 
         Ev = np.sum(vibtemps * (1.0 / 2 + 1 / (np.exp(vibtemps / T) - 1)))
 
         Ev *= PHYSICAL.GAS_CONSTANT
         Sv *= PHYSICAL.GAS_CONSTANT
 
@@ -281,26 +303,34 @@
             PHYSICAL.GAS_CONSTANT * T / (UNIT.HART_TO_KCAL * 1000)
         )
         Stot = (St + Sr + Sv + Se) / (UNIT.HART_TO_KCAL * 1000)
 
         return Ecorr, Hcorr, Stot
 
     def calc_G_corr(self, temperature=None, v0=0, method="RRHO"):
-        """returns quasi rrho free energy correction (Eh)
-        temperature     -   float/None              temperature; default is self.temperature
-        v0              -   cutoff                  for quasi-rrho or quasi-harmonic entropy
-        method          -   str/RRHO, QRRHO, QHARM  method for treating entropy"""
+        """
+        returns quasi rrho free energy correction (Eh)
+        temperature: float, temperature; default is self.temperature
+        v0: float, parameter for quasi-rrho or quasi-harmonic entropy
+        method: str (RRHO, QRRHO, QHARM) method for treating entropy
+                see CompOutput.therm_corr for references
+        """
         Ecorr, Hcorr, Stot = self.therm_corr(temperature, v0, method)
         T = temperature if temperature is not None else self.temperature
         Gcorr_qRRHO = Hcorr - T * Stot
 
         return Gcorr_qRRHO
 
     def calc_Grimme_G(self, temperature=None, v0=100):
-        """returns quasi rrho free energy (Eh)"""
+        """
+        returns quasi rrho free energy (Eh)
+        see Grimme, S. (2012), Supramolecular Binding Thermodynamics by
+        Dispersion‐Corrected Density Functional Theory. Chem. Eur. J.,
+        18: 9955-9964. (DOI: 10.1002/chem.201200497) for details
+        """
         Gcorr_qRRHO = self.calc_G_corr(
             temperature=temperature, v0=v0, method=self.QUASI_RRHO
         )
         return Gcorr_qRRHO + self.energy
 
     def bond_change(self, atom1, atom2, threshold=0.25):
         """"""
@@ -417,16 +447,16 @@
         return geom
 
     def compute_rot_temps(self):
         """sets self's 'rotational_temperature' attribute by using self.geometry
         not recommended b/c atoms should be specific isotopes, but this uses
         average atomic weights
         exists because older versions of ORCA don't print rotational temperatures"""
-        self.geometry.coord_shift(-self.geometry.COM(mass_weight=True))
-
+        COM = self.geometry.COM(mass_weight=True)
+        self.geometry.coord_shift(-COM)
         inertia_mat = np.zeros((3, 3))
         for atom in self.geometry.atoms:
             for i in range(0, 3):
                 for j in range(0, 3):
                     if i == j:
                         inertia_mat[i][j] += sum(
                             [
@@ -450,7 +480,9 @@
             for moment in principal_inertia
             if moment > 0
         ]
 
         self.rotational_temperature = [
             PHYSICAL.PLANCK * const / PHYSICAL.KB for const in rot_consts
         ]
+        # shift geometry back
+        self.geometry.coord_shift(COM)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AaronTools-1.0b8/component.py` & `AaronTools-1.0b9/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """For more complicated geometry manipulation and complex building"""
 import os
 import re
 from glob import glob
+
 import numpy as np
 
-from AaronTools.const import AARONLIB, AARONTOOLS, VDW_RADII, BONDI_RADII
+from AaronTools.const import AARONLIB, AARONTOOLS, BONDI_RADII, VDW_RADII
+from AaronTools.fileIO import read_types
+from AaronTools.finders import BondedTo, CloserTo
 from AaronTools.geometry import Geometry
 from AaronTools.substituent import Substituent
-from AaronTools.finders import BondedTo, CloserTo
-from AaronTools.fileIO import read_types
 from AaronTools.utils.utils import get_filename
 
+
 class Component(Geometry):
     """
     Attributes:
     :name:          str
     :comment:       str
     :atoms:         list(Atom)
     :other:         dict()
@@ -45,30 +47,30 @@
         self.substituents = None
         self.backbone = None
         self.key_atoms = []
 
         if isinstance(structure, str) and not os.access(structure, os.R_OK):
             for ext in read_types:
                 if structure.endswith(".%s" % ext):
-                    structure = structure[:-(1 + len(ext))]
+                    structure = structure[: -(1 + len(ext))]
 
             for lib in [Component.AARON_LIBS, Component.BUILTIN]:
                 if not os.path.exists(lib):
                     continue
                 flig = None
                 for f in os.listdir(lib):
                     name, ext = os.path.splitext(f)
                     if not any(".%s" % x == ext for x in read_types):
                         continue
-                    
+
                     match = structure == name
                     if match:
                         flig = os.path.join(lib, f)
                         break
-                    
+
                 if flig:
                     break
             else:
                 raise FileNotFoundError(
                     "Cannot find ligand in library:", structure
                 )
             structure = flig
@@ -98,64 +100,67 @@
             return len(self) < len(other)
         for a, b in zip(sorted(self.atoms), sorted(other.atoms)):
             if a < b:
                 return True
         return False
 
     @classmethod
-    def list(cls,
-            name_regex=None,
-            coordinating_elements=None,
-            denticity=None,
-            include_ext=False,
+    def list(
+        cls,
+        name_regex=None,
+        coordinating_elements=None,
+        denticity=None,
+        include_ext=False,
     ):
         names = []
         for lib in [cls.AARON_LIBS, cls.BUILTIN]:
             if not os.path.exists(lib):
                 continue
             for f in os.listdir(lib):
                 name, ext = os.path.splitext(f)
                 if not any(".%s" % x == ext for x in read_types):
                     continue
-                
+
                 if name in names:
                     continue
-                
+
                 name_ok = True
                 elements_ok = True
                 denticity_ok = True
-    
+
                 if (
                     name_regex is not None
                     and re.search(name_regex, name, re.IGNORECASE) is None
                 ):
                     name_ok = False
-    
+
                 if coordinating_elements is not None:
                     geom = Geometry(
                         os.path.join(lib, name + ext),
                         refresh_connected=False,
                         refresh_ranks=False,
                     )
                     # geom = cls(name)
-                    elements = [geom.atoms[i].element for i in geom.other["key_atoms"]]
+                    elements = [
+                        geom.atoms[i].element for i in geom.other["key_atoms"]
+                    ]
                     if not all(
                         elements.count(x) == coordinating_elements.count(x)
                         for x in coordinating_elements
                     ) or not all(
                         coordinating_elements.count(x) == elements.count(x)
                         for x in elements
                     ):
                         elements_ok = False
-    
+
                 if denticity is not None:
                     geom = cls(name)
                     if len(geom.find("key")) != denticity:
                         denticity_ok = False
-    
+
                 if name_ok and elements_ok and denticity_ok:
                     if include_ext:
                         names.append(name + ext)
                     else:
                         names.append(name)
 
         return names
@@ -350,32 +355,43 @@
             angle = sub.conf_angle
         if not angle:
             return
         self.change_dihedral(
             start, end, angle, fix=4, adjust=True, as_group=True
         )
 
-    def cone_angle(self, center, method="exact", return_cones=False, radii="umn"):
+    def cone_angle(
+        self, center=None, method="exact", return_cones=False, radii="umn"
+    ):
         """
         returns cone angle in degrees
         center - Atom() that this component is coordinating
                  used as the apex of the cone
         method (str) can be:
-            'Tolman' - Tolman cone angle for asymmetric ligands (doi 10.1021/ja00808a009)
+            'Tolman' - Tolman cone angle for asymmetric ligands 
+                       See J. Am. Chem. Soc. 1974, 96, 1, 53–60 (DOI: 10.1021/ja00808a009)
                        NOTE: this does not make assumptions about the geometry
                        NOTE: only works with monodentate and bidentate ligands
-            'exact' - cone angle from Allen et. al. (doi 10.1002/jcc.23217)
+            'exact' - cone angle from Allen et. al. 
+                      See Bilbrey, J.A., Kazez, A.H., Locklin, J. and Allen, W.D. 
+                      (2013), Exact ligand cone angles. J. Comput. Chem., 34: 
+                      1189-1197. (DOI: 10.1002/jcc.23217)
         return_cones - return cone apex, center of base, and base radius list
                        the sides of the cones will be 5 angstroms long
                        for Tolman cone angles, multiple cones will be returned, one for
                        each substituent coming off the coordinating atom
         radii: 'bondi' - Bondi vdW radii
                'umn'   - vdW radii from Mantina, Chamberlin, Valero, Cramer, and Truhlar
                dict() with elements as keys and radii as values
         """
+        if method.lower() == "tolman":
+            CITATION = "doi:10.1021/ja00808a009"
+        elif method.lower() == "exact":
+            CITATION = "doi:10.1002/jcc.23217"
+        self.LOG.citation(CITATION)
 
         key = self.find("key")
 
         center = self.find_exact(center)[0]
 
         L_axis = self.COM(key) - center.coords
         L_axis /= np.linalg.norm(L_axis)
@@ -401,15 +417,15 @@
                 key1, key2 = key
                 try:
                     bridge_path = self.shortest_path(key1, key2)
                 except LookupError:
                     bridge_path = False
 
             for key_atom in key:
-                L_axis =  key_atom.coords - center.coords
+                L_axis = key_atom.coords - center.coords
                 L_axis /= np.linalg.norm(L_axis)
                 bonded_atoms = self.find(BondedTo(key_atom))
                 for bonded_atom in bonded_atoms:
                     frag = self.get_fragment(bonded_atom, key_atom)
 
                     use_bridge = False
                     if any(k in frag for k in key):
@@ -436,42 +452,46 @@
                             if bridge_path:
                                 if key_atom is key1:
                                     other_key = key2
                                 else:
                                     other_key = key1
                                 frag = self.find(
                                     frag,
-                                    CloserTo(key_atom, other_key, include_ties=True)
+                                    CloserTo(
+                                        key_atom, other_key, include_ties=True
+                                    ),
                                 )
 
                         # some ligands like DuPhos have rings on the phosphorous atom
                         # we only want ones that are closer to the the substituent end
                         frag = self.find(frag, CloserTo(bonded_atom, key_atom))
 
                         # Geometry(frag).write(outfile="frag%s.xyz" % bonded_atom.name)
 
                         for atom in frag:
-                            beta = np.arcsin(radii_dict[atom.element] / atom.dist(center))
+                            beta = np.arcsin(
+                                radii_dict[atom.element] / atom.dist(center)
+                            )
                             v = center.bond(atom) / center.dist(atom)
                             c = np.linalg.norm(v - L_axis)
                             test_angle = beta + np.arccos((c ** 2 - 2) / -2)
 
-                            if tolman_angle is None or test_angle > tolman_angle:
+                            if (
+                                tolman_angle is None
+                                or test_angle > tolman_angle
+                            ):
                                 tolman_angle = test_angle
 
                     scale = 5 * np.cos(tolman_angle)
 
                     cones.append(
                         (
-                            (
-                                center.coords + scale * L_axis if 2 * tolman_angle < np.pi
-                                else center.coords - scale * L_axis
-                            ),
+                            center.coords + scale * L_axis,
                             center.coords,
-                            scale * abs(np.tan(tolman_angle))
+                            scale * abs(np.tan(tolman_angle)),
                         )
                     )
 
                     total_angle += 2 * tolman_angle / len(bonded_atoms)
 
             if return_cones:
                 return np.rad2deg(total_angle), cones
@@ -480,35 +500,37 @@
 
         elif method.lower() == "exact":
             beta = np.zeros(len(self.atoms), dtype=float)
 
             test_one_atom_axis = None
             max_beta = None
             for i, atom in enumerate(self.atoms):
-                beta[i] = np.arcsin(radii_dict[atom.element] / atom.dist(center))
+                beta[i] = np.arcsin(
+                    radii_dict[atom.element] / atom.dist(center)
+                )
                 if max_beta is None or beta[i] > max_beta:
                     max_beta = beta[i]
                     test_one_atom_axis = center.bond(atom)
 
             # check to see if all other atoms are in the shadow of one atom
             # e.g. cyano, carbonyl
             overshadowed_list = []
             for i, atom in enumerate(self.atoms):
                 rhs = beta[i]
 
-                if np.dot(
-                        center.bond(atom), test_one_atom_axis
-                ) / (
-                        center.dist(atom) * np.linalg.norm(test_one_atom_axis)
-                ) <= 1:
+                if (
+                    np.dot(center.bond(atom), test_one_atom_axis)
+                    / (center.dist(atom) * np.linalg.norm(test_one_atom_axis))
+                    <= 1
+                ):
                     rhs += np.arccos(
-                        np.dot(
-                            center.bond(atom), test_one_atom_axis
-                        ) / (
-                            center.dist(atom) * np.linalg.norm(test_one_atom_axis)
+                        np.dot(center.bond(atom), test_one_atom_axis)
+                        / (
+                            center.dist(atom)
+                            * np.linalg.norm(test_one_atom_axis)
                         )
                     )
                 lhs = max_beta
                 if lhs >= rhs:
                     # print(atom, "is overshadowed")
                     overshadowed_list.append(atom)
                     break
@@ -517,62 +539,62 @@
             if len(overshadowed_list) == len(self.atoms):
                 scale = 5 * np.cos(max_beta)
 
                 cones.append(
                     (
                         center.coords + scale * test_one_atom_axis,
                         center.coords,
-                        scale * abs(np.linalg.norm(test_one_atom_axis) * np.tan(max_beta))
+                        scale
+                        * abs(
+                            np.linalg.norm(test_one_atom_axis)
+                            * np.tan(max_beta)
+                        ),
                     )
                 )
 
                 if return_cones:
                     return np.rad2deg(2 * max_beta), cones
 
                 return np.rad2deg(2 * max_beta)
 
             overshadowed_list = []
             for i, atom1 in enumerate(self.atoms):
                 for j, atom2 in enumerate(self.atoms[:i]):
                     rhs = beta[i]
 
-                    if np.dot(
-                            center.bond(atom1), center.bond(atom2)
-                        ) / (
-                            center.dist(atom1) * center.dist(atom2)
-                    ) <= 1:
+                    if (
+                        np.dot(center.bond(atom1), center.bond(atom2))
+                        / (center.dist(atom1) * center.dist(atom2))
+                        <= 1
+                    ):
                         rhs += np.arccos(
-                            np.dot(
-                                center.bond(atom1), center.bond(atom2)
-                            ) / (
-                                center.dist(atom1) * center.dist(atom2)
-                            )
+                            np.dot(center.bond(atom1), center.bond(atom2))
+                            / (center.dist(atom1) * center.dist(atom2))
                         )
                     lhs = beta[j]
                     if lhs >= rhs:
                         overshadowed_list.append(atom1)
                         break
             # winow list to ones that aren't in the shadow of another
-            atom_list = [atom for atom in self.atoms if atom not in overshadowed_list]
+            atom_list = [
+                atom for atom in self.atoms if atom not in overshadowed_list
+            ]
 
             # check pairs of atoms
             max_a = None
             aij = None
             bij = None
             cij = None
             for i, atom1 in enumerate(atom_list):
                 ndx_i = self.atoms.index(atom1)
                 for j, atom2 in enumerate(atom_list[:i]):
                     ndx_j = self.atoms.index(atom2)
                     beta_ij = np.arccos(
-                        np.dot(
-                            center.bond(atom1), center.bond(atom2)
-                        ) / (
-                            atom1.dist(center) * atom2.dist(center)
-                        )
+                        np.dot(center.bond(atom1), center.bond(atom2))
+                        / (atom1.dist(center) * atom2.dist(center))
                     )
 
                     test_alpha = (beta[ndx_i] + beta[ndx_j] + beta_ij) / 2
                     if max_a is None or test_alpha > max_a:
                         max_a = test_alpha
                         mi = center.bond(atom1)
                         mi /= np.linalg.norm(mi)
@@ -582,41 +604,47 @@
                         aij = np.sin(
                             0.5 * (beta_ij + beta[ndx_i] - beta[ndx_j])
                         ) / np.sin(beta_ij)
                         bij = np.sin(
                             0.5 * (beta_ij - beta[ndx_i] + beta[ndx_j])
                         ) / np.sin(beta_ij)
                         cij = 0
-                        norm = aij * mi + bij * mj + cij * np.cross(mi, mj) / np.sin(bij)
+                        norm = (
+                            aij * mi
+                            + bij * mj
+                            + cij * np.cross(mi, mj) / np.sin(bij)
+                        )
 
             # r = 0.2 * np.tan(max_a)
             # print(
             #     ".cone %.3f %.3f %.3f   0.0 0.0 0.0   %.3f open" % (
             #         0.2 * norm[0], 0.2 * norm[1], 0.2 * norm[2], r
             #     )
             # )
 
             overshadowed_list = []
             rhs = max_a
             for atom in atom_list:
                 ndx_i = self.atoms.index(atom)
-                lhs = beta[ndx_i] + np.arccos(np.dot(center.bond(atom), norm) / center.dist(atom))
+                lhs = beta[ndx_i] + np.arccos(
+                    np.dot(center.bond(atom), norm) / center.dist(atom)
+                )
                 # this should be >=, but there can be numerical issues
                 if rhs > lhs or np.isclose(rhs, lhs):
                     overshadowed_list.append(atom)
 
             # the cone fits all atoms, we're done
             if len(overshadowed_list) == len(atom_list):
                 scale = 5 * np.cos(max_a)
 
                 cones.append(
                     (
                         center.coords + (scale * norm),
                         center.coords,
-                        scale * abs(np.tan(max_a))
+                        scale * abs(np.tan(max_a)),
                     )
                 )
 
                 if return_cones:
                     return np.rad2deg(2 * max_a), cones
 
                 return np.rad2deg(2 * max_a)
@@ -625,15 +653,15 @@
             c_vec = centroid - center.coords
             c_vec /= np.linalg.norm(c_vec)
 
             min_alpha = None
             c = 0
             for i, atom1 in enumerate(atom_list):
                 for j, atom2 in enumerate(atom_list[:i]):
-                    for k, atom3 in enumerate(atom_list[i+1:]):
+                    for k, atom3 in enumerate(atom_list[i + 1 :]):
                         c += 1
                         ndx_i = self.atoms.index(atom1)
                         ndx_j = self.atoms.index(atom2)
                         ndx_k = self.atoms.index(atom3)
                         # print(atom1.name, atom2.name, atom3.name)
 
                         mi = center.bond(atom1)
@@ -649,31 +677,31 @@
 
                         # N = gamma_ijk * np.linalg.inv(M)
 
                         N = np.column_stack(
                             (
                                 np.cross(mj, mk),
                                 np.cross(mk, mi),
-                                np.cross(mi, mj)
+                                np.cross(mi, mj),
                             )
                         )
 
                         u = np.array(
                             [
                                 np.cos(beta[ndx_i]),
                                 np.cos(beta[ndx_j]),
-                                np.cos(beta[ndx_k])
+                                np.cos(beta[ndx_k]),
                             ]
                         )
 
                         v = np.array(
                             [
                                 np.sin(beta[ndx_i]),
                                 np.sin(beta[ndx_j]),
-                                np.sin(beta[ndx_k])
+                                np.sin(beta[ndx_k]),
                             ]
                         )
 
                         P = np.dot(N.T, N)
 
                         A = np.dot(u.T, np.dot(P, u))
                         B = np.dot(v.T, np.dot(P, v))
@@ -695,43 +723,53 @@
                         # D += 2 * np.cos(beta_ik) * np.cos(beta_jk) * np.cos(beta_ij)
                         # this should be equal to the other D
 
                         t1 = (A - B) ** 2 + 4 * C ** 2
                         t2 = 2 * (A - B) * (A + B - 2 * D)
                         t3 = (A + B - 2 * D) ** 2 - 4 * C ** 2
 
-                        w_lt = (-t2 - np.sqrt(t2 ** 2 - 4 * t1 * t3)) / (2 * t1)
-                        w_gt = (-t2 + np.sqrt(t2 ** 2 - 4 * t1 * t3)) / (2 * t1)
+                        w_lt = (-t2 - np.sqrt(t2 ** 2 - 4 * t1 * t3)) / (
+                            2 * t1
+                        )
+                        w_gt = (-t2 + np.sqrt(t2 ** 2 - 4 * t1 * t3)) / (
+                            2 * t1
+                        )
 
                         alpha1 = np.arccos(w_lt) / 2
                         alpha2 = (2 * np.pi - np.arccos(w_lt)) / 2
                         alpha3 = np.arccos(w_gt) / 2
                         alpha4 = (2 * np.pi - np.arccos(w_gt)) / 2
 
                         for alpha in [alpha1, alpha2, alpha3, alpha4]:
                             if alpha < max_a:
                                 continue
 
                             if min_alpha is not None and alpha >= min_alpha:
                                 continue
 
-                            lhs = A * np.cos(alpha) ** 2 + B * np.sin(alpha) ** 2
+                            lhs = (
+                                A * np.cos(alpha) ** 2 + B * np.sin(alpha) ** 2
+                            )
                             lhs += 2 * C * np.sin(alpha) * np.cos(alpha)
                             if not np.isclose(lhs, D):
                                 continue
 
                             # print(lhs, D)
 
-                            p = np.dot(N, u * np.cos(alpha) + v * np.sin(alpha))
+                            p = np.dot(
+                                N, u * np.cos(alpha) + v * np.sin(alpha)
+                            )
                             norm = p / gamma_ijk
 
                             for atom in atom_list:
                                 ndx = self.atoms.index(atom)
                                 rhs = beta[ndx]
-                                d = np.dot(center.bond(atom), norm) / center.dist(atom)
+                                d = np.dot(
+                                    center.bond(atom), norm
+                                ) / center.dist(atom)
                                 if abs(d) < 1:
                                     rhs += np.arccos(d)
                                 if not alpha >= rhs:
                                     break
                             else:
                                 if min_alpha is None or alpha < min_alpha:
                                     # print("min_alpha set", alpha)
@@ -746,18 +784,20 @@
 
             scale = 5 * np.cos(min_alpha)
 
             cones.append(
                 (
                     center.coords + scale * min_norm,
                     center.coords,
-                    scale * abs(np.tan(min_alpha))
+                    scale * abs(np.tan(min_alpha)),
                 )
             )
 
             if return_cones:
                 return np.rad2deg(2 * min_alpha), cones
 
             return np.rad2deg(2 * min_alpha)
 
         else:
-            raise NotImplementedError("cone angle type is not implemented: %s" % method)
+            raise NotImplementedError(
+                "cone angle type is not implemented: %s" % method
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AaronTools-1.0b8/config.py` & `AaronTools-1.0b9/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import configparser
 import itertools as it
 import os
 import re
 from getpass import getuser
-from warnings import warn
 
 import AaronTools
+from AaronTools import addlogger
 from AaronTools.const import AARONLIB, AARONTOOLS
 from AaronTools.theory import (
     GAUSSIAN_COMMENT,
     GAUSSIAN_CONSTRAINTS,
     GAUSSIAN_COORDINATES,
     GAUSSIAN_GEN_BASIS,
     GAUSSIAN_GEN_ECP,
@@ -58,49 +58,49 @@
     "PSI4_MOLECULE",
     "PSI4_JOB",
     "PSI4_OPTKING",
     "PSI4_SETTINGS",
 ]
 
 
+@addlogger
 class Config(configparser.ConfigParser):
     """
     Reads configuration information from INI files found at:
         $QCHASM/AaronTools/config.ini
         $AARONLIB/config.ini
         ./config.ini or /path/to/file supplied during initialization
     Access to configuration information available using dictionary notation.
         eg: self[`section_name`][`option_name`] returns `option_value`
     See help(configparser.ConfigParser) for more information
     """
 
+    LOG = None
     SPEC_ATTRS = [
         "_changes",
         "_changed_list",
         "_args",
         "_kwargs",
         "infile",
-        "conformer",
         "metadata",
     ]
 
-    USER_SPECIFIC = ["metadata"]
-
     def __init__(
         self, infile=None, quiet=False, skip_user_default=False, **kwargs
     ):
         """
         infile: the configuration file to read
         quiet: prints helpful status information
         skip_user_default: change to True to skip importing user's default config files
         **kwargs: passed to initialization of parent class
         """
         configparser.ConfigParser.__init__(
             self, interpolation=None, comment_prefixes=("#"), **kwargs
         )
+        self.infile = infile
         if not quiet:
             print("Reading configuration...")
         self._read_config(infile, quiet, skip_user_default)
 
         # enforce case-sensitivity in certain sections
         for section in self:
             if section in [
@@ -113,48 +113,51 @@
             for option, value in self[section].items():
                 if option.lower() != option:
                     self[section][option.lower()] = value
                     del self[section][option]
 
         # handle included sections
         self._parse_includes()
+        if infile is not None:
+            self.read(infile)
 
         # set additional default values
         if infile:
             if "top_dir" not in self["DEFAULT"]:
                 self["DEFAULT"]["top_dir"] = os.path.dirname(
                     os.path.abspath(infile)
                 )
             if "name" not in self["DEFAULT"]:
                 self["DEFAULT"]["name"] = ".".join(
                     os.path.relpath(
                         infile, start=self["DEFAULT"]["top_dir"]
                     ).split(".")[:-1]
                 )
+        else:
+            if "top_dir" not in self["DEFAULT"]:
+                self["DEFAULT"]["top_dir"] = os.path.abspath(os.path.curdir)
 
         # handle substitutions/mapping
         self._changes = {}
         self._changed_list = []
         self._parse_changes()
 
         # for passing to Theory(*args, **kwargs)
         self._args = []
         self._kwargs = {}
-        self.infile = infile
 
         # metadata is username and project name
         self.metadata = {
             "user": self.get(
                 "DEFAULT",
                 "user",
                 fallback=self.get("HPC", "user", fallback=getuser()),
             ),
             "project": self.get("DEFAULT", "project", fallback=""),
         }
-        self.conformer = 0
 
     def optionxform(self, option):
         return str(option)
 
     def __str__(self):
         rv = ""
         for section in self:
@@ -164,27 +167,41 @@
             for option, value in self[section].items():
                 rv += "{} = {}\n".format(option, value)
             rv += "\n"
         return rv
 
     def copy(self):
         config = Config(infile=None, quiet=True)
-        for attr in self._sections:
-            config.add_section(attr)
-            for key, val in self[attr].items():
-                config[attr][key] = val
-        for attr in self.SPEC_ATTRS:
-            setattr(config, attr, getattr(self, attr))
+        for section in ["DEFAULT"] + self.sections():
+            try:
+                config.add_section(section)
+            except (configparser.DuplicateSectionError, ValueError):
+                pass
+            for key, val in self[section].items():
+                config[section][key] = val
+        for section in self.SPEC_ATTRS:
+            setattr(config, section, getattr(self, section))
         return config
 
+    def for_change(self, change, structure=None):
+        this_config = self.copy()
+        if structure is not None:
+            this_config["Job"]["name"] = structure.name
+        if change:
+            this_config["Job"]["name"] = os.path.join(
+                change, this_config["Job"]["name"]
+            )
+        this_config._changes = {change: self._changes[change]}
+        return this_config
+
     def _parse_changes(self):
         for section in ["Substitution", "Mapping"]:
             if section not in self:
                 continue
-            if "reopt" in self[section].getboolean(section, "reopt"):
+            if self[section].getboolean("reopt", fallback=False):
                 self._changes[""] = ({}, None)
             for key, val in self[section].items():
                 if key in self["DEFAULT"]:
                     continue
                 del self[section][key]
                 key = "\n".join(["".join(k.split()) for k in key.split("\n")])
                 val = "\n".join(["".join(v.split()) for v in val.split("\n")])
@@ -210,15 +227,18 @@
                         if i == 0 and len(v.split("=")) == 1:
                             v = "{}={}".format(key, v)
                             val[i] = v
                             del self[section][key]
                             key = ""
                             self[section]["~PLACEHOLDER~"] = ";".join(val)
                         v = v.split("=")
-                        if not key.startswith("&combinations"):
+                        if (
+                            not key.startswith("&combinations")
+                            and "(" not in v[0]
+                        ):
                             v[0] = v[0].split(",")
                         else:
                             v[0] = [v[0]]
                         for k in v[0]:
                             tmp[k] = v[1]
                     val = tmp
                 # handle request for combinations
@@ -280,15 +300,15 @@
         Pulls in values of options indicated by $option_name
         Eg:
             ppn = 4
             memory = %{ $ppn * 2 }GB --> memory = 8GB
         """
         func_patt = re.compile("%{(.*?)}")
         attr_patt = re.compile("\$([a-zA-Z0-9_:]+)")
-        for section in self._sections:
+        for section in ["DEFAULT"] + self.sections():
             # evaluate functions
             for key, val in self[section].items():
                 for match in func_patt.findall(val):
                     eval_match = match
                     for attr in attr_patt.findall(match):
                         if ":" in attr:
                             from_section, option = attr.split(":")
@@ -311,14 +331,41 @@
 
     def getlist(self, section, option, *args, delim=",", **kwargs):
         """returns a list of option values by splitting on the delimiter specified by delim"""
         raw = self.get(section, option, *args, **kwargs)
         out = [x.strip() for x in raw.split(delim) if len(x.strip()) > 0]
         return out
 
+    def read(self, filename, quiet=True):
+        is_string = False
+        try:
+            # if infile is multi-line, it's probably a string and not a file name
+            if len(filename.splitlines()) > 1:
+                is_string = True
+                self.read_string(filename)
+            else:
+                success = super().read(filename)
+                if not quiet and len(success) == 0:
+                    try:
+                        with open(filename) as f:
+                            f.readline()
+                    except Exception as e:
+                        raise Exception(
+                            "failed to read %s\n%s" % (filename, e)
+                        ) from e
+        except configparser.MissingSectionHeaderError:
+            # add global options to default section
+            if is_string:
+                contents = filename
+            else:
+                with open(filename) as f:
+                    contents = f.read()
+            contents = "[DEFAULT]\n" + contents
+            self.read_string(contents)
+
     def _read_config(self, infile, quiet, skip_user_default):
         """
         Reads configuration information from `infile` after pulling defaults
         """
         filenames = [
             os.path.join(AARONTOOLS, "config.ini"),
         ]
@@ -330,33 +377,15 @@
         for i, filename in enumerate(filenames):
             if not quiet:
                 if os.path.isfile(filename):
                     print("    ✓", end="  ")
                 else:
                     print("    ✗", end="  ")
                 print(filename)
-            try:
-                # if infile is multi-line, it's probably a string and not a file name
-                if len(filename.splitlines()) > 1:
-                    self.read_string(filename)
-                else:
-                    success = self.read(filename)
-                    if not quiet and len(success) == 0:
-                        try:
-                            with open(filename) as f:
-                                f.readline()
-                        except Exception as e:
-                            raise Exception(
-                                "failed to read %s\n%s" % (filename, e)
-                            ) from e
-            except configparser.MissingSectionHeaderError:
-                # add global options to default section
-                with open(filename) as f:
-                    contents = "[DEFAULT]\n" + f.read()
-                self.read_string(contents)
+            self.read(filename, quiet=quiet)
             # local_only can only be overridden at the user level if "False" in the system config file
             if i == 0:
                 local_only = self["DEFAULT"].getboolean("local_only")
             elif local_only:
                 self["DEFAULT"]["local_only"] = str(local_only)
 
     def get_other_kwargs(self, section="Theory"):
@@ -396,46 +425,50 @@
             ORCA_ROUTE,
             PSI4_AFTER_JOB,
             PSI4_BEFORE_GEOM,
             PSI4_BEFORE_JOB,
             PSI4_COMMENT,
         ]
 
-        job_kwargs = [
+        theory_kwargs = [
             "method",
             "charge",
             "multiplicity",
             "type",
             "basis",
             "ecp",
         ]
 
         # two layer options are separated by newline
         # individual options are split on white space, with the first defining the primary layer
         out = {}
         for option in two_layer:
             value = self[section].get(option, fallback=False)
+            value = self._kwargs.get(option, value)
             if value:
-                # if it's got brackets, it's probably a python-looking dictionary
-                # eval it instead of parsing
-                if "{" in value:
+                if isinstance(value, dict):
+                    out[option] = value
+                elif "{" in value:
+                    # if it's got brackets, it's probably a python-looking dictionary
+                    # eval it instead of parsing
                     out[option] = eval(value, {})
                 else:
                     out[option] = {}
                     for v in value.splitlines():
                         key = v.split()[0]
                         if len(v.split()) > 1:
                             info = v.split()[1].split(",")
                         else:
                             info = []
 
                         out[option][key] = [x.strip() for x in info]
 
         for option in two_layer_single_value:
             value = self.get(section, option, fallback=False)
+            value = self._kwargs.get(option, value)
             if value:
                 if "{" in value:
                     out[option] = eval(value, {})
                 else:
                     out[option] = {}
                     for v in value.splitlines():
                         key = v.split()[0]
@@ -444,30 +477,68 @@
                         else:
                             info = []
 
                         out[option][key] = [x.strip() for x in info]
 
         for option in one_layer:
             value = self[section].get(option, fallback=False)
+            value = self._kwargs.get(option, value)
             if value:
                 out[option] = value.splitlines()
 
-        for option in job_kwargs:
+        for option in theory_kwargs:
             value = self[section].get(option, fallback=False)
             if value:
                 out[option] = value
 
         return out
 
+    def get_constraints(self, geometry):
+        constraints = {}
+        try:
+            con_list = re.findall("\(.*?\)", self["Geometry"]["constraints"])
+        except KeyError:
+            try:
+                geometry.parse_comment()
+                con_list = geometry.other["constraint"]
+            except KeyError:
+                raise RuntimeError(
+                    "Constraints for forming/breaking bonds must be specified for TS search"
+                )
+        for con in con_list:
+            tmp = []
+            try:
+                for c in eval(con, {}):
+                    tmp += geometry.find(str(c))
+            except TypeError:
+                for c in con:
+                    tmp += geometry.find(str(c))
+            con = [a.name for a in tmp]
+            if len(con) == 1:
+                constraints.setdefault("atoms", [])
+                constraints["atoms"] += [con]
+            elif len(con) == 2:
+                constraints.setdefault("bonds", [])
+                constraints["bonds"] += [con]
+            elif len(con) == 3:
+                constraints.setdefault("angles", [])
+                constraints["angles"] += [con]
+            elif len(con) == 4:
+                constraints.setdefault("torsions", [])
+                constraints["torsions"] += [con]
+        return constraints
+
     def get_theory(self, geometry, section="Theory"):
         """
         Get the theory object according to configuration information
         """
         if not self.has_section(section):
-            warn('config has no "%s" section, switching to "Theory"' % section)
+            self.LOG.warning(
+                'config has no "%s" section, switching to "Theory"' % section
+            )
             section = "Theory"
 
         kwargs = self.get_other_kwargs(section=section)
         theory = Theory(*self._args, geometry=geometry, **kwargs)
 
         # build ImplicitSolvent object
         if self[section].get("solvent", fallback="gas") == "gas":
@@ -487,68 +558,26 @@
                 constraints = None
                 ts = False
                 if len(job_type) > 1:
                     if "change" in job_type[1]:
                         theory.geometry.freeze()
                         theory.geometry.relax(self._changed_list)
                     elif "constrain" in job_type[1]:
-                        constraints = {}
-                        try:
-                            con_list = re.findall(
-                                "\(.*?\)", self["Geometry"]["constraints"]
-                            )
-                        except KeyError:
-                            try:
-                                theory.geometry.parse_comment()
-                                con_list = theory.geometry.other["constraint"]
-                            except KeyError:
-                                raise RuntimeError(
-                                    "Constraints for forming/breaking bonds must be specified for TS search"
-                                )
-                        for con in con_list:
-                            try:
-                                con = tuple(
-                                    geometry.find(str(c))[0]
-                                    for c in eval(con, {})
-                                )
-                            except TypeError:
-                                con = tuple(
-                                    geometry.find(str(c))[0] for c in con
-                                )
-                            if len(con) == 1:
-                                constraints.setdefault("atoms", [])
-                                constraints["atoms"] += [con]
-                            elif len(con) == 2:
-                                constraints.setdefault("bonds", [])
-                                constraints["bonds"] += [con]
-                            elif len(con) == 3:
-                                constraints.setdefault("angles", [])
-                                constraints["angles"] += [con]
-                            elif len(con) == 4:
-                                constraints.setdefault("torsions", [])
-                                constraints["torsions"] += [con]
+                        self.get_constraints(theory.geometry)
                     elif "ts" == job_type[1]:
                         ts = True
 
-                if "opt" in job_type[0]:
+                if "opt" in job_type[0] or "conf" in job_type[0]:
                     theory.job_type += [
                         OptimizationJob(
                             transition_state=ts,
                             geometry=geometry,
                             constraints=constraints,
                         )
                     ]
-                elif "conf" in job_type[0]:
-                    theory.job_type += [
-                        CrestJob(
-                            transition_state=ts,
-                            geometry=geometry,
-                            constraints=constraints,
-                        )
-                    ]
             if "freq" in job_type[0]:
                 theory.job_type += [
                     FrequencyJob(
                         numerical=self[section].get(
                             "numerical", fallback=False
                         ),
                         temperature=self[section].get(
@@ -598,14 +627,15 @@
             return rv
 
         structure_dict = {}
         kind_dict = {}
         structure_list = []
         # load templates from AARONLIB
         if "Reaction" in self:
+            path = None
             if "template" in self["Reaction"]:
                 path = os.path.join(
                     AARONLIB,
                     "TS_geoms",
                     self["Reaction"]["reaction"],
                     self["Reaction"]["template"],
                 )
@@ -615,14 +645,18 @@
                 path = os.path.join(
                     AARONLIB,
                     "TS_geoms",
                     self["Reaction"]["reaction"],
                 )
                 for dirpath, dirnames, filenames in os.walk(path):
                     structure_list += get_multiple(filenames, path=dirpath)
+            for structure, kind in structure_list:
+                structure.name = os.path.relpath(structure.name, path)
+        if "Geometry" not in self:
+            return structure_list
 
         # load templates from config[Geometry]
         # store in structure_dict, keyed by structure option suffix
         # `structure.suffix = geom.xyz` store as {suffix: geom.xyz}
         # `structure = geom.xyz` (no suffix), store as {"": geom.xyz}
         if "structure" in self["Geometry"]:
             structure_dict[""] = self["Geometry"]["structure"]
@@ -656,15 +690,16 @@
                     self._changes[""] = ({}, None)
                 # adjust structure attributes
                 if "name" in self["Job"]:
                     structure.name = self["Job"]["name"]
                 if "Geometry" in self and "comment" in self["Geometry"]:
                     structure.comment = self["Geometry"]["comment"]
                     structure.parse_comment()
-                structure.name += ".{}".format(suffix)
+                if suffix:
+                    structure.name += ".{}".format(suffix)
                 structure_dict[suffix] = structure
                 kind_dict[suffix] = None
 
         # for loop for structure modification/creation
         # structure.suffix = geom.xyz
         # &for name in <iterator>:
         #    structure.name = structure.suffix.copy()
@@ -749,14 +784,66 @@
                             {
                                 "structure": structure,
                                 "Geometry": AaronTools.geometry.Geometry,
                             },
                         )
         return structure_list
 
+    def make_changes(self, structure):
+        if not self._changes:
+            return structure
+        changed = []
+        for name, (changes, kind) in self._changes.items():
+            for key, val in changes.items():
+                if kind == "Substitution" and "(" not in key:
+                    # regular substitutions
+                    for k in key.split(","):
+                        k = k.strip()
+                        if val.lower() == "none":
+                            structure -= structure.get_fragment(k)
+                        else:
+                            sub = structure.substitute(val, k)
+                            for atom in sub:
+                                changed += [atom.name]
+                elif kind == "Substitution":
+                    # fused ring substitutions
+                    target_patt = re.compile("\((.*?)\)")
+                    for k in target_patt.findall(key):
+                        k = [i.strip() for i in k.split(",")]
+                        if val.lower() == "none":
+                            structure -= structure.get_fragment(*k)
+                        else:
+                            sub = structure.ring_substitute(k, val)
+                            for atom in sub:
+                                changed += [atom.name]
+                elif kind == "Mapping":
+                    key = [k.strip() for k in key.split(",")]
+                    new_ligands = structure.map_ligand(val, key)
+                    for ligand in new_ligands:
+                        for atom in ligand:
+                            changed += [atom.name]
+        try:
+            con_list = list(
+                eval(self["Geometry"].get("constraints", "[]"), {})
+            )
+        except KeyError:
+            structure.parse_comment()
+            try:
+                con_list = structure.other["constraint"]
+            except KeyError:
+                con_list = []
+        for con in con_list:
+            for c in con:
+                try:
+                    changed.remove(str(c))
+                except ValueError:
+                    pass
+        self._changed_list = changed
+        return structure
+
     def _parse_includes(self):
         """
         Moves option values from subsections into parent section
         Eg:
             [HPC]
             include = Wheeler
             ppn = 12
@@ -767,19 +854,19 @@
 
             ^^^evaluates to:
             [Job]
             nodes = 1
             ppn = 12
             queue = wheeler_q
         """
-        for section in self._sections:
+        for section in ["DEFAULT"] + self.sections():
             # add requested subsections to parent section
             if self.has_option(section, "include"):
                 include_section = self[section]["include"].split(".")
-                if include_section[0] in self._sections:
+                if include_section[0] in self.sections():
                     # include specifies full section name, eg:
                     # include = Job.Minimum --> [Job.Minimum]
                     include_section = ".".join(include_section)
                 else:
                     # short-form of include, eg:
                     # [Job]
                     # include = Minimum
@@ -819,25 +906,32 @@
         for attr in self.SPEC_ATTRS:
             for s in skip_attrs:
                 if re.fullmatch(s, attr):
                     break
             else:
                 spec[attr] = getattr(self, attr)
 
-        for section in self._sections:
+        for section in ["DEFAULT"] + self.sections():
             if "." in section:
                 # these are include sections that should already be pulled into
                 # the main body of the config file
                 continue
             for option in self[section]:
                 for i, s in enumerate(skip_sections):
                     o = skip_options[i]
                     if re.fullmatch(s, section) and re.fullmatch(o, option):
                         break
                 else:
+                    # only include default options once, unless they are overridden
+                    if (
+                        section != "DEFAULT"
+                        and option in self["DEFAULT"]
+                        and self["DEFAULT"][option] == self[section][option]
+                    ):
+                        continue
                     spec["{}/{}".format(section, option)] = self[section][
                         option
                     ]
         return spec
 
     def read_spec(self, spec):
         """
@@ -854,42 +948,33 @@
 
     def for_step(self, step=None):
         """
         Generates a config copy with only options for the given step
         """
         config = self.copy()
         # find step-specific options
-        for section in config._sections:
+        for section in ["DEFAULT"] + config.sections():
             for key, val in config[section].items():
                 remove_key = key
                 key = key.strip().split()
                 if len(key) == 1:
                     continue
-                key_step = key[0]
+                key_step = float(key[0])
                 key = " ".join(key[1:])
-                try:
-                    key_step = float(key_step)
-                except ValueError:
-                    key_step = key_step.strip()
                 # screen based on step
-                if isinstance(key_step, float) and key_step == float(step):
+                if key_step == float(step):
                     config[section][key] = val
                 # clean up metadata
                 del config[section][remove_key]
         # other job-specific additions
         if "host" in config["HPC"]:
             try:
                 config["HPC"]["work_dir"] = config["HPC"].get("remote_dir")
             except TypeError as e:
                 raise RuntimeError(
                     "Must specify remote working directory for HPC (remote_dir = /path/to/HPC/work/dir)"
                 ) from e
         else:
             config["HPC"]["work_dir"] = config["DEFAULT"].get("top_dir")
-        config["Job"]["name"] = config["DEFAULT"]["name"]
-        if config.conformer:
-            config["Job"]["name"] += "_{}".format(config.conformer)
-        if step:
-            config["Job"]["name"] += ".{}".format(step)
         # parse user-supplied functions in config file
         config.parse_functions()
         return config
```

### Comparing `AaronTools-1.0b8/const.py` & `AaronTools-1.0b9/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1352,16 +1352,19 @@
     "CS",
     "OA",
     "OB",
     "OE",
     "OT",
 ]
 
-# main group vdw radii from doi 10.1021/jp8111556
-# transition metals from doi 10.1023/A:1011625728803 (crystal radii)
+# main group vdw radii from J. Phys. Chem. A 2009, 113, 19, 5806–5812
+# (DOI: 10.1021/jp8111556)
+# transition metals are crystal radii from Batsanov, S.S. Van der Waals
+# Radii of Elements. Inorganic Materials 37, 871–885 (2001).
+# (DOI: 10.1023/A:1011625728803)
 # transition metals are indented a bit more than the rest
 VDW_RADII = {
     "H": 1.10,
     "He": 1.40,
     "Li": 1.81,
     "Be": 1.53,
     "B": 1.92,
@@ -1433,15 +1436,15 @@
     "At": 2.02,
     "Rn": 2.20,
     "Fr": 3.48,
     "Ra": 2.83,
     "X": 0,
 }
 
-# doi 10.1021/j100785a001
+# J. Phys. Chem. 1964, 68, 3, 441–451 (DOI: 10.1021/j100785a001)
 BONDI_RADII = {
     "H": 1.20,
     "He": 1.40,
     "C": 1.70,
     "N": 1.55,
     "O": 1.52,
     "F": 1.47,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AaronTools-1.0b8/fileIO.py` & `AaronTools-1.0b9/fileIO.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """For parsing input/output files"""
 import os
 import re
 from copy import deepcopy
 from io import IOBase, StringIO
-from warnings import warn
 
 import numpy as np
 
+from AaronTools import addlogger
 from AaronTools.atoms import Atom
 from AaronTools.const import ELEMENTS, PHYSICAL, UNIT
 from AaronTools.theory import *
 
 read_types = [
     "xyz",
     "log",
     "com",
     "gjf",
     "sd",
     "sdf",
     "mol",
+    "mol2",
     "out",
     "dat",
     "fchk",
     "crest",
+    "xtb",
 ]
 write_types = ["xyz", "com", "inp", "in"]
 file_type_err = "File type not yet implemented: {}"
 float_num = re.compile("[-+]?\d+\.?\d*")
 NORM_FINISH = "Normal termination"
 ORCA_NORM_FINISH = "****ORCA TERMINATED NORMALLY****"
 PSI4_NORM_FINISH = "*** Psi4 exiting successfully. Buy a developer a beer!"
@@ -45,14 +47,15 @@
     "Error in internal coordinate system": "COORD",
     "galloc: could not allocate memory": "GALLOC",
     "Error imposing constraints": "CONSTR",
     "End of file reading basis center.": "BASIS_READ",
     "Atomic number out of range for .* basis set.": "BASIS",
     "Unrecognized atomic symbol": "ATOM",
     "malloc failed.": "MEM",
+    "A syntax error was detected in the input line": "SYNTAX",
     "Unknown message": "UNKNOWN",
 }
 
 ERROR_ORCA = {
     "SCF NOT CONVERGED AFTER": "SCF_CONV",
     # ORCA doesn't actually exit if the SCF doesn't converge...
     # "CONV_CDS": "",
@@ -227,121 +230,164 @@
             # write output to the requested destination
             with open(outfile, mode) as f:
                 f.write(s)
 
         return
 
     @classmethod
-    def write_com(cls, geom, theory, outfile=None, **kwargs):
-        # atom specs need flag column before coords if any atoms frozen
-        has_frozen = False
-        fmt = "{:<3s}" + " {:> 12.6f}" * 3 + "\n"
-        for atom in geom:
-            if atom.flag:
-                fmt = "{:<3s}  {:> 2d}" + " {:> 12.6f}" * 3 + "\n"
-                has_frozen = True
-                break
-
+    def write_com(
+        cls, geom, theory, outfile=None, return_warnings=False, **kwargs
+    ):
         # get file content string
-        s = theory.make_header(geom, **kwargs)
-        s += theory.make_molecule(geom, **kwargs)
-        s += theory.make_footer(geom, **kwargs)
+        header, header_warnings = theory.make_header(
+            geom, return_warnings=True, **kwargs
+        )
+        mol, mol_warnings = theory.make_molecule(
+            geom, return_warnings=True, **kwargs
+        )
+        footer, footer_warnings = theory.make_footer(
+            geom, return_warnings=True, **kwargs
+        )
+
+        s = header + mol + footer
+        warnings = header_warnings + mol_warnings + footer_warnings
 
         if outfile is None:
             # if outfile is not specified, name file in Aaron format
             if "step" in kwargs:
                 fname = "{}.{}.com".format(geom.name, step2str(kwargs["step"]))
             else:
                 fname = "{}.com".format(geom.name)
             with open(fname, "w") as f:
                 f.write(s)
         elif outfile is False:
+            if return_warnings:
+                return s, warnings
             return s
         else:
             with open(outfile, "w") as f:
                 f.write(s)
 
+        if return_warnings:
+            return warnings
         return
 
     @classmethod
-    def write_inp(cls, geom, theory, outfile=None, **kwargs):
+    def write_inp(
+        cls, geom, theory, outfile=None, return_warnings=False, **kwargs
+    ):
         fmt = "{:<3s} {: 9.5f} {: 9.5f} {: 9.5f}\n"
-        s = theory.make_header(geom, style="orca", **kwargs)
+        s, warnings = theory.make_header(
+            geom, style="orca", return_warnings=True, **kwargs
+        )
         for atom in geom.atoms:
             s += fmt.format(atom.element, *atom.coords)
 
         s += "*\n"
 
         if outfile is None:
             # if outfile is not specified, name file in Aaron format
             if "step" in kwargs:
                 fname = "{}.{}.inp".format(geom.name, step2str(kwargs["step"]))
             else:
                 fname = "{}.inp".format(geom.name)
             with open(fname, "w") as f:
                 f.write(s)
         elif outfile is False:
+            if return_warnings:
+                return s, warnings
             return s
         else:
             with open(outfile, "w") as f:
                 f.write(s)
+        if return_warnings:
+            return warnings
 
     @classmethod
-    def write_in(cls, geom, theory, outfile=None, **kwargs):
+    def write_in(
+        cls, geom, theory, outfile=None, return_warnings=False, **kwargs
+    ):
         """
         can accept "monomers" as a kwarg
         this should be a list of lists of atoms corresponding to the
         separate monomers in a sapt calculation
         this will only be used if theory.method.sapt is True
         if a sapt method is used but no monoers are given,
         geom's components attribute will be used intead
         """
         if "monomers" in kwargs:
             monomers = kwargs["monomers"]
             del kwargs["monomers"]
         else:
             monomers = None
 
-        s = theory.make_header(geom, style="psi4", **kwargs)
-        s += theory.make_molecule(geom, style="psi4", **kwargs)
-        s += theory.make_footer(geom, style="psi4", **kwargs)
+        header, header_warnings = theory.make_header(
+            geom, style="psi4", return_warnings=True, **kwargs
+        )
+        mol, mol_warnings = theory.make_molecule(
+            geom, style="psi4", return_warnings=True, **kwargs
+        )
+        footer, footer_warnings = theory.make_footer(
+            geom, style="psi4", return_warnings=True, **kwargs
+        )
+
+        s = header + mol + footer
+        warnings = header_warnings + mol_warnings + footer_warnings
 
         if outfile is None:
             # if outfile is not specified, name file in Aaron format
             if "step" in kwargs:
                 fname = "{}.{}.in".format(geom.name, step2str(kwargs["step"]))
             else:
                 fname = "{}.in".format(geom.name)
             with open(fname, "w") as f:
                 f.write(s)
         elif outfile is False:
+            if return_warnings:
+                return s, warnings
             return s
         else:
             with open(outfile, "w") as f:
                 f.write(s)
+        if return_warnings:
+            return warnings
 
 
+@addlogger
 class FileReader:
     """
     Attributes:
         name ''
         file_type ''
         comment ''
         atoms [Atom]
         other {}
     """
 
-    def __init__(self, fname, get_all=False, just_geom=True):
+    LOG = None
+    LOGLEVEL = "DEBUG"
+
+    def __init__(
+        self,
+        fname,
+        get_all=False,
+        just_geom=True,
+        freq_name=None,
+        conf_name=None,
+    ):
         """
         :fname: either a string specifying the file name of the file to read
             or a tuple of (str(name), str(file_type), str(content))
         :get_all: if true, optimization steps are  also saved in
             self.all_geom; otherwise only saves last geometry
         :just_geom: if true, does not store other information, such as
             frequencies, only what is needed to construct a Geometry() obj
+        :freq_name: Name of the file containing the frequency output. Only use
+            if this information is in a different file than `fname` (eg: xtb runs
+            using the --hess runtype option)
         """
         # Initialization
         self.name = ""
         self.file_type = ""
         self.comment = ""
         self.atoms = []
         self.other = {}
@@ -357,39 +403,47 @@
             self.file_type = fname[1]
             self.content = fname[2]
         if self.file_type not in read_types:
             raise NotImplementedError(file_type_err.format(self.file_type))
 
         # Fill in attributes with geometry information
         if self.content is None:
-            self.read_file(get_all, just_geom)
+            self.read_file(
+                get_all, just_geom, freq_name=freq_name, conf_name=conf_name
+            )
         elif isinstance(self.content, str):
             f = StringIO(self.content)
         elif isinstance(self.content, IOBase):
             f = self.content
 
         if self.content is not None:
             if self.file_type == "log":
                 self.read_log(f, get_all, just_geom)
             elif any(self.file_type == ext for ext in ["sd", "sdf", "mol"]):
                 self.read_sd(f)
             elif self.file_type == "xyz":
                 self.read_xyz(f, get_all)
+            elif self.file_type == "mol2":
+                self.read_mol2(f, get_all)
             elif any(self.file_type == ext for ext in ["com", "gjf"]):
                 self.read_com(f)
             elif self.file_type == "out":
                 self.read_orca_out(f, get_all, just_geom)
             elif self.file_type == "dat":
                 self.read_psi4_out(f, get_all, just_geom)
             elif self.file_type == "fchk":
                 self.read_fchk(f, just_geom)
             elif self.file_type == "crest":
-                self.read_crest(f)
+                self.read_crest(f, conf_name=conf_name)
+            elif self.file_type == "xtb":
+                self.read_xtb(f, freq_name=freq_name)
 
-    def read_file(self, get_all=False, just_geom=True):
+    def read_file(
+        self, get_all=False, just_geom=True, freq_name=None, conf_name=None
+    ):
         """
         Reads geometry information from fname.
         Parameters:
             get_all     If false (default), only keep the last geom
                         If true, self is last geom, but return list
                             of all others encountered
         """
@@ -410,24 +464,26 @@
             self.read_xyz(f, get_all)
         elif self.file_type == "log":
             self.read_log(f, get_all, just_geom)
         elif any(self.file_type == ext for ext in ["com", "gjf"]):
             self.read_com(f)
         elif any(self.file_type == ext for ext in ["sd", "sdf", "mol"]):
             self.read_sd(f)
+        elif self.file_type == "mol2":
+            self.read_mol2(f)
         elif self.file_type == "out":
             self.read_orca_out(f, get_all, just_geom)
         elif self.file_type == "dat":
             self.read_psi4_out(f, get_all, just_geom)
         elif self.file_type == "fchk":
             self.read_fchk(f, just_geom)
         elif self.file_type == "crest":
-            self.read_crest(f)
+            self.read_crest(f, conf_name=conf_name)
         elif self.file_type == "xtb":
-            self.read_xtb(f)
+            self.read_xtb(f, freq_name=freq_name)
 
         f.close()
         return
 
     def skip_lines(self, f, n):
         for i in range(n):
             f.readline()
@@ -466,15 +522,15 @@
         progress = 0
         for i, line in enumerate(lines):
             progress += 1
             if "$$$$" in line:
                 progress = 0
                 if get_all:
                     self.all_geom.append(
-                        [deepcopy(self.comment), deepcopy(self.geometry)]
+                        [deepcopy(self.comment), deepcopy(self.atoms)]
                     )
 
                 continue
 
             if progress == 3:
                 self.comment = line.strip()
 
@@ -495,14 +551,53 @@
                     a1, a2 = [int(x) - 1 for x in line.split()[0:2]]
                     self.atoms[a1].connected.add(self.atoms[a2])
                     self.atoms[a2].connected.add(self.atoms[a1])
 
                 for j, a in enumerate(self.atoms):
                     a.name = str(j + 1)
 
+    def read_mol2(self, f, get_all=False):
+        """
+        read TRIPOS mol2
+        """
+        atoms = []
+
+        lines = f.readlines()
+        i = 0
+        while i < len(lines):
+            if lines[i].startswith("@<TRIPOS>MOLECULE"):
+                self.comment = lines[i + 1]
+                info = lines[i + 2].split()
+                n_atoms = int(info[0])
+                n_bonds = int(info[1])
+                i += 3
+
+            elif lines[i].startswith("@<TRIPOS>ATOM"):
+                for j in range(0, n_atoms):
+                    i += 1
+                    info = lines[i].split()
+                    # name = info[1]
+                    coords = np.array([float(x) for x in info[2:5]])
+                    element = re.match("([A-Za-z]+)", info[5]).group(1)
+                    atoms.append(
+                        Atom(element=element, coords=coords, name=str(j + 1))
+                    )
+
+                self.atoms = atoms
+
+            elif lines[i].startswith("@<TRIPOS>BOND"):
+                for j in range(0, n_bonds):
+                    i += 1
+                    info = lines[i].split()
+                    a1, a2 = [int(ndx) - 1 for ndx in info[1:3]]
+                    self.atoms[a1].connected.add(self.atoms[a2])
+                    self.atoms[a2].connected.add(self.atoms[a1])
+
+            i += 1
+
     def read_psi4_out(self, f, get_all=False, just_geom=True):
         def get_atoms(f, n):
             rv = []
             self.skip_lines(f, 1)
             n += 2
             line = f.readline()
             i = 0
@@ -905,20 +1000,25 @@
 
                 elif line.startswith(" Total Charge"):
                     self.other["charge"] = int(line.split()[-1])
 
                 elif line.startswith(" Multiplicity"):
                     self.other["multiplicity"] = int(line.split()[-1])
 
-                elif "rotational symmetry number" in line.strip():
+                elif "rotational symmetry number" in line:
                     # TODO: make this cleaner
                     self.other["rotational_symmetry_number"] = int(
                         line.split()[-2]
                     )
 
+                elif "Symmetry Number:" in line:
+                    self.other["rotational_symmetry_number"] = int(
+                        line.split()[-1]
+                    )
+
                 elif line.startswith("Zero point energy"):
                     self.other["ZPVE"] = float(line.split()[4])
 
                 elif line.startswith("Total Enthalpy"):
                     self.other["enthalpy"] = float(line.split()[3])
 
                 elif line.startswith("Final Gibbs"):
@@ -1101,15 +1201,15 @@
         self.other["opt_steps"] = 0
         found_archive = False
         n = 1
         route = None
         while line != "":
             # route
             # we need to grab the route b/c sometimes 'hpmodes' can get split onto multiple lines:
-            ##B3LYP/genecp EmpiricalDispersion=GD3 int=(grid=superfinegrid) freq=(h
+            # B3LYP/genecp EmpiricalDispersion=GD3 int=(grid=superfinegrid) freq=(h
             # pmodes,noraman,temperature=313.15)
             if line.strip().startswith("#") and route is None:
                 route = ""
                 while "------" not in line:
                     route += line.strip()
                     n += 1
                     line = f.readline()
@@ -1154,15 +1254,15 @@
                     self.other["charge"] = int(match.group(1))
                     self.other["multiplicity"] = int(match.group(2))
 
             # status
             if NORM_FINISH in line:
                 self.other["finished"] = True
             if "SCF Done" in line:
-                tmp = [l.strip() for l in line.split()]
+                tmp = [word.strip() for word in line.split()]
                 idx = tmp.index("=")
                 self.other["energy"] = float(tmp[idx + 1])
             if "Molecular mass:" in line:
                 self.other["mass"] = float(float_num.search(line).group(0))
                 self.other["mass"] *= UNIT.AMU_TO_KG
 
             # Frequencies
@@ -1397,37 +1497,38 @@
                                 other_kwargs[GAUSSIAN_ROUTE][keyword] = [
                                     options
                                 ]
                             else:
                                 other_kwargs[GAUSSIAN_ROUTE][option] = []
                                 continue
 
-                    theory = Theory(
-                        charge=self.other["charge"],
-                        multiplicity=self.other["multiplicity"],
-                        job_type=job_type,
-                        basis=basis,
-                        method=method,
-                        grid=grid,
-                        solvent=solvent,
-                    )
-
-                    self.other["theory"] = theory
                     self.other["other_kwargs"] = other_kwargs
+                    try:
+                        theory = Theory(
+                            charge=self.other["charge"],
+                            multiplicity=self.other["multiplicity"],
+                            job_type=job_type,
+                            basis=basis,
+                            method=method,
+                            grid=grid,
+                            solvent=solvent,
+                        )
+                        self.other["theory"] = theory
+                    except KeyError:
+                        # if there is a serious error, too little info may be available
+                        # to properly create the theory object
+                        pass
 
         for i, a in enumerate(self.atoms):
             a.name = str(i + 1)
 
         if "finished" not in self.other:
             self.other["finished"] = False
         if "error" not in self.other:
             self.other["error"] = None
-        if not self.other["finished"] and not self.other["error"]:
-            self.other["error"] = ERROR["Unknown message"]
-            self.other["error_msg"] = "Unknown message"
         return
 
     def read_com(self, f):
         found_atoms = False
         found_constraint = False
         atoms = []
         other = {}
@@ -1554,18 +1655,14 @@
 
         int_info = re.compile("([\S\s]+?)\s*I\s*([N=]*)\s*(-?\d+)")
         real_info = re.compile(
             "([\S\s]+?)\s*R\s*([N=])*\s*(-?\d+\.?\d*[Ee]?[+-]?\d*)"
         )
 
         theory = Theory()
-        reading_orbital_data = False
-        n_alpha = 0
-        n_beta = 0
-        orbital_data = {}
 
         lines = f.readlines()
 
         i = 0
         while i < len(lines):
             line = lines[i]
             if i == 1:
@@ -1634,63 +1731,126 @@
             atom = Atom(
                 element=ELEMENTS[atnum],
                 coords=UNIT.A0_TO_BOHR * coord,
                 name=str(n + 1),
             )
             self.atoms.append(atom)
 
-    def read_crest(self, f):
+    def read_crest(self, f, conf_name=None):
+        """
+        conf_name = False to skip conformer loading (doesn't get written until crest job is done)
+        """
+        if conf_name is None:
+            conf_name = os.path.join(
+                os.path.dirname(self.name), "crest_conformers.xyz"
+            )
         line = True
+        self.other["finished"] = False
+        self.other["error"] = None
         while line:
             line = f.readline()
             if "terminated normally" in line:
                 self.other["finished"] = True
-                self.other["error"] = None
             elif "population of lowest" in line:
                 self.other["best_pop"] = float(float_num.findall(line)[0])
             elif "ensemble free energy" in line:
                 self.other["free_energy"] = float(float_num.findall(line)[0])
             elif "ensemble entropy" in line:
                 self.other["entropy"] = (
                     float(float_num.findall(line)[1]) / 1000
                 )
             elif "ensemble average energy" in line:
                 self.other["energy"] = float(float_num.findall(line)[0])
             elif "E lowest" in line:
                 self.other["best_energy"] = float(float_num.findall(line)[0])
             elif "T /K" in line:
                 self.other["temperature"] = float(float_num.findall(line)[0])
+            elif (
+                line.strip()
+                .lower()
+                .startswith(("forrtl", "warning", "*warning"))
+            ):
+                self.other["error"] = "UNKNOWN"
+                if "error_msg" not in self.other:
+                    self.other["error_msg"] = ""
+                self.other["error_msg"] += line
+            elif "-chrg" in line:
+                self.other["charge"] = int(float_num.findall(line)[0])
+            elif "-uhf" in line:
+                self.other["multiplicity"] = (
+                    int(float_num.findall(line)[0]) + 1
+                )
 
-        cfname = os.path.join(
-            os.path.dirname(self.name), "crest_conformers.xyz"
-        )
-        if os.access(cfname, os.R_OK):
+        if self.other["finished"] and conf_name:
             self.other["conformers"] = FileReader(
-                cfname,
+                conf_name,
                 get_all=True,
             ).all_geom
+            self.comment, self.atoms = self.other["conformers"][0]
+            self.other["conformers"] = self.other["conformers"][1:]
 
-    def read_xtb(self, f):
+    def read_xtb(self, f, freq_name=None):
         line = True
+        self.other["finished"] = False
+        self.other["error"] = None
+        self.atoms = []
+        self.comment = ""
         while line:
             line = f.readline()
+            if "Optimized Geometry" in line:
+                line = f.readline()
+                n_atoms = int(line.strip())
+                line = f.readline()
+                self.comment = " ".join(line.strip().split()[2:])
+                for i in range(n_atoms):
+                    line = f.readline()
+                    elem, x, y, z = line.split()
+                    self.atoms.append(Atom(element=elem, coords=[x, y, z]))
+            if "normal termination" in line:
+                self.other["finished"] = True
+            if "abnormal termination" in line:
+                self.other["error"] = "UNKNOWN"
+            if line.strip().startswith("#ERROR"):
+                if "error_msg" not in self.other:
+                    self.other["error_msg"] = ""
+                self.other["error_msg"] += line
+            if "charge" in line and ":" in line:
+                self.other["charge"] = int(float_num.findall(line)[0])
+            if "spin" in line and ":" in line:
+                self.other["multiplicity"] = (
+                    2 * float(float_num.findall(line)[0]) + 1
+                )
+            if "total energy" in line:
+                self.other["energy"] = float(float_num.findall(line)[0])
+            if "zero point energy" in line:
+                self.other["ZPVE"] = float(float_num.findall(line)[0])
+            if "total free energy" in line:
+                self.other["free_energy"] = float(float_num.findall(line)[0])
+            if "electronic temp." in line:
+                self.other["temperature"] = float(float_num.findall(line)[0])
+        if freq_name is not None:
+            with open(freq_name) as f_freq:
+                self.other["frequency"] = Frequency(f_freq.read())
 
 
+@addlogger
 class Frequency:
     """
     ATTRIBUTES
     :data: Data - contains frequencies, intensities, and normal mode vectors
     :imaginary_frequencies: list(float)
     :real_frequencies: list(float)
     :lowest_frequency: float
     :by_frequency: dict keyed by frequency containing intensities and vectors
         {freq: {intensity: float, vector: np.array}}
     :is_TS: bool - true if len(imaginary_frequencies) == 1, else False
     """
 
+    LOG = None
+
     class Data:
         """
         ATTRIBUTES
         :frequency: float
         :intensity: float
         :vector: (2D array) normal mode vectors
         """
@@ -1701,21 +1861,20 @@
             intensity=None,
             vector=None,
             forcek=None,
             symmetry=None,
         ):
             if vector is None:
                 vector = []
-            if forcek is None:
-                forcek = []
+
             self.frequency = frequency
             self.intensity = intensity
             self.symmetry = symmetry
             self.vector = np.array(vector)
-            self.forcek = np.array(forcek)
+            self.forcek = forcek
 
     def __init__(self, data, hpmodes=None, style="log"):
         """
         :data: should either be a str containing the lines of the output file
             with frequency information, or a list of Data objects
         :hpmodes: required when data is a string
         :form:    required when data is a string; denotes file format (log, out, ...)
@@ -1741,15 +1900,15 @@
 
         lines = data.split("\n")
         num_head = 0
         for line in lines:
             if "Harmonic frequencies" in line:
                 num_head += 1
         if hpmodes and num_head != 2:
-            warn("Log file damaged, cannot get frequencies")
+            self.LOG.warning("Log file damaged, cannot get frequencies")
             return
         if style == "log":
             self.parse_lines(lines, hpmodes)
         elif style == "out":
             self.parse_orca_lines(lines, hpmodes)
         elif style == "dat":
             self.parse_psi4_lines(lines, hpmodes)
@@ -1791,15 +1950,18 @@
                 force_consts = [float(x) for x in line.split()[3:]]
                 for i, data in enumerate(self.data[-nmodes:]):
                     data.forcek = force_consts[i]
 
             elif line.strip().startswith("Irrep"):
                 # sometimes psi4 doesn't identify the irrep of a mode, so we can't
                 # use line.split()
-                symm = [x.strip() if x.strip() else None for x in [line[31:40], line[51:60], line[71:80]]]
+                symm = [
+                    x.strip() if x.strip() else None
+                    for x in [line[31:40], line[51:60], line[71:80]]
+                ]
                 for i, data in enumerate(self.data[-nmodes:]):
                     data.symmetry = symm[i]
 
             elif line.strip().startswith("----"):
                 read_displacement = True
                 modes = [[] for i in range(0, nmodes)]
 
@@ -1957,7 +2119,316 @@
                 "vector": data.vector,
             }
         if len(self.data) > 0:
             self.lowest_frequency = self.data[0].frequency
         else:
             self.lowest_frequency = None
         self.is_TS = True if len(self.imaginary_frequencies) == 1 else False
+
+    def get_ir_data(
+            self,
+            point_spacing=None,
+            fwhm=15.0,
+            plot_type="transmittance",
+            peak_type="pseudo-voigt",
+            voigt_mixing=0.5,
+            linear_scale=0.0,
+            quadratic_scale=0.0,
+    ):
+        """
+        returns arrays of x_values, y_values for an IR plot
+        point_spacing - spacing between points, default is higher resolution around
+                        each peak (i.e. not uniform)
+                        this is pointless if peak_type == delta
+        fwhm - full width at half max in 1/cm
+        plot_type - transmittance or absorbance
+        peak_type - pseudo-voigt, gaussian, lorentzian, or delta
+        voigt_mixing - fraction of pseudo-voigt that is gaussian
+        linear_scale - subtract linear_scale * frequency off each mode
+        quadratic_scale - subtract quadratic_scale * frequency^2 off each mode
+        """
+        # scale frequencies
+        frequencies = np.array([freq.frequency for freq in self.data if freq.frequency > 0])
+        frequencies -= linear_scale * frequencies + quadratic_scale * frequencies ** 2
+        intensities = [freq.intensity for freq in self.data if freq.frequency > 0]
+        
+        if point_spacing:
+            x_values = []
+            x = -point_spacing
+            while x < max(frequencies):
+                x += point_spacing
+                x_values.append(x)
+            
+            x_values = np.array(x_values)
+        
+        e_factor = -4 * np.log(2) / fwhm ** 2
+        
+        if peak_type.lower() != "delta":
+            # get a list of functions
+            # we'll evaluate these at each x point later
+            functions = []
+            if not point_spacing:
+                x_values = np.linspace(0, max(frequencies) - 10 * fwhm, num=100).tolist()
+            
+            for freq, intensity in zip(frequencies, intensities):
+                if intensity is not None:
+                    if not point_spacing:
+                        x_values.extend(
+                            np.linspace(
+                                max(freq - (3.5 * fwhm), 0), 
+                                freq + (3.5 * fwhm), 
+                                num=65,
+                            ).tolist()
+                        )
+                        x_values.append(freq)
+                    
+                    if peak_type.lower() == "gaussian":
+                        functions.append(
+                            lambda x, x0=freq, inten=intensity: inten * np.exp(e_factor * (x - x0) ** 2)
+                        )
+        
+                    elif peak_type.lower() == "lorentzian":
+                        functions.append(
+                            lambda x, x0=freq, inten=intensity: inten * 0.5 * (0.5 * fwhm / ((x - x0) ** 2 + (0.5 * fwhm) ** 2))
+                        )
+                    
+                    elif peak_type.lower() == "pseudo-voigt":
+                        functions.append(
+                            lambda x, x0=freq, inten=intensity:
+                                inten * (
+                                    (1 - voigt_mixing) * 0.5 * (0.5 * fwhm / ((x - x0)**2 + (0.5 * fwhm)**2)) + 
+                                    voigt_mixing * np.exp(e_factor * (x - x0)**2)
+                                )
+                        )
+            
+            if not point_spacing:
+                x_values = np.array(list(set(x_values)))
+                x_values.sort()
+        
+            y_values = np.sum([f(x_values) for f in functions], axis=0)
+        
+        else:
+            x_values = []
+            y_values = []
+
+            for freq, intensity in zip(frequencies, intensities):
+                if intensity is not None:
+                    y_values.append(intensity)
+                    x_values.append(freq)
+
+            y_values = np.array(y_values)
+
+        if len(y_values) == 0:
+            self.LOG.warning("nothing to plot")
+            return None
+
+        y_values /= np.amax(y_values)
+
+
+        if plot_type.lower() == "transmittance":
+            y_values = np.array([10 ** (2 - y) for y in y_values])
+
+        return x_values, y_values
+  
+    def plot_ir(
+            self,
+            figure,
+            centers=None,
+            widths=None,
+            exp_data=None,
+            plot_type="transmittance",
+            peak_type="pseudo-voigt",
+            reverse_x=True,
+            **kwargs,
+    ):
+        """
+        plot IR data on figure
+        figure - matplotlib figure
+        centers - array-like of float, plot is split into sections centered
+                  on the frequency specified by centers
+                  default is to not split into sections
+        widths - array-like of float, defines the width of each section
+        exp_data - other data to plot
+                   should be a list of (x_data, y_data, color)
+        reverse_x - if True, 0 cm^-1 will be on the right
+        plot_type - see Frequency.get_ir_data
+        peak_type - any value allowed by Frequency.get_ir_data
+        kwargs - keywords for Frequency.get_ir_data
+        """
+
+        data = self.get_ir_data(
+            plot_type=plot_type,
+            peak_type=peak_type,
+            **kwargs
+        )
+        if data is None:
+            return
+        
+        x_values, y_values = data
+
+        if not centers:
+            # if no centers were specified, pretend they were so we
+            # can do everything the same way
+            axes = [figure.subplots(nrows=1, ncols=1)]
+            widths = [max(x_values)]
+            centers = [max(x_values) / 2]
+        else:
+            n_sections = len(centers)
+            figure.subplots_adjust(wspace=0.05)
+            # sort the sections so we don't jump around
+            widths = [x for _, x in sorted(
+                zip(centers, widths),
+                key=lambda p: p[0],
+                reverse=reverse_x,
+            )]
+            centers = sorted(centers, reverse=reverse_x)
+            
+            axes = figure.subplots(
+                nrows=1,
+                ncols=n_sections,
+                sharey=True,
+                gridspec_kw={'width_ratios': widths},
+            )
+            if not hasattr(axes, "__iter__"):
+                # only one section was specified (e.g. zooming in on a peak)
+                # make sure axes is iterable
+                axes = [axes]
+        
+        for i, ax in enumerate(axes):
+            if i == 0:
+                if plot_type.lower() == "transmittance":
+                    ax.set_ylabel("Transmittance (%)")
+                else:
+                    ax.set_ylabel("Absorbance (arb.)")
+                
+                # need to split plot into sections
+                # put a / on the border at the top and bottom borders
+                # of the plot
+                if len(axes) > 1:
+                    ax.spines["right"].set_visible(False)
+                    ax.tick_params(labelright=False, right=False)
+                    ax.plot(
+                        [1, 1],
+                        [0, 1],
+                        marker=((-1, -1), (1, 1)),
+                        markersize=5,
+                        linestyle='none',
+                        color='k',
+                        mec='k',
+                        mew=1,
+                        clip_on=False,
+                        transform=ax.transAxes,
+                    )
+
+            elif i == len(axes) - 1 and len(axes) > 1:
+                # last section needs a set of / too, but on the left side
+                ax.spines["left"].set_visible(False)
+                ax.tick_params(labelleft=False, left=False)
+                ax.plot(
+                    [0, 0],
+                    [0, 1],
+                    marker=((-1, -1), (1, 1)),
+                    markersize=5,
+                    linestyle='none',
+                    color='k',
+                    mec='k',
+                    mew=1,
+                    clip_on=False,
+                    transform=ax.transAxes,
+                )
+
+            elif len(axes) > 1:
+                # middle sections need two sets of /
+                ax.spines["right"].set_visible(False)
+                ax.spines["left"].set_visible(False)
+                ax.tick_params(labelleft=False, labelright=False, left=False, right=False)
+                ax.plot(
+                    [0, 0],
+                    [0, 1],
+                    marker=((-1, -1), (1, 1)),
+                    markersize=5,
+                    linestyle='none',
+                    label="Silence Between Two Subplots",
+                    color='k',
+                    mec='k',
+                    mew=1,
+                    clip_on=False,
+                    transform=ax.transAxes,
+                )
+                ax.plot(
+                    [1, 1],
+                    [0, 1],
+                    marker=((-1, -1), (1, 1)),
+                    markersize=5,
+                    label="Silence Between Two Subplots",
+                    linestyle='none',
+                    color='k',
+                    mec='k',
+                    mew=1,
+                    clip_on=False,
+                    transform=ax.transAxes,
+                )
+
+            if peak_type.lower() != "delta":
+                ax.plot(
+                    x_values,
+                    y_values,
+                    color='k',
+                    linewidth=0.5,
+                    label="computed",
+                )
+
+            else:
+                if plot_type.lower() == "transmittance":
+                    ax.vlines(
+                        x_values,
+                        y_values,
+                        [100 for y in y_values],
+                        linewidth=0.5,
+                        colors=['k' for x in x_values],
+                        label="computed"
+                    )
+                    ax.hlines(
+                        100,
+                        0,
+                        max(4000, *x_values),
+                        linewidth=0.5,
+                        colors=['k' for y in y_values],
+                        label="computed",
+                    )
+                
+                else:
+                    ax.vlines(
+                        x_values,
+                        [0 for y in y_values],
+                        y_values,
+                        linewidth=0.5,
+                        colors=['k' for x in x_values],
+                        label="computed"
+                    )
+                    ax.hlines(
+                        0,
+                        0,
+                        max(4000, *x_values),
+                        linewidth=0.5,
+                        colors=['k' for y in y_values],
+                        label="computed"
+                    )
+
+            if exp_data:
+                for x, y, color in exp_data:
+                    ax.plot(x, y, color=color, zorder=-1, linewidth=0.5, label="observed")
+
+            center = centers[i]
+            width = widths[i]
+            high = center + width / 2
+            low = center - width / 2
+            if reverse_x:
+                ax.set_xlim(high, low)
+            else:
+                ax.set_xlim(low, high)
+        
+        # b/c we're doing things in sections, we can't add an x-axis label
+        # well we could, but which section would be put it one?
+        # it wouldn't be centered
+        # so instead the x-axis label is this
+        figure.text(0.5, 0.0, r"wavenumber (cm$^{-1}$)" , ha="center", va="bottom")
```

### Comparing `AaronTools-1.0b8/finders.py` & `AaronTools-1.0b9/finders.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/geometry.py` & `AaronTools-1.0b9/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 """For storing, manipulating, and measuring molecular structures"""
 import itertools
 import re
 import ssl
 from collections import deque
 from copy import deepcopy
-from warnings import warn
 
 import numpy as np
 from scipy.spatial import distance_matrix
 
 import AaronTools
 import AaronTools.utils.utils as utils
+from AaronTools import addlogger
 from AaronTools.atoms import Atom
 from AaronTools.config import Config
 from AaronTools.const import BONDI_RADII, D_CUTOFF, ELEMENTS, TMETAL, VDW_RADII
 from AaronTools.fileIO import FileReader, FileWriter
 from AaronTools.finders import Finder
 from AaronTools.utils.prime_numbers import Primes
 
 COORD_THRESHOLD = 0.2
 CACTUS_HOST = "https://cactus.nci.nih.gov"
 OPSIN_HOST = "https://opsin.ch.cam.ac.uk"
 
-DEFAULT_CONFIG = Config(skip_user_default=True, quiet=True)
+DEFAULT_CONFIG = Config(quiet=True)
 
 if not DEFAULT_CONFIG["DEFAULT"].getboolean("local_only"):
     import urllib.parse
     from urllib.error import HTTPError
     from urllib.request import urlopen
 
 
+@addlogger
 class Geometry:
     """
     Attributes:
         name
         comment
         atoms
         other
         _iter_idx
     """
 
+    # AaronTools.addlogger decorator will add logger to this class attribute
+    LOG = None
+    # decorator uses this to set log level (defaults to WARNING if None)
+    # LOGLEVEL = "INFO"
+    # add to this dict to override log level for specific functions
+    # keys are log level, values are lists of function names
+    # LOGLEVEL_OVERRIDE = {"DEBUG": "find"}
+
     Primes()
 
     def __init__(
         self,
         structure="",
         name="",
         comment="",
@@ -66,32 +75,31 @@
         self.atoms = []
         self.center = None
         self.components = components
         self.other = {}
         self._iter_idx = None
         self._sigmat = None
         self._epsmat = None
-
-        self.debug = False
+        self.LOG.debug("hello")
 
         if isinstance(structure, Geometry):
             # new from geometry
             self.atoms = structure.atoms
             if not name:
                 self.name = structure.name
             if not comment:
                 self.comment = structure.comment
             return
         elif isinstance(structure, FileReader):
             # get info from FileReader object
             from_file = structure
-        elif isinstance(structure, str) and structure != "":
+        elif isinstance(structure, str) and structure:
             # parse file
             from_file = FileReader(structure)
-        elif hasattr(structure, "__iter__") and structure != "":
+        elif hasattr(structure, "__iter__") and structure:
             for a in structure:
                 if not isinstance(a, Atom):
                     raise TypeError
             else:
                 # list of atoms supplied
                 self.atoms = structure
                 if refresh_connected:
@@ -156,20 +164,38 @@
                     "Cannot retrieve structure from {}. External network lookup disallowed.".format(
                         CACTUS_HOST
                     )
                 )
             url_sd = "{}/cgi-bin/translate.tcl?smiles={}&format=sdf&astyle=kekule&dim=3D&file=".format(
                 CACTUS_HOST, urllib.parse.quote(smiles)
             )
-            s_sd_get = (
-                urlopen(url_sd, context=ssl.SSLContext()).read().decode("utf8")
-            )
-            tmp_url = re.search(
-                'User-defined exchange format file: <a href="(.*)"', s_sd_get
-            ).group(1)
+            s_sd_get = urlopen(url_sd, context=ssl.SSLContext())
+            msg, status = s_sd_get.msg, s_sd_get.status
+            if msg != "OK":
+                cls.LOG.error(
+                    "Issue contacting %s for SMILES lookup (status: %s)",
+                    CACTUS_HOST,
+                    status,
+                )
+                raise IOError
+            s_sd_get = s_sd_get.read().decode("utf8")
+            try:
+                tmp_url = re.search(
+                    'User-defined exchange format file: <a href="(.*)"',
+                    s_sd_get,
+                ).group(1)
+            except AttributeError as err:
+                if re.search("You entered an invalid SMILES", s_sd_get):
+                    cls.LOG.error(
+                        "Invalid SMILES encountered: %s (consult %s for syntax help)",
+                        smiles,
+                        "https://cactus.nci.nih.gov/translate/smiles.html",
+                    )
+                    exit(1)
+                raise IOError(err)
             new_url = "{}{}".format(CACTUS_HOST, tmp_url)
             s_sd = (
                 urlopen(new_url, context=ssl.SSLContext())
                 .read()
                 .decode("utf8")
             )
             return s_sd
@@ -187,40 +213,308 @@
             smiles = name
         elif form == "iupac":
             smiles = cls.iupac2smiles(name)
 
         try:
             import rdkit.Chem.AllChem as rdk
 
-            scale_coords = False
             m = rdk.MolFromSmiles(smiles)
             if m is None and not strict_use_rdkit:
                 s_sd = get_cactus_sd(smiles)
             elif m:
                 mh = rdk.AddHs(m)
                 rdk.EmbedMolecule(mh, randomSeed=0x421C52)
                 s_sd = rdk.MolToMolBlock(mh)
             else:
                 raise RuntimeError(
                     "Could not load {} with RDKit".format(smiles)
                 )
         except ImportError:
-            scale_coords = True
             s_sd = get_cactus_sd(smiles)
 
         try:
             f = FileReader((name, "sd", s_sd))
             is_sdf = True
-        except Exception:
+        except ValueError:
             # for some reason, CACTUS is giving xyz files instead of sdf...
             is_sdf = False
-            f = FileReader((name, "xyz", s_sd))
+            try:
+                f = FileReader((name, "xyz", s_sd))
+            except ValueError:
+                cls.LOG.error("Error loading geometry:\n %s", s_sd)
+                raise
 
         return cls(f, refresh_connected=not is_sdf)
 
+    @classmethod
+    def get_coordination_complexes(
+        cls,
+        center,
+        ligands,
+        shape,
+        c2_symmetric=None,
+        minimize=False
+    ):
+        """
+        get all unique coordination complexes
+        uses templates from Inorg. Chem. 2018, 57, 17, 10557–10567
+
+        center - str, element of center atom
+        ligands - list of ligand names in the ligand library
+        shape - str, e.g. octahedral - see Atom.get_shape
+        c2_symmetric - list of bools, specifies which of the bidentate ligands are C2-symmetric
+                       if this list is as long as the ligands list, the nth item corresponds
+                       to the nth ligand
+                       otherwise, the nth item indicate the symmetry of the nth bidentate ligand
+        minimize - bool, use minimize=True when mapping ligands (see Geometry.map_ligand)
+
+        returns a list of cls containing all unique coordination complexes and the
+        general formula of the complexes
+        """
+        import os.path
+        from AaronTools.atoms import BondOrder
+        from AaronTools.const import AARONTOOLS
+        from AaronTools.component import Component
+        
+        if c2_symmetric is None:
+            c2_symmetric = [False for lig in ligands]
+        
+        bo = BondOrder()
+        
+        # create a geometry with the specified shape
+        # change the elements from dummy atoms to something else
+        start_atoms = Atom.get_shape(shape)
+        n_coord = len(start_atoms) - 1
+        start_atoms[0].element = center
+        for atom in start_atoms[1:]:
+            start_atoms[0].connected.add(atom)
+            atom.connected.add(start_atoms[0])
+            atom.element = "B"
+            atom._set_connectivity()
+            atom._set_radii()
+            atom._set_vdw()
+        geom = cls(start_atoms, refresh_connected=False)
+
+        # we'll need to determine the formula of the requested complex
+        # monodentate ligands are a, b, etc
+        # symmetric bidentate are AA, BB, etc
+        # asymmetric bidentate are AB, CD, etc
+        # ligands are sorted monodentate, followed by symmetric bidentate, followed by
+        # asymmetric bidentate, then by decreasing count
+        # e.g., Ca(CO)2(ACN)4 is Ma4b2
+        alphabet = "abcdefghi"
+        symmbet = ["AA", "BB", "CC", "DD"]
+        asymmbet = ["AB", "CD", "EF", "GH"]
+        monodentate_names = []
+        symm_bidentate_names = []
+        asymm_bidentate_names = []
+        
+        n_bidentate = 0
+        # determine types of ligands
+        for i, lig in enumerate(ligands):
+            comp = Component(lig)
+            if len(comp.key_atoms) == 1:
+                monodentate_names.append(lig)
+            elif len(comp.key_atoms) == 2:
+                if len(ligands) == len(c2_symmetric):
+                    c2 = c2_symmetric[i]
+                else:
+                    c2 = c2_symmetric[n_bidentate]
+                n_bidentate += 1
+                if c2:
+                    symm_bidentate_names.append(lig)
+                else:
+                    asymm_bidentate_names.append(lig)
+            else:
+                # tridentate or something
+                raise NotImplementedError(
+                    "can only attach mono- and bidentate ligands: %s (%i)" % (
+                        lig, len(comp.key_atoms)
+                    )
+                )
+        
+        coord_num = (
+            len(monodentate_names) + 
+            2 * (
+                len(symm_bidentate_names) + len(asymm_bidentate_names)
+            )
+        )
+        if coord_num != n_coord:
+            raise RuntimeError(
+                "coordination number (%i) does not match sum of ligand denticity (%i)" % (
+                    n_coord, coord_num
+                )
+            )
+        
+        # start putting formula together
+        cc_type = "M"
+        this_name = center
+        # sorted by name count is insufficient when there's multiple monodentate ligands
+        # with the same count (e.g. Ma3b3)
+        # add the index in the library to offset this
+
+        monodentate_names = sorted(
+            monodentate_names,
+            key=lambda x: 10000 * monodentate_names.count(x) + Component.list().index(x),
+            reverse=True,
+        )
+        for i, mono_lig in enumerate(
+            sorted(
+                set(monodentate_names),
+                key=lambda x: 10000 * monodentate_names.count(x) + Component.list().index(x),
+                reverse=True,
+            )
+        ):
+            cc_type += alphabet[i]
+            this_name += "(%s)" % mono_lig
+            if monodentate_names.count(mono_lig) > 1:
+                cc_type += "%i" % monodentate_names.count(mono_lig)
+                this_name += "%i" % monodentate_names.count(mono_lig)
+
+        symm_bidentate_names = sorted(
+            symm_bidentate_names,
+            key=lambda x: 10000 * symm_bidentate_names.count(x) + Component.list().index(x),
+            reverse=True
+        )
+        for i, symbi_lig in enumerate(sorted(
+                set(symm_bidentate_names),
+                key=lambda x: 10000 * symm_bidentate_names.count(x) + Component.list().index(x),
+                reverse=True
+            )
+        ):
+            cc_type += "(%s)" % symmbet[i]
+            this_name += "(%s)" % symbi_lig
+            if symm_bidentate_names.count(symbi_lig) > 1:
+                cc_type += "%i" % symm_bidentate_names.count(symbi_lig)
+                this_name += "%i" % symm_bidentate_names.count(symbi_lig)
+        asymm_bidentate_names = sorted(
+            asymm_bidentate_names,
+            key=lambda x: 10000 * asymm_bidentate_names.count(x) + Component.list().index(x),
+            reverse=True
+        )
+        for i, asymbi_lig in enumerate(
+            sorted(
+                set(asymm_bidentate_names),
+                key=lambda x: 10000 * asymm_bidentate_names.count(x) + Component.list().index(x),
+                reverse=True
+            )
+        ):
+            cc_type += "(%s)" % asymmbet[i]
+            this_name += "(%s)" % asymbi_lig
+            if asymm_bidentate_names.count(asymbi_lig) > 1:
+                cc_type += "%i" % asymm_bidentate_names.count(asymbi_lig)
+                this_name += "%i" % asymm_bidentate_names.count(asymbi_lig)
+
+        # load the key atoms for ligand mapping from the template file
+        libdir = os.path.join(
+            AARONTOOLS,
+            "coordination_complex",
+            shape,
+            cc_type
+        )
+        if not os.path.exists(libdir):
+            raise RuntimeError("no templates for %s %s" % (cc_type, shape))
+
+        geoms = []
+        for f in os.listdir(libdir):
+            mappings = np.loadtxt(os.path.join(libdir, f), dtype=str, delimiter=",", ndmin=2)
+            
+            point_group, subset = f.rstrip(".csv").split("_")            
+            # for each possible structure, create a copy of the original template shape
+            # attach ligands in the order they would appear in the formula
+            for i, mapping in enumerate(mappings):
+                geom_copy = geom.copy()
+                geom_copy.center = [geom_copy.atoms[0]]
+                geom_copy.components = [Component([atom]) for atom in geom_copy.atoms[1:]]
+            
+                start = 0
+                for lig in monodentate_names:
+                    key = mapping[start]
+                    start += 1
+                    comp = Component(lig)
+                    d = 2.5
+                    # adjust distance to key atoms to what they should be for the new ligand
+                    try:
+                        d = bo.bonds[bo.key(center, comp.key_atoms[0])]["1.0"]
+                    except KeyError:
+                        pass
+                    geom_copy.change_distance(
+                        geom_copy.atoms[0],
+                        key,
+                        dist=d,
+                        fix=1
+                    )
+                    # attach ligand
+                    geom_copy.map_ligand(comp, key, minimize=minimize)
+                
+                for lig in symm_bidentate_names:
+                    keys = mapping[start:start + 2]
+                    start += 2
+                    comp = Component(lig)
+                    for old_key, new_key in zip(keys, comp.key_atoms):
+                        d = 2.5
+                        try:
+                            d = bo.bonds[bo.key(center, new_key)]["1.0"]
+                        except KeyError:
+                            pass
+                        geom_copy.change_distance(
+                            geom_copy.atoms[0],
+                            old_key,
+                            dist=d,
+                            fix=1,
+                            as_group=False
+                        )
+                    geom_copy.map_ligand(comp, keys, minimize=minimize)
+                    
+                for lig in asymm_bidentate_names:
+                    keys = mapping[start:start + 2]
+                    start += 2
+                    comp = Component(lig)
+                    for old_key, new_key in zip(keys, comp.key_atoms):
+                        d = 2.5
+                        try:
+                            d = bo.bonds[bo.key(center, new_key)]["1.0"]
+                        except KeyError:
+                            pass
+                        geom_copy.change_distance(
+                            geom_copy.atoms[0],
+                            old_key,
+                            dist=d,
+                            fix=1,
+                            as_group=False
+                        )
+                    geom_copy.map_ligand(comp, keys, minimize=minimize)
+            
+                geom_copy.name = "%s-%i_%s_%s" % (this_name, i + 1, point_group, subset)
+                geoms.append(geom_copy)
+        
+        return geoms, cc_type
+
+    @staticmethod
+    def weighted_percent_buried_volume(geometries, energies, temperature, *args, **kwargs):
+        """
+        Boltzmann-averaged percent buried volume
+        geometries - list of Geometry instances
+        energies - numpy array, energy in kcal/mol; ith energy corresponds to ith substituent
+        temperature - temperature in K
+        *args, **kwargs - passed to Geometry.percent_buried_volume()
+        """
+        values = []
+        
+        for geom in geometries:
+            values.append(geom.percent_buried_volume(*args, **kwargs))
+        
+        rv = utils.boltzmann_average(
+            energies,
+            np.array(values),
+            temperature,
+        )
+        
+        return rv
+        
     # attribute access
     def _stack_coords(self, atoms=None):
         """
         Generates a N x 3 coordinate matrix for atoms
         Note: the matrix rows are copies of, not references to, the
             Atom.coords objects. Run Geometry.update_geometry(matrix) after
             using this method to save changes.
@@ -252,14 +546,20 @@
             (defaults to all atoms)
         """
         if atoms is None:
             return self._stack_coords()
         return self._stack_coords(atoms)
 
     # utilities
+    def __str__(self):
+        s = ""
+        for a in self:
+            s += a.__str__() + "\n"
+        return s
+
     def __repr__(self):
         """ string representation """
         s = ""
         for a in self:
             s += a.__repr__() + "\n"
         return s
 
@@ -342,22 +642,22 @@
             # only use the first 3 decimal places of coordinates b/c numerical issues
             t.append(int(atom.get_neighbor_id()))
             if not atom._hashed:
                 atom.connected = frozenset(atom.connected)
                 atom.coords.setflags(write=False)
                 atom._hashed = True
             # make sure atoms don't move
-            # if atoms move, the hash value could change making it impossible to access
+            # if atoms move, te hash value could change making it impossible to access
             # items in a dictionary with this instance as the key
 
         if not self._hashed:
-            warn(
-                "%s %s has been hashed and will no longer be editable\n"
-                % (self.__class__.__name__, self.name)
-                + "use Geometry.copy to get an editable duplicate of this instance"
+            self.LOG.warning(
+                "Geometry `%s` has been hashed and will no longer be editable.\n"
+                "Use Geometry.copy to get an editable duplicate of this instance",
+                self.name,
             )
             self.atoms = tuple(self.atoms)
             self._hashed = True
 
         return hash(tuple(t))
 
     def tag(self, tag, targets=None):
@@ -712,59 +1012,59 @@
                 but were screened out using the && argument form
         """
 
         def _find(arg):
             """ find a single atom """
             # print(arg)
             if isinstance(arg, Atom):
-                # print('atom')
+                # print("atom")
                 return [arg]
 
             rv = []
             if isinstance(arg, Finder):
-                # print('finder')
+                # print("finder")
                 rv += arg.get_matching_atoms(self.atoms, self)
 
             name_str = re.compile("^(\*|\d)+(\.?\*|\.\d+)*$")
             if isinstance(arg, str) and name_str.match(arg) is not None:
-                # print('name')
+                # print("name")
                 test_name = arg.replace(".", "\.")
                 test_name = test_name.replace("*", "(\.?\d+\.?)*")
                 test_name = re.compile("^" + test_name + "$")
                 # this is a name
                 for a in self.atoms:
                     if test_name.search(a.name) is not None:
                         rv += [a]
 
             elif isinstance(arg, str) and len(arg.split(",")) > 1:
-                # print('comma list')
+                # print("comma list")
                 list_style = arg.split(",")
                 if len(list_style) > 1:
                     for i in list_style:
                         if len(i.split("-")) > 1:
                             rv += _find_between(i)
                         else:
                             rv += _find(i)
 
             elif (
                 isinstance(arg, str)
                 and len(arg.split("-")) > 1
                 and not re.search("[A-Za-z]", arg)
             ):
-                # print('range list')
+                # print("range list")
                 rv += _find_between(arg)
 
             elif isinstance(arg, str) and arg in ELEMENTS:
-                # print('element')
+                # print("element")
                 # this is an element
                 for a in self.atoms:
                     if a.element == arg:
                         rv += [a]
             else:
-                # print('tag')
+                # print("tag")
                 # this is a tag
                 for a in self.atoms:
                     if arg in a.tags:
                         rv += [a]
             return rv
 
         def _find_between(arg):
@@ -880,31 +1180,35 @@
         for a, con in zip(atoms, connectivity):
             a.connected = set([])
             for c in con:
                 a.connected.add(atoms[c])
 
         return atoms
 
-    def refresh_connected(self, threshold=None):
+    def refresh_connected(self, targets=None, threshold=None):
         """
         reset connected atoms
         atoms are connected if their distance from each other is less than
             the sum of their covalent radii plus a threshold
         """
         # clear current connectivity
+        if targets is None:
+            targets = self.atoms
+        else:
+            targets = self.find(targets)
         old_connectivity = []
-        for a in self.atoms:
+        for a in targets:
             old_connectivity += [a.connected]
             a.connected = set([])
 
-        D = distance_matrix(self.coords, self.coords)
+        D = distance_matrix(self.coordinates(targets), self.coordinates(targets))
 
         # determine connectivity
-        for i, a in enumerate(self.atoms):
-            for j, b in enumerate(self.atoms[:i]):
+        for i, a in enumerate(targets):
+            for j, b in enumerate(targets[:i]):
                 if a.dist_is_connected(b, D[i, j], threshold):
                     a.connected.add(b)
                     b.connected.add(a)
 
     def refresh_ranks(self, invariant=True):
         rank = self.canonical_rank(invariant=invariant)
         for a, r in zip(self.atoms, rank):
@@ -912,19 +1216,26 @@
         return
 
     def canonical_rank(
         self, heavy_only=False, break_ties=True, update=True, invariant=True
     ):
         """
         determine canonical ranking for atoms
-        invariant: bool - if True, use invariant described in 10.1021/ci00062a008
+        invariant: bool - if True, use invariant described in J. Chem. Inf. Comput. Sci. 1989, 29, 2, 97–101
+                          (DOI: 10.1021/ci00062a008)
                           if False, use neighbor IDs
 
-        algorithm described in 10.1021/acs.jcim.5b00543
+        algorithm described in J. Chem. Inf. Model. 2015, 55, 10, 2111–2120 
+        (DOI: 10.1021/acs.jcim.5b00543)
         """
+        CITATION = "doi:10.1021/ci00062a008"
+        self.LOG.citation(CITATION)
+        CITATION = "doi:10.1021/acs.jcim.5b00543"
+        self.LOG.citation(CITATION)
+
         primes = Primes.list(len(self.atoms))
         atoms = []
         ranks = []
 
         # using the catalyst's center can make it difficult
         # to compare C2 symmetric ligands
         # center = list(filter(lambda x: "center" in x.tags, self))
@@ -1103,27 +1414,31 @@
         # re-rank using neighbors until no change
         for i in range(500):
             new_ranks = neighbors_rank(ranks)
             if ranks == new_ranks:
                 break
             ranks = new_ranks
         else:
-            warn("Max cycles reached in canonical sorting (neighbor-ranks)")
+            self.LOG.warning(
+                "Max cycles reached in canonical sorting (neighbor-ranks)"
+            )
 
         # break ties using spatial positions
         # AND update neighbors until no change
         if break_ties:
             for i in range(500):
                 new_ranks = tie_break(ranks)
                 new_ranks = neighbors_rank(new_ranks)
                 if ranks == new_ranks:
                     break
                 ranks = new_ranks
             else:
-                warn("Max cycles reached in canonical sorting (tie-breaking)")
+                self.LOG.warning(
+                    "Max cycles reached in canonical sorting (tie-breaking)"
+                )
 
         return ranks
 
     def reorder(
         self,
         start=None,
         targets=None,
@@ -1315,17 +1630,14 @@
             raise LookupError(
                 "could not determine best path between {} and {}".format(
                     atom1, atom2
                 )
             )
         return [self.atoms[i] for i in path]
 
-    # nothing in AaronTools refers to short_walk anymore
-    short_walk = shortest_path
-
     # geometry measurement
     def bond(self, a1, a2):
         """ takes two atoms and returns the bond vector """
         a1, a2 = self.find_exact(a1, a2)
         return a1.bond(a2)
 
     def angle(self, a1, a2, a3=None):
@@ -1829,16 +2141,17 @@
         method="lebedev",
         rpoints=20,
         apoints=1454,
         min_iter=25,
         basis=None,
     ):
         """
-        calculates % buried volume (%V_bur)
-        Monte-Carlo or Gauss-Legendre/Lebedev integration
+        calculates % buried volume (%V_bur) using Monte-Carlo or Gauss-Legendre/Lebedev integration
+        see Organometallics 2008, 27, 12, 2679–2681 (DOI: 10.1021/om8001119) for details
+
         center  - center atom(s) or np.array of coordinates
                   if more than one atom is specified, the sphere will be centered on
                   the centroid between the atoms
         targets - atoms to use in calculation, defaults to all non-center if there
                   is only one center, otherwise all atoms
         radius  - sphere radius around center atom
         radii   - "umn" or "bondi", VDW radii to use
@@ -2443,16 +2756,19 @@
 
         # determine new bond length
         if isinstance(dist, str):
             dist = float(dist)
         if dist is None:
             if hasattr(a1, "_radii") and hasattr(a2, "_radii"):
                 new_dist = a1._radii + a2._radii
-            else:
-                warn("no radii for one of:\n%s\n%s" % (a1, a2))
+            elif not hasattr(a1, "_radii"):
+                self.LOG.warning("no radii for %s", a1)
+                return
+            elif not hasattr(a2, "_radii"):
+                self.LOG.warning("no radii for %s", a2)
                 return
         elif adjust:
             new_dist = a1.dist(a2) + dist
         else:
             new_dist = dist
         dist = a1.dist(a2)
 
@@ -2692,17 +3008,16 @@
             a1, a2, a3, a4 = self.find_exact(*args[:4])
             dihedral = args[4]
         # get fragments
         if as_group:
             a2_frag = self.get_fragment(a2, a3)[1:]
             a3_frag = self.get_fragment(a3, a2)[1:]
             if any(atom in a2_frag for atom in a3_frag):
-                warn(
-                    "changing dihedral that is in a ring:\n%s, %s"
-                    % (str(a2), str(a3))
+                self.LOG.warning(
+                    "changing dihedral that is part of a ring: %s %s", a2, a3
                 )
         else:
             a2_frag = [a1]
             a3_frag = [a4]
 
         # fix units
         if not radians:
@@ -2828,15 +3143,15 @@
 
             if E_min is None or energy < E_min:
                 E_min = energy
                 angle_min = angle
 
         # rotate to min angle
         self.rotate(
-            axis, np.deg2rad(angle_min - angle), targets=targets, center=center
+            axis, np.deg2rad(angle_min - angle), targets=targets, center=center_coords
         )
 
         return
 
     def substitute(self, sub, target, attached_to=None, minimize=False):
         """
         substitutes fragment containing `target` with substituent `sub`
@@ -3649,15 +3964,18 @@
                 new_axis = shift - new_key.coords
             else:
                 targets = old_key.connected - set(self.center)
                 new_axis = (
                     ligand.COM(targets=new_key.connected) - new_key.coords
                 )
 
-            old_axis = self.COM(targets=targets) - old_key.coords
+            if not targets:
+                old_axis = old_key.coords - self.COM(self.center)
+            else:
+                old_axis = self.COM(targets=targets) - old_key.coords
             w, angle = get_rotation(old_axis, new_axis)
             ligand.rotate(w, angle, center=new_key)
             return ligand
 
         def map_2_key(old_ligand, ligand, old_keys, new_keys, rev_ang=False):
 
             # align COM of key atoms
@@ -3674,44 +3992,51 @@
             except (LookupError, ValueError):
                 # for some ferrocene ligands, AaronTools misidentifies the Fe
                 # as another metal center
                 # we'll remove any centers that are on the path between the key atoms
                 # also, sometimes the ligand atoms don't have the center in their connected
                 # attribute, even though the center has the ligand atoms in its
                 # connected attribute, so refresh_connected
-                self.refresh_connected()
+                self.refresh_connected(targets=self.center)
                 # print("old keys:", old_keys)
                 # print("old ligand:\n", old_ligand)
-                frag = old_ligand.get_fragment(
-                    old_keys[0],
-                    stop=[
-                        atom
-                        for atom in old_keys[0].connected
-                        if atom not in old_ligand.atoms
-                    ],
-                )
-                if all(atom in frag for atom in old_keys):
-                    # for atom in frag:
-                    #     print("frag:", atom)
-                    old_walk = self.shortest_path(
-                        *old_keys,
-                        avoid=[
-                            a
-                            for a in self.center
-                            if any(k.is_connected(a) for k in old_keys)
-                        ]
+                stop=[
+                    atom
+                    for atom in old_keys[0].connected
+                    if atom not in old_ligand.atoms
+                ]
+                if stop:
+                    frag = old_ligand.get_fragment(
+                        old_keys[0],
+                        stop=stop,
                     )
-                    remove_centers = [c for c in self.center if c in old_walk]
+                    if all(atom in frag for atom in old_keys):
+                        old_walk = self.shortest_path(
+                            *old_keys,
+                            avoid=[
+                                a
+                                for a in self.center
+                                if any(k.is_connected(a) for k in old_keys)
+                            ]
+                        )
+                        remove_centers = [c for c in self.center if c in old_walk]
+                
+                else:
+                    old_walk = [a for a in old_keys]
 
             if old_walk and len(old_walk) == 2:
                 old_con = set([])
                 for k in old_keys:
                     for c in k.connected:
                         old_con.add(c)
-                old_vec = old_ligand.COM(targets=old_con) - center
+                if old_con:
+                    old_vec = old_ligand.COM(targets=old_con) - center
+                else:
+                    old_vec = center
+
             elif old_walk:
                 old_vec = old_ligand.COM(targets=old_walk[1:-1]) - center
             else:
                 old_vec = np.zeros(3)
                 for atom in old_keys:
                     if any(
                         bonded_atom not in old_ligand.atoms
@@ -4134,15 +4459,15 @@
             if conf_num in skip or skip == "all":
                 self = original
                 return conf_spec, False
             sub = self.find_substituent(start)
             # validate conf_spec
             if conf_num > sub.conf_num:
                 self = original
-                warn(
+                self.LOG.warning(
                     "Bad conformer number given: {} {} > {}".format(
                         sub.name, conf_num, sub.conf_num
                     )
                 )
                 return conf_spec, False
             if conf_num > current:
                 n_rot = conf_num - current - 1
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AaronTools-1.0b8/job_control.py` & `AaronTools-1.0b9/job_control.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import os
 import re
 import subprocess
 from time import sleep
-from warnings import warn
 
 from jinja2 import Environment, FileSystemLoader
 
+from AaronTools import addlogger
 from AaronTools.const import AARONLIB
 
 USER = os.getenv("USER")
-QUEUE_TYPE = os.getenv("QUEUE_TYPE").upper()
+QUEUE_TYPE = os.getenv("QUEUE_TYPE", "None").upper()
 
 
 class JobControl:
     pass
 
 
+@addlogger
 class SubmitProcess:
     """class for submitting jobs to the queue
     attributes:
 
     name:       name of job and input file minus the extension
     exe:        type of input file (com, in, inp)
     directory:  directory the input file is in
     walltime:   allocated walltime in hours
     processors: allocated processors
     memory:     allocated memory in GB
     template:   template job file"""
 
+    LOG = None
+
     def __init__(self, fname, walltime, processors, memory, template=None):
         """fname:   str     - path to input file (e.g. /home/CoolUser/CoolStuff/neat.com
         walltime:   int/str - walltime in hours
         processors: int/str - allocated processors
         memory:     int/str - allocated memory in GB
         template:   str     - path to template file; if template is None, will look for
                               psi4.job, orca.job, or gaussian.job (depending on
@@ -52,15 +55,15 @@
         if QUEUE_TYPE == "LSF":
             args = ["bjobs", "-l", "2"]
             proc = subprocess.Popen(
                 args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
             )
             out, err = proc.communicate()
             if len(err) != 0 and retry:
-                warn(
+                SubmitProcess.LOG.warning(
                     "error checking queue: %s\nsleeping 300s before trying again"
                     % err.decode("utf-8")
                 )
                 sleep(300)
                 return SubmitProcess.unfinished_jobs_in_dir(directory, retry)
 
             else:
@@ -82,15 +85,15 @@
         elif QUEUE_TYPE == "PBS":
             args = ["qstat", "-fx"]
             proc = subprocess.Popen(
                 args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
             )
             out, err = proc.communicate()
             if len(err) != 0 and retry:
-                warn(
+                SubmitProcess.LOG.warning(
                     "error checking queue: %s\nsleeping 300s before trying again"
                     % err.decode("utf-8")
                 )
                 sleep(300)
                 return SubmitProcess.unfinished_jobs_in_dir(directory, retry)
 
             else:
@@ -118,15 +121,15 @@
         elif QUEUE_TYPE == "SLURM":
             args = ["squeue", "-o", "%i#%Z#%t", "-u", USER]
             proc = subprocess.Popen(
                 args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
             )
             out, err = proc.communicate()
             if len(err) != 0 and retry:
-                warn(
+                SubmitProcess.LOG.warning(
                     "error checking queue: %s\nsleeping 300s before trying again"
                     % err.decode("utf-8")
                 )
                 sleep(300)
                 return SubmitProcess.unfinished_jobs_in_dir(directory, retry)
 
             else:
@@ -147,15 +150,15 @@
             # we then call qstat again to get the directory those jobs are in
             args = ["qstat", "-s", "pr", "-u", USER]
             proc = subprocess.Popen(
                 args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
             )
             out, err = proc.communicate()
             if len(err) != 0 and retry:
-                warn(
+                SubmitProcess.LOG.warning(
                     "error checking queue: %s\nsleeping 300s before trying again"
                     % err.decode("utf-8")
                 )
                 sleep(300)
                 return SubmitProcess.unfinished_jobs_in_dir(directory, retry)
 
             else:
@@ -168,15 +171,15 @@
 
                 args = ["qstat", "-j", jlist]
                 proc = subprocess.Popen(
                     args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
                 )
                 out, err = proc.communicate()
                 if len(err) != 0 and retry:
-                    warn(
+                    SubmitProcess.LOG.warning(
                         "error checking queue: %s\nsleeping 300s before trying again"
                         % err.decode("utf-8")
                     )
                     sleep(300)
                     return SubmitProcess.unfinished_jobs_in_dir(
                         directory, retry
                     )
```

### Comparing `AaronTools-1.0b8/json_extension.py` & `AaronTools-1.0b9/json_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
                     try:
                         rv["jobs"][job_type][arg] = getattr(job, arg)
                     except AttributeError:
                         pass
                 
         if obj.basis:
             rv["basis"] = {"name": [], "elements":[], "file":[], "auxiliary":[]}
-            if obj.basis:
+            if obj.basis.basis:
                 for basis in obj.basis.basis:
                     rv["basis"]["name"].append(basis.name)
                     rv["basis"]["elements"].append([])
                     for ele in basis.ele_selection:
                         if isinstance(ele, str):
                             rv["basis"]["elements"][-1].append(ele)
                         elif isinstance(ele, AnyTransitionMetal):
```

### Comparing `AaronTools-1.0b8/new_fileIO.py` & `AaronTools-1.0b9/new_fileIO.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/pathway.py` & `AaronTools-1.0b9/pathway.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/ring.py` & `AaronTools-1.0b9/ring.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/setup.py` & `AaronTools-1.0b9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     name="AaronTools",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="1.0b8",  # Required
+    version="1.0b9",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Tools for measuring and manipulating molecular structures",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `AaronTools-1.0b8/substituent.py` & `AaronTools-1.0b9/substituent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,57 @@
+#!/usr/bin/env python3
 """for fragments attached to a structure by one bond"""
 
-#!/usr/bin/env python3
 import json
 import os
 import re
 import sys
 from copy import deepcopy
-from glob import glob
-from warnings import warn
 
 import numpy as np
 
+from AaronTools import addlogger
 from AaronTools.const import AARONLIB, AARONTOOLS, BONDI_RADII, VDW_RADII
 from AaronTools.fileIO import FileReader, read_types
 from AaronTools.geometry import Geometry
-from AaronTools.utils.utils import rotation_matrix
+from AaronTools.utils.utils import perp_vector, boltzmann_average
 
 
+@addlogger
 class Substituent(Geometry):
     """
     Attributes:
         name
         atoms
         end         the atom substituent is connected to
         conf_num    number of conformers
         conf_angle  angle to rotate by to make next conformer
     """
 
+    LOG = None
     AARON_LIBS = os.path.join(AARONLIB, "Subs")
     BUILTIN = os.path.join(AARONTOOLS, "Substituents")
     CACHE_FILE = os.path.join(AARONLIB, "cache", "substituents.json")
 
     try:
         with open(CACHE_FILE) as f:
             cache = json.load(f)
     except (FileNotFoundError, json.decoder.JSONDecodeError):
         cache = {}
         cache["lengths"] = {}  # for storing number of atoms in each sub
 
     def __init__(
-            self,
-            sub=None,
-            name=None,
-            targets=None,
-            end=None,
-            conf_num=None,
-            conf_angle=None,
-            detect=True,
+        self,
+        sub=None,
+        name=None,
+        targets=None,
+        end=None,
+        conf_num=None,
+        conf_angle=None,
+        detect=True,
     ):
         """
         sub is either a file sub, a geometry, or an atom list
         """
         super().__init__()
         self.name = name
         self.atoms = []
@@ -104,15 +105,15 @@
                     name, ext = os.path.splitext(f)
                     if not any(".%s" % x == ext for x in read_types):
                         continue
                     match = sub == name
                     if match:
                         fsub = os.path.join(lib, f)
                         break
-                
+
                 if fsub:
                     break
 
             # or assume we were given a file name instead
             if not fsub and ".xyz" in sub:
                 fsub = sub
                 sub = os.path.basename(sub).rstrip(".xyz")
@@ -129,15 +130,15 @@
                         bond /= np.linalg.norm(bond)
                         rot_axis /= np.linalg.norm(rot_axis)
                         angle = np.arccos(np.dot(bond, x_axis))
                         fsub.rotate(rot_axis, angle)
                     self.atoms = fsub.atoms[1:]
                     self.refresh_connected()
                     self.name = match.group(1)
-                    warn("Conformer info not loaded for" + sub)
+                    self.LOG.warning("Conformer info not loaded for" + sub)
                     return
                 else:
                     raise RuntimeError(
                         "substituent name not recognized: %s" % sub
                     )
 
             # load in atom info
@@ -151,43 +152,76 @@
 
             # set conformer info
             conf_info = re.search(r"CF:(\d+),(\d+)", self.comment)
             if conf_info is not None:
                 self.conf_num = int(conf_info.group(1))
                 self.conf_angle = np.deg2rad(float(conf_info.group(2)))
             else:
-                warn("Conformer info not loaded for" + f)
+                self.LOG.warning("Conformer info not loaded for" + f)
 
         if not self.name:
             self.name = "sub"
         if self.name == "sub" and end is not None:
             self.name += "-{}".format(end.name)
 
     def __lt__(self, other):
         if self.end < other.end and not other.end < self.end:
             return True
         if len(self.atoms) != len(other.atoms):
             return len(self.atoms) < len(other.atoms)
         for a, b in zip(
-                self.reorder(start=self.atoms[0])[0],
-                other.reorder(start=other.atoms[0])[0],
+            self.reorder(start=self.atoms[0])[0],
+            other.reorder(start=other.atoms[0])[0],
         ):
             if a < b and not b < a:
                 return True
         return False
 
+    @staticmethod
+    def weighted_sterimol(substituents, energies, temperature, *args, **kwargs):
+        """
+        returns Boltzmann-averaged sterimol parameters for the substituents
+        substituents - list of Substituent instances
+        energies - numpy array, energy in kcal/mol; ith energy corresponds to ith substituent
+        temperature - temperature in K
+        *args, **kwargs - passed to Substituent.sterimol()
+        """
+        CITATION = "doi:10.1021/acscatal.8b04043"
+        Substituent.LOG.citation(CITATION)
+        values = {
+            "B1": [],
+            "B2": [],
+            "B3": [],
+            "B4": [],
+            "B5": [],
+            "L": [],
+        }
+        
+        rv = dict()
+        
+        for sub in substituents:
+            data = sub.sterimol(*args, **kwargs)
+            for key in data.keys():
+                values[key].append(data[key])
+        
+        for key in values.keys():
+            values[key] = np.array(values[key])
+            rv[key] = boltzmann_average(energies, values[key], temperature)
+        
+        return rv
+
     @classmethod
     def from_string(
-            cls,
-            name,
-            conf_num=None,
-            conf_angle=None,
-            form="smiles",
-            debug=False,
-            strict_use_rdkit=False,
+        cls,
+        name,
+        conf_num=None,
+        conf_angle=None,
+        form="smiles",
+        debug=False,
+        strict_use_rdkit=False,
     ):
         """
         creates a substituent from a string
         name        str     identifier for substituent
         conf_num    int     number of conformers expected for hierarchical conformer generation
         conf_angle  int     angle between conformers
         form        str     type of identifier (smiles, iupac)
@@ -223,15 +257,15 @@
                     my_rad = rad
                     break
                 elif "+" not in rad and "-" not in rad:
                     my_rad = rad
                     break
         if my_rad is None:
             if radicals:
-                warn(
+                cls.LOG.warning(
                     "radical atom may be ambiguous, be sure to check output: %s"
                     % smiles
                 )
                 my_rad = radicals[0]
             else:
                 raise RuntimeError(
                     "could not determine radical site on %s; radical site is expected to be in []"
@@ -339,18 +373,18 @@
         for lib in [cls.AARON_LIBS, cls.BUILTIN]:
             if not os.path.exists(lib):
                 continue
             for f in os.listdir(lib):
                 name, ext = os.path.splitext(os.path.basename(f))
                 if not any(".%s" % x == ext for x in read_types):
                     continue
-                
+
                 if name in names:
                     continue
-                
+
                 if include_ext:
                     names.append(name + ext)
                 else:
                     names.append(name)
 
         return names
 
@@ -374,60 +408,64 @@
             for filename in os.listdir(lib):
                 name, ext = os.path.splitext(filename)
                 if not any(".%s" % x == ext for x in read_types):
                     continue
 
                 # test number of atoms against cache
                 if (
-                        name in sub_lengths
-                        and len(test_sub.atoms) != sub_lengths[name]
+                    name in sub_lengths
+                    and len(test_sub.atoms) != sub_lengths[name]
                 ):
                     continue
-                
+
                 # use Geometry until we've done all the checks we can do without
                 # determining connectivity
                 # (for performance reasons)
                 init_ref = Geometry(
                     os.path.join(lib, name + ext),
                     refresh_connected=False,
                     refresh_ranks=False,
                 )
                 # add to cache
                 sub_lengths[name] = len(init_ref.atoms)
                 cache_changed = True
-    
+
                 # want same number of atoms
                 if len(test_sub.atoms) != len(init_ref.atoms):
                     continue
 
                 # same number of each element
                 ref_eles = [atom.element for atom in init_ref.atoms]
                 test_eles = [atom.element for atom in test_sub.atoms]
-                ref_counts = {ele:ref_eles.count(ele) for ele in set(ref_eles)}
-                test_counts = {ele:test_eles.count(ele) for ele in set(test_eles)}
+                ref_counts = {
+                    ele: ref_eles.count(ele) for ele in set(ref_eles)
+                }
+                test_counts = {
+                    ele: test_eles.count(ele) for ele in set(test_eles)
+                }
                 if ref_counts != test_counts:
                     continue
 
                 ref_sub = Substituent(init_ref, detect=False)
                 ref_sub.name = name
                 ref_sub.refresh_connected()
                 ref_sub.refresh_ranks()
-    
+
                 for a, b in zip(sorted(test_sub.atoms), sorted(ref_sub.atoms)):
                     # want correct elements
                     if a.element != b.element:
                         break
                     # and correct connections
                     if len(a.connected) != len(b.connected):
                         break
                     # and correct connected elements
                     failed = False
                     for i, j in zip(
-                            sorted([aa.element for aa in a.connected]),
-                            sorted([bb.element for bb in b.connected]),
+                        sorted([aa.element for aa in a.connected]),
+                        sorted([bb.element for bb in b.connected]),
                     ):
                         if i != j:
                             failed = True
                             break
                     if failed:
                         break
                 else:
@@ -448,319 +486,302 @@
                 os.makedirs(os.path.dirname(Substituent.CACHE_FILE))
 
             with open(Substituent.CACHE_FILE, "w") as f:
                 json.dump(Substituent.cache, f)
 
         return found
 
-    def sterimol(self, parameter="L", return_vector=False, radii="bondi"):
-        """returns sterimol parameter value for the specified parameter
-        return_vector: bool/returns tuple(vector start, vector end) instead
-        parameter (str) can be:
-            "L"
-            "B1"
-            "B5"
+    def sterimol(self, return_vector=False, radii="bondi", old_L=False):
+        """
+        returns sterimol parameter values in a dictionary
+        keys are B1, B2, B3, B4, B5, and L
+        see Verloop, A. and Tipker, J. (1976), Use of linear free energy
+        related and other parameters in the study of fungicidal
+        selectivity. Pestic. Sci., 7: 379-390.
+        (DOI: 10.1002/ps.2780070410)
+
+        return_vector: bool/returns dict of tuple(vector start, vector end) instead
         radii: "bondi" - Bondi vdW radii
                "umn"   - vdW radii from Mantina, Chamberlin, Valero, Cramer, and Truhlar
+        old_L: bool - True: use original L (ideal bond length between first substituent
+                            atom and hydrogen + 0.40 angstrom
+                      False: use AaronTools definition
+
+        AaronTools' definition of the L parameter is different than the original
+        STERIMOL program. In STERIMOL, the van der Waals radii of the substituent is
+        projected onto a plane parallel to the bond between the molecule and the substituent.
+        The L parameter is 0.40 Å plus the distance from the first substituent atom to the
+        outer van der Waals surface of the projection along the bond vector. This 0.40 Å is
+        a correction for STERIMOL using a hydrogen to represent the molecule, when a carbon
+        would be more likely. In AaronTools the substituent is projected the same, but L is
+        calculated starting from the van der Waals radius of the first substituent atom
+        instead. This means AaronTools will give the same L value even if the substituent
+        is capped with something besides a hydrogen. When comparing AaronTools' L values
+        with STERIMOL (using the same set of radii for the atoms), the values usually
+        differ by < 0.1 Å.
         """
+        from AaronTools.finders import BondedTo
+        from scipy.spatial import ConvexHull
+
+        CITATION = "doi:10.1002/ps.2780070410"
+        self.LOG.citation(CITATION)
+
         if self.end is None:
             raise RuntimeError(
                 "cannot calculate sterimol values for substituents without end"
             )
 
-        from AaronTools.finders import BondedTo
-
         atom1 = self.find(BondedTo(self.end))[0]
         atom2 = self.end
 
+        if old_L:
+            from AaronTools.atoms import Atom, BondOrder
+            bo = BondOrder
+            key = bo.key(atom1, Atom(element="H"))
+            dx = bo.bonds[key]["1.0"] + 0.4
+
         # print(atom1.name, atom2.name)
 
         L_axis = atom2.bond(atom1)
         L_axis /= np.linalg.norm(L_axis)
 
         if isinstance(radii, dict):
             radii_dict = radii
         elif radii.lower() == "bondi":
             radii_dict = BONDI_RADII
         elif radii.lower() == "umn":
             radii_dict = VDW_RADII
 
-        param_value = None
-        vector = None
-
-        for atom in self.atoms:
-            # if len(self.atoms) > 1 and atom is atom1:
-            #    continue
+        B1 = None
+        B2 = None
+        B3 = None
+        B4 = None
+        B5 = None
+        L = None
+        vector = {"B1": None, "B2": None, "B3": None, "B4": None, "B5": None, "L": None}
+        # for B1, we're going to use ConvexHull to find the minimum distance
+        # from one face of a bounding box
+        # to do this, we're going to project the substituent in a plane
+        # perpendicular to the L-axis and get a set of points along the
+        # vdw radii of the atoms
+        # ConvexHull will take these points and figure out which ones
+        # are on the outside (vertices)
+        # we then just need to find the bounding box with the minimum distance
+        # from L-axis to one side of the box
+        points = []
+        ndx = []
+        # just grab a random vector perpendicular to the L-axis
+        # it doesn't matter really
+        ip_vector = perp_vector(L_axis)
+        x_vec = np.cross(ip_vector, L_axis)
+        x_vec /= np.linalg.norm(x_vec)
+        basis = np.array([x_vec, ip_vector, L_axis]).T
 
+        for i, atom in enumerate(self.atoms):
             test_v = atom2.bond(atom)
 
-            if parameter == "L":
+            # L
+            if old_L:
                 test_L = (
                     np.dot(test_v, L_axis)
                     - atom1.dist(atom2)
-                    + VDW_RADII[atom1.element]
-                    + VDW_RADII[atom.element]
+                    + dx
+                    + radii_dict[atom.element]
                 )
-                if param_value is None or test_L > param_value:
-                    param_value = test_L
-                    start = atom1.coords - VDW_RADII[atom1.element] * L_axis
-                    vector = (start, start + param_value * L_axis)
-
-            elif parameter == "B1":
-                # if len(self.atoms) > 1 and atom is atom1:
-                #    continue
-
-                r1 = radii_dict[atom.element]
-                b = np.dot(test_v, L_axis)
-                test_B1_v = test_v - (b * L_axis)
-                test_B1 = np.linalg.norm(test_B1_v) + r1
-                obstructed = False
-                if param_value is None or test_B1 < param_value:
-                    # check to see if this atom"s B1 is obstructed by another atom
-                    if np.linalg.norm(test_B1_v) > 1e-4:
-                        perp_vec = test_B1_v / np.linalg.norm(test_B1_v)
-
-                        for a2 in self.atoms:
-                            r2 = radii_dict[a2.element]
-                            if atom is a2:
-                                continue
-
-                            test_u = atom2.bond(a2)
-                            u = np.dot(test_u, L_axis)
-                            u_v = test_u - (u * L_axis)
-                            d = np.linalg.norm(u_v - test_B1_v)
-                            if r2 - d > r1:
-                                # atom is completely in the shadow of a2
-                                obstructed = True
-                                # print(atom.name, "completely obstructed by", a2.name)
-                                break
-
-                            elif np.linalg.norm(u_v) + r2 - test_B1 < 1e-3:
-                                # a2 is closer to the L axis than atom
-                                # print(atom.name, "farther than", a2.name)
-                                continue
-
-                            # elif np.linalg.norm(u_v) < 3*np.finfo(float).eps:
-                            #    #this atom is close to the L axis
-                            #    #if it is the "B1 atom", we"ll find out when we check it
-                            #    #but we don"t need to check against it
-                            #    continue
-
-                            else:
-                                # if the atom is far enough from the L axis, check
-                                # if the B1 is blocked by another atom
-                                # - see if the vector perpendicular to the L axis that
-                                #   points towards the atom is between the vectors from
-                                #   the L axis tangent to the VDW shadow of another atom
-                                #   if it is between the tangent vectors, then this atom
-                                #   is obstructed and does not define the minimum width
-                                p_v = (
-                                    test_B1 * perp_vec / np.linalg.norm(test_B1)
-                                )
-                                u_n = u_v / np.linalg.norm(u_v)
-                                r_v = r2 * np.cross(u_n, L_axis)
-                                tan1 = u_v + r_v
-                                tan2 = u_v - r_v
-
-                                a1p = np.linalg.norm(p_v)
-                                b1p = np.linalg.norm(tan1)
-                                c1p = np.linalg.norm(p_v - tan1)
-
-                                a2p = np.linalg.norm(p_v)
-                                b2p = np.linalg.norm(tan2)
-                                c2p = np.linalg.norm(p_v - tan2)
-
-                                a12 = np.linalg.norm(tan1)
-                                b12 = np.linalg.norm(tan2)
-                                c12 = np.linalg.norm(tan2 - tan1)
-
-                                t1p = np.arccos(
-                                    (c1p ** 2 - a1p ** 2 - b1p ** 2) / (-2 * a1p * b1p)
-                                )
-                                t2p = np.arccos(
-                                    (c2p ** 2 - a2p ** 2 - b2p ** 2) / (-2 * a2p * b2p)
-                                )
-                                t12 = np.arccos(
-                                    (c12 ** 2 - a12 ** 2 - b12 ** 2) / (-2 * a12 * b12)
-                                )
-
-                                if abs(t1p + t2p - t12) < 1e-3:
-                                    # print(atom.name, "partially obstructed by", a2.name)
-                                    obstructed = True
-                                    break
-                                # else:
-                                # print(atom.name, "unobstructed by", a2.name)
-                                # print(t1p, t2p, t12, tan1, tan2, test_B1*perp_vec)
-
-                    # if the atom is close to the L axis, scan angles and check the same
-                    # thing as above
-                    else:
-                        v_n = test_v / np.linalg.norm(test_v)
-                        perp_vec = v_n[::-1]
-                        perp_vec -= np.dot(v_n, perp_vec) * v_n
-                        start_angle = None
-                        end_angle = None
-
-                        # go two full circles
-                        for angle in np.linspace(0, 4 * np.pi, num=720):
-                            partially_obstructed = False
-                            m = rotation_matrix(angle, L_axis)
-                            p_v = np.dot(m, perp_vec)
-                            p_v /= np.linalg.norm(p_v)
-                            p_v = test_B1 * p_v
-                            for a2 in self.atoms:
-                                r2 = radii_dict[a2.element]
-                                if atom is a2:
-                                    continue
-
-                                test_u = atom2.bond(a2)
-                                u = np.dot(test_u, L_axis)
-                                u_v = test_u - (u * L_axis)
-                                d = np.linalg.norm(u_v - test_B1_v)
-                                if r2 - d > r1:
-                                    # atom is completely in the shadow of a2
-                                    obstructed = True
-                                    # print(atom.name, "completely obstructed by", a2.name)
-                                    break
-
-                                elif np.linalg.norm(u_v) + r2 - test_B1 < 1e-2:
-                                    # a2 is closer to the L axis than atom
-                                    # print(
-                                    #     atom.name,
-                                    #     "farther than",
-                                    #     a2.name,
-                                    #     "at angle",
-                                    #     angle
-                                    #)
-                                    continue
-
-                                u_n = u_v / np.linalg.norm(u_v)
-                                r_v = r2 * np.cross(u_n, L_axis)
-                                tan1 = u_v + r_v
-                                tan2 = u_v - r_v
-
-                                a1p = np.linalg.norm(p_v)
-                                b1p = np.linalg.norm(tan1)
-                                c1p = np.linalg.norm(p_v - tan1)
-
-                                a2p = np.linalg.norm(p_v)
-                                b2p = np.linalg.norm(tan2)
-                                c2p = np.linalg.norm(p_v - tan2)
-
-                                a12 = np.linalg.norm(tan1)
-                                b12 = np.linalg.norm(tan2)
-                                c12 = np.linalg.norm(tan2 - tan1)
-
-                                t1p = np.arccos(
-                                    (c1p ** 2 - a1p ** 2 - b1p ** 2) / (-2 * a1p * b1p)
-                                )
-                                t2p = np.arccos(
-                                    (c2p ** 2 - a2p ** 2 - b2p ** 2) / (-2 * a2p * b2p)
-                                )
-                                t12 = np.arccos(
-                                    (c12 ** 2 - a12 ** 2 - b12 ** 2) / (-2 * a12 * b12)
-                                )
-
-                                # print(t1p, t2p, t12, t1p + t2p)
-
-                                if abs(t1p + t2p - t12) < 1e-3:
-                                    partially_obstructed = True
-                                    # print(
-                                    #     atom.name,
-                                    #     "obstructed by",
-                                    #     a2.name,
-                                    #     "at angle",
-                                    #     angle
-                                    # )
-                                    # we might have found and opening, but if it"s too small,
-                                    # it"s not really a usable opening
-                                    # must have an arc length > 1 A
-                                    if (
-                                            start_angle is not None
-                                            and end_angle is None
-                                    ):
-                                        if (angle - start_angle) * r1 < 0.9:
-                                            # print(
-                                            #     "< 1 A gap between",
-                                            #     start_angle,
-                                            #     angle,
-                                            #     (angle-start_angle) * r1
-                                            # )
-                                            start_angle = None
-                                        else:
-                                            end_angle = angle
-                                    break
-
-                            else:
-                                if (
-                                        not partially_obstructed
-                                        and start_angle is None
-                                ):
-                                    # print(atom.name, "not obstructed at angle", angle)
-                                    start_angle = angle
-                                elif end_angle is not None:
-                                    break
-
-                            if obstructed:
-                                break
-
-                        # print(atom.name, "finished scanning", start_angle, end_angle, angle)
-                        if start_angle is None or (
-                                start_angle != 0 and end_angle is None
-                        ):
-                            obstructed = True
-                        else:
-                            if end_angle is None:
-                                end_angle = start_angle + np.pi
-                            m = rotation_matrix(
-                                0.5 * (start_angle + end_angle), L_axis
-                            )
-                            perp_vec = np.dot(m, perp_vec)
-
-                    if not obstructed:
-                        # print("new B1 atom", atom.name)
-                        start = atom.coords - test_B1_v
-                        end = start + test_B1 * (
-                            perp_vec / np.linalg.norm(perp_vec)
-                        )
-                        vector = (start, end)
-                        param_value = test_B1
-
-            elif parameter == "B5":
-                b = np.dot(test_v, L_axis)
-                test_B5_v = test_v - (b * L_axis)
-                test_B5 = np.linalg.norm(test_B5_v) + radii_dict[atom.element]
-                if param_value is None or test_B5 > param_value:
-                    param_value = test_B5
-                    start = atom.coords - test_B5_v
-                    if np.linalg.norm(test_B5_v) > 3 * np.finfo(float).eps:
-                        perp_vec = test_B5_v
-                    else:
-                        v_n = test_v / np.linalg.norm(test_v)
-                        perp_vec = v_n[::-1]
-                        perp_vec -= np.dot(v_n, perp_vec) * v_n
+            else:
+                # overlap with L-axis and vector from 1st substituent
+                # atom to this atom plus the difference between the sum of
+                # the vdw radii and bond length of the 1st substituent atom
+                # and the molecule's atom
+                # the distance from atom2 is subtracted off b/c our L
+                # goes from one end of the VDW radii to the other
+                # distance from atom2 is included in test_v, so we need
+                # to subtract it off
+                test_L = (
+                    np.dot(test_v, L_axis)
+                    - atom1.dist(atom2)
+                    + radii_dict[atom1.element]
+                    + radii_dict[atom.element]
+                )
+            if L is None or test_L > L:
+                L = test_L
+                if old_L:
+                    start = atom1.coords - dx * L_axis
+                    vector["L"] = (start, start + L * L_axis)
+                else:
+                    start = atom1.coords - radii_dict[atom1.element] * L_axis
+                    vector["L"] = (start, start + L * L_axis)
 
-                    end = start + test_B5 * (
-                        perp_vec / np.linalg.norm(perp_vec)
-                    )
+            # B1-4 stuff - we come back to this later
+            r1 = radii_dict[atom.element]
+
+            new_coords = np.dot(test_v, basis)
+            # in plane coordinates - z-axis is L-axis, which
+            # we don't care about for B1
+            ip_coords = new_coords[0:2]
+            for x in np.linspace(0, 2 * np.pi, num=250):
+                ndx.append(i)
+                v = ip_coords + r1 * np.array([np.cos(x), np.sin(x)])
+                points.append(v)
+
+            # B5
+            # find distance along L-axis, then subtract this from vector from
+            # vector from molecule to this atom to get the B5 vector
+            # add the atom's radius to get the full B5
+            b = np.dot(test_v, L_axis)
+            test_B5_v = test_v - (b * L_axis)
+            test_B5 = np.linalg.norm(test_B5_v) + radii_dict[atom.element]
+            if B5 is None or test_B5 > B5:
+                B5 = test_B5
+                start = atom.coords - test_B5_v
+                if np.linalg.norm(test_B5_v) > 3 * np.finfo(float).eps:
+                    perp_vec = test_B5_v
+                else:
+                    # this atom might be along the L-axis, in which case use
+                    # any vector orthogonal to L-axis
+                    v_n = test_v / np.linalg.norm(test_v)
+                    perp_vec = perp_vector(L_axis)
+                    perp_vec -= np.dot(v_n, perp_vec) * v_n
+
+                end = start + test_B5 * (
+                    perp_vec / np.linalg.norm(perp_vec)
+                )
+
+                vector["B5"] = (start, end)
+
+        points = np.array(points)
+
+        hull = ConvexHull(points)
+
+        # import matplotlib.pyplot as plt
+        # plt.plot(points[:, 0], points[:, 1], 'o')
+        # plt.plot(0, 0, 'kx')
+        # plt.plot(points[hull.vertices,0], points[hull.vertices,1], 'ro')
+
+        # ax = plt.gca()
+        # ax.set_aspect('equal')
+
+        # go through each edge, find a vector perpendicular to the one
+        # defined by the edge that passes through the origin
+        # the length of the shortest of these vectors is B1
+        for i in range(0, len(hull.vertices) - 1):
+            # the vertices of the hull are organized in a counterclockwise
+            # direction, so neighboring indices define an edge
+            v_ndx_0, v_ndx_1 = hull.vertices[i:i + 2]
+            # find 'tangent' of the edge
+            v = points[v_ndx_1] - points[v_ndx_0]
+            v /= np.linalg.norm(v)
+            # find normal to this edge by projecting a vector from the
+            # L axis to one of the points on the edge
+            b = points[v_ndx_0]
+            t = np.dot(b, v)
+            perp = b - t * v
+            # plt.plot(perp[0], perp[1], 'g*')
+            test_b1 = np.linalg.norm(perp)
+            if B1 is None or test_b1 < B1:
+                B1 = test_b1
+                # figure out vector from L axis to represent B1
+                b1_atom = self.atoms[ndx[v_ndx_0]]
+                test_v = atom2.bond(b1_atom)
+                test_B1_v = test_v - (np.dot(test_v, L_axis) * L_axis)
+                start = b1_atom.coords - test_B1_v
+                end = x_vec * perp[0] + ip_vector * perp[1]
+                end += start
+                vector["B1"] = (start, end)
+
+        # figure out B2-4
+        # these need to be sorted in increasing order
+        # for now, they will just be Bpar for the one opposite B1
+        # and Bperp1 and Bperp2 for the ones perpendicular to B1
+        b1_norm = end - start
+        b1_norm /= np.linalg.norm(b1_norm)
+        b1_perp = np.cross(L_axis, b1_norm)
+        b1_perp /= np.linalg.norm(b1_perp)
+        Bpar = None
+        Bperp1 = None
+        Bperp2 = None
+        for atom in self.atoms:
+            test_v = atom2.bond(atom)
+            b = np.dot(test_v, L_axis)
+            test_B_v = test_v - (b * L_axis)
+            test_par_vec = np.dot(test_B_v, b1_norm) * b1_norm
+            test_par_vec -= radii_dict[atom.element] * b1_norm
+            start = atom.coords - test_B_v
+            end = start + test_par_vec
+
+            test_Bpar = np.linalg.norm(end - start)
+            if Bpar is None or test_Bpar > Bpar:
+                Bpar = test_Bpar
+                par_vec = (start, end)
+
+            perp_vec = np.dot(test_B_v, b1_perp) * b1_perp
+            if np.dot(test_B_v, b1_perp) > 0 or np.isclose(np.dot(b1_perp, test_B_v), 0):
+                test_perp_vec1 = perp_vec + radii_dict[atom.element] * b1_perp
+                end = start + test_perp_vec1
+                test_Bperp1 = np.linalg.norm(end - start)
+                if Bperp1 is None or test_Bperp1 > Bperp1:
+                    Bperp1 = test_Bperp1
+                    perp_vec1 = (start, end)
+            if np.dot(test_B_v, b1_perp) < 0 or np.isclose(np.dot(b1_perp, test_B_v), 0):
+                test_perp_vec2 = perp_vec - radii_dict[atom.element] * b1_perp
+                end = start + test_perp_vec2
+                test_Bperp2 = np.linalg.norm(end - start)
+                if Bperp2 is None or test_Bperp2 > Bperp2:
+                    Bperp2 = test_Bperp2
+                    perp_vec2 = (start, end)
+
+        # put B2-4 in order
+        i = 0
+        Bs = [Bpar, Bperp1, Bperp2]
+        Bvecs = [par_vec, perp_vec1, perp_vec2]
+        while Bs:
+            max_b = max(Bs)
+            n = Bs.index(max_b)
+            max_v = Bvecs.pop(n)
+            Bs.pop(n)
+
+            if i == 0:
+                B4 = max_b
+                vector["B4"] = max_v
+            elif i == 1:
+                B3 = max_b
+                vector["B3"] = max_v
+            elif i == 2:
+                B2 = max_b
+                vector["B2"] = max_v
+            i += 1
+
+        params = {
+            "B1": B1,
+            "B2": B2,
+            "B3": B3,
+            "B4": B4,
+            "B5": B5,
+            "L": L,
+        }
+
+        # plt.plot(points[min_ndx,0], points[min_ndx,1], 'g*')
 
-                    vector = (start, end)
+        # plt.show()
 
         if return_vector:
             return vector
-        return param_value
+        return params
 
     def align_to_bond(self, bond):
         """
         align substituent to a bond vector
         """
         bond /= np.linalg.norm(bond)
         x_axis = np.array([1.0, 0.0, 0.0])
         rot_axis = np.cross(x_axis, bond)
-        rot_axis /= np.linalg.norm(rot_axis)
+        if np.linalg.norm(rot_axis) > 1e-4:
+            rot_axis /= np.linalg.norm(rot_axis)
+        else:
+            rot_axis = np.array([0.0, 1.0, 0.0])
         angle = np.arccos(np.dot(bond, x_axis))
         self.rotate(rot_axis, angle)
 
     def sub_rotate(self, angle=None, reverse=False):
         """
         rotates substituent about bond w/ rest of geometry
         :angle: in radians
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AaronTools-1.0b8/test/__init__.py` & `AaronTools-1.0b9/test/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -94,69 +94,82 @@
         rmsd[1].write("test")
         rmsd = rmsd[2]
 
     return rmsd < thresh
 
 
 class TestWithTimer(unittest.TestCase):
-    count = 0
+    test_count = 0
     total_time = 0
+    this_class = None
     last_class = None
     last_result = None
-    _errors = 0
-    _fails = 0
+    errors = 0
+    fails = 0
+    last_errors = 0
+    last_fails = 0
+
+    @classmethod
+    def setUpClass(cls):
+        TestWithTimer.total_time = time.time()
 
     @classmethod
     def tearDownClass(cls):
-        errors = len(cls.last_result.errors)
-        fails = len(cls.last_result.failures)
-        if TestWithTimer._errors != errors:
-            TestWithTimer._errors = errors
-            print("\b ERROR")
-        elif TestWithTimer._fails != fails:
-            TestWithTimer._fails = fails
-            print("\b FAIL")
+        TestWithTimer.total_time = time.time() - TestWithTimer.total_time
+        print(TestWithTimer.get_status())
+
+        if TestWithTimer.errors - TestWithTimer.last_errors:
+            status = "ERROR"
+        elif TestWithTimer.fails - TestWithTimer.last_fails:
+            status = "FAIL"
         else:
-            print("\b ok")
+            status = "ok"
+        TestWithTimer.last_errors = TestWithTimer.errors
+        TestWithTimer.last_fails = TestWithTimer.fails
 
         print(
-            "Ran {} tests in {:.3f}s".format(
-                TestWithTimer.count, TestWithTimer.total_time
+            "Ran %d test in %.4fs  %s"
+            % (
+                TestWithTimer.last_result.testsRun - TestWithTimer.test_count,
+                TestWithTimer.total_time,
+                status,
             )
         )
-        print("-" * 70)
+        TestWithTimer.test_count = TestWithTimer.last_result.testsRun
+        print(unittest.TextTestResult.separator2)
+
+    @classmethod
+    def get_status(cls):
+        if TestWithTimer.errors != len(TestWithTimer.last_result.errors):
+            status = "ERROR"
+        elif TestWithTimer.fails != len(TestWithTimer.last_result.failures):
+            status = "FAIL"
+        else:
+            status = "ok"
+        TestWithTimer.errors = len(TestWithTimer.last_result.errors)
+        TestWithTimer.fails = len(TestWithTimer.last_result.failures)
+        return status
 
     def setUp(self):
-        errors = len(self._outcome.result.errors)
-        fails = len(self._outcome.result.failures)
-        if TestWithTimer._errors != errors:
-            TestWithTimer._errors = errors
-            print("\b ERROR")
-        elif TestWithTimer._fails != fails:
-            TestWithTimer._fails = fails
-            print("\b FAIL")
-        elif self.id().split(".")[1] == TestWithTimer.last_class:
-            print("\b ok")
-        elif TestWithTimer.last_class is not None:
-            TestWithTimer.total_time = 0
         self.start_time = time.time()
 
     def tearDown(self):
         t = time.time() - self.start_time
-        TestWithTimer.total_time += t
+        TestWithTimer.last_result = self._outcome.result
+        TestWithTimer.this_class, self.test_name = self.id().split(".")[-2:]
 
-        name = self.id().split(".")[-2:]
-        if not TestWithTimer.last_class or TestWithTimer.last_class != name[0]:
-            TestWithTimer.last_class = name[0]
-            TestWithTimer.count = 0
-            print("\r{}:".format(name[0]))
+        status = TestWithTimer.get_status()
+        if TestWithTimer.this_class != TestWithTimer.last_class:
+            TestWithTimer.last_class = TestWithTimer.this_class
+            print(TestWithTimer.this_class)
+        else:
+            print(status)
 
-        name = name[1]
-        TestWithTimer.count += 1
         print(
-            "\r    {:3.0f}: {:<30s} {: 3.3f}s  ".format(
-                TestWithTimer.count, name, t
+            "\b   %2d. %-30s %.4fs  "
+            % (
+                TestWithTimer.last_result.testsRun - TestWithTimer.test_count,
+                self.test_name,
+                t,
             ),
             end="",
         )
-
-        TestWithTimer.last_result = self._outcome.result
```

### Comparing `AaronTools-1.0b8/test/ref_files/atom.json` & `AaronTools-1.0b9/test/ref_files/atom.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/benzene_dimer_ref.xyz` & `AaronTools-1.0b9/test/ref_files/benzene_dimer_ref.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/cat.json` & `AaronTools-1.0b9/test/ref_files/cat.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/change_chirality_cls/diastereomer-1.xyz` & `AaronTools-1.0b9/test/ref_files/change_chirality_cls/diastereomer-1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/change_chirality_cls/diastereomer-2.xyz` & `AaronTools-1.0b9/test/ref_files/change_chirality_cls/diastereomer-2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/change_chirality_cls/diastereomer-3.xyz` & `AaronTools-1.0b9/test/ref_files/change_chirality_cls/diastereomer-3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/change_chirality_cls/diastereomer-4.xyz` & `AaronTools-1.0b9/test/ref_files/change_chirality_cls/diastereomer-4.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/chlorotoluene_180.xyz` & `AaronTools-1.0b9/test/ref_files/chlorotoluene_180.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/config_HOH_init.json` & `AaronTools-1.0b9/test/ref_files/config_HOH_init.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/config_blank_init.json` & `AaronTools-1.0b9/test/ref_files/config_blank_init.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/detect_components.json` & `AaronTools-1.0b9/test/ref_files/detect_components.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/file_io_died.xyz` & `AaronTools-1.0b9/test/ref_files/file_io_died.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/file_io_error.xyz` & `AaronTools-1.0b9/test/ref_files/file_io_error.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/file_io_normal.xyz` & `AaronTools-1.0b9/test/ref_files/file_io_normal.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/freq.json` & `AaronTools-1.0b9/test/ref_files/freq.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/geometry.json` & `AaronTools-1.0b9/test/ref_files/geometry.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/lig.json` & `AaronTools-1.0b9/test/ref_files/lig.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/lig_map_1.xyz` & `AaronTools-1.0b9/test/ref_files/lig_map_1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/lig_map_2.xyz` & `AaronTools-1.0b9/test/ref_files/lig_map_2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/lig_map_3.xyz` & `AaronTools-1.0b9/test/ref_files/lig_map_3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/lig_map_4.xyz` & `AaronTools-1.0b9/test/ref_files/lig_map_4.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/lig_map_5.xyz` & `AaronTools-1.0b9/test/ref_files/lig_map_5.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/lig_map_6.xyz` & `AaronTools-1.0b9/test/ref_files/lig_map_6.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/lig_map_7.xyz` & `AaronTools-1.0b9/test/ref_files/lig_map_7.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/log.json` & `AaronTools-1.0b9/test/ref_files/log.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_1.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_2.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-1.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-2.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-3.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-4.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-4.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-5.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-5.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-6.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-6.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-7.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-7.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/make_conf_cls/conformer-8.xyz` & `AaronTools-1.0b9/test/ref_files/make_conf_cls/conformer-8.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/minimize_torsion.xyz` & `AaronTools-1.0b9/test/ref_files/minimize_torsion.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/naphthalene.xyz` & `AaronTools-1.0b9/test/ref_files/naphthalene.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/pyrene.xyz` & `AaronTools-1.0b9/test/ref_files/pyrene.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/sub.json` & `AaronTools-1.0b9/test/ref_files/sub.json`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/sub_rotate.xyz` & `AaronTools-1.0b9/test/ref_files/sub_rotate.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/tetrahydronaphthalene.xyz` & `AaronTools-1.0b9/test/ref_files/tetrahydronaphthalene.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/ref_files/torsion_interpolation.xyz` & `AaronTools-1.0b9/test/ref_files/torsion_interpolation.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_atoms.py` & `AaronTools-1.0b9/test/test_atoms.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,29 +137,29 @@
         self.assertTrue(atoms[12] < atoms[10])
         # atom[3] has 3 connected atoms: C, C, Cl
         # atom[2] has 3 connected atoms: C, C, H
         self.assertTrue(atoms[3] < atoms[2])
 
     def test_repr(self):
         atom = Atom("H", [0, 0, 0], True, "1", ["test"])
-        s = str(atom)
+        s = repr(atom)
         self.assertEqual(
             s, "  H     0.00000000    0.00000000    0.00000000  -1    1"
         )
 
     def test_set_radii(self):
         atom = Atom("H", [0, 0, 0])
         self.assertEqual(atom._radii, 0.32)
         atom = Atom("X", [0, 0, 0])  # ghost atom
         self.assertEqual(atom._radii, 0.0)
         with self.assertRaises(ValueError):
             atom = Atom("NotAnElement", [0, 0, 0])
         atom = Atom()
         atom.element = "NotAnElement"
-        with self.assertWarns(UserWarning):
+        with self.assertLogs(logger=Atom.LOG, level="WARNING"):
             atom._set_radii()
 
     def test_set_connectivity(self):
         atom = Atom("H", [0, 0, 0])
         self.assertEqual(atom._connectivity, 1)
         atom = Atom("C", [0, 0, 0])
         self.assertEqual(atom._connectivity, 4)
```

### Comparing `AaronTools-1.0b8/test/test_cls.py` & `AaronTools-1.0b9/test/test_cls.py`

 * *Files 0% similar despite different names*

```diff
@@ -837,16 +837,16 @@
 
         proc = Popen(args, stdout=PIPE, stderr=PIPE)
         out, err = proc.communicate()
 
         if len(err) != 0:
             raise RuntimeError(err)
 
-        ref = """B1      B5      L       file
-        1.70    3.36    6.68    test_files/benzene.xyz
+        ref = """B1      B2      B3      B4      B5      L       file
+        1.70    1.70    3.36    3.36    3.36    6.78    test_files/benzene.xyz
 
         """
 
         ref_lines = ref.splitlines()
         ref_status_line = ref_lines[1]
 
         lines = out.decode("utf-8").splitlines()
```

### Comparing `AaronTools-1.0b8/test/test_comp_output.py` & `AaronTools-1.0b9/test/test_comp_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,13 +81,14 @@
             for j in range(3):
                 if r[j] is None:
                     self.assertTrue(test[i][j] is None)
                 else:
                     self.assertTrue(test[i][j] == r[j])
 
     def test_crest(self):
-        test = CompOutput(os.path.join(prefix, "test_files", "good.crest"))
-        print(test.__dict__)
+        test = CompOutput(
+            os.path.join(prefix, "test_files", "good.crest"), conf_name=False
+        )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `AaronTools-1.0b8/test/test_component.py` & `AaronTools-1.0b9/test/test_component.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_config.py` & `AaronTools-1.0b9/test/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 #!/usr/bin/env python3
 import json
 import os
 import unittest
 
-import AaronTools
-import AaronTools.config
 import numpy as np
+from AaronTools import addlogger
 from AaronTools.config import Config
-from AaronTools.test import TestWithTimer, prefix, rmsd_tol, validate
+from AaronTools.test import TestWithTimer, prefix
 
 
+@addlogger
 class TestConfig(TestWithTimer):
+    LOG = None
+    USER_SPECIFIC = ["metadata", "infile", (".*", ".*_dir")]
     config_list = [("blank.ini", None), ("HOH.ini", None)]
 
     def test_init(self):
         for i, (config_name, config) in enumerate(TestConfig.config_list):
             config = Config(
                 os.path.join(prefix, "test_files", config_name),
                 quiet=True,
                 skip_user_default=True,
             )
             TestConfig.config_list[i] = config_name, config
 
-            test = config.as_dict(skip=config.USER_SPECIFIC)
+            test = config.as_dict(skip=self.USER_SPECIFIC)
             ref_name = os.path.join(
                 prefix, "ref_files", config_name.replace(".ini", "_init.json")
             )
             # with open(ref_name, "w") as f:
             #     json.dump(test, f, indent=2)
 
             # need this to make sure python->json stuff is consistent,
             # eg: json doesn't distinguish between tuples and lists
             test = json.loads(json.dumps(test))
-            # print(json.dumps(test, indent=2))
+            self.LOG.debug(json.dumps(test, indent=2))
             with open(ref_name, "r") as f:
                 ref = json.load(f)
+            self.maxDiff = None
             self.assertDictEqual(ref, test, msg=config_name)
 
     def test_parse_changes(self):
         ###
         # substitutions with single point of connections
         ###
         simple = Config(
```

### Comparing `AaronTools-1.0b8/test/test_fetch.py` & `AaronTools-1.0b9/test/test_fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,22 @@
         ref.refresh_connected()
         sub.refresh_connected()
         ref.refresh_ranks()
         ref.refresh_ranks()
         ref.atoms = ref.reorder(start=ref.atoms[0])[0]
         sub.atoms = sub.reorder(start=sub.atoms[0])[0]
         self.assertTrue(
-            validate(sub, ref, thresh=thresh, heavy_only=True, sort=False, debug=False)
+            validate(
+                sub,
+                ref,
+                thresh=thresh,
+                heavy_only=True,
+                sort=False,
+                debug=False,
+            )
         )
 
     def is_NO2(self, sub):
         ref = TestFromString.NO2
         self.assertTrue(validate(sub, ref, thresh=2e-1))
 
     def test_substituent(self):
@@ -46,35 +53,37 @@
             import rdkit
 
             sub = Substituent.from_string(
                 "acetyl", form="iupac", strict_use_rdkit=True
             )
             self.is_COCH3(sub)
 
-            sub = Substituent.from_string(
-                "nitro", form="iupac", strict_use_rdkit=True
-            )
-            self.is_NO2(sub)
+            with self.assertLogs(Substituent.LOG, level="WARNING"):
+                sub = Substituent.from_string(
+                    "nitro", form="iupac", strict_use_rdkit=True
+                )
+                self.is_NO2(sub)
 
             sub = Substituent.from_string(
                 "O=[N.]=O", form="smiles", strict_use_rdkit=True
             )
             self.is_NO2(sub)
 
             sub = Substituent.from_string(
                 "O=[N]=O", form="smiles", strict_use_rdkit=True
             )
             self.is_NO2(sub)
 
         except (ImportError, ModuleNotFoundError):
             # I still want to test CACTVS things because sometimes they change stuff
             # that breaks our stuff
-            if any(user == os.getenv("USER", os.getenv("USERNAME", False)) for user in [
-                "ajs99778", "normn"
-            ]):
+            if any(
+                user == os.getenv("USER", os.getenv("USERNAME", False))
+                for user in ["ajs99778", "normn"]
+            ):
                 sub = Substituent.from_string("acetyl", form="iupac")
                 print(sub.write(outfile=False))
                 self.is_COCH3(sub, thresh=0.3)
 
                 sub = Substituent.from_string("nitro", form="iupac")
                 print(sub.write(outfile=False))
                 self.is_NO2(sub)
@@ -95,56 +104,55 @@
             import rdkit
 
             geom = Geometry.from_string(
                 "(1R,2R)-1-Chloro-2-methylcyclohexane", form="iupac"
             )
             ref = TestFromString.chiral_geom
             # really loose threshhold b/c rdkit can give a boat cyclohexane...
-            self.assertTrue(
-                validate(geom, ref, thresh=0.35, heavy_only=True, debug=False)
-            )
+            self.assertTrue(validate(geom, ref, thresh=0.35, heavy_only=True))
 
-        except:
-            if any(user == os.getenv("USER", os.getenv("USERNAME", False)) for user in [
-                "ajs99778", "normn"
-            ]):
+        except (ImportError, ModuleNotFoundError):
+            if any(
+                user == os.getenv("USER", os.getenv("USERNAME", False))
+                for user in ["ajs99778", "normn"]
+            ):
                 geom = Geometry.from_string(
                     "(1R,2R)-1-Chloro-2-methylcyclohexane", form="iupac"
                 )
-                print(geom.write(outfile=False))
                 ref = TestFromString.chiral_geom
                 # really loose threshhold b/c rdkit can give a boat cyclohexane...
                 self.assertTrue(
-                    validate(
-                        geom, ref, thresh=0.35, heavy_only=True, debug=False
-                    )
+                    validate(geom, ref, thresh=0.35, heavy_only=True)
                 )
             else:
                 self.skipTest("RDKit not installed, CACTVS is not tested")
 
     def test_ring(self):
         try:
             import rdkit
 
             ring = Ring.from_string(
                 "benzene", end_length=1, end_atom="C", form="iupac"
             )
             ref = self.benzene
-            self.assertTrue(validate(ring, ref, thresh="loose", debug=True))
+            self.assertTrue(validate(ring, ref, thresh="loose"))
 
         except ImportError:
-            if any(user == os.getenv("USER", os.getenv("USERNAME", False)) for user in [
-                "ajs99778", "normn"
-            ]):
+            if any(
+                user == os.getenv("USER", os.getenv("USERNAME", False))
+                for user in ["ajs99778", "normn"]
+            ):
                 ring = Ring.from_string(
                     "benzene", end_length=1, end_atom="C", form="iupac"
                 )
                 print(ring.comment)
                 ref = self.benzene
-                self.assertTrue(validate(ring, ref, thresh="loose", debug=True))
+                self.assertTrue(
+                    validate(ring, ref, thresh="loose", debug=True)
+                )
 
             else:
                 self.skipTest("RDKit not installed, CACTVS is not tested")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `AaronTools-1.0b8/test/test_fileIO.py` & `AaronTools-1.0b9/test/test_fileIO.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         )
 
         for line1, line2 in zip(test.splitlines(), ref.splitlines()):
             self.assertEqual(line1.strip(), line2.strip())
 
     def test_read_crest(self):
         fname = os.path.join(prefix, "test_files/good.crest")
-        res = FileReader(fname)
+        res = FileReader(fname, conf_name=False)
         self.assertDictEqual(
             res.other,
             {
                 "best_energy": -79.18948,
                 "temperature": 298.15,
                 "energy": 0.172,
                 "entropy": 0.006899,
```

### Comparing `AaronTools-1.0b8/test/test_files/5a-sub1.R.ts1.Cf1.3.com` & `AaronTools-1.0b9/test/test_files/5a-sub1.R.ts1.Cf1.3.com`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/6a2e5am1hex.xyz` & `AaronTools-1.0b9/test/test_files/6a2e5am1hex.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/R-Quinox-tBu3.xyz` & `AaronTools-1.0b9/test/test_files/R-Quinox-tBu3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/benzene.xyz` & `AaronTools-1.0b9/test/test_files/benzene.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/benzene_1-NO2_4-Cl.can.xyz` & `AaronTools-1.0b9/test/test_files/benzene_1-NO2_4-Cl.can.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/benzene_1-NO2_4-Cl.xyz` & `AaronTools-1.0b9/test/test_files/benzene_1-NO2_4-Cl.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/benzene_1-OH_4-Cl.xyz` & `AaronTools-1.0b9/test/test_files/benzene_1-OH_4-Cl.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/benzene_1-Ph_4-Cl.xyz` & `AaronTools-1.0b9/test/test_files/benzene_1-Ph_4-Cl.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/benzene_dimer.xyz` & `AaronTools-1.0b9/test/test_files/benzene_dimer.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/bpy.xyz` & `AaronTools-1.0b9/test/test_files/bpy.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/catalysts/org_1.xyz` & `AaronTools-1.0b9/test/test_files/catalysts/org_1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/catalysts/org_tri.xyz` & `AaronTools-1.0b9/test/test_files/catalysts/org_tri.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/catalysts/tm_multi-lig.xyz` & `AaronTools-1.0b9/test/test_files/catalysts/tm_multi-lig.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/catalysts/tm_single-lig.xyz` & `AaronTools-1.0b9/test/test_files/catalysts/tm_single-lig.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/change_dihedral_0.xyz` & `AaronTools-1.0b9/test/test_files/change_dihedral_0.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/chiral_centers_1.xyz` & `AaronTools-1.0b9/test/test_files/chiral_centers_1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/chiral_centers_2.xyz` & `AaronTools-1.0b9/test/test_files/chiral_centers_2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/chiral_centers_3.xyz` & `AaronTools-1.0b9/test/test_files/chiral_centers_3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/chiral_centers_4.xyz` & `AaronTools-1.0b9/test/test_files/chiral_centers_4.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/chiral_ring.xyz` & `AaronTools-1.0b9/test/test_files/chiral_ring.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/chiral_ring_mirror.xyz` & `AaronTools-1.0b9/test/test_files/chiral_ring_mirror.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/chlorotoluene.xyz` & `AaronTools-1.0b9/test/test_files/chlorotoluene.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/died.log` & `AaronTools-1.0b9/test/test_files/died.log`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/dppe.xyz` & `AaronTools-1.0b9/test/test_files/dppe.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/error.log` & `AaronTools-1.0b9/test/test_files/error.log`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/freq.log` & `AaronTools-1.0b9/test/test_files/freq.log`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/good.crest` & `AaronTools-1.0b9/test/test_files/good.crest`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/lig_1.xyz` & `AaronTools-1.0b9/test/test_files/lig_1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/lig_2.xyz` & `AaronTools-1.0b9/test/test_files/lig_2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/ligands/R-Quinox-tBu3.xyz` & `AaronTools-1.0b9/test/test_files/ligands/R-Quinox-tBu3.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/ligands/S-tBu-BOX.xyz` & `AaronTools-1.0b9/test/test_files/ligands/S-tBu-BOX.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/ligands/squaramide.xyz` & `AaronTools-1.0b9/test/test_files/ligands/squaramide.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/normal.log` & `AaronTools-1.0b9/test/test_files/normal.log`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/opt_constraint.log` & `AaronTools-1.0b9/test/test_files/opt_constraint.log`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/opt_normal.log` & `AaronTools-1.0b9/test/test_files/opt_normal.log`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/opt_running.log` & `AaronTools-1.0b9/test/test_files/opt_running.log`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/orca_geom.out` & `AaronTools-1.0b9/test/test_files/orca_geom.out`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/pentane.xyz` & `AaronTools-1.0b9/test/test_files/pentane.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/psi4-test.out` & `AaronTools-1.0b9/test/test_files/psi4-test.out`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/step3.log` & `AaronTools-1.0b9/test/test_files/step3.log`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/test-route-2.com` & `AaronTools-1.0b9/test/test_files/test-route-2.com`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/test-route.com` & `AaronTools-1.0b9/test/test_files/test-route.com`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/test_rmsd_sort1.xyz` & `AaronTools-1.0b9/test/test_files/test_rmsd_sort1.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/test_rmsd_sort2.xyz` & `AaronTools-1.0b9/test/test_files/test_rmsd_sort2.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/torsion-60.xyz` & `AaronTools-1.0b9/test/test_files/torsion-60.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_files/torsion-90.xyz` & `AaronTools-1.0b9/test/test_files/torsion-90.xyz`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_finders.py` & `AaronTools-1.0b9/test/test_finders.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_geometry.py` & `AaronTools-1.0b9/test/test_geometry.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 import unittest
 from copy import copy
 
 import AaronTools
 import numpy as np
 from AaronTools.atoms import Atom
+from AaronTools.component import Component
 from AaronTools.fileIO import FileReader
 from AaronTools.geometry import Geometry
-from AaronTools.component import Component
 from AaronTools.ring import Ring
 from AaronTools.substituent import Substituent
 from AaronTools.test import TestWithTimer, prefix, rmsd_tol, validate
 
 
 def is_close(a, b, tol=10 ** -8, debug=False):
     n = None
```

### Comparing `AaronTools-1.0b8/test/test_json_extension.py` & `AaronTools-1.0b9/test/test_json_extension.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_pathway.py` & `AaronTools-1.0b9/test/test_pathway.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_substituent.py` & `AaronTools-1.0b9/test/test_substituent.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/test/test_utils.py` & `AaronTools-1.0b9/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/theory/__init__.py` & `AaronTools-1.0b9/theory/__init__.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/theory/basis.py` & `AaronTools-1.0b9/theory/basis.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 """
 used for specifying basis information for a Theory()
 """
 
 import os
-
 from warnings import warn
 
+from AaronTools.const import ELEMENTS
+from AaronTools.finders import (
+    AnyNonTransitionMetal,
+    AnyTransitionMetal,
+    NotAny,
+)
 from AaronTools.theory import (
-    ORCA_ROUTE,
-    ORCA_BLOCKS,
-    PSI4_BEFORE_GEOM,
-    GAUSSIAN_ROUTE,
     GAUSSIAN_GEN_BASIS,
     GAUSSIAN_GEN_ECP,
+    GAUSSIAN_ROUTE,
+    ORCA_BLOCKS,
+    ORCA_ROUTE,
+    PSI4_BEFORE_GEOM,
 )
-from AaronTools.finders import AnyTransitionMetal, AnyNonTransitionMetal, NotAny
-from AaronTools.const import ELEMENTS
 
 
 class Basis:
     """
     has attributes:
     name          - same as initialization keyword
     elements      - same as initialization keyword
     aux_type      - same as initialization keyword
     elements      - list of element symbols for elements this basis applies to
                     updated with Basis.refresh_elements
                     Basis.refresh_elements is called when writing an input file
     ele_selection - list of finders used to determine which elements this basis applies to
     not_anys      - list of finders used to determine which elements this basis does not apply to
     """
+
     default_elements = [AnyTransitionMetal(), AnyNonTransitionMetal()]
+
     def __init__(self, name, elements=None, aux_type=None, user_defined=False):
         """
         name         -   basis set base name (e.g. 6-31G)
         elements     -   list of element symbols or finders to determine the basis set applies to
                          elements may also be 'tm' or 'all' to indicate any transition metal and
                          all elements, respectively
                          elements may start with '!' to exclude that element from the basis
@@ -46,37 +51,37 @@
         self.name = name
 
         if elements is None:
             self.elements = []
             self.ele_selection = self.default_elements
             self.not_anys = []
         else:
-            #a list of elements or other identifiers was given
-            #if it's an element with a ! in front, add that element to not_anys
-            #otherwise, add the appropriate thing to ele_selection
-            if not hasattr(elements, '__iter__') or isinstance(elements, str):
+            # a list of elements or other identifiers was given
+            # if it's an element with a ! in front, add that element to not_anys
+            # otherwise, add the appropriate thing to ele_selection
+            if not hasattr(elements, "__iter__") or isinstance(elements, str):
                 elements = [elements]
 
             self.elements = elements
             ele_selection = []
             not_anys = []
             for ele in elements:
                 not_any = False
-                if isinstance(ele, str) and ele.startswith('!'):
-                    ele = ele.lstrip('!')
+                if isinstance(ele, str) and ele.startswith("!"):
+                    ele = ele.lstrip("!")
                     not_any = True
 
-                if ele.lower() == 'all':
+                if ele.lower() == "all":
                     if not_any:
                         not_anys.append(AnyTransitionMetal())
                         not_anys.append(AnyNonTransitionMetal())
                     else:
                         ele_selection.append(AnyTransitionMetal())
                         ele_selection.append(AnyNonTransitionMetal())
-                elif ele.lower() == 'tm' and ele != "Tm":
+                elif ele.lower() == "tm" and ele != "Tm":
                     if not_any:
                         ele_selection.append(AnyNonTransitionMetal())
                     else:
                         ele_selection.append(AnyTransitionMetal())
                 elif ele.lower() == "!tm" and ele != "!Tm":
                     if not_any:
                         ele_selection.append(AnyNonTransitionMetal())
@@ -86,16 +91,16 @@
                     if not_any:
                         not_anys.append(ele)
                     else:
                         ele_selection.append(ele)
                 else:
                     warn("element not known: %s" % repr(ele))
 
-            if not ele_selection and not not_anys:
-                #if only not_anys were given, fall back to the default elements
+            if not ele_selection and not_anys:
+                # if only not_anys were given, fall back to the default elements
                 ele_selection = self.default_elements
 
             self.ele_selection = ele_selection
             self.not_anys = not_anys
 
         self.aux_type = aux_type
         self.user_defined = user_defined
@@ -109,110 +114,252 @@
         elif self.name == other.name and self.elements and other.elements:
             return self.elements[0] < other.elements[0]
         return False
 
     def __eq__(self, other):
         if self.__class__ is not other.__class__:
             return False
-        
-        if self.get_gaussian(self.name).lower() != other.get_gaussian(other.name).lower():
+
+        if (
+            self.get_gaussian(self.name).lower()
+            != other.get_gaussian(other.name).lower()
+        ):
             return False
-        
+
         if self.aux_type != other.aux_type:
             return False
-        
+
         for obj, obj2 in zip([self, other], [other, self]):
             for finder in obj.ele_selection:
                 if isinstance(finder, str):
                     if finder not in obj2.ele_selection:
                         return False
                 else:
                     for finder2 in obj2.ele_selection:
                         if repr(finder) == repr(finder2):
                             break
                     else:
                         return False
-        
+
         return True
 
     def refresh_elements(self, geometry):
         """sets self's elements for the geometry"""
         atoms = geometry.find(self.ele_selection, NotAny(*self.not_anys))
         elements = set([atom.element for atom in atoms])
-        self.elements = elements
+        self.elements = sorted(elements)
+
+    @staticmethod
+    def sanity_check_basis(name, program):
+        import os.path
+        from difflib import SequenceMatcher as seqmatch
+        from re import IGNORECASE, match
+
+        from AaronTools.const import AARONTOOLS
+        from numpy import argsort, loadtxt
+
+        warning = None
+
+        if program.lower() == "gaussian":
+            valid = loadtxt(
+                os.path.join(
+                    AARONTOOLS, "theory", "valid_basis_sets", "gaussian.txt"
+                ),
+                dtype=str,
+            )
+        elif program.lower() == "orca":
+            valid = loadtxt(
+                os.path.join(
+                    AARONTOOLS, "theory", "valid_basis_sets", "orca.txt"
+                ),
+                dtype=str,
+            )
+        elif program.lower() == "psi4":
+            valid = loadtxt(
+                os.path.join(
+                    AARONTOOLS, "theory", "valid_basis_sets", "psi4.txt"
+                ),
+                dtype=str,
+            )
+        else:
+            raise NotImplementedError(
+                "cannot validate basis names for %s" % program
+            )
+
+        if not any(
+            # need to escape () b/c they aren't capturing groups, it's ccsd(t) or something
+            match(
+                "%s$"
+                % (basis.replace("(", "\(").replace(")", "\)"))
+                .replace("*", "\*")
+                .replace("+", "\+"),
+                name,
+                flags=IGNORECASE,
+            )
+            for basis in valid
+        ):
+            warning = (
+                "basis '%s' may not be available in %s\n" % (name, program)
+                + "if this is incorrect, please submit a bug report at https://github.com/QChASM/AaronTools.py/issues"
+            )
+
+            # try to suggest alternatives that have similar names
+            simm = [
+                seqmatch(
+                    lambda x: x in "-_()/", name.upper(), test_basis.upper()
+                ).ratio()
+                for test_basis in valid
+            ]
+            ndx = argsort(simm)[-5:][::-1]
+            warning += "\npossible misspelling of:\n"
+            warning += "\n".join([valid[i] for i in ndx])
+
+        return warning
 
     @staticmethod
     def get_gaussian(name):
         """
         returns the Gaussian09/16 name of the basis set
         currently just removes the hyphen from the Karlsruhe def2 ones
         """
-        if name.startswith('def2-'):
-            return name.replace('def2-', 'def2', 1)
+        if name.startswith("def2-"):
+            return name.replace("def2-", "def2", 1)
 
         return name
 
     @staticmethod
     def get_orca(name):
         """
         returns the ORCA name of the basis set
         currently just adds hyphen to Karlsruhe basis if it isn't there
         """
-        if name.startswith('def2') and not name.startswith('def2-'):
-            return name.replace('def2', 'def2-', 1)
+        if name.startswith("def2") and not name.startswith("def2-"):
+            return name.replace("def2", "def2-", 1)
 
         return name
 
     @staticmethod
     def get_psi4(name):
         """
         returns the Psi4 name of the basis set
         currently just adds hyphen to Karlsruhe basis if it isn't there
         """
-        if name.startswith('def2') and not name.startswith('def2-'):
-            return name.replace('def2', 'def2-', 1)
+        if name.startswith("def2") and not name.startswith("def2-"):
+            return name.replace("def2", "def2-", 1)
 
         return name
 
 
 class ECP(Basis):
     """ECP - aux info will be ignored"""
+
     default_elements = AnyTransitionMetal()
+
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
 
     def __eq__(self, other):
         if not isinstance(other, ECP):
             return False
 
         return super().__eq__(other)
 
+    @staticmethod
+    def sanity_check_basis(name, program):
+        import os.path
+        from difflib import SequenceMatcher as seqmatch
+        from re import IGNORECASE, match
+
+        from AaronTools.const import AARONTOOLS
+        from numpy import argsort, loadtxt
+
+        warning = None
+
+        if program.lower() == "gaussian":
+            valid = loadtxt(
+                os.path.join(
+                    AARONTOOLS,
+                    "theory",
+                    "valid_basis_sets",
+                    "gaussian_ecp.txt",
+                ),
+                dtype=str,
+            )
+        elif program.lower() == "orca":
+            valid = loadtxt(
+                os.path.join(
+                    AARONTOOLS, "theory", "valid_basis_sets", "orca_ecp.txt"
+                ),
+                dtype=str,
+            )
+        else:
+            raise NotImplementedError(
+                "cannot validate basis names for %s" % program
+            )
+
+        if not any(
+            # need to escape () b/c they aren't capturing groups, it's ccsd(t) or something
+            match(
+                "%s$"
+                % (basis.replace("(", "\(").replace(")", "\)"))
+                .replace("*", "\*")
+                .replace("+", "\+"),
+                name,
+                flags=IGNORECASE,
+            )
+            for basis in valid
+        ):
+            warning = (
+                "basis '%s' may not be available in %s\n" % (name, program)
+                + "if this is incorrect, please submit a bug report at https://github.com/QChASM/AaronTools.py/issues"
+            )
+
+            # try to suggest alternatives that have similar names
+            simm = [
+                seqmatch(
+                    lambda x: x in "-_()/", name.upper(), test_basis.upper()
+                ).ratio()
+                for test_basis in valid
+            ]
+            ndx = argsort(simm)[-5:][::-1]
+            warning += "\npossible misspelling of:\n"
+            warning += "\n".join([valid[i] for i in ndx])
+
+        return warning
+
 
 class BasisSet:
     """used to more easily get basis set info for writing input files"""
+
     ORCA_AUX = ["C", "J", "JK", "CABS", "OptRI CABS"]
     PSI4_AUX = ["JK", "RI"]
 
     def __init__(self, basis=None, ecp=None):
         """
         basis: list(Basis), Basis, str, or None
         ecp: list(ECP) or None
         """
         if isinstance(basis, str):
             basis = self.parse_basis_str(basis, cls=Basis)
         elif isinstance(basis, Basis):
             basis = [basis]
+        elif isinstance(basis, BasisSet):
+            if ecp is None:
+                ecp = basis.ecp
+            basis = basis.basis
 
         if isinstance(ecp, str):
             if ecp.split():
                 ecp = self.parse_basis_str(ecp, cls=ECP)
             else:
                 ecp = [ECP(ecp)]
         elif isinstance(ecp, ECP):
             ecp = [ecp]
+        elif isinstance(ecp, BasisSet):
+            ecp = ecp.ecp
 
         self.basis = basis
         self.ecp = ecp
 
     @property
     def elements_in_basis(self):
         """returns a list of elements in self's basis"""
@@ -242,47 +389,41 @@
         info = basis_str.split()
         i = 0
         basis_sets = []
         elements = []
         aux_type = None
         user_defined = False
         while i < len(info):
-            if (
-                    info[i].lstrip("!") in ELEMENTS or
-                    any(
-                        info[i].lower().lower().lstrip("!") == x for x in ["all", "tm"]
-                    )
+            if info[i].lstrip("!") in ELEMENTS or any(
+                info[i].lower().lower().lstrip("!") == x for x in ["all", "tm"]
             ):
                 elements.append(info[i])
             elif info[i].lower().startswith("aux"):
                 try:
                     aux_type = info[i + 1]
                     i += 1
                     if aux_type.lower() == "optri":
                         aux_type += " %s" % info[i + 1]
                         i += 1
                 except:
                     raise RuntimeError(
-                        "error while parsing basis set string: %s\nfound \"aux\"" +
-                        ", but no auxilliary type followed" % basis_str
+                        'error while parsing basis set string: %s\nfound "aux"'
+                        + ", but no auxilliary type followed" % basis_str
                     )
             else:
                 basis_name = info[i]
                 try:
                     # TODO: allow spaces in paths
                     if (
-                            (
-                                # os thinks I have a file named "aux" somewhere on my computer
-                                # I don't see it, but basis file names cannot start with 'aux'
-                                os.path.exists(info[i+1]) and
-                                not info[i+1].lower().startswith("aux")
-                            )
-                            or os.sep in info[i+1]
-                    ):
-                        user_defined = info[i+1]
+                        # os thinks I have a file named "aux" somewhere on my computer
+                        # I don't see it, but basis file names cannot start with 'aux'
+                        os.path.exists(info[i + 1])
+                        and not info[i + 1].lower().startswith("aux")
+                    ) or os.sep in info[i + 1]:
+                        user_defined = info[i + 1]
                         i += 1
                 except Exception as e:
                     pass
 
                 if not elements:
                     elements = None
 
@@ -293,42 +434,40 @@
                         aux_type=aux_type,
                         user_defined=user_defined,
                     )
                 )
                 elements = []
                 aux_type = None
                 user_defined = False
-
             i += 1
-
         return basis_sets
 
     def __eq__(self, other):
         if self.__class__ is not other.__class__:
             return False
-        if self.basis and other.basis:  
+        if self.basis and other.basis:
             if len(self.basis) != len(other.basis):
                 return False
             for b1, b2 in zip(sorted(self.basis), sorted(other.basis)):
                 if b1 != b2:
                     return False
         else:
             if self.basis != other.basis:
                 return False
-        
+
         if self.ecp and other.ecp:
             if len(self.ecp) != len(other.ecp):
                 return False
             for b1, b2 in zip(sorted(self.ecp), sorted(other.ecp)):
                 if b1 != b2:
                     return False
         else:
             if bool(self.ecp) != bool(other.ecp):
                 return False
-        
+
         return True
 
     def add_ecp(self, ecp):
         """add ecp to this BasisSet
         ecp - ECP"""
         if self.ecp is None:
             self.ecp = []
@@ -353,356 +492,531 @@
         if self.ecp is not None:
             for ecp in self.ecp:
                 ecp.refresh_elements(geometry)
 
     def get_gaussian_basis_info(self):
         """returns dict used by get_gaussian_header/footer with basis info"""
         info = {}
+        warnings = []
 
         if self.basis is not None:
-            #check if we need to use gen or genecp:
+            # check if we need to use gen or genecp:
             #    -a basis set is user-defined (stored in an external file e.g. from the BSE)
             #    -multiple basis sets
             #    -an ecp
             if (
-                    all([basis == self.basis[0] for basis in self.basis])
-                    and not self.basis[0].user_defined and self.ecp is None
+                all([basis == self.basis[0] for basis in self.basis])
+                and not self.basis[0].user_defined
+                and self.ecp is None
             ):
-                info[GAUSSIAN_ROUTE] = "/%s" % Basis.get_gaussian(self.basis[0].name)
+                basis_name = Basis.get_gaussian(self.basis[0].name)
+                warning = self.basis[0].sanity_check_basis(
+                    basis_name, "gaussian"
+                )
+                if warning:
+                    warnings.append(warning)
+                info[GAUSSIAN_ROUTE] = "/%s" % basis_name
             else:
-                if self.ecp is None or all(not ecp.elements for ecp in self.ecp):
+                if self.ecp is None or all(
+                    not ecp.elements for ecp in self.ecp
+                ):
                     info[GAUSSIAN_ROUTE] = "/gen"
                 else:
                     info[GAUSSIAN_ROUTE] = "/genecp"
 
                 out_str = ""
-                #gaussian flips out if you specify basis info for an element that
-                #isn't on the molecule, so make sure the basis set has an element
+                # gaussian flips out if you specify basis info for an element that
+                # isn't on the molecule, so make sure the basis set has an element
                 for basis in self.basis:
                     if basis.elements and not basis.user_defined:
                         out_str += " ".join([ele for ele in basis.elements])
                         out_str += " 0\n"
-                        out_str += Basis.get_gaussian(basis.name)
+                        basis_name = Basis.get_gaussian(basis.name)
+                        warning = basis.sanity_check_basis(
+                            basis_name, "gaussian"
+                        )
+                        if warning:
+                            warnings.append(warning)
+                        out_str += basis_name
                         out_str += "\n****\n"
 
                 for basis in self.basis:
                     if basis.elements:
                         if basis.user_defined:
                             if os.path.exists(basis.user_defined):
                                 with open(basis.user_defined, "r") as f:
                                     lines = f.readlines()
 
                                 i = 0
                                 while i < len(lines):
                                     test = lines[i].strip()
-                                    if not test or test.startswith('!'):
+                                    if not test or test.startswith("!"):
                                         i += 1
                                         continue
 
                                     ele = test.split()[0]
                                     while i < len(lines):
                                         if ele in basis.elements:
                                             out_str += lines[i]
 
-                                        if lines[i].startswith('****'):
+                                        if lines[i].startswith("****"):
                                             break
 
                                         i += 1
 
                                     i += 1
 
-                            #if the file does not exists, just insert the path as an @ file
+                            # if the file does not exists, just insert the path as an @ file
                             else:
                                 out_str += "@%s\n" % basis.user_defined
 
-                    info[GAUSSIAN_GEN_BASIS] = out_str
+                info[GAUSSIAN_GEN_BASIS] = out_str
 
         if self.ecp is not None:
             out_str = ""
             for basis in self.ecp:
                 if basis.elements and not basis.user_defined:
                     out_str += " ".join([ele for ele in basis.elements])
                     out_str += " 0\n"
-                    out_str += Basis.get_gaussian(basis.name)
+                    basis_name = Basis.get_gaussian(basis.name)
+                    warning = basis.sanity_check_basis(basis_name, "gaussian")
+                    if warning:
+                        warnings.append(warning)
+                    out_str += basis_name
                     out_str += "\n"
 
             for basis in self.ecp:
                 if basis.elements:
                     if basis.user_defined:
                         if os.path.exists(basis.user_defined):
                             with open(basis.user_defined, "r") as f:
                                 lines = f.readlines()
 
                                 i = 0
                                 while i < len(lines):
                                     test = lines[i].strip()
-                                    if not test or test.startswith('!'):
+                                    if not test or test.startswith("!"):
                                         i += 1
                                         continue
 
                                     ele = test.split()[0]
                                     while i < len(lines):
                                         if ele in basis.elements:
                                             out_str += lines[i]
 
-                                        if lines[i].startswith('****'):
+                                        if lines[i].startswith("****"):
                                             break
 
                                         i += 1
 
                                     i += 1
 
                         else:
                             out_str += "@%s\n" % basis.user_defined
 
             info[GAUSSIAN_GEN_ECP] = out_str
 
             if self.basis is None:
                 info[GAUSSIAN_ROUTE] = " Pseudo=Read"
 
-        return info
+        return info, warnings
 
     def get_orca_basis_info(self):
         """return dict for get_orca_header"""
-        #TODO: warn if basis should be f12
-        info = {ORCA_BLOCKS:{'basis':[]}, ORCA_ROUTE:[]}
+        # TODO: warn if basis should be f12
+        info = {ORCA_BLOCKS: {"basis": []}, ORCA_ROUTE: []}
+        warnings = []
 
         first_basis = []
 
         if self.basis is not None:
             for basis in self.basis:
                 if basis.elements:
                     if basis.aux_type is None:
                         if basis.aux_type not in first_basis:
                             if not basis.user_defined:
-                                out_str = Basis.get_orca(basis.name)
+                                basis_name = Basis.get_orca(basis.name)
+                                warning = Basis.sanity_check_basis(
+                                    basis_name, "orca"
+                                )
+                                if warning:
+                                    warnings.append(warning)
+                                out_str = basis_name
                                 info[ORCA_ROUTE].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                             else:
-                                out_str = "GTOName \"%s\"" % basis.user_defined
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                out_str = 'GTOName "%s"' % basis.user_defined
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                         else:
                             for ele in basis.elements:
                                 out_str = "newGTO            %-2s " % ele
 
                                 if not basis.user_defined:
-                                    out_str += "\"%s\" end" % Basis.get_orca(basis.name)
+                                    basis_name = Basis.get_orca(basis.name)
+                                    warning = Basis.sanity_check_basis(
+                                        basis_name, "orca"
+                                    )
+                                    if warning:
+                                        warnings.append(warning)
+                                    out_str += '"%s" end' % basis_name
                                 else:
-                                    out_str += "\"%s\" end" % basis.user_defined
+                                    out_str += '"%s" end' % basis.user_defined
 
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
 
                     elif basis.aux_type.upper() == "C":
                         if basis.aux_type not in first_basis:
                             if not basis.user_defined:
-                                out_str = "%s/C" % Basis.get_orca(basis.name)
+                                basis_name = Basis.get_orca(basis.name) + "/C"
+                                warning = Basis.sanity_check_basis(
+                                    basis_name, "orca"
+                                )
+                                if warning:
+                                    warnings.append(warning)
+                                out_str = "%s" % basis_name
                                 info[ORCA_ROUTE].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                             else:
-                                out_str = "AuxCGTOName \"%s\"" % basis.user_defined
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                out_str = (
+                                    'AuxCGTOName "%s"' % basis.user_defined
+                                )
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                         else:
                             for ele in basis.elements:
                                 out_str = "newAuxCGTO        %-2s " % ele
 
                                 if not basis.user_defined:
-                                    out_str += "\"%s/C\" end" % Basis.get_orca(basis.name)
+                                    basis_name = (
+                                        Basis.get_orca(basis.name) + "/C"
+                                    )
+                                    warning = Basis.sanity_check_basis(
+                                        basis_name, "orca"
+                                    )
+                                    if warning:
+                                        warnings.append(warning)
+
+                                    out_str += '"%s" end' % basis_name
                                 else:
-                                    out_str += "\"%s\" end" % basis.user_defined
+                                    out_str += '"%s" end' % basis.user_defined
 
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
 
                     elif basis.aux_type.upper() == "J":
                         if basis.aux_type not in first_basis:
                             if not basis.user_defined:
-                                out_str = "%s/J" % Basis.get_orca(basis.name)
+                                basis_name = Basis.get_orca(basis.name) + "/J"
+                                warning = Basis.sanity_check_basis(
+                                    basis_name, "orca"
+                                )
+                                if warning:
+                                    warnings.append(warning)
+                                out_str = "%s" % basis_name
                                 info[ORCA_ROUTE].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                             else:
-                                out_str = "AuxJGTOName \"%s\"" % basis.user_defined
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                out_str = (
+                                    'AuxJGTOName "%s"' % basis.user_defined
+                                )
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                         else:
                             for ele in basis.elements:
                                 out_str = "newAuxJGTO        %-2s " % ele
 
                                 if not basis.user_defined:
-                                    out_str += "\"%s/J\" end" % Basis.get_orca(basis.name)
+                                    basis_name = (
+                                        Basis.get_orca(basis.name) + "/J"
+                                    )
+                                    warning = Basis.sanity_check_basis(
+                                        basis_name, "orca"
+                                    )
+                                    if warning:
+                                        warnings.append(warning)
+
+                                    out_str += '"%s" end' % basis_name
                                 else:
-                                    out_str += "\"%s\" end" % basis.user_defined
+                                    out_str += '"%s" end' % basis.user_defined
 
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
 
                     elif basis.aux_type.upper() == "JK":
                         if basis.aux_type not in first_basis:
                             if not basis.user_defined:
-                                out_str = "%s/JK" % Basis.get_orca(basis.name)
+                                basis_name = Basis.get_orca(basis.name) + "/JK"
+                                warning = Basis.sanity_check_basis(
+                                    basis_name, "orca"
+                                )
+                                if warning:
+                                    warnings.append(warning)
+                                out_str = "%s" % basis_name
                                 info[ORCA_ROUTE].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                             else:
-                                out_str = "AuxJKGTOName \"%s\"" % basis.user_defined
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                out_str = (
+                                    'AuxJKGTOName "%s"' % basis.user_defined
+                                )
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                         else:
                             for ele in basis.elements:
                                 out_str = "newAuxJKGTO       %-2s " % ele
 
                                 if not basis.user_defined:
-                                    out_str += "\"%s/JK\" end" % Basis.get_orca(basis.name)
+                                    basis_name = (
+                                        Basis.get_orca(basis.name) + "/JK"
+                                    )
+                                    warning = Basis.sanity_check_basis(
+                                        basis_name, "orca"
+                                    )
+                                    if warning:
+                                        warnings.append(warning)
+
+                                    out_str += '"%s" end' % basis_name
                                 else:
-                                    out_str += "\"%s\" end" % basis.user_defined
+                                    out_str += '"%s" end' % basis.user_defined
 
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
 
                     elif basis.aux_type.upper() == "CABS":
                         if basis.aux_type not in first_basis:
                             if not basis.user_defined:
-                                out_str = "%s-CABS" % Basis.get_orca(basis.name)
+                                basis_name = (
+                                    Basis.get_orca(basis.name) + "-CABS"
+                                )
+                                warning = Basis.sanity_check_basis(
+                                    basis_name, "orca"
+                                )
+                                if warning:
+                                    warnings.append(warning)
+                                out_str = "%s" % basis_name
                                 info[ORCA_ROUTE].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                             else:
-                                out_str = "CABSGTOName \"%s\"" % basis.user_defined
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                out_str = (
+                                    'CABSGTOName "%s"' % basis.user_defined
+                                )
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                         else:
                             for ele in basis.elements:
                                 out_str = "newCABSGTO        %-2s " % ele
 
                                 if not basis.user_defined:
-                                    out_str += "\"%s-CABS\" end" % Basis.get_orca(basis.name)
+                                    basis_name = (
+                                        Basis.get_orca(basis.name) + "-CABS"
+                                    )
+                                    warning = Basis.sanity_check_basis(
+                                        basis_name, "orca"
+                                    )
+                                    if warning:
+                                        warnings.append(warning)
+
+                                    out_str += '"%s" end' % basis_name
                                 else:
-                                    out_str += "\"%s\" end" % basis.user_defined
+                                    out_str += '"%s" end' % basis.user_defined
 
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
 
                     elif basis.aux_type.upper() == "OPTRI CABS":
                         if basis.aux_type not in first_basis:
                             if not basis.user_defined:
-                                out_str = "%s-OptRI" % Basis.get_orca(basis.name)
+                                basis_name = (
+                                    Basis.get_orca(basis.name) + "-OptRI"
+                                )
+                                warning = Basis.sanity_check_basis(
+                                    basis_name, "orca"
+                                )
+                                if warning:
+                                    warnings.append(warning)
+                                out_str = "%s" % basis_name
                                 info[ORCA_ROUTE].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                             else:
-                                out_str = "CABSGTOName \"%s\"" % basis.user_defined
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                out_str = (
+                                    'CABSGTOName "%s"' % basis.user_defined
+                                )
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
                                 first_basis.append(basis.aux_type)
 
                         else:
                             for ele in basis.elements:
                                 out_str = "newCABSGTO        %-2s " % ele
 
                                 if not basis.user_defined:
-                                    out_str += "\"%s-OptRI\" end" % Basis.get_orca(basis.name)
+                                    basis_name = (
+                                        Basis.get_orca(basis.name) + "-OptRI"
+                                    )
+                                    warning = Basis.sanity_check_basis(
+                                        basis_name, "orca"
+                                    )
+                                    if warning:
+                                        warnings.append(warning)
+
+                                    out_str += '"%s" end' % basis_name
                                 else:
-                                    out_str += "\"%s\" end" % basis.user_defined
+                                    out_str += '"%s" end' % basis.user_defined
 
-                                info[ORCA_BLOCKS]['basis'].append(out_str)
+                                info[ORCA_BLOCKS]["basis"].append(out_str)
 
         if self.ecp is not None:
             for basis in self.ecp:
                 if basis.elements and not basis.user_defined:
                     for ele in basis.elements:
                         out_str = "newECP            %-2s " % ele
-                        out_str += "\"%s\" end" % Basis.get_orca(basis.name)
+                        basis_name = Basis.get_orca(basis.name)
+                        warning = basis.sanity_check_basis(basis_name, "orca")
+                        if warning:
+                            warnings.append(warning)
+                        out_str += '"%s" end' % basis_name
 
-                        info[ORCA_BLOCKS]['basis'].append(out_str)
+                        info[ORCA_BLOCKS]["basis"].append(out_str)
 
                 elif basis.elements and basis.user_defined:
-                    #TODO: check if this works
-                    out_str = "GTOName \"%s\"" % basis.user_defined
+                    # TODO: check if this works
+                    out_str = 'GTOName "%s"' % basis.user_defined
 
-                    info[ORCA_BLOCKS]['basis'].append(out_str)
+                    info[ORCA_BLOCKS]["basis"].append(out_str)
 
-        return info
+        return info, warnings
 
     def get_psi4_basis_info(self, sapt=False):
         """
         sapt: bool, use df_basis_sapt instead of df_basis_scf for jk basis
         return dict for get_psi4_header
         """
         out_str = ""
         out_str2 = None
         out_str3 = None
         out_str4 = None
+        warnings = []
 
         first_basis = []
 
         if self.basis is not None:
             for basis in self.basis:
                 if basis.aux_type not in first_basis:
                     first_basis.append(basis.aux_type)
                     if basis.aux_type is None or basis.user_defined:
                         out_str += "basis {\n"
-                        out_str += "    assign    %s\n" % Basis.get_psi4(basis.name)
+                        basis_name = Basis.get_psi4(basis.name)
+                        warning = basis.sanity_check_basis(basis_name, "psi4")
+                        if warning and not basis.user_defined:
+                            warnings.append(warning)
+                        out_str += "    assign    %s\n" % basis_name
 
                     elif basis.aux_type.upper() == "JK":
                         if sapt:
                             out_str4 = "df_basis_sapt {\n"
                         else:
                             out_str4 = "df_basis_scf {\n"
 
-                        out_str4 += "    assign    %s-jkfit\n" % Basis.get_psi4(basis.name)
+                        basis_name = Basis.get_psi4(basis.name) + "-jkfit"
+                        warning = basis.sanity_check_basis(basis_name, "psi4")
+                        if warning and not basis.user_defined:
+                            warnings.append(warning)
+                        out_str4 += "    assign    %s\n" % basis_name
 
                     elif basis.aux_type.upper() == "RI":
                         out_str2 = "df_basis_%s {\n"
-                        if basis.name.lower() == "sto-3g" or basis.name.lower() == "3-21g":
-                            out_str2 += "    assign    %s-rifit\n" % Basis.get_psi4(basis.name)
+                        if (
+                            basis.name.lower() == "sto-3g"
+                            or basis.name.lower() == "3-21g"
+                        ):
+                            basis_name = Basis.get_psi4(basis.name) + "-rifit"
+                            warning = basis.sanity_check_basis(
+                                basis_name, "psi4"
+                            )
+                            if warning and not basis.user_defined:
+                                warnings.append(warning)
+
+                            out_str2 += "    assign    %s\n" % basis_name
                         else:
-                            out_str2 += "    assign    %s-ri\n" % Basis.get_psi4(basis.name)
+                            basis_name = Basis.get_psi4(basis.name) + "-ri"
+                            warning = basis.sanity_check_basis(
+                                basis_name, "psi4"
+                            )
+                            if warning and not basis.user_defined:
+                                warnings.append(warning)
+
+                            out_str2 += "    assign    %s\n" % basis_name
 
                 else:
                     if basis.aux_type is None or basis.user_defined:
+                        basis_name = Basis.get_psi4(basis.name)
+                        warning = basis.sanity_check_basis(basis_name, "psi4")
+                        if warning and not basis.user_defined:
+                            warnings.append(warning)
                         for ele in basis.elements:
-                            out_str += "    assign %-2s %s\n" % (ele, Basis.get_psi4(basis.name))
+                            out_str += "    assign %-2s %s\n" % (
+                                ele,
+                                basis_name,
+                            )
 
                     elif basis.aux_type.upper() == "JK":
+                        basis_name = Basis.get_psi4(basis.name) + "-jkfit"
+                        warning = basis.sanity_check_basis(basis_name, "psi4")
+                        if warning and not basis.user_defined:
+                            warnings.append(warning)
                         for ele in basis.elements:
-                            out_str4 += "    assign %-2s %s-jkfit\n" % (
+                            out_str4 += "    assign %-2s %s\n" % (
                                 ele,
-                                Basis.get_psi4(basis.name),
+                                basis_name,
                             )
 
                     elif basis.aux_type.upper() == "RI":
+                        basis_name = Basis.get_psi4(basis.name)
+                        if (
+                            basis_name.lower() == "sto-3g"
+                            or basis_name.lower() == "3-21g"
+                        ):
+                            basis_name += "-rifit"
+                        else:
+                            basis_name += "-ri"
+                        warning = basis.sanity_check_basis(basis_name, "psi4")
+                        if warning and not basis.user_defined:
+                            warnings.append(warning)
+
                         for ele in basis.elements:
-                            if basis.name.lower() == "sto-3g" or basis.name.lower() == "3-21g":
+                            if (
+                                basis.name.lower() == "sto-3g"
+                                or basis.name.lower() == "3-21g"
+                            ):
                                 out_str2 += "    assign %-2s %s-rifit\n" % (
                                     ele,
-                                    Basis.get_psi4(basis.name),
-                                )
-                            else:
-                                out_str2 += "    assign %-2s %s-ri\n" % (
-                                    ele,
-                                    Basis.get_psi4(basis.name),
+                                    basis_name,
                                 )
 
             if any(basis.user_defined for basis in self.basis):
                 out_str3 = ""
                 for basis in self.basis:
                     if basis.user_defined:
                         if os.path.exists(basis.user_defined):
                             out_str3 += "\n[%s]\n" % basis.name
-                            with open(basis.user_defined, 'r') as f:
+                            with open(basis.user_defined, "r") as f:
                                 lines = [
-                                    line.rstrip() for line in f.readlines()
-                                    if line.strip() and not line.startswith('!')
+                                    line.rstrip()
+                                    for line in f.readlines()
+                                    if line.strip()
+                                    and not line.startswith("!")
                                 ]
-                                out_str3 += '\n'.join(lines)
-                                out_str3 += '\n\n'
+                                out_str3 += "\n".join(lines)
+                                out_str3 += "\n\n"
 
             if out_str3 is not None:
                 out_str += out_str3
 
             if out_str:
                 out_str += "}"
 
@@ -713,48 +1027,57 @@
 
             if out_str4 is not None:
                 out_str4 += "}"
 
                 out_str += "\n\n%s" % out_str4
 
         if out_str:
-            info = {PSI4_BEFORE_GEOM:[out_str]}
+            info = {PSI4_BEFORE_GEOM: [out_str]}
         else:
             info = {}
 
-        return info
+        return info, warnings
 
     def check_for_elements(self, geometry):
         """checks to make sure each element is in a basis set"""
         warning = ""
-        #assume all elements aren't in a basis set, remove from the list if they have a basis
-        #need to check each type of aux basis
+        # assume all elements aren't in a basis set, remove from the list if they have a basis
+        # need to check each type of aux basis
         elements = list(set([str(atom.element) for atom in geometry.atoms]))
         if self.basis is not None:
             elements_without_basis = {}
             for basis in self.basis:
                 if basis.aux_type not in elements_without_basis:
-                    elements_without_basis[basis.aux_type] = [str(e) for e in elements]
+                    elements_without_basis[basis.aux_type] = [
+                        str(e) for e in elements
+                    ]
 
                 for element in basis.elements:
                     if element in elements_without_basis[basis.aux_type]:
                         elements_without_basis[basis.aux_type].remove(element)
 
-            if any(elements_without_basis[aux] for aux in elements_without_basis.keys()):
+            if any(
+                elements_without_basis[aux]
+                for aux in elements_without_basis.keys()
+            ):
                 for aux in elements_without_basis.keys():
                     if elements_without_basis[aux]:
                         if aux is not None and aux != "no":
                             warning += "%s ha%s no auxiliary %s basis; " % (
                                 ", ".join(elements_without_basis[aux]),
-                                "s" if len(elements_without_basis[aux]) == 1 else "ve",
+                                "s"
+                                if len(elements_without_basis[aux]) == 1
+                                else "ve",
                                 aux,
                             )
 
                         else:
                             warning += "%s ha%s no basis; " % (
                                 ", ".join(elements_without_basis[aux]),
-                                "s" if len(elements_without_basis[aux]) == 1 else "ve",
+                                "s"
+                                if len(elements_without_basis[aux]) == 1
+                                else "ve",
                             )
 
-                return warning.strip('; ')
+                return warning.strip("; ")
 
             return None
```

### Comparing `AaronTools-1.0b8/theory/emp_dispersion.py` & `AaronTools-1.0b9/theory/emp_dispersion.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/theory/grid.py` & `AaronTools-1.0b9/theory/grid.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/theory/implicit_solvent.py` & `AaronTools-1.0b9/theory/implicit_solvent.py`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/theory/job_types.py` & `AaronTools-1.0b9/theory/job_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     ORCA_ROUTE,
     PSI4_BEFORE_GEOM,
     PSI4_COORDINATES,
     PSI4_JOB,
     PSI4_OPTKING,
     PSI4_SETTINGS,
 )
+from AaronTools.utils.utils import range_list
 
 
 class JobType:
     """
     parent class of all job types
     initialization keywords should be the same as attribute names
     """
@@ -493,15 +494,15 @@
                         finders, val = constraint
                         hold = False
                     x_atoms = self.geometry.find(finders)
                     var_name = "gx%i" % group_count
                     group_count += 1
                     if hold:
                         add_freeze_list = True
-                        for i, atom in enumerate(y_atoms):
+                        for i, atom in enumerate(x_atoms):
                             freeze_str += "    %2i x\n" % (
                                 self.geometry.atoms.index(atom) + 1
                             )
                             coords[i][0] = val
                     else:
                         vars.append([var_name, val, True])
                         for i, atom in enumerate(self.geometry.atoms):
@@ -623,46 +624,67 @@
             out[PSI4_COORDINATES] = {
                 "coords": coords,
                 "variables": vars,
             }
 
         return out
 
-    def get_xtb(self, config):
-        rv = ""
-        if self.constraints:
-            force = config["Job"].get("force_constant", fallback=0.5)
-            constraints = it.chain.from_iterable(*self.constraints.values())
-            frozen = {
-                str(self.geometry.atoms.index(c) + 1) for c in constraints
-            }
-            frozen = ",".join(sorted(frozen, key=lambda x: int(x)))
+    def get_xcontrol(self, config, ref=None):
+        """
+        Generates xcontrol file constraints
+
+        Returns: dict(xcontrol)
+        """
+        if ref is None:
+            ref = "ref.xyz"
+        xcontrol = ""
+        # only put constraints in xcontrol file so this works with Crest also
+        frozen = [i + 1 for i, a in enumerate(self.geometry) if bool(a.flag)]
+        if frozen:
+            frozen = range_list(frozen)
+            xcontrol += "$fix\n"
+            xcontrol += "  atoms: {}\n".format(frozen)
+            xcontrol += "  freeze: {}\n".format(frozen)
+        elif self.constraints:
+            xcontrol += "$constrain\n"
+            xcontrol += "  force constant={}\n".format(
+                config["Job"].get("constrain_force", fallback="0.5")
+            )
+            xcontrol += "  reference={}\n".format(
+                config["Job"].get("constrain_ref", fallback=ref)
+            )
+            constrained = set([])
+            for bond in self.constraints.get("bonds", []):
+                bond = self.geometry.find(bond)
+                constrained.update(bond)
+                xcontrol += "  distance: {},{},auto\n".format(
+                    *(self.geometry.atoms.index(c) + 1 for c in bond)
+                )
+            for angle in self.constraints.get("angles", []):
+                angle = self.geometry.find(angle)
+                constrained.update(angle)
+                xcontrol += "  angle: {},{},{},auto\n".format(
+                    *(self.geometry.atoms.index(c) + 1 for c in angle)
+                )
+            for dihedral in self.constraints.get("torsions", []):
+                dihedral = self.geometry.find(dihedral)
+                constrained.update(dihedral)
+                xcontrol += "  dihedral: {},{},{},{},auto\n".format(
+                    *(self.geometry.atoms.index(c) + 1 for c in dihedral)
+                )
             relaxed = {
-                str(i + 1)
+                i + 1
                 for i, a in enumerate(self.geometry.atoms)
-                if a not in constraints
+                if a not in constrained
             }
-            relaxed = ",".join(sorted(relaxed, key=lambda x: int(x)))
-            rv += "$constrain\n"
-            rv += "    atoms: {}\n".format(frozen)
-            rv += "    force constant={}\n".format(force)
-            rv += "    referenct=ref.xyz\n"
-            rv += "$metadyn\n"
-            rv += "    atoms: {}\n".format(relaxed)
-        for section in config:
-            for option, value in config[section].items():
-                if "charge" in option:
-                    rv += "$chrg {}\n".format(value)
-                if "multiplicity" in option:
-                    rv += "$spin {}\n".format(int(value) - 1)
-                if "temperature" in option:
-                    rv += "$thermo\n"
-                    rv += "    temp={}".format(value)
-        rv += "$end\n"
-        return rv
+            relaxed = range_list(relaxed)
+            xcontrol += "$metadyn\n"
+            xcontrol += "  atoms: {}\n".format(relaxed)
+        xcontrol += "$end\n"
+        return xcontrol
 
 
 class FrequencyJob(JobType):
     """frequnecy job"""
 
     def __init__(self, numerical=False, temperature=None):
         """
```

### Comparing `AaronTools-1.0b8/theory/theory.py` & `AaronTools-1.0b9/theory/theory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """for constructing headers and footers for input files"""
 import itertools as it
 import re
 
-from AaronTools.const import ELEMENTS, UNIT
+from AaronTools.const import ELEMENTS, RMSD_CUTOFF, UNIT
 from AaronTools.theory import (
     GAUSSIAN_COMMENT,
     GAUSSIAN_CONSTRAINTS,
     GAUSSIAN_COORDINATES,
     GAUSSIAN_GEN_BASIS,
     GAUSSIAN_GEN_ECP,
     GAUSSIAN_POST,
@@ -161,24 +161,21 @@
         if grid is not None:
             if not isinstance(grid, IntegrationGrid):
                 self.grid = IntegrationGrid(grid)
             else:
                 self.grid = grid
 
         if basis is not None:
-            if not isinstance(basis, BasisSet):
-                self.basis = BasisSet(basis)
-            else:
-                self.basis = basis
+            self.basis = BasisSet(basis=basis)
 
         if ecp is not None:
             if self.basis is None:
                 self.basis = BasisSet(ecp=ecp)
             else:
-                self.basis.ecp = BasisSet.parse_basis_str(ecp, cls=ECP)
+                self.basis.ecp = BasisSet(ecp=ecp).ecp
 
         if empirical_dispersion is not None:
             if not isinstance(empirical_dispersion, EmpiricalDispersion):
                 self.empirical_dispersion = EmpiricalDispersion(
                     empirical_dispersion
                 )
             else:
@@ -251,27 +248,31 @@
         return True
 
     def make_header(
         self,
         geom=None,
         style="gaussian",
         conditional_kwargs=None,
+        sanity_check_method=False,
         **kwargs,
     ):
         """
         geom: Geometry
         style: str, gaussian, orca, or psi4
         conditional_kwargs: dict - keys are ORCA_*, PSI4_*, or GAUSSIAN_*
             items in conditional_kwargs will only be added
             to the input if they would otherwise be preset
             e.g. if self.job_type is FrequencyJob and a Gaussian
             input file is being written,
             conditional_kwargs = {GAUSSIAN_ROUTE:{'opt':['noeigentest']}}
             will not add opt=noeigentest to the route
             but if it's an OptimizationJob, it will add opt=noeigentest
+        sanity_check_method: bool, check if method is available in recent version
+                             of the target software package (Psi4 checks when its
+                             footer is created)
         kwargs: keywords are ORCA_*, PSI4_*, or GAUSSIAN_*
         """
         if geom is None:
             geom = self.geometry
 
         if conditional_kwargs is None:
             conditional_kwargs = {}
@@ -407,20 +408,23 @@
         NotImplementedError("no get_molecule method for style: %s" % style)
 
     def make_footer(
         self,
         geom=None,
         style="gaussian",
         conditional_kwargs=None,
+        sanity_check_method=False,
         **kwargs,
     ):
         """
         geom: Geometry
         style: str, gaussian or psi4
         conditional_kwargs: dict, see make_header
+        sanity_check_method: bool, check if method is available in recent version
+                             of the target software package (Psi4 only)
         kwargs: keywords are GAUSSIAN_*, ORCA_*, or PSI4_*
         """
         if geom is None:
             geom = self.geometry
 
         if conditional_kwargs is None:
             conditional_kwargs = {}
@@ -479,18 +483,20 @@
 
     def get_gaussian_header(
         self,
         return_warnings=False,
         conditional_kwargs=None,
         **other_kw_dict,
     ):
-        """write Gaussian09/16 input file header (up to charge mult)
+        """
+        write Gaussian09/16 input file header (up to charge mult)
         other_kw_dict is a dictionary with file positions (using GAUSSIAN_*)
         corresponding to options/keywords
-        returns warnings if a certain feature is not available in Gaussian"""
+        returns warnings if a certain feature is not available in Gaussian
+        """
 
         if conditional_kwargs is None:
             conditional_kwargs = {}
 
         warnings = []
         if self.job_type is not None:
             for job in self.job_type[::-1]:
@@ -556,17 +562,24 @@
 
         # start route line with method
         out_str += "#n "
         if self.method is not None:
             func, warning = self.method.get_gaussian()
             if warning is not None:
                 warnings.append(warning)
+            warning = self.method.sanity_check_method(func, "gaussian")
+            if warning:
+                warnings.append(warning)
             out_str += "%s" % func
             if not self.method.is_semiempirical and self.basis is not None:
-                basis_info = self.basis.get_gaussian_basis_info()
+                (
+                    basis_info,
+                    basis_warnings,
+                ) = self.basis.get_gaussian_basis_info()
+                warnings.extend(basis_warnings)
                 # check basis elements to make sure no element is
                 # in two basis sets or left out of any
                 if self.geometry is not None:
                     basis_warning = self.basis.check_for_elements(
                         self.geometry
                     )
                     if basis_warning is not None:
@@ -646,15 +659,14 @@
         out_str += "\n"
 
         # charge mult
         out_str += "%i %i\n" % (int(self.charge), int(self.multiplicity))
 
         if return_warnings:
             return out_str, warnings
-
         return out_str
 
     def get_gaussian_molecule(
         self,
         return_warnings=False,
         conditional_kwargs=None,
         **other_kw_dict,
@@ -684,18 +696,26 @@
         if "coords" not in other_kw_dict[GAUSSIAN_COORDINATES]:
             other_kw_dict[GAUSSIAN_COORDINATES][
                 "coords"
             ] = self.geometry.coords
 
         s = ""
 
+        # atom specs need flag column before coords if any atoms frozen
+        has_frozen = False
+        for atom in self.geometry.atoms:
+            if atom.flag:
+                has_frozen = True
+                break
         for atom, coord in zip(
             self.geometry.atoms, other_kw_dict[GAUSSIAN_COORDINATES]["coords"]
         ):
             s += "%-2s" % atom.element
+            if has_frozen:
+                s += " % 2d" % (-1 if atom.flag else 0)
             for val in coord:
                 s += "  "
                 if isinstance(val, float):
                     s += " %9.5f" % val
                 elif isinstance(val, str):
                     s += " %5s" % val
                 elif isinstance(val, int):
@@ -754,15 +774,15 @@
         # if method is not semi emperical, basis set might be gen or genecp
         # get basis info (will be written after constraints)
         if (
             self.method is not None
             and not self.method.is_semiempirical
             and self.basis is not None
         ):
-            basis_info = self.basis.get_gaussian_basis_info()
+            basis_info, warnings = self.basis.get_gaussian_basis_info()
 
         elif (
             self.method is not None
             and not self.method.is_semiempirical
             and self.basis is None
         ):
             basis_info = {}
@@ -831,15 +851,16 @@
                 job_dict = job.get_orca()
                 other_kw_dict = combine_dicts(job_dict, other_kw_dict)
 
         warnings = []
 
         # if method isn't semi-empirical, get basis info to write later
         if not self.method.is_semiempirical and self.basis is not None:
-            basis_info = self.basis.get_orca_basis_info()
+            basis_info, basis_warnings = self.basis.get_orca_basis_info()
+            warnings.extend(basis_warnings)
             if self.geometry is not None:
                 warning = self.basis.check_for_elements(self.geometry)
                 if warning is not None:
                     warnings.append(warning)
 
         else:
             basis_info = {}
@@ -892,14 +913,17 @@
 
         out_str += "!"
         # method
         if self.method is not None:
             func, warning = self.method.get_orca()
             if warning is not None:
                 warnings.append(warning)
+            warning = self.method.sanity_check_method(func, "orca")
+            if warning:
+                warnings.append(warning)
             out_str += " %s" % func
 
         # add other route options
         if ORCA_ROUTE in other_kw_dict:
             if not out_str.endswith(" "):
                 out_str += " "
 
@@ -979,17 +1003,18 @@
         if self.solvent is not None:
             solvent_info, warning = self.solvent.get_psi4()
             warnings.extend(warning)
             other_kw_dict = combine_dicts(other_kw_dict, solvent_info)
 
         # get basis info if method is not semi empirical
         if not self.method.is_semiempirical and self.basis is not None:
-            basis_info = self.basis.get_psi4_basis_info(
+            basis_info, basis_warnings = self.basis.get_psi4_basis_info(
                 isinstance(self.method, SAPTMethod)
             )
+            warnings.extend(basis_warnings)
             if self.geometry is not None:
                 warning = self.basis.check_for_elements(self.geometry)
                 if warning is not None:
                     warnings.append(warning)
 
             # aux basis sets might have a '%s' b/c the keyword to apply them depends on
             # the method - replace %s with the appropriate thing for the method
@@ -1099,14 +1124,26 @@
         if PSI4_COORDINATES not in other_kw_dict:
             other_kw_dict[PSI4_COORDINATES] = {}
 
         if "coords" not in other_kw_dict[PSI4_COORDINATES]:
             other_kw_dict[PSI4_COORDINATES]["coords"] = self.geometry.coords
 
         s = ""
+
+        if isinstance(self.method, SAPTMethod) and not hasattr(
+            self.charge, "__iter__"
+        ):
+            warnings.append(
+                "for a SAPTMethod, charge and multiplicity should both be lists\n"
+                "with the first item being the overall charge/multiplicity and\n"
+                "subsequent items being the charge/multiplicity of the\n"
+                "corresponding monomer"
+            )
+            return s, warnings
+
         if (
             isinstance(self.method, SAPTMethod)
             and sum(self.multiplicity[1:]) - len(self.multiplicity[1:]) + 1
             > self.multiplicity[0]
         ):
             use_molecule_array = True
             s += "mol = psi4.core.Molecule.from_arrays(\n"
@@ -1119,15 +1156,28 @@
                             keyword,
                             repr(other_kw_dict[keyword][0]),
                         )
 
         else:
             s += "molecule {\n"
             if isinstance(self.method, SAPTMethod):
+                if not hasattr(self.charge, "__iter__"):
+                    warnings.append(
+                        "for a SAPTMethod, charge and multiplicity should both be lists\n"
+                        "with the first item being the overall charge/multiplicity and\n"
+                        "subsequent items being the charge/multiplicity of the\n"
+                        "corresponding monomer"
+                    )
                 s += "    %2i %i\n" % (self.charge[0], self.multiplicity[0])
+                if len(self.charge) > 1 and self.charge[0] != sum(
+                    self.charge[1:]
+                ):
+                    warnings.append(
+                        "total charge is not equal to sum of monomer charges"
+                    )
             else:
                 s += "    %2i %i\n" % (self.charge, self.multiplicity)
 
             if PSI4_MOLECULE in other_kw_dict:
                 for keyword in other_kw_dict[PSI4_MOLECULE]:
                     if other_kw_dict[PSI4_MOLECULE][keyword]:
                         opt = other_kw_dict[PSI4_MOLECULE][keyword][0]
@@ -1400,15 +1450,25 @@
                     )
 
             out_str += "}\n\n"
 
         # method is method name + dispersion if there is dispersion
         method = self.method.get_psi4()[0]
         if self.empirical_dispersion is not None:
-            method += self.empirical_dispersion.get_psi4()[0]
+            disp = self.empirical_dispersion.get_psi4()[0]
+            if "%s" in method:
+                method = method % disp
+            else:
+                method += disp
+        elif "%s" in method:
+            method = method.replace("%s", "")
+
+        warning = self.method.sanity_check_method(method, "psi4")
+        if warning:
+            warnings.append(warning)
 
         # after job stuff - replace METHOD with method
         if PSI4_BEFORE_JOB in other_kw_dict:
             for opt in other_kw_dict[PSI4_BEFORE_JOB]:
                 if "$METHOD" in opt:
                     opt = opt.replace("$METHOD", "'%s'" % method)
 
@@ -1449,11 +1509,181 @@
                 out_str += opt
                 out_str += "\n"
 
         if return_warnings:
             return out_str, warnings
         return out_str
 
-    def write_aux(self, config):
-        for job_type in self.job_type:
-            if isinstance(job_type, CrestJob):
-                return job_type.write_aux(config)
+    def get_xtb_cmdline(self, config):
+        """
+        Uses the config and job type to set command line options for xtb and crest jobs
+
+        Returns a dictionary of option=val pairs; val is None when option doesn't take
+        an argument. This dict should be parsed by the caller into the command line
+        string.
+        """
+        if len(self.job_type) > 1:
+            raise NotImplementedError(
+                "Multiple job types not supported for crest/xtb"
+            )
+        cmdline = {}
+        job_type = self.job_type[0]
+        style = config["Job"]["exec_type"]
+        if style not in ["xtb", "crest"]:
+            raise NotImplementedError(
+                "Wrong executable type: %s (can only get command line options "
+                "for `xtb` or `crest`)" % style
+            )
+
+        # pull in stuff set by resolve_error
+        if config._args:
+            for arg in config._args:
+                cmdline[arg] = None
+        if config._kwargs:
+            for key, val in config._kwargs.items():
+                cmdline[key] = val
+        # run types
+        if "gfn" in config["Job"]:
+            cmdline["--gfn"] = config["Job"]["gfn"]
+        if (
+            style == "xtb"
+            and hasattr(job_type, "transition_state")
+            and job_type.transition_state
+        ):
+            cmdline["--optts"] = None
+        elif style == "xtb":
+            cmdline["--opt"] = None
+
+        # charge/mult/temp
+        if self.charge != 0:
+            cmdline["--chrg"] = self.charge
+        if self.multiplicity != 1:
+            cmdline["--uhf"] = self.multiplicity - 1
+        if style == "crest":
+            cmdline["--temp"] = config["Theory"].get(
+                "temperature", fallback="298"
+            )
+        else:
+            cmdline["--etemp"] = config["Theory"].get(
+                "temperature", fallback="298"
+            )
+
+        # screening parameters
+        if (
+            style == "crest"
+            and "energy_cutoff" in config["Job"]
+            and config["Job"].getfloat("energy_cutoff") > 6
+        ):
+            cmdline["--ewin"] = config["Job"]["energy_cutoff"]
+        if (
+            style == "crest"
+            and "rmsd_cutoff" in config["Job"]
+            and config["Job"].getfloat("rmsd_cutoff") < 0.125
+        ):
+            cmdline["--rthr"] = config["Job"]["rmsd_cutoff"]
+
+        # solvent stuff
+        if (
+            "solvent_model" in config["Theory"]
+            and config["Theory"]["solvent_model"] == "alpb"
+        ):
+            solvent = config["Theory"]["solvent"].split()
+            if len(solvent) > 1:
+                solvent, ref = solvent
+            elif len(solvent) == 1:
+                solvent, ref = solvent[0], None
+            else:
+                raise ValueError
+            if solvent.lower() not in [
+                "acetone",
+                "acetonitrile",
+                "aniline",
+                "benzaldehyde",
+                "benzene",
+                "ch2cl2",
+                "chcl3",
+                "cs2",
+                "dioxane",
+                "dmf",
+                "dmso",
+                "ether",
+                "ethylacetate",
+                "furane",
+                "hexandecane",
+                "hexane",
+                "methanol",
+                "nitromethane",
+                "octanol",
+                "woctanol",
+                "phenol",
+                "toluene",
+                "thf",
+                "water",
+            ]:
+                raise ValueError("%s is not a supported solvent" % solvent)
+            if ref is not None and ref.lower() not in ["reference", "bar1m"]:
+                raise ValueError(
+                    "%s Gsolv reference state not supported" % ref
+                )
+            if style.lower() == "crest" or ref is None:
+                cmdline["--alpb"] = "{}".format(solvent)
+            else:
+                cmdline["--alpb"] = "{} {}".format(solvent, ref)
+        elif (
+            "solvent_model" in config["Theory"]
+            and config["Theory"]["solvent_model"] == "gbsa"
+        ):
+            solvent = config["Theory"]["solvent"].split()
+            if len(solvent) > 1:
+                solvent, ref = solvent
+            else:
+                solvent, ref = solvent[0], None
+            if solvent.lower() not in [
+                "acetone",
+                "acetonitrile",
+                "benzene",
+                "ch2cl2",
+                "chcl3",
+                "cs2",
+                "dmf",
+                "dmso",
+                "ether",
+                "h2o",
+                "methanol",
+                "n-hexane",
+                "thf",
+                "toluene",
+            ]:
+                gfn = config["Job"].get("gfn", fallback="2")
+                if gfn != "1" and solvent.lower() in ["benzene"]:
+                    raise ValueError("%s is not a supported solvent" % solvent)
+                elif gfn != "2" and solvent.lower() in ["DMF", "n-hexane"]:
+                    raise ValueError("%s is not a supported solvent" % solvent)
+                else:
+                    raise ValueError("%s is not a supported solvent" % solvent)
+            if ref is not None and ref.lower() not in ["reference", "bar1m"]:
+                raise ValueError(
+                    "%s Gsolv reference state not supported" % ref
+                )
+            if style.lower() == "crest" or ref is None:
+                cmdline["--gbsa"] = "{}".format(solvent)
+            else:
+                cmdline["--gbsa"] = "{} {}".format(solvent, ref)
+
+        other = config["Job"].get("cmdline", fallback="").split()
+        i = 0
+        while i < len(other):
+            if other[i].startswith("-"):
+                key = other[i]
+                cmdline[key] = None
+            else:
+                cmdline[key] = other[i]
+            i += 1
+        return cmdline
+
+    def get_xcontrol(self, config, ref=None):
+        if len(self.job_type) > 1:
+            raise NotImplementedError(
+                "Multiple job types not supported for crest/xtb"
+            )
+        job_type = self.job_type[0]
+        return job_type.get_xcontrol(config, ref=ref)
```

### Comparing `AaronTools-1.0b8/utils/prime_numbers.py` & `AaronTools-1.0b9/utils/prime_numbers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 """Generates prime numbers"""
 import sys
 from math import sqrt
-from os import makedirs, path
+from os import makedirs, path, access, W_OK
 
 from AaronTools.const import AARONLIB
 
 
 class Primes:
     """
     find and cache prime numbers
@@ -16,33 +16,34 @@
     clean = False
     cache = path.join(AARONLIB, "cache", "primes.dat")
 
     def __init__(self, clean=False, cache=None):
         Primes.clean = clean
         if cache is not None:
             Primes.cache = cache
-        if Primes.clean or not path.exists(Primes.cache):
+        if Primes.clean or (not path.exists(Primes.cache) and access(Primes.cache, W_OK)):
             prime_dir, _ = path.split(Primes.cache)
             if not path.exists(prime_dir):
                 makedirs(prime_dir)
 
             with open(Primes.cache, "w") as f:
                 f.writelines([str(i) + "\n" for i in Primes.primes])
             f.close()
 
     @classmethod
     def next_prime(cls):
         """determine the next prime number"""
         # first return the ones we already found
-        with open(Primes.cache) as f:
-            for line in f:
-                prime = int(line.strip())
-                cls.primes += [prime]
-                yield prime
-        f.close()
+        if path.exists(Primes.cache):
+            with open(Primes.cache) as f:
+                for line in f:
+                    prime = int(line.strip())
+                    cls.primes += [prime]
+                    yield prime
+            f.close()
 
         # then start generating new ones
         test_prime = cls.primes[-1] + 2
         while True:
             for prime in cls.primes[1:]:
                 if test_prime % prime == 0:
                     test_prime += 2
@@ -58,14 +59,16 @@
                 cls.store_prime(test_prime)
                 yield test_prime
                 test_prime += 2
 
     @classmethod
     def store_prime(cls, prime):
         """add the prime number to the cache"""
+        if not path.exists(cls.cache):
+            return
         with open(cls.cache, "a") as f:
             if hasattr(prime, "__iter__"):
                 f.writelines([str(i) + "\n" for i in prime])
             else:
                 f.write(str(prime) + "\n")
         f.close()
```

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leb110.grid` & `AaronTools-1.0b9/utils/quad_grids/Leb110.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leb1454.grid` & `AaronTools-1.0b9/utils/quad_grids/Leb1454.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leb194.grid` & `AaronTools-1.0b9/utils/quad_grids/Leb194.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leb2030.grid` & `AaronTools-1.0b9/utils/quad_grids/Leb2030.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leb2702.grid` & `AaronTools-1.0b9/utils/quad_grids/Leb2702.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leb302.grid` & `AaronTools-1.0b9/utils/quad_grids/Leb302.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leb5810.grid` & `AaronTools-1.0b9/utils/quad_grids/Leb5810.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leb590.grid` & `AaronTools-1.0b9/utils/quad_grids/Leb590.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leb974.grid` & `AaronTools-1.0b9/utils/quad_grids/Leb974.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leg127.grid` & `AaronTools-1.0b9/utils/quad_grids/Leg127.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leg20.grid` & `AaronTools-1.0b9/utils/quad_grids/Leg20.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leg32.grid` & `AaronTools-1.0b9/utils/quad_grids/Leg32.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leg64.grid` & `AaronTools-1.0b9/utils/quad_grids/Leg64.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leg75.grid` & `AaronTools-1.0b9/utils/quad_grids/Leg75.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/Leg99.grid` & `AaronTools-1.0b9/utils/quad_grids/Leg99.grid`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/quad_grids/NOTES` & `AaronTools-1.0b9/utils/quad_grids/NOTES`

 * *Files identical despite different names*

### Comparing `AaronTools-1.0b8/utils/utils.py` & `AaronTools-1.0b9/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,44 @@
 import collections.abc
-from collections import OrderedDict
 import os
 import re
-import numpy as np
+from collections import OrderedDict
 
 import AaronTools.atoms as Atoms
-from AaronTools.const import AARONTOOLS
+import numpy as np
+from AaronTools.const import AARONTOOLS, PHYSICAL
+
+
+def range_list(number_list, sep=",", sort=True):
+    """
+    Takes a list of numbers and puts them into a string containing ranges, eg:
+    [1, 2, 3, 5, 6, 7, 9, 10] -> "1-3,5-7,9,10"
+
+    :sep: the separator to use between consecutive ranges
+    :sort: sort the list before parsing
+    """
+    if sort:
+        number_list = sorted(number_list)
+    tmp = [[]]
+    for i, n in enumerate(number_list):
+        if i == 0:
+            tmp[-1] += [n]
+        elif n == number_list[i - 1] + 1:
+            tmp[-1] += [n]
+        else:
+            tmp += [[n]]
+    rv = ""
+    for t in tmp:
+        if len(t) > 2:
+            rv += "{}-{},".format(t[0], t[-1])
+        elif len(t) == 2:
+            rv += "{},{},".format(t[0], t[-1])
+        else:
+            rv += "{},".format(t[0])
+    return rv[:-1]
 
 
 def progress_bar(this, max_num, name=None, width=50):
     if name is None:
         out_str = ""
     else:
         out_str = "{}: ".format(name)
@@ -197,14 +226,16 @@
     if a key is in d1 and d2, the items will be combined:
         if they are both dictionaries, combine_dicts is called recursively
         otherwise, d2[key] is appended to d1[key]
         if case_sensitive=False, the key in the output will be the lowercase
         of the d1 key and d2 key (only for combined items)
     dict2_conditional: bool - if True, don't add d2 keys unless they are also in d1
     """
+    from copy import deepcopy
+
     d1 = args[0]
     d2 = args[1:]
     if len(d2) > 1:
         d2 = combine_dicts(
             d2[0],
             *d2[1:],
             case_sensitive=case_sensitive,
@@ -227,27 +258,27 @@
             key.lower() if isinstance(key, str) else key for key in case_keys_2
         ]
 
     # go through keys from d1
     for case_key, key in zip(case_keys_1, keys_1):
         # if the key is only in d1, add the item to out
         if key in keys_1 and key not in keys_2:
-            out[case_key] = d1[case_key]
+            out[case_key] = deepcopy(d1[case_key])
         # if the key is in both, combine the items
         elif key in keys_1 and key in keys_2:
             key_2 = case_keys_2[keys_2.index(key)]
             if isinstance(d1[case_key], dict) and isinstance(d2[key_2], dict):
                 out[key] = combine_dicts(
                     d1[case_key],
                     d2[key_2],
                     case_sensitive=case_sensitive,
                 )
             else:
                 try:
-                    out[key] = d1[case_key] + d2[key_2]
+                    out[key] = deepcopy(d1[case_key]) + deepcopy(d2[key_2])
                 except TypeError:
                     out[key] = resolve_concatenation(d1[case_key], d2[key_2])
 
     # go through keys from d2
     if not dict2_conditional:
         for case_key, key in zip(case_keys_2, keys_2):
             # if it's only in d2, add item to out
@@ -466,15 +497,15 @@
     """rotation matrix for rotating theta radians about axis"""
     # I've only tested this for rotations in R3
     if np.linalg.norm(axis) == 0:
         axis = [1, 0, 0]
     axis = axis / np.linalg.norm(axis)
     dim = len(axis)
     outer_prod = np.dot(np.transpose([axis]), [axis])
-    outer_prod *= (1 - np.cos(theta))
+    outer_prod *= 1 - np.cos(theta)
     iden = np.identity(dim)
     cos_comp = iden * np.cos(theta)
     sin_comp = np.zeros((dim, dim))
     for i in range(0, dim):
         for j in range(0, dim):
             if i != j:
                 if (i + j) % 2 != 0:
@@ -483,15 +514,18 @@
                     p = 1
                 if i > j:
                     p = -p
                 sin_comp[i][j] = p * np.sin(theta) * axis[dim - (i + j)]
 
     return np.array(
         [
-            [outer_prod[i][j] + cos_comp[i][j] + sin_comp[i][j] for i in range(0, dim)]
+            [
+                outer_prod[i][j] + cos_comp[i][j] + sin_comp[i][j]
+                for i in range(0, dim)
+            ]
             for j in range(0, dim)
         ]
     )
 
 
 def fibonacci_sphere(radius=1, center=np.zeros(3), num=500):
     """
@@ -533,16 +567,16 @@
     # read grid data  on unit sphere
     grid_file = os.path.join(
         AARONTOOLS, "utils", "quad_grids", "Leb" + str(num) + ".grid"
     )
     if not os.path.exists(grid_file):
         # maybe some other error type?
         raise NotImplementedError(
-            "cannot use Lebedev grid with %i points\n" % num +
-            "use one of 110, 194, 302, 590, 974, 1454, 2030, 2702, 5810"
+            "cannot use Lebedev grid with %i points\n" % num
+            + "use one of 110, 194, 302, 590, 974, 1454, 2030, 2702, 5810"
         )
     grid_data = np.loadtxt(grid_file)
     grid = grid_data[:, [0, 1, 2]]
     weights = grid_data[:, 3]
 
     # scale the points to the specified radius and move the center
     grid *= radius
@@ -561,16 +595,16 @@
     # read grid points on the range [-1,1] and weights
     grid_file = os.path.join(
         AARONTOOLS, "utils", "quad_grids", "Leg" + str(num) + ".grid"
     )
     if not os.path.exists(grid_file):
         # maybe some other error type?
         raise NotImplementedError(
-            "cannot use Gauss-Legendre grid with %i points\n" % num +
-            "use one of 20, 32, 64, 75, 99, 127"
+            "cannot use Gauss-Legendre grid with %i points\n" % num
+            + "use one of 20, 32, 64, 75, 99, 127"
         )
     grid_data = np.loadtxt(grid_file)
 
     # shift grid range to [start, stop]
     grid = grid_data[:, 0] * (stop - start) / 2 + start + (stop - start) / 2
 
     # adjust weights for new range
@@ -608,19 +642,44 @@
     elif vec.ndim == 2:
         xyz = vec - np.mean(vec, axis=0)
         cov_prod = np.dot(xyz.T, xyz)
         u, s, vh = np.linalg.svd(cov_prod, compute_uv=True)
         return u[:, -1]
 
     raise NotImplementedError(
-        "cannot determine vector perpendicular to %i-dimensional array" % vec.ndim
+        "cannot determine vector perpendicular to %i-dimensional array"
+        % vec.ndim
     )
 
 
 def get_filename(path, include_parent_dir=True):
     """returns the name of the file without parent directories or extension"""
     if not include_parent_dir:
         fname = os.path.basename(path)
     else:
         fname = path
     fname, _ = os.path.splitext(fname)
     return fname
+
+
+def boltzmann_coefficients(energies, temperature):
+    """
+    returns boltzmann weights for the energies and T
+    energies - numpy array of energies in kcal/mol
+    temperature - T in K
+    """
+    min_nrg = min(energies)
+    energies -= min_nrg
+    weights = np.exp(-energies / (PHYSICAL.R * temperature))
+    return weights
+
+
+def boltzmann_average(energies, values, temperature):
+    """
+    returns the AVT result for the values corresponding to the energies
+    energies - np.array, energy for each state in kcal/mol
+    values - np.array, values that are weighted; the ith value corresponds to the ith energy
+    temperature - float, temperature in K
+    """
+    weights = boltzmann_coefficients(energies, temperature)
+    avg = np.dot(weights, values) / sum(weights)
+    return avg
```

