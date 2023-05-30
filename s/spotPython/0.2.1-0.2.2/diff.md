# Comparing `tmp/spotPython-0.2.1.tar.gz` & `tmp/spotPython-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotPython-0.2.1.tar", last modified: Mon May 29 17:35:21 2023, max compression
+gzip compressed data, was "spotPython-0.2.2.tar", last modified: Mon May 29 21:11:32 2023, max compression
```

## Comparing `spotPython-0.2.1.tar` & `spotPython-0.2.2.tar`

### file list

```diff
@@ -1,228 +1,230 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.072863 spotPython-0.2.1/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.007411 spotPython-0.2.1/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.011962 spotPython-0.2.1/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)    12811 2023-05-20 21:56:15.000000 spotPython-0.2.1/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.2.1/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.023535 spotPython-0.2.1/Figures.d/
--rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.2.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.2.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.2.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.2.1/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.2.1/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.2.1/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-29 17:35:21.072635 spotPython-0.2.1/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6577 2023-05-23 19:35:10.000000 spotPython-0.2.1/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.026333 spotPython-0.2.1/docs/
--rw-r--r--   0 bartz      (501) staff       (20)   189050 2023-05-27 21:00:53.000000 spotPython-0.2.1/docs/bart23e.html
--rw-r--r--   0 bartz      (501) staff       (20)   707240 2023-05-27 21:01:00.000000 spotPython-0.2.1/docs/bart23e.pdf
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.029944 spotPython-0.2.1/docs/figures/
--rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-19 17:04:41.000000 spotPython-0.2.1/docs/figures/parallel.png
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.030262 spotPython-0.2.1/docs/img/
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.2.1/docs/img/spotLogo.png
--rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-27 21:01:00.000000 spotPython-0.2.1/docs/index.html
--rw-r--r--   0 bartz      (501) staff       (20)    63930 2023-05-27 21:01:00.000000 spotPython-0.2.1/docs/search.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.008196 spotPython-0.2.1/docs/site_libs/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.033104 spotPython-0.2.1/docs/site_libs/bootstrap/
--rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/bootstrap/bootstrap-icons.css
--rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.2.1/docs/site_libs/bootstrap/bootstrap-icons.woff
--rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-27 21:00:51.000000 spotPython-0.2.1/docs/site_libs/bootstrap/bootstrap.min.css
--rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/bootstrap/bootstrap.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.033356 spotPython-0.2.1/docs/site_libs/clipboard/
--rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/clipboard/clipboard.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.034680 spotPython-0.2.1/docs/site_libs/quarto-html/
--rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/quarto-html/anchor.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/quarto-html/popper.min.js
--rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-23 19:54:10.000000 spotPython-0.2.1/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
--rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/quarto-html/quarto.js
--rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/quarto-html/tippy.css
--rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/quarto-html/tippy.umd.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.034900 spotPython-0.2.1/docs/site_libs/quarto-nav/
--rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/quarto-nav/quarto-nav.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.035660 spotPython-0.2.1/docs/site_libs/quarto-search/
--rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/quarto-search/autocomplete.umd.js
--rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/quarto-search/fuse.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.2.1/docs/site_libs/quarto-search/quarto-search.js
--rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-26 22:09:11.000000 spotPython-0.2.1/makeSpot.sh
--rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.2.1/mkdocs.yml
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.053310 spotPython-0.2.1/notebooks/
--rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 05:31:37.000000 spotPython-0.2.1/notebooks/00_spot_doc.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 22:27:42.000000 spotPython-0.2.1/notebooks/01_spot_intro.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 08:33:47.000000 spotPython-0.2.1/notebooks/02_spot_multidim.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 22:28:54.000000 spotPython-0.2.1/notebooks/03_spot_anisotropic.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 22:29:50.000000 spotPython-0.2.1/notebooks/04_spot_sklearn_surrogate.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 22:30:17.000000 spotPython-0.2.1/notebooks/05_spot_sklearn_optimizers.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 22:30:52.000000 spotPython-0.2.1/notebooks/06_spot_gaussian.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 22:31:54.000000 spotPython-0.2.1/notebooks/07_spot_ei.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 22:32:20.000000 spotPython-0.2.1/notebooks/08_spot_noisy.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 22:32:53.000000 spotPython-0.2.1/notebooks/09_spot_ocba.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-20 08:34:43.000000 spotPython-0.2.1/notebooks/10_spot_hpt_sklearn_classification.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    23403 2023-05-27 07:00:04.000000 spotPython-0.2.1/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    28481 2023-05-27 07:00:42.000000 spotPython-0.2.1/notebooks/12_spot_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 08:37:13.000000 spotPython-0.2.1/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   325686 2023-05-28 06:32:18.000000 spotPython-0.2.1/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 08:39:17.000000 spotPython-0.2.1/notebooks/15_spot_hpt_sklearn_regression.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)  2496232 2023-05-26 12:47:53.000000 spotPython-0.2.1/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.008406 spotPython-0.2.1/notebooks/data/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.053701 spotPython-0.2.1/notebooks/data/torch/
--rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.2.1/notebooks/data/torch/model_spot_trained.pt
--rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.2.1/notebooks/data.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.060294 spotPython-0.2.1/notebooks/figures/
--rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.2.1/notebooks/figures/spotModel.graffle
--rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.2.1/notebooks/figures/spotModel.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.2.1/notebooks/figures/spotModel.png
--rw-r--r--   0 bartz      (501) staff       (20)    21112 2023-05-22 18:09:24.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21979 2023-05-22 18:09:24.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23390 2023-05-22 18:09:24.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22172 2023-05-22 18:09:24.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23463 2023-05-22 18:09:24.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24987 2023-05-22 18:09:24.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    10009 2023-05-22 18:09:24.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7783 2023-05-22 18:09:24.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21663 2023-05-23 19:31:10.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22544 2023-05-23 19:31:10.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22042 2023-05-23 19:31:10.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21676 2023-05-23 19:31:10.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21232 2023-05-23 19:31:10.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22317 2023-05-23 19:31:10.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9376 2023-05-23 19:31:10.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6836 2023-05-23 19:31:10.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)   110037 2023-05-28 06:32:18.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png
--rw-r--r--   0 bartz      (501) staff       (20)    29542 2023-05-28 06:32:18.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    41583 2023-05-28 06:32:18.000000 spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-05-09 06:26:54.000000 spotPython-0.2.1/notebooks/plot.png
--rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-28 06:44:02.000000 spotPython-0.2.1/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-29 17:35:21.072927 spotPython-0.2.1/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.008681 spotPython-0.2.1/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.060913 spotPython-0.2.1/src/spotPython/
--rw-r--r--   0 bartz      (501) staff       (20)      194 2023-05-29 17:35:20.000000 spotPython-0.2.1/src/spotPython/_version.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.061848 spotPython-0.2.1/src/spotPython/budget/
--rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-04-13 18:20:56.000000 spotPython-0.2.1/src/spotPython/budget/ocba.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.062162 spotPython-0.2.1/src/spotPython/build/
--rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-13 19:26:45.000000 spotPython-0.2.1/src/spotPython/build/kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.2.1/src/spotPython/build/surrogates.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.063578 spotPython-0.2.1/src/spotPython/data/
--rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.2.1/src/spotPython/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.2.1/src/spotPython/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-20 18:34:33.000000 spotPython-0.2.1/src/spotPython/data/sklearn_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.2.1/src/spotPython/data/sklearn_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     5171 2023-05-29 06:45:28.000000 spotPython-0.2.1/src/spotPython/data/torch_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.2.1/src/spotPython/data/torch_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)      459 2023-05-28 07:19:43.000000 spotPython-0.2.1/src/spotPython/data/torchdata.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.064162 spotPython-0.2.1/src/spotPython/design/
--rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.2.1/src/spotPython/design/designs.py
--rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.2.1/src/spotPython/design/factorial.py
--rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.2.1/src/spotPython/design/spacefilling.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.064598 spotPython-0.2.1/src/spotPython/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     6273 2023-05-26 12:49:30.000000 spotPython-0.2.1/src/spotPython/fun/hypersklearn.py
--rw-r--r--   0 bartz      (501) staff       (20)     4911 2023-05-27 18:18:59.000000 spotPython-0.2.1/src/spotPython/fun/hypertorch.py
--rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-06 16:12:25.000000 spotPython-0.2.1/src/spotPython/fun/objectivefunctions.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.065093 spotPython-0.2.1/src/spotPython/hyperparameters/
--rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.2.1/src/spotPython/hyperparameters/categorical.py
--rw-r--r--   0 bartz      (501) staff       (20)     4137 2023-05-27 19:48:36.000000 spotPython-0.2.1/src/spotPython/hyperparameters/optimizer.py
--rw-r--r--   0 bartz      (501) staff       (20)    26033 2023-05-28 07:22:58.000000 spotPython-0.2.1/src/spotPython/hyperparameters/values.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.065369 spotPython-0.2.1/src/spotPython/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-05-29 06:13:03.000000 spotPython-0.2.1/src/spotPython/plot/contour.py
--rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 08:41:56.000000 spotPython-0.2.1/src/spotPython/plot/validation.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.065516 spotPython-0.2.1/src/spotPython/spot/
--rw-r--r--   0 bartz      (501) staff       (20)    33049 2023-05-29 06:29:51.000000 spotPython-0.2.1/src/spotPython/spot/spot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.066076 spotPython-0.2.1/src/spotPython/torch/
--rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.2.1/src/spotPython/torch/netcifar10.py
--rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.2.1/src/spotPython/torch/netcore.py
--rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.2.1/src/spotPython/torch/netfashionMNIST.py
--rw-r--r--   0 bartz      (501) staff       (20)    13380 2023-05-27 19:18:58.000000 spotPython-0.2.1/src/spotPython/torch/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.067614 spotPython-0.2.1/src/spotPython/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.2.1/src/spotPython/utils/aggregate.py
--rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.2.1/src/spotPython/utils/classes.py
--rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.2.1/src/spotPython/utils/compare.py
--rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 08:44:33.000000 spotPython-0.2.1/src/spotPython/utils/convert.py
--rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-07 19:27:47.000000 spotPython-0.2.1/src/spotPython/utils/device.py
--rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-09 21:08:48.000000 spotPython-0.2.1/src/spotPython/utils/eda.py
--rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 18:22:38.000000 spotPython-0.2.1/src/spotPython/utils/file.py
--rw-r--r--   0 bartz      (501) staff       (20)     1445 2023-05-28 07:30:22.000000 spotPython-0.2.1/src/spotPython/utils/init.py
--rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-20 20:12:12.000000 spotPython-0.2.1/src/spotPython/utils/metrics.py
--rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-13 18:37:01.000000 spotPython-0.2.1/src/spotPython/utils/progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.2.1/src/spotPython/utils/repair.py
--rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-09 23:09:07.000000 spotPython-0.2.1/src/spotPython/utils/transform.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.061684 spotPython-0.2.1/src/spotPython.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-29 17:35:20.000000 spotPython-0.2.1/src/spotPython.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)    10231 2023-05-29 17:35:21.000000 spotPython-0.2.1/src/spotPython.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-29 17:35:20.000000 spotPython-0.2.1/src/spotPython.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-29 17:35:20.000000 spotPython-0.2.1/src/spotPython.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-29 17:35:20.000000 spotPython-0.2.1/src/spotPython.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 17:35:21.072234 spotPython-0.2.1/test/
--rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_aggregate_mean_var.py
--rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.2.1/test/test_build_Psi.py
--rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.2.1/test/test_build_U.py
--rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_build_psi_vec.py
--rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_evaluate_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_evaluate_new_solutions.py
--rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.2.1/test/test_extract_from_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_generate_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_infill.py
--rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_nat_to_cod.py
--rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_nat_to_cod_init.py
--rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_ocba.py
--rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_repair_non_numeric.py
--rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_set_de_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_show_progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_suggest_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.2.1/test/test_update_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.2.1/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.104379 spotPython-0.2.2/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.038337 spotPython-0.2.2/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.043097 spotPython-0.2.2/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)    12811 2023-05-20 21:56:15.000000 spotPython-0.2.2/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.2.2/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.053714 spotPython-0.2.2/Figures.d/
+-rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.2.2/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.2.2/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.2.2/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.2.2/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.2.2/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.2.2/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-29 21:11:32.104196 spotPython-0.2.2/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6577 2023-05-23 19:35:10.000000 spotPython-0.2.2/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.055854 spotPython-0.2.2/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)   208086 2023-05-29 18:21:43.000000 spotPython-0.2.2/docs/bart23e.html
+-rw-r--r--   0 bartz      (501) staff       (20)   713146 2023-05-29 18:21:50.000000 spotPython-0.2.2/docs/bart23e.pdf
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.059191 spotPython-0.2.2/docs/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-19 17:04:41.000000 spotPython-0.2.2/docs/figures/parallel.png
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.059457 spotPython-0.2.2/docs/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.2.2/docs/img/spotLogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-29 18:21:50.000000 spotPython-0.2.2/docs/index.html
+-rw-r--r--   0 bartz      (501) staff       (20)    64921 2023-05-29 18:21:50.000000 spotPython-0.2.2/docs/search.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.039165 spotPython-0.2.2/docs/site_libs/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.061517 spotPython-0.2.2/docs/site_libs/bootstrap/
+-rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.2.2/docs/site_libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-29 18:21:41.000000 spotPython-0.2.2/docs/site_libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/bootstrap/bootstrap.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.061797 spotPython-0.2.2/docs/site_libs/clipboard/
+-rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/clipboard/clipboard.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.063604 spotPython-0.2.2/docs/site_libs/quarto-html/
+-rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/quarto-html/anchor.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/quarto-html/popper.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-23 19:54:10.000000 spotPython-0.2.2/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/quarto-html/quarto.js
+-rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/quarto-html/tippy.css
+-rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/quarto-html/tippy.umd.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.063820 spotPython-0.2.2/docs/site_libs/quarto-nav/
+-rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/quarto-nav/quarto-nav.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.064571 spotPython-0.2.2/docs/site_libs/quarto-search/
+-rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/quarto-search/autocomplete.umd.js
+-rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/quarto-search/fuse.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.2.2/docs/site_libs/quarto-search/quarto-search.js
+-rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-26 22:09:11.000000 spotPython-0.2.2/makeSpot.sh
+-rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.2.2/mkdocs.yml
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.079098 spotPython-0.2.2/notebooks/
+-rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 05:31:37.000000 spotPython-0.2.2/notebooks/00_spot_doc.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 22:27:42.000000 spotPython-0.2.2/notebooks/01_spot_intro.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 08:33:47.000000 spotPython-0.2.2/notebooks/02_spot_multidim.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 22:28:54.000000 spotPython-0.2.2/notebooks/03_spot_anisotropic.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 22:29:50.000000 spotPython-0.2.2/notebooks/04_spot_sklearn_surrogate.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 22:30:17.000000 spotPython-0.2.2/notebooks/05_spot_sklearn_optimizers.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 22:30:52.000000 spotPython-0.2.2/notebooks/06_spot_gaussian.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 22:31:54.000000 spotPython-0.2.2/notebooks/07_spot_ei.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 22:32:20.000000 spotPython-0.2.2/notebooks/08_spot_noisy.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 22:32:53.000000 spotPython-0.2.2/notebooks/09_spot_ocba.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-20 08:34:43.000000 spotPython-0.2.2/notebooks/10_spot_hpt_sklearn_classification.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    23403 2023-05-27 07:00:04.000000 spotPython-0.2.2/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    28481 2023-05-27 07:00:42.000000 spotPython-0.2.2/notebooks/12_spot_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 08:37:13.000000 spotPython-0.2.2/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   110777 2023-05-29 18:53:06.000000 spotPython-0.2.2/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 08:39:17.000000 spotPython-0.2.2/notebooks/15_spot_hpt_sklearn_regression.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    50940 2023-05-29 21:11:19.000000 spotPython-0.2.2/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.039407 spotPython-0.2.2/notebooks/data/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.079532 spotPython-0.2.2/notebooks/data/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.2.2/notebooks/data/torch/model_spot_trained.pt
+-rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.2.2/notebooks/data.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.086951 spotPython-0.2.2/notebooks/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.2.2/notebooks/figures/spotModel.graffle
+-rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.2.2/notebooks/figures/spotModel.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.2.2/notebooks/figures/spotModel.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21112 2023-05-22 18:09:24.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21979 2023-05-22 18:09:24.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23390 2023-05-22 18:09:24.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22172 2023-05-22 18:09:24.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23463 2023-05-22 18:09:24.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24987 2023-05-22 18:09:24.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    10009 2023-05-22 18:09:24.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7783 2023-05-22 18:09:24.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21663 2023-05-23 19:31:10.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22544 2023-05-23 19:31:10.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22042 2023-05-23 19:31:10.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21676 2023-05-23 19:31:10.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21232 2023-05-23 19:31:10.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22317 2023-05-23 19:31:10.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9376 2023-05-23 19:31:10.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6836 2023-05-23 19:31:10.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)   110037 2023-05-28 06:32:18.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png
+-rw-r--r--   0 bartz      (501) staff       (20)    29542 2023-05-28 06:32:18.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    41583 2023-05-28 06:32:18.000000 spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-05-09 06:26:54.000000 spotPython-0.2.2/notebooks/plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-29 19:13:55.000000 spotPython-0.2.2/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-29 21:11:32.104436 spotPython-0.2.2/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.039686 spotPython-0.2.2/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.087518 spotPython-0.2.2/src/spotPython/
+-rw-r--r--   0 bartz      (501) staff       (20)      214 2023-05-29 21:11:31.000000 spotPython-0.2.2/src/spotPython/_version.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.088443 spotPython-0.2.2/src/spotPython/budget/
+-rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-04-13 18:20:56.000000 spotPython-0.2.2/src/spotPython/budget/ocba.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.089206 spotPython-0.2.2/src/spotPython/build/
+-rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-13 19:26:45.000000 spotPython-0.2.2/src/spotPython/build/kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.2.2/src/spotPython/build/surrogates.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.091405 spotPython-0.2.2/src/spotPython/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.2.2/src/spotPython/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.2.2/src/spotPython/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-20 18:34:33.000000 spotPython-0.2.2/src/spotPython/data/sklearn_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.2.2/src/spotPython/data/sklearn_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5171 2023-05-29 06:45:28.000000 spotPython-0.2.2/src/spotPython/data/torch_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.2.2/src/spotPython/data/torch_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)      459 2023-05-28 07:19:43.000000 spotPython-0.2.2/src/spotPython/data/torchdata.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.092186 spotPython-0.2.2/src/spotPython/design/
+-rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.2.2/src/spotPython/design/designs.py
+-rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.2.2/src/spotPython/design/factorial.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.2.2/src/spotPython/design/spacefilling.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.092969 spotPython-0.2.2/src/spotPython/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     3794 2023-05-29 20:49:36.000000 spotPython-0.2.2/src/spotPython/fun/hypersklearn.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4911 2023-05-27 18:18:59.000000 spotPython-0.2.2/src/spotPython/fun/hypertorch.py
+-rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-06 16:12:25.000000 spotPython-0.2.2/src/spotPython/fun/objectivefunctions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.093841 spotPython-0.2.2/src/spotPython/hyperparameters/
+-rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.2.2/src/spotPython/hyperparameters/categorical.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4137 2023-05-27 19:48:36.000000 spotPython-0.2.2/src/spotPython/hyperparameters/optimizer.py
+-rw-r--r--   0 bartz      (501) staff       (20)    26033 2023-05-28 07:22:58.000000 spotPython-0.2.2/src/spotPython/hyperparameters/values.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.094464 spotPython-0.2.2/src/spotPython/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-05-29 06:13:03.000000 spotPython-0.2.2/src/spotPython/plot/contour.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 08:41:56.000000 spotPython-0.2.2/src/spotPython/plot/validation.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.094776 spotPython-0.2.2/src/spotPython/sklearn/
+-rw-r--r--   0 bartz      (501) staff       (20)     3711 2023-05-29 20:57:16.000000 spotPython-0.2.2/src/spotPython/sklearn/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.095052 spotPython-0.2.2/src/spotPython/spot/
+-rw-r--r--   0 bartz      (501) staff       (20)    33049 2023-05-29 06:29:51.000000 spotPython-0.2.2/src/spotPython/spot/spot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.096265 spotPython-0.2.2/src/spotPython/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.2.2/src/spotPython/torch/netcifar10.py
+-rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.2.2/src/spotPython/torch/netcore.py
+-rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.2.2/src/spotPython/torch/netfashionMNIST.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13380 2023-05-27 19:18:58.000000 spotPython-0.2.2/src/spotPython/torch/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.099460 spotPython-0.2.2/src/spotPython/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.2.2/src/spotPython/utils/aggregate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.2.2/src/spotPython/utils/classes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.2.2/src/spotPython/utils/compare.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 08:44:33.000000 spotPython-0.2.2/src/spotPython/utils/convert.py
+-rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-07 19:27:47.000000 spotPython-0.2.2/src/spotPython/utils/device.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-09 21:08:48.000000 spotPython-0.2.2/src/spotPython/utils/eda.py
+-rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 18:22:38.000000 spotPython-0.2.2/src/spotPython/utils/file.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1445 2023-05-28 07:30:22.000000 spotPython-0.2.2/src/spotPython/utils/init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-20 20:12:12.000000 spotPython-0.2.2/src/spotPython/utils/metrics.py
+-rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-13 18:37:01.000000 spotPython-0.2.2/src/spotPython/utils/progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.2.2/src/spotPython/utils/repair.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-09 23:09:07.000000 spotPython-0.2.2/src/spotPython/utils/transform.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.088281 spotPython-0.2.2/src/spotPython.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-29 21:11:31.000000 spotPython-0.2.2/src/spotPython.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)    10267 2023-05-29 21:11:32.000000 spotPython-0.2.2/src/spotPython.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-29 21:11:31.000000 spotPython-0.2.2/src/spotPython.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-29 21:11:31.000000 spotPython-0.2.2/src/spotPython.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-29 21:11:31.000000 spotPython-0.2.2/src/spotPython.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-29 21:11:32.103894 spotPython-0.2.2/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_aggregate_mean_var.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.2.2/test/test_build_Psi.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.2.2/test/test_build_U.py
+-rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_build_psi_vec.py
+-rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_evaluate_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_evaluate_new_solutions.py
+-rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.2.2/test/test_extract_from_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_generate_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_infill.py
+-rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_nat_to_cod.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_nat_to_cod_init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_ocba.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_repair_non_numeric.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_set_de_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_show_progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_suggest_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.2.2/test/test_update_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.2.2/tox.ini
```

### Comparing `spotPython-0.2.1/.github/workflows/test.yml` & `spotPython-0.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/.gitignore` & `spotPython-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf` & `spotPython-0.2.2/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf` & `spotPython-0.2.2/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf` & `spotPython-0.2.2/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf` & `spotPython-0.2.2/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf` & `spotPython-0.2.2/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf` & `spotPython-0.2.2/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/LICENSE.txt` & `spotPython-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/PKG-INFO` & `spotPython-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.2.1
+Version: 0.2.2
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.2.1/README.md` & `spotPython-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/bart23e.html` & `spotPython-0.2.2/docs/bart23e.html`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     <div class="quarto-alternate-formats"><h2>Other Formats</h2><ul><li><a href="bart23e.pdf"><i class="bi bi-file-pdf"></i>PDF</a></li></ul></div></div>
 <!-- main -->
 <main class="content" id="quarto-document-content">
 
 <header id="title-block-header" class="quarto-title-block default">
 <div class="quarto-title">
 <h1 class="title">PyTorch Hyperparameter Tuning — A Tutorial for spotPython</h1>
-<p class="subtitle lead">Version 0.2.0</p>
+<p class="subtitle lead">Version 0.2.1</p>
 </div>
 
 
 <div class="quarto-title-meta-author">
   <div class="quarto-title-meta-heading">Author</div>
   <div class="quarto-title-meta-heading">Affiliations</div>
   
@@ -172,15 +172,15 @@
 </header>
 
 <section id="sec-hyperparameter-tuning" class="level1">
 <h1>Hyperparameter Tuning</h1>
 <p>Hyperparameter tuning is an important, but often difficult and computationally intensive task. Changing the architecture of a neural network or the learning rate of an optimizer can have a significant impact on the performance.</p>
 <p>The goal of hyperparameter tuning is to optimize the hyperparameters in a way that improves the performance of the machine learning or deep learning model. The simplest, but also most computationally expensive, approach uses manual search (or trial-and-error <span class="citation" data-cites="Meignan:2015vp">(<a href="#ref-Meignan:2015vp" role="doc-biblioref">Meignan et al. 2015</a>)</span>). Commonly encountered is simple random search, i.e., random and repeated selection of hyperparameters for evaluation, and lattice search (“grid search”). In addition, methods that perform directed search and other model-free algorithms, i.e., algorithms that do not explicitly rely on a model, e.g., evolution strategies <span class="citation" data-cites="Bart13j">(<a href="#ref-Bart13j" role="doc-biblioref">Bartz-Beielstein et al. 2014</a>)</span> or pattern search <span class="citation" data-cites="Torczon00">(<a href="#ref-Torczon00" role="doc-biblioref">Lewis, Torczon, and Trosset 2000</a>)</span> play an important role. Also, “hyperband”, i.e., a multi-armed bandit strategy that dynamically allocates resources to a set of random configurations and uses successive bisections to stop configurations with poor performance <span class="citation" data-cites="Li16a">(<a href="#ref-Li16a" role="doc-biblioref">Li et al. 2016</a>)</span>, is very common in hyperparameter tuning. The most sophisticated and efficient approaches are the Bayesian optimization and surrogate model based optimization methods, which are based on the optimization of cost functions determined by simulations or experiments.</p>
 <p>We consider below a surrogate model based optimization-based hyperparameter tuning approach based on the Python version of the SPOT (“Sequential Parameter Optimization Toolbox”) <span class="citation" data-cites="BLP05">(<a href="#ref-BLP05" role="doc-biblioref">Bartz-Beielstein, Lasarczyk, and Preuss 2005</a>)</span>, which is suitable for situations where only limited resources are available. This may be due to limited availability and cost of hardware, or due to the fact that confidential data may only be processed locally, e.g., due to legal requirements. Furthermore, in our approach, the understanding of algorithms is seen as a key tool for enabling transparency and explainability. This can be enabled, for example, by quantifying the contribution of machine learning and deep learning components (nodes, layers, split decisions, activation functions, etc.). Understanding the importance of hyperparameters and the interactions between multiple hyperparameters plays a major role in the interpretability and explainability of machine learning models. SPOT provides statistical tools for understanding hyperparameters and their interactions. Last but not least, it should be noted that the SPOT software code is available in the open source <code>spotPython</code> package on github<a href="#fn1" class="footnote-ref" id="fnref1" role="doc-noteref"><sup>1</sup></a>, allowing replicability of the results. This tutorial descries the Python variant of SPOT, which is called <code>spotPython</code>. The R implementation is described in <span class="citation" data-cites="bart21i">Bartz et al. (<a href="#ref-bart21i" role="doc-biblioref">2022</a>)</span>. SPOT is an established open source software that has been maintained for more than 15 years <span class="citation" data-cites="BLP05">(<a href="#ref-BLP05" role="doc-biblioref">Bartz-Beielstein, Lasarczyk, and Preuss 2005</a>)</span> <span class="citation" data-cites="bart21i">(<a href="#ref-bart21i" role="doc-biblioref">Bartz et al. 2022</a>)</span>.</p>
-<p>This tutorial is structured as follows. The concept of the hyperparameter tuning software <code>spotPython</code> is described in <a href="#sec-spot">Section&nbsp;2</a>. <a href="#sec-hyperparameter-tuning-for-pytorch">Section&nbsp;3</a> describes the integration of <code>spotPython</code> into the <code>PyTorch</code> training workflow and presents the results. Finally, <a href="#sec-summary">Section&nbsp;4</a> presents a summary and an outlook.</p>
+<p>This tutorial is structured as follows. The concept of the hyperparameter tuning software <code>spotPython</code> is described in <a href="#sec-spot">Section&nbsp;2</a>. <a href="#sec-quickstart">Section&nbsp;3</a> (“Quickstart”) describes the execution of the example from the tutorial “Hyperparameter Tuning with Ray Tune” <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span>. <a href="#sec-hyperparameter-tuning-for-pytorch">Section&nbsp;4</a> describes the integration of <code>spotPython</code> into the <code>PyTorch</code> training workflow in detail and presents the results. Finally, <a href="#sec-summary">Section&nbsp;5</a> presents a summary and an outlook.</p>
 <div class="callout callout-style-default callout-note callout-titled">
 <div class="callout-header d-flex align-content-center">
 <div class="callout-icon-container">
 <i class="callout-icon"></i>
 </div>
 <div class="callout-title-container flex-fill">
 Note
@@ -193,83 +193,214 @@
 </section>
 <section id="sec-spot" class="level1">
 <h1>The Hyperparameter Tuning Software SPOT</h1>
 <p>Surrogate model based optimization methods are common approaches in simulation and optimization. SPOT was developed because there is a great need for sound statistical analysis of simulation and optimization algorithms. SPOT includes methods for tuning based on classical regression and analysis of variance techniques. It presents tree-based models such as classification and regression trees and random forests as well as Bayesian optimization (Gaussian process models, also known as Kriging). Combinations of different meta-modeling approaches are possible. SPOT comes with a sophisticated surrogate model based optimization method, that can handle discrete and continuous inputs. Furthermore, any model implemented in <code>scikit-learn</code> can be used out-of-the-box as a surrogate in <code>spotPython</code>.</p>
 <p>SPOT implements key techniques such as exploratory fitness landscape analysis and sensitivity analysis. It can be used to understand the performance of various algorithms, while simultaneously giving insights into their algorithmic behavior. In addition, SPOT can be used as an optimizer and for automatic and interactive tuning. Details on SPOT and its use in practice are given by <span class="citation" data-cites="bart21i">Bartz et al. (<a href="#ref-bart21i" role="doc-biblioref">2022</a>)</span>.</p>
 <p>A typical hyperparameter tuning process with <code>spotPython</code> consists of the following steps:</p>
 <ol type="1">
-<li>Loading the data (training and test datasets), see <a href="#sec-data-loading">Section&nbsp;3.3</a>.</li>
-<li>Specification of the preprocessing model, see <a href="#sec-specification-of-preprocessing-model">Section&nbsp;3.4</a>. This model is called <code>prep_model</code> (“preparation” or pre-processing). The information required for the hyperparameter tuning is stored in the dictionary <code>fun_control</code>. Thus, the information needed for the execution of the hyperparameter tuning is available in a readable form.</li>
-<li>Selection of the machine learning or deep learning model to be tuned, see <a href="#sec-selection-of-the-algorithm">Section&nbsp;3.5</a>. This is called the <code>core_model</code>. Once the <code>core_model</code> is defined, then the associated hyperparameters are stored in the <code>fun_control</code> dictionary. First, the hyperparameters of the <code>core_model</code> are initialized with the default values of the <code>core_model</code>. As default values we use the default values contained in the <code>spotPython</code> package for the algorithms of the <code>torch</code> package.</li>
-<li>Modification of the default values for the hyperparameters used in <code>core_model</code>, see <a href="#sec-modification-of-default-values">Section&nbsp;3.7.1</a>. This step is optional.
+<li>Loading the data (training and test datasets), see <a href="#sec-data-loading">Section&nbsp;4.3</a>.</li>
+<li>Specification of the preprocessing model, see <a href="#sec-specification-of-preprocessing-model">Section&nbsp;4.4</a>. This model is called <code>prep_model</code> (“preparation” or pre-processing). The information required for the hyperparameter tuning is stored in the dictionary <code>fun_control</code>. Thus, the information needed for the execution of the hyperparameter tuning is available in a readable form.</li>
+<li>Selection of the machine learning or deep learning model to be tuned, see <a href="#sec-selection-of-the-algorithm">Section&nbsp;4.5</a>. This is called the <code>core_model</code>. Once the <code>core_model</code> is defined, then the associated hyperparameters are stored in the <code>fun_control</code> dictionary. First, the hyperparameters of the <code>core_model</code> are initialized with the default values of the <code>core_model</code>. As default values we use the default values contained in the <code>spotPython</code> package for the algorithms of the <code>torch</code> package.</li>
+<li>Modification of the default values for the hyperparameters used in <code>core_model</code>, see <a href="#sec-modification-of-default-values">Section&nbsp;4.7.1</a>. This step is optional.
 <ol type="1">
 <li>numeric parameters are modified by changing the bounds.</li>
 <li>categorical parameters are modified by changing the categories (“levels”).</li>
 </ol></li>
-<li>Selection of target function (loss function) for the optimizer, see <a href="#sec-selection-of-target-function">Section&nbsp;3.8</a>.</li>
-<li>Calling SPOT with the corresponding parameters, see <a href="#sec-call-the-hyperparameter-tuner">Section&nbsp;3.9</a>. The results are stored in a dictionary and are available for further analysis.</li>
-<li>Presentation, visualization and interpretation of the results, see <a href="#sec-results-tuning">Section&nbsp;3.10</a>.</li>
+<li>Selection of target function (loss function) for the optimizer, see <a href="#sec-selection-of-target-function">Section&nbsp;4.8</a>.</li>
+<li>Calling SPOT with the corresponding parameters, see <a href="#sec-call-the-hyperparameter-tuner">Section&nbsp;4.9</a>. The results are stored in a dictionary and are available for further analysis.</li>
+<li>Presentation, visualization and interpretation of the results, see <a href="#sec-results-tuning">Section&nbsp;4.10</a>.</li>
 </ol>
 </section>
+<section id="sec-quickstart" class="level1">
+<h1>Quickstart</h1>
+<div class="cell" data-execution_count="1">
+<div class="sourceCode cell-code" id="cb1"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb1-1"><a href="#cb1-1" aria-hidden="true" tabindex="-1"></a><span class="im">import</span> numpy <span class="im">as</span> np</span>
+<span id="cb1-2"><a href="#cb1-2" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> math <span class="im">import</span> inf</span>
+<span id="cb1-3"><a href="#cb1-3" aria-hidden="true" tabindex="-1"></a><span class="im">import</span> torchmetrics</span>
+<span id="cb1-4"><a href="#cb1-4" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> torch.nn <span class="im">import</span> CrossEntropyLoss</span>
+<span id="cb1-5"><a href="#cb1-5" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.spot <span class="im">import</span> spot</span>
+<span id="cb1-6"><a href="#cb1-6" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.utils.init <span class="im">import</span> fun_control_init</span>
+<span id="cb1-7"><a href="#cb1-7" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.data.torchdata <span class="im">import</span> load_data_cifar10</span>
+<span id="cb1-8"><a href="#cb1-8" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.hyperparameters.values <span class="im">import</span> (</span>
+<span id="cb1-9"><a href="#cb1-9" aria-hidden="true" tabindex="-1"></a>    add_core_model_to_fun_control,</span>
+<span id="cb1-10"><a href="#cb1-10" aria-hidden="true" tabindex="-1"></a>    modify_hyper_parameter_levels,</span>
+<span id="cb1-11"><a href="#cb1-11" aria-hidden="true" tabindex="-1"></a>    modify_hyper_parameter_bounds,</span>
+<span id="cb1-12"><a href="#cb1-12" aria-hidden="true" tabindex="-1"></a>    get_var_type,</span>
+<span id="cb1-13"><a href="#cb1-13" aria-hidden="true" tabindex="-1"></a>    get_var_name,</span>
+<span id="cb1-14"><a href="#cb1-14" aria-hidden="true" tabindex="-1"></a>    get_bound_values,</span>
+<span id="cb1-15"><a href="#cb1-15" aria-hidden="true" tabindex="-1"></a>    get_one_core_model_from_X,</span>
+<span id="cb1-16"><a href="#cb1-16" aria-hidden="true" tabindex="-1"></a>    get_default_hyperparameters_as_array</span>
+<span id="cb1-17"><a href="#cb1-17" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb1-18"><a href="#cb1-18" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.data.torch_hyper_dict <span class="im">import</span> TorchHyperDict</span>
+<span id="cb1-19"><a href="#cb1-19" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.data.torchdata <span class="im">import</span> load_data_cifar10</span>
+<span id="cb1-20"><a href="#cb1-20" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.fun.hypertorch <span class="im">import</span> HyperTorch</span>
+<span id="cb1-21"><a href="#cb1-21" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.torch.netcifar10 <span class="im">import</span> Net_CIFAR10</span>
+<span id="cb1-22"><a href="#cb1-22" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.torch.traintest <span class="im">import</span> (</span>
+<span id="cb1-23"><a href="#cb1-23" aria-hidden="true" tabindex="-1"></a>    train_tuned,</span>
+<span id="cb1-24"><a href="#cb1-24" aria-hidden="true" tabindex="-1"></a>    test_tuned,</span>
+<span id="cb1-25"><a href="#cb1-25" aria-hidden="true" tabindex="-1"></a>    )</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<div class="cell" data-execution_count="2">
+<div class="sourceCode cell-code" id="cb2"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb2-1"><a href="#cb2-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> fun_control_init()</span>
+<span id="cb2-2"><a href="#cb2-2" aria-hidden="true" tabindex="-1"></a><span class="co"># load data</span></span>
+<span id="cb2-3"><a href="#cb2-3" aria-hidden="true" tabindex="-1"></a>train, test <span class="op">=</span> load_data_cifar10()</span>
+<span id="cb2-4"><a href="#cb2-4" aria-hidden="true" tabindex="-1"></a><span class="co"># add the dataset to the fun_control</span></span>
+<span id="cb2-5"><a href="#cb2-5" aria-hidden="true" tabindex="-1"></a>fun_control.update({</span>
+<span id="cb2-6"><a href="#cb2-6" aria-hidden="true" tabindex="-1"></a>    <span class="st">"train"</span>: train,</span>
+<span id="cb2-7"><a href="#cb2-7" aria-hidden="true" tabindex="-1"></a>    <span class="st">"test"</span>: test,</span>
+<span id="cb2-8"><a href="#cb2-8" aria-hidden="true" tabindex="-1"></a>    <span class="st">"n_samples"</span>: <span class="bu">len</span>(train)})</span>
+<span id="cb2-9"><a href="#cb2-9" aria-hidden="true" tabindex="-1"></a><span class="co"># add the nn model to the fun_control dictionary</span></span>
+<span id="cb2-10"><a href="#cb2-10" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> add_core_model_to_fun_control(core_model<span class="op">=</span>Net_CIFAR10,</span>
+<span id="cb2-11"><a href="#cb2-11" aria-hidden="true" tabindex="-1"></a>                              fun_control<span class="op">=</span>fun_control,</span>
+<span id="cb2-12"><a href="#cb2-12" aria-hidden="true" tabindex="-1"></a>                              hyper_dict<span class="op">=</span>TorchHyperDict)</span>
+<span id="cb2-13"><a href="#cb2-13" aria-hidden="true" tabindex="-1"></a><span class="co"># modify the hyperparameter levels</span></span>
+<span id="cb2-14"><a href="#cb2-14" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"lr_mult"</span>, bounds<span class="op">=</span>[<span class="fl">1e-3</span>, <span class="fl">1e-3</span>])</span>
+<span id="cb2-15"><a href="#cb2-15" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"sgd_momentum"</span>, bounds<span class="op">=</span>[<span class="fl">0.9</span>, <span class="fl">0.9</span>])</span>
+<span id="cb2-16"><a href="#cb2-16" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>,[<span class="st">"Adam"</span>, <span class="st">"SGD"</span>])</span>
+<span id="cb2-17"><a href="#cb2-17" aria-hidden="true" tabindex="-1"></a><span class="co"># select metric and loss function</span></span>
+<span id="cb2-18"><a href="#cb2-18" aria-hidden="true" tabindex="-1"></a>fun_control.update({</span>
+<span id="cb2-19"><a href="#cb2-19" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_torch"</span>: torchmetrics.Accuracy(task<span class="op">=</span><span class="st">"multiclass"</span>, num_classes<span class="op">=</span><span class="dv">10</span>),</span>
+<span id="cb2-20"><a href="#cb2-20" aria-hidden="true" tabindex="-1"></a>               <span class="st">"loss_function"</span>: CrossEntropyLoss(),</span>
+<span id="cb2-21"><a href="#cb2-21" aria-hidden="true" tabindex="-1"></a>               <span class="st">"device"</span>: <span class="st">"cpu"</span>,</span>
+<span id="cb2-22"><a href="#cb2-22" aria-hidden="true" tabindex="-1"></a>               })</span>
+<span id="cb2-23"><a href="#cb2-23" aria-hidden="true" tabindex="-1"></a><span class="co"># extract the variable types, names, and bounds</span></span>
+<span id="cb2-24"><a href="#cb2-24" aria-hidden="true" tabindex="-1"></a>var_type <span class="op">=</span> get_var_type(fun_control)</span>
+<span id="cb2-25"><a href="#cb2-25" aria-hidden="true" tabindex="-1"></a>var_name <span class="op">=</span> get_var_name(fun_control)</span>
+<span id="cb2-26"><a href="#cb2-26" aria-hidden="true" tabindex="-1"></a>fun_control.update({<span class="st">"var_type"</span>: var_type,</span>
+<span id="cb2-27"><a href="#cb2-27" aria-hidden="true" tabindex="-1"></a>                    <span class="st">"var_name"</span>: var_name})</span>
+<span id="cb2-28"><a href="#cb2-28" aria-hidden="true" tabindex="-1"></a>lower <span class="op">=</span> get_bound_values(fun_control, <span class="st">"lower"</span>)</span>
+<span id="cb2-29"><a href="#cb2-29" aria-hidden="true" tabindex="-1"></a>upper <span class="op">=</span> get_bound_values(fun_control, <span class="st">"upper"</span>)</span>
+<span id="cb2-30"><a href="#cb2-30" aria-hidden="true" tabindex="-1"></a></span>
+<span id="cb2-31"><a href="#cb2-31" aria-hidden="true" tabindex="-1"></a><span class="co"># get the default hyperparameters as array</span></span>
+<span id="cb2-32"><a href="#cb2-32" aria-hidden="true" tabindex="-1"></a>hyper_dict<span class="op">=</span>TorchHyperDict().load()</span>
+<span id="cb2-33"><a href="#cb2-33" aria-hidden="true" tabindex="-1"></a>X_start <span class="op">=</span> get_default_hyperparameters_as_array(fun_control, hyper_dict)</span>
+<span id="cb2-34"><a href="#cb2-34" aria-hidden="true" tabindex="-1"></a></span>
+<span id="cb2-35"><a href="#cb2-35" aria-hidden="true" tabindex="-1"></a><span class="co"># get the objective function</span></span>
+<span id="cb2-36"><a href="#cb2-36" aria-hidden="true" tabindex="-1"></a>fun <span class="op">=</span> HyperTorch().fun_torch</span>
+<span id="cb2-37"><a href="#cb2-37" aria-hidden="true" tabindex="-1"></a></span>
+<span id="cb2-38"><a href="#cb2-38" aria-hidden="true" tabindex="-1"></a><span class="co"># initialize spot</span></span>
+<span id="cb2-39"><a href="#cb2-39" aria-hidden="true" tabindex="-1"></a>spot_tuner <span class="op">=</span> spot.Spot(fun<span class="op">=</span>fun,</span>
+<span id="cb2-40"><a href="#cb2-40" aria-hidden="true" tabindex="-1"></a>                   lower <span class="op">=</span> lower,</span>
+<span id="cb2-41"><a href="#cb2-41" aria-hidden="true" tabindex="-1"></a>                   upper <span class="op">=</span> upper,</span>
+<span id="cb2-42"><a href="#cb2-42" aria-hidden="true" tabindex="-1"></a>                   fun_evals <span class="op">=</span> inf,</span>
+<span id="cb2-43"><a href="#cb2-43" aria-hidden="true" tabindex="-1"></a>                   fun_repeats <span class="op">=</span> <span class="dv">1</span>,</span>
+<span id="cb2-44"><a href="#cb2-44" aria-hidden="true" tabindex="-1"></a>                   max_time <span class="op">=</span> <span class="dv">30</span>,</span>
+<span id="cb2-45"><a href="#cb2-45" aria-hidden="true" tabindex="-1"></a>                   noise <span class="op">=</span> <span class="va">False</span>,</span>
+<span id="cb2-46"><a href="#cb2-46" aria-hidden="true" tabindex="-1"></a>                   tolerance_x <span class="op">=</span> np.sqrt(np.spacing(<span class="dv">1</span>)),</span>
+<span id="cb2-47"><a href="#cb2-47" aria-hidden="true" tabindex="-1"></a>                   var_type <span class="op">=</span> var_type,</span>
+<span id="cb2-48"><a href="#cb2-48" aria-hidden="true" tabindex="-1"></a>                   var_name <span class="op">=</span> var_name,</span>
+<span id="cb2-49"><a href="#cb2-49" aria-hidden="true" tabindex="-1"></a>                   infill_criterion <span class="op">=</span> <span class="st">"y"</span>,</span>
+<span id="cb2-50"><a href="#cb2-50" aria-hidden="true" tabindex="-1"></a>                   n_points <span class="op">=</span> <span class="dv">1</span>,</span>
+<span id="cb2-51"><a href="#cb2-51" aria-hidden="true" tabindex="-1"></a>                   seed<span class="op">=</span><span class="dv">123</span>,</span>
+<span id="cb2-52"><a href="#cb2-52" aria-hidden="true" tabindex="-1"></a>                   log_level <span class="op">=</span> <span class="dv">50</span>,</span>
+<span id="cb2-53"><a href="#cb2-53" aria-hidden="true" tabindex="-1"></a>                   show_models<span class="op">=</span> <span class="va">False</span>,</span>
+<span id="cb2-54"><a href="#cb2-54" aria-hidden="true" tabindex="-1"></a>                   show_progress<span class="op">=</span> <span class="va">True</span>,</span>
+<span id="cb2-55"><a href="#cb2-55" aria-hidden="true" tabindex="-1"></a>                   fun_control <span class="op">=</span> fun_control,</span>
+<span id="cb2-56"><a href="#cb2-56" aria-hidden="true" tabindex="-1"></a>                   design_control<span class="op">=</span>{<span class="st">"init_size"</span>: <span class="dv">10</span>,</span>
+<span id="cb2-57"><a href="#cb2-57" aria-hidden="true" tabindex="-1"></a>                                   <span class="st">"repeats"</span>: <span class="dv">1</span>},</span>
+<span id="cb2-58"><a href="#cb2-58" aria-hidden="true" tabindex="-1"></a>                   surrogate_control<span class="op">=</span>{<span class="st">"noise"</span>: <span class="va">True</span>,</span>
+<span id="cb2-59"><a href="#cb2-59" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"cod_type"</span>: <span class="st">"norm"</span>,</span>
+<span id="cb2-60"><a href="#cb2-60" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"min_theta"</span>: <span class="op">-</span><span class="dv">4</span>,</span>
+<span id="cb2-61"><a href="#cb2-61" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"max_theta"</span>: <span class="dv">3</span>,</span>
+<span id="cb2-62"><a href="#cb2-62" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"n_theta"</span>: <span class="bu">len</span>(var_name),</span>
+<span id="cb2-63"><a href="#cb2-63" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"model_fun_evals"</span>: <span class="dv">10_000</span>,</span>
+<span id="cb2-64"><a href="#cb2-64" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"log_level"</span>: <span class="dv">50</span></span>
+<span id="cb2-65"><a href="#cb2-65" aria-hidden="true" tabindex="-1"></a>                                      })</span>
+<span id="cb2-66"><a href="#cb2-66" aria-hidden="true" tabindex="-1"></a><span class="co"># run spot</span></span>
+<span id="cb2-67"><a href="#cb2-67" aria-hidden="true" tabindex="-1"></a>spot_tuner.run(X_start<span class="op">=</span>X_start)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<div class="cell" data-execution_count="3">
+<div class="sourceCode cell-code" id="cb3"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb3-1"><a href="#cb3-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_progress()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<div class="cell" data-execution_count="4">
+<div class="sourceCode cell-code" id="cb4"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb4-1"><a href="#cb4-1" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> spotPython.utils.eda <span class="im">import</span> gen_design_table</span>
+<span id="cb4-2"><a href="#cb4-2" aria-hidden="true" tabindex="-1"></a><span class="bu">print</span>(gen_design_table(fun_control<span class="op">=</span>fun_control, spot<span class="op">=</span>spot_tuner))</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<div class="cell" data-execution_count="5">
+<div class="sourceCode cell-code" id="cb5"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb5-1"><a href="#cb5-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_importance()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<div class="cell" data-execution_count="6">
+<div class="sourceCode cell-code" id="cb6"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb6-1"><a href="#cb6-1" aria-hidden="true" tabindex="-1"></a>X <span class="op">=</span> spot_tuner.to_all_dim(spot_tuner.min_X.reshape(<span class="dv">1</span>,<span class="op">-</span><span class="dv">1</span>))</span>
+<span id="cb6-2"><a href="#cb6-2" aria-hidden="true" tabindex="-1"></a>model_spot <span class="op">=</span> get_one_core_model_from_X(X, fun_control)</span>
+<span id="cb6-3"><a href="#cb6-3" aria-hidden="true" tabindex="-1"></a>model_spot</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<div class="cell" data-execution_count="7">
+<div class="sourceCode cell-code" id="cb7"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb7-1"><a href="#cb7-1" aria-hidden="true" tabindex="-1"></a>train_tuned(net<span class="op">=</span>model_spot, train_dataset<span class="op">=</span>train,</span>
+<span id="cb7-2"><a href="#cb7-2" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb7-3"><a href="#cb7-3" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb7-4"><a href="#cb7-4" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span><span class="va">True</span>,</span>
+<span id="cb7-5"><a href="#cb7-5" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> <span class="st">"cpu"</span>,</span>
+<span id="cb7-6"><a href="#cb7-6" aria-hidden="true" tabindex="-1"></a>        path<span class="op">=</span><span class="va">None</span>)</span>
+<span id="cb7-7"><a href="#cb7-7" aria-hidden="true" tabindex="-1"></a>test_tuned(net<span class="op">=</span>model_spot, test_dataset<span class="op">=</span>test,</span>
+<span id="cb7-8"><a href="#cb7-8" aria-hidden="true" tabindex="-1"></a>            shuffle<span class="op">=</span><span class="va">False</span>,</span>
+<span id="cb7-9"><a href="#cb7-9" aria-hidden="true" tabindex="-1"></a>            loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb7-10"><a href="#cb7-10" aria-hidden="true" tabindex="-1"></a>            metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb7-11"><a href="#cb7-11" aria-hidden="true" tabindex="-1"></a>            device <span class="op">=</span> <span class="st">"cpu"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<div class="cell" data-execution_count="8">
+<div class="sourceCode cell-code" id="cb8"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb8-1"><a href="#cb8-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_important_hyperparameter_contour()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+</section>
 <section id="sec-hyperparameter-tuning-for-pytorch" class="level1">
 <h1>Hyperparameter Tuning for PyTorch With <code>spotPython</code></h1>
 <p>In this tutorial, we will show how <code>spotPython</code> can be integrated into the <code>PyTorch</code> training workflow. It is based on the tutorial “Hyperparameter Tuning with Ray Tune” from the <code>PyTorch</code> documentation <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span>, which is an extension of the tutorial “Training a Classifier” <span class="citation" data-cites="pyto23b">(<a href="#ref-pyto23b" role="doc-biblioref">PyTorch 2023b</a>)</span> for training a CIFAR10 image classifier.</p>
 <p>This document refers to the following software versions:</p>
 <ul>
 <li><code>python</code>: 3.10.10</li>
 <li><code>torch</code>: 2.0.1</li>
 <li><code>torchvision</code>: 0.15.0</li>
-<li><code>spotPython</code>: 0.2.0</li>
+<li><code>spotPython</code>: 0.2.1</li>
 </ul>
 <p><code>spotPython</code> can be installed via pip<a href="#fn2" class="footnote-ref" id="fnref2" role="doc-noteref"><sup>2</sup></a>.</p>
 <pre class="{raw}"><code>!pip install spotPython</code></pre>
 <p>Results that refer to the <code>Ray Tune</code> package are taken from <a href="https://PyTorch.org/tutorials/beginner/hyperparameter_tuning_tutorial.html">https://PyTorch.org/tutorials/beginner/hyperparameter_tuning_tutorial.html</a><a href="#fn3" class="footnote-ref" id="fnref3" role="doc-noteref"><sup>3</sup></a>.</p>
 <section id="sec-setup" class="level2">
 <h2 class="anchored" data-anchor-id="sec-setup">Setup</h2>
 <p>Before we consider the detailed experimental setup, we select the parameters that affect run time, initial design size and the device that is used.</p>
-<div class="cell" data-execution_count="1">
-<div class="sourceCode cell-code" id="cb2"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb2-1"><a href="#cb2-1" aria-hidden="true" tabindex="-1"></a>MAX_TIME <span class="op">=</span> <span class="dv">60</span></span>
-<span id="cb2-2"><a href="#cb2-2" aria-hidden="true" tabindex="-1"></a>INIT_SIZE <span class="op">=</span> <span class="dv">20</span></span>
-<span id="cb2-3"><a href="#cb2-3" aria-hidden="true" tabindex="-1"></a>DEVICE <span class="op">=</span> <span class="st">"cpu"</span> <span class="co"># "cuda:0"</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="9">
+<div class="sourceCode cell-code" id="cb10"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb10-1"><a href="#cb10-1" aria-hidden="true" tabindex="-1"></a>MAX_TIME <span class="op">=</span> <span class="dv">60</span></span>
+<span id="cb10-2"><a href="#cb10-2" aria-hidden="true" tabindex="-1"></a>INIT_SIZE <span class="op">=</span> <span class="dv">20</span></span>
+<span id="cb10-3"><a href="#cb10-3" aria-hidden="true" tabindex="-1"></a>DEVICE <span class="op">=</span> <span class="st">"cpu"</span> <span class="co"># "cuda:0"</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 <section id="initialization-of-the-fun_control-dictionary" class="level2">
 <h2 class="anchored" data-anchor-id="initialization-of-the-fun_control-dictionary">Initialization of the <code>fun_control</code> Dictionary</h2>
 <p><code>spotPython</code> uses a Python dictionary for storing the information required for the hyperparameter tuning process. This dictionary is called <code>fun_control</code> and is initialized with the function <code>fun_control_init</code>. The function <code>fun_control_init</code> returns a skeleton dictionary. The dictionary is filled with the required information for the hyperparameter tuning process. It stores the hyperparameter tuning settings, e.g., the deep learning network architecture that should be tuned, the classification (or regression) problem, and the data that is used for the tuning. The dictionary is used as an input for the SPOT function.</p>
-<div class="cell" data-execution_count="4">
-<div class="sourceCode cell-code" id="cb3"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb3-1"><a href="#cb3-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> fun_control_init()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="12">
+<div class="sourceCode cell-code" id="cb11"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb11-1"><a href="#cb11-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> fun_control_init()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 <section id="sec-data-loading" class="level2">
 <h2 class="anchored" data-anchor-id="sec-data-loading">Data Loading</h2>
-<p>The data loading process is implemented in the same manner as described in the Section “Data loaders” in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span>. The data loaders are wrapped into the function <code>load_data</code>. A global data directory is used, which allows sharing the data directory between different trials.</p>
-<div class="cell" data-execution_count="5">
-<div class="sourceCode cell-code" id="cb4"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb4-1"><a href="#cb4-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> load_data(data_dir<span class="op">=</span><span class="st">"./data"</span>):</span>
-<span id="cb4-2"><a href="#cb4-2" aria-hidden="true" tabindex="-1"></a>    transform <span class="op">=</span> transforms.Compose([</span>
-<span id="cb4-3"><a href="#cb4-3" aria-hidden="true" tabindex="-1"></a>        transforms.ToTensor(),</span>
-<span id="cb4-4"><a href="#cb4-4" aria-hidden="true" tabindex="-1"></a>        transforms.Normalize((<span class="fl">0.5</span>, <span class="fl">0.5</span>, <span class="fl">0.5</span>), (<span class="fl">0.5</span>, <span class="fl">0.5</span>, <span class="fl">0.5</span>))</span>
-<span id="cb4-5"><a href="#cb4-5" aria-hidden="true" tabindex="-1"></a>    ])</span>
-<span id="cb4-6"><a href="#cb4-6" aria-hidden="true" tabindex="-1"></a></span>
-<span id="cb4-7"><a href="#cb4-7" aria-hidden="true" tabindex="-1"></a>    trainset <span class="op">=</span> torchvision.datasets.CIFAR10(</span>
-<span id="cb4-8"><a href="#cb4-8" aria-hidden="true" tabindex="-1"></a>        root<span class="op">=</span>data_dir, train<span class="op">=</span><span class="va">True</span>, download<span class="op">=</span><span class="va">True</span>, transform<span class="op">=</span>transform)</span>
-<span id="cb4-9"><a href="#cb4-9" aria-hidden="true" tabindex="-1"></a></span>
-<span id="cb4-10"><a href="#cb4-10" aria-hidden="true" tabindex="-1"></a>    testset <span class="op">=</span> torchvision.datasets.CIFAR10(</span>
-<span id="cb4-11"><a href="#cb4-11" aria-hidden="true" tabindex="-1"></a>        root<span class="op">=</span>data_dir, train<span class="op">=</span><span class="va">False</span>, download<span class="op">=</span><span class="va">True</span>, transform<span class="op">=</span>transform)</span>
-<span id="cb4-12"><a href="#cb4-12" aria-hidden="true" tabindex="-1"></a></span>
-<span id="cb4-13"><a href="#cb4-13" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> trainset, testset</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<p>The data loading process is implemented in the same manner as described in the Section “Data loaders” in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span>. The data loaders are wrapped into the function <code>load_data_cifar10</code> which is identical to the function <code>load_data</code> in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span>. A global data directory is used, which allows sharing the data directory between different trials.</p>
+<div class="cell" data-execution_count="13">
+<div class="sourceCode cell-code" id="cb12"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb12-1"><a href="#cb12-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> load_data_cifar10(data_dir<span class="op">=</span><span class="st">"./data"</span>):</span>
+<span id="cb12-2"><a href="#cb12-2" aria-hidden="true" tabindex="-1"></a>    transform <span class="op">=</span> transforms.Compose([</span>
+<span id="cb12-3"><a href="#cb12-3" aria-hidden="true" tabindex="-1"></a>        transforms.ToTensor(),</span>
+<span id="cb12-4"><a href="#cb12-4" aria-hidden="true" tabindex="-1"></a>        transforms.Normalize((<span class="fl">0.5</span>, <span class="fl">0.5</span>, <span class="fl">0.5</span>), (<span class="fl">0.5</span>, <span class="fl">0.5</span>, <span class="fl">0.5</span>))</span>
+<span id="cb12-5"><a href="#cb12-5" aria-hidden="true" tabindex="-1"></a>    ])</span>
+<span id="cb12-6"><a href="#cb12-6" aria-hidden="true" tabindex="-1"></a></span>
+<span id="cb12-7"><a href="#cb12-7" aria-hidden="true" tabindex="-1"></a>    trainset <span class="op">=</span> torchvision.datasets.CIFAR10(</span>
+<span id="cb12-8"><a href="#cb12-8" aria-hidden="true" tabindex="-1"></a>        root<span class="op">=</span>data_dir, train<span class="op">=</span><span class="va">True</span>, download<span class="op">=</span><span class="va">True</span>, transform<span class="op">=</span>transform)</span>
+<span id="cb12-9"><a href="#cb12-9" aria-hidden="true" tabindex="-1"></a></span>
+<span id="cb12-10"><a href="#cb12-10" aria-hidden="true" tabindex="-1"></a>    testset <span class="op">=</span> torchvision.datasets.CIFAR10(</span>
+<span id="cb12-11"><a href="#cb12-11" aria-hidden="true" tabindex="-1"></a>        root<span class="op">=</span>data_dir, train<span class="op">=</span><span class="va">False</span>, download<span class="op">=</span><span class="va">True</span>, transform<span class="op">=</span>transform)</span>
+<span id="cb12-12"><a href="#cb12-12" aria-hidden="true" tabindex="-1"></a></span>
+<span id="cb12-13"><a href="#cb12-13" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> trainset, testset</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
-<p>The test and train data are added to the dictionary <code>fun_control</code>.</p>
-<div class="cell" data-execution_count="6">
-<div class="sourceCode cell-code" id="cb5"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb5-1"><a href="#cb5-1" aria-hidden="true" tabindex="-1"></a>train, test <span class="op">=</span> load_data()</span>
-<span id="cb5-2"><a href="#cb5-2" aria-hidden="true" tabindex="-1"></a>n_samples <span class="op">=</span> <span class="bu">len</span>(train)</span>
-<span id="cb5-3"><a href="#cb5-3" aria-hidden="true" tabindex="-1"></a><span class="co"># add the dataset to the fun_control</span></span>
-<span id="cb5-4"><a href="#cb5-4" aria-hidden="true" tabindex="-1"></a>fun_control.update({</span>
-<span id="cb5-5"><a href="#cb5-5" aria-hidden="true" tabindex="-1"></a>    <span class="st">"train"</span>: train,</span>
-<span id="cb5-6"><a href="#cb5-6" aria-hidden="true" tabindex="-1"></a>    <span class="st">"test"</span>: test,</span>
-<span id="cb5-7"><a href="#cb5-7" aria-hidden="true" tabindex="-1"></a>    <span class="st">"n_samples"</span>: n_samples})</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<p>The method <code>load_data_cifar10</code> is part of the <code>spotPython</code> package and can be imported from <code>spotPython.data.torchdata</code>.</p>
+<p>In the following step, the test and train data are added to the dictionary <code>fun_control</code>.</p>
+<div class="cell" data-execution_count="14">
+<div class="sourceCode cell-code" id="cb13"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb13-1"><a href="#cb13-1" aria-hidden="true" tabindex="-1"></a>train, test <span class="op">=</span> load_data_cifar10()</span>
+<span id="cb13-2"><a href="#cb13-2" aria-hidden="true" tabindex="-1"></a>n_samples <span class="op">=</span> <span class="bu">len</span>(train)</span>
+<span id="cb13-3"><a href="#cb13-3" aria-hidden="true" tabindex="-1"></a><span class="co"># add the dataset to the fun_control</span></span>
+<span id="cb13-4"><a href="#cb13-4" aria-hidden="true" tabindex="-1"></a>fun_control.update({</span>
+<span id="cb13-5"><a href="#cb13-5" aria-hidden="true" tabindex="-1"></a>    <span class="st">"train"</span>: train,</span>
+<span id="cb13-6"><a href="#cb13-6" aria-hidden="true" tabindex="-1"></a>    <span class="st">"test"</span>: test,</span>
+<span id="cb13-7"><a href="#cb13-7" aria-hidden="true" tabindex="-1"></a>    <span class="st">"n_samples"</span>: n_samples})</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 <section id="sec-specification-of-preprocessing-model" class="level2">
 <h2 class="anchored" data-anchor-id="sec-specification-of-preprocessing-model">Specification of the Preprocessing Model</h2>
 <p>After the training and test data are specified and added to the <code>fun_control</code> dictionary, <code>spotPython</code> allows the specification of a data preprocessing pipeline, e.g., for the scaling of the data or for the one-hot encoding of categorical variables. The preprocessing model is called <code>prep_model</code> (“preparation” or pre-processing) and includes steps that are not subject to the hyperparameter tuning process. The preprocessing model is specified in the <code>fun_control</code> dictionary. The preprocessing model can be implemented as a <code>sklearn</code> pipeline. The following code shows a typical preprocessing pipeline:</p>
 <pre class="{raw}"><code>categorical_columns = ["cities", "colors"]
 one_hot_encoder = OneHotEncoder(handle_unknown="ignore",
@@ -277,22 +408,22 @@
 prep_model = ColumnTransformer(
         transformers=[
              ("categorical", one_hot_encoder, categorical_columns),
          ],
          remainder=StandardScaler(),
      )</code></pre>
 <p>Because the Ray Tune (<code>ray[tune]</code>) hyperparameter tuning as described in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span> does not use a preprocessing model, the preprocessing model is set to <code>None</code> here.</p>
-<div class="cell" data-execution_count="7">
-<div class="sourceCode cell-code" id="cb7"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb7-1"><a href="#cb7-1" aria-hidden="true" tabindex="-1"></a>prep_model <span class="op">=</span> <span class="va">None</span></span>
-<span id="cb7-2"><a href="#cb7-2" aria-hidden="true" tabindex="-1"></a>fun_control.update({<span class="st">"prep_model"</span>: prep_model})</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="15">
+<div class="sourceCode cell-code" id="cb15"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb15-1"><a href="#cb15-1" aria-hidden="true" tabindex="-1"></a>prep_model <span class="op">=</span> <span class="va">None</span></span>
+<span id="cb15-2"><a href="#cb15-2" aria-hidden="true" tabindex="-1"></a>fun_control.update({<span class="st">"prep_model"</span>: prep_model})</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 <section id="sec-selection-of-the-algorithm" class="level2">
 <h2 class="anchored" data-anchor-id="sec-selection-of-the-algorithm">Select <code>algorithm</code> and <code>core_model_hyper_dict</code></h2>
-<p>The same neural network model as implemented in the section “Configurable neural network” of the <code>PyTorch</code> tutorial <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span> is used here. We will show the implementation from <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span> in <a href="#sec-implementation-with-raytune">Section&nbsp;3.5.1</a> first, before the extended implementation with <code>spotPython</code> is shown in <a href="#sec-implementation-with-spotpython">Section&nbsp;3.5.2</a>.</p>
+<p>The same neural network model as implemented in the section “Configurable neural network” of the <code>PyTorch</code> tutorial <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span> is used here. We will show the implementation from <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span> in <a href="#sec-implementation-with-raytune">Section&nbsp;4.5.1</a> first, before the extended implementation with <code>spotPython</code> is shown in <a href="#sec-implementation-with-spotpython">Section&nbsp;4.5.2</a>.</p>
 <section id="sec-implementation-with-raytune" class="level3">
 <h3 class="anchored" data-anchor-id="sec-implementation-with-raytune">Implementing a Configurable Neural Network With Ray Tune</h3>
 <p>We used the same hyperparameters that are implemented as configurable in the <code>PyTorch</code> tutorial. We specify the layer sizes, namely <code>l1</code> and <code>l2</code>, of the fully connected layers:</p>
 <pre class="{raw}"><code>class Net(nn.Module):
     def __init__(self, l1=120, l2=84):
         super(Net, self).__init__()
         self.conv1 = nn.Conv2d(3, 6, 5)
@@ -313,20 +444,29 @@
 </code></pre>
 <p>The learning rate, i.e., <code>lr</code>, of the optimizer is made configurable, too:</p>
 <pre class="{raw}"><code>optimizer = optim.SGD(net.parameters(), lr=config["lr"], momentum=0.9)</code></pre>
 </section>
 <section id="sec-implementation-with-spotpython" class="level3">
 <h3 class="anchored" data-anchor-id="sec-implementation-with-spotpython">Implementing a Configurable Neural Network With spotPython</h3>
 <p><code>spotPython</code> implements a class which is similar to the class described in the <code>PyTorch</code> tutorial. The class is called <code>Net_CIFAR10</code> and is implemented in the file <code>netcifar10.py</code>.</p>
-<pre class="{raw}"><code>import spotPython.torch.netcore as netcore
+<pre class="{raw}"><code>from torch import nn
+import torch.nn.functional as F
+import spotPython.torch.netcore as netcore
+
+
 class Net_CIFAR10(netcore.Net_Core):
-    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience):
+    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd_momentum):
         super(Net_CIFAR10, self).__init__(
-            lr_mult=lr_mult, batch_size=batch_size, epochs=epochs, k_folds=k_folds,
-            patience=patience
+            lr_mult=lr_mult,
+            batch_size=batch_size,
+            epochs=epochs,
+            k_folds=k_folds,
+            patience=patience,
+            optimizer=optimizer,
+            sgd_momentum=sgd_momentum,
         )
         self.conv1 = nn.Conv2d(3, 6, 5)
         self.pool = nn.MaxPool2d(2, 2)
         self.conv2 = nn.Conv2d(6, 16, 5)
         self.fc1 = nn.Linear(16 * 5 * 5, l1)
         self.fc2 = nn.Linear(l1, l2)
         self.fc3 = nn.Linear(l2, 10)
@@ -340,59 +480,62 @@
         x = self.fc3(x)
         return x</code></pre>
 <p><code>Net_CIFAR10</code> inherits from the class <code>Net_Core</code> which is implemented in the file <code>netcore.py</code>. It implements the additional attributes that are common to all neural network models. The attributes are the learning rate multiplier <code>lr_mult</code>, the batch size <code>batch_size</code>, the number of epochs <code>epochs</code>, the number of folds <code>k_folds</code> for the cross validation, and the patience <code>patience</code> for the early stopping. The class <code>Net_Core</code> is shown below.</p>
 <pre class="{raw}"><code>from torch import nn
 
 
 class Net_Core(nn.Module):
-    def __init__(self, lr_mult, batch_size, epochs, k_folds, patience):
+    def __init__(self, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd_momentum):
         super(Net_Core, self).__init__()
         self.lr_mult = lr_mult
         self.batch_size = batch_size
         self.epochs = epochs
         self.k_folds = k_folds
-        self.patience = patience</code></pre>
-</section>
-<section id="sec-comparison" class="level3">
-<h3 class="anchored" data-anchor-id="sec-comparison">Comparison of the Approach Described in the PyTorch Tutorial With spotPython</h3>
-<p>Comparing the class <code>Net</code> from the <code>PyTorch</code> tutorial and the class <code>Net_CIFAR10</code> from <code>spotPython</code>, we see that the class <code>Net_CIFAR10</code> has additional attributes and does not inherit from <code>nn</code> directly. It adds an additional class, <code>Net_core</code>, that takes care of additional attributes that are common to all neural network models, e.g., the learning rate multiplier <code>lr_mult</code> or the batch size <code>batch_size</code>.</p>
-<p><code>spotPython</code>’s <code>core_model</code> implements an instance of the <code>Net_CIFAR10</code> class. In addition to the basic neural network model, the <code>core_model</code> can use these additional attributes. <code>spotPython</code> provides methods for handling these additional attributes to guarantee 100% compatibility with the <code>PyTorch</code> classes. The method <code>add_core_model_to_fun_control</code> adds the hyperparameters and additional attributes to the <code>fun_control</code> dictionary. The method is shown below.</p>
-<div class="cell" data-execution_count="8">
-<div class="sourceCode cell-code" id="cb12"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb12-1"><a href="#cb12-1" aria-hidden="true" tabindex="-1"></a>core_model <span class="op">=</span> Net_CIFAR10</span>
-<span id="cb12-2"><a href="#cb12-2" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> add_core_model_to_fun_control(core_model<span class="op">=</span>core_model,</span>
-<span id="cb12-3"><a href="#cb12-3" aria-hidden="true" tabindex="-1"></a>                              fun_control<span class="op">=</span>fun_control,</span>
-<span id="cb12-4"><a href="#cb12-4" aria-hidden="true" tabindex="-1"></a>                              hyper_dict<span class="op">=</span>TorchHyperDict,</span>
-<span id="cb12-5"><a href="#cb12-5" aria-hidden="true" tabindex="-1"></a>                              filename<span class="op">=</span><span class="va">None</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
+        self.patience = patience
+        self.optimizer = optimizer
+        self.sgd_momentum = sgd_momentum</code></pre>
 <div class="callout callout-style-default callout-note callout-titled">
 <div class="callout-header d-flex align-content-center">
 <div class="callout-icon-container">
 <i class="callout-icon"></i>
 </div>
 <div class="callout-title-container flex-fill">
-Note
+The <code>Net_Core</code> class
 </div>
 </div>
 <div class="callout-body-container callout-body">
-<p>In addition to the class Net from the <code>PyTorch</code> tutorial, the class Net_CIFAR10 has additional attributes, e.g.:</p>
+<p>The <code>Net_Core</code> class is implemented in the file <code>netcore.py</code>. It implements hyperparameters as attributes, that are not used by the <code>core_model</code>, e.g.:</p>
 <ul>
+<li>optimizer (<code>optimizer</code>),</li>
 <li>learning rate (<code>lr</code>),</li>
 <li>batch size (<code>batch_size</code>),</li>
 <li>epochs (<code>epochs</code>),</li>
 <li>k_folds (<code>k_folds</code>), and</li>
-<li>early stopping criterion “patience” (<code>patience</code>)</li>
+<li>early stopping criterion “patience” (<code>patience</code>).</li>
 </ul>
-<p>Further attributes can be easily added to the class, e.g., <code>optimizer</code>.</p>
+<p>Users can add further attributes to the class.</p>
 </div>
 </div>
 </section>
+<section id="sec-comparison" class="level3">
+<h3 class="anchored" data-anchor-id="sec-comparison">Comparison of the Approach Described in the PyTorch Tutorial With spotPython</h3>
+<p>Comparing the class <code>Net</code> from the <code>PyTorch</code> tutorial and the class <code>Net_CIFAR10</code> from <code>spotPython</code>, we see that the class <code>Net_CIFAR10</code> has additional attributes and does not inherit from <code>nn</code> directly. It adds an additional class, <code>Net_core</code>, that takes care of additional attributes that are common to all neural network models, e.g., the learning rate multiplier <code>lr_mult</code> or the batch size <code>batch_size</code>.</p>
+<p><code>spotPython</code>’s <code>core_model</code> implements an instance of the <code>Net_CIFAR10</code> class. In addition to the basic neural network model, the <code>core_model</code> can use these additional attributes. <code>spotPython</code> provides methods for handling these additional attributes to guarantee 100% compatibility with the <code>PyTorch</code> classes. The method <code>add_core_model_to_fun_control</code> adds the hyperparameters and additional attributes to the <code>fun_control</code> dictionary. The method is shown below.</p>
+<div class="cell" data-execution_count="16">
+<div class="sourceCode cell-code" id="cb20"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb20-1"><a href="#cb20-1" aria-hidden="true" tabindex="-1"></a>core_model <span class="op">=</span> Net_CIFAR10</span>
+<span id="cb20-2"><a href="#cb20-2" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> add_core_model_to_fun_control(core_model<span class="op">=</span>core_model,</span>
+<span id="cb20-3"><a href="#cb20-3" aria-hidden="true" tabindex="-1"></a>                              fun_control<span class="op">=</span>fun_control,</span>
+<span id="cb20-4"><a href="#cb20-4" aria-hidden="true" tabindex="-1"></a>                              hyper_dict<span class="op">=</span>TorchHyperDict,</span>
+<span id="cb20-5"><a href="#cb20-5" aria-hidden="true" tabindex="-1"></a>                              filename<span class="op">=</span><span class="va">None</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+</section>
 </section>
 <section id="sec-search-space" class="level2">
 <h2 class="anchored" data-anchor-id="sec-search-space">The Search Space</h2>
-<p>In <a href="#sec-configuring-the-search-space-with-ray-tune">Section&nbsp;3.6.1</a>, we first describe how to configure the search space with <code>ray[tune]</code> (as shown in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span>) and then how to configure the search space with <code>spotPython</code> in <a href="#sec-configuring-the-search-space-with-spotpython">Section&nbsp;3.6.2</a>.</p>
+<p>In <a href="#sec-configuring-the-search-space-with-ray-tune">Section&nbsp;4.6.1</a>, we first describe how to configure the search space with <code>ray[tune]</code> (as shown in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span>) and then how to configure the search space with <code>spotPython</code> in <a href="#sec-configuring-the-search-space-with-spotpython">Section&nbsp;4.6.2</a>.</p>
 <section id="sec-configuring-the-search-space-with-ray-tune" class="level3">
 <h3 class="anchored" data-anchor-id="sec-configuring-the-search-space-with-ray-tune">Configuring the Search Space With Ray Tune</h3>
 <p>Ray Tune’s search space can be configured as follows <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span>:</p>
 <pre class="{raw}"><code>config = {
     "l1": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),
     "l2": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),
     "lr": tune.loguniform(1e-4, 1e-1),
@@ -401,134 +544,134 @@
 <p>The <code>tune.sample_from()</code> function enables the user to define sample methods to obtain hyperparameters. In this example, the <code>l1</code> and <code>l2</code> parameters should be powers of 2 between 4 and 256, so either 4, 8, 16, 32, 64, 128, or 256. The <code>lr</code> (learning rate) should be uniformly sampled between 0.0001 and 0.1. Lastly, the batch size is a choice between 2, 4, 8, and 16.</p>
 <p>At each trial, <code>ray[tune]</code> will randomly sample a combination of parameters from these search spaces. It will then train a number of models in parallel and find the best performing one among these. <code>ray[tune]</code> uses the <code>ASHAScheduler</code> which will terminate bad performing trials early.</p>
 </section>
 <section id="sec-configuring-the-search-space-with-spotpython" class="level3">
 <h3 class="anchored" data-anchor-id="sec-configuring-the-search-space-with-spotpython">Configuring the Search Space With spotPython</h3>
 <section id="the-hyper_dict-hyperparameters-for-the-selected-algorithm" class="level4">
 <h4 class="anchored" data-anchor-id="the-hyper_dict-hyperparameters-for-the-selected-algorithm">The <code>hyper_dict</code> Hyperparameters for the Selected Algorithm</h4>
-<p><code>spotPython</code> uses simple <code>JSON</code> files for the specification of the hyperparameters. Users can specify their individual <code>JSON</code> files, or they can use the <code>JSON</code> files provided by <code>spotPython</code>. The <code>JSON</code> file for the <code>core_model</code> is called <code>torch_hyper_dict.json</code>.</p>
-<p>In contrast to <code>ray[tune]</code>, <code>spotPython</code> can handle numerical, boolean, and categorical hyperparameters. They can be specified in the <code>JSON</code> file in a similar way as the numerical hyperparameters as shown below:</p>
-<div class="sourceCode" id="cb14"><pre class="sourceCode json code-with-copy"><code class="sourceCode json"><span id="cb14-1"><a href="#cb14-1" aria-hidden="true" tabindex="-1"></a><span class="er">"factor_hyperparameter":</span> <span class="fu">{</span></span>
-<span id="cb14-2"><a href="#cb14-2" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"levels"</span><span class="fu">:</span> <span class="ot">[</span><span class="st">"A"</span><span class="ot">,</span> <span class="st">"B"</span><span class="ot">,</span> <span class="st">"C"</span><span class="ot">]</span><span class="fu">,</span></span>
-<span id="cb14-3"><a href="#cb14-3" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"factor"</span><span class="fu">,</span></span>
-<span id="cb14-4"><a href="#cb14-4" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"default"</span><span class="fu">:</span> <span class="st">"B"</span><span class="fu">,</span></span>
-<span id="cb14-5"><a href="#cb14-5" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
-<span id="cb14-6"><a href="#cb14-6" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"core_model_parameter_type"</span><span class="fu">:</span> <span class="st">"str"</span><span class="fu">,</span></span>
-<span id="cb14-7"><a href="#cb14-7" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">0</span><span class="fu">,</span></span>
-<span id="cb14-8"><a href="#cb14-8" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">}</span><span class="er">,</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-<p>Each entry in the <code>JSON</code> file represents one hyperparameter with the following structure: <code>type</code>, <code>default</code>, <code>transform</code>, <code>lower</code>, and <code>upper</code>. The corresponding entries for the <code>Net_CIFAR10</code> class are shown below.</p>
-<div class="sourceCode" id="cb15"><pre class="sourceCode json code-with-copy"><code class="sourceCode json"><span id="cb15-1"><a href="#cb15-1" aria-hidden="true" tabindex="-1"></a><span class="fu">{</span><span class="dt">"Net_CIFAR10"</span><span class="fu">:</span></span>
-<span id="cb15-2"><a href="#cb15-2" aria-hidden="true" tabindex="-1"></a>    <span class="fu">{</span></span>
-<span id="cb15-3"><a href="#cb15-3" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"l1"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-4"><a href="#cb15-4" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
-<span id="cb15-5"><a href="#cb15-5" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">5</span><span class="fu">,</span></span>
-<span id="cb15-6"><a href="#cb15-6" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
-<span id="cb15-7"><a href="#cb15-7" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
-<span id="cb15-8"><a href="#cb15-8" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">9</span><span class="fu">},</span></span>
-<span id="cb15-9"><a href="#cb15-9" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"l2"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-10"><a href="#cb15-10" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
-<span id="cb15-11"><a href="#cb15-11" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">5</span><span class="fu">,</span></span>
-<span id="cb15-12"><a href="#cb15-12" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
-<span id="cb15-13"><a href="#cb15-13" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
-<span id="cb15-14"><a href="#cb15-14" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">9</span><span class="fu">},</span></span>
-<span id="cb15-15"><a href="#cb15-15" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"lr_mult"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-16"><a href="#cb15-16" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"float"</span><span class="fu">,</span></span>
-<span id="cb15-17"><a href="#cb15-17" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="fl">1.0</span><span class="fu">,</span></span>
-<span id="cb15-18"><a href="#cb15-18" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
-<span id="cb15-19"><a href="#cb15-19" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="fl">0.1</span><span class="fu">,</span></span>
-<span id="cb15-20"><a href="#cb15-20" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">10</span><span class="fu">},</span></span>
-<span id="cb15-21"><a href="#cb15-21" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"batch_size"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-22"><a href="#cb15-22" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
-<span id="cb15-23"><a href="#cb15-23" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">4</span><span class="fu">,</span></span>
-<span id="cb15-24"><a href="#cb15-24" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
-<span id="cb15-25"><a href="#cb15-25" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">1</span><span class="fu">,</span></span>
-<span id="cb15-26"><a href="#cb15-26" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">4</span><span class="fu">},</span></span>
-<span id="cb15-27"><a href="#cb15-27" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"epochs"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-28"><a href="#cb15-28" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
-<span id="cb15-29"><a href="#cb15-29" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">3</span><span class="fu">,</span></span>
-<span id="cb15-30"><a href="#cb15-30" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
-<span id="cb15-31"><a href="#cb15-31" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">1</span><span class="fu">,</span></span>
-<span id="cb15-32"><a href="#cb15-32" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">4</span><span class="fu">},</span></span>
-<span id="cb15-33"><a href="#cb15-33" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"k_folds"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-34"><a href="#cb15-34" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
-<span id="cb15-35"><a href="#cb15-35" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
-<span id="cb15-36"><a href="#cb15-36" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
-<span id="cb15-37"><a href="#cb15-37" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
-<span id="cb15-38"><a href="#cb15-38" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">3</span><span class="fu">},</span></span>
-<span id="cb15-39"><a href="#cb15-39" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"patience"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-40"><a href="#cb15-40" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
-<span id="cb15-41"><a href="#cb15-41" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">5</span><span class="fu">,</span></span>
-<span id="cb15-42"><a href="#cb15-42" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
-<span id="cb15-43"><a href="#cb15-43" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
-<span id="cb15-44"><a href="#cb15-44" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">10</span><span class="fu">},</span></span>
-<span id="cb15-45"><a href="#cb15-45" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"optimizer"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-46"><a href="#cb15-46" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"levels"</span><span class="fu">:</span> <span class="ot">[</span><span class="st">"Adadelta"</span><span class="ot">,</span></span>
-<span id="cb15-47"><a href="#cb15-47" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"Adagrad"</span><span class="ot">,</span></span>
-<span id="cb15-48"><a href="#cb15-48" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"Adam"</span><span class="ot">,</span></span>
-<span id="cb15-49"><a href="#cb15-49" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"AdamW"</span><span class="ot">,</span></span>
-<span id="cb15-50"><a href="#cb15-50" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"SparseAdam"</span><span class="ot">,</span></span>
-<span id="cb15-51"><a href="#cb15-51" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"Adamax"</span><span class="ot">,</span></span>
-<span id="cb15-52"><a href="#cb15-52" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"ASGD"</span><span class="ot">,</span></span>
-<span id="cb15-53"><a href="#cb15-53" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"LBFGS"</span><span class="ot">,</span></span>
-<span id="cb15-54"><a href="#cb15-54" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"NAdam"</span><span class="ot">,</span></span>
-<span id="cb15-55"><a href="#cb15-55" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"RAdam"</span><span class="ot">,</span></span>
-<span id="cb15-56"><a href="#cb15-56" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"RMSprop"</span><span class="ot">,</span></span>
-<span id="cb15-57"><a href="#cb15-57" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"Rprop"</span><span class="ot">,</span></span>
-<span id="cb15-58"><a href="#cb15-58" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"SGD"</span><span class="ot">]</span><span class="fu">,</span></span>
-<span id="cb15-59"><a href="#cb15-59" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"factor"</span><span class="fu">,</span></span>
-<span id="cb15-60"><a href="#cb15-60" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="st">"SGD"</span><span class="fu">,</span></span>
-<span id="cb15-61"><a href="#cb15-61" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
-<span id="cb15-62"><a href="#cb15-62" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"class_name"</span><span class="fu">:</span> <span class="st">"torch.optim"</span><span class="fu">,</span></span>
-<span id="cb15-63"><a href="#cb15-63" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"core_model_parameter_type"</span><span class="fu">:</span> <span class="st">"str"</span><span class="fu">,</span></span>
-<span id="cb15-64"><a href="#cb15-64" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">0</span><span class="fu">,</span></span>
-<span id="cb15-65"><a href="#cb15-65" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">12</span><span class="fu">},</span></span>
-<span id="cb15-66"><a href="#cb15-66" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"sgd_momentum"</span><span class="fu">:</span> <span class="fu">{</span></span>
-<span id="cb15-67"><a href="#cb15-67" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"float"</span><span class="fu">,</span></span>
-<span id="cb15-68"><a href="#cb15-68" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="fl">0.0</span><span class="fu">,</span></span>
-<span id="cb15-69"><a href="#cb15-69" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
-<span id="cb15-70"><a href="#cb15-70" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="fl">0.0</span><span class="fu">,</span></span>
-<span id="cb15-71"><a href="#cb15-71" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="fl">1.0</span><span class="fu">}</span></span>
-<span id="cb15-72"><a href="#cb15-72" aria-hidden="true" tabindex="-1"></a>    <span class="fu">}</span></span>
-<span id="cb15-73"><a href="#cb15-73" aria-hidden="true" tabindex="-1"></a><span class="fu">}</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<p><code>spotPython</code> uses <code>JSON</code> files for the specification of the hyperparameters. Users can specify their individual <code>JSON</code> files, or they can use the <code>JSON</code> files provided by <code>spotPython</code>. The <code>JSON</code> file for the <code>core_model</code> is called <code>torch_hyper_dict.json</code>.</p>
+<p>In contrast to <code>ray[tune]</code>, <code>spotPython</code> can handle numerical, boolean, and categorical hyperparameters. They can be specified in the <code>JSON</code> file in a similar way as the numerical hyperparameters as shown below. Each entry in the <code>JSON</code> file represents one hyperparameter with the following structure: <code>type</code>, <code>default</code>, <code>transform</code>, <code>lower</code>, and <code>upper</code>.</p>
+<div class="sourceCode" id="cb22"><pre class="sourceCode json code-with-copy"><code class="sourceCode json"><span id="cb22-1"><a href="#cb22-1" aria-hidden="true" tabindex="-1"></a><span class="er">"factor_hyperparameter":</span> <span class="fu">{</span></span>
+<span id="cb22-2"><a href="#cb22-2" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"levels"</span><span class="fu">:</span> <span class="ot">[</span><span class="st">"A"</span><span class="ot">,</span> <span class="st">"B"</span><span class="ot">,</span> <span class="st">"C"</span><span class="ot">]</span><span class="fu">,</span></span>
+<span id="cb22-3"><a href="#cb22-3" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"factor"</span><span class="fu">,</span></span>
+<span id="cb22-4"><a href="#cb22-4" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"default"</span><span class="fu">:</span> <span class="st">"B"</span><span class="fu">,</span></span>
+<span id="cb22-5"><a href="#cb22-5" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
+<span id="cb22-6"><a href="#cb22-6" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"core_model_parameter_type"</span><span class="fu">:</span> <span class="st">"str"</span><span class="fu">,</span></span>
+<span id="cb22-7"><a href="#cb22-7" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">0</span><span class="fu">,</span></span>
+<span id="cb22-8"><a href="#cb22-8" aria-hidden="true" tabindex="-1"></a>    <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">}</span><span class="er">,</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<p>The corresponding entries for the <code>Net_CIFAR10</code> class are shown below.</p>
+<div class="sourceCode" id="cb23"><pre class="sourceCode json code-with-copy"><code class="sourceCode json"><span id="cb23-1"><a href="#cb23-1" aria-hidden="true" tabindex="-1"></a><span class="fu">{</span><span class="dt">"Net_CIFAR10"</span><span class="fu">:</span></span>
+<span id="cb23-2"><a href="#cb23-2" aria-hidden="true" tabindex="-1"></a>    <span class="fu">{</span></span>
+<span id="cb23-3"><a href="#cb23-3" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"l1"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb23-4"><a href="#cb23-4" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
+<span id="cb23-5"><a href="#cb23-5" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">5</span><span class="fu">,</span></span>
+<span id="cb23-6"><a href="#cb23-6" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
+<span id="cb23-7"><a href="#cb23-7" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
+<span id="cb23-8"><a href="#cb23-8" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">9</span><span class="fu">},</span></span>
+<span id="cb23-9"><a href="#cb23-9" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"l2"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb23-10"><a href="#cb23-10" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
+<span id="cb23-11"><a href="#cb23-11" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">5</span><span class="fu">,</span></span>
+<span id="cb23-12"><a href="#cb23-12" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
+<span id="cb23-13"><a href="#cb23-13" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
+<span id="cb23-14"><a href="#cb23-14" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">9</span><span class="fu">},</span></span>
+<span id="cb23-15"><a href="#cb23-15" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"lr_mult"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb23-16"><a href="#cb23-16" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"float"</span><span class="fu">,</span></span>
+<span id="cb23-17"><a href="#cb23-17" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="fl">1.0</span><span class="fu">,</span></span>
+<span id="cb23-18"><a href="#cb23-18" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
+<span id="cb23-19"><a href="#cb23-19" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="fl">0.1</span><span class="fu">,</span></span>
+<span id="cb23-20"><a href="#cb23-20" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">10</span><span class="fu">},</span></span>
+<span id="cb23-21"><a href="#cb23-21" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"batch_size"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb23-22"><a href="#cb23-22" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
+<span id="cb23-23"><a href="#cb23-23" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">4</span><span class="fu">,</span></span>
+<span id="cb23-24"><a href="#cb23-24" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
+<span id="cb23-25"><a href="#cb23-25" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">1</span><span class="fu">,</span></span>
+<span id="cb23-26"><a href="#cb23-26" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">4</span><span class="fu">},</span></span>
+<span id="cb23-27"><a href="#cb23-27" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"epochs"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb23-28"><a href="#cb23-28" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
+<span id="cb23-29"><a href="#cb23-29" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">3</span><span class="fu">,</span></span>
+<span id="cb23-30"><a href="#cb23-30" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"transform_power_2_int"</span><span class="fu">,</span></span>
+<span id="cb23-31"><a href="#cb23-31" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">1</span><span class="fu">,</span></span>
+<span id="cb23-32"><a href="#cb23-32" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">4</span><span class="fu">},</span></span>
+<span id="cb23-33"><a href="#cb23-33" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"k_folds"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb23-34"><a href="#cb23-34" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
+<span id="cb23-35"><a href="#cb23-35" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
+<span id="cb23-36"><a href="#cb23-36" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
+<span id="cb23-37"><a href="#cb23-37" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
+<span id="cb23-38"><a href="#cb23-38" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">3</span><span class="fu">},</span></span>
+<span id="cb23-39"><a href="#cb23-39" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"patience"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb23-40"><a href="#cb23-40" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"int"</span><span class="fu">,</span></span>
+<span id="cb23-41"><a href="#cb23-41" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="dv">5</span><span class="fu">,</span></span>
+<span id="cb23-42"><a href="#cb23-42" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
+<span id="cb23-43"><a href="#cb23-43" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">2</span><span class="fu">,</span></span>
+<span id="cb23-44"><a href="#cb23-44" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">10</span><span class="fu">},</span></span>
+<span id="cb23-45"><a href="#cb23-45" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"optimizer"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb23-46"><a href="#cb23-46" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"levels"</span><span class="fu">:</span> <span class="ot">[</span><span class="st">"Adadelta"</span><span class="ot">,</span></span>
+<span id="cb23-47"><a href="#cb23-47" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"Adagrad"</span><span class="ot">,</span></span>
+<span id="cb23-48"><a href="#cb23-48" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"Adam"</span><span class="ot">,</span></span>
+<span id="cb23-49"><a href="#cb23-49" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"AdamW"</span><span class="ot">,</span></span>
+<span id="cb23-50"><a href="#cb23-50" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"SparseAdam"</span><span class="ot">,</span></span>
+<span id="cb23-51"><a href="#cb23-51" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"Adamax"</span><span class="ot">,</span></span>
+<span id="cb23-52"><a href="#cb23-52" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"ASGD"</span><span class="ot">,</span></span>
+<span id="cb23-53"><a href="#cb23-53" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"LBFGS"</span><span class="ot">,</span></span>
+<span id="cb23-54"><a href="#cb23-54" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"NAdam"</span><span class="ot">,</span></span>
+<span id="cb23-55"><a href="#cb23-55" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"RAdam"</span><span class="ot">,</span></span>
+<span id="cb23-56"><a href="#cb23-56" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"RMSprop"</span><span class="ot">,</span></span>
+<span id="cb23-57"><a href="#cb23-57" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"Rprop"</span><span class="ot">,</span></span>
+<span id="cb23-58"><a href="#cb23-58" aria-hidden="true" tabindex="-1"></a>                       <span class="st">"SGD"</span><span class="ot">]</span><span class="fu">,</span></span>
+<span id="cb23-59"><a href="#cb23-59" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"factor"</span><span class="fu">,</span></span>
+<span id="cb23-60"><a href="#cb23-60" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="st">"SGD"</span><span class="fu">,</span></span>
+<span id="cb23-61"><a href="#cb23-61" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
+<span id="cb23-62"><a href="#cb23-62" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"class_name"</span><span class="fu">:</span> <span class="st">"torch.optim"</span><span class="fu">,</span></span>
+<span id="cb23-63"><a href="#cb23-63" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"core_model_parameter_type"</span><span class="fu">:</span> <span class="st">"str"</span><span class="fu">,</span></span>
+<span id="cb23-64"><a href="#cb23-64" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="dv">0</span><span class="fu">,</span></span>
+<span id="cb23-65"><a href="#cb23-65" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="dv">12</span><span class="fu">},</span></span>
+<span id="cb23-66"><a href="#cb23-66" aria-hidden="true" tabindex="-1"></a>        <span class="dt">"sgd_momentum"</span><span class="fu">:</span> <span class="fu">{</span></span>
+<span id="cb23-67"><a href="#cb23-67" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"type"</span><span class="fu">:</span> <span class="st">"float"</span><span class="fu">,</span></span>
+<span id="cb23-68"><a href="#cb23-68" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"default"</span><span class="fu">:</span> <span class="fl">0.0</span><span class="fu">,</span></span>
+<span id="cb23-69"><a href="#cb23-69" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"transform"</span><span class="fu">:</span> <span class="st">"None"</span><span class="fu">,</span></span>
+<span id="cb23-70"><a href="#cb23-70" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"lower"</span><span class="fu">:</span> <span class="fl">0.0</span><span class="fu">,</span></span>
+<span id="cb23-71"><a href="#cb23-71" aria-hidden="true" tabindex="-1"></a>            <span class="dt">"upper"</span><span class="fu">:</span> <span class="fl">1.0</span><span class="fu">}</span></span>
+<span id="cb23-72"><a href="#cb23-72" aria-hidden="true" tabindex="-1"></a>    <span class="fu">}</span></span>
+<span id="cb23-73"><a href="#cb23-73" aria-hidden="true" tabindex="-1"></a><span class="fu">}</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </section>
 </section>
 </section>
 <section id="sec-modification-of-hyperparameters" class="level2">
 <h2 class="anchored" data-anchor-id="sec-modification-of-hyperparameters">Modifying the Hyperparameters</h2>
 <p>Ray tune <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span> does not provide a way to change the specified hyperparameters without re-compilation. However, <code>spotPython</code> provides functions for modifying the hyperparameters, their bounds and factors as well as for activating and de-activating hyperparameters without re-compilation of the Python source code. These functions are described in the following.</p>
 <section id="sec-modification-of-default-values" class="level3">
 <h3 class="anchored" data-anchor-id="sec-modification-of-default-values">Modify <code>hyper_dict</code> Hyperparameters for the Selected Algorithm aka <code>core_model</code></h3>
 <p>After specifying the model, the corresponding hyperparameters, their types and bounds are loaded from the <code>JSON</code> file <code>torch_hyper_dict.json</code>. After loading, the user can modify the hyperparameters, e.g., the bounds. <code>spotPython</code> provides a simple rule for de-activating hyperparameters: If the lower and the upper bound are set to identical values, the hyperparameter is de-activated. This is useful for the hyperparameter tuning, because it allows to specify a hyperparameter in the <code>JSON</code> file, but to de-activate it in the <code>fun_control</code> dictionary. This is done in the next step.</p>
 </section>
 <section id="modify-hyperparameters-of-type-numeric-and-integer-boolean" class="level3">
 <h3 class="anchored" data-anchor-id="modify-hyperparameters-of-type-numeric-and-integer-boolean">Modify Hyperparameters of Type numeric and integer (boolean)</h3>
 <p>Since the hyperparameter <code>k_folds</code> is not used in the <code>PyTorch</code> tutorial, it is de-activated here by setting the lower and upper bound to the same value. Note, <code>k_folds</code> is of type “integer”.</p>
-<div class="cell" data-execution_count="9">
-<div class="sourceCode cell-code" id="cb16"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb16-1"><a href="#cb16-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"batch_size"</span>, bounds<span class="op">=</span>[<span class="dv">1</span>, <span class="dv">5</span>])</span>
-<span id="cb16-2"><a href="#cb16-2" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"k_folds"</span>, bounds<span class="op">=</span>[<span class="dv">0</span>, <span class="dv">0</span>])</span>
-<span id="cb16-3"><a href="#cb16-3" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"patience"</span>, bounds<span class="op">=</span>[<span class="dv">3</span>, <span class="dv">3</span>])</span>
-<span id="cb16-4"><a href="#cb16-4" aria-hidden="true" tabindex="-1"></a>fun_control[<span class="st">"core_model_hyper_dict"</span>]</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="17">
+<div class="sourceCode cell-code" id="cb24"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb24-1"><a href="#cb24-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"batch_size"</span>, bounds<span class="op">=</span>[<span class="dv">1</span>, <span class="dv">5</span>])</span>
+<span id="cb24-2"><a href="#cb24-2" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"k_folds"</span>, bounds<span class="op">=</span>[<span class="dv">0</span>, <span class="dv">0</span>])</span>
+<span id="cb24-3"><a href="#cb24-3" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"patience"</span>, bounds<span class="op">=</span>[<span class="dv">3</span>, <span class="dv">3</span>])</span>
+<span id="cb24-4"><a href="#cb24-4" aria-hidden="true" tabindex="-1"></a>fun_control[<span class="st">"core_model_hyper_dict"</span>]</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 <section id="modify-hyperparameter-of-type-factor" class="level3">
 <h3 class="anchored" data-anchor-id="modify-hyperparameter-of-type-factor">Modify Hyperparameter of Type factor</h3>
 <p>In a similar manner as for the numerical hyperparameters, the categorical hyperparameters can be modified. New configurations can be chosen by adding or deleting levels. For example, the hyperparameter <code>optimizer</code> can be re-configured as follows:</p>
 <p>In the following setting, two optimizers (<code>"SGD"</code> and <code>"Adam"</code>) will be compared during the <code>spotPython</code> hyperparameter tuning. The hyperparameter <code>optimizer</code> is active.</p>
-<div class="cell" data-execution_count="10">
-<div class="sourceCode cell-code" id="cb17"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb17-1"><a href="#cb17-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>, [<span class="st">"SGD"</span>, <span class="st">"Adam"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="18">
+<div class="sourceCode cell-code" id="cb25"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb25-1"><a href="#cb25-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>, [<span class="st">"SGD"</span>, <span class="st">"Adam"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>The hyperparameter <code>optimizer</code> can be de-activated by choosing only one value (level), here: <code>"SGD"</code>.</p>
-<div class="cell" data-execution_count="11">
-<div class="sourceCode cell-code" id="cb18"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb18-1"><a href="#cb18-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>, [<span class="st">"SGD"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="19">
+<div class="sourceCode cell-code" id="cb26"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb26-1"><a href="#cb26-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>, [<span class="st">"SGD"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
-<p>As discussed in <a href="#sec-optimizers">Section&nbsp;3.7.4</a>, there are some issues with the LBFGS optimizer. Therefore, the usage of the LBFGS optimizer is not deactivated in <code>spotPython</code> by default. However, the LBFGS optimizer can be activated by adding it to the list of optimizers. <code>Rprop</code> was removed, because it does perform very poorly (as some pre-tests have shown). However, it can also be activated by adding it to the list of optimizers. Since <code>SparseAdam</code> does not support dense gradients, <code>Adam</code> was used instead. Therefore, there are 10 default optimizers:</p>
-<div class="cell" data-execution_count="12">
-<div class="sourceCode cell-code" id="cb19"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb19-1"><a href="#cb19-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>,[<span class="st">"Adadelta"</span>,</span>
-<span id="cb19-2"><a href="#cb19-2" aria-hidden="true" tabindex="-1"></a>     <span class="st">"Adagrad"</span>, <span class="st">"Adam"</span>, <span class="st">"AdamW"</span>, <span class="st">"Adamax"</span>, <span class="st">"ASGD"</span>, <span class="st">"NAdam"</span>, <span class="st">"RAdam"</span>,</span>
-<span id="cb19-3"><a href="#cb19-3" aria-hidden="true" tabindex="-1"></a>      <span class="st">"RMSprop"</span>, <span class="st">"SGD"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<p>As discussed in <a href="#sec-optimizers">Section&nbsp;4.7.4</a>, there are some issues with the LBFGS optimizer. Therefore, the usage of the LBFGS optimizer is not deactivated in <code>spotPython</code> by default. However, the LBFGS optimizer can be activated by adding it to the list of optimizers. <code>Rprop</code> was removed, because it does perform very poorly (as some pre-tests have shown). However, it can also be activated by adding it to the list of optimizers. Since <code>SparseAdam</code> does not support dense gradients, <code>Adam</code> was used instead. Therefore, there are 10 default optimizers:</p>
+<div class="cell" data-execution_count="20">
+<div class="sourceCode cell-code" id="cb27"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb27-1"><a href="#cb27-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_levels(fun_control, <span class="st">"optimizer"</span>,[<span class="st">"Adadelta"</span>,</span>
+<span id="cb27-2"><a href="#cb27-2" aria-hidden="true" tabindex="-1"></a>     <span class="st">"Adagrad"</span>, <span class="st">"Adam"</span>, <span class="st">"AdamW"</span>, <span class="st">"Adamax"</span>, <span class="st">"ASGD"</span>, <span class="st">"NAdam"</span>, <span class="st">"RAdam"</span>,</span>
+<span id="cb27-3"><a href="#cb27-3" aria-hidden="true" tabindex="-1"></a>      <span class="st">"RMSprop"</span>, <span class="st">"SGD"</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 <section id="sec-optimizers" class="level3">
 <h3 class="anchored" data-anchor-id="sec-optimizers">Optimizers</h3>
 <p><a href="#tbl-optimizers">Table&nbsp;1</a> shows some of the optimizers available in <code>PyTorch</code>:</p>
 <div id="tbl-optimizers" class="anchored">
 <table class="table">
@@ -819,22 +962,22 @@
 <i class="callout-icon"></i>
 </div>
 <div class="callout-title-container flex-fill">
 A note on the learning rate
 </div>
 </div>
 <div class="callout-body-container callout-body">
-<p><code>spotPython</code> provides a multiplier for the default learning rates, because optimizers use different learning rates. Using a multiplier for the learning rates might enable a simultaneous tuning of the learning rates for all optimizers. However, this is not recommended, because the learning rates are not comparable across optimizers. Therefore, we recommend fixing the learning rate for all optimizers if multiple optimizers are used. This can be done by setting the lower and upper bounds of the learning rate multiplier to the same value as shown below.</p>
+<p><code>spotPython</code> provides a multiplier for the default learning rates, <code>lr_mult</code>, because optimizers use different learning rates. Using a multiplier for the learning rates might enable a simultaneous tuning of the learning rates for all optimizers. However, this is not recommended, because the learning rates are not comparable across optimizers. Therefore, we recommend fixing the learning rate for all optimizers if multiple optimizers are used. This can be done by setting the lower and upper bounds of the learning rate multiplier to the same value as shown below.</p>
 </div>
 </div>
 <p>Thus, the learning rate, which affects the <code>SGD</code> optimizer, will be set to a fixed value. We choose the default value of <code>1e-3</code> for the learning rate, because it is used in other <code>PyTorch</code> examples (it is also the default value used by <code>spotPython</code> as defined in the <code>optimizer_handler()</code> method). We recommend tuning the learning rate later, when a reduced set of optimizers is fixed. Here, we will demonstrate how to select in a screening phase the optimizers that should be used for the hyperparameter tuning.</p>
 <p>For the same reason, we will fix the <code>sgd_momentum</code> to <code>0.9</code>.</p>
-<div class="cell" data-execution_count="13">
-<div class="sourceCode cell-code" id="cb20"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb20-1"><a href="#cb20-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"lr_mult"</span>, bounds<span class="op">=</span>[<span class="fl">1.0</span>, <span class="fl">1.0</span>])</span>
-<span id="cb20-2"><a href="#cb20-2" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"sgd_momentum"</span>, bounds<span class="op">=</span>[<span class="fl">0.9</span>, <span class="fl">0.9</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="21">
+<div class="sourceCode cell-code" id="cb28"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb28-1"><a href="#cb28-1" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"lr_mult"</span>, bounds<span class="op">=</span>[<span class="fl">1.0</span>, <span class="fl">1.0</span>])</span>
+<span id="cb28-2"><a href="#cb28-2" aria-hidden="true" tabindex="-1"></a>fun_control <span class="op">=</span> modify_hyper_parameter_bounds(fun_control, <span class="st">"sgd_momentum"</span>, bounds<span class="op">=</span>[<span class="fl">0.9</span>, <span class="fl">0.9</span>])</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 </section>
 <section id="sec-selection-of-target-function" class="level2">
 <h2 class="anchored" data-anchor-id="sec-selection-of-target-function">Evaluation</h2>
 <p>The evaluation procedure requires the specification of two elements:</p>
 <ol type="1">
@@ -853,19 +996,19 @@
 <i class="callout-icon"></i>
 </div>
 <div class="callout-title-container flex-fill">
 Note
 </div>
 </div>
 <div class="callout-body-container callout-body">
-<p><code>spotPython</code> returns the hyperparameters of the machine learning and deep learning models, e.g., number of layers, learning rate, or optimizer, but not the model weights. Therefore, after the SPOT run is finished, the corresponding model has to be trained again with the best hyperparameter configuration. The training is performed on the training data set. The test data set is used for the final evaluation of the model.</p>
+<p><code>spotPython</code> returns the hyperparameters of the machine learning and deep learning models, e.g., number of layers, learning rate, or optimizer, but not the model weights. Therefore, after the SPOT run is finished, the corresponding model with the optimized architecture has to be trained again with the best hyperparameter configuration. The training is performed on the training data set. The test data set is used for the final evaluation of the model.</p>
 <p>Summarizing, the following splits are performed in the hold-out setting:</p>
 <ol type="1">
 <li>Run <code>spotPython</code> with <code>eval</code> set to <code>train_hold_out</code> to determine the best hyperparameter configuration.</li>
-<li>Train the model with the best hyperparameter configuration on the training data set:
+<li>Train the model with the best hyperparameter configuration (“architecture”) on the training data set:
 <ul>
 <li><code>train_tuned(model_spot, train, "model_spot.pt")</code>.</li>
 </ul></li>
 <li>Test the model on the test data:
 <ul>
 <li><code>test_tuned(model_spot, test, "model_spot.pt")</code></li>
 </ul></li>
@@ -947,357 +1090,89 @@
 </tr>
 </tbody>
 </table>
 </div>
 <ul>
 <li><code>"train_cv"</code> and <code>"test_cv"</code> use <code>sklearn.model_selection.KFold()</code> internally.</li>
 </ul>
+<p><a href="#sec-data-splitting">Section&nbsp;6.2</a> (in the Appendix) provides more details on the data splitting.</p>
 </section>
 </section>
-<section id="detailed-description-of-the-train_hold_out-setting" class="level4">
-<h4 class="anchored" data-anchor-id="detailed-description-of-the-train_hold_out-setting">Detailed Description of the <code>"train_hold_out"</code> Setting</h4>
-<p>The <code>"train_hold_out"</code> setting is used by default. It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
-<ol type="1">
-<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
-<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_hold_out()</code> as follows:</li>
-</ol>
-<div class="cell" data-execution_count="14">
-<div class="sourceCode cell-code" id="cb21"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb21-1"><a href="#cb21-1" aria-hidden="true" tabindex="-1"></a>df_eval, _ <span class="op">=</span> evaluate_hold_out(</span>
-<span id="cb21-2"><a href="#cb21-2" aria-hidden="true" tabindex="-1"></a>    model,</span>
-<span id="cb21-3"><a href="#cb21-3" aria-hidden="true" tabindex="-1"></a>    train_dataset<span class="op">=</span>fun_control[<span class="st">"train"</span>],</span>
-<span id="cb21-4"><a href="#cb21-4" aria-hidden="true" tabindex="-1"></a>    shuffle<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"shuffle"</span>],</span>
-<span id="cb21-5"><a href="#cb21-5" aria-hidden="true" tabindex="-1"></a>    loss_function<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"loss_function"</span>],</span>
-<span id="cb21-6"><a href="#cb21-6" aria-hidden="true" tabindex="-1"></a>    metric<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"metric_torch"</span>],</span>
-<span id="cb21-7"><a href="#cb21-7" aria-hidden="true" tabindex="-1"></a>    device<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"device"</span>],</span>
-<span id="cb21-8"><a href="#cb21-8" aria-hidden="true" tabindex="-1"></a>    show_batch_interval<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"show_batch_interval"</span>],</span>
-<span id="cb21-9"><a href="#cb21-9" aria-hidden="true" tabindex="-1"></a>    path<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"path"</span>],</span>
-<span id="cb21-10"><a href="#cb21-10" aria-hidden="true" tabindex="-1"></a>) </span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p>Note: Only the data set <code>fun_control["train"]</code> is used for training and validation. It is used as follows:</p>
-<div class="cell" data-execution_count="15">
-<div class="sourceCode cell-code" id="cb22"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb22-1"><a href="#cb22-1" aria-hidden="true" tabindex="-1"></a>trainloader, valloader <span class="op">=</span> create_train_val_data_loaders(</span>
-<span id="cb22-2"><a href="#cb22-2" aria-hidden="true" tabindex="-1"></a>                dataset<span class="op">=</span>train_dataset, batch_size<span class="op">=</span>batch_size_instance, shuffle<span class="op">=</span>shuffle</span>
-<span id="cb22-3"><a href="#cb22-3" aria-hidden="true" tabindex="-1"></a>            )</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p><code>create_train_val_data_loaders()</code> splits the <code>train_dataset</code> into <code>trainloader</code> and <code>valloader</code> using <code>torch.utils.data.random_split()</code> as follows:</p>
-<div class="cell" data-execution_count="16">
-<div class="sourceCode cell-code" id="cb23"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb23-1"><a href="#cb23-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers<span class="op">=</span><span class="dv">0</span>):</span>
-<span id="cb23-2"><a href="#cb23-2" aria-hidden="true" tabindex="-1"></a>    test_abs <span class="op">=</span> <span class="bu">int</span>(<span class="bu">len</span>(dataset) <span class="op">*</span> <span class="fl">0.6</span>)</span>
-<span id="cb23-3"><a href="#cb23-3" aria-hidden="true" tabindex="-1"></a>    train_subset, val_subset <span class="op">=</span> random_split(dataset, [test_abs, <span class="bu">len</span>(dataset) <span class="op">-</span> test_abs])</span>
-<span id="cb23-4"><a href="#cb23-4" aria-hidden="true" tabindex="-1"></a>    trainloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
-<span id="cb23-5"><a href="#cb23-5" aria-hidden="true" tabindex="-1"></a>        train_subset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
-<span id="cb23-6"><a href="#cb23-6" aria-hidden="true" tabindex="-1"></a>    )</span>
-<span id="cb23-7"><a href="#cb23-7" aria-hidden="true" tabindex="-1"></a>    valloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
-<span id="cb23-8"><a href="#cb23-8" aria-hidden="true" tabindex="-1"></a>        val_subset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
-<span id="cb23-9"><a href="#cb23-9" aria-hidden="true" tabindex="-1"></a>    )</span>
-<span id="cb23-10"><a href="#cb23-10" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> trainloader, valloader</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p>The optimizer is set up as follows:</p>
-<div class="cell" data-execution_count="17">
-<div class="sourceCode cell-code" id="cb24"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb24-1"><a href="#cb24-1" aria-hidden="true" tabindex="-1"></a>lr_mult_instance <span class="op">=</span> net.lr_mult</span>
-<span id="cb24-2"><a href="#cb24-2" aria-hidden="true" tabindex="-1"></a>optimizer <span class="op">=</span> optimizer_handler(optimizer_name<span class="op">=</span>optimizer_instance, params<span class="op">=</span>net.parameters(), lr_mult<span class="op">=</span>lr_mult_instance)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<ol start="3" type="1">
-<li><code>evaluate_hold_out()</code> sets the <code>net</code> attributes such as <code>epochs</code>, <code>batch_size</code>, <code>optimizer</code>, and <code>patience</code>. For each epoch, the methods <code>train_hold_out()</code> and <code>validate_fold_or_hold_out()</code> are called, the former for training and the latter for validation and early stopping. The validation loss from the last epoch (not the best validation loss) is returned from <code>evaluate_hold_out</code>.</li>
-<li>The method <code>train_hold_out()</code> is implemented as follows:</li>
-</ol>
-<div class="cell" data-execution_count="18">
-<div class="sourceCode cell-code" id="cb25"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb25-1"><a href="#cb25-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> train_hold_out(net, trainloader, batch_size, loss_function, optimizer, device, show_batch_interval<span class="op">=</span><span class="dv">10_000</span>):</span>
-<span id="cb25-2"><a href="#cb25-2" aria-hidden="true" tabindex="-1"></a>    running_loss <span class="op">=</span> <span class="fl">0.0</span></span>
-<span id="cb25-3"><a href="#cb25-3" aria-hidden="true" tabindex="-1"></a>    epoch_steps <span class="op">=</span> <span class="dv">0</span></span>
-<span id="cb25-4"><a href="#cb25-4" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> i, data <span class="kw">in</span> <span class="bu">enumerate</span>(trainloader, <span class="dv">0</span>):</span>
-<span id="cb25-5"><a href="#cb25-5" aria-hidden="true" tabindex="-1"></a>        inputs, labels <span class="op">=</span> data</span>
-<span id="cb25-6"><a href="#cb25-6" aria-hidden="true" tabindex="-1"></a>        inputs, labels <span class="op">=</span> inputs.to(device), labels.to(device)</span>
-<span id="cb25-7"><a href="#cb25-7" aria-hidden="true" tabindex="-1"></a>        optimizer.zero_grad()</span>
-<span id="cb25-8"><a href="#cb25-8" aria-hidden="true" tabindex="-1"></a>        outputs <span class="op">=</span> net(inputs)</span>
-<span id="cb25-9"><a href="#cb25-9" aria-hidden="true" tabindex="-1"></a>        loss <span class="op">=</span> loss_function(outputs, labels)</span>
-<span id="cb25-10"><a href="#cb25-10" aria-hidden="true" tabindex="-1"></a>        loss.backward()</span>
-<span id="cb25-11"><a href="#cb25-11" aria-hidden="true" tabindex="-1"></a>        torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm<span class="op">=</span><span class="fl">1.0</span>)</span>
-<span id="cb25-12"><a href="#cb25-12" aria-hidden="true" tabindex="-1"></a>        optimizer.step()</span>
-<span id="cb25-13"><a href="#cb25-13" aria-hidden="true" tabindex="-1"></a>        running_loss <span class="op">+=</span> loss.item()</span>
-<span id="cb25-14"><a href="#cb25-14" aria-hidden="true" tabindex="-1"></a>        epoch_steps <span class="op">+=</span> <span class="dv">1</span></span>
-<span id="cb25-15"><a href="#cb25-15" aria-hidden="true" tabindex="-1"></a>        <span class="cf">if</span> i <span class="op">%</span> show_batch_interval <span class="op">==</span> (show_batch_interval <span class="op">-</span> <span class="dv">1</span>):  <span class="co"># print every show_batch_interval mini-batches</span></span>
-<span id="cb25-16"><a href="#cb25-16" aria-hidden="true" tabindex="-1"></a>            <span class="bu">print</span>(</span>
-<span id="cb25-17"><a href="#cb25-17" aria-hidden="true" tabindex="-1"></a>                <span class="st">"Batch: </span><span class="sc">%5d</span><span class="st">. Batch Size: </span><span class="sc">%d</span><span class="st">. Training Loss (running): </span><span class="sc">%.3f</span><span class="st">"</span></span>
-<span id="cb25-18"><a href="#cb25-18" aria-hidden="true" tabindex="-1"></a>                <span class="op">%</span> (i <span class="op">+</span> <span class="dv">1</span>, <span class="bu">int</span>(batch_size), running_loss <span class="op">/</span> epoch_steps)</span>
-<span id="cb25-19"><a href="#cb25-19" aria-hidden="true" tabindex="-1"></a>            )</span>
-<span id="cb25-20"><a href="#cb25-20" aria-hidden="true" tabindex="-1"></a>            running_loss <span class="op">=</span> <span class="fl">0.0</span></span>
-<span id="cb25-21"><a href="#cb25-21" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> loss.item()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<ol start="5" type="1">
-<li>The method <code>validate_fold_or_hold_out()</code> is implemented as follows:</li>
-</ol>
-<div class="cell" data-execution_count="19">
-<div class="sourceCode cell-code" id="cb26"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb26-1"><a href="#cb26-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> validate_fold_or_hold_out(net, valloader, loss_function, metric, device):</span>
-<span id="cb26-2"><a href="#cb26-2" aria-hidden="true" tabindex="-1"></a>    val_loss <span class="op">=</span> <span class="fl">0.0</span></span>
-<span id="cb26-3"><a href="#cb26-3" aria-hidden="true" tabindex="-1"></a>    val_steps <span class="op">=</span> <span class="dv">0</span></span>
-<span id="cb26-4"><a href="#cb26-4" aria-hidden="true" tabindex="-1"></a>    metric.reset()</span>
-<span id="cb26-5"><a href="#cb26-5" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> i, data <span class="kw">in</span> <span class="bu">enumerate</span>(valloader, <span class="dv">0</span>):</span>
-<span id="cb26-6"><a href="#cb26-6" aria-hidden="true" tabindex="-1"></a>        <span class="cf">with</span> torch.no_grad():</span>
-<span id="cb26-7"><a href="#cb26-7" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> data</span>
-<span id="cb26-8"><a href="#cb26-8" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> inputs.to(device), labels.to(device)</span>
-<span id="cb26-9"><a href="#cb26-9" aria-hidden="true" tabindex="-1"></a>            outputs <span class="op">=</span> net(inputs)</span>
-<span id="cb26-10"><a href="#cb26-10" aria-hidden="true" tabindex="-1"></a>            _, predicted <span class="op">=</span> torch.<span class="bu">max</span>(outputs.data, <span class="dv">1</span>)</span>
-<span id="cb26-11"><a href="#cb26-11" aria-hidden="true" tabindex="-1"></a>            metric_value <span class="op">=</span> metric(predicted, labels).to(device)</span>
-<span id="cb26-12"><a href="#cb26-12" aria-hidden="true" tabindex="-1"></a>            loss <span class="op">=</span> loss_function(outputs, labels)</span>
-<span id="cb26-13"><a href="#cb26-13" aria-hidden="true" tabindex="-1"></a>            val_loss <span class="op">+=</span> loss.cpu().numpy()</span>
-<span id="cb26-14"><a href="#cb26-14" aria-hidden="true" tabindex="-1"></a>            val_steps <span class="op">+=</span> <span class="dv">1</span></span>
-<span id="cb26-15"><a href="#cb26-15" aria-hidden="true" tabindex="-1"></a>    loss <span class="op">=</span> val_loss <span class="op">/</span> val_steps</span>
-<span id="cb26-16"><a href="#cb26-16" aria-hidden="true" tabindex="-1"></a>    metric_value <span class="op">=</span> metric.compute()</span>
-<span id="cb26-17"><a href="#cb26-17" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> metric_value, loss</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-</section>
-<section id="detailed-description-of-the-test_hold_out-setting" class="level4">
-<h4 class="anchored" data-anchor-id="detailed-description-of-the-test_hold_out-setting">Detailed Description of the <code>"test_hold_out"</code> Setting</h4>
-<p>It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
-<ol type="1">
-<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
-<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_hold_out()</code> similar to the <code>"train_hold_out"</code> setting with one exception: It passes an additional <code>test</code> data set to <code>evaluate_hold_out()</code> as follows:</li>
-</ol>
-<div class="cell" data-execution_count="20">
-<div class="sourceCode cell-code" id="cb27"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb27-1"><a href="#cb27-1" aria-hidden="true" tabindex="-1"></a>test_dataset<span class="op">=</span>fun_control[<span class="st">"test"</span>]</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p><code>evaluate_hold_out()</code> calls <code>create_train_test_data_loaders</code> instead of <code>create_train_val_data_loaders</code> as follows: The two data sets are used in <code>create_train_test_data_loaders</code> as follows:</p>
-<div class="cell" data-execution_count="21">
-<div class="sourceCode cell-code" id="cb28"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb28-1"><a href="#cb28-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset, num_workers<span class="op">=</span><span class="dv">0</span>):</span>
-<span id="cb28-2"><a href="#cb28-2" aria-hidden="true" tabindex="-1"></a>    trainloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
-<span id="cb28-3"><a href="#cb28-3" aria-hidden="true" tabindex="-1"></a>        dataset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
-<span id="cb28-4"><a href="#cb28-4" aria-hidden="true" tabindex="-1"></a>    )</span>
-<span id="cb28-5"><a href="#cb28-5" aria-hidden="true" tabindex="-1"></a>    testloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
-<span id="cb28-6"><a href="#cb28-6" aria-hidden="true" tabindex="-1"></a>        test_dataset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
-<span id="cb28-7"><a href="#cb28-7" aria-hidden="true" tabindex="-1"></a>    )</span>
-<span id="cb28-8"><a href="#cb28-8" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> trainloader, testloader</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<ol start="3" type="1">
-<li>The following steps are identical to the <code>"train_hold_out"</code> setting. Only a different data loader is used for testing.</li>
-</ol>
-</section>
-<section id="detailed-description-of-the-train_cv-setting" class="level4">
-<h4 class="anchored" data-anchor-id="detailed-description-of-the-train_cv-setting">Detailed Description of the <code>"train_cv"</code> Setting</h4>
-<p>It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
-<ol type="1">
-<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
-<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_cv()</code> as follows:</li>
-</ol>
-<div class="cell" data-execution_count="22">
-<div class="sourceCode cell-code" id="cb29"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb29-1"><a href="#cb29-1" aria-hidden="true" tabindex="-1"></a>df_eval, _ <span class="op">=</span> evaluate_cv(</span>
-<span id="cb29-2"><a href="#cb29-2" aria-hidden="true" tabindex="-1"></a>    model,</span>
-<span id="cb29-3"><a href="#cb29-3" aria-hidden="true" tabindex="-1"></a>    dataset<span class="op">=</span>fun_control[<span class="st">"train"</span>],</span>
-<span id="cb29-4"><a href="#cb29-4" aria-hidden="true" tabindex="-1"></a>    shuffle<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"shuffle"</span>],</span>
-<span id="cb29-5"><a href="#cb29-5" aria-hidden="true" tabindex="-1"></a>    device<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"device"</span>],</span>
-<span id="cb29-6"><a href="#cb29-6" aria-hidden="true" tabindex="-1"></a>    show_batch_interval<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"show_batch_interval"</span>],</span>
-<span id="cb29-7"><a href="#cb29-7" aria-hidden="true" tabindex="-1"></a>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p>Note: Only the data set <code>fun_control["train"]</code> is used for CV. 3. In `evaluate_cv(), the following steps are performed: The optimizer is set up as follows:</p>
-<div class="cell" data-execution_count="23">
-<div class="sourceCode cell-code" id="cb30"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb30-1"><a href="#cb30-1" aria-hidden="true" tabindex="-1"></a>lr_instance <span class="op">=</span> net.lr</span>
-<span id="cb30-2"><a href="#cb30-2" aria-hidden="true" tabindex="-1"></a>optimizer <span class="op">=</span> optimizer_handler(optimizer_name<span class="op">=</span>optimizer_instance, params<span class="op">=</span>net.parameters(), lr_mult<span class="op">=</span>lr_mult_instance)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p><code>evaluate_cv()</code> sets the <code>net</code> attributes such as <code>epochs</code>, <code>batch_size</code>, <code>optimizer</code>, and <code>patience</code>. CV is implemented as follows:</p>
-<div class="cell" data-execution_count="24">
-<div class="sourceCode cell-code" id="cb31"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb31-1"><a href="#cb31-1" aria-hidden="true" tabindex="-1"></a>kfold <span class="op">=</span> KFold(n_splits<span class="op">=</span>k_folds_instance, shuffle<span class="op">=</span>shuffle)</span>
-<span id="cb31-2"><a href="#cb31-2" aria-hidden="true" tabindex="-1"></a><span class="cf">for</span> fold, (train_ids, val_ids) <span class="kw">in</span> <span class="bu">enumerate</span>(kfold.split(dataset)):</span>
-<span id="cb31-3"><a href="#cb31-3" aria-hidden="true" tabindex="-1"></a>    train_subsampler <span class="op">=</span> torch.utils.data.SubsetRandomSampler(train_ids)</span>
-<span id="cb31-4"><a href="#cb31-4" aria-hidden="true" tabindex="-1"></a>    val_subsampler <span class="op">=</span> torch.utils.data.SubsetRandomSampler(val_ids)</span>
-<span id="cb31-5"><a href="#cb31-5" aria-hidden="true" tabindex="-1"></a>    trainloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
-<span id="cb31-6"><a href="#cb31-6" aria-hidden="true" tabindex="-1"></a>        dataset, batch_size<span class="op">=</span>batch_size_instance, sampler<span class="op">=</span>train_subsampler, num_workers<span class="op">=</span>num_workers</span>
-<span id="cb31-7"><a href="#cb31-7" aria-hidden="true" tabindex="-1"></a>    )</span>
-<span id="cb31-8"><a href="#cb31-8" aria-hidden="true" tabindex="-1"></a>    valloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
-<span id="cb31-9"><a href="#cb31-9" aria-hidden="true" tabindex="-1"></a>        dataset, batch_size<span class="op">=</span>batch_size_instance, sampler<span class="op">=</span>val_subsampler, num_workers<span class="op">=</span>num_workers</span>
-<span id="cb31-10"><a href="#cb31-10" aria-hidden="true" tabindex="-1"></a>    )</span>
-<span id="cb31-11"><a href="#cb31-11" aria-hidden="true" tabindex="-1"></a>    reset_weights(net)</span>
-<span id="cb31-12"><a href="#cb31-12" aria-hidden="true" tabindex="-1"></a>    <span class="co"># Train fold for several epochs:</span></span>
-<span id="cb31-13"><a href="#cb31-13" aria-hidden="true" tabindex="-1"></a>    train_fold(</span>
-<span id="cb31-14"><a href="#cb31-14" aria-hidden="true" tabindex="-1"></a>        net,</span>
-<span id="cb31-15"><a href="#cb31-15" aria-hidden="true" tabindex="-1"></a>        trainloader,</span>
-<span id="cb31-16"><a href="#cb31-16" aria-hidden="true" tabindex="-1"></a>        epochs_instance,</span>
-<span id="cb31-17"><a href="#cb31-17" aria-hidden="true" tabindex="-1"></a>        loss_function,</span>
-<span id="cb31-18"><a href="#cb31-18" aria-hidden="true" tabindex="-1"></a>        optimizer,</span>
-<span id="cb31-19"><a href="#cb31-19" aria-hidden="true" tabindex="-1"></a>        device,</span>
-<span id="cb31-20"><a href="#cb31-20" aria-hidden="true" tabindex="-1"></a>        show_batch_interval<span class="op">=</span>show_batch_interval,</span>
-<span id="cb31-21"><a href="#cb31-21" aria-hidden="true" tabindex="-1"></a>    )</span>
-<span id="cb31-22"><a href="#cb31-22" aria-hidden="true" tabindex="-1"></a>    <span class="co"># Validate fold: use only loss for tuning</span></span>
-<span id="cb31-23"><a href="#cb31-23" aria-hidden="true" tabindex="-1"></a>    metric_values[fold], loss_values[fold] <span class="op">=</span> validate_fold_or_hold_out(net, valloader, loss_function, device)</span>
-<span id="cb31-24"><a href="#cb31-24" aria-hidden="true" tabindex="-1"></a>df_eval <span class="op">=</span> <span class="bu">sum</span>(loss_values.values()) <span class="op">/</span> <span class="bu">len</span>(loss_values.values())</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<ol start="4" type="1">
-<li>The method <code>train_fold()</code> is implemented as follows:</li>
-</ol>
-<div class="cell" data-execution_count="25">
-<div class="sourceCode cell-code" id="cb32"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb32-1"><a href="#cb32-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interval<span class="op">=</span><span class="dv">10_000</span>):</span>
-<span id="cb32-2"><a href="#cb32-2" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> epoch <span class="kw">in</span> <span class="bu">range</span>(epochs):</span>
-<span id="cb32-3"><a href="#cb32-3" aria-hidden="true" tabindex="-1"></a>        <span class="bu">print</span>(<span class="ss">f"Epoch: </span><span class="sc">{</span>epoch <span class="op">+</span> <span class="dv">1</span><span class="sc">}</span><span class="ss">"</span>)</span>
-<span id="cb32-4"><a href="#cb32-4" aria-hidden="true" tabindex="-1"></a>        running_loss <span class="op">=</span> <span class="fl">0.0</span></span>
-<span id="cb32-5"><a href="#cb32-5" aria-hidden="true" tabindex="-1"></a>        epoch_steps <span class="op">=</span> <span class="dv">0</span></span>
-<span id="cb32-6"><a href="#cb32-6" aria-hidden="true" tabindex="-1"></a>        <span class="cf">for</span> i, data <span class="kw">in</span> <span class="bu">enumerate</span>(trainloader, <span class="dv">0</span>):</span>
-<span id="cb32-7"><a href="#cb32-7" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> data</span>
-<span id="cb32-8"><a href="#cb32-8" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> inputs.to(device), labels.to(device)</span>
-<span id="cb32-9"><a href="#cb32-9" aria-hidden="true" tabindex="-1"></a>            optimizer.zero_grad()</span>
-<span id="cb32-10"><a href="#cb32-10" aria-hidden="true" tabindex="-1"></a>            outputs <span class="op">=</span> net(inputs)</span>
-<span id="cb32-11"><a href="#cb32-11" aria-hidden="true" tabindex="-1"></a>            loss <span class="op">=</span> loss_function(outputs, labels)</span>
-<span id="cb32-12"><a href="#cb32-12" aria-hidden="true" tabindex="-1"></a>            loss.backward()</span>
-<span id="cb32-13"><a href="#cb32-13" aria-hidden="true" tabindex="-1"></a>            torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm<span class="op">=</span><span class="fl">1.0</span>)</span>
-<span id="cb32-14"><a href="#cb32-14" aria-hidden="true" tabindex="-1"></a>            optimizer.step()</span>
-<span id="cb32-15"><a href="#cb32-15" aria-hidden="true" tabindex="-1"></a>            <span class="co"># the following is for printing the statistic only</span></span>
-<span id="cb32-16"><a href="#cb32-16" aria-hidden="true" tabindex="-1"></a>            running_loss <span class="op">+=</span> loss.item()</span>
-<span id="cb32-17"><a href="#cb32-17" aria-hidden="true" tabindex="-1"></a>            epoch_steps <span class="op">+=</span> <span class="dv">1</span></span>
-<span id="cb32-18"><a href="#cb32-18" aria-hidden="true" tabindex="-1"></a>            <span class="cf">if</span> i <span class="op">%</span> show_batch_interval <span class="op">==</span> (show_batch_interval <span class="op">-</span> <span class="dv">1</span>):  <span class="co"># print every show_batch_interval mini-batches</span></span>
-<span id="cb32-19"><a href="#cb32-19" aria-hidden="true" tabindex="-1"></a>                <span class="bu">print</span>(<span class="st">"Batch: </span><span class="sc">%5d</span><span class="st">. Training Loss (running): </span><span class="sc">%.3f</span><span class="st">"</span> <span class="op">%</span> (i <span class="op">+</span> <span class="dv">1</span>, running_loss <span class="op">/</span> epoch_steps))</span>
-<span id="cb32-20"><a href="#cb32-20" aria-hidden="true" tabindex="-1"></a>                running_loss <span class="op">=</span> <span class="fl">0.0</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<ol start="5" type="1">
-<li>The method <code>validate_fold_or_hold_out()</code> is implemented as shown above. In contrast to the hold-out setting, it is called for each of the <span class="math inline">\(k\)</span> folds. The results are stored in a dictionaries <code>metric_values</code> and <code>loss_values</code> as follows:</li>
-</ol>
-<div class="cell" data-execution_count="26">
-<div class="sourceCode cell-code" id="cb33"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb33-1"><a href="#cb33-1" aria-hidden="true" tabindex="-1"></a>    <span class="co"># Validate fold: use only loss for tuning</span></span>
-<span id="cb33-2"><a href="#cb33-2" aria-hidden="true" tabindex="-1"></a>    metric_values[fold], loss_values[fold] <span class="op">=</span> validate_fold_or_hold_out(net, valloader, loss_function, device)</span>
-<span id="cb33-3"><a href="#cb33-3" aria-hidden="true" tabindex="-1"></a>df_eval <span class="op">=</span> <span class="bu">sum</span>(loss_values.values()) <span class="op">/</span> <span class="bu">len</span>(loss_values.values())</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p>The results are averaged over the <span class="math inline">\(k\)</span> folds and returned as <code>df_eval</code>.</p>
-</section>
-<section id="detailed-description-of-the-test_cv-setting" class="level4">
-<h4 class="anchored" data-anchor-id="detailed-description-of-the-test_cv-setting">Detailed Description of the <code>"test_cv"</code> Setting</h4>
-<p>It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
-<ol type="1">
-<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
-<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_cv()</code> as follows:</li>
-</ol>
-<div class="cell" data-execution_count="27">
-<div class="sourceCode cell-code" id="cb34"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb34-1"><a href="#cb34-1" aria-hidden="true" tabindex="-1"></a>df_eval, _ <span class="op">=</span> evaluate_cv(</span>
-<span id="cb34-2"><a href="#cb34-2" aria-hidden="true" tabindex="-1"></a>    model,</span>
-<span id="cb34-3"><a href="#cb34-3" aria-hidden="true" tabindex="-1"></a>    dataset<span class="op">=</span>fun_control[<span class="st">"test"</span>],</span>
-<span id="cb34-4"><a href="#cb34-4" aria-hidden="true" tabindex="-1"></a>    shuffle<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"shuffle"</span>],</span>
-<span id="cb34-5"><a href="#cb34-5" aria-hidden="true" tabindex="-1"></a>    device<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"device"</span>],</span>
-<span id="cb34-6"><a href="#cb34-6" aria-hidden="true" tabindex="-1"></a>    show_batch_interval<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"show_batch_interval"</span>],</span>
-<span id="cb34-7"><a href="#cb34-7" aria-hidden="true" tabindex="-1"></a>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p>Note: The data set <code>fun_control["test"]</code> is used for CV. The rest is the same as for the <code>"train_cv"</code> setting.</p>
-</section>
 <section id="settings-for-the-final-evaluation-of-the-tuned-architecture" class="level4">
 <h4 class="anchored" data-anchor-id="settings-for-the-final-evaluation-of-the-tuned-architecture">Settings for the Final Evaluation of the Tuned Architecture</h4>
 <section id="training-of-the-tuned-architecture" class="level5">
 <h5 class="anchored" data-anchor-id="training-of-the-tuned-architecture">Training of the Tuned Architecture</h5>
 <p><code>train_tuned(model, train)</code>: train the model with the best hyperparameter configuration (or simply the default) on the training data set. It splits the <code>train</code>data into new <code>train</code> and <code>validation</code> sets using <code>create_train_val_data_loaders()</code>, which calls <code>torch.utils.data.random_split()</code> internally. Currently, 60% of the data is used for training and 40% for validation. The <code>train</code> data is used for training the model with <code>train_hold_out()</code>. The <code>validation</code> data is used for early stopping using <code>validate_fold_or_hold_out()</code> on the <code>validation</code> data set.</p>
-<p><code>train_tuned()</code> is just a wrapper to <code>evaluate_hold_out</code> using the <code>train</code> data set. It is implemented as follows:</p>
-<div class="cell" data-execution_count="28">
-<div class="sourceCode cell-code" id="cb35"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb35-1"><a href="#cb35-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> train_tuned(net, train_dataset, shuffle, loss_function, metric, device<span class="op">=</span><span class="va">None</span>, show_batch_interval<span class="op">=</span><span class="dv">10_000</span>, path<span class="op">=</span><span class="va">None</span>):</span>
-<span id="cb35-2"><a href="#cb35-2" aria-hidden="true" tabindex="-1"></a>    evaluate_hold_out(</span>
-<span id="cb35-3"><a href="#cb35-3" aria-hidden="true" tabindex="-1"></a>        net<span class="op">=</span>net,</span>
-<span id="cb35-4"><a href="#cb35-4" aria-hidden="true" tabindex="-1"></a>        train_dataset<span class="op">=</span>train_dataset,</span>
-<span id="cb35-5"><a href="#cb35-5" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span>shuffle,</span>
-<span id="cb35-6"><a href="#cb35-6" aria-hidden="true" tabindex="-1"></a>        test_dataset<span class="op">=</span><span class="va">None</span>,</span>
-<span id="cb35-7"><a href="#cb35-7" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>loss_function,</span>
-<span id="cb35-8"><a href="#cb35-8" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>metric,</span>
-<span id="cb35-9"><a href="#cb35-9" aria-hidden="true" tabindex="-1"></a>        device<span class="op">=</span>device,</span>
-<span id="cb35-10"><a href="#cb35-10" aria-hidden="true" tabindex="-1"></a>        show_batch_interval<span class="op">=</span>show_batch_interval,</span>
-<span id="cb35-11"><a href="#cb35-11" aria-hidden="true" tabindex="-1"></a>        path<span class="op">=</span>path,</span>
-<span id="cb35-12"><a href="#cb35-12" aria-hidden="true" tabindex="-1"></a>    )</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
-<p>Note: During training, <code>shuffle</code> is set to <code>True</code>, whereas during testing, <code>shuffle</code> is set to <code>False</code>.</p>
 </section>
 <section id="testing-of-the-tuned-architecture" class="level5">
 <h5 class="anchored" data-anchor-id="testing-of-the-tuned-architecture">Testing of the Tuned Architecture</h5>
 <p><code>test_tuned(model, test)</code>: test the model on the test data set. No data splitting is performed. The (trained) model is evaluated using the <code>validate_fold_or_hold_out()</code> function.</p>
 <p>Note: During training, <code>shuffle</code> is set to <code>True</code>, whereas during testing, <code>shuffle</code> is set to <code>False</code>.</p>
-<div class="cell" data-execution_count="29">
-<div class="sourceCode cell-code" id="cb36"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb36-1"><a href="#cb36-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> test_tuned(net, shuffle, test_dataset<span class="op">=</span><span class="va">None</span>, loss_function<span class="op">=</span><span class="va">None</span>, metric<span class="op">=</span><span class="va">None</span>, device<span class="op">=</span><span class="va">None</span>, path<span class="op">=</span><span class="va">None</span>):</span>
-<span id="cb36-2"><a href="#cb36-2" aria-hidden="true" tabindex="-1"></a>    batch_size_instance <span class="op">=</span> net.batch_size</span>
-<span id="cb36-3"><a href="#cb36-3" aria-hidden="true" tabindex="-1"></a>    removed_attributes, net <span class="op">=</span> get_removed_attributes_and_base_net(net)</span>
-<span id="cb36-4"><a href="#cb36-4" aria-hidden="true" tabindex="-1"></a>    <span class="cf">if</span> path <span class="kw">is</span> <span class="kw">not</span> <span class="va">None</span>:</span>
-<span id="cb36-5"><a href="#cb36-5" aria-hidden="true" tabindex="-1"></a>        net.load_state_dict(torch.load(path))</span>
-<span id="cb36-6"><a href="#cb36-6" aria-hidden="true" tabindex="-1"></a>        net.<span class="bu">eval</span>()</span>
-<span id="cb36-7"><a href="#cb36-7" aria-hidden="true" tabindex="-1"></a>    <span class="cf">try</span>:</span>
-<span id="cb36-8"><a href="#cb36-8" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> getDevice(device<span class="op">=</span>device)</span>
-<span id="cb36-9"><a href="#cb36-9" aria-hidden="true" tabindex="-1"></a>        <span class="cf">if</span> torch.cuda.is_available():</span>
-<span id="cb36-10"><a href="#cb36-10" aria-hidden="true" tabindex="-1"></a>            device <span class="op">=</span> <span class="st">"cuda:0"</span></span>
-<span id="cb36-11"><a href="#cb36-11" aria-hidden="true" tabindex="-1"></a>            <span class="cf">if</span> torch.cuda.device_count() <span class="op">&gt;</span> <span class="dv">1</span>:</span>
-<span id="cb36-12"><a href="#cb36-12" aria-hidden="true" tabindex="-1"></a>                <span class="bu">print</span>(<span class="st">"We will use"</span>, torch.cuda.device_count(), <span class="st">"GPUs!"</span>)</span>
-<span id="cb36-13"><a href="#cb36-13" aria-hidden="true" tabindex="-1"></a>                net <span class="op">=</span> nn.DataParallel(net)</span>
-<span id="cb36-14"><a href="#cb36-14" aria-hidden="true" tabindex="-1"></a>        net.to(device)</span>
-<span id="cb36-15"><a href="#cb36-15" aria-hidden="true" tabindex="-1"></a>        valloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
-<span id="cb36-16"><a href="#cb36-16" aria-hidden="true" tabindex="-1"></a>            test_dataset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size_instance), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span><span class="dv">0</span></span>
-<span id="cb36-17"><a href="#cb36-17" aria-hidden="true" tabindex="-1"></a>        )</span>
-<span id="cb36-18"><a href="#cb36-18" aria-hidden="true" tabindex="-1"></a>        metric_value, loss <span class="op">=</span> validate_fold_or_hold_out(</span>
-<span id="cb36-19"><a href="#cb36-19" aria-hidden="true" tabindex="-1"></a>            net, valloader<span class="op">=</span>valloader, loss_function<span class="op">=</span>loss_function, metric<span class="op">=</span>metric, device<span class="op">=</span>device</span>
-<span id="cb36-20"><a href="#cb36-20" aria-hidden="true" tabindex="-1"></a>        )</span>
-<span id="cb36-21"><a href="#cb36-21" aria-hidden="true" tabindex="-1"></a>        df_eval <span class="op">=</span> loss</span>
-<span id="cb36-22"><a href="#cb36-22" aria-hidden="true" tabindex="-1"></a>        df_metric <span class="op">=</span> metric_value</span>
-<span id="cb36-23"><a href="#cb36-23" aria-hidden="true" tabindex="-1"></a>        df_preds <span class="op">=</span> np.nan</span>
-<span id="cb36-24"><a href="#cb36-24" aria-hidden="true" tabindex="-1"></a>    <span class="cf">except</span> <span class="pp">Exception</span> <span class="im">as</span> err:</span>
-<span id="cb36-25"><a href="#cb36-25" aria-hidden="true" tabindex="-1"></a>        <span class="bu">print</span>(<span class="ss">f"Error in Net_Core. Call to test_tuned() failed. </span><span class="sc">{</span>err<span class="op">=</span><span class="sc">}</span><span class="ss">, </span><span class="sc">{</span><span class="bu">type</span>(err)<span class="op">=</span><span class="sc">}</span><span class="ss">"</span>)</span>
-<span id="cb36-26"><a href="#cb36-26" aria-hidden="true" tabindex="-1"></a>        df_eval <span class="op">=</span> np.nan</span>
-<span id="cb36-27"><a href="#cb36-27" aria-hidden="true" tabindex="-1"></a>        df_metric <span class="op">=</span> np.nan</span>
-<span id="cb36-28"><a href="#cb36-28" aria-hidden="true" tabindex="-1"></a>        df_preds <span class="op">=</span> np.nan</span>
-<span id="cb36-29"><a href="#cb36-29" aria-hidden="true" tabindex="-1"></a>    add_attributes(net, removed_attributes)</span>
-<span id="cb36-30"><a href="#cb36-30" aria-hidden="true" tabindex="-1"></a>    <span class="bu">print</span>(<span class="ss">f"Final evaluation: Validation loss: </span><span class="sc">{</span>df_eval<span class="sc">}</span><span class="ss">"</span>)</span>
-<span id="cb36-31"><a href="#cb36-31" aria-hidden="true" tabindex="-1"></a>    <span class="bu">print</span>(<span class="ss">f"Final evaluation: Validation metric: </span><span class="sc">{</span>df_metric<span class="sc">}</span><span class="ss">"</span>)</span>
-<span id="cb36-32"><a href="#cb36-32" aria-hidden="true" tabindex="-1"></a>    <span class="bu">print</span>(<span class="st">"----------------------------------------------"</span>)</span>
-<span id="cb36-33"><a href="#cb36-33" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> df_eval, df_preds, df_metric</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-</div>
+<p><a href="#sec-final-model-evaluation">Section&nbsp;6.2.5</a> describes the final evaluation of the tuned architecture.</p>
 </section>
 </section>
 </section>
 <section id="loss-functions-and-metrics" class="level3">
 <h3 class="anchored" data-anchor-id="loss-functions-and-metrics">Loss Functions and Metrics</h3>
 <p>The key <code>"loss_function"</code> specifies the loss function which is used during the optimization. There are several different loss functions under <code>PyTorch</code>’s <code>nn</code> package. For example, a simple loss is <code>MSELoss</code>, which computes the mean-squared error between the output and the target. In this tutorial we will use <code>CrossEntropyLoss</code>, because it is also used in the <code>PyTorch</code> tutorial.</p>
-<div class="cell" data-execution_count="30">
-<div class="sourceCode cell-code" id="cb37"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb37-1"><a href="#cb37-1" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> torch.nn <span class="im">import</span> CrossEntropyLoss</span>
-<span id="cb37-2"><a href="#cb37-2" aria-hidden="true" tabindex="-1"></a>loss_function <span class="op">=</span> CrossEntropyLoss()</span>
-<span id="cb37-3"><a href="#cb37-3" aria-hidden="true" tabindex="-1"></a>fun_control.update({<span class="st">"loss_function"</span>: loss_function})</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="22">
+<div class="sourceCode cell-code" id="cb29"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb29-1"><a href="#cb29-1" aria-hidden="true" tabindex="-1"></a><span class="im">from</span> torch.nn <span class="im">import</span> CrossEntropyLoss</span>
+<span id="cb29-2"><a href="#cb29-2" aria-hidden="true" tabindex="-1"></a>loss_function <span class="op">=</span> CrossEntropyLoss()</span>
+<span id="cb29-3"><a href="#cb29-3" aria-hidden="true" tabindex="-1"></a>fun_control.update({<span class="st">"loss_function"</span>: loss_function})</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
-<p>In addition to the loss functions, <code>spotPython</code> provides access to a large number of metrics. The key <code>"metric_sklearn"</code> is used for metrics that follow the <code>scikit-learn</code> conventions. The key <code>"river_metric"</code> is used for the river based evaluation <span class="citation" data-cites="mont20a">(<a href="#ref-mont20a" role="doc-biblioref">Montiel et al. 2021</a>)</span> via <code>eval_oml_iter_progressive</code>, and the key <code>"metric_torch"</code> is used for the metrics from <code>TorchMetrics</code>. <code>TorchMetrics</code> is a collection of more than 90 PyTorch metrics<a href="#fn4" class="footnote-ref" id="fnref4" role="doc-noteref"><sup>4</sup></a>. Because the <code>PyTorch</code> tutorial uses the accuracy as metric, we use the same metric here. Currently, accuracy is computed in the tutorial’s example code. We will use <code>TorchMetrics</code> instead, because it offers:</p>
+<p>In addition to the loss functions, <code>spotPython</code> provides access to a large number of metrics. The key <code>"metric_sklearn"</code> is used for metrics that follow the <code>scikit-learn</code> conventions. The key <code>"river_metric"</code> is used for the river based evaluation <span class="citation" data-cites="mont20a">(<a href="#ref-mont20a" role="doc-biblioref">Montiel et al. 2021</a>)</span> via <code>eval_oml_iter_progressive</code>, and the key <code>"metric_torch"</code> is used for the metrics from <code>TorchMetrics</code>. <code>TorchMetrics</code> is a collection of more than 90 PyTorch metrics<a href="#fn4" class="footnote-ref" id="fnref4" role="doc-noteref"><sup>4</sup></a>. Because the <code>PyTorch</code> tutorial uses the accuracy as metric, we use the same metric here. Currently, accuracy is computed in the tutorial’s example code. We will use <code>TorchMetrics</code> instead, because it offers more flexibilty, e.g., it can be used for regression and classification. Furthermore, <code>TorchMetrics</code> offers the following advantages:</p>
 <ul>
 <li>A standardized interface to increase reproducibility</li>
 <li>Reduces Boilerplate</li>
 <li>Distributed-training compatible</li>
 <li>Rigorously tested</li>
 <li>Automatic accumulation over batches</li>
 <li>Automatic synchronization between multiple devices</li>
 </ul>
 <p>Therefore, we set</p>
-<div class="cell" data-execution_count="31">
-<div class="sourceCode cell-code" id="cb38"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb38-1"><a href="#cb38-1" aria-hidden="true" tabindex="-1"></a>metric_torch <span class="op">=</span> torchmetrics.Accuracy(task<span class="op">=</span><span class="st">"multiclass"</span>, num_classes<span class="op">=</span><span class="dv">10</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="23">
+<div class="sourceCode cell-code" id="cb30"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb30-1"><a href="#cb30-1" aria-hidden="true" tabindex="-1"></a>metric_torch <span class="op">=</span> torchmetrics.Accuracy(task<span class="op">=</span><span class="st">"multiclass"</span>, num_classes<span class="op">=</span><span class="dv">10</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
-<div class="cell" data-execution_count="32">
-<div class="sourceCode cell-code" id="cb39"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb39-1"><a href="#cb39-1" aria-hidden="true" tabindex="-1"></a>loss_function <span class="op">=</span> CrossEntropyLoss()</span>
-<span id="cb39-2"><a href="#cb39-2" aria-hidden="true" tabindex="-1"></a>weights <span class="op">=</span> <span class="fl">1.0</span></span>
-<span id="cb39-3"><a href="#cb39-3" aria-hidden="true" tabindex="-1"></a>metric_torch <span class="op">=</span> torchmetrics.Accuracy(task<span class="op">=</span><span class="st">"multiclass"</span>, num_classes<span class="op">=</span><span class="dv">10</span>)</span>
-<span id="cb39-4"><a href="#cb39-4" aria-hidden="true" tabindex="-1"></a>shuffle <span class="op">=</span> <span class="va">True</span></span>
-<span id="cb39-5"><a href="#cb39-5" aria-hidden="true" tabindex="-1"></a><span class="bu">eval</span> <span class="op">=</span> <span class="st">"train_hold_out"</span></span>
-<span id="cb39-6"><a href="#cb39-6" aria-hidden="true" tabindex="-1"></a>device <span class="op">=</span> DEVICE</span>
-<span id="cb39-7"><a href="#cb39-7" aria-hidden="true" tabindex="-1"></a>show_batch_interval <span class="op">=</span> <span class="dv">100_000</span></span>
-<span id="cb39-8"><a href="#cb39-8" aria-hidden="true" tabindex="-1"></a>path<span class="op">=</span><span class="st">"torch_model.pt"</span></span>
-<span id="cb39-9"><a href="#cb39-9" aria-hidden="true" tabindex="-1"></a></span>
-<span id="cb39-10"><a href="#cb39-10" aria-hidden="true" tabindex="-1"></a>fun_control.update({</span>
-<span id="cb39-11"><a href="#cb39-11" aria-hidden="true" tabindex="-1"></a>               <span class="st">"data_dir"</span>: <span class="va">None</span>,</span>
-<span id="cb39-12"><a href="#cb39-12" aria-hidden="true" tabindex="-1"></a>               <span class="st">"checkpoint_dir"</span>: <span class="va">None</span>,</span>
-<span id="cb39-13"><a href="#cb39-13" aria-hidden="true" tabindex="-1"></a>               <span class="st">"horizon"</span>: <span class="va">None</span>,</span>
-<span id="cb39-14"><a href="#cb39-14" aria-hidden="true" tabindex="-1"></a>               <span class="st">"oml_grace_period"</span>: <span class="va">None</span>,</span>
-<span id="cb39-15"><a href="#cb39-15" aria-hidden="true" tabindex="-1"></a>               <span class="st">"weights"</span>: weights,</span>
-<span id="cb39-16"><a href="#cb39-16" aria-hidden="true" tabindex="-1"></a>               <span class="st">"step"</span>: <span class="va">None</span>,</span>
-<span id="cb39-17"><a href="#cb39-17" aria-hidden="true" tabindex="-1"></a>               <span class="st">"log_level"</span>: <span class="dv">50</span>,</span>
-<span id="cb39-18"><a href="#cb39-18" aria-hidden="true" tabindex="-1"></a>               <span class="st">"weight_coeff"</span>: <span class="va">None</span>,</span>
-<span id="cb39-19"><a href="#cb39-19" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_torch"</span>: metric_torch,</span>
-<span id="cb39-20"><a href="#cb39-20" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_river"</span>: <span class="va">None</span>,</span>
-<span id="cb39-21"><a href="#cb39-21" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_sklearn"</span>: <span class="va">None</span>,</span>
-<span id="cb39-22"><a href="#cb39-22" aria-hidden="true" tabindex="-1"></a>               <span class="st">"loss_function"</span>: loss_function,</span>
-<span id="cb39-23"><a href="#cb39-23" aria-hidden="true" tabindex="-1"></a>               <span class="st">"shuffle"</span>: shuffle,</span>
-<span id="cb39-24"><a href="#cb39-24" aria-hidden="true" tabindex="-1"></a>               <span class="st">"eval"</span>: <span class="bu">eval</span>,</span>
-<span id="cb39-25"><a href="#cb39-25" aria-hidden="true" tabindex="-1"></a>               <span class="st">"device"</span>: device,</span>
-<span id="cb39-26"><a href="#cb39-26" aria-hidden="true" tabindex="-1"></a>               <span class="st">"show_batch_interval"</span>: show_batch_interval,</span>
-<span id="cb39-27"><a href="#cb39-27" aria-hidden="true" tabindex="-1"></a>               <span class="st">"path"</span>: path,</span>
-<span id="cb39-28"><a href="#cb39-28" aria-hidden="true" tabindex="-1"></a>               })</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="24">
+<div class="sourceCode cell-code" id="cb31"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb31-1"><a href="#cb31-1" aria-hidden="true" tabindex="-1"></a>loss_function <span class="op">=</span> CrossEntropyLoss()</span>
+<span id="cb31-2"><a href="#cb31-2" aria-hidden="true" tabindex="-1"></a>weights <span class="op">=</span> <span class="fl">1.0</span></span>
+<span id="cb31-3"><a href="#cb31-3" aria-hidden="true" tabindex="-1"></a>metric_torch <span class="op">=</span> torchmetrics.Accuracy(task<span class="op">=</span><span class="st">"multiclass"</span>, num_classes<span class="op">=</span><span class="dv">10</span>)</span>
+<span id="cb31-4"><a href="#cb31-4" aria-hidden="true" tabindex="-1"></a>shuffle <span class="op">=</span> <span class="va">True</span></span>
+<span id="cb31-5"><a href="#cb31-5" aria-hidden="true" tabindex="-1"></a><span class="bu">eval</span> <span class="op">=</span> <span class="st">"train_hold_out"</span></span>
+<span id="cb31-6"><a href="#cb31-6" aria-hidden="true" tabindex="-1"></a>device <span class="op">=</span> DEVICE</span>
+<span id="cb31-7"><a href="#cb31-7" aria-hidden="true" tabindex="-1"></a>show_batch_interval <span class="op">=</span> <span class="dv">100_000</span></span>
+<span id="cb31-8"><a href="#cb31-8" aria-hidden="true" tabindex="-1"></a>path<span class="op">=</span><span class="st">"torch_model.pt"</span></span>
+<span id="cb31-9"><a href="#cb31-9" aria-hidden="true" tabindex="-1"></a></span>
+<span id="cb31-10"><a href="#cb31-10" aria-hidden="true" tabindex="-1"></a>fun_control.update({</span>
+<span id="cb31-11"><a href="#cb31-11" aria-hidden="true" tabindex="-1"></a>               <span class="st">"data_dir"</span>: <span class="va">None</span>,</span>
+<span id="cb31-12"><a href="#cb31-12" aria-hidden="true" tabindex="-1"></a>               <span class="st">"checkpoint_dir"</span>: <span class="va">None</span>,</span>
+<span id="cb31-13"><a href="#cb31-13" aria-hidden="true" tabindex="-1"></a>               <span class="st">"horizon"</span>: <span class="va">None</span>,</span>
+<span id="cb31-14"><a href="#cb31-14" aria-hidden="true" tabindex="-1"></a>               <span class="st">"oml_grace_period"</span>: <span class="va">None</span>,</span>
+<span id="cb31-15"><a href="#cb31-15" aria-hidden="true" tabindex="-1"></a>               <span class="st">"weights"</span>: weights,</span>
+<span id="cb31-16"><a href="#cb31-16" aria-hidden="true" tabindex="-1"></a>               <span class="st">"step"</span>: <span class="va">None</span>,</span>
+<span id="cb31-17"><a href="#cb31-17" aria-hidden="true" tabindex="-1"></a>               <span class="st">"log_level"</span>: <span class="dv">50</span>,</span>
+<span id="cb31-18"><a href="#cb31-18" aria-hidden="true" tabindex="-1"></a>               <span class="st">"weight_coeff"</span>: <span class="va">None</span>,</span>
+<span id="cb31-19"><a href="#cb31-19" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_torch"</span>: metric_torch,</span>
+<span id="cb31-20"><a href="#cb31-20" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_river"</span>: <span class="va">None</span>,</span>
+<span id="cb31-21"><a href="#cb31-21" aria-hidden="true" tabindex="-1"></a>               <span class="st">"metric_sklearn"</span>: <span class="va">None</span>,</span>
+<span id="cb31-22"><a href="#cb31-22" aria-hidden="true" tabindex="-1"></a>               <span class="st">"loss_function"</span>: loss_function,</span>
+<span id="cb31-23"><a href="#cb31-23" aria-hidden="true" tabindex="-1"></a>               <span class="st">"shuffle"</span>: shuffle,</span>
+<span id="cb31-24"><a href="#cb31-24" aria-hidden="true" tabindex="-1"></a>               <span class="st">"eval"</span>: <span class="bu">eval</span>,</span>
+<span id="cb31-25"><a href="#cb31-25" aria-hidden="true" tabindex="-1"></a>               <span class="st">"device"</span>: device,</span>
+<span id="cb31-26"><a href="#cb31-26" aria-hidden="true" tabindex="-1"></a>               <span class="st">"show_batch_interval"</span>: show_batch_interval,</span>
+<span id="cb31-27"><a href="#cb31-27" aria-hidden="true" tabindex="-1"></a>               <span class="st">"path"</span>: path,</span>
+<span id="cb31-28"><a href="#cb31-28" aria-hidden="true" tabindex="-1"></a>               })</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 </section>
 </section>
 <section id="sec-call-the-hyperparameter-tuner" class="level2">
 <h2 class="anchored" data-anchor-id="sec-call-the-hyperparameter-tuner">Calling the SPOT Function</h2>
 <p>Now, the dictionary <code>fun_control</code> contains all information needed for the hyperparameter tuning. Before the hyperparameter tuning is started, it is recommended to take a look at the experimental design. The method <code>gen_design_table</code> generates a design table as follows:</p>
-<div class="cell" data-execution_count="34">
-<div class="sourceCode cell-code" id="cb40"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb40-1"><a href="#cb40-1" aria-hidden="true" tabindex="-1"></a><span class="bu">print</span>(gen_design_table(fun_control))</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="26">
+<div class="sourceCode cell-code" id="cb32"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb32-1"><a href="#cb32-1" aria-hidden="true" tabindex="-1"></a><span class="bu">print</span>(gen_design_table(fun_control))</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>This allows to check if all information is available and if the information is correct. <a href="#tbl-design">Table&nbsp;3</a> shows the experimental design for the hyperparameter tuning. Hyperparameter transformations are shown in the column “transform”, e.g., the <code>l1</code> default is <code>5</code>, which results in the value <span class="math inline">\(2^5 = 32\)</span> for the network, because the transformation <code>transform_power_2_int</code> was selected in the <code>JSON</code> file. The default value of the <code>batch_size</code> is set to <code>4</code>, which results in a batch size of <span class="math inline">\(2^4 = 16\)</span>.</p>
 <div id="tbl-design" class="anchored">
 <table class="table">
 <caption>Table&nbsp;3: Experimental design for the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The transformation function is used to transform the hyperparameter values from the unit hypercube to the original domain. The transformation function is applied to the hyperparameter values before the evaluation of the objective function.</caption>
 <colgroup>
 <col style="width: 15%">
@@ -1382,48 +1257,48 @@
 <td>9</td>
 <td>None</td>
 </tr>
 </tbody>
 </table>
 </div>
 <p>The objective function <code>fun_torch</code> is selected next. It implements an interface from <code>PyTorch</code>’s training, validation, and testing methods to <code>spotPython</code>.</p>
-<div class="cell" data-execution_count="35">
-<div class="sourceCode cell-code" id="cb41"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb41-1"><a href="#cb41-1" aria-hidden="true" tabindex="-1"></a>fun <span class="op">=</span> HyperTorch().fun_torch</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="27">
+<div class="sourceCode cell-code" id="cb33"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb33-1"><a href="#cb33-1" aria-hidden="true" tabindex="-1"></a>fun <span class="op">=</span> HyperTorch().fun_torch</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>The <code>spotPython</code> hyperparameter tuning is started by calling the <code>Spot</code> function. Here, we will run the tuner for approximately 30 minutes (<code>max_time</code>). Note: the initial design is always evaluated in the <code>spotPython</code> run. As a consequence, the run may take longer than specified by <code>max_time</code>, because the evaluation time of initial design (here: <code>init_size</code>, 10 points) is performed independently of <code>max_time</code>.</p>
-<div class="cell" data-execution_count="37">
-<div class="sourceCode cell-code" id="cb42"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb42-1"><a href="#cb42-1" aria-hidden="true" tabindex="-1"></a>spot_tuner <span class="op">=</span> spot.Spot(fun<span class="op">=</span>fun,</span>
-<span id="cb42-2"><a href="#cb42-2" aria-hidden="true" tabindex="-1"></a>                   lower <span class="op">=</span> lower,</span>
-<span id="cb42-3"><a href="#cb42-3" aria-hidden="true" tabindex="-1"></a>                   upper <span class="op">=</span> upper,</span>
-<span id="cb42-4"><a href="#cb42-4" aria-hidden="true" tabindex="-1"></a>                   fun_evals <span class="op">=</span> inf,</span>
-<span id="cb42-5"><a href="#cb42-5" aria-hidden="true" tabindex="-1"></a>                   fun_repeats <span class="op">=</span> <span class="dv">1</span>,</span>
-<span id="cb42-6"><a href="#cb42-6" aria-hidden="true" tabindex="-1"></a>                   max_time <span class="op">=</span> MAX_TIME,</span>
-<span id="cb42-7"><a href="#cb42-7" aria-hidden="true" tabindex="-1"></a>                   noise <span class="op">=</span> <span class="va">False</span>,</span>
-<span id="cb42-8"><a href="#cb42-8" aria-hidden="true" tabindex="-1"></a>                   tolerance_x <span class="op">=</span> np.sqrt(np.spacing(<span class="dv">1</span>)),</span>
-<span id="cb42-9"><a href="#cb42-9" aria-hidden="true" tabindex="-1"></a>                   var_type <span class="op">=</span> var_type,</span>
-<span id="cb42-10"><a href="#cb42-10" aria-hidden="true" tabindex="-1"></a>                   var_name <span class="op">=</span> var_name,</span>
-<span id="cb42-11"><a href="#cb42-11" aria-hidden="true" tabindex="-1"></a>                   infill_criterion <span class="op">=</span> <span class="st">"y"</span>,</span>
-<span id="cb42-12"><a href="#cb42-12" aria-hidden="true" tabindex="-1"></a>                   n_points <span class="op">=</span> <span class="dv">1</span>,</span>
-<span id="cb42-13"><a href="#cb42-13" aria-hidden="true" tabindex="-1"></a>                   seed<span class="op">=</span><span class="dv">123</span>,</span>
-<span id="cb42-14"><a href="#cb42-14" aria-hidden="true" tabindex="-1"></a>                   log_level <span class="op">=</span> <span class="dv">50</span>,</span>
-<span id="cb42-15"><a href="#cb42-15" aria-hidden="true" tabindex="-1"></a>                   show_models<span class="op">=</span> <span class="va">False</span>,</span>
-<span id="cb42-16"><a href="#cb42-16" aria-hidden="true" tabindex="-1"></a>                   show_progress<span class="op">=</span> <span class="va">True</span>,</span>
-<span id="cb42-17"><a href="#cb42-17" aria-hidden="true" tabindex="-1"></a>                   fun_control <span class="op">=</span> fun_control,</span>
-<span id="cb42-18"><a href="#cb42-18" aria-hidden="true" tabindex="-1"></a>                   design_control<span class="op">=</span>{<span class="st">"init_size"</span>: INIT_SIZE,</span>
-<span id="cb42-19"><a href="#cb42-19" aria-hidden="true" tabindex="-1"></a>                                   <span class="st">"repeats"</span>: <span class="dv">1</span>},</span>
-<span id="cb42-20"><a href="#cb42-20" aria-hidden="true" tabindex="-1"></a>                   surrogate_control<span class="op">=</span>{<span class="st">"noise"</span>: <span class="va">True</span>,</span>
-<span id="cb42-21"><a href="#cb42-21" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"cod_type"</span>: <span class="st">"norm"</span>,</span>
-<span id="cb42-22"><a href="#cb42-22" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"min_theta"</span>: <span class="op">-</span><span class="dv">4</span>,</span>
-<span id="cb42-23"><a href="#cb42-23" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"max_theta"</span>: <span class="dv">3</span>,</span>
-<span id="cb42-24"><a href="#cb42-24" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"n_theta"</span>: <span class="bu">len</span>(var_name),</span>
-<span id="cb42-25"><a href="#cb42-25" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"model_optimizer"</span>: differential_evolution,</span>
-<span id="cb42-26"><a href="#cb42-26" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"model_fun_evals"</span>: <span class="dv">10_000</span>,</span>
-<span id="cb42-27"><a href="#cb42-27" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"log_level"</span>: <span class="dv">50</span></span>
-<span id="cb42-28"><a href="#cb42-28" aria-hidden="true" tabindex="-1"></a>                                      })</span>
-<span id="cb42-29"><a href="#cb42-29" aria-hidden="true" tabindex="-1"></a>spot_tuner.run(X_start<span class="op">=</span>X_start)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="29">
+<div class="sourceCode cell-code" id="cb34"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb34-1"><a href="#cb34-1" aria-hidden="true" tabindex="-1"></a>spot_tuner <span class="op">=</span> spot.Spot(fun<span class="op">=</span>fun,</span>
+<span id="cb34-2"><a href="#cb34-2" aria-hidden="true" tabindex="-1"></a>                   lower <span class="op">=</span> lower,</span>
+<span id="cb34-3"><a href="#cb34-3" aria-hidden="true" tabindex="-1"></a>                   upper <span class="op">=</span> upper,</span>
+<span id="cb34-4"><a href="#cb34-4" aria-hidden="true" tabindex="-1"></a>                   fun_evals <span class="op">=</span> inf,</span>
+<span id="cb34-5"><a href="#cb34-5" aria-hidden="true" tabindex="-1"></a>                   fun_repeats <span class="op">=</span> <span class="dv">1</span>,</span>
+<span id="cb34-6"><a href="#cb34-6" aria-hidden="true" tabindex="-1"></a>                   max_time <span class="op">=</span> MAX_TIME,</span>
+<span id="cb34-7"><a href="#cb34-7" aria-hidden="true" tabindex="-1"></a>                   noise <span class="op">=</span> <span class="va">False</span>,</span>
+<span id="cb34-8"><a href="#cb34-8" aria-hidden="true" tabindex="-1"></a>                   tolerance_x <span class="op">=</span> np.sqrt(np.spacing(<span class="dv">1</span>)),</span>
+<span id="cb34-9"><a href="#cb34-9" aria-hidden="true" tabindex="-1"></a>                   var_type <span class="op">=</span> var_type,</span>
+<span id="cb34-10"><a href="#cb34-10" aria-hidden="true" tabindex="-1"></a>                   var_name <span class="op">=</span> var_name,</span>
+<span id="cb34-11"><a href="#cb34-11" aria-hidden="true" tabindex="-1"></a>                   infill_criterion <span class="op">=</span> <span class="st">"y"</span>,</span>
+<span id="cb34-12"><a href="#cb34-12" aria-hidden="true" tabindex="-1"></a>                   n_points <span class="op">=</span> <span class="dv">1</span>,</span>
+<span id="cb34-13"><a href="#cb34-13" aria-hidden="true" tabindex="-1"></a>                   seed<span class="op">=</span><span class="dv">123</span>,</span>
+<span id="cb34-14"><a href="#cb34-14" aria-hidden="true" tabindex="-1"></a>                   log_level <span class="op">=</span> <span class="dv">50</span>,</span>
+<span id="cb34-15"><a href="#cb34-15" aria-hidden="true" tabindex="-1"></a>                   show_models<span class="op">=</span> <span class="va">False</span>,</span>
+<span id="cb34-16"><a href="#cb34-16" aria-hidden="true" tabindex="-1"></a>                   show_progress<span class="op">=</span> <span class="va">True</span>,</span>
+<span id="cb34-17"><a href="#cb34-17" aria-hidden="true" tabindex="-1"></a>                   fun_control <span class="op">=</span> fun_control,</span>
+<span id="cb34-18"><a href="#cb34-18" aria-hidden="true" tabindex="-1"></a>                   design_control<span class="op">=</span>{<span class="st">"init_size"</span>: INIT_SIZE,</span>
+<span id="cb34-19"><a href="#cb34-19" aria-hidden="true" tabindex="-1"></a>                                   <span class="st">"repeats"</span>: <span class="dv">1</span>},</span>
+<span id="cb34-20"><a href="#cb34-20" aria-hidden="true" tabindex="-1"></a>                   surrogate_control<span class="op">=</span>{<span class="st">"noise"</span>: <span class="va">True</span>,</span>
+<span id="cb34-21"><a href="#cb34-21" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"cod_type"</span>: <span class="st">"norm"</span>,</span>
+<span id="cb34-22"><a href="#cb34-22" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"min_theta"</span>: <span class="op">-</span><span class="dv">4</span>,</span>
+<span id="cb34-23"><a href="#cb34-23" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"max_theta"</span>: <span class="dv">3</span>,</span>
+<span id="cb34-24"><a href="#cb34-24" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"n_theta"</span>: <span class="bu">len</span>(var_name),</span>
+<span id="cb34-25"><a href="#cb34-25" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"model_optimizer"</span>: differential_evolution,</span>
+<span id="cb34-26"><a href="#cb34-26" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"model_fun_evals"</span>: <span class="dv">10_000</span>,</span>
+<span id="cb34-27"><a href="#cb34-27" aria-hidden="true" tabindex="-1"></a>                                      <span class="st">"log_level"</span>: <span class="dv">50</span></span>
+<span id="cb34-28"><a href="#cb34-28" aria-hidden="true" tabindex="-1"></a>                                      })</span>
+<span id="cb34-29"><a href="#cb34-29" aria-hidden="true" tabindex="-1"></a>spot_tuner.run(X_start<span class="op">=</span>X_start)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>During the run, the following output is shown:</p>
 <pre class="{raw}"><code>config: {'l1': 4, 'l2': 64, 'lr_mult': 1.0, 'batch_size': 16, 'epochs': 16, 'k_folds': 0, 'patience': 3, 'optimizer': 'Adadelta', 'sgd_momentum': 0.9}
 Epoch: 1
 Loss on hold-out set: 1.602842689704895
 Accuracy on hold-out set: 0.4006
 Metric value on hold-out data: 0.40059998631477356
@@ -1476,28 +1351,28 @@
 ----------------------------------------------</code></pre>
 </section>
 <section id="sec-results-tuning" class="level2">
 <h2 class="anchored" data-anchor-id="sec-results-tuning">Results</h2>
 <p>After the hyperparameter tuning run is finished, the progress of the hyperparameter tuning can be visualized. The following code generates the progress plot from <a href="#fig-progress">Figure&nbsp;2</a>.</p>
 <div id="fig-progress" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
-<div class="sourceCode cell-code" id="cb44"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb44-1"><a href="#cb44-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_progress(log_y<span class="op">=</span><span class="va">False</span>, filename<span class="op">=</span><span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_progress.png"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="sourceCode cell-code" id="cb36"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb36-1"><a href="#cb36-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_progress(log_y<span class="op">=</span><span class="va">False</span>, filename<span class="op">=</span><span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_progress.png"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 <figcaption class="figure-caption">Figure&nbsp;1: <strong>?(caption)</strong></figcaption>
 </figure>
 </div>
 <div id="fig-progress" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png" class="img-fluid figure-img"></p>
 <figcaption class="figure-caption">Figure&nbsp;2: Progress plot. <code>Black</code> dots denote results from the initial design. <code>Red</code> dots illustrate the improvement found by the surrogate model based optimization (surrogate model based optimization).</figcaption>
 </figure>
 </div>
 <p><a href="#fig-progress">Figure&nbsp;2</a> shows a typical behaviour that can be observed in many hyperparameter studies <span class="citation" data-cites="bart21i">(<a href="#ref-bart21i" role="doc-biblioref">Bartz et al. 2022</a>)</span>: the largest improvement is obtained during the evaluation of the initial design. The surrogate model based optimization-optimization with the surrogate refines the results. <a href="#fig-progress">Figure&nbsp;2</a> also illustrates one major difference between <code>ray[tune]</code> as used in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span> and <code>spotPython</code>: the <code>ray[tune]</code> uses a random search and will generate results similar to the <em>black</em> dots, whereas <code>spotPython</code> uses a surrogate model based optimization and presents results represented by <em>red</em> dots in <a href="#fig-progress">Figure&nbsp;2</a>. The surrogate model based optimization is considered to be more efficient than a random search, because the surrogate model guides the search towards promising regions in the hyperparameter space.</p>
 <p>In addition to the improved (“optimized”) hyperparameter values, <code>spotPython</code> allows a statistical analysis, e.g., a sensitivity analysis, of the results. We can print the results of the hyperparameter tuning, see <a href="#tbl-results">Table&nbsp;4</a>.</p>
-<div class="cell" data-execution_count="40">
-<div class="sourceCode cell-code" id="cb45"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb45-1"><a href="#cb45-1" aria-hidden="true" tabindex="-1"></a><span class="bu">print</span>(gen_design_table(fun_control<span class="op">=</span>fun_control, spot<span class="op">=</span>spot_tuner))</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="32">
+<div class="sourceCode cell-code" id="cb37"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb37-1"><a href="#cb37-1" aria-hidden="true" tabindex="-1"></a><span class="bu">print</span>(gen_design_table(fun_control<span class="op">=</span>fun_control, spot<span class="op">=</span>spot_tuner))</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <div id="tbl-results" class="anchored">
 <table class="table">
 <caption>Table&nbsp;4: Results of the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The column “tuned” shows the tuned values. The column “importance” shows the importance of the hyperparameters. The column “stars” shows the importance of the hyperparameters in stars. The importance is computed by the SPOT software.</caption>
 <colgroup>
 <col style="width: 10%">
 <col style="width: 7%">
@@ -1611,50 +1486,50 @@
 <td style="text-align: right;">0.16</td>
 <td>.</td>
 </tr>
 </tbody>
 </table>
 </div>
 <p>To visualize the most important hyperparameters, <code>spotPython</code> provides the function <code>plot_importance</code>. The following code generates the importance plot from <a href="#fig-importance">Figure&nbsp;3</a>.</p>
-<div class="cell" data-execution_count="41">
-<div class="sourceCode cell-code" id="cb46"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb46-1"><a href="#cb46-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_importance(threshold<span class="op">=</span><span class="fl">0.025</span>, filename<span class="op">=</span><span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_importance.png"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="33">
+<div class="sourceCode cell-code" id="cb38"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb38-1"><a href="#cb38-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_importance(threshold<span class="op">=</span><span class="fl">0.025</span>, filename<span class="op">=</span><span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_importance.png"</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <div id="fig-importance" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png" class="img-fluid figure-img" style="width:50.0%"></p>
 <figcaption class="figure-caption">Figure&nbsp;3: Variable importance</figcaption>
 </figure>
 </div>
 </section>
 <section id="sec-get-spot-results" class="level2">
 <h2 class="anchored" data-anchor-id="sec-get-spot-results">Get SPOT Results</h2>
 <p>The architecture of the <code>spotPython</code> model can be obtained by the following code:</p>
-<div class="cell" data-execution_count="42">
-<div class="sourceCode cell-code" id="cb47"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb47-1"><a href="#cb47-1" aria-hidden="true" tabindex="-1"></a>X <span class="op">=</span> spot_tuner.to_all_dim(spot_tuner.min_X.reshape(<span class="dv">1</span>,<span class="op">-</span><span class="dv">1</span>))</span>
-<span id="cb47-2"><a href="#cb47-2" aria-hidden="true" tabindex="-1"></a>model_spot <span class="op">=</span> get_one_core_model_from_X(X, fun_control)</span>
-<span id="cb47-3"><a href="#cb47-3" aria-hidden="true" tabindex="-1"></a>model_spot</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="34">
+<div class="sourceCode cell-code" id="cb39"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb39-1"><a href="#cb39-1" aria-hidden="true" tabindex="-1"></a>X <span class="op">=</span> spot_tuner.to_all_dim(spot_tuner.min_X.reshape(<span class="dv">1</span>,<span class="op">-</span><span class="dv">1</span>))</span>
+<span id="cb39-2"><a href="#cb39-2" aria-hidden="true" tabindex="-1"></a>model_spot <span class="op">=</span> get_one_core_model_from_X(X, fun_control)</span>
+<span id="cb39-3"><a href="#cb39-3" aria-hidden="true" tabindex="-1"></a>model_spot</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>First, the numerical representation of the hyperparameters are obtained, i.e., the numpy array <code>X</code> is generated. This array is then used to generate the model <code>model_spot</code> by the function <code>get_one_core_model_from_X</code>. The model <code>model_spot</code> has the following architecture:</p>
 <pre class="{raw}"><code>Net_CIFAR10(
   (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))
   (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
   (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))
   (fc1): Linear(in_features=400, out_features=64, bias=True)
   (fc2): Linear(in_features=64, out_features=32, bias=True)
   (fc3): Linear(in_features=32, out_features=10, bias=True)
 )</code></pre>
 </section>
 <section id="get-default-hyperparameters" class="level2">
 <h2 class="anchored" data-anchor-id="get-default-hyperparameters">Get Default Hyperparameters</h2>
-<p>In a similar manner as in <a href="#sec-get-spot-results">Section&nbsp;3.11</a>, the default hyperparameters can be obtained.</p>
-<div class="cell" data-execution_count="43">
-<div class="sourceCode cell-code" id="cb49"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb49-1"><a href="#cb49-1" aria-hidden="true" tabindex="-1"></a><span class="co"># fun_control was modified, we generate a new one with the original default hyperparameters</span></span>
-<span id="cb49-2"><a href="#cb49-2" aria-hidden="true" tabindex="-1"></a>fc <span class="op">=</span> copy.deepcopy(fun_control)</span>
-<span id="cb49-3"><a href="#cb49-3" aria-hidden="true" tabindex="-1"></a>fc.update({<span class="st">"core_model_hyper_dict"</span>: hyper_dict[fun_control[<span class="st">"core_model"</span>].<span class="va">__name__</span>]})</span>
-<span id="cb49-4"><a href="#cb49-4" aria-hidden="true" tabindex="-1"></a>model_default <span class="op">=</span> get_one_core_model_from_X(X_start, fun_control<span class="op">=</span>fc)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<p>In a similar manner as in <a href="#sec-get-spot-results">Section&nbsp;4.11</a>, the default hyperparameters can be obtained.</p>
+<div class="cell" data-execution_count="35">
+<div class="sourceCode cell-code" id="cb41"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb41-1"><a href="#cb41-1" aria-hidden="true" tabindex="-1"></a><span class="co"># fun_control was modified, we generate a new one with the original default hyperparameters</span></span>
+<span id="cb41-2"><a href="#cb41-2" aria-hidden="true" tabindex="-1"></a>fc <span class="op">=</span> copy.deepcopy(fun_control)</span>
+<span id="cb41-3"><a href="#cb41-3" aria-hidden="true" tabindex="-1"></a>fc.update({<span class="st">"core_model_hyper_dict"</span>: hyper_dict[fun_control[<span class="st">"core_model"</span>].<span class="va">__name__</span>]})</span>
+<span id="cb41-4"><a href="#cb41-4" aria-hidden="true" tabindex="-1"></a>model_default <span class="op">=</span> get_one_core_model_from_X(X_start, fun_control<span class="op">=</span>fc)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>The corresponding default model has the following architecture:</p>
 <pre class="{raw}"><code>Net_CIFAR10(
   (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))
   (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
   (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))
   (fc1): Linear(in_features=400, out_features=32, bias=True)
@@ -1662,44 +1537,44 @@
   (fc3): Linear(in_features=32, out_features=10, bias=True)
 )</code></pre>
 </section>
 <section id="evaluation-of-the-tuned-architecture" class="level2">
 <h2 class="anchored" data-anchor-id="evaluation-of-the-tuned-architecture">Evaluation of the Tuned Architecture</h2>
 <p>The method <code>train_tuned</code> takes a model architecture without trained weights and trains this model with the train data. The train data is split into train and validation data. The validation data is used for early stopping. The trained model weights are saved as a dictionary.</p>
 <p>This evaluation is similar to the final evaluation in <span class="citation" data-cites="pyto23a">PyTorch (<a href="#ref-pyto23a" role="doc-biblioref">2023a</a>)</span>.</p>
-<div class="cell" data-execution_count="44">
-<div class="sourceCode cell-code" id="cb51"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb51-1"><a href="#cb51-1" aria-hidden="true" tabindex="-1"></a>train_tuned(net<span class="op">=</span>model_default, train_dataset<span class="op">=</span>train, shuffle<span class="op">=</span><span class="va">True</span>,</span>
-<span id="cb51-2"><a href="#cb51-2" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
-<span id="cb51-3"><a href="#cb51-3" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
-<span id="cb51-4"><a href="#cb51-4" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> DEVICE, show_batch_interval<span class="op">=</span><span class="dv">1_000</span>,)</span>
-<span id="cb51-5"><a href="#cb51-5" aria-hidden="true" tabindex="-1"></a>test_tuned(net<span class="op">=</span>model_default, test_dataset<span class="op">=</span>test, </span>
-<span id="cb51-6"><a href="#cb51-6" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
-<span id="cb51-7"><a href="#cb51-7" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
-<span id="cb51-8"><a href="#cb51-8" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span><span class="va">False</span>, </span>
-<span id="cb51-9"><a href="#cb51-9" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> DEVICE)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="36">
+<div class="sourceCode cell-code" id="cb43"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb43-1"><a href="#cb43-1" aria-hidden="true" tabindex="-1"></a>train_tuned(net<span class="op">=</span>model_default, train_dataset<span class="op">=</span>train, shuffle<span class="op">=</span><span class="va">True</span>,</span>
+<span id="cb43-2"><a href="#cb43-2" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb43-3"><a href="#cb43-3" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb43-4"><a href="#cb43-4" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> DEVICE, show_batch_interval<span class="op">=</span><span class="dv">1_000</span>,)</span>
+<span id="cb43-5"><a href="#cb43-5" aria-hidden="true" tabindex="-1"></a>test_tuned(net<span class="op">=</span>model_default, test_dataset<span class="op">=</span>test, </span>
+<span id="cb43-6"><a href="#cb43-6" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb43-7"><a href="#cb43-7" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb43-8"><a href="#cb43-8" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span><span class="va">False</span>, </span>
+<span id="cb43-9"><a href="#cb43-9" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> DEVICE)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <p>The following code trains the model <code>model_spot</code>. If <code>path</code> is set to a filename, e.g., <code>path = "model_spot_trained.pt"</code>, the weights of the trained model will be saved to this file.</p>
-<div class="cell" data-execution_count="45">
-<div class="sourceCode cell-code" id="cb52"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb52-1"><a href="#cb52-1" aria-hidden="true" tabindex="-1"></a>train_tuned(net<span class="op">=</span>model_spot, train_dataset<span class="op">=</span>train,</span>
-<span id="cb52-2"><a href="#cb52-2" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
-<span id="cb52-3"><a href="#cb52-3" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
-<span id="cb52-4"><a href="#cb52-4" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span><span class="va">True</span>,</span>
-<span id="cb52-5"><a href="#cb52-5" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> DEVICE,</span>
-<span id="cb52-6"><a href="#cb52-6" aria-hidden="true" tabindex="-1"></a>        path<span class="op">=</span><span class="va">None</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="37">
+<div class="sourceCode cell-code" id="cb44"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb44-1"><a href="#cb44-1" aria-hidden="true" tabindex="-1"></a>train_tuned(net<span class="op">=</span>model_spot, train_dataset<span class="op">=</span>train,</span>
+<span id="cb44-2"><a href="#cb44-2" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb44-3"><a href="#cb44-3" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb44-4"><a href="#cb44-4" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span><span class="va">True</span>,</span>
+<span id="cb44-5"><a href="#cb44-5" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> DEVICE,</span>
+<span id="cb44-6"><a href="#cb44-6" aria-hidden="true" tabindex="-1"></a>        path<span class="op">=</span><span class="va">None</span>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <pre class="{raw}"><code>Loss on hold-out set: 1.2267619131326675
 Accuracy on hold-out set: 0.58955
 Early stopping at epoch 13</code></pre>
 <p>If <code>path</code> is set to a filename, e.g., <code>path = "model_spot_trained.pt"</code>, the weights of the trained model will be loaded from this file.</p>
-<div class="cell" data-execution_count="46">
-<div class="sourceCode cell-code" id="cb54"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb54-1"><a href="#cb54-1" aria-hidden="true" tabindex="-1"></a>test_tuned(net<span class="op">=</span>model_spot, test_dataset<span class="op">=</span>test,</span>
-<span id="cb54-2"><a href="#cb54-2" aria-hidden="true" tabindex="-1"></a>            shuffle<span class="op">=</span><span class="va">False</span>,</span>
-<span id="cb54-3"><a href="#cb54-3" aria-hidden="true" tabindex="-1"></a>            loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
-<span id="cb54-4"><a href="#cb54-4" aria-hidden="true" tabindex="-1"></a>            metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
-<span id="cb54-5"><a href="#cb54-5" aria-hidden="true" tabindex="-1"></a>            device <span class="op">=</span> DEVICE)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+<div class="cell" data-execution_count="38">
+<div class="sourceCode cell-code" id="cb46"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb46-1"><a href="#cb46-1" aria-hidden="true" tabindex="-1"></a>test_tuned(net<span class="op">=</span>model_spot, test_dataset<span class="op">=</span>test,</span>
+<span id="cb46-2"><a href="#cb46-2" aria-hidden="true" tabindex="-1"></a>            shuffle<span class="op">=</span><span class="va">False</span>,</span>
+<span id="cb46-3"><a href="#cb46-3" aria-hidden="true" tabindex="-1"></a>            loss_function<span class="op">=</span>fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb46-4"><a href="#cb46-4" aria-hidden="true" tabindex="-1"></a>            metric<span class="op">=</span>fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb46-5"><a href="#cb46-5" aria-hidden="true" tabindex="-1"></a>            device <span class="op">=</span> DEVICE)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <pre class="{raw}"><code>Loss on hold-out set: 1.242568492603302
 Accuracy on hold-out set: 0.5957</code></pre>
 </section>
 <section id="comparison-with-default-hyperparameters-and-ray-tune" class="level2">
 <h2 class="anchored" data-anchor-id="comparison-with-default-hyperparameters-and-ray-tune">Comparison with Default Hyperparameters and Ray Tune</h2>
 <p><a href="#tbl-comparison">Table&nbsp;5</a> shows the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from <code>ray[tune]</code>.</p>
@@ -1747,77 +1622,62 @@
 </tbody>
 </table>
 </div>
 </section>
 <section id="detailed-hyperparameter-plots" class="level2">
 <h2 class="anchored" data-anchor-id="detailed-hyperparameter-plots">Detailed Hyperparameter Plots</h2>
 <p>The contour plots in this section visualize the interactions of the three most important hyperparameters, <code>l1</code>, <code>l2</code>, and <code>epochs</code>, and <code>optimizer</code> of the surrogate model used to optimize the hyperparameters. Since some of these hyperparameters take fatorial or integer values, sometimes step-like fitness landcapes (or response surfaces) are generated. SPOT draws the interactions of the main hyperparameters by default. It is also possible to visualize all interactions. For this, again refer to the notebook <span class="citation" data-cites="bart23e">(<a href="#ref-bart23e" role="doc-biblioref">Bartz-Beielstein 2023</a>)</span>.</p>
-<div id="fig-contour" class="quarto-figure quarto-figure-center anchored">
-<figure class="figure">
-<div class="sourceCode cell-code" id="cb56"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb56-1"><a href="#cb56-1" aria-hidden="true" tabindex="-1"></a>threshold <span class="op">=</span> <span class="fl">0.025</span></span>
-<span id="cb56-2"><a href="#cb56-2" aria-hidden="true" tabindex="-1"></a>impo <span class="op">=</span> spot_tuner.print_importance(threshold<span class="op">=</span>threshold, print_screen<span class="op">=</span><span class="va">True</span>)</span>
-<span id="cb56-3"><a href="#cb56-3" aria-hidden="true" tabindex="-1"></a>var_plots <span class="op">=</span> [i <span class="cf">for</span> i, x <span class="kw">in</span> <span class="bu">enumerate</span>(impo) <span class="cf">if</span> x[<span class="dv">1</span>] <span class="op">&gt;</span> threshold]</span>
-<span id="cb56-4"><a href="#cb56-4" aria-hidden="true" tabindex="-1"></a>min_z <span class="op">=</span> <span class="bu">min</span>(spot_tuner.y)</span>
-<span id="cb56-5"><a href="#cb56-5" aria-hidden="true" tabindex="-1"></a>max_z <span class="op">=</span> <span class="bu">max</span>(spot_tuner.y)</span>
-<span id="cb56-6"><a href="#cb56-6" aria-hidden="true" tabindex="-1"></a>n <span class="op">=</span> spot_tuner.k</span>
-<span id="cb56-7"><a href="#cb56-7" aria-hidden="true" tabindex="-1"></a><span class="cf">for</span> i <span class="kw">in</span> var_plots:</span>
-<span id="cb56-8"><a href="#cb56-8" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> j <span class="kw">in</span> var_plots:</span>
-<span id="cb56-9"><a href="#cb56-9" aria-hidden="true" tabindex="-1"></a>        <span class="cf">if</span> j <span class="op">&gt;</span> i:</span>
-<span id="cb56-10"><a href="#cb56-10" aria-hidden="true" tabindex="-1"></a>            filename <span class="op">=</span> <span class="st">"./figures"</span> <span class="op">+</span> experiment_name<span class="op">+</span><span class="st">"_contour_"</span><span class="op">+</span><span class="bu">str</span>(i)<span class="op">+</span><span class="st">"_"</span><span class="op">+</span><span class="bu">str</span>(j)<span class="op">+</span><span class="st">".png"</span></span>
-<span id="cb56-11"><a href="#cb56-11" aria-hidden="true" tabindex="-1"></a>            spot_tuner.plot_contour(i<span class="op">=</span>i, j<span class="op">=</span>j, min_z<span class="op">=</span>min_z, max_z <span class="op">=</span> max_z, filename<span class="op">=</span>filename)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-<figcaption class="figure-caption">Figure&nbsp;4: <strong>?(caption)</strong></figcaption>
-</figure>
+<div class="cell" data-execution_count="39">
+<div class="sourceCode cell-code" id="cb48"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb48-1"><a href="#cb48-1" aria-hidden="true" tabindex="-1"></a>filename <span class="op">=</span> <span class="st">"./figures"</span> <span class="op">+</span> experiment_name</span>
+<span id="cb48-2"><a href="#cb48-2" aria-hidden="true" tabindex="-1"></a>spot_tuner.plot_important_hyperparameter_contour(filename<span class="op">=</span>filename)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <div id="fig-contour-0-1" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png" class="img-fluid figure-img"></p>
-<figcaption class="figure-caption">Figure&nbsp;5: Contour plot of the loss as a function of <code>l1</code> and <code>l2</code>, i.e., the number of neurons in the layers.</figcaption>
+<figcaption class="figure-caption">Figure&nbsp;4: Contour plot of the loss as a function of <code>l1</code> and <code>l2</code>, i.e., the number of neurons in the layers.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-0-3" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png" class="img-fluid figure-img"></p>
-<figcaption class="figure-caption">Figure&nbsp;6: Contour plot of the loss as a function of the number of epochs and the neurons in layer <code>l1</code>.</figcaption>
+<figcaption class="figure-caption">Figure&nbsp;5: Contour plot of the loss as a function of the number of epochs and the neurons in layer <code>l1</code>.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-0-4" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png" class="img-fluid figure-img"></p>
-<figcaption class="figure-caption">Figure&nbsp;7: Contour plot of the loss as a function of the optimizer and the neurons in layer <code>l1</code>.</figcaption>
+<figcaption class="figure-caption">Figure&nbsp;6: Contour plot of the loss as a function of the optimizer and the neurons in layer <code>l1</code>.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-1-3" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png" class="img-fluid figure-img"></p>
-<figcaption class="figure-caption">Figure&nbsp;8: Contour plot of the loss as a function of the number of epochs and the neurons in layer <code>l2</code>.</figcaption>
+<figcaption class="figure-caption">Figure&nbsp;7: Contour plot of the loss as a function of the number of epochs and the neurons in layer <code>l2</code>.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-1-3" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png" class="img-fluid figure-img"></p>
-<figcaption class="figure-caption">Figure&nbsp;9: Contour plot of the loss as a function of the optimizer and the neurons in layer <code>l2</code>.</figcaption>
+<figcaption class="figure-caption">Figure&nbsp;8: Contour plot of the loss as a function of the optimizer and the neurons in layer <code>l2</code>.</figcaption>
 </figure>
 </div>
 <div id="fig-contour-3-4" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png" class="img-fluid figure-img"></p>
-<figcaption class="figure-caption">Figure&nbsp;10: Contour plot of the loss as a function of the optimizer and the number of epochs.</figcaption>
+<figcaption class="figure-caption">Figure&nbsp;9: Contour plot of the loss as a function of the optimizer and the number of epochs.</figcaption>
 </figure>
 </div>
-<p><a href="#fig-contour-0-1">Figure&nbsp;5</a> to <a href="#fig-contour-3-4">Figure&nbsp;10</a> show the contour plots of the loss as a function of the hyperparameters. These plots are very helpful for benchmark studies and for understanding neural networks. <code>spotPython</code> provides additional tools for a visual inspection of the results and give valuable insights into the hyperparameter tuning process. This is especially useful for model explainability, transparency, and trustworthiness. In addition to the contour plots, <a href="#fig-parallel">Figure&nbsp;12</a> shows the parallel plot of the hyperparameters.</p>
-<div id="fig-parallel" class="quarto-figure quarto-figure-center anchored">
-<figure class="figure">
-<div class="sourceCode cell-code" id="cb57"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb57-1"><a href="#cb57-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.parallel_plot()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
-<figcaption class="figure-caption">Figure&nbsp;11: <strong>?(caption)</strong></figcaption>
-</figure>
+<p><a href="#fig-contour-0-1">Figure&nbsp;4</a> to <a href="#fig-contour-3-4">Figure&nbsp;9</a> show the contour plots of the loss as a function of the hyperparameters. These plots are very helpful for benchmark studies and for understanding neural networks. <code>spotPython</code> provides additional tools for a visual inspection of the results and give valuable insights into the hyperparameter tuning process. This is especially useful for model explainability, transparency, and trustworthiness. In addition to the contour plots, <a href="#fig-parallel">Figure&nbsp;10</a> shows the parallel plot of the hyperparameters.</p>
+<div class="cell" data-execution_count="40">
+<div class="sourceCode cell-code" id="cb49"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb49-1"><a href="#cb49-1" aria-hidden="true" tabindex="-1"></a>spot_tuner.parallel_plot()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
 </div>
 <div id="fig-parallel" class="quarto-figure quarto-figure-center anchored">
 <figure class="figure">
 <p><img src="./figures/parallel.png" class="img-fluid figure-img"></p>
-<figcaption class="figure-caption">Figure&nbsp;12: Parallel plot</figcaption>
+<figcaption class="figure-caption">Figure&nbsp;10: Parallel plot</figcaption>
 </figure>
 </div>
 </section>
 </section>
 <section id="sec-summary" class="level1">
 <h1>Summary and Outlook</h1>
 <p>This tutorial presents the hyperparameter tuning open source software <code>spotPython</code> for <code>PyTorch</code>. To show its basic features, a comparison with the “official” <code>PyTorch</code> hyperparameter tuning tutorial <span class="citation" data-cites="pyto23a">(<a href="#ref-pyto23a" role="doc-biblioref">PyTorch 2023a</a>)</span> is presented. Some of the advantages of <code>spotPython</code> are:</p>
@@ -1842,16 +1702,16 @@
 <div class="callout-body-container callout-body">
 <p>Important: This tutorial does not present a complete benchmarking study <span class="citation" data-cites="bart20gArxiv">(<a href="#ref-bart20gArxiv" role="doc-biblioref">Bartz-Beielstein et al. 2020</a>)</span>. The results are only preliminary and highly dependent on the local configuration (hard- and software). Our goal is to provide a first impression of the performance of the hyperparameter tuning package <code>spotPython</code>. To demonstrate its capabilities, a quick comparison with <code>ray[tune]</code> was performed. <code>ray[tune]</code> was chosen, because it is presented as “an industry standard tool for distributed hyperparameter tuning.” The results should be interpreted with care.</p>
 </div>
 </div>
 </section>
 <section id="sec-appendix" class="level1">
 <h1>Appendix</h1>
-<section id="sample-output-from-ray-tunes-run" class="level2 unnumbered">
-<h2 class="unnumbered anchored" data-anchor-id="sample-output-from-ray-tunes-run">Sample Output From Ray Tune’s Run</h2>
+<section id="sample-output-from-ray-tunes-run" class="level2">
+<h2 class="anchored" data-anchor-id="sample-output-from-ray-tunes-run">Sample Output From Ray Tune’s Run</h2>
 <p>The output from <code>ray[tune]</code> could look like this <span class="citation" data-cites="pyto23b">(<a href="#ref-pyto23b" role="doc-biblioref">PyTorch 2023b</a>)</span>:</p>
 <pre class="{raw}"><code>Number of trials: 10 (10 TERMINATED)
 ------+------+-------------+--------------+---------+------------+--------------------+
 |   l1 |   l2 |          lr |   batch_size |    loss |   accuracy | training_iteration |
 +------+------+-------------+--------------+---------+------------+--------------------|
 |   64 |    4 | 0.00011629  |            2 | 1.87273 |     0.244  |                  2 |
 |   32 |   64 | 0.000339763 |            8 | 1.23603 |     0.567  |                  8 |
@@ -1866,14 +1726,294 @@
 +-----+------+------+-------------+--------------+---------+------------+--------------------+
 Best trial config: {'l1': 8, 'l2': 16, 'lr': 0.00276249, 'batch_size': 16, 'data_dir': '...'}
 Best trial final validation loss: 1.181501
 Best trial final validation accuracy: 0.5836
 Best trial test set accuracy: 0.5806</code></pre>
 <div style="page-break-after: always;"></div>
 </section>
+<section id="sec-data-splitting" class="level2">
+<h2 class="anchored" data-anchor-id="sec-data-splitting">Detailed Description of the Data Splitting</h2>
+<section id="description-of-the-train_hold_out-setting" class="level3">
+<h3 class="anchored" data-anchor-id="description-of-the-train_hold_out-setting">Description of the <code>"train_hold_out"</code> Setting</h3>
+<p>The <code>"train_hold_out"</code> setting is used by default. It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
+<ol type="1">
+<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
+<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_hold_out()</code> as follows:</li>
+</ol>
+<div class="cell" data-execution_count="41">
+<div class="sourceCode cell-code" id="cb51"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb51-1"><a href="#cb51-1" aria-hidden="true" tabindex="-1"></a>df_eval, _ <span class="op">=</span> evaluate_hold_out(</span>
+<span id="cb51-2"><a href="#cb51-2" aria-hidden="true" tabindex="-1"></a>    model,</span>
+<span id="cb51-3"><a href="#cb51-3" aria-hidden="true" tabindex="-1"></a>    train_dataset<span class="op">=</span>fun_control[<span class="st">"train"</span>],</span>
+<span id="cb51-4"><a href="#cb51-4" aria-hidden="true" tabindex="-1"></a>    shuffle<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"shuffle"</span>],</span>
+<span id="cb51-5"><a href="#cb51-5" aria-hidden="true" tabindex="-1"></a>    loss_function<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"loss_function"</span>],</span>
+<span id="cb51-6"><a href="#cb51-6" aria-hidden="true" tabindex="-1"></a>    metric<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"metric_torch"</span>],</span>
+<span id="cb51-7"><a href="#cb51-7" aria-hidden="true" tabindex="-1"></a>    device<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"device"</span>],</span>
+<span id="cb51-8"><a href="#cb51-8" aria-hidden="true" tabindex="-1"></a>    show_batch_interval<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"show_batch_interval"</span>],</span>
+<span id="cb51-9"><a href="#cb51-9" aria-hidden="true" tabindex="-1"></a>    path<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"path"</span>],</span>
+<span id="cb51-10"><a href="#cb51-10" aria-hidden="true" tabindex="-1"></a>) </span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>Note: Only the data set <code>fun_control["train"]</code> is used for training and validation. It is used as follows:</p>
+<div class="cell" data-execution_count="42">
+<div class="sourceCode cell-code" id="cb52"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb52-1"><a href="#cb52-1" aria-hidden="true" tabindex="-1"></a>trainloader, valloader <span class="op">=</span> create_train_val_data_loaders(</span>
+<span id="cb52-2"><a href="#cb52-2" aria-hidden="true" tabindex="-1"></a>                dataset<span class="op">=</span>train_dataset, batch_size<span class="op">=</span>batch_size_instance, shuffle<span class="op">=</span>shuffle</span>
+<span id="cb52-3"><a href="#cb52-3" aria-hidden="true" tabindex="-1"></a>            )</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p><code>create_train_val_data_loaders()</code> splits the <code>train_dataset</code> into <code>trainloader</code> and <code>valloader</code> using <code>torch.utils.data.random_split()</code> as follows:</p>
+<div class="cell" data-execution_count="43">
+<div class="sourceCode cell-code" id="cb53"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb53-1"><a href="#cb53-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers<span class="op">=</span><span class="dv">0</span>):</span>
+<span id="cb53-2"><a href="#cb53-2" aria-hidden="true" tabindex="-1"></a>    test_abs <span class="op">=</span> <span class="bu">int</span>(<span class="bu">len</span>(dataset) <span class="op">*</span> <span class="fl">0.6</span>)</span>
+<span id="cb53-3"><a href="#cb53-3" aria-hidden="true" tabindex="-1"></a>    train_subset, val_subset <span class="op">=</span> random_split(dataset, [test_abs, <span class="bu">len</span>(dataset) <span class="op">-</span> test_abs])</span>
+<span id="cb53-4"><a href="#cb53-4" aria-hidden="true" tabindex="-1"></a>    trainloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb53-5"><a href="#cb53-5" aria-hidden="true" tabindex="-1"></a>        train_subset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb53-6"><a href="#cb53-6" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb53-7"><a href="#cb53-7" aria-hidden="true" tabindex="-1"></a>    valloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb53-8"><a href="#cb53-8" aria-hidden="true" tabindex="-1"></a>        val_subset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb53-9"><a href="#cb53-9" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb53-10"><a href="#cb53-10" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> trainloader, valloader</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>The optimizer is set up as follows:</p>
+<div class="cell" data-execution_count="44">
+<div class="sourceCode cell-code" id="cb54"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb54-1"><a href="#cb54-1" aria-hidden="true" tabindex="-1"></a>lr_mult_instance <span class="op">=</span> net.lr_mult</span>
+<span id="cb54-2"><a href="#cb54-2" aria-hidden="true" tabindex="-1"></a>optimizer <span class="op">=</span> optimizer_handler(optimizer_name<span class="op">=</span>optimizer_instance, params<span class="op">=</span>net.parameters(), lr_mult<span class="op">=</span>lr_mult_instance)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="3" type="1">
+<li><code>evaluate_hold_out()</code> sets the <code>net</code> attributes such as <code>epochs</code>, <code>batch_size</code>, <code>optimizer</code>, and <code>patience</code>. For each epoch, the methods <code>train_hold_out()</code> and <code>validate_fold_or_hold_out()</code> are called, the former for training and the latter for validation and early stopping. The validation loss from the last epoch (not the best validation loss) is returned from <code>evaluate_hold_out</code>.</li>
+<li>The method <code>train_hold_out()</code> is implemented as follows:</li>
+</ol>
+<div class="cell" data-execution_count="45">
+<div class="sourceCode cell-code" id="cb55"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb55-1"><a href="#cb55-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> train_hold_out(net, trainloader, batch_size, loss_function, optimizer, device, show_batch_interval<span class="op">=</span><span class="dv">10_000</span>):</span>
+<span id="cb55-2"><a href="#cb55-2" aria-hidden="true" tabindex="-1"></a>    running_loss <span class="op">=</span> <span class="fl">0.0</span></span>
+<span id="cb55-3"><a href="#cb55-3" aria-hidden="true" tabindex="-1"></a>    epoch_steps <span class="op">=</span> <span class="dv">0</span></span>
+<span id="cb55-4"><a href="#cb55-4" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> i, data <span class="kw">in</span> <span class="bu">enumerate</span>(trainloader, <span class="dv">0</span>):</span>
+<span id="cb55-5"><a href="#cb55-5" aria-hidden="true" tabindex="-1"></a>        inputs, labels <span class="op">=</span> data</span>
+<span id="cb55-6"><a href="#cb55-6" aria-hidden="true" tabindex="-1"></a>        inputs, labels <span class="op">=</span> inputs.to(device), labels.to(device)</span>
+<span id="cb55-7"><a href="#cb55-7" aria-hidden="true" tabindex="-1"></a>        optimizer.zero_grad()</span>
+<span id="cb55-8"><a href="#cb55-8" aria-hidden="true" tabindex="-1"></a>        outputs <span class="op">=</span> net(inputs)</span>
+<span id="cb55-9"><a href="#cb55-9" aria-hidden="true" tabindex="-1"></a>        loss <span class="op">=</span> loss_function(outputs, labels)</span>
+<span id="cb55-10"><a href="#cb55-10" aria-hidden="true" tabindex="-1"></a>        loss.backward()</span>
+<span id="cb55-11"><a href="#cb55-11" aria-hidden="true" tabindex="-1"></a>        torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm<span class="op">=</span><span class="fl">1.0</span>)</span>
+<span id="cb55-12"><a href="#cb55-12" aria-hidden="true" tabindex="-1"></a>        optimizer.step()</span>
+<span id="cb55-13"><a href="#cb55-13" aria-hidden="true" tabindex="-1"></a>        running_loss <span class="op">+=</span> loss.item()</span>
+<span id="cb55-14"><a href="#cb55-14" aria-hidden="true" tabindex="-1"></a>        epoch_steps <span class="op">+=</span> <span class="dv">1</span></span>
+<span id="cb55-15"><a href="#cb55-15" aria-hidden="true" tabindex="-1"></a>        <span class="cf">if</span> i <span class="op">%</span> show_batch_interval <span class="op">==</span> (show_batch_interval <span class="op">-</span> <span class="dv">1</span>):  <span class="co"># print every show_batch_interval mini-batches</span></span>
+<span id="cb55-16"><a href="#cb55-16" aria-hidden="true" tabindex="-1"></a>            <span class="bu">print</span>(</span>
+<span id="cb55-17"><a href="#cb55-17" aria-hidden="true" tabindex="-1"></a>                <span class="st">"Batch: </span><span class="sc">%5d</span><span class="st">. Batch Size: </span><span class="sc">%d</span><span class="st">. Training Loss (running): </span><span class="sc">%.3f</span><span class="st">"</span></span>
+<span id="cb55-18"><a href="#cb55-18" aria-hidden="true" tabindex="-1"></a>                <span class="op">%</span> (i <span class="op">+</span> <span class="dv">1</span>, <span class="bu">int</span>(batch_size), running_loss <span class="op">/</span> epoch_steps)</span>
+<span id="cb55-19"><a href="#cb55-19" aria-hidden="true" tabindex="-1"></a>            )</span>
+<span id="cb55-20"><a href="#cb55-20" aria-hidden="true" tabindex="-1"></a>            running_loss <span class="op">=</span> <span class="fl">0.0</span></span>
+<span id="cb55-21"><a href="#cb55-21" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> loss.item()</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="5" type="1">
+<li>The method <code>validate_fold_or_hold_out()</code> is implemented as follows:</li>
+</ol>
+<div class="cell" data-execution_count="46">
+<div class="sourceCode cell-code" id="cb56"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb56-1"><a href="#cb56-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> validate_fold_or_hold_out(net, valloader, loss_function, metric, device):</span>
+<span id="cb56-2"><a href="#cb56-2" aria-hidden="true" tabindex="-1"></a>    val_loss <span class="op">=</span> <span class="fl">0.0</span></span>
+<span id="cb56-3"><a href="#cb56-3" aria-hidden="true" tabindex="-1"></a>    val_steps <span class="op">=</span> <span class="dv">0</span></span>
+<span id="cb56-4"><a href="#cb56-4" aria-hidden="true" tabindex="-1"></a>    metric.reset()</span>
+<span id="cb56-5"><a href="#cb56-5" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> i, data <span class="kw">in</span> <span class="bu">enumerate</span>(valloader, <span class="dv">0</span>):</span>
+<span id="cb56-6"><a href="#cb56-6" aria-hidden="true" tabindex="-1"></a>        <span class="cf">with</span> torch.no_grad():</span>
+<span id="cb56-7"><a href="#cb56-7" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> data</span>
+<span id="cb56-8"><a href="#cb56-8" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> inputs.to(device), labels.to(device)</span>
+<span id="cb56-9"><a href="#cb56-9" aria-hidden="true" tabindex="-1"></a>            outputs <span class="op">=</span> net(inputs)</span>
+<span id="cb56-10"><a href="#cb56-10" aria-hidden="true" tabindex="-1"></a>            _, predicted <span class="op">=</span> torch.<span class="bu">max</span>(outputs.data, <span class="dv">1</span>)</span>
+<span id="cb56-11"><a href="#cb56-11" aria-hidden="true" tabindex="-1"></a>            metric_value <span class="op">=</span> metric(predicted, labels).to(device)</span>
+<span id="cb56-12"><a href="#cb56-12" aria-hidden="true" tabindex="-1"></a>            loss <span class="op">=</span> loss_function(outputs, labels)</span>
+<span id="cb56-13"><a href="#cb56-13" aria-hidden="true" tabindex="-1"></a>            val_loss <span class="op">+=</span> loss.cpu().numpy()</span>
+<span id="cb56-14"><a href="#cb56-14" aria-hidden="true" tabindex="-1"></a>            val_steps <span class="op">+=</span> <span class="dv">1</span></span>
+<span id="cb56-15"><a href="#cb56-15" aria-hidden="true" tabindex="-1"></a>    loss <span class="op">=</span> val_loss <span class="op">/</span> val_steps</span>
+<span id="cb56-16"><a href="#cb56-16" aria-hidden="true" tabindex="-1"></a>    metric_value <span class="op">=</span> metric.compute()</span>
+<span id="cb56-17"><a href="#cb56-17" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> metric_value, loss</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+</section>
+<section id="description-of-the-test_hold_out-setting" class="level3">
+<h3 class="anchored" data-anchor-id="description-of-the-test_hold_out-setting">Description of the <code>"test_hold_out"</code> Setting</h3>
+<p>It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
+<ol type="1">
+<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
+<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_hold_out()</code> similar to the <code>"train_hold_out"</code> setting with one exception: It passes an additional <code>test</code> data set to <code>evaluate_hold_out()</code> as follows:</li>
+</ol>
+<div class="cell" data-execution_count="47">
+<div class="sourceCode cell-code" id="cb57"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb57-1"><a href="#cb57-1" aria-hidden="true" tabindex="-1"></a>test_dataset<span class="op">=</span>fun_control[<span class="st">"test"</span>]</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p><code>evaluate_hold_out()</code> calls <code>create_train_test_data_loaders</code> instead of <code>create_train_val_data_loaders</code> as follows: The two data sets are used in <code>create_train_test_data_loaders</code> as follows:</p>
+<div class="cell" data-execution_count="48">
+<div class="sourceCode cell-code" id="cb58"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb58-1"><a href="#cb58-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset, num_workers<span class="op">=</span><span class="dv">0</span>):</span>
+<span id="cb58-2"><a href="#cb58-2" aria-hidden="true" tabindex="-1"></a>    trainloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb58-3"><a href="#cb58-3" aria-hidden="true" tabindex="-1"></a>        dataset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb58-4"><a href="#cb58-4" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb58-5"><a href="#cb58-5" aria-hidden="true" tabindex="-1"></a>    testloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb58-6"><a href="#cb58-6" aria-hidden="true" tabindex="-1"></a>        test_dataset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb58-7"><a href="#cb58-7" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb58-8"><a href="#cb58-8" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> trainloader, testloader</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="3" type="1">
+<li>The following steps are identical to the <code>"train_hold_out"</code> setting. Only a different data loader is used for testing.</li>
+</ol>
+</section>
+<section id="detailed-description-of-the-train_cv-setting" class="level3">
+<h3 class="anchored" data-anchor-id="detailed-description-of-the-train_cv-setting">Detailed Description of the <code>"train_cv"</code> Setting</h3>
+<p>It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
+<ol type="1">
+<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
+<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_cv()</code> as follows:</li>
+</ol>
+<div class="cell" data-execution_count="49">
+<div class="sourceCode cell-code" id="cb59"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb59-1"><a href="#cb59-1" aria-hidden="true" tabindex="-1"></a>df_eval, _ <span class="op">=</span> evaluate_cv(</span>
+<span id="cb59-2"><a href="#cb59-2" aria-hidden="true" tabindex="-1"></a>    model,</span>
+<span id="cb59-3"><a href="#cb59-3" aria-hidden="true" tabindex="-1"></a>    dataset<span class="op">=</span>fun_control[<span class="st">"train"</span>],</span>
+<span id="cb59-4"><a href="#cb59-4" aria-hidden="true" tabindex="-1"></a>    shuffle<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"shuffle"</span>],</span>
+<span id="cb59-5"><a href="#cb59-5" aria-hidden="true" tabindex="-1"></a>    device<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"device"</span>],</span>
+<span id="cb59-6"><a href="#cb59-6" aria-hidden="true" tabindex="-1"></a>    show_batch_interval<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"show_batch_interval"</span>],</span>
+<span id="cb59-7"><a href="#cb59-7" aria-hidden="true" tabindex="-1"></a>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>Note: Only the data set <code>fun_control["train"]</code> is used for CV. 3. In `evaluate_cv(), the following steps are performed: The optimizer is set up as follows:</p>
+<div class="cell" data-execution_count="50">
+<div class="sourceCode cell-code" id="cb60"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb60-1"><a href="#cb60-1" aria-hidden="true" tabindex="-1"></a>lr_instance <span class="op">=</span> net.lr</span>
+<span id="cb60-2"><a href="#cb60-2" aria-hidden="true" tabindex="-1"></a>optimizer <span class="op">=</span> optimizer_handler(optimizer_name<span class="op">=</span>optimizer_instance, params<span class="op">=</span>net.parameters(), lr_mult<span class="op">=</span>lr_mult_instance)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p><code>evaluate_cv()</code> sets the <code>net</code> attributes such as <code>epochs</code>, <code>batch_size</code>, <code>optimizer</code>, and <code>patience</code>. CV is implemented as follows:</p>
+<div class="cell" data-execution_count="51">
+<div class="sourceCode cell-code" id="cb61"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb61-1"><a href="#cb61-1" aria-hidden="true" tabindex="-1"></a>kfold <span class="op">=</span> KFold(n_splits<span class="op">=</span>k_folds_instance, shuffle<span class="op">=</span>shuffle)</span>
+<span id="cb61-2"><a href="#cb61-2" aria-hidden="true" tabindex="-1"></a><span class="cf">for</span> fold, (train_ids, val_ids) <span class="kw">in</span> <span class="bu">enumerate</span>(kfold.split(dataset)):</span>
+<span id="cb61-3"><a href="#cb61-3" aria-hidden="true" tabindex="-1"></a>    train_subsampler <span class="op">=</span> torch.utils.data.SubsetRandomSampler(train_ids)</span>
+<span id="cb61-4"><a href="#cb61-4" aria-hidden="true" tabindex="-1"></a>    val_subsampler <span class="op">=</span> torch.utils.data.SubsetRandomSampler(val_ids)</span>
+<span id="cb61-5"><a href="#cb61-5" aria-hidden="true" tabindex="-1"></a>    trainloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb61-6"><a href="#cb61-6" aria-hidden="true" tabindex="-1"></a>        dataset, batch_size<span class="op">=</span>batch_size_instance, sampler<span class="op">=</span>train_subsampler, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb61-7"><a href="#cb61-7" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb61-8"><a href="#cb61-8" aria-hidden="true" tabindex="-1"></a>    valloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb61-9"><a href="#cb61-9" aria-hidden="true" tabindex="-1"></a>        dataset, batch_size<span class="op">=</span>batch_size_instance, sampler<span class="op">=</span>val_subsampler, num_workers<span class="op">=</span>num_workers</span>
+<span id="cb61-10"><a href="#cb61-10" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb61-11"><a href="#cb61-11" aria-hidden="true" tabindex="-1"></a>    reset_weights(net)</span>
+<span id="cb61-12"><a href="#cb61-12" aria-hidden="true" tabindex="-1"></a>    <span class="co"># Train fold for several epochs:</span></span>
+<span id="cb61-13"><a href="#cb61-13" aria-hidden="true" tabindex="-1"></a>    train_fold(</span>
+<span id="cb61-14"><a href="#cb61-14" aria-hidden="true" tabindex="-1"></a>        net,</span>
+<span id="cb61-15"><a href="#cb61-15" aria-hidden="true" tabindex="-1"></a>        trainloader,</span>
+<span id="cb61-16"><a href="#cb61-16" aria-hidden="true" tabindex="-1"></a>        epochs_instance,</span>
+<span id="cb61-17"><a href="#cb61-17" aria-hidden="true" tabindex="-1"></a>        loss_function,</span>
+<span id="cb61-18"><a href="#cb61-18" aria-hidden="true" tabindex="-1"></a>        optimizer,</span>
+<span id="cb61-19"><a href="#cb61-19" aria-hidden="true" tabindex="-1"></a>        device,</span>
+<span id="cb61-20"><a href="#cb61-20" aria-hidden="true" tabindex="-1"></a>        show_batch_interval<span class="op">=</span>show_batch_interval,</span>
+<span id="cb61-21"><a href="#cb61-21" aria-hidden="true" tabindex="-1"></a>    )</span>
+<span id="cb61-22"><a href="#cb61-22" aria-hidden="true" tabindex="-1"></a>    <span class="co"># Validate fold: use only loss for tuning</span></span>
+<span id="cb61-23"><a href="#cb61-23" aria-hidden="true" tabindex="-1"></a>    metric_values[fold], loss_values[fold] <span class="op">=</span> validate_fold_or_hold_out(net, valloader, loss_function, device)</span>
+<span id="cb61-24"><a href="#cb61-24" aria-hidden="true" tabindex="-1"></a>df_eval <span class="op">=</span> <span class="bu">sum</span>(loss_values.values()) <span class="op">/</span> <span class="bu">len</span>(loss_values.values())</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="4" type="1">
+<li>The method <code>train_fold()</code> is implemented as follows:</li>
+</ol>
+<div class="cell" data-execution_count="52">
+<div class="sourceCode cell-code" id="cb62"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb62-1"><a href="#cb62-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interval<span class="op">=</span><span class="dv">10_000</span>):</span>
+<span id="cb62-2"><a href="#cb62-2" aria-hidden="true" tabindex="-1"></a>    <span class="cf">for</span> epoch <span class="kw">in</span> <span class="bu">range</span>(epochs):</span>
+<span id="cb62-3"><a href="#cb62-3" aria-hidden="true" tabindex="-1"></a>        <span class="bu">print</span>(<span class="ss">f"Epoch: </span><span class="sc">{</span>epoch <span class="op">+</span> <span class="dv">1</span><span class="sc">}</span><span class="ss">"</span>)</span>
+<span id="cb62-4"><a href="#cb62-4" aria-hidden="true" tabindex="-1"></a>        running_loss <span class="op">=</span> <span class="fl">0.0</span></span>
+<span id="cb62-5"><a href="#cb62-5" aria-hidden="true" tabindex="-1"></a>        epoch_steps <span class="op">=</span> <span class="dv">0</span></span>
+<span id="cb62-6"><a href="#cb62-6" aria-hidden="true" tabindex="-1"></a>        <span class="cf">for</span> i, data <span class="kw">in</span> <span class="bu">enumerate</span>(trainloader, <span class="dv">0</span>):</span>
+<span id="cb62-7"><a href="#cb62-7" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> data</span>
+<span id="cb62-8"><a href="#cb62-8" aria-hidden="true" tabindex="-1"></a>            inputs, labels <span class="op">=</span> inputs.to(device), labels.to(device)</span>
+<span id="cb62-9"><a href="#cb62-9" aria-hidden="true" tabindex="-1"></a>            optimizer.zero_grad()</span>
+<span id="cb62-10"><a href="#cb62-10" aria-hidden="true" tabindex="-1"></a>            outputs <span class="op">=</span> net(inputs)</span>
+<span id="cb62-11"><a href="#cb62-11" aria-hidden="true" tabindex="-1"></a>            loss <span class="op">=</span> loss_function(outputs, labels)</span>
+<span id="cb62-12"><a href="#cb62-12" aria-hidden="true" tabindex="-1"></a>            loss.backward()</span>
+<span id="cb62-13"><a href="#cb62-13" aria-hidden="true" tabindex="-1"></a>            torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm<span class="op">=</span><span class="fl">1.0</span>)</span>
+<span id="cb62-14"><a href="#cb62-14" aria-hidden="true" tabindex="-1"></a>            optimizer.step()</span>
+<span id="cb62-15"><a href="#cb62-15" aria-hidden="true" tabindex="-1"></a>            <span class="co"># the following is for printing the statistic only</span></span>
+<span id="cb62-16"><a href="#cb62-16" aria-hidden="true" tabindex="-1"></a>            running_loss <span class="op">+=</span> loss.item()</span>
+<span id="cb62-17"><a href="#cb62-17" aria-hidden="true" tabindex="-1"></a>            epoch_steps <span class="op">+=</span> <span class="dv">1</span></span>
+<span id="cb62-18"><a href="#cb62-18" aria-hidden="true" tabindex="-1"></a>            <span class="cf">if</span> i <span class="op">%</span> show_batch_interval <span class="op">==</span> (show_batch_interval <span class="op">-</span> <span class="dv">1</span>):  <span class="co"># print every show_batch_interval mini-batches</span></span>
+<span id="cb62-19"><a href="#cb62-19" aria-hidden="true" tabindex="-1"></a>                <span class="bu">print</span>(<span class="st">"Batch: </span><span class="sc">%5d</span><span class="st">. Training Loss (running): </span><span class="sc">%.3f</span><span class="st">"</span> <span class="op">%</span> (i <span class="op">+</span> <span class="dv">1</span>, running_loss <span class="op">/</span> epoch_steps))</span>
+<span id="cb62-20"><a href="#cb62-20" aria-hidden="true" tabindex="-1"></a>                running_loss <span class="op">=</span> <span class="fl">0.0</span></span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<ol start="5" type="1">
+<li>The method <code>validate_fold_or_hold_out()</code> is implemented as shown above. In contrast to the hold-out setting, it is called for each of the <span class="math inline">\(k\)</span> folds. The results are stored in a dictionaries <code>metric_values</code> and <code>loss_values</code> as follows:</li>
+</ol>
+<div class="cell" data-execution_count="53">
+<div class="sourceCode cell-code" id="cb63"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb63-1"><a href="#cb63-1" aria-hidden="true" tabindex="-1"></a><span class="co"># Validate fold: use only loss for tuning</span></span>
+<span id="cb63-2"><a href="#cb63-2" aria-hidden="true" tabindex="-1"></a>    metric_values[fold], loss_values[fold] <span class="op">=</span> validate_fold_or_hold_out(net, valloader, loss_function, device)</span>
+<span id="cb63-3"><a href="#cb63-3" aria-hidden="true" tabindex="-1"></a>df_eval <span class="op">=</span> <span class="bu">sum</span>(loss_values.values()) <span class="op">/</span> <span class="bu">len</span>(loss_values.values())</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>The results are averaged over the <span class="math inline">\(k\)</span> folds and returned as <code>df_eval</code>.</p>
+</section>
+<section id="detailed-description-of-the-test_cv-setting" class="level3">
+<h3 class="anchored" data-anchor-id="detailed-description-of-the-test_cv-setting">Detailed Description of the <code>"test_cv"</code> Setting</h3>
+<p>It uses the loss function specfied in <code>fun_control</code> and the metric specified in <code>fun_control</code>.</p>
+<ol type="1">
+<li>First, the method <code>HyperTorch().fun_torch</code> is called.</li>
+<li><code>fun_torc()</code> calls <code>spotPython.torch.traintest.evaluate_cv()</code> as follows:</li>
+</ol>
+<div class="cell" data-execution_count="54">
+<div class="sourceCode cell-code" id="cb64"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb64-1"><a href="#cb64-1" aria-hidden="true" tabindex="-1"></a>df_eval, _ <span class="op">=</span> evaluate_cv(</span>
+<span id="cb64-2"><a href="#cb64-2" aria-hidden="true" tabindex="-1"></a>    model,</span>
+<span id="cb64-3"><a href="#cb64-3" aria-hidden="true" tabindex="-1"></a>    dataset<span class="op">=</span>fun_control[<span class="st">"test"</span>],</span>
+<span id="cb64-4"><a href="#cb64-4" aria-hidden="true" tabindex="-1"></a>    shuffle<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"shuffle"</span>],</span>
+<span id="cb64-5"><a href="#cb64-5" aria-hidden="true" tabindex="-1"></a>    device<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"device"</span>],</span>
+<span id="cb64-6"><a href="#cb64-6" aria-hidden="true" tabindex="-1"></a>    show_batch_interval<span class="op">=</span><span class="va">self</span>.fun_control[<span class="st">"show_batch_interval"</span>],</span>
+<span id="cb64-7"><a href="#cb64-7" aria-hidden="true" tabindex="-1"></a>)</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>Note: The data set <code>fun_control["test"]</code> is used for CV. The rest is the same as for the <code>"train_cv"</code> setting.</p>
+</section>
+<section id="sec-final-model-evaluation" class="level3">
+<h3 class="anchored" data-anchor-id="sec-final-model-evaluation">Detailed Description of the Final Model Training and Evaluation</h3>
+<section id="detailed-description-of-the-train_tuned-procedure" class="level4">
+<h4 class="anchored" data-anchor-id="detailed-description-of-the-train_tuned-procedure">Detailed Description of the <code>"train_tuned</code> Procedure</h4>
+<p><code>train_tuned()</code> is just a wrapper to <code>evaluate_hold_out</code> using the <code>train</code> data set. It is implemented as follows:</p>
+<div class="cell" data-execution_count="55">
+<div class="sourceCode cell-code" id="cb65"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb65-1"><a href="#cb65-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> train_tuned(net, train_dataset, shuffle, loss_function, metric, device<span class="op">=</span><span class="va">None</span>, show_batch_interval<span class="op">=</span><span class="dv">10_000</span>, path<span class="op">=</span><span class="va">None</span>):</span>
+<span id="cb65-2"><a href="#cb65-2" aria-hidden="true" tabindex="-1"></a>    evaluate_hold_out(</span>
+<span id="cb65-3"><a href="#cb65-3" aria-hidden="true" tabindex="-1"></a>        net<span class="op">=</span>net,</span>
+<span id="cb65-4"><a href="#cb65-4" aria-hidden="true" tabindex="-1"></a>        train_dataset<span class="op">=</span>train_dataset,</span>
+<span id="cb65-5"><a href="#cb65-5" aria-hidden="true" tabindex="-1"></a>        shuffle<span class="op">=</span>shuffle,</span>
+<span id="cb65-6"><a href="#cb65-6" aria-hidden="true" tabindex="-1"></a>        test_dataset<span class="op">=</span><span class="va">None</span>,</span>
+<span id="cb65-7"><a href="#cb65-7" aria-hidden="true" tabindex="-1"></a>        loss_function<span class="op">=</span>loss_function,</span>
+<span id="cb65-8"><a href="#cb65-8" aria-hidden="true" tabindex="-1"></a>        metric<span class="op">=</span>metric,</span>
+<span id="cb65-9"><a href="#cb65-9" aria-hidden="true" tabindex="-1"></a>        device<span class="op">=</span>device,</span>
+<span id="cb65-10"><a href="#cb65-10" aria-hidden="true" tabindex="-1"></a>        show_batch_interval<span class="op">=</span>show_batch_interval,</span>
+<span id="cb65-11"><a href="#cb65-11" aria-hidden="true" tabindex="-1"></a>        path<span class="op">=</span>path,</span>
+<span id="cb65-12"><a href="#cb65-12" aria-hidden="true" tabindex="-1"></a>    )</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<p>The <code>test_tuned()</code> procedure is implemented as follows:</p>
+<div class="cell" data-execution_count="56">
+<div class="sourceCode cell-code" id="cb66"><pre class="sourceCode python code-with-copy"><code class="sourceCode python"><span id="cb66-1"><a href="#cb66-1" aria-hidden="true" tabindex="-1"></a><span class="kw">def</span> test_tuned(net, shuffle, test_dataset<span class="op">=</span><span class="va">None</span>, loss_function<span class="op">=</span><span class="va">None</span>, metric<span class="op">=</span><span class="va">None</span>, device<span class="op">=</span><span class="va">None</span>, path<span class="op">=</span><span class="va">None</span>):</span>
+<span id="cb66-2"><a href="#cb66-2" aria-hidden="true" tabindex="-1"></a>    batch_size_instance <span class="op">=</span> net.batch_size</span>
+<span id="cb66-3"><a href="#cb66-3" aria-hidden="true" tabindex="-1"></a>    removed_attributes, net <span class="op">=</span> get_removed_attributes_and_base_net(net)</span>
+<span id="cb66-4"><a href="#cb66-4" aria-hidden="true" tabindex="-1"></a>    <span class="cf">if</span> path <span class="kw">is</span> <span class="kw">not</span> <span class="va">None</span>:</span>
+<span id="cb66-5"><a href="#cb66-5" aria-hidden="true" tabindex="-1"></a>        net.load_state_dict(torch.load(path))</span>
+<span id="cb66-6"><a href="#cb66-6" aria-hidden="true" tabindex="-1"></a>        net.<span class="bu">eval</span>()</span>
+<span id="cb66-7"><a href="#cb66-7" aria-hidden="true" tabindex="-1"></a>    <span class="cf">try</span>:</span>
+<span id="cb66-8"><a href="#cb66-8" aria-hidden="true" tabindex="-1"></a>        device <span class="op">=</span> getDevice(device<span class="op">=</span>device)</span>
+<span id="cb66-9"><a href="#cb66-9" aria-hidden="true" tabindex="-1"></a>        <span class="cf">if</span> torch.cuda.is_available():</span>
+<span id="cb66-10"><a href="#cb66-10" aria-hidden="true" tabindex="-1"></a>            device <span class="op">=</span> <span class="st">"cuda:0"</span></span>
+<span id="cb66-11"><a href="#cb66-11" aria-hidden="true" tabindex="-1"></a>            <span class="cf">if</span> torch.cuda.device_count() <span class="op">&gt;</span> <span class="dv">1</span>:</span>
+<span id="cb66-12"><a href="#cb66-12" aria-hidden="true" tabindex="-1"></a>                <span class="bu">print</span>(<span class="st">"We will use"</span>, torch.cuda.device_count(), <span class="st">"GPUs!"</span>)</span>
+<span id="cb66-13"><a href="#cb66-13" aria-hidden="true" tabindex="-1"></a>                net <span class="op">=</span> nn.DataParallel(net)</span>
+<span id="cb66-14"><a href="#cb66-14" aria-hidden="true" tabindex="-1"></a>        net.to(device)</span>
+<span id="cb66-15"><a href="#cb66-15" aria-hidden="true" tabindex="-1"></a>        valloader <span class="op">=</span> torch.utils.data.DataLoader(</span>
+<span id="cb66-16"><a href="#cb66-16" aria-hidden="true" tabindex="-1"></a>            test_dataset, batch_size<span class="op">=</span><span class="bu">int</span>(batch_size_instance), shuffle<span class="op">=</span>shuffle, num_workers<span class="op">=</span><span class="dv">0</span></span>
+<span id="cb66-17"><a href="#cb66-17" aria-hidden="true" tabindex="-1"></a>        )</span>
+<span id="cb66-18"><a href="#cb66-18" aria-hidden="true" tabindex="-1"></a>        metric_value, loss <span class="op">=</span> validate_fold_or_hold_out(</span>
+<span id="cb66-19"><a href="#cb66-19" aria-hidden="true" tabindex="-1"></a>            net, valloader<span class="op">=</span>valloader, loss_function<span class="op">=</span>loss_function, metric<span class="op">=</span>metric, device<span class="op">=</span>device</span>
+<span id="cb66-20"><a href="#cb66-20" aria-hidden="true" tabindex="-1"></a>        )</span>
+<span id="cb66-21"><a href="#cb66-21" aria-hidden="true" tabindex="-1"></a>        df_eval <span class="op">=</span> loss</span>
+<span id="cb66-22"><a href="#cb66-22" aria-hidden="true" tabindex="-1"></a>        df_metric <span class="op">=</span> metric_value</span>
+<span id="cb66-23"><a href="#cb66-23" aria-hidden="true" tabindex="-1"></a>        df_preds <span class="op">=</span> np.nan</span>
+<span id="cb66-24"><a href="#cb66-24" aria-hidden="true" tabindex="-1"></a>    <span class="cf">except</span> <span class="pp">Exception</span> <span class="im">as</span> err:</span>
+<span id="cb66-25"><a href="#cb66-25" aria-hidden="true" tabindex="-1"></a>        <span class="bu">print</span>(<span class="ss">f"Error in Net_Core. Call to test_tuned() failed. </span><span class="sc">{</span>err<span class="op">=</span><span class="sc">}</span><span class="ss">, </span><span class="sc">{</span><span class="bu">type</span>(err)<span class="op">=</span><span class="sc">}</span><span class="ss">"</span>)</span>
+<span id="cb66-26"><a href="#cb66-26" aria-hidden="true" tabindex="-1"></a>        df_eval <span class="op">=</span> np.nan</span>
+<span id="cb66-27"><a href="#cb66-27" aria-hidden="true" tabindex="-1"></a>        df_metric <span class="op">=</span> np.nan</span>
+<span id="cb66-28"><a href="#cb66-28" aria-hidden="true" tabindex="-1"></a>        df_preds <span class="op">=</span> np.nan</span>
+<span id="cb66-29"><a href="#cb66-29" aria-hidden="true" tabindex="-1"></a>    add_attributes(net, removed_attributes)</span>
+<span id="cb66-30"><a href="#cb66-30" aria-hidden="true" tabindex="-1"></a>    <span class="bu">print</span>(<span class="ss">f"Final evaluation: Validation loss: </span><span class="sc">{</span>df_eval<span class="sc">}</span><span class="ss">"</span>)</span>
+<span id="cb66-31"><a href="#cb66-31" aria-hidden="true" tabindex="-1"></a>    <span class="bu">print</span>(<span class="ss">f"Final evaluation: Validation metric: </span><span class="sc">{</span>df_metric<span class="sc">}</span><span class="ss">"</span>)</span>
+<span id="cb66-32"><a href="#cb66-32" aria-hidden="true" tabindex="-1"></a>    <span class="bu">print</span>(<span class="st">"----------------------------------------------"</span>)</span>
+<span id="cb66-33"><a href="#cb66-33" aria-hidden="true" tabindex="-1"></a>    <span class="cf">return</span> df_eval, df_preds, df_metric</span></code><button title="Copy to Clipboard" class="code-copy-button"><i class="bi"></i></button></pre></div>
+</div>
+<div style="page-break-after: always;"></div>
+</section>
+</section>
+</section>
 </section>
 <section id="references" class="level1 unnumbered">
 <h1 class="unnumbered">References</h1>
 <div id="refs" class="references csl-bib-body hanging-indent" role="list">
 <div id="ref-bart21i" class="csl-entry" role="listitem">
 Bartz, Eva, Thomas Bartz-Beielstein, Martin Zaefferer, and Olaf Mersmann, eds. 2022. <em><span class="nocase">Hyperparameter Tuning for Machine and Deep Learning with R - A Practical Guide</span></em>. Springer.
 </div>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 
 
 
 ***** Other Formats *****
     * PDF
 
 ****** PyTorch Hyperparameter Tuning â A Tutorial for spotPython ******
-Version 0.2.0
+Version 0.2.1
 Author
 Affiliations
 Thomas_Bartz-Beielstein [data:image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/
 9hAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAA2ZpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/
 eHBhY2tldCBiZWdpbj0i77u/
 IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuMC1jMDYwIDYxLjEzNDc3NywgMjAxMC8wMi8xMi0xNzozMjowMCAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wTU09Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9tbS8iIHhtbG5zOnN0UmVmPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvc1R5cGUvUmVzb3VyY2VSZWYjIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDo1N0NEMjA4MDI1MjA2ODExOTk0QzkzNTEzRjZEQTg1NyIgeG1wTU06RG9jdW1lbnRJRD0ieG1wLmRpZDozM0NDOEJGNEZGNTcxMUUxODdBOEVCODg2RjdCQ0QwOSIgeG1wTU06SW5zdGFuY2VJRD0ieG1wLmlpZDozM0NDOEJGM0ZGNTcxMUUxODdBOEVCODg2RjdCQ0QwOSIgeG1wOkNyZWF0b3JUb29sPSJBZG9iZSBQaG90b3Nob3AgQ1M1IE1hY2ludG9zaCI+IDx4bXBNTTpEZXJpdmVkRnJvbSBzdFJlZjppbnN0YW5jZUlEPSJ4bXAuaWlkOkZDN0YxMTc0MDcyMDY4MTE5NUZFRDc5MUM2MUUwNEREIiBzdFJlZjpkb2N1bWVudElEPSJ4bXAuZGlkOjU3Q0QyMDgwMjUyMDY4MTE5OTRDOTM1MTNGNkRBODU3Ii8+IDwvcmRmOkRlc2NyaXB0aW9uPiA8L3JkZjpSREY+IDwveDp4bXBtZXRhPiA8P3hwYWNrZXQgZW5kPSJyIj8+84NovQAAAR1JREFUeNpiZEADy85ZJgCpeCB2QJM6AMQLo4yOL0AWZETSqACk1gOxAQN+cAGIA4EGPQBxmJA0nwdpjjQ8xqArmczw5tMHXAaALDgP1QMxAGqzAAPxQACqh4ER6uf5MBlkm0X4EGayMfMw/
@@ -78,17 +78,19 @@
 Last but not least, it should be noted that the SPOT software code is available
 in the open source spotPython package on github1, allowing replicability of the
 results. This tutorial descries the Python variant of SPOT, which is called
 spotPython. The R implementation is described in Bartz et al. (2022). SPOT is
 an established open source software that has been maintained for more than 15
 years (Bartz-Beielstein,_Lasarczyk,_and_Preuss_2005) (Bartz_et_al._2022).
 This tutorial is structured as follows. The concept of the hyperparameter
-tuning software spotPython is described in Section 2. Section 3 describes the
-integration of spotPython into the PyTorch training workflow and presents the
-results. Finally, Section 4 presents a summary and an outlook.
+tuning software spotPython is described in Section 2. Section 3
+(âQuickstartâ) describes the execution of the example from the tutorial
+âHyperparameter Tuning with Ray Tuneâ (PyTorch_2023a). Section 4 describes
+the integration of spotPython into the PyTorch training workflow in detail and
+presents the results. Finally, Section 5 presents a summary and an outlook.
 Note
 The corresponding .ipynb notebook (Bartz-Beielstein_2023) is updated regularly
 and reflects updates and changes in the spotPython package. It can be
 downloaded from https://github.com/sequential-parameter-optimization/
 spotPython/blob/main/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb.
 
 ****** The Hyperparameter Tuning Software SPOT ******
@@ -107,51 +109,168 @@
 and sensitivity analysis. It can be used to understand the performance of
 various algorithms, while simultaneously giving insights into their algorithmic
 behavior. In addition, SPOT can be used as an optimizer and for automatic and
 interactive tuning. Details on SPOT and its use in practice are given by Bartz
 et al. (2022).
 A typical hyperparameter tuning process with spotPython consists of the
 following steps:
-   1. Loading the data (training and test datasets), see Section 3.3.
-   2. Specification of the preprocessing model, see Section 3.4. This model is
+   1. Loading the data (training and test datasets), see Section 4.3.
+   2. Specification of the preprocessing model, see Section 4.4. This model is
       called prep_model (âpreparationâ or pre-processing). The information
       required for the hyperparameter tuning is stored in the dictionary
       fun_control. Thus, the information needed for the execution of the
       hyperparameter tuning is available in a readable form.
    3. Selection of the machine learning or deep learning model to be tuned, see
-      Section 3.5. This is called the core_model. Once the core_model is
+      Section 4.5. This is called the core_model. Once the core_model is
       defined, then the associated hyperparameters are stored in the
       fun_control dictionary. First, the hyperparameters of the core_model are
       initialized with the default values of the core_model. As default values
       we use the default values contained in the spotPython package for the
       algorithms of the torch package.
    4. Modification of the default values for the hyperparameters used in
-      core_model, see Section 3.7.1. This step is optional.
+      core_model, see Section 4.7.1. This step is optional.
          1. numeric parameters are modified by changing the bounds.
          2. categorical parameters are modified by changing the categories
             (âlevelsâ).
    5. Selection of target function (loss function) for the optimizer, see
-      Section 3.8.
-   6. Calling SPOT with the corresponding parameters, see Section 3.9. The
+      Section 4.8.
+   6. Calling SPOT with the corresponding parameters, see Section 4.9. The
       results are stored in a dictionary and are available for further
       analysis.
    7. Presentation, visualization and interpretation of the results, see
-      Section 3.10.
+      Section 4.10.
+
+****** Quickstart ******
+import numpy as np
+from math import inf
+import torchmetrics
+from torch.nn import CrossEntropyLoss
+from spotPython.spot import spot
+from spotPython.utils.init import fun_control_init
+from spotPython.data.torchdata import load_data_cifar10
+from spotPython.hyperparameters.values import (
+    add_core_model_to_fun_control,
+    modify_hyper_parameter_levels,
+    modify_hyper_parameter_bounds,
+    get_var_type,
+    get_var_name,
+    get_bound_values,
+    get_one_core_model_from_X,
+    get_default_hyperparameters_as_array
+    )
+from spotPython.data.torch_hyper_dict import TorchHyperDict
+from spotPython.data.torchdata import load_data_cifar10
+from spotPython.fun.hypertorch import HyperTorch
+from spotPython.torch.netcifar10 import Net_CIFAR10
+from spotPython.torch.traintest import (
+    train_tuned,
+    test_tuned,
+    )
+fun_control = fun_control_init()
+# load data
+train, test = load_data_cifar10()
+# add the dataset to the fun_control
+fun_control.update({
+    "train": train,
+    "test": test,
+    "n_samples": len(train)})
+# add the nn model to the fun_control dictionary
+fun_control = add_core_model_to_fun_control(core_model=Net_CIFAR10,
+                              fun_control=fun_control,
+                              hyper_dict=TorchHyperDict)
+# modify the hyperparameter levels
+fun_control = modify_hyper_parameter_bounds(fun_control, "lr_mult", bounds=[1e-
+3, 1e-3])
+fun_control = modify_hyper_parameter_bounds(fun_control, "sgd_momentum",
+bounds=[0.9, 0.9])
+fun_control = modify_hyper_parameter_levels(fun_control, "optimizer",["Adam",
+"SGD"])
+# select metric and loss function
+fun_control.update({
+               "metric_torch": torchmetrics.Accuracy(task="multiclass",
+num_classes=10),
+               "loss_function": CrossEntropyLoss(),
+               "device": "cpu",
+               })
+# extract the variable types, names, and bounds
+var_type = get_var_type(fun_control)
+var_name = get_var_name(fun_control)
+fun_control.update({"var_type": var_type,
+                    "var_name": var_name})
+lower = get_bound_values(fun_control, "lower")
+upper = get_bound_values(fun_control, "upper")
+
+# get the default hyperparameters as array
+hyper_dict=TorchHyperDict().load()
+X_start = get_default_hyperparameters_as_array(fun_control, hyper_dict)
+
+# get the objective function
+fun = HyperTorch().fun_torch
+
+# initialize spot
+spot_tuner = spot.Spot(fun=fun,
+                   lower = lower,
+                   upper = upper,
+                   fun_evals = inf,
+                   fun_repeats = 1,
+                   max_time = 30,
+                   noise = False,
+                   tolerance_x = np.sqrt(np.spacing(1)),
+                   var_type = var_type,
+                   var_name = var_name,
+                   infill_criterion = "y",
+                   n_points = 1,
+                   seed=123,
+                   log_level = 50,
+                   show_models= False,
+                   show_progress= True,
+                   fun_control = fun_control,
+                   design_control={"init_size": 10,
+                                   "repeats": 1},
+                   surrogate_control={"noise": True,
+                                      "cod_type": "norm",
+                                      "min_theta": -4,
+                                      "max_theta": 3,
+                                      "n_theta": len(var_name),
+                                      "model_fun_evals": 10_000,
+                                      "log_level": 50
+                                      })
+# run spot
+spot_tuner.run(X_start=X_start)
+spot_tuner.plot_progress()
+from spotPython.utils.eda import gen_design_table
+print(gen_design_table(fun_control=fun_control, spot=spot_tuner))
+spot_tuner.plot_importance()
+X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1,-1))
+model_spot = get_one_core_model_from_X(X, fun_control)
+model_spot
+train_tuned(net=model_spot, train_dataset=train,
+        loss_function=fun_control["loss_function"],
+        metric=fun_control["metric_torch"],
+        shuffle=True,
+        device = "cpu",
+        path=None)
+test_tuned(net=model_spot, test_dataset=test,
+            shuffle=False,
+            loss_function=fun_control["loss_function"],
+            metric=fun_control["metric_torch"],
+            device = "cpu")
+spot_tuner.plot_important_hyperparameter_contour()
 
 ****** Hyperparameter Tuning for PyTorch With spotPython ******
 In this tutorial, we will show how spotPython can be integrated into the
 PyTorch training workflow. It is based on the tutorial âHyperparameter Tuning
 with Ray Tuneâ from the PyTorch documentation (PyTorch_2023a), which is an
 extension of the tutorial âTraining a Classifierâ (PyTorch_2023b) for
 training a CIFAR10 image classifier.
 This document refers to the following software versions:
     * python: 3.10.10
     * torch: 2.0.1
     * torchvision: 0.15.0
-    * spotPython: 0.2.0
+    * spotPython: 0.2.1
 spotPython can be installed via pip2.
 !pip install spotPython
 Results that refer to the Ray Tune package are taken from https://PyTorch.org/
 tutorials/beginner/hyperparameter_tuning_tutorial.html3.
 ***** Setup *****
 Before we consider the detailed experimental setup, we select the parameters
 that affect run time, initial design size and the device that is used.
@@ -169,31 +288,35 @@
 tuned, the classification (or regression) problem, and the data that is used
 for the tuning. The dictionary is used as an input for the SPOT function.
 fun_control = fun_control_init()
 
 ***** Data Loading *****
 The data loading process is implemented in the same manner as described in the
 Section âData loadersâ in PyTorch (2023a). The data loaders are wrapped
-into the function load_data. A global data directory is used, which allows
+into the function load_data_cifar10 which is identical to the function
+load_data in PyTorch (2023a). A global data directory is used, which allows
 sharing the data directory between different trials.
-def load_data(data_dir="./data"):
+def load_data_cifar10(data_dir="./data"):
     transform = transforms.Compose([
         transforms.ToTensor(),
         transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))
     ])
 
     trainset = torchvision.datasets.CIFAR10(
         root=data_dir, train=True, download=True, transform=transform)
 
     testset = torchvision.datasets.CIFAR10(
         root=data_dir, train=False, download=True, transform=transform)
 
     return trainset, testset
-The test and train data are added to the dictionary fun_control.
-train, test = load_data()
+The method load_data_cifar10 is part of the spotPython package and can be
+imported from spotPython.data.torchdata.
+In the following step, the test and train data are added to the dictionary
+fun_control.
+train, test = load_data_cifar10()
 n_samples = len(train)
 # add the dataset to the fun_control
 fun_control.update({
     "train": train,
     "test": test,
     "n_samples": n_samples})
 
@@ -220,16 +343,16 @@
 None here.
 prep_model = None
 fun_control.update({"prep_model": prep_model})
 
 ***** Select algorithm and core_model_hyper_dict *****
 The same neural network model as implemented in the section âConfigurable
 neural networkâ of the PyTorch tutorial (PyTorch_2023a) is used here. We will
-show the implementation from PyTorch (2023a) in Section 3.5.1 first, before the
-extended implementation with spotPython is shown in Section 3.5.2.
+show the implementation from PyTorch (2023a) in Section 4.5.1 first, before the
+extended implementation with spotPython is shown in Section 4.5.2.
 **** Implementing a Configurable Neural Network With Ray Tune ****
 We used the same hyperparameters that are implemented as configurable in the
 PyTorch tutorial. We specify the layer sizes, namely l1 and l2, of the fully
 connected layers:
 class Net(nn.Module):
     def __init__(self, l1=120, l2=84):
         super(Net, self).__init__()
@@ -251,21 +374,30 @@
 The learning rate, i.e., lr, of the optimizer is made configurable, too:
 optimizer = optim.SGD(net.parameters(), lr=config["lr"], momentum=0.9)
 
 **** Implementing a Configurable Neural Network With spotPython ****
 spotPython implements a class which is similar to the class described in the
 PyTorch tutorial. The class is called Net_CIFAR10 and is implemented in the
 file netcifar10.py.
+from torch import nn
+import torch.nn.functional as F
 import spotPython.torch.netcore as netcore
+
+
 class Net_CIFAR10(netcore.Net_Core):
-    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience):
+    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience,
+optimizer, sgd_momentum):
         super(Net_CIFAR10, self).__init__(
-            lr_mult=lr_mult, batch_size=batch_size, epochs=epochs,
-k_folds=k_folds,
-            patience=patience
+            lr_mult=lr_mult,
+            batch_size=batch_size,
+            epochs=epochs,
+            k_folds=k_folds,
+            patience=patience,
+            optimizer=optimizer,
+            sgd_momentum=sgd_momentum,
         )
         self.conv1 = nn.Conv2d(3, 6, 5)
         self.pool = nn.MaxPool2d(2, 2)
         self.conv2 = nn.Conv2d(6, 16, 5)
         self.fc1 = nn.Linear(16 * 5 * 5, l1)
         self.fc2 = nn.Linear(l1, l2)
         self.fc3 = nn.Linear(l2, 10)
@@ -284,21 +416,34 @@
 the batch size batch_size, the number of epochs epochs, the number of folds
 k_folds for the cross validation, and the patience patience for the early
 stopping. The class Net_Core is shown below.
 from torch import nn
 
 
 class Net_Core(nn.Module):
-    def __init__(self, lr_mult, batch_size, epochs, k_folds, patience):
+    def __init__(self, lr_mult, batch_size, epochs, k_folds, patience,
+optimizer, sgd_momentum):
         super(Net_Core, self).__init__()
         self.lr_mult = lr_mult
         self.batch_size = batch_size
         self.epochs = epochs
         self.k_folds = k_folds
         self.patience = patience
+        self.optimizer = optimizer
+        self.sgd_momentum = sgd_momentum
+The Net_Core class
+The Net_Core class is implemented in the file netcore.py. It implements
+hyperparameters as attributes, that are not used by the core_model, e.g.:
+    * optimizer (optimizer),
+    * learning rate (lr),
+    * batch size (batch_size),
+    * epochs (epochs),
+    * k_folds (k_folds), and
+    * early stopping criterion âpatienceâ (patience).
+Users can add further attributes to the class.
 
 **** Comparison of the Approach Described in the PyTorch Tutorial With
 spotPython ****
 Comparing the class Net from the PyTorch tutorial and the class Net_CIFAR10
 from spotPython, we see that the class Net_CIFAR10 has additional attributes
 and does not inherit from nn directly. It adds an additional class, Net_core,
 that takes care of additional attributes that are common to all neural network
@@ -311,28 +456,19 @@
 The method add_core_model_to_fun_control adds the hyperparameters and
 additional attributes to the fun_control dictionary. The method is shown below.
 core_model = Net_CIFAR10
 fun_control = add_core_model_to_fun_control(core_model=core_model,
                               fun_control=fun_control,
                               hyper_dict=TorchHyperDict,
                               filename=None)
-Note
-In addition to the class Net from the PyTorch tutorial, the class Net_CIFAR10
-has additional attributes, e.g.:
-    * learning rate (lr),
-    * batch size (batch_size),
-    * epochs (epochs),
-    * k_folds (k_folds), and
-    * early stopping criterion âpatienceâ (patience)
-Further attributes can be easily added to the class, e.g., optimizer.
 
 ***** The Search Space *****
-In Section 3.6.1, we first describe how to configure the search space with ray
+In Section 4.6.1, we first describe how to configure the search space with ray
 [tune] (as shown in PyTorch (2023a)) and then how to configure the search space
-with spotPython in Section 3.6.2.
+with spotPython in Section 4.6.2.
 **** Configuring the Search Space With Ray Tune ****
 Ray Tuneâs search space can be configured as follows (PyTorch_2023a):
 config = {
     "l1": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),
     "l2": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),
     "lr": tune.loguniform(1e-4, 1e-1),
     "batch_size": tune.choice([2, 4, 8, 16])
@@ -345,32 +481,32 @@
 At each trial, ray[tune] will randomly sample a combination of parameters from
 these search spaces. It will then train a number of models in parallel and find
 the best performing one among these. ray[tune] uses the ASHAScheduler which
 will terminate bad performing trials early.
 
 **** Configuring the Search Space With spotPython ****
 *** The hyper_dict Hyperparameters for the Selected Algorithm ***
-spotPython uses simple JSON files for the specification of the hyperparameters.
-Users can specify their individual JSON files, or they can use the JSON files
+spotPython uses JSON files for the specification of the hyperparameters. Users
+can specify their individual JSON files, or they can use the JSON files
 provided by spotPython. The JSON file for the core_model is called
 torch_hyper_dict.json.
 In contrast to ray[tune], spotPython can handle numerical, boolean, and
 categorical hyperparameters. They can be specified in the JSON file in a
-similar way as the numerical hyperparameters as shown below:
+similar way as the numerical hyperparameters as shown below. Each entry in the
+JSON file represents one hyperparameter with the following structure: type,
+default, transform, lower, and upper.
 "factor_hyperparameter": {
     "levels": ["A", "B", "C"],
     "type": "factor",
     "default": "B",
     "transform": "None",
     "core_model_parameter_type": "str",
     "lower": 0,
     "upper": 2},
-Each entry in the JSON file represents one hyperparameter with the following
-structure: type, default, transform, lower, and upper. The corresponding
-entries for the Net_CIFAR10 class are shown below.
+The corresponding entries for the Net_CIFAR10 class are shown below.
 {"Net_CIFAR10":
     {
         "l1": {
             "type": "int",
             "default": 5,
             "transform": "transform_power_2_int",
             "lower": 2,
@@ -479,15 +615,15 @@
 during the spotPython hyperparameter tuning. The hyperparameter optimizer is
 active.
 fun_control = modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD",
 "Adam"])
 The hyperparameter optimizer can be de-activated by choosing only one value
 (level), here: "SGD".
 fun_control = modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD"])
-As discussed in Section 3.7.4, there are some issues with the LBFGS optimizer.
+As discussed in Section 4.7.4, there are some issues with the LBFGS optimizer.
 Therefore, the usage of the LBFGS optimizer is not deactivated in spotPython by
 default. However, the LBFGS optimizer can be activated by adding it to the list
 of optimizers. Rprop was removed, because it does perform very poorly (as some
 pre-tests have shown). However, it can also be activated by adding it to the
 list of optimizers. Since SparseAdam does not support dense gradients, Adam was
 used instead. Therefore, there are 10 default optimizers:
 fun_control = modify_hyper_parameter_levels(fun_control, "optimizer",
@@ -528,17 +664,17 @@
 Furthermore, the LBFGS optimizer is not compatible with the PyTorch tutorial.
 The reason is that the LBFGS optimizer requires the closure function, which is
 not implemented in the PyTorch tutorial. Therefore, the LBFGS optimizer is
 recommended here.
 Since there are 10 optimizers in the portfolio, it is not recommended tuning
 the hyperparameters that effect one single optimizer only.
 A note on the learning rate
-spotPython provides a multiplier for the default learning rates, because
-optimizers use different learning rates. Using a multiplier for the learning
-rates might enable a simultaneous tuning of the learning rates for all
+spotPython provides a multiplier for the default learning rates, lr_mult,
+because optimizers use different learning rates. Using a multiplier for the
+learning rates might enable a simultaneous tuning of the learning rates for all
 optimizers. However, this is not recommended, because the learning rates are
 not comparable across optimizers. Therefore, we recommend fixing the learning
 rate for all optimizers if multiple optimizers are used. This can be done by
 setting the lower and upper bounds of the learning rate multiplier to the same
 value as shown below.
 Thus, the learning rate, which affects the SGD optimizer, will be set to a
 fixed value. We choose the default value of 1e-3 for the learning rate, because
@@ -571,22 +707,22 @@
 The following splits are performed in the hold-out setting: \(\{\text{train}_0,
 \text{test}\} \rightarrow \{\text{train}_1, \text{validation}_1, \text
 {test}\}\), where \(\text{train}_1 \cup \text{validation}_1 = \text{train}_0\).
 Note
 spotPython returns the hyperparameters of the machine learning and deep
 learning models, e.g., number of layers, learning rate, or optimizer, but not
 the model weights. Therefore, after the SPOT run is finished, the corresponding
-model has to be trained again with the best hyperparameter configuration. The
-training is performed on the training data set. The test data set is used for
-the final evaluation of the model.
+model with the optimized architecture has to be trained again with the best
+hyperparameter configuration. The training is performed on the training data
+set. The test data set is used for the final evaluation of the model.
 Summarizing, the following splits are performed in the hold-out setting:
    1. Run spotPython with eval set to train_hold_out to determine the best
       hyperparameter configuration.
-   2. Train the model with the best hyperparameter configuration on the
-      training data set:
+   2. Train the model with the best hyperparameter configuration
+      (âarchitectureâ) on the training data set:
           o train_tuned(model_spot, train, "model_spot.pt").
    3. Test the model on the test data:
           o test_tuned(model_spot, test, "model_spot.pt")
 These steps will be exemplified in the following sections.
 In addition to this hold-out setting, spotPython provides another hold-out
 setting, where an explicit test data is specified by the user that will be used
 as the validation set. To choose this option, the eval parameter is set to
@@ -624,296 +760,34 @@
 "train_cv"       \                           evaluate_cv(net, train)   CV using the train data
                  (\checkmark\)                                         set
                                                                        CV using the test data
 "test_cv"                      \             evaluate_cv(net, test)    set . Identical to
                                (\checkmark\)                           "train_cv", uses only
                                                                        test data.
     * "train_cv" and "test_cv" use sklearn.model_selection.KFold() internally.
-
-*** Detailed Description of the "train_hold_out" Setting ***
-The "train_hold_out" setting is used by default. It uses the loss function
-specfied in fun_control and the metric specified in fun_control.
-   1. First, the method HyperTorch().fun_torch is called.
-   2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() as
-      follows:
-df_eval, _ = evaluate_hold_out(
-    model,
-    train_dataset=fun_control["train"],
-    shuffle=self.fun_control["shuffle"],
-    loss_function=self.fun_control["loss_function"],
-    metric=self.fun_control["metric_torch"],
-    device=self.fun_control["device"],
-    show_batch_interval=self.fun_control["show_batch_interval"],
-    path=self.fun_control["path"],
-)
-Note: Only the data set fun_control["train"] is used for training and
-validation. It is used as follows:
-trainloader, valloader = create_train_val_data_loaders(
-                dataset=train_dataset, batch_size=batch_size_instance,
-shuffle=shuffle
-            )
-create_train_val_data_loaders() splits the train_dataset into trainloader and
-valloader using torch.utils.data.random_split() as follows:
-def create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):
-    test_abs = int(len(dataset) * 0.6)
-    train_subset, val_subset = random_split(dataset, [test_abs, len(dataset) -
-test_abs])
-    trainloader = torch.utils.data.DataLoader(
-        train_subset, batch_size=int(batch_size), shuffle=shuffle,
-num_workers=num_workers
-    )
-    valloader = torch.utils.data.DataLoader(
-        val_subset, batch_size=int(batch_size), shuffle=shuffle,
-num_workers=num_workers
-    )
-    return trainloader, valloader
-The optimizer is set up as follows:
-lr_mult_instance = net.lr_mult
-optimizer = optimizer_handler(optimizer_name=optimizer_instance,
-params=net.parameters(), lr_mult=lr_mult_instance)
-   1. evaluate_hold_out() sets the net attributes such as epochs, batch_size,
-      optimizer, and patience. For each epoch, the methods train_hold_out() and
-      validate_fold_or_hold_out() are called, the former for training and the
-      latter for validation and early stopping. The validation loss from the
-      last epoch (not the best validation loss) is returned from
-      evaluate_hold_out.
-   2. The method train_hold_out() is implemented as follows:
-def train_hold_out(net, trainloader, batch_size, loss_function, optimizer,
-device, show_batch_interval=10_000):
-    running_loss = 0.0
-    epoch_steps = 0
-    for i, data in enumerate(trainloader, 0):
-        inputs, labels = data
-        inputs, labels = inputs.to(device), labels.to(device)
-        optimizer.zero_grad()
-        outputs = net(inputs)
-        loss = loss_function(outputs, labels)
-        loss.backward()
-        torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
-        optimizer.step()
-        running_loss += loss.item()
-        epoch_steps += 1
-        if i % show_batch_interval == (show_batch_interval - 1):  # print every
-show_batch_interval mini-batches
-            print(
-                "Batch: %5d. Batch Size: %d. Training Loss (running): %.3f"
-                % (i + 1, int(batch_size), running_loss / epoch_steps)
-            )
-            running_loss = 0.0
-    return loss.item()
-   1. The method validate_fold_or_hold_out() is implemented as follows:
-def validate_fold_or_hold_out(net, valloader, loss_function, metric, device):
-    val_loss = 0.0
-    val_steps = 0
-    metric.reset()
-    for i, data in enumerate(valloader, 0):
-        with torch.no_grad():
-            inputs, labels = data
-            inputs, labels = inputs.to(device), labels.to(device)
-            outputs = net(inputs)
-            _, predicted = torch.max(outputs.data, 1)
-            metric_value = metric(predicted, labels).to(device)
-            loss = loss_function(outputs, labels)
-            val_loss += loss.cpu().numpy()
-            val_steps += 1
-    loss = val_loss / val_steps
-    metric_value = metric.compute()
-    return metric_value, loss
-
-*** Detailed Description of the "test_hold_out" Setting ***
-It uses the loss function specfied in fun_control and the metric specified in
-fun_control.
-   1. First, the method HyperTorch().fun_torch is called.
-   2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() similar
-      to the "train_hold_out" setting with one exception: It passes an
-      additional test data set to evaluate_hold_out() as follows:
-test_dataset=fun_control["test"]
-evaluate_hold_out() calls create_train_test_data_loaders instead of
-create_train_val_data_loaders as follows: The two data sets are used in
-create_train_test_data_loaders as follows:
-def create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset,
-num_workers=0):
-    trainloader = torch.utils.data.DataLoader(
-        dataset, batch_size=int(batch_size), shuffle=shuffle,
-num_workers=num_workers
-    )
-    testloader = torch.utils.data.DataLoader(
-        test_dataset, batch_size=int(batch_size), shuffle=shuffle,
-num_workers=num_workers
-    )
-    return trainloader, testloader
-   1. The following steps are identical to the "train_hold_out" setting. Only a
-      different data loader is used for testing.
-
-*** Detailed Description of the "train_cv" Setting ***
-It uses the loss function specfied in fun_control and the metric specified in
-fun_control.
-   1. First, the method HyperTorch().fun_torch is called.
-   2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
-df_eval, _ = evaluate_cv(
-    model,
-    dataset=fun_control["train"],
-    shuffle=self.fun_control["shuffle"],
-    device=self.fun_control["device"],
-    show_batch_interval=self.fun_control["show_batch_interval"],
-)
-Note: Only the data set fun_control["train"] is used for CV. 3. In `evaluate_cv
-(), the following steps are performed: The optimizer is set up as follows:
-lr_instance = net.lr
-optimizer = optimizer_handler(optimizer_name=optimizer_instance,
-params=net.parameters(), lr_mult=lr_mult_instance)
-evaluate_cv() sets the net attributes such as epochs, batch_size, optimizer,
-and patience. CV is implemented as follows:
-kfold = KFold(n_splits=k_folds_instance, shuffle=shuffle)
-for fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):
-    train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)
-    val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)
-    trainloader = torch.utils.data.DataLoader(
-        dataset, batch_size=batch_size_instance, sampler=train_subsampler,
-num_workers=num_workers
-    )
-    valloader = torch.utils.data.DataLoader(
-        dataset, batch_size=batch_size_instance, sampler=val_subsampler,
-num_workers=num_workers
-    )
-    reset_weights(net)
-    # Train fold for several epochs:
-    train_fold(
-        net,
-        trainloader,
-        epochs_instance,
-        loss_function,
-        optimizer,
-        device,
-        show_batch_interval=show_batch_interval,
-    )
-    # Validate fold: use only loss for tuning
-    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net,
-valloader, loss_function, device)
-df_eval = sum(loss_values.values()) / len(loss_values.values())
-   1. The method train_fold() is implemented as follows:
-def train_fold(net, trainloader, epochs, loss_function, optimizer, device,
-show_batch_interval=10_000):
-    for epoch in range(epochs):
-        print(f"Epoch: {epoch + 1}")
-        running_loss = 0.0
-        epoch_steps = 0
-        for i, data in enumerate(trainloader, 0):
-            inputs, labels = data
-            inputs, labels = inputs.to(device), labels.to(device)
-            optimizer.zero_grad()
-            outputs = net(inputs)
-            loss = loss_function(outputs, labels)
-            loss.backward()
-            torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
-            optimizer.step()
-            # the following is for printing the statistic only
-            running_loss += loss.item()
-            epoch_steps += 1
-            if i % show_batch_interval == (show_batch_interval - 1):  # print
-every show_batch_interval mini-batches
-                print("Batch: %5d. Training Loss (running): %.3f" % (i + 1,
-running_loss / epoch_steps))
-                running_loss = 0.0
-   1. The method validate_fold_or_hold_out() is implemented as shown above. In
-      contrast to the hold-out setting, it is called for each of the \(k\)
-      folds. The results are stored in a dictionaries metric_values and
-      loss_values as follows:
-    # Validate fold: use only loss for tuning
-    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net,
-valloader, loss_function, device)
-df_eval = sum(loss_values.values()) / len(loss_values.values())
-The results are averaged over the \(k\) folds and returned as df_eval.
-
-*** Detailed Description of the "test_cv" Setting ***
-It uses the loss function specfied in fun_control and the metric specified in
-fun_control.
-   1. First, the method HyperTorch().fun_torch is called.
-   2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
-df_eval, _ = evaluate_cv(
-    model,
-    dataset=fun_control["test"],
-    shuffle=self.fun_control["shuffle"],
-    device=self.fun_control["device"],
-    show_batch_interval=self.fun_control["show_batch_interval"],
-)
-Note: The data set fun_control["test"] is used for CV. The rest is the same as
-for the "train_cv" setting.
+Section 6.2 (in the Appendix) provides more details on the data splitting.
 
 *** Settings for the Final Evaluation of the Tuned Architecture ***
 ** Training of the Tuned Architecture **
 train_tuned(model, train): train the model with the best hyperparameter
 configuration (or simply the default) on the training data set. It splits the
 traindata into new train and validation sets using
 create_train_val_data_loaders(), which calls torch.utils.data.random_split()
 internally. Currently, 60% of the data is used for training and 40% for
 validation. The train data is used for training the model with train_hold_out
 (). The validation data is used for early stopping using
 validate_fold_or_hold_out() on the validation data set.
-train_tuned() is just a wrapper to evaluate_hold_out using the train data set.
-It is implemented as follows:
-def train_tuned(net, train_dataset, shuffle, loss_function, metric,
-device=None, show_batch_interval=10_000, path=None):
-    evaluate_hold_out(
-        net=net,
-        train_dataset=train_dataset,
-        shuffle=shuffle,
-        test_dataset=None,
-        loss_function=loss_function,
-        metric=metric,
-        device=device,
-        show_batch_interval=show_batch_interval,
-        path=path,
-    )
-Note: During training, shuffle is set to True, whereas during testing, shuffle
-is set to False.
 
 ** Testing of the Tuned Architecture **
 test_tuned(model, test): test the model on the test data set. No data splitting
 is performed. The (trained) model is evaluated using the
 validate_fold_or_hold_out() function.
 Note: During training, shuffle is set to True, whereas during testing, shuffle
 is set to False.
-def test_tuned(net, shuffle, test_dataset=None, loss_function=None,
-metric=None, device=None, path=None):
-    batch_size_instance = net.batch_size
-    removed_attributes, net = get_removed_attributes_and_base_net(net)
-    if path is not None:
-        net.load_state_dict(torch.load(path))
-        net.eval()
-    try:
-        device = getDevice(device=device)
-        if torch.cuda.is_available():
-            device = "cuda:0"
-            if torch.cuda.device_count() > 1:
-                print("We will use", torch.cuda.device_count(), "GPUs!")
-                net = nn.DataParallel(net)
-        net.to(device)
-        valloader = torch.utils.data.DataLoader(
-            test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle,
-num_workers=0
-        )
-        metric_value, loss = validate_fold_or_hold_out(
-            net, valloader=valloader, loss_function=loss_function,
-metric=metric, device=device
-        )
-        df_eval = loss
-        df_metric = metric_value
-        df_preds = np.nan
-    except Exception as err:
-        print(f"Error in Net_Core. Call to test_tuned() failed. {err=}, {type
-(err)=}")
-        df_eval = np.nan
-        df_metric = np.nan
-        df_preds = np.nan
-    add_attributes(net, removed_attributes)
-    print(f"Final evaluation: Validation loss: {df_eval}")
-    print(f"Final evaluation: Validation metric: {df_metric}")
-    print("----------------------------------------------")
-    return df_eval, df_preds, df_metric
+Section 6.2.5 describes the final evaluation of the tuned architecture.
 
 **** Loss Functions and Metrics ****
 The key "loss_function" specifies the loss function which is used during the
 optimization. There are several different loss functions under PyTorchâs nn
 package. For example, a simple loss is MSELoss, which computes the mean-squared
 error between the output and the target. In this tutorial we will use
 CrossEntropyLoss, because it is also used in the PyTorch tutorial.
@@ -924,15 +798,16 @@
 of metrics. The key "metric_sklearn" is used for metrics that follow the
 scikit-learn conventions. The key "river_metric" is used for the river based
 evaluation (Montiel_et_al._2021) via eval_oml_iter_progressive, and the key
 "metric_torch" is used for the metrics from TorchMetrics. TorchMetrics is a
 collection of more than 90 PyTorch metrics4. Because the PyTorch tutorial uses
 the accuracy as metric, we use the same metric here. Currently, accuracy is
 computed in the tutorialâs example code. We will use TorchMetrics instead,
-because it offers:
+because it offers more flexibilty, e.g., it can be used for regression and
+classification. Furthermore, TorchMetrics offers the following advantages:
     * A standardized interface to increase reproducibility
     * Reduces Boilerplate
     * Distributed-training compatible
     * Rigorously tested
     * Automatic accumulation over batches
     * Automatic synchronization between multiple devices
 Therefore, we set
@@ -1158,15 +1033,15 @@
   (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))
   (fc1): Linear(in_features=400, out_features=64, bias=True)
   (fc2): Linear(in_features=64, out_features=32, bias=True)
   (fc3): Linear(in_features=32, out_features=10, bias=True)
 )
 
 ***** Get Default Hyperparameters *****
-In a similar manner as in Section 3.11, the default hyperparameters can be
+In a similar manner as in Section 4.11, the default hyperparameters can be
 obtained.
 # fun_control was modified, we generate a new one with the original default
 hyperparameters
 fc = copy.deepcopy(fun_control)
 fc.update({"core_model_hyper_dict": hyper_dict[fun_control
 ["core_model"].__name__]})
 model_default = get_one_core_model_from_X(X_start, fun_control=fc)
@@ -1236,63 +1111,50 @@
 The contour plots in this section visualize the interactions of the three most
 important hyperparameters, l1, l2, and epochs, and optimizer of the surrogate
 model used to optimize the hyperparameters. Since some of these hyperparameters
 take fatorial or integer values, sometimes step-like fitness landcapes (or
 response surfaces) are generated. SPOT draws the interactions of the main
 hyperparameters by default. It is also possible to visualize all interactions.
 For this, again refer to the notebook (Bartz-Beielstein_2023).
-threshold = 0.025
-impo = spot_tuner.print_importance(threshold=threshold, print_screen=True)
-var_plots = [i for i, x in enumerate(impo) if x[1] > threshold]
-min_z = min(spot_tuner.y)
-max_z = max(spot_tuner.y)
-n = spot_tuner.k
-for i in var_plots:
-    for j in var_plots:
-        if j > i:
-            filename = "./figures" + experiment_name+"_contour_"+str(i)+"_"+str
-(j)+".png"
-            spot_tuner.plot_contour(i=i, j=j, min_z=min_z, max_z = max_z,
-filename=filename)
-Figure 4: ?(caption)
+filename = "./figures" + experiment_name
+spot_tuner.plot_important_hyperparameter_contour(filename=filename)
 [./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
 33_contour_0_1.png]
-Figure 5: Contour plot of the loss as a function of l1 and l2, i.e., the number
+Figure 4: Contour plot of the loss as a function of l1 and l2, i.e., the number
 of neurons in the layers.
 [./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
 33_contour_0_3.png]
-Figure 6: Contour plot of the loss as a function of the number of epochs and
+Figure 5: Contour plot of the loss as a function of the number of epochs and
 the neurons in layer l1.
 [./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
 33_contour_0_4.png]
-Figure 7: Contour plot of the loss as a function of the optimizer and the
+Figure 6: Contour plot of the loss as a function of the optimizer and the
 neurons in layer l1.
 [./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
 33_contour_1_3.png]
-Figure 8: Contour plot of the loss as a function of the number of epochs and
+Figure 7: Contour plot of the loss as a function of the number of epochs and
 the neurons in layer l2.
 [./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
 33_contour_1_4.png]
-Figure 9: Contour plot of the loss as a function of the optimizer and the
+Figure 8: Contour plot of the loss as a function of the optimizer and the
 neurons in layer l2.
 [./figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-
 33_contour_3_4.png]
-Figure 10: Contour plot of the loss as a function of the optimizer and the
+Figure 9: Contour plot of the loss as a function of the optimizer and the
 number of epochs.
-Figure 5 to Figure 10 show the contour plots of the loss as a function of the
+Figure 4 to Figure 9 show the contour plots of the loss as a function of the
 hyperparameters. These plots are very helpful for benchmark studies and for
 understanding neural networks. spotPython provides additional tools for a
 visual inspection of the results and give valuable insights into the
 hyperparameter tuning process. This is especially useful for model
 explainability, transparency, and trustworthiness. In addition to the contour
-plots, Figure 12 shows the parallel plot of the hyperparameters.
+plots, Figure 10 shows the parallel plot of the hyperparameters.
 spot_tuner.parallel_plot()
-Figure 11: ?(caption)
 [./figures/parallel.png]
-Figure 12: Parallel plot
+Figure 10: Parallel plot
 
 ****** Summary and Outlook ******
 This tutorial presents the hyperparameter tuning open source software
 spotPython for PyTorch. To show its basic features, a comparison with the
 âofficialâ PyTorch hyperparameter tuning tutorial (PyTorch_2023a) is
 presented. Some of the advantages of spotPython are:
     * Numerical and categorical hyperparameters.
@@ -1349,14 +1211,281 @@
 --------------+
 Best trial config: {'l1': 8, 'l2': 16, 'lr': 0.00276249, 'batch_size': 16,
 'data_dir': '...'}
 Best trial final validation loss: 1.181501
 Best trial final validation accuracy: 0.5836
 Best trial test set accuracy: 0.5806
 
+***** Detailed Description of the Data Splitting *****
+**** Description of the "train_hold_out" Setting ****
+The "train_hold_out" setting is used by default. It uses the loss function
+specfied in fun_control and the metric specified in fun_control.
+   1. First, the method HyperTorch().fun_torch is called.
+   2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() as
+      follows:
+df_eval, _ = evaluate_hold_out(
+    model,
+    train_dataset=fun_control["train"],
+    shuffle=self.fun_control["shuffle"],
+    loss_function=self.fun_control["loss_function"],
+    metric=self.fun_control["metric_torch"],
+    device=self.fun_control["device"],
+    show_batch_interval=self.fun_control["show_batch_interval"],
+    path=self.fun_control["path"],
+)
+Note: Only the data set fun_control["train"] is used for training and
+validation. It is used as follows:
+trainloader, valloader = create_train_val_data_loaders(
+                dataset=train_dataset, batch_size=batch_size_instance,
+shuffle=shuffle
+            )
+create_train_val_data_loaders() splits the train_dataset into trainloader and
+valloader using torch.utils.data.random_split() as follows:
+def create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):
+    test_abs = int(len(dataset) * 0.6)
+    train_subset, val_subset = random_split(dataset, [test_abs, len(dataset) -
+test_abs])
+    trainloader = torch.utils.data.DataLoader(
+        train_subset, batch_size=int(batch_size), shuffle=shuffle,
+num_workers=num_workers
+    )
+    valloader = torch.utils.data.DataLoader(
+        val_subset, batch_size=int(batch_size), shuffle=shuffle,
+num_workers=num_workers
+    )
+    return trainloader, valloader
+The optimizer is set up as follows:
+lr_mult_instance = net.lr_mult
+optimizer = optimizer_handler(optimizer_name=optimizer_instance,
+params=net.parameters(), lr_mult=lr_mult_instance)
+   1. evaluate_hold_out() sets the net attributes such as epochs, batch_size,
+      optimizer, and patience. For each epoch, the methods train_hold_out() and
+      validate_fold_or_hold_out() are called, the former for training and the
+      latter for validation and early stopping. The validation loss from the
+      last epoch (not the best validation loss) is returned from
+      evaluate_hold_out.
+   2. The method train_hold_out() is implemented as follows:
+def train_hold_out(net, trainloader, batch_size, loss_function, optimizer,
+device, show_batch_interval=10_000):
+    running_loss = 0.0
+    epoch_steps = 0
+    for i, data in enumerate(trainloader, 0):
+        inputs, labels = data
+        inputs, labels = inputs.to(device), labels.to(device)
+        optimizer.zero_grad()
+        outputs = net(inputs)
+        loss = loss_function(outputs, labels)
+        loss.backward()
+        torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
+        optimizer.step()
+        running_loss += loss.item()
+        epoch_steps += 1
+        if i % show_batch_interval == (show_batch_interval - 1):  # print every
+show_batch_interval mini-batches
+            print(
+                "Batch: %5d. Batch Size: %d. Training Loss (running): %.3f"
+                % (i + 1, int(batch_size), running_loss / epoch_steps)
+            )
+            running_loss = 0.0
+    return loss.item()
+   1. The method validate_fold_or_hold_out() is implemented as follows:
+def validate_fold_or_hold_out(net, valloader, loss_function, metric, device):
+    val_loss = 0.0
+    val_steps = 0
+    metric.reset()
+    for i, data in enumerate(valloader, 0):
+        with torch.no_grad():
+            inputs, labels = data
+            inputs, labels = inputs.to(device), labels.to(device)
+            outputs = net(inputs)
+            _, predicted = torch.max(outputs.data, 1)
+            metric_value = metric(predicted, labels).to(device)
+            loss = loss_function(outputs, labels)
+            val_loss += loss.cpu().numpy()
+            val_steps += 1
+    loss = val_loss / val_steps
+    metric_value = metric.compute()
+    return metric_value, loss
+
+**** Description of the "test_hold_out" Setting ****
+It uses the loss function specfied in fun_control and the metric specified in
+fun_control.
+   1. First, the method HyperTorch().fun_torch is called.
+   2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() similar
+      to the "train_hold_out" setting with one exception: It passes an
+      additional test data set to evaluate_hold_out() as follows:
+test_dataset=fun_control["test"]
+evaluate_hold_out() calls create_train_test_data_loaders instead of
+create_train_val_data_loaders as follows: The two data sets are used in
+create_train_test_data_loaders as follows:
+def create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset,
+num_workers=0):
+    trainloader = torch.utils.data.DataLoader(
+        dataset, batch_size=int(batch_size), shuffle=shuffle,
+num_workers=num_workers
+    )
+    testloader = torch.utils.data.DataLoader(
+        test_dataset, batch_size=int(batch_size), shuffle=shuffle,
+num_workers=num_workers
+    )
+    return trainloader, testloader
+   1. The following steps are identical to the "train_hold_out" setting. Only a
+      different data loader is used for testing.
+
+**** Detailed Description of the "train_cv" Setting ****
+It uses the loss function specfied in fun_control and the metric specified in
+fun_control.
+   1. First, the method HyperTorch().fun_torch is called.
+   2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
+df_eval, _ = evaluate_cv(
+    model,
+    dataset=fun_control["train"],
+    shuffle=self.fun_control["shuffle"],
+    device=self.fun_control["device"],
+    show_batch_interval=self.fun_control["show_batch_interval"],
+)
+Note: Only the data set fun_control["train"] is used for CV. 3. In `evaluate_cv
+(), the following steps are performed: The optimizer is set up as follows:
+lr_instance = net.lr
+optimizer = optimizer_handler(optimizer_name=optimizer_instance,
+params=net.parameters(), lr_mult=lr_mult_instance)
+evaluate_cv() sets the net attributes such as epochs, batch_size, optimizer,
+and patience. CV is implemented as follows:
+kfold = KFold(n_splits=k_folds_instance, shuffle=shuffle)
+for fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):
+    train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)
+    val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)
+    trainloader = torch.utils.data.DataLoader(
+        dataset, batch_size=batch_size_instance, sampler=train_subsampler,
+num_workers=num_workers
+    )
+    valloader = torch.utils.data.DataLoader(
+        dataset, batch_size=batch_size_instance, sampler=val_subsampler,
+num_workers=num_workers
+    )
+    reset_weights(net)
+    # Train fold for several epochs:
+    train_fold(
+        net,
+        trainloader,
+        epochs_instance,
+        loss_function,
+        optimizer,
+        device,
+        show_batch_interval=show_batch_interval,
+    )
+    # Validate fold: use only loss for tuning
+    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net,
+valloader, loss_function, device)
+df_eval = sum(loss_values.values()) / len(loss_values.values())
+   1. The method train_fold() is implemented as follows:
+def train_fold(net, trainloader, epochs, loss_function, optimizer, device,
+show_batch_interval=10_000):
+    for epoch in range(epochs):
+        print(f"Epoch: {epoch + 1}")
+        running_loss = 0.0
+        epoch_steps = 0
+        for i, data in enumerate(trainloader, 0):
+            inputs, labels = data
+            inputs, labels = inputs.to(device), labels.to(device)
+            optimizer.zero_grad()
+            outputs = net(inputs)
+            loss = loss_function(outputs, labels)
+            loss.backward()
+            torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
+            optimizer.step()
+            # the following is for printing the statistic only
+            running_loss += loss.item()
+            epoch_steps += 1
+            if i % show_batch_interval == (show_batch_interval - 1):  # print
+every show_batch_interval mini-batches
+                print("Batch: %5d. Training Loss (running): %.3f" % (i + 1,
+running_loss / epoch_steps))
+                running_loss = 0.0
+   1. The method validate_fold_or_hold_out() is implemented as shown above. In
+      contrast to the hold-out setting, it is called for each of the \(k\)
+      folds. The results are stored in a dictionaries metric_values and
+      loss_values as follows:
+# Validate fold: use only loss for tuning
+    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net,
+valloader, loss_function, device)
+df_eval = sum(loss_values.values()) / len(loss_values.values())
+The results are averaged over the \(k\) folds and returned as df_eval.
+
+**** Detailed Description of the "test_cv" Setting ****
+It uses the loss function specfied in fun_control and the metric specified in
+fun_control.
+   1. First, the method HyperTorch().fun_torch is called.
+   2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
+df_eval, _ = evaluate_cv(
+    model,
+    dataset=fun_control["test"],
+    shuffle=self.fun_control["shuffle"],
+    device=self.fun_control["device"],
+    show_batch_interval=self.fun_control["show_batch_interval"],
+)
+Note: The data set fun_control["test"] is used for CV. The rest is the same as
+for the "train_cv" setting.
+
+**** Detailed Description of the Final Model Training and Evaluation ****
+*** Detailed Description of the "train_tuned Procedure ***
+train_tuned() is just a wrapper to evaluate_hold_out using the train data set.
+It is implemented as follows:
+def train_tuned(net, train_dataset, shuffle, loss_function, metric,
+device=None, show_batch_interval=10_000, path=None):
+    evaluate_hold_out(
+        net=net,
+        train_dataset=train_dataset,
+        shuffle=shuffle,
+        test_dataset=None,
+        loss_function=loss_function,
+        metric=metric,
+        device=device,
+        show_batch_interval=show_batch_interval,
+        path=path,
+    )
+The test_tuned() procedure is implemented as follows:
+def test_tuned(net, shuffle, test_dataset=None, loss_function=None,
+metric=None, device=None, path=None):
+    batch_size_instance = net.batch_size
+    removed_attributes, net = get_removed_attributes_and_base_net(net)
+    if path is not None:
+        net.load_state_dict(torch.load(path))
+        net.eval()
+    try:
+        device = getDevice(device=device)
+        if torch.cuda.is_available():
+            device = "cuda:0"
+            if torch.cuda.device_count() > 1:
+                print("We will use", torch.cuda.device_count(), "GPUs!")
+                net = nn.DataParallel(net)
+        net.to(device)
+        valloader = torch.utils.data.DataLoader(
+            test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle,
+num_workers=0
+        )
+        metric_value, loss = validate_fold_or_hold_out(
+            net, valloader=valloader, loss_function=loss_function,
+metric=metric, device=device
+        )
+        df_eval = loss
+        df_metric = metric_value
+        df_preds = np.nan
+    except Exception as err:
+        print(f"Error in Net_Core. Call to test_tuned() failed. {err=}, {type
+(err)=}")
+        df_eval = np.nan
+        df_metric = np.nan
+        df_preds = np.nan
+    add_attributes(net, removed_attributes)
+    print(f"Final evaluation: Validation loss: {df_eval}")
+    print(f"Final evaluation: Validation metric: {df_metric}")
+    print("----------------------------------------------")
+    return df_eval, df_preds, df_metric
+
 ****** References ******
 Bartz, Eva, Thomas Bartz-Beielstein, Martin Zaefferer, and Olaf Mersmann, eds.
 2022. Hyperparameter Tuning for Machine and Deep Learning with R - A Practical
 Guide. Springer.
 Bartz-Beielstein, Thomas. 2023. âPyTorch Hyperparameter Tuning with SPOT:
 Comparison with Ray Tuner and Default Hyperparameters on CIFAR10.â https://
 github.com/sequential-parameter-optimization/spotPython/blob/main/notebooks/
```

### Comparing `spotPython-0.2.1/docs/bart23e.pdf` & `spotPython-0.2.2/docs/bart23e.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,10 +1,10 @@
 PyTorch Hyperparameter Tuning — A Tutorial
 for spotPython
-Version 0.2.0
+Version 0.2.1
 
 Thomas Bartz-Beielstein
 bartzbeielstein@gmail.com
 https://orcid.org/0000-0002-5938-5158
 May, 27th 2023
 
 1 Hyperparameter Tuning
@@ -36,17 +36,18 @@
 the interactions between multiple hyperparameters plays a major role in the interpretability
 and explainability of machine learning models. SPOT provides statistical tools for understanding hyperparameters and their interactions. Last but not least, it should be noted that the
 SPOT software code is available in the open source spotPython package on github1 , allowing
 replicability of the results. This tutorial descries the Python variant of SPOT, which is called
 spotPython. The R implementation is described in Bartz et al. (2022). SPOT is an established open source software that has been maintained for more than 15 years (Bartz-Beielstein,
 Lasarczyk, and Preuss 2005) (Bartz et al. 2022).
 This tutorial is structured as follows. The concept of the hyperparameter tuning software
-spotPython is described in Section 2. Section 3 describes the integration of spotPython into
-the PyTorch training workflow and presents the results. Finally, Section 4 presents a summary
-and an outlook.
+spotPython is described in Section 2. Section 3 (“Quickstart”) describes the execution of
+the example from the tutorial “Hyperparameter Tuning with Ray Tune” (PyTorch 2023a).
+Section 4 describes the integration of spotPython into the PyTorch training workflow in detail
+and presents the results. Finally, Section 5 presents a summary and an outlook.
 Ĺ Note
 The corresponding .ipynb notebook (Bartz-Beielstein 2023) is updated regularly and
 reflects updates and changes in the spotPython package. It can be downloaded from
 https://github.com/sequential-parameter-optimization/spotPython/blob/main/notebo
 oks/14_spot_ray_hpt_torch_cifar10.ipynb.
 
 2 The Hyperparameter Tuning Software SPOT
@@ -64,130 +65,254 @@
 https://github.com/sequential-parameter-optimization
 
 2
 
 optimizer and for automatic and interactive tuning. Details on SPOT and its use in practice
 are given by Bartz et al. (2022).
 A typical hyperparameter tuning process with spotPython consists of the following steps:
-1. Loading the data (training and test datasets), see Section 3.3.
-2. Specification of the preprocessing model, see Section 3.4. This model is called
+1. Loading the data (training and test datasets), see Section 4.3.
+2. Specification of the preprocessing model, see Section 4.4. This model is called
 prep_model (“preparation” or pre-processing). The information required for the
 hyperparameter tuning is stored in the dictionary fun_control. Thus, the information
 needed for the execution of the hyperparameter tuning is available in a readable form.
-3. Selection of the machine learning or deep learning model to be tuned, see Section 3.5.
+3. Selection of the machine learning or deep learning model to be tuned, see Section 4.5.
 This is called the core_model. Once the core_model is defined, then the associated
 hyperparameters are stored in the fun_control dictionary. First, the hyperparameters
 of the core_model are initialized with the default values of the core_model. As default
 values we use the default values contained in the spotPython package for the algorithms
 of the torch package.
 4. Modification of the default values for the hyperparameters used in core_model, see
-Section 3.7.1. This step is optional.
+Section 4.7.1. This step is optional.
 1. numeric parameters are modified by changing the bounds.
 2. categorical parameters are modified by changing the categories (“levels”).
-5. Selection of target function (loss function) for the optimizer, see Section 3.8.
-6. Calling SPOT with the corresponding parameters, see Section 3.9. The results are stored
+5. Selection of target function (loss function) for the optimizer, see Section 4.8.
+6. Calling SPOT with the corresponding parameters, see Section 4.9. The results are stored
 in a dictionary and are available for further analysis.
-7. Presentation, visualization and interpretation of the results, see Section 3.10.
+7. Presentation, visualization and interpretation of the results, see Section 4.10.
 
-3 Hyperparameter Tuning for PyTorch With spotPython
+3 Quickstart
+import numpy as np
+from math import inf
+import torchmetrics
+from torch.nn import CrossEntropyLoss
+from spotPython.spot import spot
+from spotPython.utils.init import fun_control_init
+from spotPython.data.torchdata import load_data_cifar10
+from spotPython.hyperparameters.values import (
+add_core_model_to_fun_control,
+modify_hyper_parameter_levels,
+modify_hyper_parameter_bounds,
+get_var_type,
+get_var_name,
+
+3
+
+get_bound_values,
+get_one_core_model_from_X,
+get_default_hyperparameters_as_array
+)
+from spotPython.data.torch_hyper_dict import TorchHyperDict
+from spotPython.data.torchdata import load_data_cifar10
+from spotPython.fun.hypertorch import HyperTorch
+from spotPython.torch.netcifar10 import Net_CIFAR10
+from spotPython.torch.traintest import (
+train_tuned,
+test_tuned,
+)
+fun_control = fun_control_init()
+# load data
+train, test = load_data_cifar10()
+# add the dataset to the fun_control
+fun_control.update({
+"train": train,
+"test": test,
+"n_samples": len(train)})
+# add the nn model to the fun_control dictionary
+fun_control = add_core_model_to_fun_control(core_model=Net_CIFAR10,
+fun_control=fun_control,
+hyper_dict=TorchHyperDict)
+# modify the hyperparameter levels
+fun_control = modify_hyper_parameter_bounds(fun_control, "lr_mult", bounds=[1e-3, 1e-3])
+fun_control = modify_hyper_parameter_bounds(fun_control, "sgd_momentum", bounds=[0.9, 0.9])
+fun_control = modify_hyper_parameter_levels(fun_control, "optimizer",["Adam", "SGD"])
+# select metric and loss function
+fun_control.update({
+"metric_torch": torchmetrics.Accuracy(task="multiclass", num_classes=10),
+"loss_function": CrossEntropyLoss(),
+"device": "cpu",
+})
+# extract the variable types, names, and bounds
+var_type = get_var_type(fun_control)
+var_name = get_var_name(fun_control)
+fun_control.update({"var_type": var_type,
+"var_name": var_name})
+lower = get_bound_values(fun_control, "lower")
+upper = get_bound_values(fun_control, "upper")
+
+4
+
+# get the default hyperparameters as array
+hyper_dict=TorchHyperDict().load()
+X_start = get_default_hyperparameters_as_array(fun_control, hyper_dict)
+# get the objective function
+fun = HyperTorch().fun_torch
+# initialize spot
+spot_tuner = spot.Spot(fun=fun,
+lower = lower,
+upper = upper,
+fun_evals = inf,
+fun_repeats = 1,
+max_time = 30,
+noise = False,
+tolerance_x = np.sqrt(np.spacing(1)),
+var_type = var_type,
+var_name = var_name,
+infill_criterion = "y",
+n_points = 1,
+seed=123,
+log_level = 50,
+show_models= False,
+show_progress= True,
+fun_control = fun_control,
+design_control={"init_size": 10,
+"repeats": 1},
+surrogate_control={"noise": True,
+"cod_type": "norm",
+"min_theta": -4,
+"max_theta": 3,
+"n_theta": len(var_name),
+"model_fun_evals": 10_000,
+"log_level": 50
+})
+# run spot
+spot_tuner.run(X_start=X_start)
+spot_tuner.plot_progress()
+
+5
+
+from spotPython.utils.eda import gen_design_table
+print(gen_design_table(fun_control=fun_control, spot=spot_tuner))
+spot_tuner.plot_importance()
+X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1,-1))
+model_spot = get_one_core_model_from_X(X, fun_control)
+model_spot
+train_tuned(net=model_spot, train_dataset=train,
+loss_function=fun_control["loss_function"],
+metric=fun_control["metric_torch"],
+shuffle=True,
+device = "cpu",
+path=None)
+test_tuned(net=model_spot, test_dataset=test,
+shuffle=False,
+loss_function=fun_control["loss_function"],
+metric=fun_control["metric_torch"],
+device = "cpu")
+spot_tuner.plot_important_hyperparameter_contour()
+
+4 Hyperparameter Tuning for PyTorch With spotPython
 In this tutorial, we will show how spotPython can be integrated into the PyTorch training
 workflow. It is based on the tutorial “Hyperparameter Tuning with Ray Tune” from the
 PyTorch documentation (PyTorch 2023a), which is an extension of the tutorial “Training a
 Classifier” (PyTorch 2023b) for training a CIFAR10 image classifier.
 This document refers to the following software versions:
 • python: 3.10.10
 • torch: 2.0.1
 • torchvision: 0.15.0
-• spotPython: 0.2.0
+• spotPython: 0.2.1
 spotPython can be installed via pip2 .
 2
 
 Alternatively, the source code can be downloaded from gitHub: https://github.com/sequential-parameteroptimization/spotPython.
 
-3
+6
 
 !pip install spotPython
 Results that refer to the Ray Tune package are taken from https://PyTorch.org/tutorials/be
 ginner/hyperparameter_tuning_tutorial.html3 .
 
-3.1 Setup
+4.1 Setup
 Before we consider the detailed experimental setup, we select the parameters that affect run
 time, initial design size and the device that is used.
 MAX_TIME = 60
 INIT_SIZE = 20
 DEVICE = "cpu" # "cuda:0"
 
-3.2 Initialization of the fun_control Dictionary
+4.2 Initialization of the fun_control Dictionary
 spotPython uses a Python dictionary for storing the information required for the hyperparameter tuning process. This dictionary is called fun_control and is initialized with the function
 fun_control_init. The function fun_control_init returns a skeleton dictionary. The dictionary is filled with the required information for the hyperparameter tuning process. It stores
 the hyperparameter tuning settings, e.g., the deep learning network architecture that should
 be tuned, the classification (or regression) problem, and the data that is used for the tuning.
 The dictionary is used as an input for the SPOT function.
 fun_control = fun_control_init()
 
-3.3 Data Loading
-The data loading process is implemented in the same manner as described in the Section “Data
-loaders” in PyTorch (2023a). The data loaders are wrapped into the function load_data. A
-global data directory is used, which allows sharing the data directory between different trials.
-def load_data(data_dir="./data"):
-transform = transforms.Compose([
-transforms.ToTensor(),
-transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))
-])
+4.3 Data Loading
+The data loading process is implemented in the same manner as described in the Section
+“Data loaders” in PyTorch (2023a). The data loaders are wrapped into the function
+load_data_cifar10 which is identical to the function load_data in PyTorch (2023a). A
+global data directory is used, which allows sharing the data directory between different
+trials.
+
 3
 
 We were not able to install Ray Tune on our system. Therefore, we used the results from the PyTorch tutorial.
 
-4
+7
 
-trainset = torchvision.datasets.CIFAR10(
+def load_data_cifar10(data_dir="./data"):
+transform = transforms.Compose([
+transforms.ToTensor(),
+transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))
+])
+trainset = torchvision.datasets.CIFAR10(
 root=data_dir, train=True, download=True, transform=transform)
 testset = torchvision.datasets.CIFAR10(
 root=data_dir, train=False, download=True, transform=transform)
 return trainset, testset
-The test and train data are added to the dictionary fun_control.
-train, test = load_data()
+The method load_data_cifar10 is part of the spotPython package and can be imported from
+spotPython.data.torchdata.
+In the following step, the test and train data are added to the dictionary fun_control.
+train, test = load_data_cifar10()
 n_samples = len(train)
 # add the dataset to the fun_control
 fun_control.update({
 "train": train,
 "test": test,
 "n_samples": n_samples})
 
-3.4 Specification of the Preprocessing Model
+4.4 Specification of the Preprocessing Model
 After the training and test data are specified and added to the fun_control dictionary,
 spotPython allows the specification of a data preprocessing pipeline, e.g., for the scaling
 of the data or for the one-hot encoding of categorical variables. The preprocessing model is
 called prep_model (“preparation” or pre-processing) and includes steps that are not subject to
 the hyperparameter tuning process. The preprocessing model is specified in the fun_control
 dictionary. The preprocessing model can be implemented as a sklearn pipeline. The following
 code shows a typical preprocessing pipeline:
 categorical_columns = ["cities", "colors"]
 one_hot_encoder = OneHotEncoder(handle_unknown="ignore",
 sparse_output=False)
 prep_model = ColumnTransformer(
-transformers=[
+
+8
+
+transformers=[
 ("categorical", one_hot_encoder, categorical_columns),
 ],
 remainder=StandardScaler(),
 )
 Because the Ray Tune (ray[tune]) hyperparameter tuning as described in PyTorch (2023a)
 does not use a preprocessing model, the preprocessing model is set to None here.
-
-5
-
-prep_model = None
+prep_model = None
 fun_control.update({"prep_model": prep_model})
 
-3.5 Select algorithm and core_model_hyper_dict
+4.5 Select algorithm and core_model_hyper_dict
 The same neural network model as implemented in the section “Configurable neural network”
 of the PyTorch tutorial (PyTorch 2023a) is used here. We will show the implementation from
-PyTorch (2023a) in Section 3.5.1 first, before the extended implementation with spotPython
-is shown in Section 3.5.2.
-3.5.1 Implementing a Configurable Neural Network With Ray Tune
+PyTorch (2023a) in Section 4.5.1 first, before the extended implementation with spotPython
+is shown in Section 4.5.2.
+4.5.1 Implementing a Configurable Neural Network With Ray Tune
 We used the same hyperparameters that are implemented as configurable in the PyTorch
 tutorial. We specify the layer sizes, namely l1 and l2, of the fully connected layers:
 class Net(nn.Module):
 def __init__(self, l1=120, l2=84):
 super(Net, self).__init__()
 self.conv1 = nn.Conv2d(3, 6, 5)
 self.pool = nn.MaxPool2d(2, 2)
@@ -197,132 +322,143 @@
 self.fc3 = nn.Linear(l2, 10)
 def forward(self, x):
 x = self.pool(F.relu(self.conv1(x)))
 x = self.pool(F.relu(self.conv2(x)))
 x = x.view(-1, 16 * 5 * 5)
 x = F.relu(self.fc1(x))
 x = F.relu(self.fc2(x))
-x = self.fc3(x)
+
+9
+
+x = self.fc3(x)
 return x
 The learning rate, i.e., lr, of the optimizer is made configurable, too:
 optimizer = optim.SGD(net.parameters(), lr=config["lr"], momentum=0.9)
 
-6
-
-3.5.2 Implementing a Configurable Neural Network With spotPython
+4.5.2 Implementing a Configurable Neural Network With spotPython
 spotPython implements a class which is similar to the class described in the PyTorch tutorial.
 The class is called Net_CIFAR10 and is implemented in the file netcifar10.py.
+from torch import nn
+import torch.nn.functional as F
 import spotPython.torch.netcore as netcore
+
 class Net_CIFAR10(netcore.Net_Core):
-def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience):
+def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd
 super(Net_CIFAR10, self).__init__(
-lr_mult=lr_mult, batch_size=batch_size, epochs=epochs, k_folds=k_folds,
-patience=patience
+lr_mult=lr_mult,
+batch_size=batch_size,
+epochs=epochs,
+k_folds=k_folds,
+patience=patience,
+optimizer=optimizer,
+sgd_momentum=sgd_momentum,
 )
 self.conv1 = nn.Conv2d(3, 6, 5)
 self.pool = nn.MaxPool2d(2, 2)
 self.conv2 = nn.Conv2d(6, 16, 5)
 self.fc1 = nn.Linear(16 * 5 * 5, l1)
 self.fc2 = nn.Linear(l1, l2)
 self.fc3 = nn.Linear(l2, 10)
 def forward(self, x):
 x = self.pool(F.relu(self.conv1(x)))
 x = self.pool(F.relu(self.conv2(x)))
 x = x.view(-1, 16 * 5 * 5)
 x = F.relu(self.fc1(x))
 x = F.relu(self.fc2(x))
-x = self.fc3(x)
+
+10
+
+x = self.fc3(x)
 return x
 Net_CIFAR10 inherits from the class Net_Core which is implemented in the file netcore.py.
 It implements the additional attributes that are common to all neural network models. The
 attributes are the learning rate multiplier lr_mult, the batch size batch_size, the number
 of epochs epochs, the number of folds k_folds for the cross validation, and the patience
 patience for the early stopping. The class Net_Core is shown below.
 from torch import nn
 
 class Net_Core(nn.Module):
-def __init__(self, lr_mult, batch_size, epochs, k_folds, patience):
+def __init__(self, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd_momentu
 super(Net_Core, self).__init__()
 self.lr_mult = lr_mult
 self.batch_size = batch_size
-
-7
-
-self.epochs = epochs
+self.epochs = epochs
 self.k_folds = k_folds
 self.patience = patience
+self.optimizer = optimizer
+self.sgd_momentum = sgd_momentum
+Ĺ The Net_Core class
+The Net_Core class is implemented in the file netcore.py. It implements hyperparameters as attributes, that are not used by the core_model, e.g.:
+• optimizer (optimizer),
+• learning rate (lr),
+• batch size (batch_size),
+• epochs (epochs),
+• k_folds (k_folds), and
+• early stopping criterion “patience” (patience).
+Users can add further attributes to the class.
 
-3.5.3 Comparison of the Approach Described in the PyTorch Tutorial With spotPython
+4.5.3 Comparison of the Approach Described in the PyTorch Tutorial With spotPython
 Comparing the class Net from the PyTorch tutorial and the class Net_CIFAR10 from
 spotPython, we see that the class Net_CIFAR10 has additional attributes and does not
-inherit from nn directly. It adds an additional class, Net_core, that takes care of additional
+
+11
+
+inherit from nn directly. It adds an additional class, Net_core, that takes care of additional
 attributes that are common to all neural network models, e.g., the learning rate multiplier
 lr_mult or the batch size batch_size.
 spotPython’s core_model implements an instance of the Net_CIFAR10 class. In addition to the
 basic neural network model, the core_model can use these additional attributes. spotPython
 provides methods for handling these additional attributes to guarantee 100% compatibility
 with the PyTorch classes. The method add_core_model_to_fun_control adds the hyperparameters and additional attributes to the fun_control dictionary. The method is shown
 below.
 core_model = Net_CIFAR10
 fun_control = add_core_model_to_fun_control(core_model=core_model,
 fun_control=fun_control,
 hyper_dict=TorchHyperDict,
 filename=None)
-Ĺ Note
-In addition to the class Net from the PyTorch tutorial, the class Net_CIFAR10 has
-additional attributes, e.g.:
-• learning rate (lr),
-• batch size (batch_size),
-• epochs (epochs),
-• k_folds (k_folds), and
-• early stopping criterion “patience” (patience)
-Further attributes can be easily added to the class, e.g., optimizer.
 
-8
-
-3.6 The Search Space
-In Section 3.6.1, we first describe how to configure the search space with ray[tune] (as
+4.6 The Search Space
+In Section 4.6.1, we first describe how to configure the search space with ray[tune] (as
 shown in PyTorch (2023a)) and then how to configure the search space with spotPython in
-Section 3.6.2.
-3.6.1 Configuring the Search Space With Ray Tune
+Section 4.6.2.
+4.6.1 Configuring the Search Space With Ray Tune
 Ray Tune’s search space can be configured as follows (PyTorch 2023a):
 config = {
 "l1": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),
 "l2": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),
 "lr": tune.loguniform(1e-4, 1e-1),
 "batch_size": tune.choice([2, 4, 8, 16])
 }
 The tune.sample_from() function enables the user to define sample methods to obtain hyperparameters. In this example, the l1 and l2 parameters should be powers of 2 between 4
 and 256, so either 4, 8, 16, 32, 64, 128, or 256. The lr (learning rate) should be uniformly
 sampled between 0.0001 and 0.1. Lastly, the batch size is a choice between 2, 4, 8, and 16.
 At each trial, ray[tune] will randomly sample a combination of parameters from these search
 spaces. It will then train a number of models in parallel and find the best performing one
 among these. ray[tune] uses the ASHAScheduler which will terminate bad performing trials
 early.
-3.6.2 Configuring the Search Space With spotPython
-3.6.2.1 The hyper_dict Hyperparameters for the Selected Algorithm
-spotPython uses simple JSON files for the specification of the hyperparameters. Users can
-specify their individual JSON files, or they can use the JSON files provided by spotPython. The
-JSON file for the core_model is called torch_hyper_dict.json.
-In contrast to ray[tune], spotPython can handle numerical, boolean, and categorical hyperparameters. They can be specified in the JSON file in a similar way as the numerical
-hyperparameters as shown below:
 
-9
+12
 
-"factor_hyperparameter": {
+4.6.2 Configuring the Search Space With spotPython
+4.6.2.1 The hyper_dict Hyperparameters for the Selected Algorithm
+spotPython uses JSON files for the specification of the hyperparameters. Users can specify
+their individual JSON files, or they can use the JSON files provided by spotPython. The JSON
+file for the core_model is called torch_hyper_dict.json.
+In contrast to ray[tune], spotPython can handle numerical, boolean, and categorical hyperparameters. They can be specified in the JSON file in a similar way as the numerical
+hyperparameters as shown below. Each entry in the JSON file represents one hyperparameter
+with the following structure: type, default, transform, lower, and upper.
+"factor_hyperparameter": {
 "levels": ["A", "B", "C"],
 "type": "factor",
 "default": "B",
 "transform": "None",
 "core_model_parameter_type": "str",
 "lower": 0,
 "upper": 2},
-Each entry in the JSON file represents one hyperparameter with the following structure: type,
-default, transform, lower, and upper. The corresponding entries for the Net_CIFAR10 class
-are shown below.
+The corresponding entries for the Net_CIFAR10 class are shown below.
 {"Net_CIFAR10":
 {
 "l1": {
 "type": "int",
 "default": 5,
 "transform": "transform_power_2_int",
 "lower": 2,
@@ -334,28 +470,28 @@
 "lower": 2,
 "upper": 9},
 "lr_mult": {
 "type": "float",
 "default": 1.0,
 "transform": "None",
 "lower": 0.1,
-"upper": 10},
+
+13
+
+"upper": 10},
 "batch_size": {
 "type": "int",
 "default": 4,
 "transform": "transform_power_2_int",
 "lower": 1,
 "upper": 4},
 "epochs": {
 "type": "int",
 "default": 3,
-
-10
-
-"transform": "transform_power_2_int",
+"transform": "transform_power_2_int",
 "lower": 1,
 "upper": 4},
 "k_folds": {
 "type": "int",
 "default": 2,
 "transform": "None",
 "lower": 2,
@@ -379,146 +515,149 @@
 "RAdam",
 "RMSprop",
 "Rprop",
 "SGD"],
 "type": "factor",
 "default": "SGD",
 "transform": "None",
-"class_name": "torch.optim",
+
+14
+
+"class_name": "torch.optim",
 "core_model_parameter_type": "str",
 "lower": 0,
 "upper": 12},
 "sgd_momentum": {
 "type": "float",
 "default": 0.0,
 "transform": "None",
 "lower": 0.0,
 "upper": 1.0}
-
-11
-
-}
+}
 }
 
-3.7 Modifying the Hyperparameters
+4.7 Modifying the Hyperparameters
 Ray tune (PyTorch 2023a) does not provide a way to change the specified hyperparameters
 without re-compilation. However, spotPython provides functions for modifying the hyperparameters, their bounds and factors as well as for activating and de-activating hyperparameters
 without re-compilation of the Python source code. These functions are described in the following.
-3.7.1 Modify hyper_dict Hyperparameters for the Selected Algorithm aka core_model
+4.7.1 Modify hyper_dict Hyperparameters for the Selected Algorithm aka core_model
 After specifying the model, the corresponding hyperparameters, their types and bounds are
 loaded from the JSON file torch_hyper_dict.json. After loading, the user can modify the
 hyperparameters, e.g., the bounds. spotPython provides a simple rule for de-activating hyperparameters: If the lower and the upper bound are set to identical values, the hyperparameter
 is de-activated. This is useful for the hyperparameter tuning, because it allows to specify a
 hyperparameter in the JSON file, but to de-activate it in the fun_control dictionary. This is
 done in the next step.
-3.7.2 Modify Hyperparameters of Type numeric and integer (boolean)
+4.7.2 Modify Hyperparameters of Type numeric and integer (boolean)
 Since the hyperparameter k_folds is not used in the PyTorch tutorial, it is de-activated here
 by setting the lower and upper bound to the same value. Note, k_folds is of type “integer”.
 fun_control = modify_hyper_parameter_bounds(fun_control, "batch_size", bounds=[1, 5])
 fun_control = modify_hyper_parameter_bounds(fun_control, "k_folds", bounds=[0, 0])
 fun_control = modify_hyper_parameter_bounds(fun_control, "patience", bounds=[3, 3])
 fun_control["core_model_hyper_dict"]
 
-3.7.3 Modify Hyperparameter of Type factor
+15
+
+4.7.3 Modify Hyperparameter of Type factor
 In a similar manner as for the numerical hyperparameters, the categorical hyperparameters
 can be modified. New configurations can be chosen by adding or deleting levels. For example,
 the hyperparameter optimizer can be re-configured as follows:
 In the following setting, two optimizers ("SGD" and "Adam") will be compared during the
 spotPython hyperparameter tuning. The hyperparameter optimizer is active.
-
-12
-
-fun_control = modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD", "Adam"])
+fun_control = modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD", "Adam"])
 The hyperparameter optimizer can be de-activated by choosing only one value (level), here:
 "SGD".
 fun_control = modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD"])
-As discussed in Section 3.7.4, there are some issues with the LBFGS optimizer. Therefore,
+As discussed in Section 4.7.4, there are some issues with the LBFGS optimizer. Therefore,
 the usage of the LBFGS optimizer is not deactivated in spotPython by default. However, the
 LBFGS optimizer can be activated by adding it to the list of optimizers. Rprop was removed,
 because it does perform very poorly (as some pre-tests have shown). However, it can also be
 activated by adding it to the list of optimizers. Since SparseAdam does not support dense
 gradients, Adam was used instead. Therefore, there are 10 default optimizers:
 fun_control = modify_hyper_parameter_levels(fun_control, "optimizer",["Adadelta",
 "Adagrad", "Adam", "AdamW", "Adamax", "ASGD", "NAdam", "RAdam",
 "RMSprop", "SGD"])
 
-3.7.4 Optimizers
+4.7.4 Optimizers
 Table 1 shows some of the optimizers available in PyTorch:
 Table 1: Optimizers available in PyTorch (selection). “mom” denotes momentum, “weight”
 weight_decay, “damp” dampening, “nest” nesterov, “lr_sc” learning rate for
 scaling delta, “mom_dec” for momentum_decay, and “step_s” for step_sizes.
 The default values are shown in the table.
 Optimizer
 lr
 
 mom weightdamp nest rho
 
-Adadelta
-Adagrad1e- 2
-Adam 1e- 3
-AdamW1e- 3
-SparseAdam
-1e- 3
-Adamax2e- 3
-
 lr_sc lr_decay
 betas lambd alpha mom_decay
 etas step_s
 
-0.
-0.
-
--
-
--
+Adadelta
+Adagrad1e2
 
-0.9
 -
 
 1.0
 -
 
 0.
-
--
-
 0.
 
 -
 
 -
 
+0.9
 -
 
--
+16
 
--
+0.
 
-1e2
 -
 
 -
 
 -
 
 -
 
 -
 
 -
 
--
+Optimizer
+lr
 
--
+mom weightdamp nest rho
 
+Adam 1e- 3
+AdamW1e- 3
+SparseAdam
+1e- 3
+Adamax2e- 3
+ASGD 1e- 0.9
+2
+LBFGS 1.
+NAdam2e- 3
+RAdam1e- 3
+RMSprop
+1e- 0.
+2
+Rprop 1e- 2
+SGD
+
+required
 0.
 
--
+lr_sc lr_decay
+betas lambd alpha mom_decay
+etas step_s
 
--
+0.
 
 -
 
 -
 
 -
 
@@ -533,183 +672,165 @@
 
 -
 
 -
 
 -
 
+1e2
 -
 
-(0.9,0.999)
 -
 
 -
 
 -
 
 -
 
 -
 
+(0.9,0.999)
 -
 
 -
 
-(0.9,0.999)
 -
 
 -
 
 -
 
 -
 
 -
 
 -
 
 -
 
-(0.9, 0.999)
-
 -
 
+(0.9,0.999)
 -
 
 -
 
 -
 
-13
-
 -
 
-Optimizer
-lr
-
-mom weightdamp nest rho
-
-lr_sc lr_decay
-betas lambd alpha mom_decay
-etas step_s
-
-ASGD 1e2
-LBFGS 1.
-NAdam2e3
-RAdam1e3
-RMSprop
-1e2
-Rprop 1e2
-
-0.9
+-
 
 0.
 
 -
 
-False -
-
 -
 
 -
 
 -
 
 -
 
-0.
-
 -
 
 -
 
 -
 
 -
 
--
+0.
 
 -
 
-0.
+False -
 
 -
 
 -
 
+(0.9, 0.999)
+1e-4
+
+0.75
+
 -
 
 -
 
-0.
+-
 
 0.
 
 -
 
 -
 
 -
 
 -
 
 -
 
+(0.9,0.999)
 -
 
 -
 
-required
-0.
+0
 
-0.
+-
 
-0.
+-
 
-SGD
+0.
 
-1e-4
+-
 
-0.75
+-
 
 -
 
 -
 
 -
 
 (0.9,0.999)
 -
 
 -
 
-0
+-
 
 -
 
 -
 
+0.
+
 -
 
-(0.9,0.999)
 -
 
 -
 
 -
 
 -
 
+(0.9,0.999)
 -
 
 -
 
 -
 
-(0.9,0.999)
 -
 
 -
 
 -
 
 -
@@ -726,14 +847,18 @@
 
 -
 
 -
 
 -
 
+0.
+
+0.
+
 False -
 
 -
 
 -
 
 -
@@ -757,86 +882,86 @@
 torch.optim.LBFGS.html#torch.optim.LBFGS, states:
 This is a very memory intensive optimizer (it requires additional param_bytes
 * (history_size + 1) bytes). If it doesn’t fit in memory try reducing the
 history size, or use a different algorithm.
 Furthermore, the LBFGS optimizer is not compatible with the PyTorch tutorial. The
 reason is that the LBFGS optimizer requires the closure function, which is not implemented in the PyTorch tutorial. Therefore, the LBFGS optimizer is recommended here.
 Since there are 10 optimizers in the portfolio, it is not recommended tuning the hyperparameters that effect one single optimizer only.
-Ĺ A note on the learning rate
-spotPython provides a multiplier for the default learning rates, because optimizers use
-different learning rates. Using a multiplier for the learning rates might enable a simultaneous tuning of the learning rates for all optimizers. However, this is not recommended,
-because the learning rates are not comparable across optimizers. Therefore, we recom-
 
-14
+17
 
-mend fixing the learning rate for all optimizers if multiple optimizers are used. This can
-be done by setting the lower and upper bounds of the learning rate multiplier to the same
-value as shown below.
+Ĺ A note on the learning rate
+spotPython provides a multiplier for the default learning rates, lr_mult, because optimizers use different learning rates. Using a multiplier for the learning rates might enable
+a simultaneous tuning of the learning rates for all optimizers. However, this is not recommended, because the learning rates are not comparable across optimizers. Therefore,
+we recommend fixing the learning rate for all optimizers if multiple optimizers are used.
+This can be done by setting the lower and upper bounds of the learning rate multiplier
+to the same value as shown below.
 Thus, the learning rate, which affects the SGD optimizer, will be set to a fixed value. We choose
 the default value of 1e-3 for the learning rate, because it is used in other PyTorch examples (it
 is also the default value used by spotPython as defined in the optimizer_handler() method).
 We recommend tuning the learning rate later, when a reduced set of optimizers is fixed. Here,
 we will demonstrate how to select in a screening phase the optimizers that should be used for
 the hyperparameter tuning.
 For the same reason, we will fix the sgd_momentum to 0.9.
 fun_control = modify_hyper_parameter_bounds(fun_control, "lr_mult", bounds=[1.0, 1.0])
 fun_control = modify_hyper_parameter_bounds(fun_control, "sgd_momentum", bounds=[0.9, 0.9])
 
-3.8 Evaluation
+4.8 Evaluation
 The evaluation procedure requires the specification of two elements:
 1. the way how the data is split into a train and a test set and
 2. the loss function (and a metric).
-3.8.1 Hold-out Data Split and Cross-Validation
+4.8.1 Hold-out Data Split and Cross-Validation
 As a default, spotPython provides a standard hold-out data split and cross validation.
-3.8.1.1 Hold-out Data Split
+4.8.1.1 Hold-out Data Split
 If a hold-out data split is used, the data will be partitioned into a training, a validation,
 and a test data set. The split depends on the setting of the eval parameter. If eval is set
 to train_hold_out, one data set, usually the original training data set, is split into a new
 training and a validation data set. The training data set is used for training the model. The
 validation data set is used for the evaluation of the hyperparameter configuration and early
 stopping to prevent overfitting. In this case, the original test data set is not used. The following
-splits are performed in the hold-out setting: {train0 , test} → {train1 , validation1 , test}, where
-train1 ∪ validation1 = train0 .
 
-15
+18
 
-Ĺ Note
-spotPython returns the hyperparameters of the machine learning and deep learning models, e.g., number of layers, learning rate, or optimizer, but not the model weights. Therefore, after the SPOT run is finished, the corresponding model has to be trained again
-with the best hyperparameter configuration. The training is performed on the training
-data set. The test data set is used for the final evaluation of the model.
+splits are performed in the hold-out setting: {train0 , test} → {train1 , validation1 , test}, where
+train1 ∪ validation1 = train0 .
+Ĺ Note
+spotPython returns the hyperparameters of the machine learning and deep learning models, e.g., number of layers, learning rate, or optimizer, but not the model weights. Therefore, after the SPOT run is finished, the corresponding model with the optimized architecture has to be trained again with the best hyperparameter configuration. The training
+is performed on the training data set. The test data set is used for the final evaluation
+of the model.
 Summarizing, the following splits are performed in the hold-out setting:
 1. Run spotPython with eval set to train_hold_out to determine the best hyperparameter configuration.
-2. Train the model with the best hyperparameter configuration on the training data
-set:
+2. Train the model with the best hyperparameter configuration (“architecture”) on
+the training data set:
 • train_tuned(model_spot, train, "model_spot.pt").
 3. Test the model on the test data:
 • test_tuned(model_spot, test, "model_spot.pt")
 These steps will be exemplified in the following sections.
 In addition to this hold-out setting, spotPython provides another hold-out setting, where an
 explicit test data is specified by the user that will be used as the validation set. To choose this
 option, the eval parameter is set to test_hold_out. In this case, the training data set is used
 for the model training. Then, the explicitly defined test data set is used for the evaluation of
 the hyperparameter configuration (the validation).
-3.8.1.2 Cross-Validation
+4.8.1.2 Cross-Validation
 The cross validation setting is used by setting the eval parameter to train_cv or test_cv. In
 both cases, the data set is split into 𝑘 folds. The model is trained on 𝑘 − 1 folds and evaluated
 on the remaining fold. This is repeated 𝑘 times, so that each fold is used exactly once for
 evaluation. The final evaluation is performed on the test data set. The cross validation setting
 is useful for small data sets, because it allows to use all data for training and evaluation.
 However, it is computationally expensive, because the model has to be trained 𝑘 times.
-Ĺ Note
+
+19
+
+Ĺ Note
 Combinations of the above settings are possible, e.g., cross validation can be used for
 training and hold-out for evaluation or vice versa. Also, cross validation can be used
 for training and testing. Because cross validation is not used in the PyTorch tutorial
 (PyTorch 2023a), it is not considered further here.
 
-16
-
-3.8.1.3 Overview of the Evaluation Settings
-3.8.1.3.1 Settings for the Hyperparameter Tuning
+4.8.1.3 Overview of the Evaluation Settings
+4.8.1.3.1 Settings for the Hyperparameter Tuning
 Table 2 provides an overview of the training evaluations.
 Table 2: Overview of the evaluation settings.
 eval
 
 train
 
 "train_hold_out"
@@ -866,330 +991,80 @@
 train_hold_out(),
 splits the
 validate_fold_or_hold_out()
 train data
 for early
 set internally
 stopping
-train_hold_out(),
 use the test
-validate_fold_or_hold_out()
+train_hold_out(),
 data set for
-for early
+validate_fold_or_hold_out()
 validate_fold_or_hold_out(
+for early
 stopping
-CV using
 evaluate_cv(net,
+CV using
 train)
 the train
 data set
 evaluate_cv(net,
 CV using
 test)
 the test
 data set .
 Identical to
 "train_cv",
 uses only
 test data.
 
 • "train_cv" and "test_cv" use sklearn.model_selection.KFold() internally.
-3.8.1.4 Detailed Description of the "train_hold_out" Setting
-The "train_hold_out" setting is used by default. It uses the loss function specfied in
-fun_control and the metric specified in fun_control.
-1. First, the method HyperTorch().fun_torch is called.
-2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() as follows:
-df_eval, _ = evaluate_hold_out(
-model,
-train_dataset=fun_control["train"],
-shuffle=self.fun_control["shuffle"],
-
-17
-
-loss_function=self.fun_control["loss_function"],
-metric=self.fun_control["metric_torch"],
-device=self.fun_control["device"],
-show_batch_interval=self.fun_control["show_batch_interval"],
-path=self.fun_control["path"],
-)
-Note: Only the data set fun_control["train"] is used for training and validation. It is used
-as follows:
-trainloader, valloader = create_train_val_data_loaders(
-dataset=train_dataset, batch_size=batch_size_instance, shuffle=shuffle
-)
-create_train_val_data_loaders() splits the train_dataset into trainloader and
-valloader using torch.utils.data.random_split() as follows:
-def create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):
-test_abs = int(len(dataset) * 0.6)
-train_subset, val_subset = random_split(dataset, [test_abs, len(dataset) - test_abs])
-trainloader = torch.utils.data.DataLoader(
-train_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers
-)
-valloader = torch.utils.data.DataLoader(
-val_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers
-)
-return trainloader, valloader
-The optimizer is set up as follows:
-
-lr_mult_instance = net.lr_mult
-optimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_
-3. evaluate_hold_out() sets the net attributes such as epochs, batch_size,
-optimizer, and patience. For each epoch, the methods train_hold_out() and
-validate_fold_or_hold_out() are called, the former for training and the latter for
-validation and early stopping. The validation loss from the last epoch (not the best
-validation loss) is returned from evaluate_hold_out.
-4. The method train_hold_out() is implemented as follows:
-
-18
-
-def train_hold_out(net, trainloader, batch_size, loss_function, optimizer, device, show_batch
-running_loss = 0.0
-epoch_steps = 0
-for i, data in enumerate(trainloader, 0):
-inputs, labels = data
-inputs, labels = inputs.to(device), labels.to(device)
-optimizer.zero_grad()
-outputs = net(inputs)
-loss = loss_function(outputs, labels)
-loss.backward()
-torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
-optimizer.step()
-running_loss += loss.item()
-epoch_steps += 1
-if i % show_batch_interval == (show_batch_interval - 1): # print every show_batch_in
-print(
-"Batch: %5d. Batch Size: %d. Training Loss (running): %.3f"
-% (i + 1, int(batch_size), running_loss / epoch_steps)
-)
-running_loss = 0.0
-return loss.item()
-5. The method validate_fold_or_hold_out() is implemented as follows:
-def validate_fold_or_hold_out(net, valloader, loss_function, metric, device):
-val_loss = 0.0
-val_steps = 0
-metric.reset()
-for i, data in enumerate(valloader, 0):
-with torch.no_grad():
-inputs, labels = data
-inputs, labels = inputs.to(device), labels.to(device)
-outputs = net(inputs)
-_, predicted = torch.max(outputs.data, 1)
-metric_value = metric(predicted, labels).to(device)
-loss = loss_function(outputs, labels)
-val_loss += loss.cpu().numpy()
-val_steps += 1
-loss = val_loss / val_steps
-metric_value = metric.compute()
-return metric_value, loss
-
-19
-
-3.8.1.5 Detailed Description of the "test_hold_out" Setting
-It uses the loss function specfied in fun_control and the metric specified in fun_control.
-1. First, the method HyperTorch().fun_torch is called.
-2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() similar to the
-"train_hold_out" setting with one exception: It passes an additional test data set to
-evaluate_hold_out() as follows:
-test_dataset=fun_control["test"]
-evaluate_hold_out() calls create_train_test_data_loaders instead of create_train_val_data_loaders
-as follows: The two data sets are used in create_train_test_data_loaders as follows:
-
-def create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset, num_workers=0)
-trainloader = torch.utils.data.DataLoader(
-dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers
-)
-testloader = torch.utils.data.DataLoader(
-test_dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers
-)
-return trainloader, testloader
-3. The following steps are identical to the "train_hold_out" setting. Only a different data
-loader is used for testing.
-3.8.1.6 Detailed Description of the "train_cv" Setting
-It uses the loss function specfied in fun_control and the metric specified in fun_control.
-1. First, the method HyperTorch().fun_torch is called.
-2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
-df_eval, _ = evaluate_cv(
-model,
-dataset=fun_control["train"],
-shuffle=self.fun_control["shuffle"],
-device=self.fun_control["device"],
-show_batch_interval=self.fun_control["show_batch_interval"],
-)
-Note: Only the data set fun_control["train"] is used for CV. 3. In ‘evaluate_cv(), the
-following steps are performed: The optimizer is set up as follows:
+Section 6.2 (in the Appendix) provides more details on the data splitting.
+4.8.1.4 Settings for the Final Evaluation of the Tuned Architecture
 
 20
 
-lr_instance = net.lr
-optimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_
-evaluate_cv() sets the net attributes such as epochs, batch_size, optimizer, and
-patience. CV is implemented as follows:
-
-kfold = KFold(n_splits=k_folds_instance, shuffle=shuffle)
-for fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):
-train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)
-val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)
-trainloader = torch.utils.data.DataLoader(
-dataset, batch_size=batch_size_instance, sampler=train_subsampler, num_workers=num_wo
-)
-valloader = torch.utils.data.DataLoader(
-dataset, batch_size=batch_size_instance, sampler=val_subsampler, num_workers=num_work
-)
-reset_weights(net)
-# Train fold for several epochs:
-train_fold(
-net,
-trainloader,
-epochs_instance,
-loss_function,
-optimizer,
-device,
-show_batch_interval=show_batch_interval,
-)
-# Validate fold: use only loss for tuning
-metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_f
-df_eval = sum(loss_values.values()) / len(loss_values.values())
-4. The method train_fold() is implemented as follows:
-
-def train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interva
-for epoch in range(epochs):
-print(f"Epoch: {epoch + 1}")
-running_loss = 0.0
-epoch_steps = 0
-for i, data in enumerate(trainloader, 0):
-inputs, labels = data
-inputs, labels = inputs.to(device), labels.to(device)
-optimizer.zero_grad()
-
-21
-
-outputs = net(inputs)
-loss = loss_function(outputs, labels)
-loss.backward()
-torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
-optimizer.step()
-# the following is for printing the statistic only
-running_loss += loss.item()
-epoch_steps += 1
-if i % show_batch_interval == (show_batch_interval - 1): # print every show_batc
-print("Batch: %5d. Training Loss (running): %.3f" % (i + 1, running_loss / ep
-running_loss = 0.0
-5. The method validate_fold_or_hold_out() is implemented as shown above. In contrast to the hold-out setting, it is called for each of the 𝑘 folds. The results are stored in
-a dictionaries metric_values and loss_values as follows:
-
-# Validate fold: use only loss for tuning
-metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_f
-df_eval = sum(loss_values.values()) / len(loss_values.values())
-The results are averaged over the 𝑘 folds and returned as df_eval.
-3.8.1.7 Detailed Description of the "test_cv" Setting
-It uses the loss function specfied in fun_control and the metric specified in fun_control.
-1. First, the method HyperTorch().fun_torch is called.
-2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
-df_eval, _ = evaluate_cv(
-model,
-dataset=fun_control["test"],
-shuffle=self.fun_control["shuffle"],
-device=self.fun_control["device"],
-show_batch_interval=self.fun_control["show_batch_interval"],
-)
-Note: The data set fun_control["test"] is used for CV. The rest is the same as for the
-"train_cv" setting.
-3.8.1.8 Settings for the Final Evaluation of the Tuned Architecture
-
-22
-
-3.8.1.8.1 Training of the Tuned Architecture
+4.8.1.4.1 Training of the Tuned Architecture
 train_tuned(model, train): train the model with the best hyperparameter configuration (or simply the default) on the training data set. It splits the traindata into
 new train and validation sets using create_train_val_data_loaders(), which
 calls torch.utils.data.random_split() internally.
 Currently, 60% of the data is
 used for training and 40% for validation. The train data is used for training the
 model with train_hold_out(). The validation data is used for early stopping using
 validate_fold_or_hold_out() on the validation data set.
-train_tuned() is just a wrapper to evaluate_hold_out using the train data set. It is
-implemented as follows:
-
-def train_tuned(net, train_dataset, shuffle, loss_function, metric, device=None, show_batch_i
-evaluate_hold_out(
-net=net,
-train_dataset=train_dataset,
-shuffle=shuffle,
-test_dataset=None,
-loss_function=loss_function,
-metric=metric,
-device=device,
-show_batch_interval=show_batch_interval,
-path=path,
-)
-Note: During training, shuffle is set to True, whereas during testing, shuffle is set to
-False.
-3.8.1.8.2 Testing of the Tuned Architecture
+4.8.1.4.2 Testing of the Tuned Architecture
 test_tuned(model, test): test the model on the test data set. No data splitting is performed.
 The (trained) model is evaluated using the validate_fold_or_hold_out() function.
 Note: During training, shuffle is set to True, whereas during testing, shuffle is set to
 False.
-
-def test_tuned(net, shuffle, test_dataset=None, loss_function=None, metric=None, device=None,
-batch_size_instance = net.batch_size
-removed_attributes, net = get_removed_attributes_and_base_net(net)
-if path is not None:
-net.load_state_dict(torch.load(path))
-net.eval()
-
-23
-
-try:
-
-device = getDevice(device=device)
-if torch.cuda.is_available():
-device = "cuda:0"
-if torch.cuda.device_count() > 1:
-print("We will use", torch.cuda.device_count(), "GPUs!")
-net = nn.DataParallel(net)
-net.to(device)
-valloader = torch.utils.data.DataLoader(
-test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle, num_workers=0
-)
-metric_value, loss = validate_fold_or_hold_out(
-net, valloader=valloader, loss_function=loss_function, metric=metric, device=devi
-)
-df_eval = loss
-df_metric = metric_value
-df_preds = np.nan
-except Exception as err:
-print(f"Error in Net_Core. Call to test_tuned() failed. {err=}, {type(err)=}")
-df_eval = np.nan
-df_metric = np.nan
-df_preds = np.nan
-add_attributes(net, removed_attributes)
-print(f"Final evaluation: Validation loss: {df_eval}")
-print(f"Final evaluation: Validation metric: {df_metric}")
-print("----------------------------------------------")
-return df_eval, df_preds, df_metric
-
-3.8.2 Loss Functions and Metrics
+Section 6.2.5 describes the final evaluation of the tuned architecture.
+4.8.2 Loss Functions and Metrics
 The key "loss_function" specifies the loss function which is used during the optimization.
 There are several different loss functions under PyTorch’s nn package. For example, a simple
 loss is MSELoss, which computes the mean-squared error between the output and the target. In
 this tutorial we will use CrossEntropyLoss, because it is also used in the PyTorch tutorial.
 from torch.nn import CrossEntropyLoss
 loss_function = CrossEntropyLoss()
 fun_control.update({"loss_function": loss_function})
 In addition to the loss functions, spotPython provides access to a large number of metrics.
 The key "metric_sklearn" is used for metrics that follow the scikit-learn conventions.
-
-24
-
-The key "river_metric" is used for the river based evaluation (Montiel et al. 2021) via
+The key "river_metric" is used for the river based evaluation (Montiel et al. 2021) via
 eval_oml_iter_progressive, and the key "metric_torch" is used for the metrics from
 TorchMetrics. TorchMetrics is a collection of more than 90 PyTorch metrics4 . Because
-the PyTorch tutorial uses the accuracy as metric, we use the same metric here. Currently, accuracy is computed in the tutorial’s example code. We will use TorchMetrics instead, because
-it offers:
+the PyTorch tutorial uses the accuracy as metric, we use the same metric here. Currently,
+accuracy is computed in the tutorial’s example code. We will use TorchMetrics instead, because it offers more flexibilty, e.g., it can be used for regression and classification. Furthermore,
+TorchMetrics offers the following advantages:
 • A standardized interface to increase reproducibility
-• Reduces Boilerplate
+4
+
+https://torchmetrics.readthedocs.io/en/latest/.
+
+21
+
+• Reduces Boilerplate
 • Distributed-training compatible
 • Rigorously tested
 • Automatic accumulation over batches
 • Automatic synchronization between multiple devices
 Therefore, we set
 metric_torch = torchmetrics.Accuracy(task="multiclass", num_classes=10)
 loss_function = CrossEntropyLoss()
@@ -1210,27 +1085,23 @@
 "log_level": 50,
 "weight_coeff": None,
 "metric_torch": metric_torch,
 "metric_river": None,
 "metric_sklearn": None,
 "loss_function": loss_function,
 "shuffle": shuffle,
-4
-
-https://torchmetrics.readthedocs.io/en/latest/.
-
-25
-
-"eval": eval,
+"eval": eval,
 "device": device,
 "show_batch_interval": show_batch_interval,
 "path": path,
 })
 
-3.9 Calling the SPOT Function
+22
+
+4.9 Calling the SPOT Function
 Now, the dictionary fun_control contains all information needed for the hyperparameter
 tuning. Before the hyperparameter tuning is started, it is recommended to take a look at the
 experimental design. The method gen_design_table generates a design table as follows:
 print(gen_design_table(fun_control))
 This allows to check if all information is available and if the information is correct. Table 3
 shows the experimental design for the hyperparameter tuning. Hyperparameter transformations are shown in the column “transform”, e.g., the l1 default is 5, which results in the value
 25 = 32 for the network, because the transformation transform_power_2_int was selected in
@@ -1303,24 +1174,24 @@
 transform_power_2_int
 None
 None
 None
 
 The objective function fun_torch is selected next. It implements an interface from PyTorch’s
 training, validation, and testing methods to spotPython.
-
-26
-
-fun = HyperTorch().fun_torch
+fun = HyperTorch().fun_torch
 The spotPython hyperparameter tuning is started by calling the Spot function. Here, we will
 run the tuner for approximately 30 minutes (max_time). Note: the initial design is always
 evaluated in the spotPython run. As a consequence, the run may take longer than specified
 by max_time, because the evaluation time of initial design (here: init_size, 10 points) is
 performed independently of max_time.
-spot_tuner = spot.Spot(fun=fun,
+
+23
+
+spot_tuner = spot.Spot(fun=fun,
 lower = lower,
 upper = upper,
 fun_evals = inf,
 fun_repeats = 1,
 max_time = MAX_TIME,
 noise = False,
 tolerance_x = np.sqrt(np.spacing(1)),
@@ -1343,27 +1214,28 @@
 "model_optimizer": differential_evolution,
 "model_fun_evals": 10_000,
 "log_level": 50
 })
 spot_tuner.run(X_start=X_start)
 During the run, the following output is shown:
 
-27
-
-config: {'l1': 4, 'l2': 64, 'lr_mult': 1.0, 'batch_size': 16, 'epochs': 16, 'k_folds': 0, 'pa
+config: {'l1': 4, 'l2': 64, 'lr_mult': 1.0, 'batch_size': 16, 'epochs': 16, 'k_folds': 0, 'pa
 Epoch: 1
 Loss on hold-out set: 1.602842689704895
 Accuracy on hold-out set: 0.4006
 Metric value on hold-out data: 0.40059998631477356
 Epoch: 2
 Loss on hold-out set: 1.4648857820034027
 Accuracy on hold-out set: 0.47685
 Metric value on hold-out data: 0.4768500030040741
 Epoch: 3
-Loss on hold-out set: 1.403354868555069
+
+24
+
+Loss on hold-out set: 1.403354868555069
 Accuracy on hold-out set: 0.482
 Metric value on hold-out data: 0.4819999933242798
 Epoch: 4
 Loss on hold-out set: 1.384560032081604
 Accuracy on hold-out set: 0.49065
 Metric value on hold-out data: 0.4906499981880188
 Epoch: 5
@@ -1387,53 +1259,52 @@
 Accuracy on hold-out set: 0.5304
 Metric value on hold-out data: 0.5303999781608582
 Epoch: 10
 Loss on hold-out set: 1.3481314319610596
 Accuracy on hold-out set: 0.5268
 Metric value on hold-out data: 0.5267999768257141
 Epoch: 11
-
-28
-
-Loss on hold-out set: 1.3608774542331696
+Loss on hold-out set: 1.3608774542331696
 Accuracy on hold-out set: 0.51525
 Metric value on hold-out data: 0.515250027179718
 Epoch: 12
 Loss on hold-out set: 1.359324642753601
 Accuracy on hold-out set: 0.52355
 Metric value on hold-out data: 0.5235499739646912
 Early stopping at epoch 11
 Returned to Spot: Validation loss: 1.359324642753601
 ----------------------------------------------
 
-3.10 Results
+25
+
+4.10 Results
 After the hyperparameter tuning run is finished, the progress of the hyperparameter tuning
 can be visualized. The following code generates the progress plot from Figure 2.
 
 spot_tuner.plot_progress(log_y=False, filename="./figures" + experiment_name+"_progress.png")
 Figure 1: ?(caption)
 
 Figure 2: Progress plot. Black dots denote results from the initial design. Red dots illustrate
 the improvement found by the surrogate model based optimization (surrogate model
 based optimization).
 Figure 2 shows a typical behaviour that can be observed in many hyperparameter studies
 (Bartz et al. 2022): the largest improvement is obtained during the evaluation of the initial
 design. The surrogate model based optimization-optimization with the surrogate refines the
 results. Figure 2 also illustrates one major difference between ray[tune] as used in PyTorch
-
-29
-
-(2023a) and spotPython: the ray[tune] uses a random search and will generate results similar to the black dots, whereas spotPython uses a surrogate model based optimization and
+(2023a) and spotPython: the ray[tune] uses a random search and will generate results similar to the black dots, whereas spotPython uses a surrogate model based optimization and
 presents results represented by red dots in Figure 2. The surrogate model based optimization
 is considered to be more eﬀicient than a random search, because the surrogate model guides
 the search towards promising regions in the hyperparameter space.
 In addition to the improved (“optimized”) hyperparameter values, spotPython allows a statistical analysis, e.g., a sensitivity analysis, of the results. We can print the results of the
 hyperparameter tuning, see Table 4.
 print(gen_design_table(fun_control=fun_control, spot=spot_tuner))
-Table 4: Results of the hyperparameter tuning. The table shows the hyperparameters, their
+
+26
+
+Table 4: Results of the hyperparameter tuning. The table shows the hyperparameters, their
 types, default values, lower and upper bounds, and the transformation function. The
 column “tuned” shows the tuned values. The column “importance” shows the importance of the hyperparameters. The column “stars” shows the importance of the
 hyperparameters in stars. The importance is computed by the SPOT software.
 name
 
 type
 
@@ -1522,55 +1393,55 @@
 .
 
 To visualize the most important hyperparameters, spotPython provides the function
 plot_importance. The following code generates the importance plot from Figure 3.
 
 spot_tuner.plot_importance(threshold=0.025, filename="./figures" + experiment_name+"_importan
 
-3.11 Get SPOT Results
+Figure 3: Variable importance
+
+4.11 Get SPOT Results
 The architecture of the spotPython model can be obtained by the following code:
-X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1,-1))
-model_spot = get_one_core_model_from_X(X, fun_control)
-model_spot
 
-30
+27
 
-Figure 3: Variable importance
+X = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1,-1))
+model_spot = get_one_core_model_from_X(X, fun_control)
+model_spot
 First, the numerical representation of the hyperparameters are obtained, i.e., the numpy array
 X is generated. This array is then used to generate the model model_spot by the function
 get_one_core_model_from_X. The model model_spot has the following architecture:
 Net_CIFAR10(
 (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))
 (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
 (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))
 (fc1): Linear(in_features=400, out_features=64, bias=True)
 (fc2): Linear(in_features=64, out_features=32, bias=True)
 (fc3): Linear(in_features=32, out_features=10, bias=True)
 )
 
-3.12 Get Default Hyperparameters
-In a similar manner as in Section 3.11, the default hyperparameters can be obtained.
+4.12 Get Default Hyperparameters
+In a similar manner as in Section 4.11, the default hyperparameters can be obtained.
 # fun_control was modified, we generate a new one with the original default hyperparameters
 fc = copy.deepcopy(fun_control)
 fc.update({"core_model_hyper_dict": hyper_dict[fun_control["core_model"].__name__]})
 model_default = get_one_core_model_from_X(X_start, fun_control=fc)
 The corresponding default model has the following architecture:
-
-31
-
-Net_CIFAR10(
+Net_CIFAR10(
 (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))
 (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
 (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))
 (fc1): Linear(in_features=400, out_features=32, bias=True)
 (fc2): Linear(in_features=32, out_features=32, bias=True)
 (fc3): Linear(in_features=32, out_features=10, bias=True)
 )
 
-3.13 Evaluation of the Tuned Architecture
+28
+
+4.13 Evaluation of the Tuned Architecture
 The method train_tuned takes a model architecture without trained weights and trains this
 model with the train data. The train data is split into train and validation data. The validation
 data is used for early stopping. The trained model weights are saved as a dictionary.
 This evaluation is similar to the final evaluation in PyTorch (2023a).
 train_tuned(net=model_default, train_dataset=train, shuffle=True,
 loss_function=fun_control["loss_function"],
 metric=fun_control["metric_torch"],
@@ -1587,28 +1458,28 @@
 metric=fun_control["metric_torch"],
 shuffle=True,
 device = DEVICE,
 path=None)
 Loss on hold-out set: 1.2267619131326675
 Accuracy on hold-out set: 0.58955
 Early stopping at epoch 13
-
-32
-
-If path is set to a filename, e.g., path = "model_spot_trained.pt", the weights of the trained
+If path is set to a filename, e.g., path = "model_spot_trained.pt", the weights of the trained
 model will be loaded from this file.
 test_tuned(net=model_spot, test_dataset=test,
 shuffle=False,
 loss_function=fun_control["loss_function"],
 metric=fun_control["metric_torch"],
 device = DEVICE)
-Loss on hold-out set: 1.242568492603302
+
+29
+
+Loss on hold-out set: 1.242568492603302
 Accuracy on hold-out set: 0.5957
 
-3.14 Comparison with Default Hyperparameters and Ray Tune
+4.14 Comparison with Default Hyperparameters and Ray Tune
 Table 5 shows the loss and accuracy of the default model, the model with the hyperparameters
 from SPOT, and the model with the hyperparameters from ray[tune].
 Table 5: Comparison of the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from ray[tune].
 ray[tune] only shows the validation loss, because training loss is not reported by
 ray[tune].
 Model
 Default
@@ -1635,91 +1506,79 @@
 1.2426
 -
 
 0.2425
 0.5957
 0.5806
 
-3.15 Detailed Hyperparameter Plots
+4.15 Detailed Hyperparameter Plots
 The contour plots in this section visualize the interactions of the three most important hyperparameters, l1, l2, and epochs, and optimizer of the surrogate model used to optimize
 the hyperparameters. Since some of these hyperparameters take fatorial or integer values,
 sometimes step-like fitness landcapes (or response surfaces) are generated. SPOT draws the
 interactions of the main hyperparameters by default. It is also possible to visualize all interactions. For this, again refer to the notebook (Bartz-Beielstein 2023).
-Figure 5 to Figure 10 show the contour plots of the loss as a function of the hyperparameters.
+filename = "./figures" + experiment_name
+spot_tuner.plot_important_hyperparameter_contour(filename=filename)
+Figure 4 to Figure 9 show the contour plots of the loss as a function of the hyperparameters.
 These plots are very helpful for benchmark studies and for understanding neural networks.
 spotPython provides additional tools for a visual inspection of the results and give valuable
+insights into the hyperparameter tuning process. This is especially useful for model explainability, transparency, and trustworthiness. In addition to the contour plots, Figure 10 shows
+the parallel plot of the hyperparameters.
+spot_tuner.parallel_plot()
 
-33
-
-threshold = 0.025
-impo = spot_tuner.print_importance(threshold=threshold, print_screen=True)
-var_plots = [i for i, x in enumerate(impo) if x[1] > threshold]
-min_z = min(spot_tuner.y)
-max_z = max(spot_tuner.y)
-n = spot_tuner.k
-for i in var_plots:
-for j in var_plots:
-if j > i:
-filename = "./figures" + experiment_name+"_contour_"+str(i)+"_"+str(j)+".png"
-spot_tuner.plot_contour(i=i, j=j, min_z=min_z, max_z = max_z, filename=filename)
-Figure 4: ?(caption)
+30
 
-Figure 5: Contour plot of the loss as a function of l1 and l2, i.e., the number of neurons in
+Figure 4: Contour plot of the loss as a function of l1 and l2, i.e., the number of neurons in
 the layers.
 
-34
-
-Figure 6: Contour plot of the loss as a function of the number of epochs and the neurons in
+Figure 5: Contour plot of the loss as a function of the number of epochs and the neurons in
 layer l1.
 
-Figure 7: Contour plot of the loss as a function of the optimizer and the neurons in layer l1.
+31
 
-35
+Figure 6: Contour plot of the loss as a function of the optimizer and the neurons in layer l1.
 
-Figure 8: Contour plot of the loss as a function of the number of epochs and the neurons in
+Figure 7: Contour plot of the loss as a function of the number of epochs and the neurons in
 layer l2.
 
-Figure 9: Contour plot of the loss as a function of the optimizer and the neurons in layer l2.
+32
 
-36
+Figure 8: Contour plot of the loss as a function of the optimizer and the neurons in layer l2.
 
-Figure 10: Contour plot of the loss as a function of the optimizer and the number of epochs.
-insights into the hyperparameter tuning process. This is especially useful for model explainability, transparency, and trustworthiness. In addition to the contour plots, Figure 12 shows
-the parallel plot of the hyperparameters.
-spot_tuner.parallel_plot()
-Figure 11: ?(caption)
+Figure 9: Contour plot of the loss as a function of the optimizer and the number of epochs.
 
-4 Summary and Outlook
+33
+
+Figure 10: Parallel plot
+
+5 Summary and Outlook
 This tutorial presents the hyperparameter tuning open source software spotPython for
 PyTorch. To show its basic features, a comparison with the “oﬀicial” PyTorch hyperparameter tuning tutorial (PyTorch 2023a) is presented. Some of the advantages of spotPython
 are:
 • Numerical and categorical hyperparameters.
 • Powerful surrogate models.
 • Flexible approach and easy to use.
 • Simple JSON files for the specification of the hyperparameters.
 • Extension of default and user specified network classes.
 • Noise handling techniques.
 Currently, only rudimentary parallel and distributed neural network training is possible, but
 these capabilities will be extended in the future. The next version of spotPython will also
 include a more detailed documentation and more examples.
-
-37
-
-Figure 12: Parallel plot
-
 ĺ Important
 Important: This tutorial does not present a complete benchmarking study (BartzBeielstein et al. 2020). The results are only preliminary and highly dependent on the
 local configuration (hard- and software). Our goal is to provide a first impression of
 the performance of the hyperparameter tuning package spotPython. To demonstrate its
 capabilities, a quick comparison with ray[tune] was performed. ray[tune] was chosen, because it is presented as “an industry standard tool for distributed hyperparameter
 tuning.” The results should be interpreted with care.
 
-5 Appendix
-Sample Output From Ray Tune’s Run
+34
+
+6 Appendix
+6.1 Sample Output From Ray Tune’s Run
 The output from ray[tune] could look like this (PyTorch 2023b):
+
 Number of trials: 10 (10 TERMINATED)
 ------+------+-------------+--------------+---------+------------+--------------------+
 |
 l1 |
 l2 |
 lr |
 batch_size |
@@ -1752,18 +1611,15 @@
 8 |
 |
 32 |
 16 | 0.000340753 |
 8 | 1.26454 |
 0.5444 |
 8 |
-
-38
-
-|
+|
 8 |
 4 | 0.000699775 |
 8 | 1.99594 |
 0.1983 |
 2 |
 | 256 |
 8 | 0.0839654
@@ -1790,16 +1646,278 @@
 0.1945 |
 1 |
 +-----+------+------+-------------+--------------+---------+------------+-------------------Best trial config: {'l1': 8, 'l2': 16, 'lr': 0.00276249, 'batch_size': 16, 'data_dir': '...'}
 Best trial final validation loss: 1.181501
 Best trial final validation accuracy: 0.5836
 Best trial test set accuracy: 0.5806
 
+35
+
+6.2 Detailed Description of the Data Splitting
+6.2.1 Description of the "train_hold_out" Setting
+The "train_hold_out" setting is used by default. It uses the loss function specfied in
+fun_control and the metric specified in fun_control.
+1. First, the method HyperTorch().fun_torch is called.
+2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() as follows:
+df_eval, _ = evaluate_hold_out(
+model,
+train_dataset=fun_control["train"],
+shuffle=self.fun_control["shuffle"],
+loss_function=self.fun_control["loss_function"],
+metric=self.fun_control["metric_torch"],
+device=self.fun_control["device"],
+show_batch_interval=self.fun_control["show_batch_interval"],
+path=self.fun_control["path"],
+)
+Note: Only the data set fun_control["train"] is used for training and validation. It is used
+as follows:
+trainloader, valloader = create_train_val_data_loaders(
+dataset=train_dataset, batch_size=batch_size_instance, shuffle=shuffle
+)
+create_train_val_data_loaders() splits the train_dataset into trainloader and
+valloader using torch.utils.data.random_split() as follows:
+def create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):
+test_abs = int(len(dataset) * 0.6)
+train_subset, val_subset = random_split(dataset, [test_abs, len(dataset) - test_abs])
+trainloader = torch.utils.data.DataLoader(
+train_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers
+)
+valloader = torch.utils.data.DataLoader(
+val_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers
+)
+return trainloader, valloader
+
+36
+
+The optimizer is set up as follows:
+
+lr_mult_instance = net.lr_mult
+optimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_
+3. evaluate_hold_out() sets the net attributes such as epochs, batch_size,
+optimizer, and patience. For each epoch, the methods train_hold_out() and
+validate_fold_or_hold_out() are called, the former for training and the latter for
+validation and early stopping. The validation loss from the last epoch (not the best
+validation loss) is returned from evaluate_hold_out.
+4. The method train_hold_out() is implemented as follows:
+
+def train_hold_out(net, trainloader, batch_size, loss_function, optimizer, device, show_batch
+running_loss = 0.0
+epoch_steps = 0
+for i, data in enumerate(trainloader, 0):
+inputs, labels = data
+inputs, labels = inputs.to(device), labels.to(device)
+optimizer.zero_grad()
+outputs = net(inputs)
+loss = loss_function(outputs, labels)
+loss.backward()
+torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
+optimizer.step()
+running_loss += loss.item()
+epoch_steps += 1
+if i % show_batch_interval == (show_batch_interval - 1): # print every show_batch_in
+print(
+"Batch: %5d. Batch Size: %d. Training Loss (running): %.3f"
+% (i + 1, int(batch_size), running_loss / epoch_steps)
+)
+running_loss = 0.0
+return loss.item()
+5. The method validate_fold_or_hold_out() is implemented as follows:
+def validate_fold_or_hold_out(net, valloader, loss_function, metric, device):
+val_loss = 0.0
+val_steps = 0
+metric.reset()
+for i, data in enumerate(valloader, 0):
+with torch.no_grad():
+
+37
+
+inputs, labels = data
+inputs, labels = inputs.to(device), labels.to(device)
+outputs = net(inputs)
+_, predicted = torch.max(outputs.data, 1)
+metric_value = metric(predicted, labels).to(device)
+loss = loss_function(outputs, labels)
+val_loss += loss.cpu().numpy()
+val_steps += 1
+loss = val_loss / val_steps
+metric_value = metric.compute()
+return metric_value, loss
+
+6.2.2 Description of the "test_hold_out" Setting
+It uses the loss function specfied in fun_control and the metric specified in fun_control.
+1. First, the method HyperTorch().fun_torch is called.
+2. fun_torc() calls spotPython.torch.traintest.evaluate_hold_out() similar to the
+"train_hold_out" setting with one exception: It passes an additional test data set to
+evaluate_hold_out() as follows:
+test_dataset=fun_control["test"]
+evaluate_hold_out() calls create_train_test_data_loaders instead of create_train_val_data_loaders
+as follows: The two data sets are used in create_train_test_data_loaders as follows:
+
+def create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset, num_workers=0)
+trainloader = torch.utils.data.DataLoader(
+dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers
+)
+testloader = torch.utils.data.DataLoader(
+test_dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers
+)
+return trainloader, testloader
+3. The following steps are identical to the "train_hold_out" setting. Only a different data
+loader is used for testing.
+
+38
+
+6.2.3 Detailed Description of the "train_cv" Setting
+It uses the loss function specfied in fun_control and the metric specified in fun_control.
+1. First, the method HyperTorch().fun_torch is called.
+2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
+df_eval, _ = evaluate_cv(
+model,
+dataset=fun_control["train"],
+shuffle=self.fun_control["shuffle"],
+device=self.fun_control["device"],
+show_batch_interval=self.fun_control["show_batch_interval"],
+)
+Note: Only the data set fun_control["train"] is used for CV. 3. In ‘evaluate_cv(), the
+following steps are performed: The optimizer is set up as follows:
+
+lr_instance = net.lr
+optimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_
+evaluate_cv() sets the net attributes such as epochs, batch_size, optimizer, and
+patience. CV is implemented as follows:
+
+kfold = KFold(n_splits=k_folds_instance, shuffle=shuffle)
+for fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):
+train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)
+val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)
+trainloader = torch.utils.data.DataLoader(
+dataset, batch_size=batch_size_instance, sampler=train_subsampler, num_workers=num_wo
+)
+valloader = torch.utils.data.DataLoader(
+dataset, batch_size=batch_size_instance, sampler=val_subsampler, num_workers=num_work
+)
+reset_weights(net)
+# Train fold for several epochs:
+train_fold(
+net,
+trainloader,
+epochs_instance,
+loss_function,
+optimizer,
+
 39
 
+device,
+show_batch_interval=show_batch_interval,
+
+)
+# Validate fold: use only loss for tuning
+metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_f
+df_eval = sum(loss_values.values()) / len(loss_values.values())
+4. The method train_fold() is implemented as follows:
+
+def train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interva
+for epoch in range(epochs):
+print(f"Epoch: {epoch + 1}")
+running_loss = 0.0
+epoch_steps = 0
+for i, data in enumerate(trainloader, 0):
+inputs, labels = data
+inputs, labels = inputs.to(device), labels.to(device)
+optimizer.zero_grad()
+outputs = net(inputs)
+loss = loss_function(outputs, labels)
+loss.backward()
+torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
+optimizer.step()
+# the following is for printing the statistic only
+running_loss += loss.item()
+epoch_steps += 1
+if i % show_batch_interval == (show_batch_interval - 1): # print every show_batc
+print("Batch: %5d. Training Loss (running): %.3f" % (i + 1, running_loss / ep
+running_loss = 0.0
+5. The method validate_fold_or_hold_out() is implemented as shown above. In contrast to the hold-out setting, it is called for each of the 𝑘 folds. The results are stored in
+a dictionaries metric_values and loss_values as follows:
+
+# Validate fold: use only loss for tuning
+metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_f
+df_eval = sum(loss_values.values()) / len(loss_values.values())
+The results are averaged over the 𝑘 folds and returned as df_eval.
+
+40
+
+6.2.4 Detailed Description of the "test_cv" Setting
+It uses the loss function specfied in fun_control and the metric specified in fun_control.
+1. First, the method HyperTorch().fun_torch is called.
+2. fun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:
+df_eval, _ = evaluate_cv(
+model,
+dataset=fun_control["test"],
+shuffle=self.fun_control["shuffle"],
+device=self.fun_control["device"],
+show_batch_interval=self.fun_control["show_batch_interval"],
+)
+Note: The data set fun_control["test"] is used for CV. The rest is the same as for the
+"train_cv" setting.
+6.2.5 Detailed Description of the Final Model Training and Evaluation
+6.2.5.1 Detailed Description of the "train_tuned Procedure
+train_tuned() is just a wrapper to evaluate_hold_out using the train data set. It is
+implemented as follows:
+
+def train_tuned(net, train_dataset, shuffle, loss_function, metric, device=None, show_batch_i
+evaluate_hold_out(
+net=net,
+train_dataset=train_dataset,
+shuffle=shuffle,
+test_dataset=None,
+loss_function=loss_function,
+metric=metric,
+device=device,
+show_batch_interval=show_batch_interval,
+path=path,
+)
+The test_tuned() procedure is implemented as follows:
+
+41
+
+def test_tuned(net, shuffle, test_dataset=None, loss_function=None, metric=None, device=None,
+batch_size_instance = net.batch_size
+removed_attributes, net = get_removed_attributes_and_base_net(net)
+if path is not None:
+net.load_state_dict(torch.load(path))
+net.eval()
+try:
+device = getDevice(device=device)
+if torch.cuda.is_available():
+device = "cuda:0"
+if torch.cuda.device_count() > 1:
+print("We will use", torch.cuda.device_count(), "GPUs!")
+net = nn.DataParallel(net)
+net.to(device)
+valloader = torch.utils.data.DataLoader(
+test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle, num_workers=0
+)
+metric_value, loss = validate_fold_or_hold_out(
+net, valloader=valloader, loss_function=loss_function, metric=metric, device=devi
+)
+df_eval = loss
+df_metric = metric_value
+df_preds = np.nan
+except Exception as err:
+print(f"Error in Net_Core. Call to test_tuned() failed. {err=}, {type(err)=}")
+df_eval = np.nan
+df_metric = np.nan
+df_preds = np.nan
+add_attributes(net, removed_attributes)
+print(f"Final evaluation: Validation loss: {df_eval}")
+print(f"Final evaluation: Validation metric: {df_metric}")
+print("----------------------------------------------")
+return df_eval, df_preds, df_metric
+
+42
+
 References
 Bartz, Eva, Thomas Bartz-Beielstein, Martin Zaefferer, and Olaf Mersmann, eds. 2022. Hyperparameter Tuning for Machine and Deep Learning with R - A Practical Guide. Springer.
 Bartz-Beielstein, Thomas. 2023. “PyTorch Hyperparameter Tuning with SPOT: Comparison
 with Ray Tuner and Default Hyperparameters on CIFAR10.” https://github.com/sequent
 ial-parameter-optimization/spotPython/blob/main/notebooks/14_spot_ray_hpt_torc
 h_cifar10.ipynb.
 Bartz-Beielstein, Thomas, Jürgen Branke, Jörn Mehnen, and Olaf Mersmann. 2014. “Evolutionary Algorithms.” Wiley Interdisciplinary Reviews: Data Mining and Knowledge Discovery 4 (3): 178–95.
@@ -1819,10 +1937,10 @@
 Robin Vaysse, Adil Zouitine, et al. 2021. “River: Machine Learning for Streaming Data in
 Python.”
 PyTorch. 2023a. “Hyperparameter Tuning with Ray Tune.” https://pytorch.org/tutorials/be
 ginner/hyperparameter_tuning_tutorial.html.
 ———. 2023b. “Training a Classifier.” https://pytorch.org/tutorials/beginner/blitz/cifar10
 _tutorial.html.
 
-40
+43
```

### Comparing `spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png` & `spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png` & `spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png` & `spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png` & `spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png` & `spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png` & `spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png` & `spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png` & `spotPython-0.2.2/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/figures/parallel.png` & `spotPython-0.2.2/docs/figures/parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/img/spotLogo.png` & `spotPython-0.2.2/docs/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/search.json` & `spotPython-0.2.2/docs/search.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.905263157894737%*

 * *Differences: {'0': "{'text': 'Hyperparameter tuning is an important, but often difficult and computationally "*

 * *      'intensive task. Changing the architecture of a neural network or the learning rate of an '*

 * *      'optimizer can have a significant impact on the performance.\\nThe goal of hyperparameter '*

 * *      'tuning is to optimize the hyperparameters in a way that improves the performance of the '*

 * *      'machine learning or deep learning model. The simplest, but also most computationally '*

 * *      'expensive, approach  […]*

```diff
@@ -1,13 +1,13 @@
 [
     {
         "href": "bart23e.html",
         "objectID": "bart23e.html",
         "section": "",
-        "text": "Hyperparameter tuning is an important, but often difficult and computationally intensive task. Changing the architecture of a neural network or the learning rate of an optimizer can have a significant impact on the performance.\nThe goal of hyperparameter tuning is to optimize the hyperparameters in a way that improves the performance of the machine learning or deep learning model. The simplest, but also most computationally expensive, approach uses manual search (or trial-and-error (Meignan et al. 2015)). Commonly encountered is simple random search, i.e., random and repeated selection of hyperparameters for evaluation, and lattice search (\u201cgrid search\u201d). In addition, methods that perform directed search and other model-free algorithms, i.e., algorithms that do not explicitly rely on a model, e.g., evolution strategies (Bartz-Beielstein et al. 2014) or pattern search (Lewis, Torczon, and Trosset 2000) play an important role. Also, \u201chyperband\u201d, i.e., a multi-armed bandit strategy that dynamically allocates resources to a set of random configurations and uses successive bisections to stop configurations with poor performance (Li et al. 2016), is very common in hyperparameter tuning. The most sophisticated and efficient approaches are the Bayesian optimization and surrogate model based optimization methods, which are based on the optimization of cost functions determined by simulations or experiments.\nWe consider below a surrogate model based optimization-based hyperparameter tuning approach based on the Python version of the SPOT (\u201cSequential Parameter Optimization Toolbox\u201d) (Bartz-Beielstein, Lasarczyk, and Preuss 2005), which is suitable for situations where only limited resources are available. This may be due to limited availability and cost of hardware, or due to the fact that confidential data may only be processed locally, e.g., due to legal requirements. Furthermore, in our approach, the understanding of algorithms is seen as a key tool for enabling transparency and explainability. This can be enabled, for example, by quantifying the contribution of machine learning and deep learning components (nodes, layers, split decisions, activation functions, etc.). Understanding the importance of hyperparameters and the interactions between multiple hyperparameters plays a major role in the interpretability and explainability of machine learning models. SPOT provides statistical tools for understanding hyperparameters and their interactions. Last but not least, it should be noted that the SPOT software code is available in the open source spotPython package on github1, allowing replicability of the results. This tutorial descries the Python variant of SPOT, which is called spotPython. The R implementation is described in Bartz et al. (2022). SPOT is an established open source software that has been maintained for more than 15 years (Bartz-Beielstein, Lasarczyk, and Preuss 2005) (Bartz et al. 2022).\nThis tutorial is structured as follows. The concept of the hyperparameter tuning software spotPython is described in Section\u00a02. Section\u00a03 describes the integration of spotPython into the PyTorch training workflow and presents the results. Finally, Section\u00a04 presents a summary and an outlook.\n\n\n\n\n\n\nNote\n\n\n\nThe corresponding .ipynb notebook (Bartz-Beielstein 2023) is updated regularly and reflects updates and changes in the spotPython package. It can be downloaded from https://github.com/sequential-parameter-optimization/spotPython/blob/main/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb.",
+        "text": "Hyperparameter tuning is an important, but often difficult and computationally intensive task. Changing the architecture of a neural network or the learning rate of an optimizer can have a significant impact on the performance.\nThe goal of hyperparameter tuning is to optimize the hyperparameters in a way that improves the performance of the machine learning or deep learning model. The simplest, but also most computationally expensive, approach uses manual search (or trial-and-error (Meignan et al. 2015)). Commonly encountered is simple random search, i.e., random and repeated selection of hyperparameters for evaluation, and lattice search (\u201cgrid search\u201d). In addition, methods that perform directed search and other model-free algorithms, i.e., algorithms that do not explicitly rely on a model, e.g., evolution strategies (Bartz-Beielstein et al. 2014) or pattern search (Lewis, Torczon, and Trosset 2000) play an important role. Also, \u201chyperband\u201d, i.e., a multi-armed bandit strategy that dynamically allocates resources to a set of random configurations and uses successive bisections to stop configurations with poor performance (Li et al. 2016), is very common in hyperparameter tuning. The most sophisticated and efficient approaches are the Bayesian optimization and surrogate model based optimization methods, which are based on the optimization of cost functions determined by simulations or experiments.\nWe consider below a surrogate model based optimization-based hyperparameter tuning approach based on the Python version of the SPOT (\u201cSequential Parameter Optimization Toolbox\u201d) (Bartz-Beielstein, Lasarczyk, and Preuss 2005), which is suitable for situations where only limited resources are available. This may be due to limited availability and cost of hardware, or due to the fact that confidential data may only be processed locally, e.g., due to legal requirements. Furthermore, in our approach, the understanding of algorithms is seen as a key tool for enabling transparency and explainability. This can be enabled, for example, by quantifying the contribution of machine learning and deep learning components (nodes, layers, split decisions, activation functions, etc.). Understanding the importance of hyperparameters and the interactions between multiple hyperparameters plays a major role in the interpretability and explainability of machine learning models. SPOT provides statistical tools for understanding hyperparameters and their interactions. Last but not least, it should be noted that the SPOT software code is available in the open source spotPython package on github1, allowing replicability of the results. This tutorial descries the Python variant of SPOT, which is called spotPython. The R implementation is described in Bartz et al. (2022). SPOT is an established open source software that has been maintained for more than 15 years (Bartz-Beielstein, Lasarczyk, and Preuss 2005) (Bartz et al. 2022).\nThis tutorial is structured as follows. The concept of the hyperparameter tuning software spotPython is described in Section\u00a02. Section\u00a03 (\u201cQuickstart\u201d) describes the execution of the example from the tutorial \u201cHyperparameter Tuning with Ray Tune\u201d (PyTorch 2023a). Section\u00a04 describes the integration of spotPython into the PyTorch training workflow in detail and presents the results. Finally, Section\u00a05 presents a summary and an outlook.\n\n\n\n\n\n\nNote\n\n\n\nThe corresponding .ipynb notebook (Bartz-Beielstein 2023) is updated regularly and reflects updates and changes in the spotPython package. It can be downloaded from https://github.com/sequential-parameter-optimization/spotPython/blob/main/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb.",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-setup",
         "objectID": "bart23e.html#sec-setup",
         "section": "Setup",
         "text": "Setup\nBefore we consider the detailed experimental setup, we select the parameters that affect run time, initial design size and the device that is used.\n\nMAX_TIME = 60\nINIT_SIZE = 20\nDEVICE = \"cpu\" # \"cuda:0\"",
@@ -20,50 +20,50 @@
         "text": "Initialization of the fun_control Dictionary\nspotPython uses a Python dictionary for storing the information required for the hyperparameter tuning process. This dictionary is called fun_control and is initialized with the function fun_control_init. The function fun_control_init returns a skeleton dictionary. The dictionary is filled with the required information for the hyperparameter tuning process. It stores the hyperparameter tuning settings, e.g., the deep learning network architecture that should be tuned, the classification (or regression) problem, and the data that is used for the tuning. The dictionary is used as an input for the SPOT function.\n\nfun_control = fun_control_init()",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-data-loading",
         "objectID": "bart23e.html#sec-data-loading",
         "section": "Data Loading",
-        "text": "Data Loading\nThe data loading process is implemented in the same manner as described in the Section \u201cData loaders\u201d in PyTorch (2023a). The data loaders are wrapped into the function load_data. A global data directory is used, which allows sharing the data directory between different trials.\n\ndef load_data(data_dir=\"./data\"):\n    transform = transforms.Compose([\n        transforms.ToTensor(),\n        transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))\n    ])\n\n    trainset = torchvision.datasets.CIFAR10(\n        root=data_dir, train=True, download=True, transform=transform)\n\n    testset = torchvision.datasets.CIFAR10(\n        root=data_dir, train=False, download=True, transform=transform)\n\n    return trainset, testset\n\nThe test and train data are added to the dictionary fun_control.\n\ntrain, test = load_data()\nn_samples = len(train)\n# add the dataset to the fun_control\nfun_control.update({\n    \"train\": train,\n    \"test\": test,\n    \"n_samples\": n_samples})",
+        "text": "Data Loading\nThe data loading process is implemented in the same manner as described in the Section \u201cData loaders\u201d in PyTorch (2023a). The data loaders are wrapped into the function load_data_cifar10 which is identical to the function load_data in PyTorch (2023a). A global data directory is used, which allows sharing the data directory between different trials.\n\ndef load_data_cifar10(data_dir=\"./data\"):\n    transform = transforms.Compose([\n        transforms.ToTensor(),\n        transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))\n    ])\n\n    trainset = torchvision.datasets.CIFAR10(\n        root=data_dir, train=True, download=True, transform=transform)\n\n    testset = torchvision.datasets.CIFAR10(\n        root=data_dir, train=False, download=True, transform=transform)\n\n    return trainset, testset\n\nThe method load_data_cifar10 is part of the spotPython package and can be imported from spotPython.data.torchdata.\nIn the following step, the test and train data are added to the dictionary fun_control.\n\ntrain, test = load_data_cifar10()\nn_samples = len(train)\n# add the dataset to the fun_control\nfun_control.update({\n    \"train\": train,\n    \"test\": test,\n    \"n_samples\": n_samples})",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-specification-of-preprocessing-model",
         "objectID": "bart23e.html#sec-specification-of-preprocessing-model",
         "section": "Specification of the Preprocessing Model",
         "text": "Specification of the Preprocessing Model\nAfter the training and test data are specified and added to the fun_control dictionary, spotPython allows the specification of a data preprocessing pipeline, e.g., for the scaling of the data or for the one-hot encoding of categorical variables. The preprocessing model is called prep_model (\u201cpreparation\u201d or pre-processing) and includes steps that are not subject to the hyperparameter tuning process. The preprocessing model is specified in the fun_control dictionary. The preprocessing model can be implemented as a sklearn pipeline. The following code shows a typical preprocessing pipeline:\ncategorical_columns = [\"cities\", \"colors\"]\none_hot_encoder = OneHotEncoder(handle_unknown=\"ignore\",\n                                    sparse_output=False)\nprep_model = ColumnTransformer(\n        transformers=[\n             (\"categorical\", one_hot_encoder, categorical_columns),\n         ],\n         remainder=StandardScaler(),\n     )\nBecause the Ray Tune (ray[tune]) hyperparameter tuning as described in PyTorch (2023a) does not use a preprocessing model, the preprocessing model is set to None here.\n\nprep_model = None\nfun_control.update({\"prep_model\": prep_model})",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-selection-of-the-algorithm",
         "objectID": "bart23e.html#sec-selection-of-the-algorithm",
         "section": "Select algorithm and core_model_hyper_dict",
-        "text": "Select algorithm and core_model_hyper_dict\nThe same neural network model as implemented in the section \u201cConfigurable neural network\u201d of the PyTorch tutorial (PyTorch 2023a) is used here. We will show the implementation from PyTorch (2023a) in Section\u00a03.5.1 first, before the extended implementation with spotPython is shown in Section\u00a03.5.2.\n\nImplementing a Configurable Neural Network With Ray Tune\nWe used the same hyperparameters that are implemented as configurable in the PyTorch tutorial. We specify the layer sizes, namely l1 and l2, of the fully connected layers:\nclass Net(nn.Module):\n    def __init__(self, l1=120, l2=84):\n        super(Net, self).__init__()\n        self.conv1 = nn.Conv2d(3, 6, 5)\n        self.pool = nn.MaxPool2d(2, 2)\n        self.conv2 = nn.Conv2d(6, 16, 5)\n        self.fc1 = nn.Linear(16 * 5 * 5, l1)\n        self.fc2 = nn.Linear(l1, l2)\n        self.fc3 = nn.Linear(l2, 10)\n\n    def forward(self, x):\n        x = self.pool(F.relu(self.conv1(x)))\n        x = self.pool(F.relu(self.conv2(x)))\n        x = x.view(-1, 16 * 5 * 5)\n        x = F.relu(self.fc1(x))\n        x = F.relu(self.fc2(x))\n        x = self.fc3(x)\n        return x\n\nThe learning rate, i.e., lr, of the optimizer is made configurable, too:\noptimizer = optim.SGD(net.parameters(), lr=config[\"lr\"], momentum=0.9)\n\n\nImplementing a Configurable Neural Network With spotPython\nspotPython implements a class which is similar to the class described in the PyTorch tutorial. The class is called Net_CIFAR10 and is implemented in the file netcifar10.py.\nimport spotPython.torch.netcore as netcore\nclass Net_CIFAR10(netcore.Net_Core):\n    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience):\n        super(Net_CIFAR10, self).__init__(\n            lr_mult=lr_mult, batch_size=batch_size, epochs=epochs, k_folds=k_folds,\n            patience=patience\n        )\n        self.conv1 = nn.Conv2d(3, 6, 5)\n        self.pool = nn.MaxPool2d(2, 2)\n        self.conv2 = nn.Conv2d(6, 16, 5)\n        self.fc1 = nn.Linear(16 * 5 * 5, l1)\n        self.fc2 = nn.Linear(l1, l2)\n        self.fc3 = nn.Linear(l2, 10)\n\n    def forward(self, x):\n        x = self.pool(F.relu(self.conv1(x)))\n        x = self.pool(F.relu(self.conv2(x)))\n        x = x.view(-1, 16 * 5 * 5)\n        x = F.relu(self.fc1(x))\n        x = F.relu(self.fc2(x))\n        x = self.fc3(x)\n        return x\nNet_CIFAR10 inherits from the class Net_Core which is implemented in the file netcore.py. It implements the additional attributes that are common to all neural network models. The attributes are the learning rate multiplier lr_mult, the batch size batch_size, the number of epochs epochs, the number of folds k_folds for the cross validation, and the patience patience for the early stopping. The class Net_Core is shown below.\nfrom torch import nn\n\n\nclass Net_Core(nn.Module):\n    def __init__(self, lr_mult, batch_size, epochs, k_folds, patience):\n        super(Net_Core, self).__init__()\n        self.lr_mult = lr_mult\n        self.batch_size = batch_size\n        self.epochs = epochs\n        self.k_folds = k_folds\n        self.patience = patience\n\n\nComparison of the Approach Described in the PyTorch Tutorial With spotPython\nComparing the class Net from the PyTorch tutorial and the class Net_CIFAR10 from spotPython, we see that the class Net_CIFAR10 has additional attributes and does not inherit from nn directly. It adds an additional class, Net_core, that takes care of additional attributes that are common to all neural network models, e.g., the learning rate multiplier lr_mult or the batch size batch_size.\nspotPython\u2019s core_model implements an instance of the Net_CIFAR10 class. In addition to the basic neural network model, the core_model can use these additional attributes. spotPython provides methods for handling these additional attributes to guarantee 100% compatibility with the PyTorch classes. The method add_core_model_to_fun_control adds the hyperparameters and additional attributes to the fun_control dictionary. The method is shown below.\n\ncore_model = Net_CIFAR10\nfun_control = add_core_model_to_fun_control(core_model=core_model,\n                              fun_control=fun_control,\n                              hyper_dict=TorchHyperDict,\n                              filename=None)\n\n\n\n\n\n\n\nNote\n\n\n\nIn addition to the class Net from the PyTorch tutorial, the class Net_CIFAR10 has additional attributes, e.g.:\n\nlearning rate (lr),\nbatch size (batch_size),\nepochs (epochs),\nk_folds (k_folds), and\nearly stopping criterion \u201cpatience\u201d (patience)\n\nFurther attributes can be easily added to the class, e.g., optimizer.",
+        "text": "Select algorithm and core_model_hyper_dict\nThe same neural network model as implemented in the section \u201cConfigurable neural network\u201d of the PyTorch tutorial (PyTorch 2023a) is used here. We will show the implementation from PyTorch (2023a) in Section\u00a04.5.1 first, before the extended implementation with spotPython is shown in Section\u00a04.5.2.\n\nImplementing a Configurable Neural Network With Ray Tune\nWe used the same hyperparameters that are implemented as configurable in the PyTorch tutorial. We specify the layer sizes, namely l1 and l2, of the fully connected layers:\nclass Net(nn.Module):\n    def __init__(self, l1=120, l2=84):\n        super(Net, self).__init__()\n        self.conv1 = nn.Conv2d(3, 6, 5)\n        self.pool = nn.MaxPool2d(2, 2)\n        self.conv2 = nn.Conv2d(6, 16, 5)\n        self.fc1 = nn.Linear(16 * 5 * 5, l1)\n        self.fc2 = nn.Linear(l1, l2)\n        self.fc3 = nn.Linear(l2, 10)\n\n    def forward(self, x):\n        x = self.pool(F.relu(self.conv1(x)))\n        x = self.pool(F.relu(self.conv2(x)))\n        x = x.view(-1, 16 * 5 * 5)\n        x = F.relu(self.fc1(x))\n        x = F.relu(self.fc2(x))\n        x = self.fc3(x)\n        return x\n\nThe learning rate, i.e., lr, of the optimizer is made configurable, too:\noptimizer = optim.SGD(net.parameters(), lr=config[\"lr\"], momentum=0.9)\n\n\nImplementing a Configurable Neural Network With spotPython\nspotPython implements a class which is similar to the class described in the PyTorch tutorial. The class is called Net_CIFAR10 and is implemented in the file netcifar10.py.\nfrom torch import nn\nimport torch.nn.functional as F\nimport spotPython.torch.netcore as netcore\n\n\nclass Net_CIFAR10(netcore.Net_Core):\n    def __init__(self, l1, l2, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd_momentum):\n        super(Net_CIFAR10, self).__init__(\n            lr_mult=lr_mult,\n            batch_size=batch_size,\n            epochs=epochs,\n            k_folds=k_folds,\n            patience=patience,\n            optimizer=optimizer,\n            sgd_momentum=sgd_momentum,\n        )\n        self.conv1 = nn.Conv2d(3, 6, 5)\n        self.pool = nn.MaxPool2d(2, 2)\n        self.conv2 = nn.Conv2d(6, 16, 5)\n        self.fc1 = nn.Linear(16 * 5 * 5, l1)\n        self.fc2 = nn.Linear(l1, l2)\n        self.fc3 = nn.Linear(l2, 10)\n\n    def forward(self, x):\n        x = self.pool(F.relu(self.conv1(x)))\n        x = self.pool(F.relu(self.conv2(x)))\n        x = x.view(-1, 16 * 5 * 5)\n        x = F.relu(self.fc1(x))\n        x = F.relu(self.fc2(x))\n        x = self.fc3(x)\n        return x\nNet_CIFAR10 inherits from the class Net_Core which is implemented in the file netcore.py. It implements the additional attributes that are common to all neural network models. The attributes are the learning rate multiplier lr_mult, the batch size batch_size, the number of epochs epochs, the number of folds k_folds for the cross validation, and the patience patience for the early stopping. The class Net_Core is shown below.\nfrom torch import nn\n\n\nclass Net_Core(nn.Module):\n    def __init__(self, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd_momentum):\n        super(Net_Core, self).__init__()\n        self.lr_mult = lr_mult\n        self.batch_size = batch_size\n        self.epochs = epochs\n        self.k_folds = k_folds\n        self.patience = patience\n        self.optimizer = optimizer\n        self.sgd_momentum = sgd_momentum\n\n\n\n\n\n\nThe Net_Core class\n\n\n\nThe Net_Core class is implemented in the file netcore.py. It implements hyperparameters as attributes, that are not used by the core_model, e.g.:\n\noptimizer (optimizer),\nlearning rate (lr),\nbatch size (batch_size),\nepochs (epochs),\nk_folds (k_folds), and\nearly stopping criterion \u201cpatience\u201d (patience).\n\nUsers can add further attributes to the class.\n\n\n\n\nComparison of the Approach Described in the PyTorch Tutorial With spotPython\nComparing the class Net from the PyTorch tutorial and the class Net_CIFAR10 from spotPython, we see that the class Net_CIFAR10 has additional attributes and does not inherit from nn directly. It adds an additional class, Net_core, that takes care of additional attributes that are common to all neural network models, e.g., the learning rate multiplier lr_mult or the batch size batch_size.\nspotPython\u2019s core_model implements an instance of the Net_CIFAR10 class. In addition to the basic neural network model, the core_model can use these additional attributes. spotPython provides methods for handling these additional attributes to guarantee 100% compatibility with the PyTorch classes. The method add_core_model_to_fun_control adds the hyperparameters and additional attributes to the fun_control dictionary. The method is shown below.\n\ncore_model = Net_CIFAR10\nfun_control = add_core_model_to_fun_control(core_model=core_model,\n                              fun_control=fun_control,\n                              hyper_dict=TorchHyperDict,\n                              filename=None)",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-search-space",
         "objectID": "bart23e.html#sec-search-space",
         "section": "The Search Space",
-        "text": "The Search Space\nIn Section\u00a03.6.1, we first describe how to configure the search space with ray[tune] (as shown in PyTorch (2023a)) and then how to configure the search space with spotPython in Section\u00a03.6.2.\n\nConfiguring the Search Space With Ray Tune\nRay Tune\u2019s search space can be configured as follows (PyTorch 2023a):\nconfig = {\n    \"l1\": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),\n    \"l2\": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),\n    \"lr\": tune.loguniform(1e-4, 1e-1),\n    \"batch_size\": tune.choice([2, 4, 8, 16])\n}\nThe tune.sample_from() function enables the user to define sample methods to obtain hyperparameters. In this example, the l1 and l2 parameters should be powers of 2 between 4 and 256, so either 4, 8, 16, 32, 64, 128, or 256. The lr (learning rate) should be uniformly sampled between 0.0001 and 0.1. Lastly, the batch size is a choice between 2, 4, 8, and 16.\nAt each trial, ray[tune] will randomly sample a combination of parameters from these search spaces. It will then train a number of models in parallel and find the best performing one among these. ray[tune] uses the ASHAScheduler which will terminate bad performing trials early.\n\n\nConfiguring the Search Space With spotPython\n\nThe hyper_dict Hyperparameters for the Selected Algorithm\nspotPython uses simple JSON files for the specification of the hyperparameters. Users can specify their individual JSON files, or they can use the JSON files provided by spotPython. The JSON file for the core_model is called torch_hyper_dict.json.\nIn contrast to ray[tune], spotPython can handle numerical, boolean, and categorical hyperparameters. They can be specified in the JSON file in a similar way as the numerical hyperparameters as shown below:\n\"factor_hyperparameter\": {\n    \"levels\": [\"A\", \"B\", \"C\"],\n    \"type\": \"factor\",\n    \"default\": \"B\",\n    \"transform\": \"None\",\n    \"core_model_parameter_type\": \"str\",\n    \"lower\": 0,\n    \"upper\": 2},\nEach entry in the JSON file represents one hyperparameter with the following structure: type, default, transform, lower, and upper. The corresponding entries for the Net_CIFAR10 class are shown below.\n{\"Net_CIFAR10\":\n    {\n        \"l1\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 2,\n            \"upper\": 9},\n        \"l2\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 2,\n            \"upper\": 9},\n        \"lr_mult\": {\n            \"type\": \"float\",\n            \"default\": 1.0,\n            \"transform\": \"None\",\n            \"lower\": 0.1,\n            \"upper\": 10},\n        \"batch_size\": {\n            \"type\": \"int\",\n            \"default\": 4,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 1,\n            \"upper\": 4},\n        \"epochs\": {\n            \"type\": \"int\",\n            \"default\": 3,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 1,\n            \"upper\": 4},\n        \"k_folds\": {\n            \"type\": \"int\",\n            \"default\": 2,\n            \"transform\": \"None\",\n            \"lower\": 2,\n            \"upper\": 3},\n        \"patience\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"None\",\n            \"lower\": 2,\n            \"upper\": 10},\n        \"optimizer\": {\n            \"levels\": [\"Adadelta\",\n                       \"Adagrad\",\n                       \"Adam\",\n                       \"AdamW\",\n                       \"SparseAdam\",\n                       \"Adamax\",\n                       \"ASGD\",\n                       \"LBFGS\",\n                       \"NAdam\",\n                       \"RAdam\",\n                       \"RMSprop\",\n                       \"Rprop\",\n                       \"SGD\"],\n            \"type\": \"factor\",\n            \"default\": \"SGD\",\n            \"transform\": \"None\",\n            \"class_name\": \"torch.optim\",\n            \"core_model_parameter_type\": \"str\",\n            \"lower\": 0,\n            \"upper\": 12},\n        \"sgd_momentum\": {\n            \"type\": \"float\",\n            \"default\": 0.0,\n            \"transform\": \"None\",\n            \"lower\": 0.0,\n            \"upper\": 1.0}\n    }\n}",
+        "text": "The Search Space\nIn Section\u00a04.6.1, we first describe how to configure the search space with ray[tune] (as shown in PyTorch (2023a)) and then how to configure the search space with spotPython in Section\u00a04.6.2.\n\nConfiguring the Search Space With Ray Tune\nRay Tune\u2019s search space can be configured as follows (PyTorch 2023a):\nconfig = {\n    \"l1\": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),\n    \"l2\": tune.sample_from(lambda _: 2**np.random.randint(2, 9)),\n    \"lr\": tune.loguniform(1e-4, 1e-1),\n    \"batch_size\": tune.choice([2, 4, 8, 16])\n}\nThe tune.sample_from() function enables the user to define sample methods to obtain hyperparameters. In this example, the l1 and l2 parameters should be powers of 2 between 4 and 256, so either 4, 8, 16, 32, 64, 128, or 256. The lr (learning rate) should be uniformly sampled between 0.0001 and 0.1. Lastly, the batch size is a choice between 2, 4, 8, and 16.\nAt each trial, ray[tune] will randomly sample a combination of parameters from these search spaces. It will then train a number of models in parallel and find the best performing one among these. ray[tune] uses the ASHAScheduler which will terminate bad performing trials early.\n\n\nConfiguring the Search Space With spotPython\n\nThe hyper_dict Hyperparameters for the Selected Algorithm\nspotPython uses JSON files for the specification of the hyperparameters. Users can specify their individual JSON files, or they can use the JSON files provided by spotPython. The JSON file for the core_model is called torch_hyper_dict.json.\nIn contrast to ray[tune], spotPython can handle numerical, boolean, and categorical hyperparameters. They can be specified in the JSON file in a similar way as the numerical hyperparameters as shown below. Each entry in the JSON file represents one hyperparameter with the following structure: type, default, transform, lower, and upper.\n\"factor_hyperparameter\": {\n    \"levels\": [\"A\", \"B\", \"C\"],\n    \"type\": \"factor\",\n    \"default\": \"B\",\n    \"transform\": \"None\",\n    \"core_model_parameter_type\": \"str\",\n    \"lower\": 0,\n    \"upper\": 2},\nThe corresponding entries for the Net_CIFAR10 class are shown below.\n{\"Net_CIFAR10\":\n    {\n        \"l1\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 2,\n            \"upper\": 9},\n        \"l2\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 2,\n            \"upper\": 9},\n        \"lr_mult\": {\n            \"type\": \"float\",\n            \"default\": 1.0,\n            \"transform\": \"None\",\n            \"lower\": 0.1,\n            \"upper\": 10},\n        \"batch_size\": {\n            \"type\": \"int\",\n            \"default\": 4,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 1,\n            \"upper\": 4},\n        \"epochs\": {\n            \"type\": \"int\",\n            \"default\": 3,\n            \"transform\": \"transform_power_2_int\",\n            \"lower\": 1,\n            \"upper\": 4},\n        \"k_folds\": {\n            \"type\": \"int\",\n            \"default\": 2,\n            \"transform\": \"None\",\n            \"lower\": 2,\n            \"upper\": 3},\n        \"patience\": {\n            \"type\": \"int\",\n            \"default\": 5,\n            \"transform\": \"None\",\n            \"lower\": 2,\n            \"upper\": 10},\n        \"optimizer\": {\n            \"levels\": [\"Adadelta\",\n                       \"Adagrad\",\n                       \"Adam\",\n                       \"AdamW\",\n                       \"SparseAdam\",\n                       \"Adamax\",\n                       \"ASGD\",\n                       \"LBFGS\",\n                       \"NAdam\",\n                       \"RAdam\",\n                       \"RMSprop\",\n                       \"Rprop\",\n                       \"SGD\"],\n            \"type\": \"factor\",\n            \"default\": \"SGD\",\n            \"transform\": \"None\",\n            \"class_name\": \"torch.optim\",\n            \"core_model_parameter_type\": \"str\",\n            \"lower\": 0,\n            \"upper\": 12},\n        \"sgd_momentum\": {\n            \"type\": \"float\",\n            \"default\": 0.0,\n            \"transform\": \"None\",\n            \"lower\": 0.0,\n            \"upper\": 1.0}\n    }\n}",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-modification-of-hyperparameters",
         "objectID": "bart23e.html#sec-modification-of-hyperparameters",
         "section": "Modifying the Hyperparameters",
-        "text": "Modifying the Hyperparameters\nRay tune (PyTorch 2023a) does not provide a way to change the specified hyperparameters without re-compilation. However, spotPython provides functions for modifying the hyperparameters, their bounds and factors as well as for activating and de-activating hyperparameters without re-compilation of the Python source code. These functions are described in the following.\n\nModify hyper_dict Hyperparameters for the Selected Algorithm aka core_model\nAfter specifying the model, the corresponding hyperparameters, their types and bounds are loaded from the JSON file torch_hyper_dict.json. After loading, the user can modify the hyperparameters, e.g., the bounds. spotPython provides a simple rule for de-activating hyperparameters: If the lower and the upper bound are set to identical values, the hyperparameter is de-activated. This is useful for the hyperparameter tuning, because it allows to specify a hyperparameter in the JSON file, but to de-activate it in the fun_control dictionary. This is done in the next step.\n\n\nModify Hyperparameters of Type numeric and integer (boolean)\nSince the hyperparameter k_folds is not used in the PyTorch tutorial, it is de-activated here by setting the lower and upper bound to the same value. Note, k_folds is of type \u201cinteger\u201d.\n\nfun_control = modify_hyper_parameter_bounds(fun_control, \"batch_size\", bounds=[1, 5])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"k_folds\", bounds=[0, 0])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"patience\", bounds=[3, 3])\nfun_control[\"core_model_hyper_dict\"]\n\n\n\nModify Hyperparameter of Type factor\nIn a similar manner as for the numerical hyperparameters, the categorical hyperparameters can be modified. New configurations can be chosen by adding or deleting levels. For example, the hyperparameter optimizer can be re-configured as follows:\nIn the following setting, two optimizers (\"SGD\" and \"Adam\") will be compared during the spotPython hyperparameter tuning. The hyperparameter optimizer is active.\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\", [\"SGD\", \"Adam\"])\n\nThe hyperparameter optimizer can be de-activated by choosing only one value (level), here: \"SGD\".\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\", [\"SGD\"])\n\nAs discussed in Section\u00a03.7.4, there are some issues with the LBFGS optimizer. Therefore, the usage of the LBFGS optimizer is not deactivated in spotPython by default. However, the LBFGS optimizer can be activated by adding it to the list of optimizers. Rprop was removed, because it does perform very poorly (as some pre-tests have shown). However, it can also be activated by adding it to the list of optimizers. Since SparseAdam does not support dense gradients, Adam was used instead. Therefore, there are 10 default optimizers:\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\",[\"Adadelta\",\n     \"Adagrad\", \"Adam\", \"AdamW\", \"Adamax\", \"ASGD\", \"NAdam\", \"RAdam\",\n      \"RMSprop\", \"SGD\"])\n\n\n\nOptimizers\nTable\u00a01 shows some of the optimizers available in PyTorch:\n\n\nTable\u00a01: Optimizers available in PyTorch (selection). \u201cmom\u201d denotes momentum, \u201cweight\u201d weight_decay, \u201cdamp\u201d dampening, \u201cnest\u201d nesterov, \u201clr_sc\u201d learning rate for scaling delta, \u201cmom_dec\u201d for momentum_decay, and \u201cstep_s\u201d for step_sizes. The default values are shown in the table.\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\nOptimizer\nlr\nmom\nweight\ndamp\nnest\nrho\nlr_sc\nlr_decay\nbetas\nlambd\nalpha\nmom_decay\netas\nstep_s\n\n\n\n\nAdadelta\n-\n-\n0.\n-\n-\n0.9\n1.0\n-\n-\n-\n-\n-\n-\n-\n\n\nAdagrad\n1e-2\n-\n0.\n-\n-\n-\n-\n0.\n-\n-\n-\n-\n-\n-\n\n\nAdam\n1e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nAdamW\n1e-3\n-\n1e-2\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nSparseAdam\n1e-3\n-\n-\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nAdamax\n2e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9, 0.999)\n-\n-\n-\n-\n-\n\n\nASGD\n1e-2\n0.9\n0.\n-\nFalse\n-\n-\n-\n-\n1e-4\n0.75\n-\n-\n-\n\n\nLBFGS\n1.\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n\n\nNAdam\n2e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n0\n-\n-\n\n\nRAdam\n1e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nRMSprop\n1e-2\n0.\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nRprop\n1e-2\n-\n-\n-\n-\n-\n-\n-\n-\n-\n(0.5,1.2)\n(1e-6, 50)\n-\n-\n\n\nSGD\nrequired\n0.\n0.\n0.\nFalse\n-\n-\n-\n-\n-\n-\n-\n-\n-\n\n\n\n\nspotPython implements an optimization handler that maps the optimizer names to the corresponding PyTorch optimizers.\n\n\n\n\n\n\nA note on LBFGS\n\n\n\nWe recommend deactivating PyTorch\u2019s LBFGS optimizer, because it does not perform very well. The PyTorch documentation, see https://pytorch.org/docs/stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS, states:\n\nThis is a very memory intensive optimizer (it requires additional param_bytes * (history_size + 1) bytes). If it doesn\u2019t fit in memory try reducing the history size, or use a different algorithm.\n\nFurthermore, the LBFGS optimizer is not compatible with the PyTorch tutorial. The reason is that the LBFGS optimizer requires the closure function, which is not implemented in the PyTorch tutorial. Therefore, the LBFGS optimizer is recommended here.\n\n\nSince there are 10 optimizers in the portfolio, it is not recommended tuning the hyperparameters that effect one single optimizer only.\n\n\n\n\n\n\nA note on the learning rate\n\n\n\nspotPython provides a multiplier for the default learning rates, because optimizers use different learning rates. Using a multiplier for the learning rates might enable a simultaneous tuning of the learning rates for all optimizers. However, this is not recommended, because the learning rates are not comparable across optimizers. Therefore, we recommend fixing the learning rate for all optimizers if multiple optimizers are used. This can be done by setting the lower and upper bounds of the learning rate multiplier to the same value as shown below.\n\n\nThus, the learning rate, which affects the SGD optimizer, will be set to a fixed value. We choose the default value of 1e-3 for the learning rate, because it is used in other PyTorch examples (it is also the default value used by spotPython as defined in the optimizer_handler() method). We recommend tuning the learning rate later, when a reduced set of optimizers is fixed. Here, we will demonstrate how to select in a screening phase the optimizers that should be used for the hyperparameter tuning.\nFor the same reason, we will fix the sgd_momentum to 0.9.\n\nfun_control = modify_hyper_parameter_bounds(fun_control, \"lr_mult\", bounds=[1.0, 1.0])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"sgd_momentum\", bounds=[0.9, 0.9])",
+        "text": "Modifying the Hyperparameters\nRay tune (PyTorch 2023a) does not provide a way to change the specified hyperparameters without re-compilation. However, spotPython provides functions for modifying the hyperparameters, their bounds and factors as well as for activating and de-activating hyperparameters without re-compilation of the Python source code. These functions are described in the following.\n\nModify hyper_dict Hyperparameters for the Selected Algorithm aka core_model\nAfter specifying the model, the corresponding hyperparameters, their types and bounds are loaded from the JSON file torch_hyper_dict.json. After loading, the user can modify the hyperparameters, e.g., the bounds. spotPython provides a simple rule for de-activating hyperparameters: If the lower and the upper bound are set to identical values, the hyperparameter is de-activated. This is useful for the hyperparameter tuning, because it allows to specify a hyperparameter in the JSON file, but to de-activate it in the fun_control dictionary. This is done in the next step.\n\n\nModify Hyperparameters of Type numeric and integer (boolean)\nSince the hyperparameter k_folds is not used in the PyTorch tutorial, it is de-activated here by setting the lower and upper bound to the same value. Note, k_folds is of type \u201cinteger\u201d.\n\nfun_control = modify_hyper_parameter_bounds(fun_control, \"batch_size\", bounds=[1, 5])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"k_folds\", bounds=[0, 0])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"patience\", bounds=[3, 3])\nfun_control[\"core_model_hyper_dict\"]\n\n\n\nModify Hyperparameter of Type factor\nIn a similar manner as for the numerical hyperparameters, the categorical hyperparameters can be modified. New configurations can be chosen by adding or deleting levels. For example, the hyperparameter optimizer can be re-configured as follows:\nIn the following setting, two optimizers (\"SGD\" and \"Adam\") will be compared during the spotPython hyperparameter tuning. The hyperparameter optimizer is active.\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\", [\"SGD\", \"Adam\"])\n\nThe hyperparameter optimizer can be de-activated by choosing only one value (level), here: \"SGD\".\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\", [\"SGD\"])\n\nAs discussed in Section\u00a04.7.4, there are some issues with the LBFGS optimizer. Therefore, the usage of the LBFGS optimizer is not deactivated in spotPython by default. However, the LBFGS optimizer can be activated by adding it to the list of optimizers. Rprop was removed, because it does perform very poorly (as some pre-tests have shown). However, it can also be activated by adding it to the list of optimizers. Since SparseAdam does not support dense gradients, Adam was used instead. Therefore, there are 10 default optimizers:\n\nfun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\",[\"Adadelta\",\n     \"Adagrad\", \"Adam\", \"AdamW\", \"Adamax\", \"ASGD\", \"NAdam\", \"RAdam\",\n      \"RMSprop\", \"SGD\"])\n\n\n\nOptimizers\nTable\u00a01 shows some of the optimizers available in PyTorch:\n\n\nTable\u00a01: Optimizers available in PyTorch (selection). \u201cmom\u201d denotes momentum, \u201cweight\u201d weight_decay, \u201cdamp\u201d dampening, \u201cnest\u201d nesterov, \u201clr_sc\u201d learning rate for scaling delta, \u201cmom_dec\u201d for momentum_decay, and \u201cstep_s\u201d for step_sizes. The default values are shown in the table.\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\nOptimizer\nlr\nmom\nweight\ndamp\nnest\nrho\nlr_sc\nlr_decay\nbetas\nlambd\nalpha\nmom_decay\netas\nstep_s\n\n\n\n\nAdadelta\n-\n-\n0.\n-\n-\n0.9\n1.0\n-\n-\n-\n-\n-\n-\n-\n\n\nAdagrad\n1e-2\n-\n0.\n-\n-\n-\n-\n0.\n-\n-\n-\n-\n-\n-\n\n\nAdam\n1e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nAdamW\n1e-3\n-\n1e-2\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nSparseAdam\n1e-3\n-\n-\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nAdamax\n2e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9, 0.999)\n-\n-\n-\n-\n-\n\n\nASGD\n1e-2\n0.9\n0.\n-\nFalse\n-\n-\n-\n-\n1e-4\n0.75\n-\n-\n-\n\n\nLBFGS\n1.\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n-\n\n\nNAdam\n2e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n0\n-\n-\n\n\nRAdam\n1e-3\n-\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nRMSprop\n1e-2\n0.\n0.\n-\n-\n-\n-\n-\n(0.9,0.999)\n-\n-\n-\n-\n-\n\n\nRprop\n1e-2\n-\n-\n-\n-\n-\n-\n-\n-\n-\n(0.5,1.2)\n(1e-6, 50)\n-\n-\n\n\nSGD\nrequired\n0.\n0.\n0.\nFalse\n-\n-\n-\n-\n-\n-\n-\n-\n-\n\n\n\n\nspotPython implements an optimization handler that maps the optimizer names to the corresponding PyTorch optimizers.\n\n\n\n\n\n\nA note on LBFGS\n\n\n\nWe recommend deactivating PyTorch\u2019s LBFGS optimizer, because it does not perform very well. The PyTorch documentation, see https://pytorch.org/docs/stable/generated/torch.optim.LBFGS.html#torch.optim.LBFGS, states:\n\nThis is a very memory intensive optimizer (it requires additional param_bytes * (history_size + 1) bytes). If it doesn\u2019t fit in memory try reducing the history size, or use a different algorithm.\n\nFurthermore, the LBFGS optimizer is not compatible with the PyTorch tutorial. The reason is that the LBFGS optimizer requires the closure function, which is not implemented in the PyTorch tutorial. Therefore, the LBFGS optimizer is recommended here.\n\n\nSince there are 10 optimizers in the portfolio, it is not recommended tuning the hyperparameters that effect one single optimizer only.\n\n\n\n\n\n\nA note on the learning rate\n\n\n\nspotPython provides a multiplier for the default learning rates, lr_mult, because optimizers use different learning rates. Using a multiplier for the learning rates might enable a simultaneous tuning of the learning rates for all optimizers. However, this is not recommended, because the learning rates are not comparable across optimizers. Therefore, we recommend fixing the learning rate for all optimizers if multiple optimizers are used. This can be done by setting the lower and upper bounds of the learning rate multiplier to the same value as shown below.\n\n\nThus, the learning rate, which affects the SGD optimizer, will be set to a fixed value. We choose the default value of 1e-3 for the learning rate, because it is used in other PyTorch examples (it is also the default value used by spotPython as defined in the optimizer_handler() method). We recommend tuning the learning rate later, when a reduced set of optimizers is fixed. Here, we will demonstrate how to select in a screening phase the optimizers that should be used for the hyperparameter tuning.\nFor the same reason, we will fix the sgd_momentum to 0.9.\n\nfun_control = modify_hyper_parameter_bounds(fun_control, \"lr_mult\", bounds=[1.0, 1.0])\nfun_control = modify_hyper_parameter_bounds(fun_control, \"sgd_momentum\", bounds=[0.9, 0.9])",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-selection-of-target-function",
         "objectID": "bart23e.html#sec-selection-of-target-function",
         "section": "Evaluation",
-        "text": "Evaluation\nThe evaluation procedure requires the specification of two elements:\n\nthe way how the data is split into a train and a test set and\nthe loss function (and a metric).\n\n\nHold-out Data Split and Cross-Validation\nAs a default, spotPython provides a standard hold-out data split and cross validation.\n\nHold-out Data Split\nIf a hold-out data split is used, the data will be partitioned into a training, a validation, and a test data set. The split depends on the setting of the eval parameter. If eval is set to train_hold_out, one data set, usually the original training data set, is split into a new training and a validation data set. The training data set is used for training the model. The validation data set is used for the evaluation of the hyperparameter configuration and early stopping to prevent overfitting. In this case, the original test data set is not used. The following splits are performed in the hold-out setting: \\(\\{\\text{train}_0, \\text{test}\\} \\rightarrow \\{\\text{train}_1, \\text{validation}_1, \\text{test}\\}\\), where \\(\\text{train}_1 \\cup \\text{validation}_1 = \\text{train}_0\\).\n\n\n\n\n\n\nNote\n\n\n\nspotPython returns the hyperparameters of the machine learning and deep learning models, e.g., number of layers, learning rate, or optimizer, but not the model weights. Therefore, after the SPOT run is finished, the corresponding model has to be trained again with the best hyperparameter configuration. The training is performed on the training data set. The test data set is used for the final evaluation of the model.\nSummarizing, the following splits are performed in the hold-out setting:\n\nRun spotPython with eval set to train_hold_out to determine the best hyperparameter configuration.\nTrain the model with the best hyperparameter configuration on the training data set:\n\ntrain_tuned(model_spot, train, \"model_spot.pt\").\n\nTest the model on the test data:\n\ntest_tuned(model_spot, test, \"model_spot.pt\")\n\n\nThese steps will be exemplified in the following sections.\n\n\nIn addition to this hold-out setting, spotPython provides another hold-out setting, where an explicit test data is specified by the user that will be used as the validation set. To choose this option, the eval parameter is set to test_hold_out. In this case, the training data set is used for the model training. Then, the explicitly defined test data set is used for the evaluation of the hyperparameter configuration (the validation).\n\n\nCross-Validation\nThe cross validation setting is used by setting the eval parameter to train_cv or test_cv. In both cases, the data set is split into \\(k\\) folds. The model is trained on \\(k-1\\) folds and evaluated on the remaining fold. This is repeated \\(k\\) times, so that each fold is used exactly once for evaluation. The final evaluation is performed on the test data set. The cross validation setting is useful for small data sets, because it allows to use all data for training and evaluation. However, it is computationally expensive, because the model has to be trained \\(k\\) times.\n\n\n\n\n\n\nNote\n\n\n\nCombinations of the above settings are possible, e.g., cross validation can be used for training and hold-out for evaluation or vice versa. Also, cross validation can be used for training and testing. Because cross validation is not used in the PyTorch tutorial (PyTorch 2023a), it is not considered further here.\n\n\n\n\nOverview of the Evaluation Settings\n\nSettings for the Hyperparameter Tuning\nTable\u00a02 provides an overview of the training evaluations.\n\n\nTable\u00a02: Overview of the evaluation settings.\n\n\n\n\n\n\n\n\n\neval\ntrain\ntest\nfunction\ncomment\n\n\n\n\n\"train_hold_out\"\n\\(\\checkmark\\)\n\ntrain_hold_out(), validate_fold_or_hold_out() for early stopping\nsplits the train data set internally\n\n\n\"test_hold_out\"\n\\(\\checkmark\\)\n\\(\\checkmark\\)\ntrain_hold_out(), validate_fold_or_hold_out() for early stopping\nuse the test data set for validate_fold_or_hold_out()\n\n\n\"train_cv\"\n\\(\\checkmark\\)\n\nevaluate_cv(net, train)\nCV using the train data set\n\n\n\"test_cv\"\n\n\\(\\checkmark\\)\nevaluate_cv(net, test)\nCV using the test data set . Identical to \"train_cv\", uses only test data.\n\n\n\n\n\n\"train_cv\" and \"test_cv\" use sklearn.model_selection.KFold() internally.\n\n\n\n\nDetailed Description of the \"train_hold_out\" Setting\nThe \"train_hold_out\" setting is used by default. It uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_hold_out() as follows:\n\n\ndf_eval, _ = evaluate_hold_out(\n    model,\n    train_dataset=fun_control[\"train\"],\n    shuffle=self.fun_control[\"shuffle\"],\n    loss_function=self.fun_control[\"loss_function\"],\n    metric=self.fun_control[\"metric_torch\"],\n    device=self.fun_control[\"device\"],\n    show_batch_interval=self.fun_control[\"show_batch_interval\"],\n    path=self.fun_control[\"path\"],\n) \n\nNote: Only the data set fun_control[\"train\"] is used for training and validation. It is used as follows:\n\ntrainloader, valloader = create_train_val_data_loaders(\n                dataset=train_dataset, batch_size=batch_size_instance, shuffle=shuffle\n            )\n\ncreate_train_val_data_loaders() splits the train_dataset into trainloader and valloader using torch.utils.data.random_split() as follows:\n\ndef create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):\n    test_abs = int(len(dataset) * 0.6)\n    train_subset, val_subset = random_split(dataset, [test_abs, len(dataset) - test_abs])\n    trainloader = torch.utils.data.DataLoader(\n        train_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    valloader = torch.utils.data.DataLoader(\n        val_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    return trainloader, valloader\n\nThe optimizer is set up as follows:\n\nlr_mult_instance = net.lr_mult\noptimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_mult=lr_mult_instance)\n\n\nevaluate_hold_out() sets the net attributes such as epochs, batch_size, optimizer, and patience. For each epoch, the methods train_hold_out() and validate_fold_or_hold_out() are called, the former for training and the latter for validation and early stopping. The validation loss from the last epoch (not the best validation loss) is returned from evaluate_hold_out.\nThe method train_hold_out() is implemented as follows:\n\n\ndef train_hold_out(net, trainloader, batch_size, loss_function, optimizer, device, show_batch_interval=10_000):\n    running_loss = 0.0\n    epoch_steps = 0\n    for i, data in enumerate(trainloader, 0):\n        inputs, labels = data\n        inputs, labels = inputs.to(device), labels.to(device)\n        optimizer.zero_grad()\n        outputs = net(inputs)\n        loss = loss_function(outputs, labels)\n        loss.backward()\n        torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)\n        optimizer.step()\n        running_loss += loss.item()\n        epoch_steps += 1\n        if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches\n            print(\n                \"Batch: %5d. Batch Size: %d. Training Loss (running): %.3f\"\n                % (i + 1, int(batch_size), running_loss / epoch_steps)\n            )\n            running_loss = 0.0\n    return loss.item()\n\n\nThe method validate_fold_or_hold_out() is implemented as follows:\n\n\ndef validate_fold_or_hold_out(net, valloader, loss_function, metric, device):\n    val_loss = 0.0\n    val_steps = 0\n    metric.reset()\n    for i, data in enumerate(valloader, 0):\n        with torch.no_grad():\n            inputs, labels = data\n            inputs, labels = inputs.to(device), labels.to(device)\n            outputs = net(inputs)\n            _, predicted = torch.max(outputs.data, 1)\n            metric_value = metric(predicted, labels).to(device)\n            loss = loss_function(outputs, labels)\n            val_loss += loss.cpu().numpy()\n            val_steps += 1\n    loss = val_loss / val_steps\n    metric_value = metric.compute()\n    return metric_value, loss\n\n\n\nDetailed Description of the \"test_hold_out\" Setting\nIt uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_hold_out() similar to the \"train_hold_out\" setting with one exception: It passes an additional test data set to evaluate_hold_out() as follows:\n\n\ntest_dataset=fun_control[\"test\"]\n\nevaluate_hold_out() calls create_train_test_data_loaders instead of create_train_val_data_loaders as follows: The two data sets are used in create_train_test_data_loaders as follows:\n\ndef create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset, num_workers=0):\n    trainloader = torch.utils.data.DataLoader(\n        dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    testloader = torch.utils.data.DataLoader(\n        test_dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    return trainloader, testloader\n\n\nThe following steps are identical to the \"train_hold_out\" setting. Only a different data loader is used for testing.\n\n\n\nDetailed Description of the \"train_cv\" Setting\nIt uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:\n\n\ndf_eval, _ = evaluate_cv(\n    model,\n    dataset=fun_control[\"train\"],\n    shuffle=self.fun_control[\"shuffle\"],\n    device=self.fun_control[\"device\"],\n    show_batch_interval=self.fun_control[\"show_batch_interval\"],\n)\n\nNote: Only the data set fun_control[\"train\"] is used for CV. 3. In `evaluate_cv(), the following steps are performed: The optimizer is set up as follows:\n\nlr_instance = net.lr\noptimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_mult=lr_mult_instance)\n\nevaluate_cv() sets the net attributes such as epochs, batch_size, optimizer, and patience. CV is implemented as follows:\n\nkfold = KFold(n_splits=k_folds_instance, shuffle=shuffle)\nfor fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):\n    train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)\n    val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)\n    trainloader = torch.utils.data.DataLoader(\n        dataset, batch_size=batch_size_instance, sampler=train_subsampler, num_workers=num_workers\n    )\n    valloader = torch.utils.data.DataLoader(\n        dataset, batch_size=batch_size_instance, sampler=val_subsampler, num_workers=num_workers\n    )\n    reset_weights(net)\n    # Train fold for several epochs:\n    train_fold(\n        net,\n        trainloader,\n        epochs_instance,\n        loss_function,\n        optimizer,\n        device,\n        show_batch_interval=show_batch_interval,\n    )\n    # Validate fold: use only loss for tuning\n    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_function, device)\ndf_eval = sum(loss_values.values()) / len(loss_values.values())\n\n\nThe method train_fold() is implemented as follows:\n\n\ndef train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interval=10_000):\n    for epoch in range(epochs):\n        print(f\"Epoch: {epoch + 1}\")\n        running_loss = 0.0\n        epoch_steps = 0\n        for i, data in enumerate(trainloader, 0):\n            inputs, labels = data\n            inputs, labels = inputs.to(device), labels.to(device)\n            optimizer.zero_grad()\n            outputs = net(inputs)\n            loss = loss_function(outputs, labels)\n            loss.backward()\n            torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)\n            optimizer.step()\n            # the following is for printing the statistic only\n            running_loss += loss.item()\n            epoch_steps += 1\n            if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches\n                print(\"Batch: %5d. Training Loss (running): %.3f\" % (i + 1, running_loss / epoch_steps))\n                running_loss = 0.0\n\n\nThe method validate_fold_or_hold_out() is implemented as shown above. In contrast to the hold-out setting, it is called for each of the \\(k\\) folds. The results are stored in a dictionaries metric_values and loss_values as follows:\n\n\n    # Validate fold: use only loss for tuning\n    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_function, device)\ndf_eval = sum(loss_values.values()) / len(loss_values.values())\n\nThe results are averaged over the \\(k\\) folds and returned as df_eval.\n\n\nDetailed Description of the \"test_cv\" Setting\nIt uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:\n\n\ndf_eval, _ = evaluate_cv(\n    model,\n    dataset=fun_control[\"test\"],\n    shuffle=self.fun_control[\"shuffle\"],\n    device=self.fun_control[\"device\"],\n    show_batch_interval=self.fun_control[\"show_batch_interval\"],\n)\n\nNote: The data set fun_control[\"test\"] is used for CV. The rest is the same as for the \"train_cv\" setting.\n\n\nSettings for the Final Evaluation of the Tuned Architecture\n\nTraining of the Tuned Architecture\ntrain_tuned(model, train): train the model with the best hyperparameter configuration (or simply the default) on the training data set. It splits the traindata into new train and validation sets using create_train_val_data_loaders(), which calls torch.utils.data.random_split() internally. Currently, 60% of the data is used for training and 40% for validation. The train data is used for training the model with train_hold_out(). The validation data is used for early stopping using validate_fold_or_hold_out() on the validation data set.\ntrain_tuned() is just a wrapper to evaluate_hold_out using the train data set. It is implemented as follows:\n\ndef train_tuned(net, train_dataset, shuffle, loss_function, metric, device=None, show_batch_interval=10_000, path=None):\n    evaluate_hold_out(\n        net=net,\n        train_dataset=train_dataset,\n        shuffle=shuffle,\n        test_dataset=None,\n        loss_function=loss_function,\n        metric=metric,\n        device=device,\n        show_batch_interval=show_batch_interval,\n        path=path,\n    )\n\nNote: During training, shuffle is set to True, whereas during testing, shuffle is set to False.\n\n\nTesting of the Tuned Architecture\ntest_tuned(model, test): test the model on the test data set. No data splitting is performed. The (trained) model is evaluated using the validate_fold_or_hold_out() function.\nNote: During training, shuffle is set to True, whereas during testing, shuffle is set to False.\n\ndef test_tuned(net, shuffle, test_dataset=None, loss_function=None, metric=None, device=None, path=None):\n    batch_size_instance = net.batch_size\n    removed_attributes, net = get_removed_attributes_and_base_net(net)\n    if path is not None:\n        net.load_state_dict(torch.load(path))\n        net.eval()\n    try:\n        device = getDevice(device=device)\n        if torch.cuda.is_available():\n            device = \"cuda:0\"\n            if torch.cuda.device_count() &gt; 1:\n                print(\"We will use\", torch.cuda.device_count(), \"GPUs!\")\n                net = nn.DataParallel(net)\n        net.to(device)\n        valloader = torch.utils.data.DataLoader(\n            test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle, num_workers=0\n        )\n        metric_value, loss = validate_fold_or_hold_out(\n            net, valloader=valloader, loss_function=loss_function, metric=metric, device=device\n        )\n        df_eval = loss\n        df_metric = metric_value\n        df_preds = np.nan\n    except Exception as err:\n        print(f\"Error in Net_Core. Call to test_tuned() failed. {err=}, {type(err)=}\")\n        df_eval = np.nan\n        df_metric = np.nan\n        df_preds = np.nan\n    add_attributes(net, removed_attributes)\n    print(f\"Final evaluation: Validation loss: {df_eval}\")\n    print(f\"Final evaluation: Validation metric: {df_metric}\")\n    print(\"----------------------------------------------\")\n    return df_eval, df_preds, df_metric\n\n\n\n\n\nLoss Functions and Metrics\nThe key \"loss_function\" specifies the loss function which is used during the optimization. There are several different loss functions under PyTorch\u2019s nn package. For example, a simple loss is MSELoss, which computes the mean-squared error between the output and the target. In this tutorial we will use CrossEntropyLoss, because it is also used in the PyTorch tutorial.\n\nfrom torch.nn import CrossEntropyLoss\nloss_function = CrossEntropyLoss()\nfun_control.update({\"loss_function\": loss_function})\n\nIn addition to the loss functions, spotPython provides access to a large number of metrics. The key \"metric_sklearn\" is used for metrics that follow the scikit-learn conventions. The key \"river_metric\" is used for the river based evaluation (Montiel et al. 2021) via eval_oml_iter_progressive, and the key \"metric_torch\" is used for the metrics from TorchMetrics. TorchMetrics is a collection of more than 90 PyTorch metrics4. Because the PyTorch tutorial uses the accuracy as metric, we use the same metric here. Currently, accuracy is computed in the tutorial\u2019s example code. We will use TorchMetrics instead, because it offers:\n\nA standardized interface to increase reproducibility\nReduces Boilerplate\nDistributed-training compatible\nRigorously tested\nAutomatic accumulation over batches\nAutomatic synchronization between multiple devices\n\nTherefore, we set\n\nmetric_torch = torchmetrics.Accuracy(task=\"multiclass\", num_classes=10)\n\n\nloss_function = CrossEntropyLoss()\nweights = 1.0\nmetric_torch = torchmetrics.Accuracy(task=\"multiclass\", num_classes=10)\nshuffle = True\neval = \"train_hold_out\"\ndevice = DEVICE\nshow_batch_interval = 100_000\npath=\"torch_model.pt\"\n\nfun_control.update({\n               \"data_dir\": None,\n               \"checkpoint_dir\": None,\n               \"horizon\": None,\n               \"oml_grace_period\": None,\n               \"weights\": weights,\n               \"step\": None,\n               \"log_level\": 50,\n               \"weight_coeff\": None,\n               \"metric_torch\": metric_torch,\n               \"metric_river\": None,\n               \"metric_sklearn\": None,\n               \"loss_function\": loss_function,\n               \"shuffle\": shuffle,\n               \"eval\": eval,\n               \"device\": device,\n               \"show_batch_interval\": show_batch_interval,\n               \"path\": path,\n               })",
+        "text": "Evaluation\nThe evaluation procedure requires the specification of two elements:\n\nthe way how the data is split into a train and a test set and\nthe loss function (and a metric).\n\n\nHold-out Data Split and Cross-Validation\nAs a default, spotPython provides a standard hold-out data split and cross validation.\n\nHold-out Data Split\nIf a hold-out data split is used, the data will be partitioned into a training, a validation, and a test data set. The split depends on the setting of the eval parameter. If eval is set to train_hold_out, one data set, usually the original training data set, is split into a new training and a validation data set. The training data set is used for training the model. The validation data set is used for the evaluation of the hyperparameter configuration and early stopping to prevent overfitting. In this case, the original test data set is not used. The following splits are performed in the hold-out setting: \\(\\{\\text{train}_0, \\text{test}\\} \\rightarrow \\{\\text{train}_1, \\text{validation}_1, \\text{test}\\}\\), where \\(\\text{train}_1 \\cup \\text{validation}_1 = \\text{train}_0\\).\n\n\n\n\n\n\nNote\n\n\n\nspotPython returns the hyperparameters of the machine learning and deep learning models, e.g., number of layers, learning rate, or optimizer, but not the model weights. Therefore, after the SPOT run is finished, the corresponding model with the optimized architecture has to be trained again with the best hyperparameter configuration. The training is performed on the training data set. The test data set is used for the final evaluation of the model.\nSummarizing, the following splits are performed in the hold-out setting:\n\nRun spotPython with eval set to train_hold_out to determine the best hyperparameter configuration.\nTrain the model with the best hyperparameter configuration (\u201carchitecture\u201d) on the training data set:\n\ntrain_tuned(model_spot, train, \"model_spot.pt\").\n\nTest the model on the test data:\n\ntest_tuned(model_spot, test, \"model_spot.pt\")\n\n\nThese steps will be exemplified in the following sections.\n\n\nIn addition to this hold-out setting, spotPython provides another hold-out setting, where an explicit test data is specified by the user that will be used as the validation set. To choose this option, the eval parameter is set to test_hold_out. In this case, the training data set is used for the model training. Then, the explicitly defined test data set is used for the evaluation of the hyperparameter configuration (the validation).\n\n\nCross-Validation\nThe cross validation setting is used by setting the eval parameter to train_cv or test_cv. In both cases, the data set is split into \\(k\\) folds. The model is trained on \\(k-1\\) folds and evaluated on the remaining fold. This is repeated \\(k\\) times, so that each fold is used exactly once for evaluation. The final evaluation is performed on the test data set. The cross validation setting is useful for small data sets, because it allows to use all data for training and evaluation. However, it is computationally expensive, because the model has to be trained \\(k\\) times.\n\n\n\n\n\n\nNote\n\n\n\nCombinations of the above settings are possible, e.g., cross validation can be used for training and hold-out for evaluation or vice versa. Also, cross validation can be used for training and testing. Because cross validation is not used in the PyTorch tutorial (PyTorch 2023a), it is not considered further here.\n\n\n\n\nOverview of the Evaluation Settings\n\nSettings for the Hyperparameter Tuning\nTable\u00a02 provides an overview of the training evaluations.\n\n\nTable\u00a02: Overview of the evaluation settings.\n\n\n\n\n\n\n\n\n\neval\ntrain\ntest\nfunction\ncomment\n\n\n\n\n\"train_hold_out\"\n\\(\\checkmark\\)\n\ntrain_hold_out(), validate_fold_or_hold_out() for early stopping\nsplits the train data set internally\n\n\n\"test_hold_out\"\n\\(\\checkmark\\)\n\\(\\checkmark\\)\ntrain_hold_out(), validate_fold_or_hold_out() for early stopping\nuse the test data set for validate_fold_or_hold_out()\n\n\n\"train_cv\"\n\\(\\checkmark\\)\n\nevaluate_cv(net, train)\nCV using the train data set\n\n\n\"test_cv\"\n\n\\(\\checkmark\\)\nevaluate_cv(net, test)\nCV using the test data set . Identical to \"train_cv\", uses only test data.\n\n\n\n\n\n\"train_cv\" and \"test_cv\" use sklearn.model_selection.KFold() internally.\n\nSection\u00a06.2 (in the Appendix) provides more details on the data splitting.\n\n\n\nSettings for the Final Evaluation of the Tuned Architecture\n\nTraining of the Tuned Architecture\ntrain_tuned(model, train): train the model with the best hyperparameter configuration (or simply the default) on the training data set. It splits the traindata into new train and validation sets using create_train_val_data_loaders(), which calls torch.utils.data.random_split() internally. Currently, 60% of the data is used for training and 40% for validation. The train data is used for training the model with train_hold_out(). The validation data is used for early stopping using validate_fold_or_hold_out() on the validation data set.\n\n\nTesting of the Tuned Architecture\ntest_tuned(model, test): test the model on the test data set. No data splitting is performed. The (trained) model is evaluated using the validate_fold_or_hold_out() function.\nNote: During training, shuffle is set to True, whereas during testing, shuffle is set to False.\nSection\u00a06.2.5 describes the final evaluation of the tuned architecture.\n\n\n\n\nLoss Functions and Metrics\nThe key \"loss_function\" specifies the loss function which is used during the optimization. There are several different loss functions under PyTorch\u2019s nn package. For example, a simple loss is MSELoss, which computes the mean-squared error between the output and the target. In this tutorial we will use CrossEntropyLoss, because it is also used in the PyTorch tutorial.\n\nfrom torch.nn import CrossEntropyLoss\nloss_function = CrossEntropyLoss()\nfun_control.update({\"loss_function\": loss_function})\n\nIn addition to the loss functions, spotPython provides access to a large number of metrics. The key \"metric_sklearn\" is used for metrics that follow the scikit-learn conventions. The key \"river_metric\" is used for the river based evaluation (Montiel et al. 2021) via eval_oml_iter_progressive, and the key \"metric_torch\" is used for the metrics from TorchMetrics. TorchMetrics is a collection of more than 90 PyTorch metrics4. Because the PyTorch tutorial uses the accuracy as metric, we use the same metric here. Currently, accuracy is computed in the tutorial\u2019s example code. We will use TorchMetrics instead, because it offers more flexibilty, e.g., it can be used for regression and classification. Furthermore, TorchMetrics offers the following advantages:\n\nA standardized interface to increase reproducibility\nReduces Boilerplate\nDistributed-training compatible\nRigorously tested\nAutomatic accumulation over batches\nAutomatic synchronization between multiple devices\n\nTherefore, we set\n\nmetric_torch = torchmetrics.Accuracy(task=\"multiclass\", num_classes=10)\n\n\nloss_function = CrossEntropyLoss()\nweights = 1.0\nmetric_torch = torchmetrics.Accuracy(task=\"multiclass\", num_classes=10)\nshuffle = True\neval = \"train_hold_out\"\ndevice = DEVICE\nshow_batch_interval = 100_000\npath=\"torch_model.pt\"\n\nfun_control.update({\n               \"data_dir\": None,\n               \"checkpoint_dir\": None,\n               \"horizon\": None,\n               \"oml_grace_period\": None,\n               \"weights\": weights,\n               \"step\": None,\n               \"log_level\": 50,\n               \"weight_coeff\": None,\n               \"metric_torch\": metric_torch,\n               \"metric_river\": None,\n               \"metric_sklearn\": None,\n               \"loss_function\": loss_function,\n               \"shuffle\": shuffle,\n               \"eval\": eval,\n               \"device\": device,\n               \"show_batch_interval\": show_batch_interval,\n               \"path\": path,\n               })",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sec-call-the-hyperparameter-tuner",
         "objectID": "bart23e.html#sec-call-the-hyperparameter-tuner",
         "section": "Calling the SPOT Function",
         "text": "Calling the SPOT Function\nNow, the dictionary fun_control contains all information needed for the hyperparameter tuning. Before the hyperparameter tuning is started, it is recommended to take a look at the experimental design. The method gen_design_table generates a design table as follows:\n\nprint(gen_design_table(fun_control))\n\nThis allows to check if all information is available and if the information is correct. Table\u00a03 shows the experimental design for the hyperparameter tuning. Hyperparameter transformations are shown in the column \u201ctransform\u201d, e.g., the l1 default is 5, which results in the value \\(2^5 = 32\\) for the network, because the transformation transform_power_2_int was selected in the JSON file. The default value of the batch_size is set to 4, which results in a batch size of \\(2^4 = 16\\).\n\n\nTable\u00a03: Experimental design for the hyperparameter tuning. The table shows the hyperparameters, their types, default values, lower and upper bounds, and the transformation function. The transformation function is used to transform the hyperparameter values from the unit hypercube to the original domain. The transformation function is applied to the hyperparameter values before the evaluation of the objective function.\n\n\n\n\n\n\n\n\n\n\nname\ntype\ndefault\nlower\nupper\ntransform\n\n\n\n\nl1\nint\n5\n2\n9\ntransform_power_2_int\n\n\nl2\nint\n5\n2\n9\ntransform_power_2_int\n\n\nlr\nfloat\n0.001\n0.001\n0.001\nNone\n\n\nbatch_size\nint\n4\n1\n5\ntransform_power_2_int\n\n\nepochs\nint\n3\n3\n4\ntransform_power_2_int\n\n\nk_folds\nint\n2\n0\n0\nNone\n\n\npatience\nint\n5\n3\n3\nNone\n\n\noptimizer\nfactor\nSGD\n0\n9\nNone\n\n\n\n\nThe objective function fun_torch is selected next. It implements an interface from PyTorch\u2019s training, validation, and testing methods to spotPython.\n\nfun = HyperTorch().fun_torch\n\nThe spotPython hyperparameter tuning is started by calling the Spot function. Here, we will run the tuner for approximately 30 minutes (max_time). Note: the initial design is always evaluated in the spotPython run. As a consequence, the run may take longer than specified by max_time, because the evaluation time of initial design (here: init_size, 10 points) is performed independently of max_time.\n\nspot_tuner = spot.Spot(fun=fun,\n                   lower = lower,\n                   upper = upper,\n                   fun_evals = inf,\n                   fun_repeats = 1,\n                   max_time = MAX_TIME,\n                   noise = False,\n                   tolerance_x = np.sqrt(np.spacing(1)),\n                   var_type = var_type,\n                   var_name = var_name,\n                   infill_criterion = \"y\",\n                   n_points = 1,\n                   seed=123,\n                   log_level = 50,\n                   show_models= False,\n                   show_progress= True,\n                   fun_control = fun_control,\n                   design_control={\"init_size\": INIT_SIZE,\n                                   \"repeats\": 1},\n                   surrogate_control={\"noise\": True,\n                                      \"cod_type\": \"norm\",\n                                      \"min_theta\": -4,\n                                      \"max_theta\": 3,\n                                      \"n_theta\": len(var_name),\n                                      \"model_optimizer\": differential_evolution,\n                                      \"model_fun_evals\": 10_000,\n                                      \"log_level\": 50\n                                      })\nspot_tuner.run(X_start=X_start)\n\nDuring the run, the following output is shown:\nconfig: {'l1': 4, 'l2': 64, 'lr_mult': 1.0, 'batch_size': 16, 'epochs': 16, 'k_folds': 0, 'patience': 3, 'optimizer': 'Adadelta', 'sgd_momentum': 0.9}\nEpoch: 1\nLoss on hold-out set: 1.602842689704895\nAccuracy on hold-out set: 0.4006\nMetric value on hold-out data: 0.40059998631477356\nEpoch: 2\nLoss on hold-out set: 1.4648857820034027\nAccuracy on hold-out set: 0.47685\nMetric value on hold-out data: 0.4768500030040741\nEpoch: 3\nLoss on hold-out set: 1.403354868555069\nAccuracy on hold-out set: 0.482\nMetric value on hold-out data: 0.4819999933242798\nEpoch: 4\nLoss on hold-out set: 1.384560032081604\nAccuracy on hold-out set: 0.49065\nMetric value on hold-out data: 0.4906499981880188\nEpoch: 5\nLoss on hold-out set: 1.4326466094970702\nAccuracy on hold-out set: 0.4809\nMetric value on hold-out data: 0.48089998960494995\nEpoch: 6\nLoss on hold-out set: 1.3759961807250976\nAccuracy on hold-out set: 0.4995\nMetric value on hold-out data: 0.49950000643730164\nEpoch: 7\nLoss on hold-out set: 1.3684927892208099\nAccuracy on hold-out set: 0.50695\nMetric value on hold-out data: 0.5069500207901001\nEpoch: 8\nLoss on hold-out set: 1.3642385012149811\nAccuracy on hold-out set: 0.506\nMetric value on hold-out data: 0.5059999823570251\nEpoch: 9\nLoss on hold-out set: 1.3157437609672546\nAccuracy on hold-out set: 0.5304\nMetric value on hold-out data: 0.5303999781608582\nEpoch: 10\nLoss on hold-out set: 1.3481314319610596\nAccuracy on hold-out set: 0.5268\nMetric value on hold-out data: 0.5267999768257141\nEpoch: 11\nLoss on hold-out set: 1.3608774542331696\nAccuracy on hold-out set: 0.51525\nMetric value on hold-out data: 0.515250027179718\nEpoch: 12\nLoss on hold-out set: 1.359324642753601\nAccuracy on hold-out set: 0.52355\nMetric value on hold-out data: 0.5235499739646912\nEarly stopping at epoch 11\nReturned to Spot: Validation loss: 1.359324642753601\n----------------------------------------------",
@@ -83,15 +83,15 @@
         "text": "Get SPOT Results\nThe architecture of the spotPython model can be obtained by the following code:\n\nX = spot_tuner.to_all_dim(spot_tuner.min_X.reshape(1,-1))\nmodel_spot = get_one_core_model_from_X(X, fun_control)\nmodel_spot\n\nFirst, the numerical representation of the hyperparameters are obtained, i.e., the numpy array X is generated. This array is then used to generate the model model_spot by the function get_one_core_model_from_X. The model model_spot has the following architecture:\nNet_CIFAR10(\n  (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))\n  (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)\n  (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))\n  (fc1): Linear(in_features=400, out_features=64, bias=True)\n  (fc2): Linear(in_features=64, out_features=32, bias=True)\n  (fc3): Linear(in_features=32, out_features=10, bias=True)\n)",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#get-default-hyperparameters",
         "objectID": "bart23e.html#get-default-hyperparameters",
         "section": "Get Default Hyperparameters",
-        "text": "Get Default Hyperparameters\nIn a similar manner as in Section\u00a03.11, the default hyperparameters can be obtained.\n\n# fun_control was modified, we generate a new one with the original default hyperparameters\nfc = copy.deepcopy(fun_control)\nfc.update({\"core_model_hyper_dict\": hyper_dict[fun_control[\"core_model\"].__name__]})\nmodel_default = get_one_core_model_from_X(X_start, fun_control=fc)\n\nThe corresponding default model has the following architecture:\nNet_CIFAR10(\n  (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))\n  (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)\n  (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))\n  (fc1): Linear(in_features=400, out_features=32, bias=True)\n  (fc2): Linear(in_features=32, out_features=32, bias=True)\n  (fc3): Linear(in_features=32, out_features=10, bias=True)\n)",
+        "text": "Get Default Hyperparameters\nIn a similar manner as in Section\u00a04.11, the default hyperparameters can be obtained.\n\n# fun_control was modified, we generate a new one with the original default hyperparameters\nfc = copy.deepcopy(fun_control)\nfc.update({\"core_model_hyper_dict\": hyper_dict[fun_control[\"core_model\"].__name__]})\nmodel_default = get_one_core_model_from_X(X_start, fun_control=fc)\n\nThe corresponding default model has the following architecture:\nNet_CIFAR10(\n  (conv1): Conv2d(3, 6, kernel_size=(5, 5), stride=(1, 1))\n  (pool): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)\n  (conv2): Conv2d(6, 16, kernel_size=(5, 5), stride=(1, 1))\n  (fc1): Linear(in_features=400, out_features=32, bias=True)\n  (fc2): Linear(in_features=32, out_features=32, bias=True)\n  (fc3): Linear(in_features=32, out_features=10, bias=True)\n)",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#evaluation-of-the-tuned-architecture",
         "objectID": "bart23e.html#evaluation-of-the-tuned-architecture",
         "section": "Evaluation of the Tuned Architecture",
         "text": "Evaluation of the Tuned Architecture\nThe method train_tuned takes a model architecture without trained weights and trains this model with the train data. The train data is split into train and validation data. The validation data is used for early stopping. The trained model weights are saved as a dictionary.\nThis evaluation is similar to the final evaluation in PyTorch (2023a).\n\ntrain_tuned(net=model_default, train_dataset=train, shuffle=True,\n        loss_function=fun_control[\"loss_function\"],\n        metric=fun_control[\"metric_torch\"],\n        device = DEVICE, show_batch_interval=1_000,)\ntest_tuned(net=model_default, test_dataset=test, \n        loss_function=fun_control[\"loss_function\"],\n        metric=fun_control[\"metric_torch\"],\n        shuffle=False, \n        device = DEVICE)\n\nThe following code trains the model model_spot. If path is set to a filename, e.g., path = \"model_spot_trained.pt\", the weights of the trained model will be saved to this file.\n\ntrain_tuned(net=model_spot, train_dataset=train,\n        loss_function=fun_control[\"loss_function\"],\n        metric=fun_control[\"metric_torch\"],\n        shuffle=True,\n        device = DEVICE,\n        path=None)\n\nLoss on hold-out set: 1.2267619131326675\nAccuracy on hold-out set: 0.58955\nEarly stopping at epoch 13\nIf path is set to a filename, e.g., path = \"model_spot_trained.pt\", the weights of the trained model will be loaded from this file.\n\ntest_tuned(net=model_spot, test_dataset=test,\n            shuffle=False,\n            loss_function=fun_control[\"loss_function\"],\n            metric=fun_control[\"metric_torch\"],\n            device = DEVICE)\n\nLoss on hold-out set: 1.242568492603302\nAccuracy on hold-out set: 0.5957",
@@ -104,25 +104,32 @@
         "text": "Comparison with Default Hyperparameters and Ray Tune\nTable\u00a05 shows the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from ray[tune].\n\n\nTable\u00a05: Comparison of the loss and accuracy of the default model, the model with the hyperparameters from SPOT, and the model with the hyperparameters from ray[tune]. ray[tune] only shows the validation loss, because training loss is not reported by ray[tune].\n\n\n\n\n\n\n\n\n\nModel\nValidation Loss\nValidation Accuracy\nLoss\nAccuracy\n\n\n\n\nDefault\n2.1221\n0.2452\n2.1182\n0.2425\n\n\nspotPython\n1.2268\n0.5896\n1.2426\n0.5957\n\n\nray[tune]\n1.1815\n0.5836\n-\n0.5806",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#detailed-hyperparameter-plots",
         "objectID": "bart23e.html#detailed-hyperparameter-plots",
         "section": "Detailed Hyperparameter Plots",
-        "text": "Detailed Hyperparameter Plots\nThe contour plots in this section visualize the interactions of the three most important hyperparameters, l1, l2, and epochs, and optimizer of the surrogate model used to optimize the hyperparameters. Since some of these hyperparameters take fatorial or integer values, sometimes step-like fitness landcapes (or response surfaces) are generated. SPOT draws the interactions of the main hyperparameters by default. It is also possible to visualize all interactions. For this, again refer to the notebook (Bartz-Beielstein 2023).\n\n\nthreshold = 0.025\nimpo = spot_tuner.print_importance(threshold=threshold, print_screen=True)\nvar_plots = [i for i, x in enumerate(impo) if x[1] &gt; threshold]\nmin_z = min(spot_tuner.y)\nmax_z = max(spot_tuner.y)\nn = spot_tuner.k\nfor i in var_plots:\n    for j in var_plots:\n        if j &gt; i:\n            filename = \"./figures\" + experiment_name+\"_contour_\"+str(i)+\"_\"+str(j)+\".png\"\n            spot_tuner.plot_contour(i=i, j=j, min_z=min_z, max_z = max_z, filename=filename)\nFigure\u00a04: ?(caption)\n\n\n\n\n\nFigure\u00a05: Contour plot of the loss as a function of l1 and l2, i.e., the number of neurons in the layers.\n\n\n\n\n\nFigure\u00a06: Contour plot of the loss as a function of the number of epochs and the neurons in layer l1.\n\n\n\n\n\nFigure\u00a07: Contour plot of the loss as a function of the optimizer and the neurons in layer l1.\n\n\n\n\n\nFigure\u00a08: Contour plot of the loss as a function of the number of epochs and the neurons in layer l2.\n\n\n\n\n\nFigure\u00a09: Contour plot of the loss as a function of the optimizer and the neurons in layer l2.\n\n\n\n\n\nFigure\u00a010: Contour plot of the loss as a function of the optimizer and the number of epochs.\n\n\nFigure\u00a05 to Figure\u00a010 show the contour plots of the loss as a function of the hyperparameters. These plots are very helpful for benchmark studies and for understanding neural networks. spotPython provides additional tools for a visual inspection of the results and give valuable insights into the hyperparameter tuning process. This is especially useful for model explainability, transparency, and trustworthiness. In addition to the contour plots, Figure\u00a012 shows the parallel plot of the hyperparameters.\n\n\nspot_tuner.parallel_plot()\nFigure\u00a011: ?(caption)\n\n\n\n\n\nFigure\u00a012: Parallel plot",
+        "text": "Detailed Hyperparameter Plots\nThe contour plots in this section visualize the interactions of the three most important hyperparameters, l1, l2, and epochs, and optimizer of the surrogate model used to optimize the hyperparameters. Since some of these hyperparameters take fatorial or integer values, sometimes step-like fitness landcapes (or response surfaces) are generated. SPOT draws the interactions of the main hyperparameters by default. It is also possible to visualize all interactions. For this, again refer to the notebook (Bartz-Beielstein 2023).\n\nfilename = \"./figures\" + experiment_name\nspot_tuner.plot_important_hyperparameter_contour(filename=filename)\n\n\n\n\nFigure\u00a04: Contour plot of the loss as a function of l1 and l2, i.e., the number of neurons in the layers.\n\n\n\n\n\nFigure\u00a05: Contour plot of the loss as a function of the number of epochs and the neurons in layer l1.\n\n\n\n\n\nFigure\u00a06: Contour plot of the loss as a function of the optimizer and the neurons in layer l1.\n\n\n\n\n\nFigure\u00a07: Contour plot of the loss as a function of the number of epochs and the neurons in layer l2.\n\n\n\n\n\nFigure\u00a08: Contour plot of the loss as a function of the optimizer and the neurons in layer l2.\n\n\n\n\n\nFigure\u00a09: Contour plot of the loss as a function of the optimizer and the number of epochs.\n\n\nFigure\u00a04 to Figure\u00a09 show the contour plots of the loss as a function of the hyperparameters. These plots are very helpful for benchmark studies and for understanding neural networks. spotPython provides additional tools for a visual inspection of the results and give valuable insights into the hyperparameter tuning process. This is especially useful for model explainability, transparency, and trustworthiness. In addition to the contour plots, Figure\u00a010 shows the parallel plot of the hyperparameters.\n\nspot_tuner.parallel_plot()\n\n\n\n\nFigure\u00a010: Parallel plot",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
         "href": "bart23e.html#sample-output-from-ray-tunes-run",
         "objectID": "bart23e.html#sample-output-from-ray-tunes-run",
         "section": "Sample Output From Ray Tune\u2019s Run",
         "text": "Sample Output From Ray Tune\u2019s Run\nThe output from ray[tune] could look like this (PyTorch 2023b):\nNumber of trials: 10 (10 TERMINATED)\n------+------+-------------+--------------+---------+------------+--------------------+\n|   l1 |   l2 |          lr |   batch_size |    loss |   accuracy | training_iteration |\n+------+------+-------------+--------------+---------+------------+--------------------|\n|   64 |    4 | 0.00011629  |            2 | 1.87273 |     0.244  |                  2 |\n|   32 |   64 | 0.000339763 |            8 | 1.23603 |     0.567  |                  8 |\n|    8 |   16 | 0.00276249  |           16 | 1.1815  |     0.5836 |                 10 |\n|    4 |   64 | 0.000648721 |            4 | 1.31131 |     0.5224 |                  8 |\n|   32 |   16 | 0.000340753 |            8 | 1.26454 |     0.5444 |                  8 |\n|    8 |    4 | 0.000699775 |            8 | 1.99594 |     0.1983 |                  2 |\n|  256 |    8 | 0.0839654   |           16 | 2.3119  |     0.0993 |                  1 |\n|   16 |  128 | 0.0758154   |           16 | 2.33575 |     0.1327 |                  1 |\n|   16 |    8 | 0.0763312   |           16 | 2.31129 |     0.1042 |                  4 |\n|  128 |   16 | 0.000124903 |            4 | 2.26917 |     0.1945 |                  1 |\n+-----+------+------+-------------+--------------+---------+------------+--------------------+\nBest trial config: {'l1': 8, 'l2': 16, 'lr': 0.00276249, 'batch_size': 16, 'data_dir': '...'}\nBest trial final validation loss: 1.181501\nBest trial final validation accuracy: 0.5836\nBest trial test set accuracy: 0.5806",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     },
     {
+        "href": "bart23e.html#sec-data-splitting",
+        "objectID": "bart23e.html#sec-data-splitting",
+        "section": "Detailed Description of the Data Splitting",
+        "text": "Detailed Description of the Data Splitting\n\nDescription of the \"train_hold_out\" Setting\nThe \"train_hold_out\" setting is used by default. It uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_hold_out() as follows:\n\n\ndf_eval, _ = evaluate_hold_out(\n    model,\n    train_dataset=fun_control[\"train\"],\n    shuffle=self.fun_control[\"shuffle\"],\n    loss_function=self.fun_control[\"loss_function\"],\n    metric=self.fun_control[\"metric_torch\"],\n    device=self.fun_control[\"device\"],\n    show_batch_interval=self.fun_control[\"show_batch_interval\"],\n    path=self.fun_control[\"path\"],\n) \n\nNote: Only the data set fun_control[\"train\"] is used for training and validation. It is used as follows:\n\ntrainloader, valloader = create_train_val_data_loaders(\n                dataset=train_dataset, batch_size=batch_size_instance, shuffle=shuffle\n            )\n\ncreate_train_val_data_loaders() splits the train_dataset into trainloader and valloader using torch.utils.data.random_split() as follows:\n\ndef create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):\n    test_abs = int(len(dataset) * 0.6)\n    train_subset, val_subset = random_split(dataset, [test_abs, len(dataset) - test_abs])\n    trainloader = torch.utils.data.DataLoader(\n        train_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    valloader = torch.utils.data.DataLoader(\n        val_subset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    return trainloader, valloader\n\nThe optimizer is set up as follows:\n\nlr_mult_instance = net.lr_mult\noptimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_mult=lr_mult_instance)\n\n\nevaluate_hold_out() sets the net attributes such as epochs, batch_size, optimizer, and patience. For each epoch, the methods train_hold_out() and validate_fold_or_hold_out() are called, the former for training and the latter for validation and early stopping. The validation loss from the last epoch (not the best validation loss) is returned from evaluate_hold_out.\nThe method train_hold_out() is implemented as follows:\n\n\ndef train_hold_out(net, trainloader, batch_size, loss_function, optimizer, device, show_batch_interval=10_000):\n    running_loss = 0.0\n    epoch_steps = 0\n    for i, data in enumerate(trainloader, 0):\n        inputs, labels = data\n        inputs, labels = inputs.to(device), labels.to(device)\n        optimizer.zero_grad()\n        outputs = net(inputs)\n        loss = loss_function(outputs, labels)\n        loss.backward()\n        torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)\n        optimizer.step()\n        running_loss += loss.item()\n        epoch_steps += 1\n        if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches\n            print(\n                \"Batch: %5d. Batch Size: %d. Training Loss (running): %.3f\"\n                % (i + 1, int(batch_size), running_loss / epoch_steps)\n            )\n            running_loss = 0.0\n    return loss.item()\n\n\nThe method validate_fold_or_hold_out() is implemented as follows:\n\n\ndef validate_fold_or_hold_out(net, valloader, loss_function, metric, device):\n    val_loss = 0.0\n    val_steps = 0\n    metric.reset()\n    for i, data in enumerate(valloader, 0):\n        with torch.no_grad():\n            inputs, labels = data\n            inputs, labels = inputs.to(device), labels.to(device)\n            outputs = net(inputs)\n            _, predicted = torch.max(outputs.data, 1)\n            metric_value = metric(predicted, labels).to(device)\n            loss = loss_function(outputs, labels)\n            val_loss += loss.cpu().numpy()\n            val_steps += 1\n    loss = val_loss / val_steps\n    metric_value = metric.compute()\n    return metric_value, loss\n\n\n\nDescription of the \"test_hold_out\" Setting\nIt uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_hold_out() similar to the \"train_hold_out\" setting with one exception: It passes an additional test data set to evaluate_hold_out() as follows:\n\n\ntest_dataset=fun_control[\"test\"]\n\nevaluate_hold_out() calls create_train_test_data_loaders instead of create_train_val_data_loaders as follows: The two data sets are used in create_train_test_data_loaders as follows:\n\ndef create_train_test_data_loaders(dataset, batch_size, shuffle, test_dataset, num_workers=0):\n    trainloader = torch.utils.data.DataLoader(\n        dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    testloader = torch.utils.data.DataLoader(\n        test_dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers\n    )\n    return trainloader, testloader\n\n\nThe following steps are identical to the \"train_hold_out\" setting. Only a different data loader is used for testing.\n\n\n\nDetailed Description of the \"train_cv\" Setting\nIt uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:\n\n\ndf_eval, _ = evaluate_cv(\n    model,\n    dataset=fun_control[\"train\"],\n    shuffle=self.fun_control[\"shuffle\"],\n    device=self.fun_control[\"device\"],\n    show_batch_interval=self.fun_control[\"show_batch_interval\"],\n)\n\nNote: Only the data set fun_control[\"train\"] is used for CV. 3. In `evaluate_cv(), the following steps are performed: The optimizer is set up as follows:\n\nlr_instance = net.lr\noptimizer = optimizer_handler(optimizer_name=optimizer_instance, params=net.parameters(), lr_mult=lr_mult_instance)\n\nevaluate_cv() sets the net attributes such as epochs, batch_size, optimizer, and patience. CV is implemented as follows:\n\nkfold = KFold(n_splits=k_folds_instance, shuffle=shuffle)\nfor fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):\n    train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)\n    val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)\n    trainloader = torch.utils.data.DataLoader(\n        dataset, batch_size=batch_size_instance, sampler=train_subsampler, num_workers=num_workers\n    )\n    valloader = torch.utils.data.DataLoader(\n        dataset, batch_size=batch_size_instance, sampler=val_subsampler, num_workers=num_workers\n    )\n    reset_weights(net)\n    # Train fold for several epochs:\n    train_fold(\n        net,\n        trainloader,\n        epochs_instance,\n        loss_function,\n        optimizer,\n        device,\n        show_batch_interval=show_batch_interval,\n    )\n    # Validate fold: use only loss for tuning\n    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_function, device)\ndf_eval = sum(loss_values.values()) / len(loss_values.values())\n\n\nThe method train_fold() is implemented as follows:\n\n\ndef train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interval=10_000):\n    for epoch in range(epochs):\n        print(f\"Epoch: {epoch + 1}\")\n        running_loss = 0.0\n        epoch_steps = 0\n        for i, data in enumerate(trainloader, 0):\n            inputs, labels = data\n            inputs, labels = inputs.to(device), labels.to(device)\n            optimizer.zero_grad()\n            outputs = net(inputs)\n            loss = loss_function(outputs, labels)\n            loss.backward()\n            torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)\n            optimizer.step()\n            # the following is for printing the statistic only\n            running_loss += loss.item()\n            epoch_steps += 1\n            if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches\n                print(\"Batch: %5d. Training Loss (running): %.3f\" % (i + 1, running_loss / epoch_steps))\n                running_loss = 0.0\n\n\nThe method validate_fold_or_hold_out() is implemented as shown above. In contrast to the hold-out setting, it is called for each of the \\(k\\) folds. The results are stored in a dictionaries metric_values and loss_values as follows:\n\n\n# Validate fold: use only loss for tuning\n    metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_function, device)\ndf_eval = sum(loss_values.values()) / len(loss_values.values())\n\nThe results are averaged over the \\(k\\) folds and returned as df_eval.\n\n\nDetailed Description of the \"test_cv\" Setting\nIt uses the loss function specfied in fun_control and the metric specified in fun_control.\n\nFirst, the method HyperTorch().fun_torch is called.\nfun_torc() calls spotPython.torch.traintest.evaluate_cv() as follows:\n\n\ndf_eval, _ = evaluate_cv(\n    model,\n    dataset=fun_control[\"test\"],\n    shuffle=self.fun_control[\"shuffle\"],\n    device=self.fun_control[\"device\"],\n    show_batch_interval=self.fun_control[\"show_batch_interval\"],\n)\n\nNote: The data set fun_control[\"test\"] is used for CV. The rest is the same as for the \"train_cv\" setting.\n\n\nDetailed Description of the Final Model Training and Evaluation\n\nDetailed Description of the \"train_tuned Procedure\ntrain_tuned() is just a wrapper to evaluate_hold_out using the train data set. It is implemented as follows:\n\ndef train_tuned(net, train_dataset, shuffle, loss_function, metric, device=None, show_batch_interval=10_000, path=None):\n    evaluate_hold_out(\n        net=net,\n        train_dataset=train_dataset,\n        shuffle=shuffle,\n        test_dataset=None,\n        loss_function=loss_function,\n        metric=metric,\n        device=device,\n        show_batch_interval=show_batch_interval,\n        path=path,\n    )\n\nThe test_tuned() procedure is implemented as follows:\n\ndef test_tuned(net, shuffle, test_dataset=None, loss_function=None, metric=None, device=None, path=None):\n    batch_size_instance = net.batch_size\n    removed_attributes, net = get_removed_attributes_and_base_net(net)\n    if path is not None:\n        net.load_state_dict(torch.load(path))\n        net.eval()\n    try:\n        device = getDevice(device=device)\n        if torch.cuda.is_available():\n            device = \"cuda:0\"\n            if torch.cuda.device_count() &gt; 1:\n                print(\"We will use\", torch.cuda.device_count(), \"GPUs!\")\n                net = nn.DataParallel(net)\n        net.to(device)\n        valloader = torch.utils.data.DataLoader(\n            test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle, num_workers=0\n        )\n        metric_value, loss = validate_fold_or_hold_out(\n            net, valloader=valloader, loss_function=loss_function, metric=metric, device=device\n        )\n        df_eval = loss\n        df_metric = metric_value\n        df_preds = np.nan\n    except Exception as err:\n        print(f\"Error in Net_Core. Call to test_tuned() failed. {err=}, {type(err)=}\")\n        df_eval = np.nan\n        df_metric = np.nan\n        df_preds = np.nan\n    add_attributes(net, removed_attributes)\n    print(f\"Final evaluation: Validation loss: {df_eval}\")\n    print(f\"Final evaluation: Validation metric: {df_metric}\")\n    print(\"----------------------------------------------\")\n    return df_eval, df_preds, df_metric",
+        "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
+    },
+    {
         "href": "bart23e.html#footnotes",
         "objectID": "bart23e.html#footnotes",
         "section": "Footnotes",
         "text": "Footnotes\n\n\nhttps://github.com/sequential-parameter-optimization\u21a9\ufe0e\nAlternatively, the source code can be downloaded from gitHub: https://github.com/sequential-parameter-optimization/spotPython.\u21a9\ufe0e\nWe were not able to install Ray Tune on our system. Therefore, we used the results from the PyTorch tutorial.\u21a9\ufe0e\nhttps://torchmetrics.readthedocs.io/en/latest/.\u21a9\ufe0e",
         "title": "PyTorch Hyperparameter Tuning \u2014 A Tutorial for spotPython"
     }
 ]
```

### Comparing `spotPython-0.2.1/docs/site_libs/bootstrap/bootstrap-icons.css` & `spotPython-0.2.2/docs/site_libs/bootstrap/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/bootstrap/bootstrap-icons.woff` & `spotPython-0.2.2/docs/site_libs/bootstrap/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/bootstrap/bootstrap.min.css` & `spotPython-0.2.2/docs/site_libs/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/bootstrap/bootstrap.min.js` & `spotPython-0.2.2/docs/site_libs/bootstrap/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/clipboard/clipboard.min.js` & `spotPython-0.2.2/docs/site_libs/clipboard/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-html/anchor.min.js` & `spotPython-0.2.2/docs/site_libs/quarto-html/anchor.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-html/popper.min.js` & `spotPython-0.2.2/docs/site_libs/quarto-html/popper.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-html/quarto-syntax-highlighting.css` & `spotPython-0.2.2/docs/site_libs/quarto-html/quarto-syntax-highlighting.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-html/quarto.js` & `spotPython-0.2.2/docs/site_libs/quarto-html/quarto.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-html/tippy.css` & `spotPython-0.2.2/docs/site_libs/quarto-html/tippy.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-html/tippy.umd.min.js` & `spotPython-0.2.2/docs/site_libs/quarto-html/tippy.umd.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-nav/quarto-nav.js` & `spotPython-0.2.2/docs/site_libs/quarto-nav/quarto-nav.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-search/autocomplete.umd.js` & `spotPython-0.2.2/docs/site_libs/quarto-search/autocomplete.umd.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-search/fuse.min.js` & `spotPython-0.2.2/docs/site_libs/quarto-search/fuse.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/docs/site_libs/quarto-search/quarto-search.js` & `spotPython-0.2.2/docs/site_libs/quarto-search/quarto-search.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/00_spot_doc.ipynb` & `spotPython-0.2.2/notebooks/00_spot_doc.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/01_spot_intro.ipynb` & `spotPython-0.2.2/notebooks/01_spot_intro.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/02_spot_multidim.ipynb` & `spotPython-0.2.2/notebooks/02_spot_multidim.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/03_spot_anisotropic.ipynb` & `spotPython-0.2.2/notebooks/03_spot_anisotropic.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/04_spot_sklearn_surrogate.ipynb` & `spotPython-0.2.2/notebooks/04_spot_sklearn_surrogate.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/05_spot_sklearn_optimizers.ipynb` & `spotPython-0.2.2/notebooks/05_spot_sklearn_optimizers.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/06_spot_gaussian.ipynb` & `spotPython-0.2.2/notebooks/06_spot_gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/07_spot_ei.ipynb` & `spotPython-0.2.2/notebooks/07_spot_ei.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/08_spot_noisy.ipynb` & `spotPython-0.2.2/notebooks/08_spot_noisy.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/09_spot_ocba.ipynb` & `spotPython-0.2.2/notebooks/09_spot_ocba.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/10_spot_hpt_sklearn_classification.ipynb` & `spotPython-0.2.2/notebooks/10_spot_hpt_sklearn_classification.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb` & `spotPython-0.2.2/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/12_spot_hpt_torch_cifar10.ipynb` & `spotPython-0.2.2/notebooks/12_spot_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb` & `spotPython-0.2.2/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/15_spot_hpt_sklearn_regression.ipynb` & `spotPython-0.2.2/notebooks/15_spot_hpt_sklearn_regression.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/data/torch/model_spot_trained.pt` & `spotPython-0.2.2/notebooks/data/torch/model_spot_trained.pt`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png` & `spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png` & `spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png` & `spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png` & `spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png` & `spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png` & `spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png` & `spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png` & `spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png` & `spotPython-0.2.2/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/spotModel.graffle` & `spotPython-0.2.2/notebooks/figures/spotModel.graffle`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/spotModel.pdf` & `spotPython-0.2.2/notebooks/figures/spotModel.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures/spotModel.png` & `spotPython-0.2.2/notebooks/figures/spotModel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png` & `spotPython-0.2.2/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/notebooks/plot.png` & `spotPython-0.2.2/notebooks/plot.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/pyproject.toml` & `spotPython-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotPython"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotPython - Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotPython-0.2.1/src/spotPython/budget/ocba.py` & `spotPython-0.2.2/src/spotPython/budget/ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/build/kriging.py` & `spotPython-0.2.2/src/spotPython/build/kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/data/base.py` & `spotPython-0.2.2/src/spotPython/data/base.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/data/sklearn_hyper_dict.json` & `spotPython-0.2.2/src/spotPython/data/sklearn_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/data/torch_hyper_dict.json` & `spotPython-0.2.2/src/spotPython/data/torch_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/design/spacefilling.py` & `spotPython-0.2.2/src/spotPython/design/spacefilling.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/fun/hypertorch.py` & `spotPython-0.2.2/src/spotPython/fun/hypertorch.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/fun/objectivefunctions.py` & `spotPython-0.2.2/src/spotPython/fun/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/hyperparameters/categorical.py` & `spotPython-0.2.2/src/spotPython/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/hyperparameters/optimizer.py` & `spotPython-0.2.2/src/spotPython/hyperparameters/optimizer.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/hyperparameters/values.py` & `spotPython-0.2.2/src/spotPython/hyperparameters/values.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/plot/contour.py` & `spotPython-0.2.2/src/spotPython/plot/contour.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/plot/validation.py` & `spotPython-0.2.2/src/spotPython/plot/validation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/spot/spot.py` & `spotPython-0.2.2/src/spotPython/spot/spot.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/torch/netcifar10.py` & `spotPython-0.2.2/src/spotPython/torch/netcifar10.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/torch/netfashionMNIST.py` & `spotPython-0.2.2/src/spotPython/torch/netfashionMNIST.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/torch/traintest.py` & `spotPython-0.2.2/src/spotPython/torch/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/aggregate.py` & `spotPython-0.2.2/src/spotPython/utils/aggregate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/compare.py` & `spotPython-0.2.2/src/spotPython/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/convert.py` & `spotPython-0.2.2/src/spotPython/utils/convert.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/device.py` & `spotPython-0.2.2/src/spotPython/utils/device.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/eda.py` & `spotPython-0.2.2/src/spotPython/utils/eda.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/init.py` & `spotPython-0.2.2/src/spotPython/utils/init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/metrics.py` & `spotPython-0.2.2/src/spotPython/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/progress.py` & `spotPython-0.2.2/src/spotPython/utils/progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/repair.py` & `spotPython-0.2.2/src/spotPython/utils/repair.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython/utils/transform.py` & `spotPython-0.2.2/src/spotPython/utils/transform.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/src/spotPython.egg-info/PKG-INFO` & `spotPython-0.2.2/src/spotPython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.2.1
+Version: 0.2.2
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.2.1/src/spotPython.egg-info/SOURCES.txt` & `spotPython-0.2.2/src/spotPython.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 src/spotPython/fun/hypertorch.py
 src/spotPython/fun/objectivefunctions.py
 src/spotPython/hyperparameters/categorical.py
 src/spotPython/hyperparameters/optimizer.py
 src/spotPython/hyperparameters/values.py
 src/spotPython/plot/contour.py
 src/spotPython/plot/validation.py
+src/spotPython/sklearn/traintest.py
 src/spotPython/spot/spot.py
 src/spotPython/torch/netcifar10.py
 src/spotPython/torch/netcore.py
 src/spotPython/torch/netfashionMNIST.py
 src/spotPython/torch/traintest.py
 src/spotPython/utils/aggregate.py
 src/spotPython/utils/classes.py
```

### Comparing `spotPython-0.2.1/test/test_aggregate_mean_var.py` & `spotPython-0.2.2/test/test_aggregate_mean_var.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_build_Psi.py` & `spotPython-0.2.2/test/test_build_Psi.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_build_U.py` & `spotPython-0.2.2/test/test_build_U.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_build_psi_vec.py` & `spotPython-0.2.2/test/test_build_psi_vec.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_evaluate_new_X.py` & `spotPython-0.2.2/test/test_evaluate_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_evaluate_new_solutions.py` & `spotPython-0.2.2/test/test_evaluate_new_solutions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_extract_from_bounds.py` & `spotPython-0.2.2/test/test_extract_from_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_generate_design.py` & `spotPython-0.2.2/test/test_generate_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_infill.py` & `spotPython-0.2.2/test/test_infill.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_nat_to_cod.py` & `spotPython-0.2.2/test/test_nat_to_cod.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_nat_to_cod_init.py` & `spotPython-0.2.2/test/test_nat_to_cod_init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_ocba.py` & `spotPython-0.2.2/test/test_ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_repair_non_numeric.py` & `spotPython-0.2.2/test/test_repair_non_numeric.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_set_de_bounds.py` & `spotPython-0.2.2/test/test_set_de_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_show_progress.py` & `spotPython-0.2.2/test/test_show_progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_suggest_new_X.py` & `spotPython-0.2.2/test/test_suggest_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.1/test/test_update_surrogate.py` & `spotPython-0.2.2/test/test_update_surrogate.py`

 * *Files identical despite different names*

