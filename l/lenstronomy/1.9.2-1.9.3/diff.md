# Comparing `tmp/lenstronomy-1.9.2.tar.gz` & `tmp/lenstronomy-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenstronomy-1.9.2.tar", last modified: Sun Dec 12 19:44:22 2021, max compression
+gzip compressed data, was "lenstronomy-1.9.3.tar", last modified: Wed Dec 22 14:55:12 2021, max compression
```

## Comparing `lenstronomy-1.9.2.tar` & `lenstronomy-1.9.3.tar`

### file list

```diff
@@ -1,969 +1,969 @@
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.413382 lenstronomy-1.9.2/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:21.869716 lenstronomy-1.9.2/.github/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:21.891555 lenstronomy-1.9.2/.github/workflows/
--rw-r--r--   0 sibirrer   (501) staff       (20)     1947 2021-10-28 20:30:23.000000 lenstronomy-1.9.2/.github/workflows/ci_test.yml
--rw-r--r--   0 sibirrer   (501) staff       (20)      422 2019-05-28 01:02:43.000000 lenstronomy-1.9.2/.gitignore
--rw-r--r--   0 sibirrer   (501) staff       (20)      603 2021-12-11 18:31:29.000000 lenstronomy-1.9.2/.readthedocs.yml
--rw-r--r--   0 sibirrer   (501) staff       (20)      750 2020-02-15 05:36:21.000000 lenstronomy-1.9.2/.travis.yml
--rw-r--r--   0 sibirrer   (501) staff       (20)     2835 2021-11-26 19:23:09.000000 lenstronomy-1.9.2/AFFILIATEDPACKAGES.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1774 2021-11-30 17:45:54.000000 lenstronomy-1.9.2/AUTHORS.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     7477 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/CONTRIBUTING.md
--rw-r--r--   0 sibirrer   (501) staff       (20)       31 2020-02-15 05:36:21.000000 lenstronomy-1.9.2/Gemfile
--rw-r--r--   0 sibirrer   (501) staff       (20)     6855 2021-12-12 19:19:53.000000 lenstronomy-1.9.2/HISTORY.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1095 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/LICENSE
--rw-r--r--   0 sibirrer   (501) staff       (20)      456 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/MAILINGLIST.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      261 2021-09-17 17:39:06.000000 lenstronomy-1.9.2/MANIFEST.in
--rw-r--r--   0 sibirrer   (501) staff       (20)     1341 2021-09-03 21:13:49.000000 lenstronomy-1.9.2/Makefile
--rw-r--r--   0 sibirrer   (501) staff       (20)    10628 2021-12-12 19:44:22.413510 lenstronomy-1.9.2/PKG-INFO
--rw-r--r--   0 sibirrer   (501) staff       (20)    18101 2021-12-09 05:54:15.000000 lenstronomy-1.9.2/PUBLISHED.rst
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:21.893597 lenstronomy-1.9.2/Paper/
--rw-r--r--   0 sibirrer   (501) staff       (20)    73738 2021-08-02 20:31:35.000000 lenstronomy-1.9.2/Paper/paper.bib
--rw-r--r--   0 sibirrer   (501) staff       (20)    16009 2021-08-02 20:31:35.000000 lenstronomy-1.9.2/Paper/paper.md
--rw-r--r--   0 sibirrer   (501) staff       (20)   288390 2021-08-02 20:31:35.000000 lenstronomy-1.9.2/Paper/paper_fig.png
--rw-r--r--   0 sibirrer   (501) staff       (20)     9864 2021-10-28 20:30:23.000000 lenstronomy-1.9.2/README.rst
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:21.925357 lenstronomy-1.9.2/docs/
--rw-r--r--   0 sibirrer   (501) staff       (20)     1195 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/.coverage
--rw-r--r--   0 sibirrer   (501) staff       (20)     6777 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/Makefile
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:21.870365 lenstronomy-1.9.2/docs/_build/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:21.991605 lenstronomy-1.9.2/docs/_build/doctrees/
--rw-r--r--   0 sibirrer   (501) staff       (20)    15988 2021-12-08 00:08:16.000000 lenstronomy-1.9.2/docs/_build/doctrees/affiliatedpackages.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    20390 2021-12-08 00:08:16.000000 lenstronomy-1.9.2/docs/_build/doctrees/authors.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    41548 2021-12-08 00:08:16.000000 lenstronomy-1.9.2/docs/_build/doctrees/contributing.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)  2445960 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 sibirrer   (501) staff       (20)    46805 2021-12-08 00:08:16.000000 lenstronomy-1.9.2/docs/_build/doctrees/history.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    58849 2021-12-08 00:08:16.000000 lenstronomy-1.9.2/docs/_build/doctrees/index.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    14500 2021-12-08 00:08:16.000000 lenstronomy-1.9.2/docs/_build/doctrees/installation.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   258972 2021-12-08 00:08:18.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Analysis.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   168875 2021-12-08 00:08:19.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Cosmo.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    81278 2021-12-08 00:08:19.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Data.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   386510 2021-12-08 00:08:20.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.GalKin.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   135356 2021-12-08 00:08:20.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.ImSim.MultiBand.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   158153 2021-12-08 00:08:20.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.ImSim.Numerics.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   181209 2021-12-08 00:08:20.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.ImSim.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    22941 2021-12-08 00:08:21.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.LightConeSim.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)  3252051 2021-12-08 00:08:26.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.Profiles.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    89092 2021-12-08 00:08:26.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.QuadOptimizer.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   140969 2021-12-08 00:08:26.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.Solver.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   315367 2021-12-08 00:08:21.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   574910 2021-12-08 00:08:27.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LightModel.Profiles.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    28715 2021-12-08 00:08:27.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LightModel.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   291807 2021-12-08 00:08:29.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Plots.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   105421 2021-12-08 00:08:29.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.PointSource.Types.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   128020 2021-12-08 00:08:29.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.PointSource.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    95058 2021-12-08 00:08:29.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Sampling.Likelihoods.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    44878 2021-12-08 00:08:30.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Sampling.Pool.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    76703 2021-12-08 00:08:30.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Sampling.Samplers.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   165307 2021-12-08 00:08:29.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Sampling.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    46618 2021-12-08 00:08:30.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.SimulationAPI.ObservationConfig.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   127487 2021-12-08 00:08:30.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.SimulationAPI.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   535448 2021-12-08 00:08:31.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Util.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   287625 2021-12-08 00:08:31.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Workflow.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)     3981 2021-12-08 00:08:16.000000 lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)     4427 2021-12-08 00:08:31.000000 lenstronomy-1.9.2/docs/_build/doctrees/mailinglist.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)     2695 2021-12-08 00:08:31.000000 lenstronomy-1.9.2/docs/_build/doctrees/modules.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)   141212 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/doctrees/published.doctree
--rw-r--r--   0 sibirrer   (501) staff       (20)    24877 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/doctrees/usage.doctree
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.042619 lenstronomy-1.9.2/docs/_build/html/
--rw-r--r--   0 sibirrer   (501) staff       (20)      230 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/.buildinfo
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.042932 lenstronomy-1.9.2/docs/_build/html/_modules/
--rw-r--r--   0 sibirrer   (501) staff       (20)    23857 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/index.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:21.874222 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.046072 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/
--rw-r--r--   0 sibirrer   (501) staff       (20)    77355 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/kinematics_api.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    43476 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/lens_profile.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    16224 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/light2mass.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    34232 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/light_profile.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    36443 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/td_cosmography.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.049351 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/
--rw-r--r--   0 sibirrer   (501) staff       (20)    13695 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/background.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    26335 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/cosmo_solver.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    10431 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/kde_likelihood.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    13287 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/lcdm.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    49556 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/lens_cosmo.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20133 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/nfw_param.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.050721 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Data/
--rw-r--r--   0 sibirrer   (501) staff       (20)    23200 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Data/coord_transforms.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    17660 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Data/imaging_data.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    30799 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Data/psf.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.057775 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/
--rw-r--r--   0 sibirrer   (501) staff       (20)    37492 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/analytic_kinematics.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    63137 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/anisotropy.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     9384 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/aperture.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    33921 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/aperture_types.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    10060 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/cosmo.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    22737 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/galkin.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    15490 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/galkin_model.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    46730 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/light_profile.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    61939 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/numeric_kinematics.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     5362 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/observation.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    12191 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/psf.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    22127 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/velocity_util.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.060815 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.063689 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/
--rw-r--r--   0 sibirrer   (501) staff       (20)    30648 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/joint_linear.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    15531 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/multi_data_base.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20653 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/multi_linear.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    40022 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/single_band_multi_model.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.070283 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/
--rw-r--r--   0 sibirrer   (501) staff       (20)    15522 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/adaptive_numerics.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    61422 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/convolution.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    45201 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/grid.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    43260 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/numba_convolution.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    31131 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/numerics.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    13719 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/partial_image.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    17303 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/point_source_rendering.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    17449 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/de_lens.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    47001 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/image2source_mapping.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    91252 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/image_linear_solve.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    66368 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/image_model.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.074954 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.075606 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/LightConeSim/
--rw-r--r--   0 sibirrer   (501) staff       (20)    21359 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/LightConeSim/light_cone.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.115418 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/
--rw-r--r--   0 sibirrer   (501) staff       (20)    30372 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/arc_perturbations.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    12515 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/base_profile.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   132820 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/chameleon.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    70183 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cnfw.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    27677 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cnfw_ellipse.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    23800 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/const_mag.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    10228 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/constant_shift.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    11984 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/convergence.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   105656 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/coreBurkert.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    34905 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    38222 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_2.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    35823 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_exp.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20235 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_mst.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    38251 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_const.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    32133 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_sis_mst.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    28595 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_spp.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    21960 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_spt.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    34474 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_tan_diff.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    22901 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/dipole.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    67632 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/elliptical_density_slice.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    47893 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/epl.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    34219 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/epl_numba.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    13428 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/flexion.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    18093 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/flexionfg.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    97965 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gauss_decomposition.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    68901 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_ellipse_kappa.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    30528 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_ellipse_potential.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    43585 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_kappa.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    14828 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_potential.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    48687 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hernquist.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    30408 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hernquist_ellipse.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    13788 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hessian.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    75930 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/interpol.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    46790 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/multi_gaussian_kappa.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20060 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/multipole.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    75261 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    28198 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_ellipse.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20937 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_mass_concentration.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    23516 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_vir_trunc.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    51488 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nie.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    42446 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nie_potential.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    15051 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/numerical_deflections.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    51307 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/p_jaffe.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    24027 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/p_jaffe_ellipse.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20705 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/pemd.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    19747 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/point_mass.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20859 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    38612 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_ellipse_kappa.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    23006 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_ellipse_potential.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    37823 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_utils.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    50460 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shapelet_pot_cartesian.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    58374 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shapelet_pot_polar.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    37365 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shear.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    32646 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sie.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    29440 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sis.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    31044 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sis_truncate.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    44696 2021-12-08 00:08:37.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spemd.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    37745 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spep.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    47279 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/splcore.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    40778 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spp.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    75831 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/tnfw.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    47696 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/uldm.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.117738 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/
--rw-r--r--   0 sibirrer   (501) staff       (20)    30642 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/multi_plane_fast.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    23390 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/optimizer.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    37799 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/param_manager.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.120808 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Solver/
--rw-r--r--   0 sibirrer   (501) staff       (20)    84323 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Solver/lens_equation_solver.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    14864 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    42583 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver2point.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    52153 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver4point.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    28880 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/convergence_integrals.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    72595 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/lens_model.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   141411 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/lens_model_extensions.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    38113 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/lens_param.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    16285 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/profile_integrals.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    57055 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/profile_list_base.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    34593 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/single_plane.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.121895 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.130785 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/
--rw-r--r--   0 sibirrer   (501) staff       (20)    45062 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/chameleon.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    12482 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/ellipsoid.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    50201 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/gaussian.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    17824 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/hernquist.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20932 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/interpolation.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     9146 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/moffat.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    14377 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/nie.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    18287 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/p_jaffe.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    14596 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/power_law.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    25617 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/sersic.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    56529 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/shapelets.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    66260 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/shapelets_polar.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     6300 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/uniform.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     8159 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/light_model.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    40966 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/light_param.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.137579 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/
--rw-r--r--   0 sibirrer   (501) staff       (20)    38482 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/chain_plot.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    97701 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/lens_plot.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   152673 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/model_band_plot.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    42350 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/model_plot.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    47376 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/plot_util.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.139819 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.141636 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/Types/
--rw-r--r--   0 sibirrer   (501) staff       (20)    17313 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/Types/base_ps.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    21193 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/Types/lensed_position.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20162 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/Types/source_position.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    10598 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/Types/unlensed.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    67316 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/point_source.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    18698 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/point_source_cached.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    44695 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/point_source_param.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.144569 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.146716 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/
--rw-r--r--   0 sibirrer   (501) staff       (20)    16054 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/image_likelihood.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    44713 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/position_likelihood.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    33463 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/prior_likelihood.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    15293 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/time_delay_likelihood.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.147572 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Pool/
--rw-r--r--   0 sibirrer   (501) staff       (20)    16736 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Pool/multiprocessing.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    12748 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Pool/pool.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.149396 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/
--rw-r--r--   0 sibirrer   (501) staff       (20)    12805 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/base_nested_sampler.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    23802 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/dynesty_sampler.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    30665 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/multinest_sampler.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    36330 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/polychord_sampler.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    56765 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/likelihood.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   122506 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/parameters.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    37833 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/sampler.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    49306 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/special_param.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.152487 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.154803 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/
--rw-r--r--   0 sibirrer   (501) staff       (20)    16716 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/DES.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    11721 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/Euclid.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    14063 2021-12-08 00:08:38.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/HST.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    18473 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/LSST.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    10371 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/data_api.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    21958 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/model_api.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    44306 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/observation_api.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    11062 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/observation_constructor.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20441 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/point_source_variability.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    18007 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/sim_api.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.169105 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/
--rw-r--r--   0 sibirrer   (501) staff       (20)    30616 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/analysis_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    36056 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/class_creator.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     8010 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/constants.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     8405 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/correlation.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    13715 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/data_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20135 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/derivative_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    56899 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/image_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    92234 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/kernel_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    17040 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/mask_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    15414 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/multi_gauss_expansion.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    17719 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/numba_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    22707 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/param_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    25878 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/prob_density.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    22985 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/sampling_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    12910 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/simulation_util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   106662 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/util.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.172671 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Workflow/
--rw-r--r--   0 sibirrer   (501) staff       (20)    24610 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Workflow/alignment_matching.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    88074 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Workflow/fitting_sequence.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   107519 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Workflow/psf_fitting.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    66434 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Workflow/update_manager.html
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.186190 lenstronomy-1.9.2/docs/_build/html/_sources/
--rw-r--r--   0 sibirrer   (501) staff       (20)       38 2020-01-25 06:27:26.000000 lenstronomy-1.9.2/docs/_build/html/_sources/affiliatedpackages.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)       27 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/_build/html/_sources/authors.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      116 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/docs/_build/html/_sources/contributing.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)       27 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/_build/html/_sources/history.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      649 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     2767 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/_build/html/_sources/installation.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1182 2019-12-04 01:20:28.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Analysis.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1262 2020-03-31 14:44:06.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Cosmo.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      738 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Data.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     2400 2020-03-31 14:44:06.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.GalKin.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1135 2019-05-23 03:37:31.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.ImSim.MultiBand.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1725 2019-05-23 03:37:31.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.ImSim.Numerics.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1066 2019-05-23 03:37:31.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.ImSim.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      481 2020-01-16 13:20:36.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LensModel.LightConeSim.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)    14055 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LensModel.Profiles.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      975 2020-12-17 01:32:55.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LensModel.QuadOptimizer.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1132 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LensModel.Solver.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1901 2021-12-07 21:58:06.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LensModel.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     3023 2019-11-06 19:40:51.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LightModel.Profiles.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      694 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LightModel.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1102 2019-11-06 19:40:51.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Plots.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1106 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.PointSource.Types.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      942 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.PointSource.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1236 2019-04-13 18:55:33.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Sampling.Likelihoods.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      622 2020-04-05 22:07:20.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Sampling.Pool.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1179 2019-07-06 16:40:32.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Sampling.Samplers.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1093 2020-04-05 22:10:59.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Sampling.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1223 2020-09-07 18:48:43.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.SimulationAPI.ObservationConfig.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1605 2020-09-07 18:54:25.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.SimulationAPI.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     3069 2019-12-04 01:20:28.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Util.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     1015 2019-02-01 19:49:19.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Workflow.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      536 2021-12-08 00:08:10.000000 lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)       31 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/_build/html/_sources/mailinglist.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)       70 2021-12-08 00:08:10.000000 lenstronomy-1.9.2/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)       29 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/_build/html/_sources/published.rst.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     3966 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/_build/html/_sources/usage.rst.txt
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.192049 lenstronomy-1.9.2/docs/_build/html/_static/
--rw-r--r--   0 sibirrer   (501) staff       (20)    14667 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_static/basic.css
--rw-r--r--   0 sibirrer   (501) staff       (20)     4256 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_static/classic.css
--rw-r--r--   0 sibirrer   (501) staff       (20)       28 2021-12-07 21:51:58.000000 lenstronomy-1.9.2/docs/_build/html/_static/default.css
--rw-r--r--   0 sibirrer   (501) staff       (20)     9630 2021-12-07 21:51:58.000000 lenstronomy-1.9.2/docs/_build/html/_static/doctools.js
--rw-r--r--   0 sibirrer   (501) staff       (20)      355 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 sibirrer   (501) staff       (20)      286 2021-12-07 21:51:58.000000 lenstronomy-1.9.2/docs/_build/html/_static/file.png
--rw-r--r--   0 sibirrer   (501) staff       (20)    89476 2021-12-07 21:51:58.000000 lenstronomy-1.9.2/docs/_build/html/_static/jquery.js
--rw-r--r--   0 sibirrer   (501) staff       (20)       90 2021-12-07 21:51:58.000000 lenstronomy-1.9.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 sibirrer   (501) staff       (20)       90 2021-12-07 21:51:58.000000 lenstronomy-1.9.2/docs/_build/html/_static/plus.png
--rw-r--r--   0 sibirrer   (501) staff       (20)     4846 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_static/pygments.css
--rw-r--r--   0 sibirrer   (501) staff       (20)    16793 2021-12-07 21:51:58.000000 lenstronomy-1.9.2/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 sibirrer   (501) staff       (20)     4803 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/_static/sidebar.js
--rw-r--r--   0 sibirrer   (501) staff       (20)    19530 2021-12-07 21:51:58.000000 lenstronomy-1.9.2/docs/_build/html/_static/underscore.js
--rw-r--r--   0 sibirrer   (501) staff       (20)     8317 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/affiliatedpackages.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     8506 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/authors.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    18156 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/contributing.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   427308 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/genindex.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20221 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/history.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    29132 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/index.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     9254 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/installation.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    92949 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Analysis.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     7568 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Conf.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    69491 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Cosmo.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    33715 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Data.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   140488 2021-12-08 00:08:33.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.GalKin.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    55472 2021-12-08 00:08:33.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.ImSim.MultiBand.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    65023 2021-12-08 00:08:33.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.ImSim.Numerics.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    72214 2021-12-08 00:08:33.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.ImSim.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    13077 2021-12-08 00:08:33.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.LightConeSim.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    43961 2021-12-08 00:08:33.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.MultiPlane.html
--rw-r--r--   0 sibirrer   (501) staff       (20)  1168562 2021-12-08 00:08:34.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.Profiles.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    39749 2021-12-08 00:08:34.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.QuadOptimizer.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    52776 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.Solver.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    20841 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.Util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   130191 2021-12-08 00:08:33.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   215054 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.LightModel.Profiles.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    18614 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.LightModel.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   110961 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Plots.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    42614 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.PointSource.Types.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    51099 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.PointSource.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    40530 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Sampling.Likelihoods.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    19436 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Sampling.Pool.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    33968 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Sampling.Samplers.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    68897 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Sampling.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    22071 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.SimulationAPI.ObservationConfig.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    53581 2021-12-08 00:08:35.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.SimulationAPI.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   199118 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Util.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   102796 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.Workflow.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    55006 2021-12-08 00:08:32.000000 lenstronomy-1.9.2/docs/_build/html/lenstronomy.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     4934 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/mailinglist.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    24013 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/modules.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    14405 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/objects.inv
--rw-r--r--   0 sibirrer   (501) staff       (20)    32516 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/published.html
--rw-r--r--   0 sibirrer   (501) staff       (20)    62683 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/py-modindex.html
--rw-r--r--   0 sibirrer   (501) staff       (20)     3392 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/search.html
--rw-r--r--   0 sibirrer   (501) staff       (20)   162096 2021-12-08 00:08:39.000000 lenstronomy-1.9.2/docs/_build/html/searchindex.js
--rw-r--r--   0 sibirrer   (501) staff       (20)    10073 2021-12-08 00:08:36.000000 lenstronomy-1.9.2/docs/_build/html/usage.html
--rw-r--r--   0 sibirrer   (501) staff       (20)       38 2020-01-25 06:27:26.000000 lenstronomy-1.9.2/docs/affiliatedpackages.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)       27 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/authors.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      515 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/check_sphinx.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8380 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/conf.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      116 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/docs/contributing.rst
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.192520 lenstronomy-1.9.2/docs/figures/
--rw-r--r--   0 sibirrer   (501) staff       (20)   322886 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/figures/readme_fig.png
--rw-r--r--   0 sibirrer   (501) staff       (20)       27 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/history.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      649 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/index.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     2767 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/installation.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     2641 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/junit-docs-ci.xml
--rw-r--r--   0 sibirrer   (501) staff       (20)     1182 2019-12-04 01:20:28.000000 lenstronomy-1.9.2/docs/lenstronomy.Analysis.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      382 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/docs/lenstronomy.Conf.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1262 2020-03-31 14:44:06.000000 lenstronomy-1.9.2/docs/lenstronomy.Cosmo.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      738 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/lenstronomy.Data.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     2400 2020-03-31 14:44:06.000000 lenstronomy-1.9.2/docs/lenstronomy.GalKin.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1135 2019-05-23 03:37:31.000000 lenstronomy-1.9.2/docs/lenstronomy.ImSim.MultiBand.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1725 2019-05-23 03:37:31.000000 lenstronomy-1.9.2/docs/lenstronomy.ImSim.Numerics.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1066 2019-05-23 03:37:31.000000 lenstronomy-1.9.2/docs/lenstronomy.ImSim.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      481 2020-01-16 13:20:36.000000 lenstronomy-1.9.2/docs/lenstronomy.LensModel.LightConeSim.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      715 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/docs/lenstronomy.LensModel.MultiPlane.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)    14055 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/lenstronomy.LensModel.Profiles.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      975 2020-12-17 01:32:55.000000 lenstronomy-1.9.2/docs/lenstronomy.LensModel.QuadOptimizer.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1132 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/lenstronomy.LensModel.Solver.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      420 2021-12-07 21:52:15.000000 lenstronomy-1.9.2/docs/lenstronomy.LensModel.Util.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1901 2021-12-07 21:58:06.000000 lenstronomy-1.9.2/docs/lenstronomy.LensModel.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     3023 2019-11-06 19:40:51.000000 lenstronomy-1.9.2/docs/lenstronomy.LightModel.Profiles.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      694 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/lenstronomy.LightModel.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1102 2019-11-06 19:40:51.000000 lenstronomy-1.9.2/docs/lenstronomy.Plots.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1106 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/lenstronomy.PointSource.Types.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      942 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/lenstronomy.PointSource.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1236 2019-04-13 18:55:33.000000 lenstronomy-1.9.2/docs/lenstronomy.Sampling.Likelihoods.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      622 2020-04-05 22:07:20.000000 lenstronomy-1.9.2/docs/lenstronomy.Sampling.Pool.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1179 2019-07-06 16:40:32.000000 lenstronomy-1.9.2/docs/lenstronomy.Sampling.Samplers.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1093 2020-04-05 22:10:59.000000 lenstronomy-1.9.2/docs/lenstronomy.Sampling.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1223 2020-09-07 18:48:43.000000 lenstronomy-1.9.2/docs/lenstronomy.SimulationAPI.ObservationConfig.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1605 2020-09-07 18:54:25.000000 lenstronomy-1.9.2/docs/lenstronomy.SimulationAPI.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     3069 2019-12-04 01:20:28.000000 lenstronomy-1.9.2/docs/lenstronomy.Util.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)     1015 2019-02-01 19:49:19.000000 lenstronomy-1.9.2/docs/lenstronomy.Workflow.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)      536 2021-12-08 00:08:10.000000 lenstronomy-1.9.2/docs/lenstronomy.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)       31 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/mailinglist.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)       70 2021-12-08 00:08:10.000000 lenstronomy-1.9.2/docs/modules.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)       29 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/docs/published.rst
--rw-r--r--   0 sibirrer   (501) staff       (20)       66 2021-10-28 15:54:18.000000 lenstronomy-1.9.2/docs/requirements.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)     3966 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/docs/usage.rst
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.194255 lenstronomy-1.9.2/lenstronomy/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.202075 lenstronomy-1.9.2/lenstronomy/Analysis/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/Analysis/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10048 2021-02-15 19:18:04.000000 lenstronomy-1.9.2/lenstronomy/Analysis/image_reconstruction.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    25577 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/Analysis/kinematics_api.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10401 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/Analysis/lens_profile.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3097 2020-10-30 21:06:27.000000 lenstronomy-1.9.2/lenstronomy/Analysis/light2mass.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8912 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/Analysis/light_profile.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10613 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/Analysis/multi_patch_reconstruction.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11402 2021-10-25 18:10:27.000000 lenstronomy-1.9.2/lenstronomy/Analysis/td_cosmography.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.203203 lenstronomy-1.9.2/lenstronomy/Conf/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/Conf/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      931 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/Conf/conf_default.yaml
--rw-r--r--   0 sibirrer   (501) staff       (20)     1874 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/Conf/config_loader.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.209673 lenstronomy-1.9.2/lenstronomy/Cosmo/
--rw-r--r--   0 sibirrer   (501) staff       (20)      115 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1627 2021-11-26 19:23:09.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/_cosmo_interp_astropy_v4.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2385 2021-11-26 19:23:09.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/_cosmo_interp_astropy_v5.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2439 2021-03-03 19:21:56.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/background.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6973 2021-11-26 19:23:09.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/cosmo_interp.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4500 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/cosmo_solver.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1954 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/kde_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2320 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/lcdm.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10671 2021-10-06 21:46:19.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/lens_cosmo.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4001 2020-12-13 20:49:46.000000 lenstronomy-1.9.2/lenstronomy/Cosmo/nfw_param.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.213544 lenstronomy-1.9.2/lenstronomy/Data/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/Data/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5400 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/Data/coord_transforms.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5500 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Data/image_noise.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4968 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Data/imaging_data.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2176 2021-02-15 00:49:48.000000 lenstronomy-1.9.2/lenstronomy/Data/pixel_grid.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8336 2021-11-09 21:30:13.000000 lenstronomy-1.9.2/lenstronomy/Data/psf.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.221419 lenstronomy-1.9.2/lenstronomy/GalKin/
--rw-r--r--   0 sibirrer   (501) staff       (20)       83 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/GalKin/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8653 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/GalKin/analytic_kinematics.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12596 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/GalKin/anisotropy.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1724 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/GalKin/aperture.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7728 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/GalKin/aperture_types.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1763 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/GalKin/cosmo.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7851 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/GalKin/galkin.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5208 2020-12-22 20:20:25.000000 lenstronomy-1.9.2/lenstronomy/GalKin/galkin_model.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3749 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/GalKin/galkin_multiobservation.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11455 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/GalKin/light_profile.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    18059 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/GalKin/numeric_kinematics.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      418 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/GalKin/observation.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2251 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/GalKin/psf.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3284 2021-11-16 21:48:23.000000 lenstronomy-1.9.2/lenstronomy/GalKin/velocity_util.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.224477 lenstronomy-1.9.2/lenstronomy/ImSim/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.226894 lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-11-22 19:22:24.000000 lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8090 2021-02-10 19:13:54.000000 lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/joint_linear.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2931 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/multi_data_base.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6685 2020-10-30 03:00:29.000000 lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/multi_linear.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12547 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/single_band_multi_model.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.233672 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-04-27 21:27:23.000000 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4082 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/adaptive_numerics.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    15416 2021-10-01 20:56:04.000000 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/convolution.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11539 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/grid.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11712 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/numba_convolution.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9575 2021-10-01 16:53:19.000000 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/numerics.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7879 2021-07-08 17:17:42.000000 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/numerics_subframe.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2357 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/partial_image.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3494 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/point_source_rendering.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      115 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/ImSim/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2680 2020-12-29 06:38:34.000000 lenstronomy-1.9.2/lenstronomy/ImSim/de_lens.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1984 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/ImSim/differential_extinction.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12536 2021-09-03 21:13:41.000000 lenstronomy-1.9.2/lenstronomy/ImSim/image2source_mapping.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    28614 2021-10-05 15:56:32.000000 lenstronomy-1.9.2/lenstronomy/ImSim/image_linear_solve.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    20544 2021-09-03 21:13:41.000000 lenstronomy-1.9.2/lenstronomy/ImSim/image_model.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.236473 lenstronomy-1.9.2/lenstronomy/LensModel/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.237048 lenstronomy-1.9.2/lenstronomy/LensModel/LightConeSim/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-01-02 08:21:31.000000 lenstronomy-1.9.2/lenstronomy/LensModel/LightConeSim/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5152 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/lenstronomy/LensModel/LightConeSim/light_cone.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.238417 lenstronomy-1.9.2/lenstronomy/LensModel/MultiPlane/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/MultiPlane/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    16452 2021-09-03 21:13:41.000000 lenstronomy-1.9.2/lenstronomy/LensModel/MultiPlane/multi_plane.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    17290 2021-09-03 21:13:41.000000 lenstronomy-1.9.2/lenstronomy/LensModel/MultiPlane/multi_plane_base.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.267761 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/
--rw-r--r--   0 sibirrer   (501) staff       (20)      116 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6389 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/arc_perturbations.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2849 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/base_profile.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    28357 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/chameleon.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11840 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cnfw.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4132 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cnfw_ellipse.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5025 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/const_mag.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1626 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/constant_shift.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1862 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/convergence.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    15347 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/coreBurkert.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7022 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cored_density.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7825 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cored_density_2.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8054 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cored_density_exp.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4728 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cored_density_mst.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10251 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_const.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8133 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_sis_mst.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7173 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_spp.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5361 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_spt.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8534 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_tan_diff.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3495 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/dipole.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12684 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/elliptical_density_slice.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11797 2021-12-11 07:14:22.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/epl.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7201 2021-09-04 18:51:06.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/epl_numba.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1125 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/flexion.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3202 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/flexionfg.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    29497 2021-11-16 21:48:23.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gauss_decomposition.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    15621 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gaussian_ellipse_kappa.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4572 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gaussian_ellipse_potential.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6663 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gaussian_kappa.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1747 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gaussian_potential.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10076 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/hernquist.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5473 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/hernquist_ellipse.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2404 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/hessian.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    18794 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/interpol.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7461 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/multi_gaussian_kappa.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3296 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/multipole.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    15584 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nfw.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6277 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nfw_ellipse.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4176 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nfw_mass_concentration.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3519 2021-09-03 21:13:41.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nfw_vir_trunc.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10496 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nie.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8892 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nie_potential.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3269 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/numerical_deflections.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10420 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/p_jaffe.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3245 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/p_jaffe_ellipse.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5416 2021-11-12 00:53:27.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/pemd.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2766 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/point_mass.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3222 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sersic.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6674 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sersic_ellipse_kappa.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3312 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sersic_ellipse_potential.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7681 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sersic_utils.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9039 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/shapelet_pot_cartesian.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9633 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/shapelet_pot_polar.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7554 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/shear.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6503 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sie.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5375 2021-12-11 07:02:32.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sis.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4621 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sis_truncate.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11340 2021-12-07 22:04:00.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/spemd.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5969 2021-12-09 23:58:51.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/spep.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11232 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/splcore.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6508 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/spp.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    14193 2021-09-03 21:13:49.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/tnfw.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6518 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/tnfw_ellipse.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10793 2021-11-16 21:48:23.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/uldm.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.269967 lenstronomy-1.9.2/lenstronomy/LensModel/QuadOptimizer/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-12-02 02:08:01.000000 lenstronomy-1.9.2/lenstronomy/LensModel/QuadOptimizer/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7324 2021-09-03 21:13:41.000000 lenstronomy-1.9.2/lenstronomy/LensModel/QuadOptimizer/multi_plane_fast.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6116 2020-12-02 02:08:01.000000 lenstronomy-1.9.2/lenstronomy/LensModel/QuadOptimizer/optimizer.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9463 2020-12-02 02:08:01.000000 lenstronomy-1.9.2/lenstronomy/LensModel/QuadOptimizer/param_manager.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.272506 lenstronomy-1.9.2/lenstronomy/LensModel/Solver/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Solver/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    13847 2021-09-09 01:10:22.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Solver/epl_shear_solver.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    26224 2021-12-07 21:57:45.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Solver/lens_equation_solver.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3161 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Solver/solver.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8429 2021-01-03 05:32:38.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Solver/solver2point.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10148 2021-01-22 18:14:45.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Solver/solver4point.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.273221 lenstronomy-1.9.2/lenstronomy/LensModel/Util/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-09-04 18:31:10.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Util/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5326 2021-09-04 18:31:10.000000 lenstronomy-1.9.2/lenstronomy/LensModel/Util/epl_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/LensModel/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6764 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/LensModel/convergence_integrals.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    21232 2021-11-10 23:25:07.000000 lenstronomy-1.9.2/lenstronomy/LensModel/lens_model.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    37747 2021-11-16 21:48:23.000000 lenstronomy-1.9.2/lenstronomy/LensModel/lens_model_extensions.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9137 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LensModel/lens_param.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2955 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LensModel/profile_integrals.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    17872 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/lenstronomy/LensModel/profile_list_base.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7616 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LensModel/single_plane.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.275226 lenstronomy-1.9.2/lenstronomy/LightModel/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.282329 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7820 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/chameleon.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1675 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/ellipsoid.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10957 2021-03-08 04:47:32.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/gaussian.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2577 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/hernquist.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4287 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/interpolation.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1159 2021-12-07 18:51:02.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/moffat.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2722 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/nie.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2506 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/p_jaffe.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1947 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/power_law.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      810 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/profile_base.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5423 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/sersic.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12035 2021-12-07 18:07:04.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/shapelets.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12520 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/shapelets_polar.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7969 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/starlets.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3169 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/starlets_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      551 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/uniform.py
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/LightModel/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2148 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LightModel/light_model.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11725 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LightModel/light_model_base.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9702 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LightModel/light_param.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8805 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/LightModel/linear_basis.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.284486 lenstronomy-1.9.2/lenstronomy/Plots/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/Plots/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6093 2021-11-11 21:26:21.000000 lenstronomy-1.9.2/lenstronomy/Plots/chain_plot.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    23933 2021-11-30 16:52:36.000000 lenstronomy-1.9.2/lenstronomy/Plots/lens_plot.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    31919 2021-11-30 16:52:36.000000 lenstronomy-1.9.2/lenstronomy/Plots/model_band_plot.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10220 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Plots/model_plot.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9525 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/Plots/multi_patch_plot.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4379 2021-02-08 02:07:45.000000 lenstronomy-1.9.2/lenstronomy/Plots/plot_quasar_images.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9126 2021-11-30 16:52:36.000000 lenstronomy-1.9.2/lenstronomy/Plots/plot_util.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.286115 lenstronomy-1.9.2/lenstronomy/PointSource/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.288086 lenstronomy-1.9.2/lenstronomy/PointSource/Types/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/lenstronomy/PointSource/Types/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4102 2021-11-05 02:38:33.000000 lenstronomy-1.9.2/lenstronomy/PointSource/Types/base_ps.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5731 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/lenstronomy/PointSource/Types/lensed_position.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5441 2021-11-05 02:38:33.000000 lenstronomy-1.9.2/lenstronomy/PointSource/Types/source_position.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1911 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/lenstronomy/PointSource/Types/unlensed.py
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/PointSource/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    19125 2021-01-06 05:50:40.000000 lenstronomy-1.9.2/lenstronomy/PointSource/point_source.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4506 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/lenstronomy/PointSource/point_source_cached.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9817 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/lenstronomy/PointSource/point_source_param.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.291906 lenstronomy-1.9.2/lenstronomy/Sampling/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.294097 lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-04-06 20:25:36.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4000 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/flux_ratio_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4205 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/image_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12492 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/position_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8448 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/prior_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3421 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/time_delay_likelihood.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.295647 lenstronomy-1.9.2/lenstronomy/Sampling/Pool/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-03-31 20:11:58.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Pool/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4422 2020-09-07 19:40:59.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Pool/multiprocessing.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3675 2021-11-16 21:48:23.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Pool/pool.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.301523 lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-06-21 13:54:49.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2490 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/base_nested_sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6055 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/dynesty_sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7295 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/multinest_sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9155 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/polychord_sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    14647 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/pso.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      115 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/Sampling/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    17530 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/lenstronomy/Sampling/likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    39986 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/Sampling/parameters.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9596 2021-11-16 21:48:23.000000 lenstronomy-1.9.2/lenstronomy/Sampling/sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11491 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/Sampling/special_param.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.305993 lenstronomy-1.9.2/lenstronomy/SimulationAPI/
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.309944 lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/
--rw-r--r--   0 sibirrer   (501) staff       (20)     3830 2021-02-11 22:10:04.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/DES.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2574 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/Euclid.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3813 2021-10-25 16:41:19.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/HST.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4250 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/LSST.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3507 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/ZTF.py
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-08-03 19:28:48.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2157 2021-02-11 23:38:44.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/data_api.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6341 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/model_api.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    13045 2021-02-11 23:18:15.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/observation_api.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2064 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/observation_constructor.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4989 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/point_source_variability.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4391 2020-12-29 06:56:09.000000 lenstronomy-1.9.2/lenstronomy/SimulationAPI/sim_api.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.319003 lenstronomy-1.9.2/lenstronomy/Util/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/Util/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5210 2020-10-30 21:06:27.000000 lenstronomy-1.9.2/lenstronomy/Util/analysis_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12123 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/lenstronomy/Util/class_creator.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1123 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Util/constants.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1228 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Util/correlation.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3346 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/Util/data_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2710 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Util/derivative_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11371 2021-12-11 07:00:42.000000 lenstronomy-1.9.2/lenstronomy/Util/image_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    19127 2021-11-05 05:39:13.000000 lenstronomy-1.9.2/lenstronomy/Util/kernel_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5068 2021-02-08 02:07:45.000000 lenstronomy-1.9.2/lenstronomy/Util/magnification_finite_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2733 2020-10-30 21:15:33.000000 lenstronomy-1.9.2/lenstronomy/Util/mask_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2322 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Util/multi_gauss_expansion.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3119 2021-09-04 21:22:27.000000 lenstronomy-1.9.2/lenstronomy/Util/numba_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3092 2021-11-16 21:48:23.000000 lenstronomy-1.9.2/lenstronomy/Util/package_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4274 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/lenstronomy/Util/param_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4486 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Util/prob_density.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4629 2021-12-09 23:23:05.000000 lenstronomy-1.9.2/lenstronomy/Util/sampling_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2689 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Util/simulation_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    21441 2021-12-11 06:59:33.000000 lenstronomy-1.9.2/lenstronomy/Util/util.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.321641 lenstronomy-1.9.2/lenstronomy/Workflow/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/lenstronomy/Workflow/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4553 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/lenstronomy/Workflow/alignment_matching.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    27567 2021-11-17 22:11:20.000000 lenstronomy-1.9.2/lenstronomy/Workflow/fitting_sequence.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4390 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/Workflow/multi_band_manager.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    32233 2021-12-12 19:11:51.000000 lenstronomy-1.9.2/lenstronomy/Workflow/psf_fitting.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    18975 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/lenstronomy/Workflow/update_manager.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      173 2021-12-12 19:13:44.000000 lenstronomy-1.9.2/lenstronomy/__init__.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.195804 lenstronomy-1.9.2/lenstronomy.egg-info/
--rw-r--r--   0 sibirrer   (501) staff       (20)    10628 2021-12-12 19:44:21.000000 lenstronomy-1.9.2/lenstronomy.egg-info/PKG-INFO
--rw-r--r--   0 sibirrer   (501) staff       (20)    42439 2021-12-12 19:44:21.000000 lenstronomy-1.9.2/lenstronomy.egg-info/SOURCES.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)        1 2021-12-12 19:44:21.000000 lenstronomy-1.9.2/lenstronomy.egg-info/dependency_links.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)        1 2021-12-12 19:44:21.000000 lenstronomy-1.9.2/lenstronomy.egg-info/not-zip-safe
--rw-r--r--   0 sibirrer   (501) staff       (20)       39 2021-12-12 19:44:21.000000 lenstronomy-1.9.2/lenstronomy.egg-info/requires.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)       17 2021-12-12 19:44:21.000000 lenstronomy-1.9.2/lenstronomy.egg-info/top_level.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)      384 2021-11-26 19:23:09.000000 lenstronomy-1.9.2/requirements.txt
--rw-r--r--   0 sibirrer   (501) staff       (20)       80 2021-12-12 19:44:22.414049 lenstronomy-1.9.2/setup.cfg
--rw-r--r--   0 sibirrer   (501) staff       (20)     2090 2021-12-12 19:13:44.000000 lenstronomy-1.9.2/setup.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.322244 lenstronomy-1.9.2/test/
--rw-r--r--   0 sibirrer   (501) staff       (20)      108 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/__init__.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.325751 lenstronomy-1.9.2/test/test_Analysis/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_Analysis/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7643 2021-02-15 19:18:04.000000 lenstronomy-1.9.2/test/test_Analysis/test_image_reconstruction.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    21596 2020-12-26 03:28:26.000000 lenstronomy-1.9.2/test/test_Analysis/test_kinematics_api.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8487 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_Analysis/test_lens_profile.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1839 2019-11-17 06:45:53.000000 lenstronomy-1.9.2/test/test_Analysis/test_light2mass.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    16487 2019-11-17 06:45:53.000000 lenstronomy-1.9.2/test/test_Analysis/test_light_profile.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9456 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_Analysis/test_multi_patch_reconstruction.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6071 2020-03-31 14:44:06.000000 lenstronomy-1.9.2/test/test_Analysis/test_td_cosmography.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.326276 lenstronomy-1.9.2/test/test_Conf/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_Conf/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      502 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_Conf/test_config_loader.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.329519 lenstronomy-1.9.2/test/test_Cosmo/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_Cosmo/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1020 2021-03-03 19:21:56.000000 lenstronomy-1.9.2/test/test_Cosmo/test_background.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3110 2021-03-03 19:21:56.000000 lenstronomy-1.9.2/test/test_Cosmo/test_cosmo_interp.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3386 2020-03-10 01:47:46.000000 lenstronomy-1.9.2/test/test_Cosmo/test_cosmo_solver.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3539 2020-03-10 00:45:58.000000 lenstronomy-1.9.2/test/test_Cosmo/test_kde_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1367 2019-11-17 06:45:53.000000 lenstronomy-1.9.2/test/test_Cosmo/test_lcdm.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4159 2021-01-22 18:14:45.000000 lenstronomy-1.9.2/test/test_Cosmo/test_lens_cosmo.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3159 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_Cosmo/test_nfw_param.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.333643 lenstronomy-1.9.2/test/test_Data/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_Data/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5534 2019-06-06 11:33:10.000000 lenstronomy-1.9.2/test/test_Data/test_coord_transforms.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3174 2020-07-14 22:15:02.000000 lenstronomy-1.9.2/test/test_Data/test_image_noise.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4143 2020-09-07 17:12:41.000000 lenstronomy-1.9.2/test/test_Data/test_imaging_data.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9367 2021-11-09 21:30:13.000000 lenstronomy-1.9.2/test/test_Data/test_psf.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.340081 lenstronomy-1.9.2/test/test_GalKin/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_GalKin/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      799 2020-03-31 14:44:06.000000 lenstronomy-1.9.2/test/test_GalKin/test_analytic_kinematics.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5933 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_GalKin/test_anisotropy.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1573 2020-06-08 15:47:55.000000 lenstronomy-1.9.2/test/test_GalKin/test_aperture.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2077 2020-06-08 15:51:50.000000 lenstronomy-1.9.2/test/test_GalKin/test_aperture_types.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      272 2020-02-27 21:30:55.000000 lenstronomy-1.9.2/test/test_GalKin/test_cosmo.py
--rwxr-xr-x   0 sibirrer   (501) staff       (20)    20202 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_GalKin/test_galkin.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1606 2020-09-01 04:13:15.000000 lenstronomy-1.9.2/test/test_GalKin/test_galkin_model.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2217 2020-04-02 00:11:19.000000 lenstronomy-1.9.2/test/test_GalKin/test_galkin_multiobservation.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2857 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_GalKin/test_gom.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11783 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_GalKin/test_light_profile.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12377 2020-03-31 14:44:06.000000 lenstronomy-1.9.2/test/test_GalKin/test_multi_gauss_expansion.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    15350 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_GalKin/test_numeric_kinematics.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      705 2020-02-27 21:30:55.000000 lenstronomy-1.9.2/test/test_GalKin/test_psf.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2263 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_GalKin/test_velocity_util.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.342511 lenstronomy-1.9.2/test/test_ImSim/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_ImSim/__init__.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.343759 lenstronomy-1.9.2/test/test_ImSim/test_MultiBand/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-11-22 19:35:29.000000 lenstronomy-1.9.2/test/test_ImSim/test_MultiBand/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5186 2020-04-05 21:30:54.000000 lenstronomy-1.9.2/test/test_ImSim/test_MultiBand/test_joint_linear.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5396 2020-04-05 21:30:19.000000 lenstronomy-1.9.2/test/test_ImSim/test_MultiBand/test_multi_linear.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.346785 lenstronomy-1.9.2/test/test_ImSim/test_Numerics/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-04-27 21:29:20.000000 lenstronomy-1.9.2/test/test_ImSim/test_Numerics/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3282 2019-11-06 05:25:56.000000 lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_adaptive_numerics.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7429 2020-09-07 16:18:10.000000 lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_convolution.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4457 2020-09-07 16:18:10.000000 lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_grid.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    18125 2021-10-04 16:37:35.000000 lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_numerics.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1042 2019-05-06 23:14:58.000000 lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_partial_image.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3777 2019-11-06 05:25:56.000000 lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_pixel_convolution.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2582 2019-08-14 17:23:40.000000 lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_point_source_rendering.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4416 2020-12-29 06:44:24.000000 lenstronomy-1.9.2/test/test_ImSim/test_de_lens.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1005 2019-11-06 05:25:56.000000 lenstronomy-1.9.2/test/test_ImSim/test_differential_extinction.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11675 2019-07-07 18:00:37.000000 lenstronomy-1.9.2/test/test_ImSim/test_image2soure_mapping.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    15264 2020-12-29 06:08:43.000000 lenstronomy-1.9.2/test/test_ImSim/test_image_model.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    20608 2020-09-07 16:18:10.000000 lenstronomy-1.9.2/test/test_ImSim/test_image_model_pixelbased.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.349887 lenstronomy-1.9.2/test/test_LensModel/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_LensModel/__init__.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.350381 lenstronomy-1.9.2/test/test_LensModel/test_LightConeSim/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-01-02 08:21:31.000000 lenstronomy-1.9.2/test/test_LensModel/test_LightConeSim/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6709 2020-04-30 23:19:55.000000 lenstronomy-1.9.2/test/test_LensModel/test_LightConeSim/test_light_cone.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.350903 lenstronomy-1.9.2/test/test_LensModel/test_MultiPlane/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_MultiPlane/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    19772 2021-09-03 21:13:41.000000 lenstronomy-1.9.2/test/test_LensModel/test_MultiPlane/test_multi_plane.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.352065 lenstronomy-1.9.2/test/test_LensModel/test_Optimizer/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_LensModel/test_Optimizer/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4096 2021-09-03 21:13:41.000000 lenstronomy-1.9.2/test/test_LensModel/test_Optimizer/test_fast_rayshooting.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9621 2020-12-02 02:08:01.000000 lenstronomy-1.9.2/test/test_LensModel/test_Optimizer/test_optimizer.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6687 2020-12-02 02:08:01.000000 lenstronomy-1.9.2/test/test_LensModel/test_Optimizer/test_param_classes.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.375563 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2153 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_arc_perturbations.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      746 2020-02-15 05:36:21.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_base_profile.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    18032 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_chameleon.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3047 2020-02-15 05:36:21.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cnfw.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4582 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cnfw_ellipse.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8463 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_const_mag.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1930 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_constant_shift.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2233 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_convergence.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1976 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_coreBurkert.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2106 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cored_density.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2351 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cored_density_2.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2279 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cored_density_exp.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3339 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cored_profile_mst.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4633 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_const.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11885 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_sis_mst.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8821 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_spp.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2407 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_spt.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8043 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_tan_diff.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3858 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_dipole.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3215 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_elliptical_density_slice.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7055 2021-12-10 00:16:02.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_epl.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4506 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_epl_numba.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3243 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_flexion.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3549 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_flexionfg.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10412 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_gauss_decomposition.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4768 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_gaussian.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5323 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_gaussian_ellipse_kappa.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2672 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_gaussian_ellipse_potential.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5022 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_hernquist.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2251 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_hessian.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10298 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_interpol.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5204 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_multi_gaussian_kappa.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3454 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_multipole.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7093 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nfw.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4262 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nfw_ellipse.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2733 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nfw_mass_concentration.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2440 2021-09-03 21:13:41.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nfw_vir_trunc.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5073 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nie.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10428 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nie_potential.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5403 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_numerical_deflections.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3541 2021-10-28 16:11:02.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_p_jaffe.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3604 2021-10-28 16:14:46.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_p_jaffe_ellipse.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8572 2021-11-12 00:53:27.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_pemd.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2261 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_point_mass.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8669 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_sersic_lens.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2688 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_shapelet_pot_cartesian.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2946 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_shapelet_pot_polar.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5618 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_shear.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2648 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_sie.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2403 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_sis.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2381 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_sis_truncate.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3983 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_spemd.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4619 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_spep.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4897 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_splcore.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5523 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_spp.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5156 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_tnfw.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3845 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_tnfw_ellipse.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2384 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_uldm.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.376989 lenstronomy-1.9.2/test/test_LensModel/test_Solver/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_LensModel/test_Solver/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    11941 2021-09-04 18:31:10.000000 lenstronomy-1.9.2/test/test_LensModel/test_Solver/test_lens_equation_solver.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5073 2020-03-01 18:41:08.000000 lenstronomy-1.9.2/test/test_LensModel/test_Solver/test_solver.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    15823 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_Solver/test_solver2.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    19676 2020-03-01 18:41:08.000000 lenstronomy-1.9.2/test/test_LensModel/test_Solver/test_solver4.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.377609 lenstronomy-1.9.2/test/test_LensModel/test_Util/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-09-04 18:31:10.000000 lenstronomy-1.9.2/test/test_LensModel/test_Util/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      347 2021-09-04 18:31:10.000000 lenstronomy-1.9.2/test/test_LensModel/test_Util/test_epl_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    23250 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_arc_distortions.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5571 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_convergence_integrals.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8892 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_lens_model.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    15927 2021-11-05 02:38:33.000000 lenstronomy-1.9.2/test/test_LensModel/test_lens_model_extensions.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5177 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_LensModel/test_lens_param.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    17862 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_numeric_lens_differentials.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    15544 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_LensModel/test_profile_integrals.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3531 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LensModel/test_single_plane.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.378810 lenstronomy-1.9.2/test/test_LightModel/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_LightModel/__init__.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.382994 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5061 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_chameleon.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      943 2019-11-06 05:25:56.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_ellipsoid.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2844 2020-07-24 22:44:06.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_gaussian.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2949 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_interpolation.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      475 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_moffat.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1407 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_nie.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1149 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_power_law.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      409 2020-03-03 04:43:49.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_profile_base.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6557 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_sersic.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4489 2019-05-29 01:21:04.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_shapelets.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10760 2019-05-29 01:31:36.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_shapelets_polar.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9962 2020-09-07 16:18:10.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_starlets.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      412 2018-12-14 21:53:39.000000 lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_uniform.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2653 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_LightModel/test_light3d.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8425 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_LightModel/test_light_model.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9618 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_LightModel/test_light_param.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.385268 lenstronomy-1.9.2/test/test_Plots/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_Plots/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3339 2020-10-30 21:21:07.000000 lenstronomy-1.9.2/test/test_Plots/test_chain_plot.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3606 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_Plots/test_lens_plot.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    13672 2020-06-19 03:08:07.000000 lenstronomy-1.9.2/test/test_Plots/test_model_plot.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6961 2021-02-16 18:11:11.000000 lenstronomy-1.9.2/test/test_Plots/test_multi_patch_plot.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1031 2021-02-08 02:07:45.000000 lenstronomy-1.9.2/test/test_Plots/test_plot_quasar_images.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4485 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_Plots/test_plot_util.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.386168 lenstronomy-1.9.2/test/test_PointSource/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_PointSource/__init__.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.387320 lenstronomy-1.9.2/test/test_PointSource/test_Types/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/test/test_PointSource/test_Types/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2980 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/test/test_PointSource/test_Types/test_lensed_position.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2344 2021-11-05 02:38:33.000000 lenstronomy-1.9.2/test/test_PointSource/test_Types/test_ps_base.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3015 2021-11-05 02:38:33.000000 lenstronomy-1.9.2/test/test_PointSource/test_Types/test_source_position.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1241 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/test/test_PointSource/test_Types/test_unlensed.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12309 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/test/test_PointSource/test_point_source.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3100 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/test/test_PointSource/test_point_source_cached.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2893 2020-12-29 04:53:22.000000 lenstronomy-1.9.2/test/test_PointSource/test_point_source_param.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.388831 lenstronomy-1.9.2/test/test_Sampling/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_Sampling/__init__.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.391438 lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-04-07 23:54:50.000000 lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4647 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/test_flux_ratio_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      275 2019-05-30 23:33:58.000000 lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/test_image_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5387 2020-07-25 21:00:43.000000 lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/test_position_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3267 2020-04-20 00:19:22.000000 lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/test_prior_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4296 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/test_time_delay_likelihood.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.392027 lenstronomy-1.9.2/test/test_Sampling/test_Pool/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-03-31 20:11:58.000000 lenstronomy-1.9.2/test/test_Sampling/test_Pool/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      863 2020-03-31 20:11:58.000000 lenstronomy-1.9.2/test/test_Sampling/test_Pool/test_pool.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.393792 lenstronomy-1.9.2/test/test_Sampling/test_Samplers/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-06-21 13:54:49.000000 lenstronomy-1.9.2/test/test_Sampling/test_Samplers/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6752 2020-03-01 18:41:08.000000 lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_base_nested_sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7408 2020-03-01 18:41:08.000000 lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_dynesty_sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     7868 2021-11-26 19:23:09.000000 lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_multinest_sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     8699 2020-03-01 18:41:08.000000 lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_polychord_sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4093 2020-03-08 04:10:00.000000 lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_pso.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10058 2021-09-01 20:12:05.000000 lenstronomy-1.9.2/test/test_Sampling/test_likelihood.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    19096 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_Sampling/test_parameters.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     6035 2020-05-13 15:43:38.000000 lenstronomy-1.9.2/test/test_Sampling/test_sampler.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4167 2020-09-07 16:18:10.000000 lenstronomy-1.9.2/test/test_Sampling/test_special_param.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.397109 lenstronomy-1.9.2/test/test_SimulationAPI/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_SimulationAPI/__init__.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.402631 lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-08-12 04:13:35.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3417 2020-08-12 04:13:35.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_DES.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2482 2020-08-12 04:13:35.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_Euclid.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3142 2020-08-12 04:13:35.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_HST.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3791 2020-08-19 03:06:04.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_LSST.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2930 2020-09-09 18:10:31.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_ZTF.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3519 2019-09-06 03:41:28.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_data_api.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3257 2019-08-14 17:23:40.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_model_api.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     9386 2020-07-21 19:44:53.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_observation_api.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1293 2019-02-25 16:57:40.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_observation_constructor.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2837 2020-07-21 18:07:27.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_point_source_variability.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1991 2021-11-09 21:30:13.000000 lenstronomy-1.9.2/test/test_SimulationAPI/test_sim_api.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.410874 lenstronomy-1.9.2/test/test_Util/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_Util/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      932 2019-05-25 23:49:17.000000 lenstronomy-1.9.2/test/test_Util/simulation_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3704 2019-11-17 06:45:53.000000 lenstronomy-1.9.2/test/test_Util/test_analysis_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5297 2019-07-20 02:39:46.000000 lenstronomy-1.9.2/test/test_Util/test_class_creator.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1476 2019-11-06 05:25:56.000000 lenstronomy-1.9.2/test/test_Util/test_correlation.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1720 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_Util/test_data_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4514 2019-11-06 05:25:56.000000 lenstronomy-1.9.2/test/test_Util/test_derivative_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    12988 2020-09-07 16:18:10.000000 lenstronomy-1.9.2/test/test_Util/test_image_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    14389 2021-11-05 05:38:10.000000 lenstronomy-1.9.2/test/test_Util/test_kernel_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3660 2021-02-08 02:07:45.000000 lenstronomy-1.9.2/test/test_Util/test_magnification_finite_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)      942 2019-12-04 01:20:28.000000 lenstronomy-1.9.2/test/test_Util/test_mask_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    10781 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/test/test_Util/test_multi_gauss_expansion.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     1710 2020-10-20 02:22:46.000000 lenstronomy-1.9.2/test/test_Util/test_package_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     5582 2020-06-28 04:53:02.000000 lenstronomy-1.9.2/test/test_Util/test_param_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3246 2020-12-26 00:49:32.000000 lenstronomy-1.9.2/test/test_Util/test_prob_density.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     3878 2021-10-05 16:57:51.000000 lenstronomy-1.9.2/test/test_Util/test_sampling_util.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    13249 2021-11-30 16:27:09.000000 lenstronomy-1.9.2/test/test_Util/test_util.py
-drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-12 19:44:22.413075 lenstronomy-1.9.2/test/test_Workflow/
--rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test/test_Workflow/__init__.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    17213 2021-12-11 07:14:22.000000 lenstronomy-1.9.2/test/test_Workflow/test_fitting_sequence.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     2167 2019-07-20 02:39:46.000000 lenstronomy-1.9.2/test/test_Workflow/test_multiband_update_manager.py
--rw-r--r--   0 sibirrer   (501) staff       (20)    16275 2021-11-11 21:26:21.000000 lenstronomy-1.9.2/test/test_Workflow/test_psf_fitting.py
--rw-r--r--   0 sibirrer   (501) staff       (20)     4747 2021-08-23 22:00:09.000000 lenstronomy-1.9.2/test/test_Workflow/test_update_manager.py
--rw-r--r--   0 sibirrer   (501) staff       (20)       35 2018-09-21 04:29:26.000000 lenstronomy-1.9.2/test_helper.rb
--rw-r--r--   0 sibirrer   (501) staff       (20)      860 2021-08-02 20:31:36.000000 lenstronomy-1.9.2/tox.ini
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.695824 lenstronomy-1.9.3/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.183317 lenstronomy-1.9.3/.github/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.209220 lenstronomy-1.9.3/.github/workflows/
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1947 2021-10-28 20:30:23.000000 lenstronomy-1.9.3/.github/workflows/ci_test.yml
+-rw-r--r--   0 sibirrer   (501) staff       (20)      422 2019-05-28 01:02:43.000000 lenstronomy-1.9.3/.gitignore
+-rw-r--r--   0 sibirrer   (501) staff       (20)      603 2021-12-11 18:31:29.000000 lenstronomy-1.9.3/.readthedocs.yml
+-rw-r--r--   0 sibirrer   (501) staff       (20)      750 2020-02-15 05:36:21.000000 lenstronomy-1.9.3/.travis.yml
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2835 2021-11-26 19:23:09.000000 lenstronomy-1.9.3/AFFILIATEDPACKAGES.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1774 2021-11-30 17:45:54.000000 lenstronomy-1.9.3/AUTHORS.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7477 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/CONTRIBUTING.md
+-rw-r--r--   0 sibirrer   (501) staff       (20)       31 2020-02-15 05:36:21.000000 lenstronomy-1.9.3/Gemfile
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6954 2021-12-22 14:44:11.000000 lenstronomy-1.9.3/HISTORY.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1095 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/LICENSE
+-rw-r--r--   0 sibirrer   (501) staff       (20)      456 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/MAILINGLIST.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      261 2021-09-17 17:39:06.000000 lenstronomy-1.9.3/MANIFEST.in
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1341 2021-09-03 21:13:49.000000 lenstronomy-1.9.3/Makefile
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10628 2021-12-22 14:55:12.695949 lenstronomy-1.9.3/PKG-INFO
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18101 2021-12-09 05:54:15.000000 lenstronomy-1.9.3/PUBLISHED.rst
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.211827 lenstronomy-1.9.3/Paper/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    73738 2021-08-02 20:31:35.000000 lenstronomy-1.9.3/Paper/paper.bib
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16009 2021-08-02 20:31:35.000000 lenstronomy-1.9.3/Paper/paper.md
+-rw-r--r--   0 sibirrer   (501) staff       (20)   288390 2021-08-02 20:31:35.000000 lenstronomy-1.9.3/Paper/paper_fig.png
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9864 2021-10-28 20:30:23.000000 lenstronomy-1.9.3/README.rst
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.244955 lenstronomy-1.9.3/docs/
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1195 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/.coverage
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6777 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/Makefile
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.183808 lenstronomy-1.9.3/docs/_build/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.299440 lenstronomy-1.9.3/docs/_build/doctrees/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15988 2021-12-08 00:08:16.000000 lenstronomy-1.9.3/docs/_build/doctrees/affiliatedpackages.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20390 2021-12-08 00:08:16.000000 lenstronomy-1.9.3/docs/_build/doctrees/authors.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    41548 2021-12-08 00:08:16.000000 lenstronomy-1.9.3/docs/_build/doctrees/contributing.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)  2445960 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 sibirrer   (501) staff       (20)    46805 2021-12-08 00:08:16.000000 lenstronomy-1.9.3/docs/_build/doctrees/history.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    58849 2021-12-08 00:08:16.000000 lenstronomy-1.9.3/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14500 2021-12-08 00:08:16.000000 lenstronomy-1.9.3/docs/_build/doctrees/installation.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   258972 2021-12-08 00:08:18.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Analysis.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   168875 2021-12-08 00:08:19.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Cosmo.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    81278 2021-12-08 00:08:19.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Data.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   386510 2021-12-08 00:08:20.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.GalKin.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   135356 2021-12-08 00:08:20.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.ImSim.MultiBand.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   158153 2021-12-08 00:08:20.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.ImSim.Numerics.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   181209 2021-12-08 00:08:20.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.ImSim.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    22941 2021-12-08 00:08:21.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.LightConeSim.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)  3252051 2021-12-08 00:08:26.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.Profiles.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    89092 2021-12-08 00:08:26.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.QuadOptimizer.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   140969 2021-12-08 00:08:26.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.Solver.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   315367 2021-12-08 00:08:21.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   574910 2021-12-08 00:08:27.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LightModel.Profiles.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    28715 2021-12-08 00:08:27.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LightModel.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   291807 2021-12-08 00:08:29.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Plots.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   105421 2021-12-08 00:08:29.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.PointSource.Types.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   128020 2021-12-08 00:08:29.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.PointSource.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    95058 2021-12-08 00:08:29.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Sampling.Likelihoods.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    44878 2021-12-08 00:08:30.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Sampling.Pool.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    76703 2021-12-08 00:08:30.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Sampling.Samplers.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   165307 2021-12-08 00:08:29.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Sampling.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    46618 2021-12-08 00:08:30.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.SimulationAPI.ObservationConfig.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   127487 2021-12-08 00:08:30.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.SimulationAPI.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   535448 2021-12-08 00:08:31.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Util.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   287625 2021-12-08 00:08:31.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Workflow.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3981 2021-12-08 00:08:16.000000 lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4427 2021-12-08 00:08:31.000000 lenstronomy-1.9.3/docs/_build/doctrees/mailinglist.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2695 2021-12-08 00:08:31.000000 lenstronomy-1.9.3/docs/_build/doctrees/modules.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)   141212 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/doctrees/published.doctree
+-rw-r--r--   0 sibirrer   (501) staff       (20)    24877 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/doctrees/usage.doctree
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.338247 lenstronomy-1.9.3/docs/_build/html/
+-rw-r--r--   0 sibirrer   (501) staff       (20)      230 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/.buildinfo
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.338510 lenstronomy-1.9.3/docs/_build/html/_modules/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    23857 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/index.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.187677 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.341299 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    77355 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/kinematics_api.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    43476 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/lens_profile.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16224 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/light2mass.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    34232 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/light_profile.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    36443 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/td_cosmography.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.343641 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13695 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/background.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    26335 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/cosmo_solver.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10431 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/kde_likelihood.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13287 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/lcdm.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    49556 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/lens_cosmo.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20133 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/nfw_param.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.344964 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Data/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    23200 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Data/coord_transforms.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17660 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Data/imaging_data.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    30799 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Data/psf.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.352002 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    37492 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/analytic_kinematics.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    63137 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/anisotropy.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9384 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/aperture.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    33921 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/aperture_types.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10060 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/cosmo.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    22737 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/galkin.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15490 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/galkin_model.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    46730 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/light_profile.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    61939 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/numeric_kinematics.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5362 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/observation.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12191 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/psf.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    22127 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/velocity_util.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.354605 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.357893 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    30648 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/joint_linear.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15531 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/multi_data_base.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20653 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/multi_linear.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    40022 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/single_band_multi_model.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.362054 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15522 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/adaptive_numerics.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    61422 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/convolution.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    45201 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/grid.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    43260 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/numba_convolution.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    31131 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/numerics.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13719 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/partial_image.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17303 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/point_source_rendering.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17449 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/de_lens.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    47001 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/image2source_mapping.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    91252 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/image_linear_solve.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    66368 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/image_model.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.366697 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.367292 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/LightConeSim/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    21359 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/LightConeSim/light_cone.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.403983 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    30372 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/arc_perturbations.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12515 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/base_profile.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   132820 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/chameleon.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    70183 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cnfw.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    27677 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cnfw_ellipse.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    23800 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/const_mag.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10228 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/constant_shift.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11984 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/convergence.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   105656 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/coreBurkert.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    34905 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    38222 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_2.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    35823 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_exp.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20235 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_mst.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    38251 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_const.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    32133 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_sis_mst.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    28595 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_spp.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    21960 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_spt.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    34474 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_tan_diff.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    22901 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/dipole.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    67632 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/elliptical_density_slice.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    47893 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/epl.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    34219 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/epl_numba.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13428 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/flexion.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18093 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/flexionfg.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    97965 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gauss_decomposition.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    68901 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_ellipse_kappa.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    30528 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_ellipse_potential.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    43585 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_kappa.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14828 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_potential.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    48687 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hernquist.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    30408 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hernquist_ellipse.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13788 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hessian.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    75930 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/interpol.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    46790 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/multi_gaussian_kappa.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20060 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/multipole.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    75261 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    28198 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_ellipse.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20937 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_mass_concentration.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    23516 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_vir_trunc.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    51488 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nie.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    42446 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nie_potential.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15051 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/numerical_deflections.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    51307 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/p_jaffe.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    24027 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/p_jaffe_ellipse.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20705 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/pemd.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    19747 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/point_mass.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20859 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    38612 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_ellipse_kappa.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    23006 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_ellipse_potential.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    37823 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_utils.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    50460 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shapelet_pot_cartesian.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    58374 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shapelet_pot_polar.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    37365 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shear.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    32646 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sie.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    29440 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sis.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    31044 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sis_truncate.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    44696 2021-12-08 00:08:37.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spemd.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    37745 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spep.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    47279 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/splcore.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    40778 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spp.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    75831 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/tnfw.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    47696 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/uldm.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.405476 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    30642 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/multi_plane_fast.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    23390 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/optimizer.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    37799 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/param_manager.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.407188 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Solver/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    84323 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Solver/lens_equation_solver.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14864 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    42583 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver2point.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    52153 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver4point.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    28880 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/convergence_integrals.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    72595 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/lens_model.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   141411 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/lens_model_extensions.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    38113 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/lens_param.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16285 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/profile_integrals.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    57055 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/profile_list_base.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    34593 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/single_plane.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.408075 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.413883 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    45062 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/chameleon.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12482 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/ellipsoid.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    50201 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/gaussian.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17824 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/hernquist.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20932 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/interpolation.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9146 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/moffat.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14377 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/nie.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18287 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/p_jaffe.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14596 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/power_law.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    25617 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/sersic.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    56529 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/shapelets.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    66260 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/shapelets_polar.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6300 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/uniform.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8159 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/light_model.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    40966 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/light_param.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.417945 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    38482 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/chain_plot.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    97701 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/lens_plot.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   152673 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/model_band_plot.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    42350 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/model_plot.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    47376 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/plot_util.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.419814 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.421173 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/Types/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17313 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/Types/base_ps.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    21193 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/Types/lensed_position.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20162 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/Types/source_position.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10598 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/Types/unlensed.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    67316 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/point_source.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18698 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/point_source_cached.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    44695 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/point_source_param.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.423652 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.425494 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16054 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/image_likelihood.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    44713 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/position_likelihood.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    33463 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/prior_likelihood.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15293 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/time_delay_likelihood.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.426077 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Pool/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16736 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Pool/multiprocessing.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12748 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Pool/pool.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.428194 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12805 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/base_nested_sampler.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    23802 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/dynesty_sampler.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    30665 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/multinest_sampler.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    36330 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/polychord_sampler.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    56765 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/likelihood.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   122506 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/parameters.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    37833 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/sampler.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    49306 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/special_param.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.430403 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.431774 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16716 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/DES.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11721 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/Euclid.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14063 2021-12-08 00:08:38.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/HST.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18473 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/LSST.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10371 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/data_api.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    21958 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/model_api.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    44306 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/observation_api.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11062 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/observation_constructor.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20441 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/point_source_variability.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18007 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/sim_api.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.438111 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    30616 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/analysis_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    36056 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/class_creator.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8010 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/constants.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8405 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/correlation.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13715 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/data_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20135 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/derivative_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    56899 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/image_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    92234 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/kernel_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17040 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/mask_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15414 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/multi_gauss_expansion.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17719 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/numba_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    22707 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/param_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    25878 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/prob_density.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    22985 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/sampling_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12910 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/simulation_util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   106662 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/util.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.440250 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Workflow/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    24610 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Workflow/alignment_matching.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    88074 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Workflow/fitting_sequence.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   107519 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Workflow/psf_fitting.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    66434 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Workflow/update_manager.html
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.453057 lenstronomy-1.9.3/docs/_build/html/_sources/
+-rw-r--r--   0 sibirrer   (501) staff       (20)       38 2020-01-25 06:27:26.000000 lenstronomy-1.9.3/docs/_build/html/_sources/affiliatedpackages.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)       27 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/_build/html/_sources/authors.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      116 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/docs/_build/html/_sources/contributing.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)       27 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/_build/html/_sources/history.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      649 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2767 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/_build/html/_sources/installation.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1182 2019-12-04 01:20:28.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Analysis.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1262 2020-03-31 14:44:06.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Cosmo.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      738 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Data.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2400 2020-03-31 14:44:06.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.GalKin.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1135 2019-05-23 03:37:31.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.ImSim.MultiBand.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1725 2019-05-23 03:37:31.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.ImSim.Numerics.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1066 2019-05-23 03:37:31.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.ImSim.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      481 2020-01-16 13:20:36.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LensModel.LightConeSim.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14055 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LensModel.Profiles.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      975 2020-12-17 01:32:55.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LensModel.QuadOptimizer.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1132 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LensModel.Solver.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1901 2021-12-07 21:58:06.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LensModel.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3023 2019-11-06 19:40:51.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LightModel.Profiles.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      694 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LightModel.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1102 2019-11-06 19:40:51.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Plots.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1106 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.PointSource.Types.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      942 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.PointSource.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1236 2019-04-13 18:55:33.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Sampling.Likelihoods.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      622 2020-04-05 22:07:20.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Sampling.Pool.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1179 2019-07-06 16:40:32.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Sampling.Samplers.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1093 2020-04-05 22:10:59.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Sampling.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1223 2020-09-07 18:48:43.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.SimulationAPI.ObservationConfig.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1605 2020-09-07 18:54:25.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.SimulationAPI.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3069 2019-12-04 01:20:28.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Util.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1015 2019-02-01 19:49:19.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Workflow.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      536 2021-12-08 00:08:10.000000 lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)       31 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/_build/html/_sources/mailinglist.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)       70 2021-12-08 00:08:10.000000 lenstronomy-1.9.3/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)       29 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/_build/html/_sources/published.rst.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3966 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/_build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.459202 lenstronomy-1.9.3/docs/_build/html/_static/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14667 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_static/basic.css
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4256 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_static/classic.css
+-rw-r--r--   0 sibirrer   (501) staff       (20)       28 2021-12-07 21:51:58.000000 lenstronomy-1.9.3/docs/_build/html/_static/default.css
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9630 2021-12-07 21:51:58.000000 lenstronomy-1.9.3/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 sibirrer   (501) staff       (20)      355 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 sibirrer   (501) staff       (20)      286 2021-12-07 21:51:58.000000 lenstronomy-1.9.3/docs/_build/html/_static/file.png
+-rw-r--r--   0 sibirrer   (501) staff       (20)    89476 2021-12-07 21:51:58.000000 lenstronomy-1.9.3/docs/_build/html/_static/jquery.js
+-rw-r--r--   0 sibirrer   (501) staff       (20)       90 2021-12-07 21:51:58.000000 lenstronomy-1.9.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sibirrer   (501) staff       (20)       90 2021-12-07 21:51:58.000000 lenstronomy-1.9.3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4846 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16793 2021-12-07 21:51:58.000000 lenstronomy-1.9.3/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4803 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/_static/sidebar.js
+-rw-r--r--   0 sibirrer   (501) staff       (20)    19530 2021-12-07 21:51:58.000000 lenstronomy-1.9.3/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8317 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/affiliatedpackages.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8506 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/authors.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18156 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/contributing.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   427308 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/genindex.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20221 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/history.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    29132 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/index.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9254 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/installation.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    92949 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Analysis.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7568 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Conf.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    69491 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Cosmo.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    33715 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Data.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   140488 2021-12-08 00:08:33.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.GalKin.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    55472 2021-12-08 00:08:33.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.ImSim.MultiBand.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    65023 2021-12-08 00:08:33.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.ImSim.Numerics.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    72214 2021-12-08 00:08:33.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.ImSim.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13077 2021-12-08 00:08:33.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.LightConeSim.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    43961 2021-12-08 00:08:33.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.MultiPlane.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)  1168562 2021-12-08 00:08:34.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.Profiles.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    39749 2021-12-08 00:08:34.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.QuadOptimizer.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    52776 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.Solver.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20841 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.Util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   130191 2021-12-08 00:08:33.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   215054 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.LightModel.Profiles.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18614 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.LightModel.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   110961 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Plots.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    42614 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.PointSource.Types.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    51099 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.PointSource.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    40530 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Sampling.Likelihoods.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    19436 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Sampling.Pool.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    33968 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Sampling.Samplers.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    68897 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Sampling.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    22071 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.SimulationAPI.ObservationConfig.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    53581 2021-12-08 00:08:35.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.SimulationAPI.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   199118 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Util.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   102796 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.Workflow.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    55006 2021-12-08 00:08:32.000000 lenstronomy-1.9.3/docs/_build/html/lenstronomy.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4934 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/mailinglist.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    24013 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/modules.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14405 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/objects.inv
+-rw-r--r--   0 sibirrer   (501) staff       (20)    32516 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/published.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)    62683 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/py-modindex.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3392 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/search.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)   162096 2021-12-08 00:08:39.000000 lenstronomy-1.9.3/docs/_build/html/searchindex.js
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10073 2021-12-08 00:08:36.000000 lenstronomy-1.9.3/docs/_build/html/usage.html
+-rw-r--r--   0 sibirrer   (501) staff       (20)       38 2020-01-25 06:27:26.000000 lenstronomy-1.9.3/docs/affiliatedpackages.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)       27 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/authors.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      515 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/check_sphinx.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8380 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/conf.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      116 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/docs/contributing.rst
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.459504 lenstronomy-1.9.3/docs/figures/
+-rw-r--r--   0 sibirrer   (501) staff       (20)   322886 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/figures/readme_fig.png
+-rw-r--r--   0 sibirrer   (501) staff       (20)       27 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/history.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      649 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/index.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2767 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/installation.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2641 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/junit-docs-ci.xml
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1182 2019-12-04 01:20:28.000000 lenstronomy-1.9.3/docs/lenstronomy.Analysis.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      382 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/docs/lenstronomy.Conf.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1262 2020-03-31 14:44:06.000000 lenstronomy-1.9.3/docs/lenstronomy.Cosmo.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      738 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/lenstronomy.Data.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2400 2020-03-31 14:44:06.000000 lenstronomy-1.9.3/docs/lenstronomy.GalKin.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1135 2019-05-23 03:37:31.000000 lenstronomy-1.9.3/docs/lenstronomy.ImSim.MultiBand.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1725 2019-05-23 03:37:31.000000 lenstronomy-1.9.3/docs/lenstronomy.ImSim.Numerics.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1066 2019-05-23 03:37:31.000000 lenstronomy-1.9.3/docs/lenstronomy.ImSim.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      481 2020-01-16 13:20:36.000000 lenstronomy-1.9.3/docs/lenstronomy.LensModel.LightConeSim.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      715 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/docs/lenstronomy.LensModel.MultiPlane.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14055 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/lenstronomy.LensModel.Profiles.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      975 2020-12-17 01:32:55.000000 lenstronomy-1.9.3/docs/lenstronomy.LensModel.QuadOptimizer.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1132 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/lenstronomy.LensModel.Solver.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      420 2021-12-07 21:52:15.000000 lenstronomy-1.9.3/docs/lenstronomy.LensModel.Util.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1901 2021-12-07 21:58:06.000000 lenstronomy-1.9.3/docs/lenstronomy.LensModel.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3023 2019-11-06 19:40:51.000000 lenstronomy-1.9.3/docs/lenstronomy.LightModel.Profiles.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      694 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/lenstronomy.LightModel.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1102 2019-11-06 19:40:51.000000 lenstronomy-1.9.3/docs/lenstronomy.Plots.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1106 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/lenstronomy.PointSource.Types.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      942 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/lenstronomy.PointSource.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1236 2019-04-13 18:55:33.000000 lenstronomy-1.9.3/docs/lenstronomy.Sampling.Likelihoods.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      622 2020-04-05 22:07:20.000000 lenstronomy-1.9.3/docs/lenstronomy.Sampling.Pool.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1179 2019-07-06 16:40:32.000000 lenstronomy-1.9.3/docs/lenstronomy.Sampling.Samplers.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1093 2020-04-05 22:10:59.000000 lenstronomy-1.9.3/docs/lenstronomy.Sampling.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1223 2020-09-07 18:48:43.000000 lenstronomy-1.9.3/docs/lenstronomy.SimulationAPI.ObservationConfig.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1605 2020-09-07 18:54:25.000000 lenstronomy-1.9.3/docs/lenstronomy.SimulationAPI.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3069 2019-12-04 01:20:28.000000 lenstronomy-1.9.3/docs/lenstronomy.Util.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1015 2019-02-01 19:49:19.000000 lenstronomy-1.9.3/docs/lenstronomy.Workflow.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)      536 2021-12-08 00:08:10.000000 lenstronomy-1.9.3/docs/lenstronomy.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)       31 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/mailinglist.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)       70 2021-12-08 00:08:10.000000 lenstronomy-1.9.3/docs/modules.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)       29 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/docs/published.rst
+-rw-r--r--   0 sibirrer   (501) staff       (20)       66 2021-10-28 15:54:18.000000 lenstronomy-1.9.3/docs/requirements.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3966 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/docs/usage.rst
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.460856 lenstronomy-1.9.3/lenstronomy/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.465519 lenstronomy-1.9.3/lenstronomy/Analysis/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/Analysis/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10048 2021-02-15 19:18:04.000000 lenstronomy-1.9.3/lenstronomy/Analysis/image_reconstruction.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    25577 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/Analysis/kinematics_api.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10401 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/Analysis/lens_profile.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3097 2020-10-30 21:06:27.000000 lenstronomy-1.9.3/lenstronomy/Analysis/light2mass.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8912 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/Analysis/light_profile.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10613 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/Analysis/multi_patch_reconstruction.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11402 2021-10-25 18:10:27.000000 lenstronomy-1.9.3/lenstronomy/Analysis/td_cosmography.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.466757 lenstronomy-1.9.3/lenstronomy/Conf/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/Conf/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      931 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/Conf/conf_default.yaml
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1874 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/Conf/config_loader.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.470671 lenstronomy-1.9.3/lenstronomy/Cosmo/
+-rw-r--r--   0 sibirrer   (501) staff       (20)      115 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1627 2021-11-26 19:23:09.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/_cosmo_interp_astropy_v4.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2382 2021-12-18 17:28:59.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/_cosmo_interp_astropy_v5.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2439 2021-03-03 19:21:56.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/background.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6973 2021-11-26 19:23:09.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/cosmo_interp.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4500 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/cosmo_solver.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1954 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/kde_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2320 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/lcdm.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10671 2021-10-06 21:46:19.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/lens_cosmo.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4001 2020-12-13 20:49:46.000000 lenstronomy-1.9.3/lenstronomy/Cosmo/nfw_param.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.473158 lenstronomy-1.9.3/lenstronomy/Data/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/Data/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5400 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/Data/coord_transforms.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5500 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Data/image_noise.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4968 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Data/imaging_data.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2176 2021-02-15 00:49:48.000000 lenstronomy-1.9.3/lenstronomy/Data/pixel_grid.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8336 2021-11-09 21:30:13.000000 lenstronomy-1.9.3/lenstronomy/Data/psf.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.479156 lenstronomy-1.9.3/lenstronomy/GalKin/
+-rw-r--r--   0 sibirrer   (501) staff       (20)       83 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/GalKin/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8653 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/GalKin/analytic_kinematics.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12596 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/GalKin/anisotropy.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1724 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/GalKin/aperture.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7728 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/GalKin/aperture_types.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1763 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/GalKin/cosmo.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7851 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/GalKin/galkin.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5208 2020-12-22 20:20:25.000000 lenstronomy-1.9.3/lenstronomy/GalKin/galkin_model.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3749 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/GalKin/galkin_multiobservation.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11455 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/GalKin/light_profile.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18059 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/GalKin/numeric_kinematics.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      418 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/GalKin/observation.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2251 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/GalKin/psf.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3284 2021-11-16 21:48:23.000000 lenstronomy-1.9.3/lenstronomy/GalKin/velocity_util.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.487162 lenstronomy-1.9.3/lenstronomy/ImSim/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.491956 lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-11-22 19:22:24.000000 lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8090 2021-02-10 19:13:54.000000 lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/joint_linear.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2931 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/multi_data_base.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6685 2020-10-30 03:00:29.000000 lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/multi_linear.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12547 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/single_band_multi_model.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.497761 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-04-27 21:27:23.000000 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4082 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/adaptive_numerics.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15416 2021-10-01 20:56:04.000000 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/convolution.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11539 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/grid.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11712 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/numba_convolution.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9575 2021-10-01 16:53:19.000000 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/numerics.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7879 2021-07-08 17:17:42.000000 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/numerics_subframe.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2357 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/partial_image.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3494 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/point_source_rendering.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      115 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/ImSim/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2680 2020-12-29 06:38:34.000000 lenstronomy-1.9.3/lenstronomy/ImSim/de_lens.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1984 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/ImSim/differential_extinction.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12536 2021-09-03 21:13:41.000000 lenstronomy-1.9.3/lenstronomy/ImSim/image2source_mapping.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    28616 2021-12-22 11:00:55.000000 lenstronomy-1.9.3/lenstronomy/ImSim/image_linear_solve.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20544 2021-09-03 21:13:41.000000 lenstronomy-1.9.3/lenstronomy/ImSim/image_model.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.501510 lenstronomy-1.9.3/lenstronomy/LensModel/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.502047 lenstronomy-1.9.3/lenstronomy/LensModel/LightConeSim/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-01-02 08:21:31.000000 lenstronomy-1.9.3/lenstronomy/LensModel/LightConeSim/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5152 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/lenstronomy/LensModel/LightConeSim/light_cone.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.505118 lenstronomy-1.9.3/lenstronomy/LensModel/MultiPlane/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/MultiPlane/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16452 2021-09-03 21:13:41.000000 lenstronomy-1.9.3/lenstronomy/LensModel/MultiPlane/multi_plane.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17290 2021-09-03 21:13:41.000000 lenstronomy-1.9.3/lenstronomy/LensModel/MultiPlane/multi_plane_base.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.539511 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/
+-rw-r--r--   0 sibirrer   (501) staff       (20)      116 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6389 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/arc_perturbations.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2849 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/base_profile.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    28357 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/chameleon.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11840 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cnfw.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4132 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cnfw_ellipse.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5025 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/const_mag.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1626 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/constant_shift.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1862 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/convergence.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15347 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/coreBurkert.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7022 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cored_density.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7825 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cored_density_2.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8054 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cored_density_exp.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4728 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cored_density_mst.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10251 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_const.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8133 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_sis_mst.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7173 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_spp.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5361 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_spt.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8534 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_tan_diff.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3495 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/dipole.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12684 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/elliptical_density_slice.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11797 2021-12-11 07:14:22.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/epl.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7201 2021-09-04 18:51:06.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/epl_numba.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1125 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/flexion.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3202 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/flexionfg.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    29497 2021-11-16 21:48:23.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gauss_decomposition.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15621 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gaussian_ellipse_kappa.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4572 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gaussian_ellipse_potential.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6663 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gaussian_kappa.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1747 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gaussian_potential.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10076 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/hernquist.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5473 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/hernquist_ellipse.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2404 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/hessian.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18794 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/interpol.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7461 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/multi_gaussian_kappa.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3296 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/multipole.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15584 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nfw.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6277 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nfw_ellipse.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4176 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nfw_mass_concentration.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3519 2021-09-03 21:13:41.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nfw_vir_trunc.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10496 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nie.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8892 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nie_potential.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3269 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/numerical_deflections.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10420 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/p_jaffe.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3245 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/p_jaffe_ellipse.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5416 2021-11-12 00:53:27.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/pemd.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2766 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/point_mass.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3222 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sersic.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6674 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sersic_ellipse_kappa.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3312 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sersic_ellipse_potential.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7681 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sersic_utils.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9039 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/shapelet_pot_cartesian.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9633 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/shapelet_pot_polar.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7554 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/shear.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6503 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sie.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5375 2021-12-11 07:02:32.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sis.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4621 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sis_truncate.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11340 2021-12-07 22:04:00.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/spemd.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5969 2021-12-09 23:58:51.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/spep.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11232 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/splcore.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6508 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/spp.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14193 2021-09-03 21:13:49.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/tnfw.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6518 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/tnfw_ellipse.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10793 2021-11-16 21:48:23.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/uldm.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.541087 lenstronomy-1.9.3/lenstronomy/LensModel/QuadOptimizer/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-12-02 02:08:01.000000 lenstronomy-1.9.3/lenstronomy/LensModel/QuadOptimizer/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7324 2021-09-03 21:13:41.000000 lenstronomy-1.9.3/lenstronomy/LensModel/QuadOptimizer/multi_plane_fast.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6116 2020-12-02 02:08:01.000000 lenstronomy-1.9.3/lenstronomy/LensModel/QuadOptimizer/optimizer.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9463 2020-12-02 02:08:01.000000 lenstronomy-1.9.3/lenstronomy/LensModel/QuadOptimizer/param_manager.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.543505 lenstronomy-1.9.3/lenstronomy/LensModel/Solver/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Solver/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13847 2021-09-09 01:10:22.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Solver/epl_shear_solver.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    26224 2021-12-07 21:57:45.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Solver/lens_equation_solver.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3161 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Solver/solver.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8429 2021-01-03 05:32:38.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Solver/solver2point.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10148 2021-01-22 18:14:45.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Solver/solver4point.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.544312 lenstronomy-1.9.3/lenstronomy/LensModel/Util/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-09-04 18:31:10.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Util/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5326 2021-09-04 18:31:10.000000 lenstronomy-1.9.3/lenstronomy/LensModel/Util/epl_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/LensModel/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6764 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/LensModel/convergence_integrals.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    21232 2021-11-10 23:25:07.000000 lenstronomy-1.9.3/lenstronomy/LensModel/lens_model.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    37747 2021-11-16 21:48:23.000000 lenstronomy-1.9.3/lenstronomy/LensModel/lens_model_extensions.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9137 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LensModel/lens_param.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2955 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LensModel/profile_integrals.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17872 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/lenstronomy/LensModel/profile_list_base.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7616 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LensModel/single_plane.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.546138 lenstronomy-1.9.3/lenstronomy/LightModel/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.554690 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7820 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/chameleon.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1675 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/ellipsoid.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10957 2021-03-08 04:47:32.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/gaussian.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2577 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/hernquist.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4287 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/interpolation.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1159 2021-12-07 18:51:02.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/moffat.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2722 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/nie.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2506 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/p_jaffe.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1947 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/power_law.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      810 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/profile_base.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5423 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/sersic.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12035 2021-12-07 18:07:04.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/shapelets.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12520 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/shapelets_polar.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7969 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/starlets.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3169 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/starlets_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      551 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/uniform.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/LightModel/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2148 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LightModel/light_model.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11725 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LightModel/light_model_base.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9702 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LightModel/light_param.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8805 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/LightModel/linear_basis.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.558282 lenstronomy-1.9.3/lenstronomy/Plots/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/Plots/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6093 2021-11-11 21:26:21.000000 lenstronomy-1.9.3/lenstronomy/Plots/chain_plot.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    23933 2021-11-30 16:52:36.000000 lenstronomy-1.9.3/lenstronomy/Plots/lens_plot.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    31919 2021-11-30 16:52:36.000000 lenstronomy-1.9.3/lenstronomy/Plots/model_band_plot.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10220 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Plots/model_plot.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9525 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/Plots/multi_patch_plot.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4379 2021-02-08 02:07:45.000000 lenstronomy-1.9.3/lenstronomy/Plots/plot_quasar_images.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9126 2021-11-30 16:52:36.000000 lenstronomy-1.9.3/lenstronomy/Plots/plot_util.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.560146 lenstronomy-1.9.3/lenstronomy/PointSource/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.562545 lenstronomy-1.9.3/lenstronomy/PointSource/Types/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/lenstronomy/PointSource/Types/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4102 2021-11-05 02:38:33.000000 lenstronomy-1.9.3/lenstronomy/PointSource/Types/base_ps.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5731 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/lenstronomy/PointSource/Types/lensed_position.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5441 2021-11-05 02:38:33.000000 lenstronomy-1.9.3/lenstronomy/PointSource/Types/source_position.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1911 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/lenstronomy/PointSource/Types/unlensed.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/PointSource/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    19125 2021-01-06 05:50:40.000000 lenstronomy-1.9.3/lenstronomy/PointSource/point_source.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4506 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/lenstronomy/PointSource/point_source_cached.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9817 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/lenstronomy/PointSource/point_source_param.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.564874 lenstronomy-1.9.3/lenstronomy/Sampling/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.566909 lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-04-06 20:25:36.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4000 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/flux_ratio_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4205 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/image_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12492 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/position_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8448 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/prior_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3421 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/time_delay_likelihood.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.568133 lenstronomy-1.9.3/lenstronomy/Sampling/Pool/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-03-31 20:11:58.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Pool/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4422 2020-09-07 19:40:59.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Pool/multiprocessing.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3675 2021-11-16 21:48:23.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Pool/pool.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.571121 lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-06-21 13:54:49.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2490 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/base_nested_sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6055 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/dynesty_sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7295 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/multinest_sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9155 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/polychord_sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14647 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/pso.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      115 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/Sampling/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17530 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/lenstronomy/Sampling/likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    39986 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/Sampling/parameters.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9596 2021-11-16 21:48:23.000000 lenstronomy-1.9.3/lenstronomy/Sampling/sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11491 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/Sampling/special_param.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.574198 lenstronomy-1.9.3/lenstronomy/SimulationAPI/
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.576560 lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3830 2021-02-11 22:10:04.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/DES.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2574 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/Euclid.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3813 2021-10-25 16:41:19.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/HST.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4250 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/LSST.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3507 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/ZTF.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-08-03 19:28:48.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2157 2021-02-11 23:38:44.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/data_api.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6341 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/model_api.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13045 2021-02-11 23:18:15.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/observation_api.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2064 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/observation_constructor.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4989 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/point_source_variability.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4391 2020-12-29 06:56:09.000000 lenstronomy-1.9.3/lenstronomy/SimulationAPI/sim_api.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.585315 lenstronomy-1.9.3/lenstronomy/Util/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/Util/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5210 2020-10-30 21:06:27.000000 lenstronomy-1.9.3/lenstronomy/Util/analysis_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12123 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/lenstronomy/Util/class_creator.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1123 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Util/constants.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1228 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Util/correlation.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3346 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/Util/data_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2710 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Util/derivative_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11371 2021-12-11 07:00:42.000000 lenstronomy-1.9.3/lenstronomy/Util/image_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    19127 2021-11-05 05:39:13.000000 lenstronomy-1.9.3/lenstronomy/Util/kernel_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5068 2021-02-08 02:07:45.000000 lenstronomy-1.9.3/lenstronomy/Util/magnification_finite_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2733 2020-10-30 21:15:33.000000 lenstronomy-1.9.3/lenstronomy/Util/mask_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2322 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Util/multi_gauss_expansion.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3119 2021-09-04 21:22:27.000000 lenstronomy-1.9.3/lenstronomy/Util/numba_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3092 2021-11-16 21:48:23.000000 lenstronomy-1.9.3/lenstronomy/Util/package_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4274 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/lenstronomy/Util/param_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4486 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Util/prob_density.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4629 2021-12-09 23:23:05.000000 lenstronomy-1.9.3/lenstronomy/Util/sampling_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2689 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Util/simulation_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    21441 2021-12-11 06:59:33.000000 lenstronomy-1.9.3/lenstronomy/Util/util.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.588560 lenstronomy-1.9.3/lenstronomy/Workflow/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/lenstronomy/Workflow/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4553 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/lenstronomy/Workflow/alignment_matching.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    27567 2021-11-17 22:11:20.000000 lenstronomy-1.9.3/lenstronomy/Workflow/fitting_sequence.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4390 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/Workflow/multi_band_manager.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    32233 2021-12-12 19:11:51.000000 lenstronomy-1.9.3/lenstronomy/Workflow/psf_fitting.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18975 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/lenstronomy/Workflow/update_manager.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      173 2021-12-22 14:42:57.000000 lenstronomy-1.9.3/lenstronomy/__init__.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.462562 lenstronomy-1.9.3/lenstronomy.egg-info/
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10628 2021-12-22 14:55:11.000000 lenstronomy-1.9.3/lenstronomy.egg-info/PKG-INFO
+-rw-r--r--   0 sibirrer   (501) staff       (20)    42439 2021-12-22 14:55:12.000000 lenstronomy-1.9.3/lenstronomy.egg-info/SOURCES.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)        1 2021-12-22 14:55:11.000000 lenstronomy-1.9.3/lenstronomy.egg-info/dependency_links.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)        1 2021-12-22 14:55:11.000000 lenstronomy-1.9.3/lenstronomy.egg-info/not-zip-safe
+-rw-r--r--   0 sibirrer   (501) staff       (20)       39 2021-12-22 14:55:11.000000 lenstronomy-1.9.3/lenstronomy.egg-info/requires.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)       17 2021-12-22 14:55:11.000000 lenstronomy-1.9.3/lenstronomy.egg-info/top_level.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)      541 2021-12-20 20:31:40.000000 lenstronomy-1.9.3/requirements.txt
+-rw-r--r--   0 sibirrer   (501) staff       (20)       80 2021-12-22 14:55:12.696357 lenstronomy-1.9.3/setup.cfg
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2090 2021-12-22 14:42:57.000000 lenstronomy-1.9.3/setup.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.589039 lenstronomy-1.9.3/test/
+-rw-r--r--   0 sibirrer   (501) staff       (20)      108 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/__init__.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.594557 lenstronomy-1.9.3/test/test_Analysis/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_Analysis/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7643 2021-02-15 19:18:04.000000 lenstronomy-1.9.3/test/test_Analysis/test_image_reconstruction.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    21596 2020-12-26 03:28:26.000000 lenstronomy-1.9.3/test/test_Analysis/test_kinematics_api.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8487 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_Analysis/test_lens_profile.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1839 2019-11-17 06:45:53.000000 lenstronomy-1.9.3/test/test_Analysis/test_light2mass.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16487 2019-11-17 06:45:53.000000 lenstronomy-1.9.3/test/test_Analysis/test_light_profile.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9456 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_Analysis/test_multi_patch_reconstruction.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6071 2020-03-31 14:44:06.000000 lenstronomy-1.9.3/test/test_Analysis/test_td_cosmography.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.595289 lenstronomy-1.9.3/test/test_Conf/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_Conf/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      502 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_Conf/test_config_loader.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.599149 lenstronomy-1.9.3/test/test_Cosmo/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_Cosmo/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1020 2021-03-03 19:21:56.000000 lenstronomy-1.9.3/test/test_Cosmo/test_background.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3110 2021-03-03 19:21:56.000000 lenstronomy-1.9.3/test/test_Cosmo/test_cosmo_interp.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3386 2020-03-10 01:47:46.000000 lenstronomy-1.9.3/test/test_Cosmo/test_cosmo_solver.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3539 2020-03-10 00:45:58.000000 lenstronomy-1.9.3/test/test_Cosmo/test_kde_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1367 2019-11-17 06:45:53.000000 lenstronomy-1.9.3/test/test_Cosmo/test_lcdm.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4159 2021-01-22 18:14:45.000000 lenstronomy-1.9.3/test/test_Cosmo/test_lens_cosmo.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3159 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_Cosmo/test_nfw_param.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.601337 lenstronomy-1.9.3/test/test_Data/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_Data/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5534 2019-06-06 11:33:10.000000 lenstronomy-1.9.3/test/test_Data/test_coord_transforms.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3174 2020-07-14 22:15:02.000000 lenstronomy-1.9.3/test/test_Data/test_image_noise.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4143 2020-09-07 17:12:41.000000 lenstronomy-1.9.3/test/test_Data/test_imaging_data.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9367 2021-11-09 21:30:13.000000 lenstronomy-1.9.3/test/test_Data/test_psf.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.609848 lenstronomy-1.9.3/test/test_GalKin/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_GalKin/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      799 2020-03-31 14:44:06.000000 lenstronomy-1.9.3/test/test_GalKin/test_analytic_kinematics.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5933 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_GalKin/test_anisotropy.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1573 2020-06-08 15:47:55.000000 lenstronomy-1.9.3/test/test_GalKin/test_aperture.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2077 2020-06-08 15:51:50.000000 lenstronomy-1.9.3/test/test_GalKin/test_aperture_types.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      272 2020-02-27 21:30:55.000000 lenstronomy-1.9.3/test/test_GalKin/test_cosmo.py
+-rwxr-xr-x   0 sibirrer   (501) staff       (20)    20202 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_GalKin/test_galkin.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1606 2020-09-01 04:13:15.000000 lenstronomy-1.9.3/test/test_GalKin/test_galkin_model.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2217 2020-04-02 00:11:19.000000 lenstronomy-1.9.3/test/test_GalKin/test_galkin_multiobservation.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2857 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_GalKin/test_gom.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11783 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_GalKin/test_light_profile.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12377 2020-03-31 14:44:06.000000 lenstronomy-1.9.3/test/test_GalKin/test_multi_gauss_expansion.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15350 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_GalKin/test_numeric_kinematics.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      705 2020-02-27 21:30:55.000000 lenstronomy-1.9.3/test/test_GalKin/test_psf.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2263 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_GalKin/test_velocity_util.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.612481 lenstronomy-1.9.3/test/test_ImSim/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_ImSim/__init__.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.613737 lenstronomy-1.9.3/test/test_ImSim/test_MultiBand/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-11-22 19:35:29.000000 lenstronomy-1.9.3/test/test_ImSim/test_MultiBand/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5186 2020-04-05 21:30:54.000000 lenstronomy-1.9.3/test/test_ImSim/test_MultiBand/test_joint_linear.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5396 2020-04-05 21:30:19.000000 lenstronomy-1.9.3/test/test_ImSim/test_MultiBand/test_multi_linear.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.616853 lenstronomy-1.9.3/test/test_ImSim/test_Numerics/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-04-27 21:29:20.000000 lenstronomy-1.9.3/test/test_ImSim/test_Numerics/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3282 2019-11-06 05:25:56.000000 lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_adaptive_numerics.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7429 2020-09-07 16:18:10.000000 lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_convolution.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4457 2020-09-07 16:18:10.000000 lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_grid.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18125 2021-10-04 16:37:35.000000 lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_numerics.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1042 2019-05-06 23:14:58.000000 lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_partial_image.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3777 2019-11-06 05:25:56.000000 lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_pixel_convolution.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2582 2019-08-14 17:23:40.000000 lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_point_source_rendering.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4416 2020-12-29 06:44:24.000000 lenstronomy-1.9.3/test/test_ImSim/test_de_lens.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1005 2019-11-06 05:25:56.000000 lenstronomy-1.9.3/test/test_ImSim/test_differential_extinction.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11675 2019-07-07 18:00:37.000000 lenstronomy-1.9.3/test/test_ImSim/test_image2soure_mapping.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15264 2020-12-29 06:08:43.000000 lenstronomy-1.9.3/test/test_ImSim/test_image_model.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    20608 2020-09-07 16:18:10.000000 lenstronomy-1.9.3/test/test_ImSim/test_image_model_pixelbased.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.620578 lenstronomy-1.9.3/test/test_LensModel/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_LensModel/__init__.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.621154 lenstronomy-1.9.3/test/test_LensModel/test_LightConeSim/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-01-02 08:21:31.000000 lenstronomy-1.9.3/test/test_LensModel/test_LightConeSim/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6709 2020-04-30 23:19:55.000000 lenstronomy-1.9.3/test/test_LensModel/test_LightConeSim/test_light_cone.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.622008 lenstronomy-1.9.3/test/test_LensModel/test_MultiPlane/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_MultiPlane/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    19772 2021-09-03 21:13:41.000000 lenstronomy-1.9.3/test/test_LensModel/test_MultiPlane/test_multi_plane.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.623627 lenstronomy-1.9.3/test/test_LensModel/test_Optimizer/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_LensModel/test_Optimizer/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4096 2021-09-03 21:13:41.000000 lenstronomy-1.9.3/test/test_LensModel/test_Optimizer/test_fast_rayshooting.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9621 2020-12-02 02:08:01.000000 lenstronomy-1.9.3/test/test_LensModel/test_Optimizer/test_optimizer.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6687 2020-12-02 02:08:01.000000 lenstronomy-1.9.3/test/test_LensModel/test_Optimizer/test_param_classes.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.648904 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2153 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_arc_perturbations.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      746 2020-02-15 05:36:21.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_base_profile.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    18032 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_chameleon.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3047 2020-02-15 05:36:21.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cnfw.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4582 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cnfw_ellipse.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8463 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_const_mag.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1930 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_constant_shift.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2233 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_convergence.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1976 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_coreBurkert.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2106 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cored_density.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2351 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cored_density_2.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2279 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cored_density_exp.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3339 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cored_profile_mst.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4633 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_const.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11885 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_sis_mst.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8821 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_spp.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2407 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_spt.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8043 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_tan_diff.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3858 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_dipole.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3215 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_elliptical_density_slice.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7055 2021-12-10 00:16:02.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_epl.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4506 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_epl_numba.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3243 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_flexion.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3549 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_flexionfg.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10412 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_gauss_decomposition.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4768 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_gaussian.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5323 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_gaussian_ellipse_kappa.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2672 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_gaussian_ellipse_potential.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5022 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_hernquist.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2251 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_hessian.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10298 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_interpol.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5204 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_multi_gaussian_kappa.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3454 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_multipole.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7093 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nfw.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4262 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nfw_ellipse.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2733 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nfw_mass_concentration.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2440 2021-09-03 21:13:41.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nfw_vir_trunc.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5073 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nie.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10428 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nie_potential.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5403 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_numerical_deflections.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3541 2021-10-28 16:11:02.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_p_jaffe.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3604 2021-10-28 16:14:46.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_p_jaffe_ellipse.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8572 2021-11-12 00:53:27.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_pemd.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2261 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_point_mass.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8669 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_sersic_lens.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2688 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_shapelet_pot_cartesian.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2946 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_shapelet_pot_polar.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5618 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_shear.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2648 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_sie.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2403 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_sis.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2381 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_sis_truncate.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3983 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_spemd.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4619 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_spep.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4897 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_splcore.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5523 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_spp.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5156 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_tnfw.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3845 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_tnfw_ellipse.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2384 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_uldm.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.650768 lenstronomy-1.9.3/test/test_LensModel/test_Solver/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_LensModel/test_Solver/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    11941 2021-09-04 18:31:10.000000 lenstronomy-1.9.3/test/test_LensModel/test_Solver/test_lens_equation_solver.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5073 2020-03-01 18:41:08.000000 lenstronomy-1.9.3/test/test_LensModel/test_Solver/test_solver.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15823 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_Solver/test_solver2.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    19676 2020-03-01 18:41:08.000000 lenstronomy-1.9.3/test/test_LensModel/test_Solver/test_solver4.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.651535 lenstronomy-1.9.3/test/test_LensModel/test_Util/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2021-09-04 18:31:10.000000 lenstronomy-1.9.3/test/test_LensModel/test_Util/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      347 2021-09-04 18:31:10.000000 lenstronomy-1.9.3/test/test_LensModel/test_Util/test_epl_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    23250 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_arc_distortions.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5571 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_convergence_integrals.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8892 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_lens_model.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15927 2021-11-05 02:38:33.000000 lenstronomy-1.9.3/test/test_LensModel/test_lens_model_extensions.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5177 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_LensModel/test_lens_param.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17862 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_numeric_lens_differentials.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    15544 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_LensModel/test_profile_integrals.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3531 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LensModel/test_single_plane.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.652755 lenstronomy-1.9.3/test/test_LightModel/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_LightModel/__init__.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.657849 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5061 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_chameleon.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      943 2019-11-06 05:25:56.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_ellipsoid.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2844 2020-07-24 22:44:06.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_gaussian.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2949 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_interpolation.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      475 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_moffat.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1407 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_nie.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1149 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_power_law.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      409 2020-03-03 04:43:49.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_profile_base.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6557 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_sersic.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4489 2019-05-29 01:21:04.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_shapelets.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10760 2019-05-29 01:31:36.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_shapelets_polar.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9962 2020-09-07 16:18:10.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_starlets.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      412 2018-12-14 21:53:39.000000 lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_uniform.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2653 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_LightModel/test_light3d.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8425 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_LightModel/test_light_model.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9618 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_LightModel/test_light_param.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.660983 lenstronomy-1.9.3/test/test_Plots/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_Plots/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3339 2020-10-30 21:21:07.000000 lenstronomy-1.9.3/test/test_Plots/test_chain_plot.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3606 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_Plots/test_lens_plot.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13672 2020-06-19 03:08:07.000000 lenstronomy-1.9.3/test/test_Plots/test_model_plot.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6961 2021-02-16 18:11:11.000000 lenstronomy-1.9.3/test/test_Plots/test_multi_patch_plot.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1031 2021-02-08 02:07:45.000000 lenstronomy-1.9.3/test/test_Plots/test_plot_quasar_images.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4485 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_Plots/test_plot_util.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.662140 lenstronomy-1.9.3/test/test_PointSource/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_PointSource/__init__.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.663829 lenstronomy-1.9.3/test/test_PointSource/test_Types/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/test/test_PointSource/test_Types/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2980 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/test/test_PointSource/test_Types/test_lensed_position.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2344 2021-11-05 02:38:33.000000 lenstronomy-1.9.3/test/test_PointSource/test_Types/test_ps_base.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3015 2021-11-05 02:38:33.000000 lenstronomy-1.9.3/test/test_PointSource/test_Types/test_source_position.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1241 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/test/test_PointSource/test_Types/test_unlensed.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12309 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/test/test_PointSource/test_point_source.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3100 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/test/test_PointSource/test_point_source_cached.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2893 2020-12-29 04:53:22.000000 lenstronomy-1.9.3/test/test_PointSource/test_point_source_param.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.665952 lenstronomy-1.9.3/test/test_Sampling/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_Sampling/__init__.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.668625 lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-04-07 23:54:50.000000 lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4647 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/test_flux_ratio_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      275 2019-05-30 23:33:58.000000 lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/test_image_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5387 2020-07-25 21:00:43.000000 lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/test_position_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3267 2020-04-20 00:19:22.000000 lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/test_prior_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4296 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/test_time_delay_likelihood.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.669289 lenstronomy-1.9.3/test/test_Sampling/test_Pool/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-03-31 20:11:58.000000 lenstronomy-1.9.3/test/test_Sampling/test_Pool/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      863 2020-03-31 20:11:58.000000 lenstronomy-1.9.3/test/test_Sampling/test_Pool/test_pool.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.672420 lenstronomy-1.9.3/test/test_Sampling/test_Samplers/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2019-06-21 13:54:49.000000 lenstronomy-1.9.3/test/test_Sampling/test_Samplers/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6752 2020-03-01 18:41:08.000000 lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_base_nested_sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7408 2020-03-01 18:41:08.000000 lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_dynesty_sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     7868 2021-11-26 19:23:09.000000 lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_multinest_sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     8699 2020-03-01 18:41:08.000000 lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_polychord_sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4093 2020-03-08 04:10:00.000000 lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_pso.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10058 2021-09-01 20:12:05.000000 lenstronomy-1.9.3/test/test_Sampling/test_likelihood.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    19096 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_Sampling/test_parameters.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     6035 2020-05-13 15:43:38.000000 lenstronomy-1.9.3/test/test_Sampling/test_sampler.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4167 2020-09-07 16:18:10.000000 lenstronomy-1.9.3/test/test_Sampling/test_special_param.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.681703 lenstronomy-1.9.3/test/test_SimulationAPI/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_SimulationAPI/__init__.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.684420 lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2020-08-12 04:13:35.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3417 2020-08-12 04:13:35.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_DES.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2482 2020-08-12 04:13:35.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_Euclid.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3142 2020-08-12 04:13:35.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_HST.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3791 2020-08-19 03:06:04.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_LSST.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2930 2020-09-09 18:10:31.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_ZTF.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3519 2019-09-06 03:41:28.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_data_api.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3257 2019-08-14 17:23:40.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_model_api.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     9386 2020-07-21 19:44:53.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_observation_api.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1293 2019-02-25 16:57:40.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_observation_constructor.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2837 2020-07-21 18:07:27.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_point_source_variability.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1991 2021-11-09 21:30:13.000000 lenstronomy-1.9.3/test/test_SimulationAPI/test_sim_api.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.692762 lenstronomy-1.9.3/test/test_Util/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_Util/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      932 2019-05-25 23:49:17.000000 lenstronomy-1.9.3/test/test_Util/simulation_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3704 2019-11-17 06:45:53.000000 lenstronomy-1.9.3/test/test_Util/test_analysis_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5297 2019-07-20 02:39:46.000000 lenstronomy-1.9.3/test/test_Util/test_class_creator.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1476 2019-11-06 05:25:56.000000 lenstronomy-1.9.3/test/test_Util/test_correlation.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1720 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_Util/test_data_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4514 2019-11-06 05:25:56.000000 lenstronomy-1.9.3/test/test_Util/test_derivative_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    12988 2020-09-07 16:18:10.000000 lenstronomy-1.9.3/test/test_Util/test_image_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    14389 2021-11-05 05:38:10.000000 lenstronomy-1.9.3/test/test_Util/test_kernel_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3660 2021-02-08 02:07:45.000000 lenstronomy-1.9.3/test/test_Util/test_magnification_finite_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)      942 2019-12-04 01:20:28.000000 lenstronomy-1.9.3/test/test_Util/test_mask_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    10781 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/test/test_Util/test_multi_gauss_expansion.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     1710 2020-10-20 02:22:46.000000 lenstronomy-1.9.3/test/test_Util/test_package_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     5582 2020-06-28 04:53:02.000000 lenstronomy-1.9.3/test/test_Util/test_param_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3246 2020-12-26 00:49:32.000000 lenstronomy-1.9.3/test/test_Util/test_prob_density.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     3878 2021-10-05 16:57:51.000000 lenstronomy-1.9.3/test/test_Util/test_sampling_util.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    13249 2021-11-30 16:27:09.000000 lenstronomy-1.9.3/test/test_Util/test_util.py
+drwxr-xr-x   0 sibirrer   (501) staff       (20)        0 2021-12-22 14:55:12.695416 lenstronomy-1.9.3/test/test_Workflow/
+-rw-r--r--   0 sibirrer   (501) staff       (20)        0 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test/test_Workflow/__init__.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    17213 2021-12-11 07:14:22.000000 lenstronomy-1.9.3/test/test_Workflow/test_fitting_sequence.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     2167 2019-07-20 02:39:46.000000 lenstronomy-1.9.3/test/test_Workflow/test_multiband_update_manager.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)    16275 2021-11-11 21:26:21.000000 lenstronomy-1.9.3/test/test_Workflow/test_psf_fitting.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)     4747 2021-08-23 22:00:09.000000 lenstronomy-1.9.3/test/test_Workflow/test_update_manager.py
+-rw-r--r--   0 sibirrer   (501) staff       (20)       35 2018-09-21 04:29:26.000000 lenstronomy-1.9.3/test_helper.rb
+-rw-r--r--   0 sibirrer   (501) staff       (20)      860 2021-08-02 20:31:36.000000 lenstronomy-1.9.3/tox.ini
```

### Comparing `lenstronomy-1.9.2/.github/workflows/ci_test.yml` & `lenstronomy-1.9.3/.github/workflows/ci_test.yml`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/.readthedocs.yml` & `lenstronomy-1.9.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/.travis.yml` & `lenstronomy-1.9.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/AFFILIATEDPACKAGES.rst` & `lenstronomy-1.9.3/AFFILIATEDPACKAGES.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/AUTHORS.rst` & `lenstronomy-1.9.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/CONTRIBUTING.md` & `lenstronomy-1.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/HISTORY.rst` & `lenstronomy-1.9.3/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -261,8 +261,12 @@
 
 1.9.2 (2020-12-12)
 ++++++++++++++++++
 * support for astropy v5
 * new PSF iteration procedure implemented
 * updated caustic plotting feature
 * magnification perturbations in point source amplitudes
-* analytic point source solver for SIE+shear
+* analytic point source solver for SIE+shear
+
+1.9.3 (2020-12-22)
+++++++++++++++++++
+* changed syntax to be compatible with python3 version <3.9
```

### Comparing `lenstronomy-1.9.2/LICENSE` & `lenstronomy-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/Makefile` & `lenstronomy-1.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/PKG-INFO` & `lenstronomy-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: lenstronomy
-Version: 1.9.2
+Version: 1.9.3
 Summary: Strong lens modeling package.
 Home-page: https://github.com/sibirrer/lenstronomy
 Author: Simon Birrer
 Author-email: sibirrer@gmail.com
 License: MIT
-Download-URL: https://github.com/sibirrer/lenstronomy/archive/1.9.2.tar.gz
+Download-URL: https://github.com/sibirrer/lenstronomy/archive/1.9.3.tar.gz
 Keywords: lenstronomy
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ====================================================
 lenstronomy - gravitational lensing software package
 ====================================================
```

### Comparing `lenstronomy-1.9.2/PUBLISHED.rst` & `lenstronomy-1.9.3/PUBLISHED.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/Paper/paper.bib` & `lenstronomy-1.9.3/Paper/paper.bib`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/Paper/paper.md` & `lenstronomy-1.9.3/Paper/paper.md`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/Paper/paper_fig.png` & `lenstronomy-1.9.3/Paper/paper_fig.png`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/README.rst` & `lenstronomy-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/.coverage` & `lenstronomy-1.9.3/docs/.coverage`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/Makefile` & `lenstronomy-1.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/affiliatedpackages.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/affiliatedpackages.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/authors.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/authors.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/contributing.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/contributing.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/environment.pickle` & `lenstronomy-1.9.3/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/history.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/history.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/index.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/installation.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Analysis.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Analysis.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Cosmo.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Cosmo.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Data.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Data.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.GalKin.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.GalKin.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.ImSim.MultiBand.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.ImSim.MultiBand.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.ImSim.Numerics.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.ImSim.Numerics.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.ImSim.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.ImSim.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.LightConeSim.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.LightConeSim.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.Profiles.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.Profiles.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.QuadOptimizer.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.QuadOptimizer.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.Solver.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.Solver.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LensModel.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LensModel.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LightModel.Profiles.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LightModel.Profiles.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.LightModel.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.LightModel.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Plots.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Plots.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.PointSource.Types.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.PointSource.Types.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.PointSource.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.PointSource.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Sampling.Likelihoods.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Sampling.Likelihoods.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Sampling.Pool.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Sampling.Pool.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Sampling.Samplers.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Sampling.Samplers.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Sampling.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Sampling.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.SimulationAPI.ObservationConfig.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.SimulationAPI.ObservationConfig.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.SimulationAPI.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.SimulationAPI.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Util.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Util.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.Workflow.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.Workflow.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/lenstronomy.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/lenstronomy.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/mailinglist.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/mailinglist.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/modules.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/published.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/published.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/doctrees/usage.doctree` & `lenstronomy-1.9.3/docs/_build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/index.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/kinematics_api.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/kinematics_api.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/lens_profile.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/lens_profile.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/light2mass.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/light2mass.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/light_profile.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/light_profile.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Analysis/td_cosmography.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Analysis/td_cosmography.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/background.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/background.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/cosmo_solver.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/cosmo_solver.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/kde_likelihood.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/kde_likelihood.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/lcdm.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/lcdm.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/lens_cosmo.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/lens_cosmo.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Cosmo/nfw_param.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Cosmo/nfw_param.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Data/coord_transforms.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Data/coord_transforms.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Data/imaging_data.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Data/imaging_data.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Data/psf.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Data/psf.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/analytic_kinematics.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/analytic_kinematics.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/anisotropy.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/anisotropy.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/aperture.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/aperture.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/aperture_types.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/aperture_types.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/cosmo.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/cosmo.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/galkin.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/galkin.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/galkin_model.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/galkin_model.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/light_profile.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/light_profile.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/numeric_kinematics.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/numeric_kinematics.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/observation.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/observation.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/psf.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/psf.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/GalKin/velocity_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/GalKin/velocity_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/joint_linear.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/joint_linear.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/multi_data_base.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/multi_data_base.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/multi_linear.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/multi_linear.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/single_band_multi_model.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/MultiBand/single_band_multi_model.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/adaptive_numerics.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/adaptive_numerics.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/convolution.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/convolution.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/grid.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/grid.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/numba_convolution.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/numba_convolution.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/numerics.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/numerics.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/partial_image.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/partial_image.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/point_source_rendering.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/Numerics/point_source_rendering.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/de_lens.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/de_lens.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/image2source_mapping.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/image2source_mapping.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/image_linear_solve.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/image_linear_solve.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/ImSim/image_model.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/ImSim/image_model.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/LightConeSim/light_cone.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/LightConeSim/light_cone.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/arc_perturbations.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/arc_perturbations.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/base_profile.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/base_profile.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/chameleon.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/chameleon.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cnfw.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cnfw.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cnfw_ellipse.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cnfw_ellipse.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/const_mag.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/const_mag.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/constant_shift.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/constant_shift.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/convergence.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/convergence.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/coreBurkert.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/coreBurkert.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_2.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_2.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_exp.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_exp.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_mst.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/cored_density_mst.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_const.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_const.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_sis_mst.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_sis_mst.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_spp.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_spp.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_spt.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_spt.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_tan_diff.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/curved_arc_tan_diff.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/dipole.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/dipole.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/elliptical_density_slice.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/elliptical_density_slice.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/epl.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/epl.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/epl_numba.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/epl_numba.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/flexion.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/flexion.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/flexionfg.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/flexionfg.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gauss_decomposition.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gauss_decomposition.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_ellipse_kappa.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_ellipse_kappa.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_ellipse_potential.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_ellipse_potential.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_kappa.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_kappa.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_potential.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/gaussian_potential.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hernquist.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hernquist.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hernquist_ellipse.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hernquist_ellipse.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hessian.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/hessian.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/interpol.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/interpol.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/multi_gaussian_kappa.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/multi_gaussian_kappa.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/multipole.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/multipole.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_ellipse.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_ellipse.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_mass_concentration.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_mass_concentration.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_vir_trunc.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nfw_vir_trunc.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nie.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nie.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nie_potential.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/nie_potential.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/numerical_deflections.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/numerical_deflections.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/p_jaffe.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/p_jaffe.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/p_jaffe_ellipse.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/p_jaffe_ellipse.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/pemd.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/pemd.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/point_mass.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/point_mass.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_ellipse_kappa.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_ellipse_kappa.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_ellipse_potential.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_ellipse_potential.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_utils.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sersic_utils.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shapelet_pot_cartesian.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shapelet_pot_cartesian.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shapelet_pot_polar.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shapelet_pot_polar.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shear.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/shear.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sie.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sie.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sis.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sis.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sis_truncate.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/sis_truncate.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spemd.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spemd.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spep.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spep.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/splcore.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/splcore.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spp.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/spp.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/tnfw.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/tnfw.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/uldm.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Profiles/uldm.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/multi_plane_fast.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/multi_plane_fast.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/optimizer.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/optimizer.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/param_manager.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/QuadOptimizer/param_manager.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Solver/lens_equation_solver.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Solver/lens_equation_solver.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver2point.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver2point.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver4point.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/Solver/solver4point.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/convergence_integrals.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/convergence_integrals.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/lens_model.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/lens_model.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/lens_model_extensions.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/lens_model_extensions.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/lens_param.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/lens_param.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/profile_integrals.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/profile_integrals.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/profile_list_base.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/profile_list_base.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LensModel/single_plane.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LensModel/single_plane.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/chameleon.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/chameleon.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/ellipsoid.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/ellipsoid.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/gaussian.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/gaussian.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/hernquist.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/hernquist.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/interpolation.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/interpolation.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/moffat.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/moffat.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/nie.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/nie.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/p_jaffe.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/p_jaffe.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/power_law.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/power_law.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/sersic.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/sersic.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/shapelets.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/shapelets.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/shapelets_polar.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/shapelets_polar.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/uniform.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/Profiles/uniform.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/light_model.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/light_model.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/LightModel/light_param.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/LightModel/light_param.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/chain_plot.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/chain_plot.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/lens_plot.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/lens_plot.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/model_band_plot.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/model_band_plot.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/model_plot.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/model_plot.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Plots/plot_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Plots/plot_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/Types/base_ps.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/Types/base_ps.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/Types/lensed_position.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/Types/lensed_position.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/Types/source_position.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/Types/source_position.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/Types/unlensed.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/Types/unlensed.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/point_source.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/point_source.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/point_source_cached.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/point_source_cached.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/PointSource/point_source_param.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/PointSource/point_source_param.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/image_likelihood.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/image_likelihood.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/position_likelihood.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/position_likelihood.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/prior_likelihood.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/prior_likelihood.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/time_delay_likelihood.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Likelihoods/time_delay_likelihood.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Pool/multiprocessing.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Pool/multiprocessing.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Pool/pool.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Pool/pool.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/base_nested_sampler.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/base_nested_sampler.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/dynesty_sampler.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/dynesty_sampler.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/multinest_sampler.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/multinest_sampler.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/polychord_sampler.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/Samplers/polychord_sampler.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/likelihood.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/likelihood.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/parameters.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/parameters.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/sampler.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/sampler.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Sampling/special_param.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Sampling/special_param.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/DES.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/DES.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/Euclid.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/Euclid.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/HST.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/HST.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/LSST.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/ObservationConfig/LSST.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/data_api.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/data_api.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/model_api.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/model_api.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/observation_api.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/observation_api.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/observation_constructor.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/observation_constructor.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/point_source_variability.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/point_source_variability.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/SimulationAPI/sim_api.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/SimulationAPI/sim_api.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/analysis_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/analysis_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/class_creator.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/class_creator.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/constants.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/constants.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/correlation.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/correlation.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/data_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/data_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/derivative_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/derivative_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/image_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/image_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/kernel_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/kernel_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/mask_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/mask_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/multi_gauss_expansion.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/multi_gauss_expansion.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/numba_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/numba_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/param_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/param_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/prob_density.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/prob_density.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/sampling_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/sampling_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/simulation_util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/simulation_util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Util/util.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Util/util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Workflow/alignment_matching.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Workflow/alignment_matching.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Workflow/fitting_sequence.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Workflow/fitting_sequence.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Workflow/psf_fitting.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Workflow/psf_fitting.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_modules/lenstronomy/Workflow/update_manager.html` & `lenstronomy-1.9.3/docs/_build/html/_modules/lenstronomy/Workflow/update_manager.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/index.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/installation.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Analysis.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Analysis.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Cosmo.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Cosmo.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Data.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Data.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.GalKin.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.GalKin.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.ImSim.MultiBand.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.ImSim.MultiBand.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.ImSim.Numerics.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.ImSim.Numerics.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.ImSim.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.ImSim.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LensModel.Profiles.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LensModel.Profiles.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LensModel.QuadOptimizer.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LensModel.QuadOptimizer.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LensModel.Solver.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LensModel.Solver.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LensModel.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LensModel.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LightModel.Profiles.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LightModel.Profiles.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.LightModel.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.LightModel.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Plots.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Plots.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.PointSource.Types.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.PointSource.Types.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.PointSource.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.PointSource.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Sampling.Likelihoods.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Sampling.Likelihoods.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Sampling.Pool.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Sampling.Pool.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Sampling.Samplers.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Sampling.Samplers.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Sampling.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Sampling.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.SimulationAPI.ObservationConfig.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.SimulationAPI.ObservationConfig.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.SimulationAPI.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.SimulationAPI.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Util.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Util.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.Workflow.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.Workflow.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/lenstronomy.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/lenstronomy.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_sources/usage.rst.txt` & `lenstronomy-1.9.3/docs/_build/html/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_static/basic.css` & `lenstronomy-1.9.3/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_static/classic.css` & `lenstronomy-1.9.3/docs/_build/html/_static/classic.css`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_static/doctools.js` & `lenstronomy-1.9.3/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_static/jquery.js` & `lenstronomy-1.9.3/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_static/pygments.css` & `lenstronomy-1.9.3/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_static/searchtools.js` & `lenstronomy-1.9.3/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_static/sidebar.js` & `lenstronomy-1.9.3/docs/_build/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/_static/underscore.js` & `lenstronomy-1.9.3/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/affiliatedpackages.html` & `lenstronomy-1.9.3/docs/_build/html/affiliatedpackages.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/authors.html` & `lenstronomy-1.9.3/docs/_build/html/authors.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/contributing.html` & `lenstronomy-1.9.3/docs/_build/html/contributing.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/genindex.html` & `lenstronomy-1.9.3/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/history.html` & `lenstronomy-1.9.3/docs/_build/html/history.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/index.html` & `lenstronomy-1.9.3/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/installation.html` & `lenstronomy-1.9.3/docs/_build/html/installation.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Analysis.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Analysis.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Conf.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Conf.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Cosmo.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Cosmo.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Data.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Data.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.GalKin.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.GalKin.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.ImSim.MultiBand.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.ImSim.MultiBand.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.ImSim.Numerics.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.ImSim.Numerics.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.ImSim.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.ImSim.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.LightConeSim.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.LightConeSim.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.MultiPlane.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.MultiPlane.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.Profiles.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.Profiles.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.QuadOptimizer.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.QuadOptimizer.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.Solver.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.Solver.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.Util.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.Util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.LensModel.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.LensModel.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.LightModel.Profiles.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.LightModel.Profiles.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.LightModel.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.LightModel.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Plots.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Plots.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.PointSource.Types.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.PointSource.Types.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.PointSource.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.PointSource.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Sampling.Likelihoods.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Sampling.Likelihoods.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Sampling.Pool.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Sampling.Pool.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Sampling.Samplers.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Sampling.Samplers.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Sampling.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Sampling.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.SimulationAPI.ObservationConfig.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.SimulationAPI.ObservationConfig.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.SimulationAPI.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.SimulationAPI.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Util.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Util.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.Workflow.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.Workflow.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/lenstronomy.html` & `lenstronomy-1.9.3/docs/_build/html/lenstronomy.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/mailinglist.html` & `lenstronomy-1.9.3/docs/_build/html/mailinglist.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/modules.html` & `lenstronomy-1.9.3/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/objects.inv` & `lenstronomy-1.9.3/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/published.html` & `lenstronomy-1.9.3/docs/_build/html/published.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/py-modindex.html` & `lenstronomy-1.9.3/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/search.html` & `lenstronomy-1.9.3/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/searchindex.js` & `lenstronomy-1.9.3/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/_build/html/usage.html` & `lenstronomy-1.9.3/docs/_build/html/usage.html`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/check_sphinx.py` & `lenstronomy-1.9.3/docs/check_sphinx.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/conf.py` & `lenstronomy-1.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/figures/readme_fig.png` & `lenstronomy-1.9.3/docs/figures/readme_fig.png`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/index.rst` & `lenstronomy-1.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/installation.rst` & `lenstronomy-1.9.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/junit-docs-ci.xml` & `lenstronomy-1.9.3/docs/junit-docs-ci.xml`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Analysis.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Analysis.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Cosmo.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Cosmo.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Data.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Data.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.GalKin.rst` & `lenstronomy-1.9.3/docs/lenstronomy.GalKin.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.ImSim.MultiBand.rst` & `lenstronomy-1.9.3/docs/lenstronomy.ImSim.MultiBand.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.ImSim.Numerics.rst` & `lenstronomy-1.9.3/docs/lenstronomy.ImSim.Numerics.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.ImSim.rst` & `lenstronomy-1.9.3/docs/lenstronomy.ImSim.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.LensModel.MultiPlane.rst` & `lenstronomy-1.9.3/docs/lenstronomy.LensModel.MultiPlane.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.LensModel.Profiles.rst` & `lenstronomy-1.9.3/docs/lenstronomy.LensModel.Profiles.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.LensModel.QuadOptimizer.rst` & `lenstronomy-1.9.3/docs/lenstronomy.LensModel.QuadOptimizer.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.LensModel.Solver.rst` & `lenstronomy-1.9.3/docs/lenstronomy.LensModel.Solver.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.LensModel.rst` & `lenstronomy-1.9.3/docs/lenstronomy.LensModel.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.LightModel.Profiles.rst` & `lenstronomy-1.9.3/docs/lenstronomy.LightModel.Profiles.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.LightModel.rst` & `lenstronomy-1.9.3/docs/lenstronomy.LightModel.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Plots.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Plots.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.PointSource.Types.rst` & `lenstronomy-1.9.3/docs/lenstronomy.PointSource.Types.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.PointSource.rst` & `lenstronomy-1.9.3/docs/lenstronomy.PointSource.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Sampling.Likelihoods.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Sampling.Likelihoods.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Sampling.Pool.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Sampling.Pool.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Sampling.Samplers.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Sampling.Samplers.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Sampling.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Sampling.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.SimulationAPI.ObservationConfig.rst` & `lenstronomy-1.9.3/docs/lenstronomy.SimulationAPI.ObservationConfig.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.SimulationAPI.rst` & `lenstronomy-1.9.3/docs/lenstronomy.SimulationAPI.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Util.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Util.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.Workflow.rst` & `lenstronomy-1.9.3/docs/lenstronomy.Workflow.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/lenstronomy.rst` & `lenstronomy-1.9.3/docs/lenstronomy.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/docs/usage.rst` & `lenstronomy-1.9.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Analysis/image_reconstruction.py` & `lenstronomy-1.9.3/lenstronomy/Analysis/image_reconstruction.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Analysis/kinematics_api.py` & `lenstronomy-1.9.3/lenstronomy/Analysis/kinematics_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Analysis/lens_profile.py` & `lenstronomy-1.9.3/lenstronomy/Analysis/lens_profile.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Analysis/light2mass.py` & `lenstronomy-1.9.3/lenstronomy/Analysis/light2mass.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Analysis/light_profile.py` & `lenstronomy-1.9.3/lenstronomy/Analysis/light_profile.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Analysis/multi_patch_reconstruction.py` & `lenstronomy-1.9.3/lenstronomy/Analysis/multi_patch_reconstruction.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Analysis/td_cosmography.py` & `lenstronomy-1.9.3/lenstronomy/Analysis/td_cosmography.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Conf/conf_default.yaml` & `lenstronomy-1.9.3/lenstronomy/Conf/conf_default.yaml`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Conf/config_loader.py` & `lenstronomy-1.9.3/lenstronomy/Conf/config_loader.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Cosmo/_cosmo_interp_astropy_v4.py` & `lenstronomy-1.9.3/lenstronomy/Cosmo/_cosmo_interp_astropy_v4.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Cosmo/_cosmo_interp_astropy_v5.py` & `lenstronomy-1.9.3/lenstronomy/Cosmo/_cosmo_interp_astropy_v5.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         d : `~astropy.units.Quantity` ['length']
             Comoving distance in Mpc between each input redshift.
         """
 
         return self._cosmo._hubble_distance * self._integral_comoving_distance_z1z2_scalar(z1, z2)
 
     @vectorize_redshift_method(nin=2)
-    def _integral_comoving_distance_z1z2_scalar(self, z1, z2, /):
+    def _integral_comoving_distance_z1z2_scalar(self, z1, z2):
         """
         Comoving line-of-sight distance between objects at redshifts ``z1`` and
         ``z2``. Value in Mpc.
 
         The comoving distance along the line-of-sight between two objects
         remains constant with time for objects in the Hubble flow.
```

### Comparing `lenstronomy-1.9.2/lenstronomy/Cosmo/background.py` & `lenstronomy-1.9.3/lenstronomy/Cosmo/background.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Cosmo/cosmo_interp.py` & `lenstronomy-1.9.3/lenstronomy/Cosmo/cosmo_interp.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Cosmo/cosmo_solver.py` & `lenstronomy-1.9.3/lenstronomy/Cosmo/cosmo_solver.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Cosmo/kde_likelihood.py` & `lenstronomy-1.9.3/lenstronomy/Cosmo/kde_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Cosmo/lcdm.py` & `lenstronomy-1.9.3/lenstronomy/Cosmo/lcdm.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Cosmo/lens_cosmo.py` & `lenstronomy-1.9.3/lenstronomy/Cosmo/lens_cosmo.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Cosmo/nfw_param.py` & `lenstronomy-1.9.3/lenstronomy/Cosmo/nfw_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Data/coord_transforms.py` & `lenstronomy-1.9.3/lenstronomy/Data/coord_transforms.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Data/image_noise.py` & `lenstronomy-1.9.3/lenstronomy/Data/image_noise.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Data/imaging_data.py` & `lenstronomy-1.9.3/lenstronomy/Data/imaging_data.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Data/pixel_grid.py` & `lenstronomy-1.9.3/lenstronomy/Data/pixel_grid.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Data/psf.py` & `lenstronomy-1.9.3/lenstronomy/Data/psf.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/analytic_kinematics.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/analytic_kinematics.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/anisotropy.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/anisotropy.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/aperture.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/aperture.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/aperture_types.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/aperture_types.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/cosmo.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/cosmo.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/galkin.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/galkin.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/galkin_model.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/galkin_model.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/galkin_multiobservation.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/galkin_multiobservation.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/light_profile.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/light_profile.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/numeric_kinematics.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/numeric_kinematics.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/psf.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/psf.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/GalKin/velocity_util.py` & `lenstronomy-1.9.3/lenstronomy/GalKin/velocity_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/joint_linear.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/joint_linear.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/multi_data_base.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/multi_data_base.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/multi_linear.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/multi_linear.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/MultiBand/single_band_multi_model.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/MultiBand/single_band_multi_model.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/adaptive_numerics.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/adaptive_numerics.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/convolution.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/convolution.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/grid.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/grid.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/numba_convolution.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/numba_convolution.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/numerics.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/numerics.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/numerics_subframe.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/numerics_subframe.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/partial_image.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/partial_image.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/Numerics/point_source_rendering.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/Numerics/point_source_rendering.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/de_lens.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/de_lens.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/differential_extinction.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/differential_extinction.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/image2source_mapping.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/image2source_mapping.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/image_linear_solve.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/image_linear_solve.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     
     When light models use pixel-based profile types, such as 'SLIT_STARLETS', 
     the WLS linear inversion is replaced by the regularized inversion performed by an external solver.
     The current pixel-based solver is provided by the SLITronomy plug-in.
     """
     def __init__(self, data_class, psf_class=None, lens_model_class=None, source_model_class=None,
                  lens_light_model_class=None, point_source_class=None, extinction_class=None, 
-                 kwargs_numerics={}, likelihood_mask=None,
+                 kwargs_numerics=None, likelihood_mask=None,
                  psf_error_map_bool_list=None, kwargs_pixelbased=None):
         """
 
         :param data_class: ImageData() instance
         :param psf_class: PSF() instance
         :param lens_model_class: LensModel() instance
         :param source_model_class: LightModel() instance
```

### Comparing `lenstronomy-1.9.2/lenstronomy/ImSim/image_model.py` & `lenstronomy-1.9.3/lenstronomy/ImSim/image_model.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/LightConeSim/light_cone.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/LightConeSim/light_cone.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/MultiPlane/multi_plane.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/MultiPlane/multi_plane.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/MultiPlane/multi_plane_base.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/MultiPlane/multi_plane_base.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/arc_perturbations.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/arc_perturbations.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/base_profile.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/base_profile.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/chameleon.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/chameleon.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cnfw.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cnfw.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cnfw_ellipse.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cnfw_ellipse.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/const_mag.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/const_mag.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/constant_shift.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/constant_shift.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/convergence.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/convergence.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/coreBurkert.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/coreBurkert.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cored_density.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cored_density.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cored_density_2.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cored_density_2.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cored_density_exp.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cored_density_exp.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/cored_density_mst.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/cored_density_mst.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_const.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_const.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_sis_mst.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_sis_mst.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_spp.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_spp.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_spt.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_spt.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/curved_arc_tan_diff.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/curved_arc_tan_diff.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/dipole.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/dipole.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/elliptical_density_slice.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/elliptical_density_slice.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/epl.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/epl.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/epl_numba.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/epl_numba.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/flexion.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/flexion.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/flexionfg.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/flexionfg.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gauss_decomposition.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gauss_decomposition.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gaussian_ellipse_kappa.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gaussian_ellipse_kappa.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gaussian_ellipse_potential.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gaussian_ellipse_potential.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gaussian_kappa.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gaussian_kappa.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/gaussian_potential.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/gaussian_potential.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/hernquist.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/hernquist.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/hernquist_ellipse.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/hernquist_ellipse.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/hessian.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/hessian.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/interpol.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/interpol.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/multi_gaussian_kappa.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/multi_gaussian_kappa.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/multipole.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/multipole.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nfw.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nfw.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nfw_ellipse.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nfw_ellipse.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nfw_mass_concentration.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nfw_mass_concentration.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nfw_vir_trunc.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nfw_vir_trunc.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nie.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nie.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/nie_potential.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/nie_potential.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/numerical_deflections.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/numerical_deflections.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/p_jaffe.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/p_jaffe.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/p_jaffe_ellipse.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/p_jaffe_ellipse.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/pemd.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/pemd.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/point_mass.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/point_mass.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sersic.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sersic.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sersic_ellipse_kappa.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sersic_ellipse_kappa.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sersic_ellipse_potential.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sersic_ellipse_potential.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sersic_utils.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sersic_utils.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/shapelet_pot_cartesian.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/shapelet_pot_cartesian.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/shapelet_pot_polar.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/shapelet_pot_polar.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/shear.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/shear.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sie.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sie.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sis.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sis.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/sis_truncate.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/sis_truncate.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/spemd.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/spemd.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/spep.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/spep.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/splcore.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/splcore.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/spp.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/spp.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/tnfw.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/tnfw.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/tnfw_ellipse.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/tnfw_ellipse.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Profiles/uldm.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Profiles/uldm.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/QuadOptimizer/multi_plane_fast.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/QuadOptimizer/multi_plane_fast.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/QuadOptimizer/optimizer.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/QuadOptimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/QuadOptimizer/param_manager.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/QuadOptimizer/param_manager.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Solver/epl_shear_solver.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Solver/epl_shear_solver.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Solver/lens_equation_solver.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Solver/lens_equation_solver.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Solver/solver.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Solver/solver.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Solver/solver2point.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Solver/solver2point.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Solver/solver4point.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Solver/solver4point.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/Util/epl_util.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/Util/epl_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/convergence_integrals.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/convergence_integrals.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/lens_model.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/lens_model.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/lens_model_extensions.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/lens_model_extensions.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/lens_param.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/lens_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/profile_integrals.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/profile_integrals.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/profile_list_base.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/profile_list_base.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LensModel/single_plane.py` & `lenstronomy-1.9.3/lenstronomy/LensModel/single_plane.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/chameleon.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/chameleon.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/ellipsoid.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/ellipsoid.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/gaussian.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/gaussian.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/hernquist.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/hernquist.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/interpolation.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/interpolation.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/moffat.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/moffat.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/nie.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/nie.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/p_jaffe.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/p_jaffe.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/power_law.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/power_law.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/profile_base.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/profile_base.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/sersic.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/sersic.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/shapelets.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/shapelets.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/shapelets_polar.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/shapelets_polar.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/starlets.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/starlets.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/starlets_util.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/starlets_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/Profiles/uniform.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/Profiles/uniform.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/light_model.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/light_model.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/light_model_base.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/light_model_base.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/light_param.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/light_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/LightModel/linear_basis.py` & `lenstronomy-1.9.3/lenstronomy/LightModel/linear_basis.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Plots/chain_plot.py` & `lenstronomy-1.9.3/lenstronomy/Plots/chain_plot.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Plots/lens_plot.py` & `lenstronomy-1.9.3/lenstronomy/Plots/lens_plot.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Plots/model_band_plot.py` & `lenstronomy-1.9.3/lenstronomy/Plots/model_band_plot.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Plots/model_plot.py` & `lenstronomy-1.9.3/lenstronomy/Plots/model_plot.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Plots/multi_patch_plot.py` & `lenstronomy-1.9.3/lenstronomy/Plots/multi_patch_plot.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Plots/plot_quasar_images.py` & `lenstronomy-1.9.3/lenstronomy/Plots/plot_quasar_images.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Plots/plot_util.py` & `lenstronomy-1.9.3/lenstronomy/Plots/plot_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/PointSource/Types/base_ps.py` & `lenstronomy-1.9.3/lenstronomy/PointSource/Types/base_ps.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/PointSource/Types/lensed_position.py` & `lenstronomy-1.9.3/lenstronomy/PointSource/Types/lensed_position.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/PointSource/Types/source_position.py` & `lenstronomy-1.9.3/lenstronomy/PointSource/Types/source_position.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/PointSource/Types/unlensed.py` & `lenstronomy-1.9.3/lenstronomy/PointSource/Types/unlensed.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/PointSource/point_source.py` & `lenstronomy-1.9.3/lenstronomy/PointSource/point_source.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/PointSource/point_source_cached.py` & `lenstronomy-1.9.3/lenstronomy/PointSource/point_source_cached.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/PointSource/point_source_param.py` & `lenstronomy-1.9.3/lenstronomy/PointSource/point_source_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/flux_ratio_likelihood.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/flux_ratio_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/image_likelihood.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/image_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/position_likelihood.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/position_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/prior_likelihood.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/prior_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Likelihoods/time_delay_likelihood.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Likelihoods/time_delay_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Pool/multiprocessing.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Pool/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Pool/pool.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Pool/pool.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/base_nested_sampler.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/base_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/dynesty_sampler.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/dynesty_sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/multinest_sampler.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/multinest_sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/polychord_sampler.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/polychord_sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/Samplers/pso.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/Samplers/pso.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/likelihood.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/parameters.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/parameters.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/sampler.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Sampling/special_param.py` & `lenstronomy-1.9.3/lenstronomy/Sampling/special_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/DES.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/DES.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/Euclid.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/Euclid.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/HST.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/HST.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/LSST.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/LSST.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/ObservationConfig/ZTF.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/ObservationConfig/ZTF.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/data_api.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/data_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/model_api.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/model_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/observation_api.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/observation_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/observation_constructor.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/observation_constructor.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/point_source_variability.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/point_source_variability.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/SimulationAPI/sim_api.py` & `lenstronomy-1.9.3/lenstronomy/SimulationAPI/sim_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/analysis_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/analysis_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/class_creator.py` & `lenstronomy-1.9.3/lenstronomy/Util/class_creator.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/constants.py` & `lenstronomy-1.9.3/lenstronomy/Util/constants.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/correlation.py` & `lenstronomy-1.9.3/lenstronomy/Util/correlation.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/data_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/data_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/derivative_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/derivative_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/image_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/image_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/kernel_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/kernel_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/magnification_finite_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/magnification_finite_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/mask_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/mask_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/multi_gauss_expansion.py` & `lenstronomy-1.9.3/lenstronomy/Util/multi_gauss_expansion.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/numba_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/numba_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/package_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/package_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/param_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/param_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/prob_density.py` & `lenstronomy-1.9.3/lenstronomy/Util/prob_density.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/sampling_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/sampling_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/simulation_util.py` & `lenstronomy-1.9.3/lenstronomy/Util/simulation_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Util/util.py` & `lenstronomy-1.9.3/lenstronomy/Util/util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Workflow/alignment_matching.py` & `lenstronomy-1.9.3/lenstronomy/Workflow/alignment_matching.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Workflow/fitting_sequence.py` & `lenstronomy-1.9.3/lenstronomy/Workflow/fitting_sequence.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Workflow/multi_band_manager.py` & `lenstronomy-1.9.3/lenstronomy/Workflow/multi_band_manager.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Workflow/psf_fitting.py` & `lenstronomy-1.9.3/lenstronomy/Workflow/psf_fitting.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy/Workflow/update_manager.py` & `lenstronomy-1.9.3/lenstronomy/Workflow/update_manager.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/lenstronomy.egg-info/PKG-INFO` & `lenstronomy-1.9.3/lenstronomy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: lenstronomy
-Version: 1.9.2
+Version: 1.9.3
 Summary: Strong lens modeling package.
 Home-page: https://github.com/sibirrer/lenstronomy
 Author: Simon Birrer
 Author-email: sibirrer@gmail.com
 License: MIT
-Download-URL: https://github.com/sibirrer/lenstronomy/archive/1.9.2.tar.gz
+Download-URL: https://github.com/sibirrer/lenstronomy/archive/1.9.3.tar.gz
 Keywords: lenstronomy
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ====================================================
 lenstronomy - gravitational lensing software package
 ====================================================
```

### Comparing `lenstronomy-1.9.2/lenstronomy.egg-info/SOURCES.txt` & `lenstronomy-1.9.3/lenstronomy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/setup.py` & `lenstronomy-1.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,35 +42,35 @@
 tests_require = ['pytest>=2.3', "mock"]
 
 PACKAGE_PATH = os.path.abspath(os.path.join(__file__, os.pardir))
 
 
 setup(
     name='lenstronomy',
-    version='1.9.2',
+    version='1.9.3',
     description='Strong lens modeling package.',
     long_description=desc,
     author='Simon Birrer',
     author_email='sibirrer@gmail.com',
     url='https://github.com/sibirrer/lenstronomy',
-    download_url='https://github.com/sibirrer/lenstronomy/archive/1.9.2.tar.gz',
+    download_url='https://github.com/sibirrer/lenstronomy/archive/1.9.3.tar.gz',
     packages=find_packages(PACKAGE_PATH, "test"),
     package_dir={'lenstronomy': 'lenstronomy'},
     include_package_data=True,
     # setup_requires=requires,
     install_requires=requires,
     license='MIT',
     zip_safe=False,
     keywords='lenstronomy',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
     tests_require=tests_require,
     cmdclass={'test': PyTest},  # 'build_ext':build_ext,
 )
```

### Comparing `lenstronomy-1.9.2/test/test_Analysis/test_image_reconstruction.py` & `lenstronomy-1.9.3/test/test_Analysis/test_image_reconstruction.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Analysis/test_kinematics_api.py` & `lenstronomy-1.9.3/test/test_Analysis/test_kinematics_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Analysis/test_lens_profile.py` & `lenstronomy-1.9.3/test/test_Analysis/test_lens_profile.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Analysis/test_light2mass.py` & `lenstronomy-1.9.3/test/test_Analysis/test_light2mass.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Analysis/test_light_profile.py` & `lenstronomy-1.9.3/test/test_Analysis/test_light_profile.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Analysis/test_multi_patch_reconstruction.py` & `lenstronomy-1.9.3/test/test_Analysis/test_multi_patch_reconstruction.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Analysis/test_td_cosmography.py` & `lenstronomy-1.9.3/test/test_Analysis/test_td_cosmography.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Cosmo/test_background.py` & `lenstronomy-1.9.3/test/test_Cosmo/test_background.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Cosmo/test_cosmo_interp.py` & `lenstronomy-1.9.3/test/test_Cosmo/test_cosmo_interp.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Cosmo/test_cosmo_solver.py` & `lenstronomy-1.9.3/test/test_Cosmo/test_cosmo_solver.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Cosmo/test_kde_likelihood.py` & `lenstronomy-1.9.3/test/test_Cosmo/test_kde_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Cosmo/test_lcdm.py` & `lenstronomy-1.9.3/test/test_Cosmo/test_lcdm.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Cosmo/test_lens_cosmo.py` & `lenstronomy-1.9.3/test/test_Cosmo/test_lens_cosmo.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Cosmo/test_nfw_param.py` & `lenstronomy-1.9.3/test/test_Cosmo/test_nfw_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Data/test_coord_transforms.py` & `lenstronomy-1.9.3/test/test_Data/test_coord_transforms.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Data/test_image_noise.py` & `lenstronomy-1.9.3/test/test_Data/test_image_noise.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Data/test_imaging_data.py` & `lenstronomy-1.9.3/test/test_Data/test_imaging_data.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Data/test_psf.py` & `lenstronomy-1.9.3/test/test_Data/test_psf.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_analytic_kinematics.py` & `lenstronomy-1.9.3/test/test_GalKin/test_analytic_kinematics.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_anisotropy.py` & `lenstronomy-1.9.3/test/test_GalKin/test_anisotropy.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_aperture.py` & `lenstronomy-1.9.3/test/test_GalKin/test_aperture.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_aperture_types.py` & `lenstronomy-1.9.3/test/test_GalKin/test_aperture_types.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_galkin.py` & `lenstronomy-1.9.3/test/test_GalKin/test_galkin.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_galkin_model.py` & `lenstronomy-1.9.3/test/test_GalKin/test_galkin_model.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_galkin_multiobservation.py` & `lenstronomy-1.9.3/test/test_GalKin/test_galkin_multiobservation.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_gom.py` & `lenstronomy-1.9.3/test/test_GalKin/test_gom.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_light_profile.py` & `lenstronomy-1.9.3/test/test_GalKin/test_light_profile.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_multi_gauss_expansion.py` & `lenstronomy-1.9.3/test/test_GalKin/test_multi_gauss_expansion.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_numeric_kinematics.py` & `lenstronomy-1.9.3/test/test_GalKin/test_numeric_kinematics.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_psf.py` & `lenstronomy-1.9.3/test/test_GalKin/test_psf.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_GalKin/test_velocity_util.py` & `lenstronomy-1.9.3/test/test_GalKin/test_velocity_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_MultiBand/test_joint_linear.py` & `lenstronomy-1.9.3/test/test_ImSim/test_MultiBand/test_joint_linear.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_MultiBand/test_multi_linear.py` & `lenstronomy-1.9.3/test/test_ImSim/test_MultiBand/test_multi_linear.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_adaptive_numerics.py` & `lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_adaptive_numerics.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_convolution.py` & `lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_convolution.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_grid.py` & `lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_grid.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_numerics.py` & `lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_numerics.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_partial_image.py` & `lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_partial_image.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_pixel_convolution.py` & `lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_pixel_convolution.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_Numerics/test_point_source_rendering.py` & `lenstronomy-1.9.3/test/test_ImSim/test_Numerics/test_point_source_rendering.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_de_lens.py` & `lenstronomy-1.9.3/test/test_ImSim/test_de_lens.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_differential_extinction.py` & `lenstronomy-1.9.3/test/test_ImSim/test_differential_extinction.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_image2soure_mapping.py` & `lenstronomy-1.9.3/test/test_ImSim/test_image2soure_mapping.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_image_model.py` & `lenstronomy-1.9.3/test/test_ImSim/test_image_model.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_ImSim/test_image_model_pixelbased.py` & `lenstronomy-1.9.3/test/test_ImSim/test_image_model_pixelbased.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_LightConeSim/test_light_cone.py` & `lenstronomy-1.9.3/test/test_LensModel/test_LightConeSim/test_light_cone.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_MultiPlane/test_multi_plane.py` & `lenstronomy-1.9.3/test/test_LensModel/test_MultiPlane/test_multi_plane.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Optimizer/test_fast_rayshooting.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Optimizer/test_fast_rayshooting.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Optimizer/test_optimizer.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Optimizer/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Optimizer/test_param_classes.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Optimizer/test_param_classes.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_arc_perturbations.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_arc_perturbations.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_base_profile.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_base_profile.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_chameleon.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_chameleon.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cnfw.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cnfw.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cnfw_ellipse.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cnfw_ellipse.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_const_mag.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_const_mag.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_constant_shift.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_constant_shift.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_convergence.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_convergence.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_coreBurkert.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_coreBurkert.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cored_density.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cored_density.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cored_density_2.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cored_density_2.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cored_density_exp.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cored_density_exp.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_cored_profile_mst.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_cored_profile_mst.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_const.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_const.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_sis_mst.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_sis_mst.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_spp.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_spp.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_spt.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_spt.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_curved_arc_tan_diff.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_curved_arc_tan_diff.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_dipole.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_dipole.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_elliptical_density_slice.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_elliptical_density_slice.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_epl.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_epl.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_epl_numba.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_epl_numba.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_flexion.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_flexion.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_flexionfg.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_flexionfg.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_gauss_decomposition.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_gauss_decomposition.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_gaussian.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_gaussian_ellipse_kappa.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_gaussian_ellipse_kappa.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_gaussian_ellipse_potential.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_gaussian_ellipse_potential.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_hernquist.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_hernquist.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_hessian.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_hessian.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_interpol.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_interpol.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_multi_gaussian_kappa.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_multi_gaussian_kappa.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_multipole.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_multipole.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nfw.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nfw.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nfw_ellipse.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nfw_ellipse.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nfw_mass_concentration.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nfw_mass_concentration.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nfw_vir_trunc.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nfw_vir_trunc.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nie.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nie.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_nie_potential.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_nie_potential.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_numerical_deflections.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_numerical_deflections.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_p_jaffe.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_p_jaffe.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_p_jaffe_ellipse.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_p_jaffe_ellipse.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_pemd.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_pemd.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_point_mass.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_sersic_lens.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_sersic_lens.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_shapelet_pot_cartesian.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_shapelet_pot_cartesian.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_shapelet_pot_polar.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_shapelet_pot_polar.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_shear.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_shear.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_sie.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_sie.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_sis.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_sis.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_sis_truncate.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_sis_truncate.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_spemd.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_spemd.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_spep.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_spep.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_splcore.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_splcore.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_spp.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_spp.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_tnfw.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_tnfw.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_tnfw_ellipse.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_tnfw_ellipse.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Profiles/test_uldm.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Profiles/test_uldm.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Solver/test_lens_equation_solver.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Solver/test_lens_equation_solver.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Solver/test_solver.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Solver/test_solver.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Solver/test_solver2.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Solver/test_solver2.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_Solver/test_solver4.py` & `lenstronomy-1.9.3/test/test_LensModel/test_Solver/test_solver4.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_arc_distortions.py` & `lenstronomy-1.9.3/test/test_LensModel/test_arc_distortions.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_convergence_integrals.py` & `lenstronomy-1.9.3/test/test_LensModel/test_convergence_integrals.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_lens_model.py` & `lenstronomy-1.9.3/test/test_LensModel/test_lens_model.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_lens_model_extensions.py` & `lenstronomy-1.9.3/test/test_LensModel/test_lens_model_extensions.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_lens_param.py` & `lenstronomy-1.9.3/test/test_LensModel/test_lens_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_numeric_lens_differentials.py` & `lenstronomy-1.9.3/test/test_LensModel/test_numeric_lens_differentials.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_profile_integrals.py` & `lenstronomy-1.9.3/test/test_LensModel/test_profile_integrals.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LensModel/test_single_plane.py` & `lenstronomy-1.9.3/test/test_LensModel/test_single_plane.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_chameleon.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_chameleon.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_ellipsoid.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_gaussian.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_interpolation.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_nie.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_nie.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_power_law.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_power_law.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_sersic.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_sersic.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_shapelets.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_shapelets.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_shapelets_polar.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_shapelets_polar.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_Profiles/test_starlets.py` & `lenstronomy-1.9.3/test/test_LightModel/test_Profiles/test_starlets.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_light3d.py` & `lenstronomy-1.9.3/test/test_LightModel/test_light3d.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_light_model.py` & `lenstronomy-1.9.3/test/test_LightModel/test_light_model.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_LightModel/test_light_param.py` & `lenstronomy-1.9.3/test/test_LightModel/test_light_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Plots/test_chain_plot.py` & `lenstronomy-1.9.3/test/test_Plots/test_chain_plot.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Plots/test_lens_plot.py` & `lenstronomy-1.9.3/test/test_Plots/test_lens_plot.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Plots/test_model_plot.py` & `lenstronomy-1.9.3/test/test_Plots/test_model_plot.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Plots/test_multi_patch_plot.py` & `lenstronomy-1.9.3/test/test_Plots/test_multi_patch_plot.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Plots/test_plot_quasar_images.py` & `lenstronomy-1.9.3/test/test_Plots/test_plot_quasar_images.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Plots/test_plot_util.py` & `lenstronomy-1.9.3/test/test_Plots/test_plot_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_PointSource/test_Types/test_lensed_position.py` & `lenstronomy-1.9.3/test/test_PointSource/test_Types/test_lensed_position.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_PointSource/test_Types/test_ps_base.py` & `lenstronomy-1.9.3/test/test_PointSource/test_Types/test_ps_base.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_PointSource/test_Types/test_source_position.py` & `lenstronomy-1.9.3/test/test_PointSource/test_Types/test_source_position.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_PointSource/test_Types/test_unlensed.py` & `lenstronomy-1.9.3/test/test_PointSource/test_Types/test_unlensed.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_PointSource/test_point_source.py` & `lenstronomy-1.9.3/test/test_PointSource/test_point_source.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_PointSource/test_point_source_cached.py` & `lenstronomy-1.9.3/test/test_PointSource/test_point_source_cached.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_PointSource/test_point_source_param.py` & `lenstronomy-1.9.3/test/test_PointSource/test_point_source_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/test_flux_ratio_likelihood.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/test_flux_ratio_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/test_position_likelihood.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/test_position_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/test_prior_likelihood.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/test_prior_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Likelihoods/test_time_delay_likelihood.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Likelihoods/test_time_delay_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Pool/test_pool.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Pool/test_pool.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_base_nested_sampler.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_base_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_dynesty_sampler.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_dynesty_sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_multinest_sampler.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_multinest_sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_polychord_sampler.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_polychord_sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_Samplers/test_pso.py` & `lenstronomy-1.9.3/test/test_Sampling/test_Samplers/test_pso.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_likelihood.py` & `lenstronomy-1.9.3/test/test_Sampling/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_parameters.py` & `lenstronomy-1.9.3/test/test_Sampling/test_parameters.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_sampler.py` & `lenstronomy-1.9.3/test/test_Sampling/test_sampler.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Sampling/test_special_param.py` & `lenstronomy-1.9.3/test/test_Sampling/test_special_param.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_DES.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_DES.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_Euclid.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_Euclid.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_HST.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_HST.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_LSST.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_LSST.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_ObservationConfig/test_ZTF.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_ObservationConfig/test_ZTF.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_data_api.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_data_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_model_api.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_model_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_observation_api.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_observation_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_observation_constructor.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_observation_constructor.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_point_source_variability.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_point_source_variability.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_SimulationAPI/test_sim_api.py` & `lenstronomy-1.9.3/test/test_SimulationAPI/test_sim_api.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/simulation_util.py` & `lenstronomy-1.9.3/test/test_Util/simulation_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_analysis_util.py` & `lenstronomy-1.9.3/test/test_Util/test_analysis_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_class_creator.py` & `lenstronomy-1.9.3/test/test_Util/test_class_creator.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_correlation.py` & `lenstronomy-1.9.3/test/test_Util/test_correlation.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_data_util.py` & `lenstronomy-1.9.3/test/test_Util/test_data_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_derivative_util.py` & `lenstronomy-1.9.3/test/test_Util/test_derivative_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_image_util.py` & `lenstronomy-1.9.3/test/test_Util/test_image_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_kernel_util.py` & `lenstronomy-1.9.3/test/test_Util/test_kernel_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_magnification_finite_util.py` & `lenstronomy-1.9.3/test/test_Util/test_magnification_finite_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_mask_util.py` & `lenstronomy-1.9.3/test/test_Util/test_mask_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_multi_gauss_expansion.py` & `lenstronomy-1.9.3/test/test_Util/test_multi_gauss_expansion.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_package_util.py` & `lenstronomy-1.9.3/test/test_Util/test_package_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_param_util.py` & `lenstronomy-1.9.3/test/test_Util/test_param_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_prob_density.py` & `lenstronomy-1.9.3/test/test_Util/test_prob_density.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_sampling_util.py` & `lenstronomy-1.9.3/test/test_Util/test_sampling_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Util/test_util.py` & `lenstronomy-1.9.3/test/test_Util/test_util.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Workflow/test_fitting_sequence.py` & `lenstronomy-1.9.3/test/test_Workflow/test_fitting_sequence.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Workflow/test_multiband_update_manager.py` & `lenstronomy-1.9.3/test/test_Workflow/test_multiband_update_manager.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Workflow/test_psf_fitting.py` & `lenstronomy-1.9.3/test/test_Workflow/test_psf_fitting.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/test/test_Workflow/test_update_manager.py` & `lenstronomy-1.9.3/test/test_Workflow/test_update_manager.py`

 * *Files identical despite different names*

### Comparing `lenstronomy-1.9.2/tox.ini` & `lenstronomy-1.9.3/tox.ini`

 * *Files identical despite different names*

