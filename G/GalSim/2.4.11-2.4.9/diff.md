# Comparing `tmp/GalSim-2.4.11.tar.gz` & `tmp/GalSim-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GalSim-2.4.11.tar", last modified: Sat Aug  5 06:38:41 2023, max compression
+gzip compressed data, was "GalSim-2.4.9.tar", last modified: Wed May 17 14:44:59 2023, max compression
```

## Comparing `GalSim-2.4.11.tar` & `GalSim-2.4.9.tar`

### file list

```diff
@@ -1,754 +1,754 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.287955 GalSim-2.4.11/
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-08-05 06:37:37.000000 GalSim-2.4.11/CHANGELOG.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.147956 GalSim-2.4.11/GalSim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-08-05 06:38:40.000000 GalSim-2.4.11/GalSim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-08-05 06:38:41.000000 GalSim-2.4.11/GalSim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 06:38:40.000000 GalSim-2.4.11/GalSim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-05 06:38:40.000000 GalSim-2.4.11/GalSim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 06:38:40.000000 GalSim-2.4.11/GalSim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-05 06:38:40.000000 GalSim-2.4.11/GalSim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 06:38:40.000000 GalSim-2.4.11/GalSim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-05 06:37:37.000000 GalSim-2.4.11/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-05 06:37:37.000000 GalSim-2.4.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-05 06:37:37.000000 GalSim-2.4.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-08-05 06:38:41.287955 GalSim-2.4.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-08-05 06:37:37.000000 GalSim-2.4.11/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.155956 GalSim-2.4.11/galsim/
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/_pyfits.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/airy.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    33326 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/bandpass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/bessel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/cdmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/celestial.py
--rw-r--r--   0 runner    (1001) docker     (123)   174490 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/chromatic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.159956 GalSim-2.4.11/galsim/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/bandpass.py
--rw-r--r--   0 runner    (1001) docker     (123)    23288 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/extra_badpix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/extra_psf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/extra_truth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/extra_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/gsobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    25719 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/image_scattered.py
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/image_tiled.py
--rw-r--r--   0 runner    (1001) docker     (123)    30729 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/input_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/input_fitsheader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/input_nfw.py
--rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/input_powerspectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/input_real.py
--rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    24359 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/output_datacube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/output_multifits.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/photon_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/sed.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    55175 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/stamp_ring.py
--rw-r--r--   0 runner    (1001) docker     (123)    45344 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    34823 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/value_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/value_random.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/config/wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40999 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    88490 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/correlatednoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/dcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/deltafunction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.159956 GalSim-2.4.11/galsim/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/deprecated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/deprecated/correlatednoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/deprecated/integ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/deprecated/randwalk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.163956 GalSim-2.4.11/galsim/des/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/des/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/des/des_meds.py
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/des/des_psfex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/des/des_shapelet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/download_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)    65951 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/fits.py
--rw-r--r--   0 runner    (1001) docker     (123)    83990 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/fitswcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/fouriersqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    50214 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/galaxy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)   132375 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/gsobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/gsparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    37460 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/hsm.py
--rw-r--r--   0 runner    (1001) docker     (123)    83673 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    21113 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/inclined.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.163956 GalSim-2.4.11/galsim/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/GalSim.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.163956 GalSim-2.4.11/galsim/include/fftw3/
--rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/fftw3/fftw3.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.171956 GalSim-2.4.11/galsim/include/galsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/BinomFact.h
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Bounds.h
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/CDModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/CorrelatedNoise.h
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/GSParams.h
--rw-r--r--   0 runner    (1001) docker     (123)    30925 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Image.h
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/ImageArith.h
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Interpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/LRUCache.h
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Laguerre.h
--rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/OneDimensionalDeviate.h
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/PhotonArray.h
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Polygon.h
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/ProbabilityTree.h
--rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/RealGalaxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBAdd.h
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBAddImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBAiry.h
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBAiryImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBBox.h
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBBoxImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBConvolve.h
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBConvolveImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBDeconvolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBDeconvolveImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBDeltaFunction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBDeltaFunctionImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBExponential.h
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBExponentialImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBFourierSqrt.h
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBFourierSqrtImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBGaussian.h
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBGaussianImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBInclinedExponential.h
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBInclinedExponentialImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBInclinedSersic.h
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBInclinedSersicImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBInterpolatedImage.h
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBInterpolatedImageImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBKolmogorov.h
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBKolmogorovImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBMoffat.h
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBMoffatImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBProfile.h
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBProfileImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBSecondKick.h
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBSecondKickImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBSersic.h
--rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBSersicImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBShapelet.h
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBShapeletImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBSpergel.h
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBSpergelImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBTransform.h
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBTransformImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBVonKarman.h
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/SBVonKarmanImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Silicon.h
--rw-r--r--   0 runner    (1001) docker     (123)    16801 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Std.h
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Stopwatch.h
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/Table.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-05 06:38:40.000000 GalSim-2.4.11/galsim/include/galsim/Version.h
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/WCS.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.171956 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/LICENSE_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/README
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/assert.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.171956 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/config/
--rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/config/suffix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/current_function.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.171956 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/binomial_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.171956 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/detail/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/detail/seed.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/exponential_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/gamma_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/mersenne_twister.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/normal_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/poisson_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/uniform_01.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/weibull_distribution.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.175956 GalSim-2.4.11/galsim/include/galsim/fmath/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/README
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/avx2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/bench.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/bench.sln
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/bench.vcproj
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/ck.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/fastexp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23954 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/fmath.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.143957 GalSim-2.4.11/galsim/include/galsim/fmath/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.175956 GalSim-2.4.11/galsim/include/galsim/fmath/include/cybozu/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/include/cybozu/benchmark.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/include/cybozu/inttype.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/fmath/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.175956 GalSim-2.4.11/galsim/include/galsim/hsm/
--rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/hsm/PSFCorr.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.175956 GalSim-2.4.11/galsim/include/galsim/integ/
--rw-r--r--   0 runner    (1001) docker     (123)    45294 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/integ/Int.h
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/integ/IntGKPData1.h
--rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/integ/IntGKPData10.h
--rw-r--r--   0 runner    (1001) docker     (123)    32193 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/integ/MoreFunctional.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.175956 GalSim-2.4.11/galsim/include/galsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/math/Angle.h
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/math/Bessel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/math/Gamma.h
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/math/Hankel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/math/Horner.h
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/math/Nan.h
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/math/Sinc.h
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/include/galsim/mmgr.h
--rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/integ.py
--rw-r--r--   0 runner    (1001) docker     (123)    23701 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/interpolant.py
--rw-r--r--   0 runner    (1001) docker     (123)    58114 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/interpolatedimage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12980 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/knots.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/kolmogorov.py
--rw-r--r--   0 runner    (1001) docker     (123)    77535 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/lensing_ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/moffat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/nfw_halo.py
--rw-r--r--   0 runner    (1001) docker     (123)    26020 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)   107582 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/phase_psf.py
--rw-r--r--   0 runner    (1001) docker     (123)    61323 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/phase_screens.py
--rw-r--r--   0 runner    (1001) docker     (123)    53397 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/photon_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/position.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/pse.py
--rw-r--r--   0 runner    (1001) docker     (123)    39867 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    70867 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/real.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.175956 GalSim-2.4.11/galsim/roman/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/roman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/roman/roman_backgrounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/roman/roman_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/roman/roman_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/roman/roman_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/roman/roman_psfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36583 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/roman/roman_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/second_kick.py
--rw-r--r--   0 runner    (1001) docker     (123)    52182 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/sed.py
--rw-r--r--   0 runner    (1001) docker     (123)    24811 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/sersic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/shapelet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.175956 GalSim-2.4.11/galsim/share/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.179956 GalSim-2.4.11/galsim/share/SEDs/
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/CWW_E_ext.sed
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/CWW_E_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/CWW_Im_ext.sed
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/CWW_Im_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/CWW_Sbc_ext.sed
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/CWW_Sbc_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/CWW_Scd_ext.sed
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/CWW_Scd_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   102422 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/SEDs/vega.txt
--rw-r--r--   0 runner    (1001) docker     (123)    57600 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/acs_I_unrot_sci_20_cf.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.179956 GalSim-2.4.11/galsim/share/bandpasses/
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F435W.dat
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F606W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F775W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F814W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F850LP.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/LSST_g.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/LSST_i.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/LSST_r.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/LSST_u.dat
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/LSST_y.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/LSST_z.dat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/WFC3_ir_F105W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/WFC3_ir_F125W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/WFC3_ir_F160W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/WFC3_uvis_F275W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/bandpasses/WFC3_uvis_F336W.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.191956 GalSim-2.4.11/galsim/share/roman/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_01.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_02.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_03.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_04.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_05.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_06.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_07.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_08.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_12.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_13.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_14.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_15.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_16.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_17.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_18.txt
--rw-r--r--   0 runner    (1001) docker     (123)   204929 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)   207326 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43524 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA10_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA10_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43726 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA11_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43282 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA11_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43689 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA12_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43476 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA12_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43504 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA13_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43409 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA13_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43821 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA14_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43330 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA14_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA15_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43401 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA15_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43623 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA16_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43477 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA16_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA17_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43451 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA17_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43708 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA18_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43389 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA18_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43499 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA1_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43287 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA1_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA2_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43288 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA2_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43600 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA3_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43454 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA3_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43556 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA4_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43428 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA4_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43621 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA5_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43300 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA5_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43583 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA6_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43388 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA6_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43508 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA7_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43488 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA7_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43689 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA8_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43457 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA8_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43619 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA9_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43394 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/SCA9_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/afta_throughput.txt
--rw-r--r--   0 runner    (1001) docker     (123)   251160 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/roman_sky_backgrounds.txt
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/sca_positions_7_6_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/roman/sip_7_6_8.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.195956 GalSim-2.4.11/galsim/share/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/abs_length.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_e2v_32.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_e2v_32.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_e2v_50_32.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_e2v_50_32.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_e2v_50_8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_e2v_50_8.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_e2v_8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_e2v_8.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_itl_32.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_itl_32.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_itl_50_32.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_itl_50_32.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_itl_50_8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_itl_50_8.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_itl_8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/sensors/lsst_itl_8.dat
--rw-r--r--   0 runner    (1001) docker     (123)   122780 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/share/wfc_F814W.dat.gz
--rw-r--r--   0 runner    (1001) docker     (123)    17146 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/shear.py
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/spergel.py
--rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/sum.py
--rw-r--r--   0 runner    (1001) docker     (123)    51390 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    23848 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    78545 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/vonkarman.py
--rw-r--r--   0 runner    (1001) docker     (123)   121609 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/wfirst.py
--rw-r--r--   0 runner    (1001) docker     (123)    32968 2023-08-05 06:37:38.000000 GalSim-2.4.11/galsim/zernike.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.195956 GalSim-2.4.11/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/GalSim.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.195956 GalSim-2.4.11/include/fftw3/
--rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/fftw3/fftw3.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.211956 GalSim-2.4.11/include/galsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/BinomFact.h
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Bounds.h
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/CDModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/CorrelatedNoise.h
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/GSParams.h
--rw-r--r--   0 runner    (1001) docker     (123)    30925 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Image.h
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/ImageArith.h
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Interpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/LRUCache.h
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Laguerre.h
--rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/OneDimensionalDeviate.h
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/PhotonArray.h
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Polygon.h
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/ProbabilityTree.h
--rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/RealGalaxy.h
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBAdd.h
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBAddImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBAiry.h
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBAiryImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBBox.h
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBBoxImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBConvolve.h
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBConvolveImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBDeconvolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBDeconvolveImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBDeltaFunction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBDeltaFunctionImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBExponential.h
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBExponentialImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBFourierSqrt.h
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBFourierSqrtImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBGaussian.h
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBGaussianImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBInclinedExponential.h
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBInclinedExponentialImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBInclinedSersic.h
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBInclinedSersicImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBInterpolatedImage.h
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBInterpolatedImageImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBKolmogorov.h
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBKolmogorovImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBMoffat.h
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBMoffatImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBProfile.h
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBProfileImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBSecondKick.h
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBSecondKickImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBSersic.h
--rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBSersicImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBShapelet.h
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBShapeletImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBSpergel.h
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBSpergelImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBTransform.h
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBTransformImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBVonKarman.h
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/SBVonKarmanImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Silicon.h
--rw-r--r--   0 runner    (1001) docker     (123)    16801 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Std.h
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Stopwatch.h
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/Table.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-05 06:38:40.000000 GalSim-2.4.11/include/galsim/Version.h
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/WCS.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.211956 GalSim-2.4.11/include/galsim/boost1_48_0/
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/assert.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.211956 GalSim-2.4.11/include/galsim/boost1_48_0/config/
--rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/config/suffix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/current_function.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.211956 GalSim-2.4.11/include/galsim/boost1_48_0/random/
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/binomial_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.215956 GalSim-2.4.11/include/galsim/boost1_48_0/random/detail/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/detail/seed.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/exponential_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/gamma_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/mersenne_twister.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/normal_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/poisson_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/uniform_01.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/boost1_48_0/random/weibull_distribution.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.215956 GalSim-2.4.11/include/galsim/fmath/
--rw-r--r--   0 runner    (1001) docker     (123)    23954 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/fmath/fmath.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.143957 GalSim-2.4.11/include/galsim/fmath/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.215956 GalSim-2.4.11/include/galsim/fmath/include/cybozu/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/fmath/include/cybozu/benchmark.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/fmath/include/cybozu/inttype.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.215956 GalSim-2.4.11/include/galsim/hsm/
--rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/hsm/PSFCorr.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.215956 GalSim-2.4.11/include/galsim/integ/
--rw-r--r--   0 runner    (1001) docker     (123)    45294 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/integ/Int.h
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/integ/IntGKPData1.h
--rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/integ/IntGKPData10.h
--rw-r--r--   0 runner    (1001) docker     (123)    32193 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/integ/MoreFunctional.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.215956 GalSim-2.4.11/include/galsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/math/Angle.h
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/math/Bessel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/math/Gamma.h
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/math/Hankel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/math/Horner.h
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/math/Nan.h
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/math/Sinc.h
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-08-05 06:37:38.000000 GalSim-2.4.11/include/galsim/mmgr.h
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-05 06:37:38.000000 GalSim-2.4.11/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.223956 GalSim-2.4.11/pysrc/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/Bessel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/Bounds.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/CDModel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/HSM.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/Horner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/Image.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/Integ.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/Interpolant.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/PhotonArray.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/PyBind11Helper.h
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/Random.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/RealGalaxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBAdd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBAiry.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBBox.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBConvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBDeconvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBDeltaFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBExponential.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBFourierSqrt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBGaussian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBInclinedExponential.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBInclinedSersic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBInterpolatedImage.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBKolmogorov.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBMoffat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBProfile.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBSecondKick.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBSersic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBShapelet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBSpergel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBTransform.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/SBVonKarman.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/Silicon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/Table.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/WCS.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-05 06:37:38.000000 GalSim-2.4.11/pysrc/module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 06:38:41.287955 GalSim-2.4.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    56240 2023-08-05 06:37:38.000000 GalSim-2.4.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.227956 GalSim-2.4.11/share/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.227956 GalSim-2.4.11/share/SEDs/
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/CWW_E_ext.sed
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/CWW_E_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/CWW_Im_ext.sed
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/CWW_Im_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/CWW_Sbc_ext.sed
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/CWW_Sbc_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/CWW_Scd_ext.sed
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/CWW_Scd_ext_more.sed
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   102422 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/SEDs/vega.txt
--rw-r--r--   0 runner    (1001) docker     (123)    57600 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/acs_I_unrot_sci_20_cf.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.231956 GalSim-2.4.11/share/bandpasses/
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/ACS_wfc_F435W.dat
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/ACS_wfc_F606W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/ACS_wfc_F775W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/ACS_wfc_F814W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/ACS_wfc_F850LP.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/LSST_g.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/LSST_i.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/LSST_r.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/LSST_u.dat
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/LSST_y.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/LSST_z.dat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/WFC3_ir_F105W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/WFC3_ir_F125W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/WFC3_ir_F160W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/WFC3_uvis_F275W.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/bandpasses/WFC3_uvis_F336W.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.247956 GalSim-2.4.11/share/roman/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_01.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_02.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_03.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_04.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_05.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_06.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_07.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_08.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_12.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_13.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_14.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_15.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_16.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_17.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_18.txt
--rw-r--r--   0 runner    (1001) docker     (123)   204929 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)   207326 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43524 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA10_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA10_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43726 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA11_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43282 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA11_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43689 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA12_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43476 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA12_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43504 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA13_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43409 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA13_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43821 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA14_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43330 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA14_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA15_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43401 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA15_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43623 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA16_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43477 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA16_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA17_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43451 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA17_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43708 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA18_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43389 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA18_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43499 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA1_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43287 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA1_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA2_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43288 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA2_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43600 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA3_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43454 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA3_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43556 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA4_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43428 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA4_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43621 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA5_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43300 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA5_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43583 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA6_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43388 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA6_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43508 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA7_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43488 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA7_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43689 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA8_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43457 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA8_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43619 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA9_full_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    43394 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/SCA9_rim_mask.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/afta_throughput.txt
--rw-r--r--   0 runner    (1001) docker     (123)   251160 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/roman_sky_backgrounds.txt
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/sca_positions_7_6_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/roman/sip_7_6_8.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.255956 GalSim-2.4.11/share/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/abs_length.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_e2v_32.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_e2v_32.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_e2v_50_32.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_e2v_50_32.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_e2v_50_8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_e2v_50_8.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_e2v_8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_e2v_8.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_itl_32.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_itl_32.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_itl_50_32.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_itl_50_32.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_itl_50_8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_itl_50_8.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_itl_8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/sensors/lsst_itl_8.dat
--rw-r--r--   0 runner    (1001) docker     (123)   122780 2023-08-05 06:37:38.000000 GalSim-2.4.11/share/wfc_F814W.dat.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.267956 GalSim-2.4.11/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/BinomFact.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/CDModel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/CorrelatedNoise.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/GSParams.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    54337 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/Image.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/Image.inst
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/Interpolant.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19072 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/Laguerre.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/OneDimensionalDeviate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/PhotonArray.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/Polygon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/Random.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/RealGalaxy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/RealSpaceConvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBAdd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBAiry.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17398 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBBox.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBConvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBDeconvolve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBDeltaFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25768 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBExponential.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBFourierSqrt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBGaussian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBInclinedExponential.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBInclinedSersic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    62389 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBInterpolatedImage.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBKolmogorov.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25091 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBMoffat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBProfile.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBSecondKick.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    33842 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBSersic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBShapelet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    29887 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBSpergel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    44878 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBTransform.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/SBVonKarman.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    44894 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/Silicon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    53187 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/Table.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/Version.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/WCS.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.267956 GalSim-2.4.11/src/hsm/
--rw-r--r--   0 runner    (1001) docker     (123)    78798 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/hsm/PSFCorr.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.267956 GalSim-2.4.11/src/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/Angle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/Bessel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    43843 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/BesselI.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    74848 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/BesselJ.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    45424 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/BesselK.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/BesselRoots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    63931 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/BesselY.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/Gamma.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/Hankel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/Horner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/Nan.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/math/Sinc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    73348 2023-08-05 06:37:38.000000 GalSim-2.4.11/src/mmgr.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 06:38:41.287955 GalSim-2.4.11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_airy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_bessel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_cdmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    37420 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_celestial.py
--rw-r--r--   0 runner    (1001) docker     (123)   141699 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_chromatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    88450 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_config_gsobject.py
--rw-r--r--   0 runner    (1001) docker     (123)   134139 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_config_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_config_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_config_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    73330 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_config_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    87142 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_config_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    44668 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    69463 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_correlatednoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_deltafunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20533 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    34166 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_des.py
--rw-r--r--   0 runner    (1001) docker     (123)    22196 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    86441 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_fitsheader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_fouriersqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_galaxy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    48696 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_hsm.py
--rw-r--r--   0 runner    (1001) docker     (123)   167108 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    29519 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_inclined.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_integ.py
--rw-r--r--   0 runner    (1001) docker     (123)    85661 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_interpolatedimage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_knots.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_kolmogorov.py
--rw-r--r--   0 runner    (1001) docker     (123)    78587 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_lensing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_metacal.py
--rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_moffat.py
--rw-r--r--   0 runner    (1001) docker     (123)    35454 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    48308 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_optics.py
--rw-r--r--   0 runner    (1001) docker     (123)    64437 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_phase_psf.py
--rw-r--r--   0 runner    (1001) docker     (123)    71019 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_photon_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_pse.py
--rw-r--r--   0 runner    (1001) docker     (123)    79822 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)    43849 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_real.py
--rw-r--r--   0 runner    (1001) docker     (123)    58841 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_roman.py
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_second_kick.py
--rw-r--r--   0 runner    (1001) docker     (123)    51884 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_sed.py
--rw-r--r--   0 runner    (1001) docker     (123)    56330 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27306 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_sersic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_shapelet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_shear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_shear_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_spergel.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)    52794 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    47866 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    57324 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    15804 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_vonkarman.py
--rw-r--r--   0 runner    (1001) docker     (123)   152073 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-08-05 06:37:38.000000 GalSim-2.4.11/tests/test_zernike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.846001 GalSim-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-17 14:44:05.000000 GalSim-2.4.9/CHANGELOG.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.733999 GalSim-2.4.9/GalSim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-17 14:44:59.000000 GalSim-2.4.9/GalSim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-05-17 14:44:59.000000 GalSim-2.4.9/GalSim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:44:59.000000 GalSim-2.4.9/GalSim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-17 14:44:59.000000 GalSim-2.4.9/GalSim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:44:59.000000 GalSim-2.4.9/GalSim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-17 14:44:59.000000 GalSim-2.4.9/GalSim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 14:44:59.000000 GalSim-2.4.9/GalSim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-17 14:44:05.000000 GalSim-2.4.9/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-17 14:44:05.000000 GalSim-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-17 14:44:05.000000 GalSim-2.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-17 14:44:59.846001 GalSim-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-17 14:44:05.000000 GalSim-2.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.741999 GalSim-2.4.9/galsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/_pyfits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/airy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33326 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/bessel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/cdmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/celestial.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174490 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/chromatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.745999 GalSim-2.4.9/galsim/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23288 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/extra_badpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/extra_psf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/extra_truth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/extra_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/gsobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25719 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/image_scattered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/image_tiled.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30729 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/input_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/input_fitsheader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/input_nfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/input_powerspectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/input_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24359 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/output_datacube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/output_multifits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/photon_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/sed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55175 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/stamp_ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45344 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34823 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/value_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/value_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/config/wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40999 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88490 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/correlatednoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/dcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/deltafunction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.749999 GalSim-2.4.9/galsim/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/deprecated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/deprecated/correlatednoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/deprecated/integ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/deprecated/randwalk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.749999 GalSim-2.4.9/galsim/des/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/des/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/des/des_meds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/des/des_psfex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/des/des_shapelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/download_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65951 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83990 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/fitswcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/fouriersqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50214 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/galaxy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132375 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/gsobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/gsparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37460 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/hsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83673 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21113 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/inclined.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.749999 GalSim-2.4.9/galsim/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/GalSim.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.749999 GalSim-2.4.9/galsim/include/fftw3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/fftw3/fftw3.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.758000 GalSim-2.4.9/galsim/include/galsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/BinomFact.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Bounds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/CDModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/CorrelatedNoise.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/GSParams.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30925 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/ImageArith.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Interpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/LRUCache.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Laguerre.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/OneDimensionalDeviate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/PhotonArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Polygon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/ProbabilityTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/RealGalaxy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBAdd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBAddImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBAiry.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBAiryImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBBox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBBoxImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBConvolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBConvolveImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBDeconvolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBDeconvolveImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBDeltaFunction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBDeltaFunctionImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBExponential.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBExponentialImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBFourierSqrt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBFourierSqrtImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBGaussian.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBGaussianImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBInclinedExponential.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBInclinedExponentialImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBInclinedSersic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBInclinedSersicImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBInterpolatedImage.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBInterpolatedImageImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBKolmogorov.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBKolmogorovImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBMoffat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBMoffatImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBProfile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBProfileImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBSecondKick.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBSecondKickImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBSersic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBSersicImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBShapelet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBShapeletImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBSpergel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBSpergelImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBTransform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBTransformImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBVonKarman.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/SBVonKarmanImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Silicon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16801 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Std.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Stopwatch.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/Table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-17 14:44:59.000000 GalSim-2.4.9/galsim/include/galsim/Version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/WCS.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.758000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/LICENSE_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/assert.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.758000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/config/suffix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/current_function.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.758000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/binomial_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.762000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/detail/seed.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/exponential_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/gamma_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/mersenne_twister.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/normal_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/poisson_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/uniform_01.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/weibull_distribution.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.762000 GalSim-2.4.9/galsim/include/galsim/fmath/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/bench.sln
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/bench.vcproj
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/ck.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/fastexp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23954 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/fmath.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.729999 GalSim-2.4.9/galsim/include/galsim/fmath/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.762000 GalSim-2.4.9/galsim/include/galsim/fmath/include/cybozu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/include/cybozu/benchmark.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/include/cybozu/inttype.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/fmath/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.762000 GalSim-2.4.9/galsim/include/galsim/hsm/
+-rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/hsm/PSFCorr.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.762000 GalSim-2.4.9/galsim/include/galsim/integ/
+-rw-r--r--   0 runner    (1001) docker     (123)    45294 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/integ/Int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/integ/IntGKPData1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/integ/IntGKPData10.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32193 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/integ/MoreFunctional.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.762000 GalSim-2.4.9/galsim/include/galsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/math/Angle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/math/Bessel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/math/Gamma.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/math/Hankel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/math/Horner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/math/Nan.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/math/Sinc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/include/galsim/mmgr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/integ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23701 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/interpolant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58114 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/interpolatedimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12980 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/knots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/kolmogorov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77535 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/lensing_ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/moffat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/nfw_halo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26020 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107582 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/phase_psf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61323 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/phase_screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53397 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/photon_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/pse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39867 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70867 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/real.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.766000 GalSim-2.4.9/galsim/roman/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/roman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/roman/roman_backgrounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/roman/roman_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/roman/roman_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/roman/roman_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/roman/roman_psfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36583 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/roman/roman_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/second_kick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52182 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/sed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24811 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/sersic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/shapelet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.766000 GalSim-2.4.9/galsim/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.766000 GalSim-2.4.9/galsim/share/SEDs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/CWW_E_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/CWW_E_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/CWW_Im_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/CWW_Im_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/CWW_Sbc_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/CWW_Sbc_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/CWW_Scd_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/CWW_Scd_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   102422 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/SEDs/vega.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    57600 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/acs_I_unrot_sci_20_cf.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.770000 GalSim-2.4.9/galsim/share/bandpasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F435W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F606W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F775W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F814W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F850LP.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/LSST_g.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/LSST_i.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/LSST_r.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/LSST_u.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/LSST_y.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/LSST_z.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/WFC3_ir_F105W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/WFC3_ir_F125W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/WFC3_ir_F160W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/WFC3_uvis_F275W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/bandpasses/WFC3_uvis_F336W.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.778000 GalSim-2.4.9/galsim/share/roman/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_01.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_02.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_03.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_04.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_06.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_07.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_08.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_12.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_13.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_14.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_16.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_17.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_18.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   204929 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   207326 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43524 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA10_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA10_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43726 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA11_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43282 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA11_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43689 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA12_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43476 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA12_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43504 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA13_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43409 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA13_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43821 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA14_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43330 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA14_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA15_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43401 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA15_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43623 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA16_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43477 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA16_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA17_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43451 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA17_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43708 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA18_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43389 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA18_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43499 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA1_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43287 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA1_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA2_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43288 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA2_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43600 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA3_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43454 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA3_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43556 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA4_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43428 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA4_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43621 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA5_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43300 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA5_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43583 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA6_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43388 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA6_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43508 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA7_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43488 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA7_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43689 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA8_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43457 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA8_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43619 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA9_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43394 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/SCA9_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/afta_throughput.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   251160 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/roman_sky_backgrounds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/sca_positions_7_6_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/roman/sip_7_6_8.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.786000 GalSim-2.4.9/galsim/share/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/abs_length.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_e2v_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_e2v_32.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_e2v_50_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_e2v_50_32.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_e2v_50_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_e2v_50_8.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_e2v_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_e2v_8.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_itl_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_itl_32.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_itl_50_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_itl_50_32.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_itl_50_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_itl_50_8.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_itl_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/sensors/lsst_itl_8.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   122780 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/share/wfc_F814W.dat.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    17146 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/shear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/spergel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51390 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23848 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78545 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/vonkarman.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121609 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/wfirst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32968 2023-05-17 14:44:05.000000 GalSim-2.4.9/galsim/zernike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.786000 GalSim-2.4.9/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/GalSim.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.786000 GalSim-2.4.9/include/fftw3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/fftw3/fftw3.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.794000 GalSim-2.4.9/include/galsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/BinomFact.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Bounds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/CDModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/CorrelatedNoise.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/GSParams.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30925 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/ImageArith.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Interpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/LRUCache.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Laguerre.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/OneDimensionalDeviate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/PhotonArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Polygon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/ProbabilityTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/RealGalaxy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBAdd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBAddImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBAiry.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBAiryImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBBox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBBoxImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBConvolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBConvolveImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBDeconvolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBDeconvolveImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBDeltaFunction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBDeltaFunctionImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBExponential.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBExponentialImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBFourierSqrt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBFourierSqrtImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBGaussian.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBGaussianImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBInclinedExponential.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBInclinedExponentialImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBInclinedSersic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBInclinedSersicImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBInterpolatedImage.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBInterpolatedImageImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBKolmogorov.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBKolmogorovImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBMoffat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBMoffatImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBProfile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBProfileImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBSecondKick.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBSecondKickImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBSersic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBSersicImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBShapelet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBShapeletImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBSpergel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBSpergelImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBTransform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBTransformImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBVonKarman.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/SBVonKarmanImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Silicon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16801 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Std.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Stopwatch.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/Table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-17 14:44:59.000000 GalSim-2.4.9/include/galsim/Version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/WCS.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.794000 GalSim-2.4.9/include/galsim/boost1_48_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/assert.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.794000 GalSim-2.4.9/include/galsim/boost1_48_0/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/config/suffix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/current_function.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.798000 GalSim-2.4.9/include/galsim/boost1_48_0/random/
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/binomial_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.798000 GalSim-2.4.9/include/galsim/boost1_48_0/random/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/detail/seed.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/exponential_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/gamma_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/mersenne_twister.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/normal_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/poisson_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/uniform_01.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/boost1_48_0/random/weibull_distribution.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.798000 GalSim-2.4.9/include/galsim/fmath/
+-rw-r--r--   0 runner    (1001) docker     (123)    23954 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/fmath/fmath.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.729999 GalSim-2.4.9/include/galsim/fmath/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.798000 GalSim-2.4.9/include/galsim/fmath/include/cybozu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/fmath/include/cybozu/benchmark.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/fmath/include/cybozu/inttype.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.798000 GalSim-2.4.9/include/galsim/hsm/
+-rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/hsm/PSFCorr.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.798000 GalSim-2.4.9/include/galsim/integ/
+-rw-r--r--   0 runner    (1001) docker     (123)    45294 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/integ/Int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/integ/IntGKPData1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/integ/IntGKPData10.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32193 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/integ/MoreFunctional.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.798000 GalSim-2.4.9/include/galsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/math/Angle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/math/Bessel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/math/Gamma.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/math/Hankel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/math/Horner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/math/Nan.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/math/Sinc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-17 14:44:05.000000 GalSim-2.4.9/include/galsim/mmgr.h
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 14:44:05.000000 GalSim-2.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.806000 GalSim-2.4.9/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/Bessel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/Bounds.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/CDModel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/HSM.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/Horner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/Image.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/Integ.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/Interpolant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/PhotonArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/PyBind11Helper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/Random.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/RealGalaxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBAdd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBAiry.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBBox.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBConvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBDeconvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBDeltaFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBExponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBFourierSqrt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBGaussian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBInclinedExponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBInclinedSersic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBInterpolatedImage.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBKolmogorov.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBMoffat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBProfile.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBSecondKick.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBSersic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBShapelet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBSpergel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBTransform.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/SBVonKarman.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/Silicon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/Table.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/WCS.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-17 14:44:05.000000 GalSim-2.4.9/pysrc/module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:44:59.846001 GalSim-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    56240 2023-05-17 14:44:05.000000 GalSim-2.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.806000 GalSim-2.4.9/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.806000 GalSim-2.4.9/share/SEDs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/CWW_E_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/CWW_E_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/CWW_Im_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/CWW_Im_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/CWW_Sbc_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/CWW_Sbc_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/CWW_Scd_ext.sed
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/CWW_Scd_ext_more.sed
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   102422 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/SEDs/vega.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    57600 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/acs_I_unrot_sci_20_cf.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.810000 GalSim-2.4.9/share/bandpasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/ACS_wfc_F435W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/ACS_wfc_F606W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/ACS_wfc_F775W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/ACS_wfc_F814W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/ACS_wfc_F850LP.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/LSST_g.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/LSST_i.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/LSST_r.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/LSST_u.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/LSST_y.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/LSST_z.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/WFC3_ir_F105W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/WFC3_ir_F125W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/WFC3_ir_F160W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/WFC3_uvis_F275W.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/bandpasses/WFC3_uvis_F336W.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.818000 GalSim-2.4.9/share/roman/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_01.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_02.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_03.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_04.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_06.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_07.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_08.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_12.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_13.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_14.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_16.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_17.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_18.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   204929 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   207326 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43524 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA10_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA10_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43726 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA11_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43282 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA11_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43689 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA12_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43476 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA12_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43504 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA13_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43409 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA13_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43821 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA14_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43330 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA14_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA15_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43401 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA15_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43623 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA16_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43477 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA16_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA17_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43451 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA17_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43708 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA18_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43389 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA18_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43499 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA1_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43287 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA1_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA2_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43288 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA2_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43600 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA3_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43454 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA3_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43556 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA4_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43428 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA4_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43621 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA5_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43300 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA5_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43583 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA6_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43388 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA6_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43508 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA7_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43488 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA7_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43689 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA8_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43457 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA8_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43619 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA9_full_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43394 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/SCA9_rim_mask.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/afta_throughput.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   251160 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/roman_sky_backgrounds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/sca_positions_7_6_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/roman/sip_7_6_8.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.826001 GalSim-2.4.9/share/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/abs_length.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_e2v_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_e2v_32.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_e2v_50_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_e2v_50_32.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_e2v_50_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_e2v_50_8.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_e2v_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_e2v_8.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_itl_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_itl_32.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_itl_50_32.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   812668 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_itl_50_32.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_itl_50_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_itl_50_8.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_itl_8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   221692 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/sensors/lsst_itl_8.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   122780 2023-05-17 14:44:05.000000 GalSim-2.4.9/share/wfc_F814W.dat.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.830001 GalSim-2.4.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/BinomFact.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/CDModel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/CorrelatedNoise.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/GSParams.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    54337 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/Image.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/Image.inst
+-rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/Interpolant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19072 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/Laguerre.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/OneDimensionalDeviate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/PhotonArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/Polygon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/Random.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/RealGalaxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/RealSpaceConvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBAdd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBAiry.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17398 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBBox.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBConvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBDeconvolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBDeltaFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25768 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBExponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBFourierSqrt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBGaussian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBInclinedExponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBInclinedSersic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    62389 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBInterpolatedImage.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBKolmogorov.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25091 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBMoffat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBProfile.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBSecondKick.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    33842 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBSersic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBShapelet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29887 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBSpergel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    44878 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBTransform.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/SBVonKarman.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    44538 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/Silicon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    53187 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/Table.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/Version.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/WCS.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.830001 GalSim-2.4.9/src/hsm/
+-rw-r--r--   0 runner    (1001) docker     (123)    78798 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/hsm/PSFCorr.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.834001 GalSim-2.4.9/src/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/Angle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/Bessel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    43843 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/BesselI.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74848 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/BesselJ.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    45424 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/BesselK.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/BesselRoots.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    63931 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/BesselY.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/Gamma.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/Hankel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/Horner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/Nan.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/math/Sinc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    73348 2023-05-17 14:44:05.000000 GalSim-2.4.9/src/mmgr.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:44:59.846001 GalSim-2.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_airy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_bessel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_cdmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37420 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_celestial.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141699 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_chromatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88450 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_config_gsobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132988 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_config_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_config_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_config_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73330 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_config_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87142 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_config_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44668 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69463 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_correlatednoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_deltafunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20533 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34166 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22196 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86441 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_fitsheader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_fouriersqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_galaxy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48696 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_hsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167108 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29519 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_inclined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_integ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85661 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_interpolatedimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_knots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_kolmogorov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78587 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_lensing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_metacal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_moffat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35454 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48308 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_optics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64437 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_phase_psf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71019 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_photon_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_pse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79822 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43849 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58841 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_roman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_second_kick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51884 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_sed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54759 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27306 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_sersic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_shapelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_shear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_shear_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_spergel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52729 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47866 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57324 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15804 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_vonkarman.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152073 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-05-17 14:44:06.000000 GalSim-2.4.9/tests/test_zernike.py
```

### Comparing `GalSim-2.4.11/CHANGELOG.rst` & `GalSim-2.4.9/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -139,40 +139,26 @@
 
 - Fixed drawImage to work correctly for method=fft when using photon_ops. (#1193)
 - Fixed the proxies used by config Input items to allow access to attributes. (#1195)
 
 Changes from v2.4.6 to v2.4.7
 =============================
 
-- Fixed the flux scaling of drawReal for objects with non-diagonal jacobian. (#1197, #1198)
-- Added --log_format option to galsim executable. (#1201)
-- Allowed input objects with has_nobj=True to return an approximate number of objects for the
+- Fix the flux scaling of drawReal for objects with non-diagonal jacobian. (#1197, #1198)
+- Add --log_format option to galsim executable. (#1201)
+- Allow input objects with has_nobj=True to return an approximate number of objects for the
   initial pass, rather than the eventual exact number. (#1202)
-- Updated the Great3 links to non-broken URLs. (#1205)
-- Added options to InputLoader to make inputs with AtmosphericScreens work properly. (#1206)
+- Update the Great3 links to non-broken URLs. (#1205)
+- Add options to InputLoader to make inputs with AtmosphericScreens work properly. (#1206)
 - Only use proxies for input objects if not yet in a multiprocessing context. This had been
   causing significant slow downs in some imsim runs. (#1206)
 
 Changes from v2.4.7 to v2.4.8
 =============================
 
-- Fixed a slow-down in multiprocessing especially when running very many (>10) processes. (#1213)
+- Fix a slow-down in multiprocessing especially when running very many (>10) processes. (#1213)
 
 Changes from v2.4.8 to v2.4.9
 =============================
 
-- Fixed a potential segmentation fault that could happen when using photon_ops with FFT drawing.
+- Fix a potential segmentation fault that could happen when using photon_ops with FFT drawing.
   (#1216)
-
-Changes from v2.4.9 to v2.4.10
-==============================
-
-- Fixed the Silicon class to handle invalid wavelengths gracefully rather than raise an
-  exception. (#1227)
-
-Changes from v2.4.10 to v2.4.11
-===============================
-
-- Fixed the config template processing to handle recursive templates. (#1233)
-- Fixed the processing of modules in config files to allow sub-modules to be included without
-  requiring the parent module.  E.g. to include astropy.time as a module no longer requires
-  astropy to also be in the list of modules. (#1233)
```

### Comparing `GalSim-2.4.11/GalSim.egg-info/PKG-INFO` & `GalSim-2.4.9/GalSim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: GalSim
-Version: 2.4.11
+Version: 2.4.9
 Summary: The modular galaxy image simulation toolkit
 Home-page: https://github.com/GalSim-developers/GalSim
-Download-URL: https://github.com/GalSim-developers/GalSim/releases/tag/v2.4.11.zip
+Download-URL: https://github.com/GalSim-developers/GalSim/releases/tag/v2.4.9.zip
 Author: GalSim Developers (point of contact: Mike Jarvis)
 Author-email: michael@jarvis.net
 License: BSD License
 License-File: LICENSE
 
 .. image:: https://github.com/GalSim-developers/GalSim/workflows/GalSim%20CI/badge.svg
         :target: https://github.com/GalSim-developers/GalSim
```

### Comparing `GalSim-2.4.11/GalSim.egg-info/SOURCES.txt` & `GalSim-2.4.9/GalSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/INSTALL.rst` & `GalSim-2.4.9/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/LICENSE` & `GalSim-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/PKG-INFO` & `GalSim-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: GalSim
-Version: 2.4.11
+Version: 2.4.9
 Summary: The modular galaxy image simulation toolkit
 Home-page: https://github.com/GalSim-developers/GalSim
-Download-URL: https://github.com/GalSim-developers/GalSim/releases/tag/v2.4.11.zip
+Download-URL: https://github.com/GalSim-developers/GalSim/releases/tag/v2.4.9.zip
 Author: GalSim Developers (point of contact: Mike Jarvis)
 Author-email: michael@jarvis.net
 License: BSD License
 License-File: LICENSE
 
 .. image:: https://github.com/GalSim-developers/GalSim/workflows/GalSim%20CI/badge.svg
         :target: https://github.com/GalSim-developers/GalSim
```

### Comparing `GalSim-2.4.11/README.rst` & `GalSim-2.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/__init__.py` & `GalSim-2.4.9/galsim/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/__main__.py` & `GalSim-2.4.9/galsim/__main__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/_pyfits.py` & `GalSim-2.4.9/galsim/_pyfits.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/_version.py` & `GalSim-2.4.9/galsim/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions, and the disclaimer given in the accompanying LICENSE
 #    file.
 # 2. Redistributions in binary form must reproduce the above copyright notice,
 #    this list of conditions, and the disclaimer given in the documentation
 #    and/or other materials provided with the distribution.
 #
-__version__ = '2.4.11'
+__version__ = '2.4.9'
 __version_info__ = tuple(map(lambda x:int(x.split('-')[0]), __version__.split('.')))[:3]
```

### Comparing `GalSim-2.4.11/galsim/airy.py` & `GalSim-2.4.9/galsim/airy.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/angle.py` & `GalSim-2.4.9/galsim/angle.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/bandpass.py` & `GalSim-2.4.9/galsim/bandpass.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/bessel.py` & `GalSim-2.4.9/galsim/bessel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/bounds.py` & `GalSim-2.4.9/galsim/bounds.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/box.py` & `GalSim-2.4.9/galsim/box.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/catalog.py` & `GalSim-2.4.9/galsim/catalog.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/cdmodel.py` & `GalSim-2.4.9/galsim/cdmodel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/celestial.py` & `GalSim-2.4.9/galsim/celestial.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/chromatic.py` & `GalSim-2.4.9/galsim/chromatic.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/__init__.py` & `GalSim-2.4.9/galsim/config/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/bandpass.py` & `GalSim-2.4.9/galsim/config/bandpass.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/extra.py` & `GalSim-2.4.9/galsim/config/extra.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/extra_badpix.py` & `GalSim-2.4.9/galsim/config/extra_badpix.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/extra_psf.py` & `GalSim-2.4.9/galsim/config/extra_psf.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/extra_truth.py` & `GalSim-2.4.9/galsim/config/extra_truth.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/extra_weight.py` & `GalSim-2.4.9/galsim/config/extra_weight.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/gsobject.py` & `GalSim-2.4.9/galsim/config/gsobject.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/image.py` & `GalSim-2.4.9/galsim/config/image.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/image_scattered.py` & `GalSim-2.4.9/galsim/config/image_scattered.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/image_tiled.py` & `GalSim-2.4.9/galsim/config/image_tiled.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/input.py` & `GalSim-2.4.9/galsim/config/input.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/input_cosmos.py` & `GalSim-2.4.9/galsim/config/input_cosmos.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/input_fitsheader.py` & `GalSim-2.4.9/galsim/config/input_fitsheader.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/input_nfw.py` & `GalSim-2.4.9/galsim/config/input_nfw.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/input_powerspectrum.py` & `GalSim-2.4.9/galsim/config/input_powerspectrum.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/input_real.py` & `GalSim-2.4.9/galsim/config/input_real.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/noise.py` & `GalSim-2.4.9/galsim/config/noise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/output.py` & `GalSim-2.4.9/galsim/config/output.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/output_datacube.py` & `GalSim-2.4.9/galsim/config/output_datacube.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/output_multifits.py` & `GalSim-2.4.9/galsim/config/output_multifits.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/photon_ops.py` & `GalSim-2.4.9/galsim/config/photon_ops.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/process.py` & `GalSim-2.4.9/galsim/config/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,25 +112,26 @@
     effects of the import statements will persist.  In particular, these are allowed to
     register additional custom types that can then be used in the current config dict.
 
     Parameters:
         config:     The configuration dict.
     """
     import sys
+    from importlib import import_module
     if gdict is None:
         gdict = globals()
     if 'modules' in config:
         for module in config['modules']:
             try:
-                exec('import ' + module, gdict)
+                gdict[module] = import_module(module)
             except ImportError:
                 # Try adding '.' to path, in case loading a local module and '.' not present.
                 if '.' not in sys.path:
                     sys.path.append('.')
-                    exec('import ' + module, gdict)
+                    gdict[module] = import_module(module)
                 else:
                     raise
 
 def ProcessTemplate(config, base, logger=None):
     """If the config dict has a 'template' item, read in the appropriate file and
     make any requested updates.
 
@@ -170,17 +171,14 @@
         else:
             template = base
 
         # Pull out the specified field, if any
         if field is not None:
             template = GetFromConfig(template, field)
 
-        # In case template has further templates to process, do that now.
-        ProcessTemplate(template, base=base, logger=logger)
-
         # Copy over the template config into this one.
         new_params = config.copy()  # N.B. Already popped config['template'].
         config.clear()
 
         config.update(template)
 
         if 'modules' in config:
```

### Comparing `GalSim-2.4.11/galsim/config/sed.py` & `GalSim-2.4.9/galsim/config/sed.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/sensor.py` & `GalSim-2.4.9/galsim/config/sensor.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/stamp.py` & `GalSim-2.4.9/galsim/config/stamp.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/stamp_ring.py` & `GalSim-2.4.9/galsim/config/stamp_ring.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/util.py` & `GalSim-2.4.9/galsim/config/util.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/value.py` & `GalSim-2.4.9/galsim/config/value.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/value_eval.py` & `GalSim-2.4.9/galsim/config/value_eval.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/value_random.py` & `GalSim-2.4.9/galsim/config/value_random.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/config/wcs.py` & `GalSim-2.4.9/galsim/config/wcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/convolve.py` & `GalSim-2.4.9/galsim/convolve.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/correlatednoise.py` & `GalSim-2.4.9/galsim/correlatednoise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/dcr.py` & `GalSim-2.4.9/galsim/dcr.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/deltafunction.py` & `GalSim-2.4.9/galsim/deltafunction.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/deprecated/__init__.py` & `GalSim-2.4.9/galsim/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/deprecated/correlatednoise.py` & `GalSim-2.4.9/galsim/deprecated/correlatednoise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/deprecated/integ.py` & `GalSim-2.4.9/galsim/deprecated/integ.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/deprecated/randwalk.py` & `GalSim-2.4.9/galsim/deprecated/randwalk.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/des/__init__.py` & `GalSim-2.4.9/galsim/des/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/des/des_meds.py` & `GalSim-2.4.9/galsim/des/des_meds.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/des/des_psfex.py` & `GalSim-2.4.9/galsim/des/des_psfex.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/des/des_shapelet.py` & `GalSim-2.4.9/galsim/des/des_shapelet.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/detectors.py` & `GalSim-2.4.9/galsim/detectors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/download_cosmos.py` & `GalSim-2.4.9/galsim/download_cosmos.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/errors.py` & `GalSim-2.4.9/galsim/errors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/exponential.py` & `GalSim-2.4.9/galsim/exponential.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/fft.py` & `GalSim-2.4.9/galsim/fft.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/fits.py` & `GalSim-2.4.9/galsim/fits.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/fitswcs.py` & `GalSim-2.4.9/galsim/fitswcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/fouriersqrt.py` & `GalSim-2.4.9/galsim/fouriersqrt.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/galaxy_sample.py` & `GalSim-2.4.9/galsim/galaxy_sample.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/gaussian.py` & `GalSim-2.4.9/galsim/gaussian.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/gsobject.py` & `GalSim-2.4.9/galsim/gsobject.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/gsparams.py` & `GalSim-2.4.9/galsim/gsparams.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/hsm.py` & `GalSim-2.4.9/galsim/hsm.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/image.py` & `GalSim-2.4.9/galsim/image.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/inclined.py` & `GalSim-2.4.9/galsim/inclined.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/GalSim.h` & `GalSim-2.4.9/galsim/include/GalSim.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/fftw3/fftw3.h` & `GalSim-2.4.9/galsim/include/fftw3/fftw3.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/BinomFact.h` & `GalSim-2.4.9/galsim/include/galsim/BinomFact.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Bounds.h` & `GalSim-2.4.9/galsim/include/galsim/Bounds.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/CDModel.h` & `GalSim-2.4.9/galsim/include/galsim/CDModel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/CorrelatedNoise.h` & `GalSim-2.4.9/galsim/include/galsim/CorrelatedNoise.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/GSParams.h` & `GalSim-2.4.9/galsim/include/galsim/GSParams.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Image.h` & `GalSim-2.4.9/galsim/include/galsim/Image.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/ImageArith.h` & `GalSim-2.4.9/galsim/include/galsim/ImageArith.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Interpolant.h` & `GalSim-2.4.9/galsim/include/galsim/Interpolant.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/LRUCache.h` & `GalSim-2.4.9/galsim/include/galsim/LRUCache.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Laguerre.h` & `GalSim-2.4.9/galsim/include/galsim/Laguerre.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/OneDimensionalDeviate.h` & `GalSim-2.4.9/galsim/include/galsim/OneDimensionalDeviate.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/PhotonArray.h` & `GalSim-2.4.9/galsim/include/galsim/PhotonArray.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Polygon.h` & `GalSim-2.4.9/galsim/include/galsim/Polygon.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/ProbabilityTree.h` & `GalSim-2.4.9/galsim/include/galsim/ProbabilityTree.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Random.h` & `GalSim-2.4.9/galsim/include/galsim/Random.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/RealGalaxy.h` & `GalSim-2.4.9/galsim/include/galsim/RealGalaxy.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBAdd.h` & `GalSim-2.4.9/galsim/include/galsim/SBAdd.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBAddImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBAddImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBAiry.h` & `GalSim-2.4.9/galsim/include/galsim/SBAiry.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBAiryImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBAiryImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBBox.h` & `GalSim-2.4.9/galsim/include/galsim/SBBox.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBBoxImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBBoxImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBConvolve.h` & `GalSim-2.4.9/galsim/include/galsim/SBConvolve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBConvolveImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBConvolveImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBDeconvolve.h` & `GalSim-2.4.9/galsim/include/galsim/SBDeconvolve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBDeconvolveImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBDeconvolveImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBDeltaFunction.h` & `GalSim-2.4.9/galsim/include/galsim/SBDeltaFunction.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBDeltaFunctionImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBDeltaFunctionImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBExponential.h` & `GalSim-2.4.9/galsim/include/galsim/SBExponential.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBExponentialImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBExponentialImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBFourierSqrt.h` & `GalSim-2.4.9/galsim/include/galsim/SBFourierSqrt.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBFourierSqrtImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBFourierSqrtImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBGaussian.h` & `GalSim-2.4.9/galsim/include/galsim/SBGaussian.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBGaussianImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBGaussianImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBInclinedExponential.h` & `GalSim-2.4.9/galsim/include/galsim/SBInclinedExponential.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBInclinedExponentialImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBInclinedExponentialImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBInclinedSersic.h` & `GalSim-2.4.9/galsim/include/galsim/SBInclinedSersic.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBInclinedSersicImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBInclinedSersicImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBInterpolatedImage.h` & `GalSim-2.4.9/galsim/include/galsim/SBInterpolatedImage.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBInterpolatedImageImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBInterpolatedImageImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBKolmogorov.h` & `GalSim-2.4.9/galsim/include/galsim/SBKolmogorov.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBKolmogorovImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBKolmogorovImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBMoffat.h` & `GalSim-2.4.9/galsim/include/galsim/SBMoffat.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBMoffatImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBMoffatImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBProfile.h` & `GalSim-2.4.9/galsim/include/galsim/SBProfile.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBProfileImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBProfileImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBSecondKick.h` & `GalSim-2.4.9/galsim/include/galsim/SBSecondKick.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBSecondKickImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBSecondKickImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBSersic.h` & `GalSim-2.4.9/galsim/include/galsim/SBSersic.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBSersicImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBSersicImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBShapelet.h` & `GalSim-2.4.9/galsim/include/galsim/SBShapelet.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBShapeletImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBShapeletImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBSpergel.h` & `GalSim-2.4.9/galsim/include/galsim/SBSpergel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBSpergelImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBSpergelImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBTransform.h` & `GalSim-2.4.9/galsim/include/galsim/SBTransform.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBTransformImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBTransformImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBVonKarman.h` & `GalSim-2.4.9/galsim/include/galsim/SBVonKarman.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/SBVonKarmanImpl.h` & `GalSim-2.4.9/galsim/include/galsim/SBVonKarmanImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Silicon.h` & `GalSim-2.4.9/galsim/include/galsim/Silicon.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Solve.h` & `GalSim-2.4.9/galsim/include/galsim/Solve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Std.h` & `GalSim-2.4.9/galsim/include/galsim/Std.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Stopwatch.h` & `GalSim-2.4.9/galsim/include/galsim/Stopwatch.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Table.h` & `GalSim-2.4.9/galsim/include/galsim/Table.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/Version.h` & `GalSim-2.4.9/galsim/include/galsim/Version.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 // This file is auto-generated by setup.py.  Do not edit.
 #define GALSIM_MAJOR 2
 #define GALSIM_MINOR 4
-#define GALSIM_REVISION 11
+#define GALSIM_REVISION 9
 
 #include <string>
 #include <sstream>
 
 #if defined(__GNUC__)
 #define PUBLIC_API __attribute__ ((visibility ("default")))
 #else
```

### Comparing `GalSim-2.4.11/galsim/include/galsim/WCS.h` & `GalSim-2.4.9/galsim/include/galsim/WCS.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/LICENSE_1_0.txt` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/LICENSE_1_0.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/README` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/README`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/assert.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/assert.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/config/suffix.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/config/suffix.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/current_function.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/current_function.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/binomial_distribution.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/binomial_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/detail/seed.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/detail/seed.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/exponential_distribution.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/exponential_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/gamma_distribution.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/gamma_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/mersenne_twister.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/mersenne_twister.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/normal_distribution.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/normal_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/poisson_distribution.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/poisson_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/uniform_01.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/uniform_01.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/boost1_48_0/random/weibull_distribution.hpp` & `GalSim-2.4.9/galsim/include/galsim/boost1_48_0/random/weibull_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/Makefile` & `GalSim-2.4.9/galsim/include/galsim/fmath/Makefile`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/avx2.cpp` & `GalSim-2.4.9/galsim/include/galsim/fmath/avx2.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/bench.cpp` & `GalSim-2.4.9/galsim/include/galsim/fmath/bench.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/bench.sln` & `GalSim-2.4.9/galsim/include/galsim/fmath/bench.sln`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/bench.vcproj` & `GalSim-2.4.9/galsim/include/galsim/fmath/bench.vcproj`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/ck.cpp` & `GalSim-2.4.9/galsim/include/galsim/fmath/ck.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/fastexp.cpp` & `GalSim-2.4.9/galsim/include/galsim/fmath/fastexp.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/fmath.hpp` & `GalSim-2.4.9/galsim/include/galsim/fmath/fmath.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/include/cybozu/benchmark.hpp` & `GalSim-2.4.9/galsim/include/galsim/fmath/include/cybozu/benchmark.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/include/cybozu/inttype.hpp` & `GalSim-2.4.9/galsim/include/galsim/fmath/include/cybozu/inttype.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/readme.md` & `GalSim-2.4.9/galsim/include/galsim/fmath/readme.md`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/fmath/readme.txt` & `GalSim-2.4.9/galsim/include/galsim/fmath/readme.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/hsm/PSFCorr.h` & `GalSim-2.4.9/galsim/include/galsim/hsm/PSFCorr.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/integ/Int.h` & `GalSim-2.4.9/galsim/include/galsim/integ/Int.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/integ/IntGKPData1.h` & `GalSim-2.4.9/galsim/include/galsim/integ/IntGKPData1.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/integ/IntGKPData10.h` & `GalSim-2.4.9/galsim/include/galsim/integ/IntGKPData10.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/integ/MoreFunctional.h` & `GalSim-2.4.9/galsim/include/galsim/integ/MoreFunctional.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/math/Angle.h` & `GalSim-2.4.9/galsim/include/galsim/math/Angle.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/math/Bessel.h` & `GalSim-2.4.9/galsim/include/galsim/math/Bessel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/math/Gamma.h` & `GalSim-2.4.9/galsim/include/galsim/math/Gamma.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/math/Hankel.h` & `GalSim-2.4.9/galsim/include/galsim/math/Hankel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/math/Horner.h` & `GalSim-2.4.9/galsim/include/galsim/math/Horner.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/math/Nan.h` & `GalSim-2.4.9/galsim/include/galsim/math/Nan.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/math/Sinc.h` & `GalSim-2.4.9/galsim/include/galsim/math/Sinc.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/include/galsim/mmgr.h` & `GalSim-2.4.9/galsim/include/galsim/mmgr.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/integ.py` & `GalSim-2.4.9/galsim/integ.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/interpolant.py` & `GalSim-2.4.9/galsim/interpolant.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/interpolatedimage.py` & `GalSim-2.4.9/galsim/interpolatedimage.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/knots.py` & `GalSim-2.4.9/galsim/knots.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/kolmogorov.py` & `GalSim-2.4.9/galsim/kolmogorov.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/lensing_ps.py` & `GalSim-2.4.9/galsim/lensing_ps.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/main.py` & `GalSim-2.4.9/galsim/main.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/meta_data.py` & `GalSim-2.4.9/galsim/meta_data.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/moffat.py` & `GalSim-2.4.9/galsim/moffat.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/nfw_halo.py` & `GalSim-2.4.9/galsim/nfw_halo.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/noise.py` & `GalSim-2.4.9/galsim/noise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/phase_psf.py` & `GalSim-2.4.9/galsim/phase_psf.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/phase_screens.py` & `GalSim-2.4.9/galsim/phase_screens.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/photon_array.py` & `GalSim-2.4.9/galsim/photon_array.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/position.py` & `GalSim-2.4.9/galsim/position.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/pse.py` & `GalSim-2.4.9/galsim/pse.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/random.py` & `GalSim-2.4.9/galsim/random.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/real.py` & `GalSim-2.4.9/galsim/real.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/roman/__init__.py` & `GalSim-2.4.9/galsim/roman/__init__.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/roman/roman_backgrounds.py` & `GalSim-2.4.9/galsim/roman/roman_backgrounds.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/roman/roman_bandpass.py` & `GalSim-2.4.9/galsim/roman/roman_bandpass.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/roman/roman_config.py` & `GalSim-2.4.9/galsim/roman/roman_config.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/roman/roman_detectors.py` & `GalSim-2.4.9/galsim/roman/roman_detectors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/roman/roman_psfs.py` & `GalSim-2.4.9/galsim/roman/roman_psfs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/roman/roman_wcs.py` & `GalSim-2.4.9/galsim/roman/roman_wcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/second_kick.py` & `GalSim-2.4.9/galsim/second_kick.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/sed.py` & `GalSim-2.4.9/galsim/sed.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/sensor.py` & `GalSim-2.4.9/galsim/sensor.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/sersic.py` & `GalSim-2.4.9/galsim/sersic.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/shapelet.py` & `GalSim-2.4.9/galsim/shapelet.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/SEDs/CWW_E_ext.sed` & `GalSim-2.4.9/galsim/share/SEDs/CWW_E_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/SEDs/CWW_E_ext_more.sed` & `GalSim-2.4.9/galsim/share/SEDs/CWW_E_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/SEDs/CWW_Im_ext.sed` & `GalSim-2.4.9/galsim/share/SEDs/CWW_Im_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/SEDs/CWW_Im_ext_more.sed` & `GalSim-2.4.9/galsim/share/SEDs/CWW_Im_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/SEDs/CWW_Sbc_ext.sed` & `GalSim-2.4.9/galsim/share/SEDs/CWW_Sbc_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/SEDs/CWW_Sbc_ext_more.sed` & `GalSim-2.4.9/galsim/share/SEDs/CWW_Sbc_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/SEDs/CWW_Scd_ext.sed` & `GalSim-2.4.9/galsim/share/SEDs/CWW_Scd_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/SEDs/CWW_Scd_ext_more.sed` & `GalSim-2.4.9/galsim/share/SEDs/CWW_Scd_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/SEDs/vega.txt` & `GalSim-2.4.9/galsim/share/SEDs/vega.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/acs_I_unrot_sci_20_cf.fits` & `GalSim-2.4.9/galsim/share/acs_I_unrot_sci_20_cf.fits`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F435W.dat` & `GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F435W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F606W.dat` & `GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F606W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F775W.dat` & `GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F775W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F814W.dat` & `GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F814W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/ACS_wfc_F850LP.dat` & `GalSim-2.4.9/galsim/share/bandpasses/ACS_wfc_F850LP.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/LSST_g.dat` & `GalSim-2.4.9/galsim/share/bandpasses/LSST_g.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/LSST_i.dat` & `GalSim-2.4.9/galsim/share/bandpasses/LSST_i.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/LSST_r.dat` & `GalSim-2.4.9/galsim/share/bandpasses/LSST_r.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/LSST_u.dat` & `GalSim-2.4.9/galsim/share/bandpasses/LSST_u.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/LSST_y.dat` & `GalSim-2.4.9/galsim/share/bandpasses/LSST_y.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/LSST_z.dat` & `GalSim-2.4.9/galsim/share/bandpasses/LSST_z.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/WFC3_ir_F105W.dat` & `GalSim-2.4.9/galsim/share/bandpasses/WFC3_ir_F105W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/WFC3_ir_F125W.dat` & `GalSim-2.4.9/galsim/share/bandpasses/WFC3_ir_F125W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/WFC3_ir_F160W.dat` & `GalSim-2.4.9/galsim/share/bandpasses/WFC3_ir_F160W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/WFC3_uvis_F275W.dat` & `GalSim-2.4.9/galsim/share/bandpasses/WFC3_uvis_F275W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/bandpasses/WFC3_uvis_F336W.dat` & `GalSim-2.4.9/galsim/share/bandpasses/WFC3_uvis_F336W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_01.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_01.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_02.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_02.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_03.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_03.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_04.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_04.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_05.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_05.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_06.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_06.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_07.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_07.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_08.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_08.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_09.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_09.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_10.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_10.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_11.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_11.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_12.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_12.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_13.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_13.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_14.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_14.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_15.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_15.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_16.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_16.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_17.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_17.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_18.txt` & `GalSim-2.4.9/galsim/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_18.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz` & `GalSim-2.4.9/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz` & `GalSim-2.4.9/galsim/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA10_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA10_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA10_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA10_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA11_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA11_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA11_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA11_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA12_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA12_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA12_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA12_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA13_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA13_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA13_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA13_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA14_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA14_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA14_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA14_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA15_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA15_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA15_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA15_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA16_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA16_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA16_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA16_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA17_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA17_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA17_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA17_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA18_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA18_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA18_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA18_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA1_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA1_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA1_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA1_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA2_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA2_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA2_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA2_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA3_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA3_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA3_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA3_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA4_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA4_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA4_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA4_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA5_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA5_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA5_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA5_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA6_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA6_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA6_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA6_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA7_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA7_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA7_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA7_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA8_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA8_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA8_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA8_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA9_full_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA9_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/SCA9_rim_mask.fits.gz` & `GalSim-2.4.9/galsim/share/roman/SCA9_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/afta_throughput.txt` & `GalSim-2.4.9/galsim/share/roman/afta_throughput.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/roman_sky_backgrounds.txt` & `GalSim-2.4.9/galsim/share/roman/roman_sky_backgrounds.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/sca_positions_7_6_8.txt` & `GalSim-2.4.9/galsim/share/roman/sca_positions_7_6_8.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/roman/sip_7_6_8.txt` & `GalSim-2.4.9/galsim/share/roman/sip_7_6_8.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/abs_length.dat` & `GalSim-2.4.9/galsim/share/sensors/abs_length.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_e2v_32.cfg` & `GalSim-2.4.9/galsim/share/sensors/lsst_e2v_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_e2v_32.dat` & `GalSim-2.4.9/galsim/share/sensors/lsst_e2v_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_e2v_50_32.cfg` & `GalSim-2.4.9/galsim/share/sensors/lsst_e2v_50_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_e2v_50_32.dat` & `GalSim-2.4.9/galsim/share/sensors/lsst_e2v_50_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_e2v_50_8.cfg` & `GalSim-2.4.9/galsim/share/sensors/lsst_e2v_50_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_e2v_50_8.dat` & `GalSim-2.4.9/galsim/share/sensors/lsst_e2v_50_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_e2v_8.cfg` & `GalSim-2.4.9/galsim/share/sensors/lsst_e2v_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_e2v_8.dat` & `GalSim-2.4.9/galsim/share/sensors/lsst_e2v_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_itl_32.cfg` & `GalSim-2.4.9/galsim/share/sensors/lsst_itl_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_itl_32.dat` & `GalSim-2.4.9/galsim/share/sensors/lsst_itl_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_itl_50_32.cfg` & `GalSim-2.4.9/galsim/share/sensors/lsst_itl_50_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_itl_50_32.dat` & `GalSim-2.4.9/galsim/share/sensors/lsst_itl_50_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_itl_50_8.cfg` & `GalSim-2.4.9/galsim/share/sensors/lsst_itl_50_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_itl_50_8.dat` & `GalSim-2.4.9/galsim/share/sensors/lsst_itl_50_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_itl_8.cfg` & `GalSim-2.4.9/galsim/share/sensors/lsst_itl_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/sensors/lsst_itl_8.dat` & `GalSim-2.4.9/galsim/share/sensors/lsst_itl_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/share/wfc_F814W.dat.gz` & `GalSim-2.4.9/galsim/share/wfc_F814W.dat.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/shear.py` & `GalSim-2.4.9/galsim/shear.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/spergel.py` & `GalSim-2.4.9/galsim/spergel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/sum.py` & `GalSim-2.4.9/galsim/sum.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/table.py` & `GalSim-2.4.9/galsim/table.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/transform.py` & `GalSim-2.4.9/galsim/transform.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/utilities.py` & `GalSim-2.4.9/galsim/utilities.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/vonkarman.py` & `GalSim-2.4.9/galsim/vonkarman.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/wcs.py` & `GalSim-2.4.9/galsim/wcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/wfirst.py` & `GalSim-2.4.9/galsim/wfirst.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/galsim/zernike.py` & `GalSim-2.4.9/galsim/zernike.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/GalSim.h` & `GalSim-2.4.9/include/GalSim.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/fftw3/fftw3.h` & `GalSim-2.4.9/include/fftw3/fftw3.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/BinomFact.h` & `GalSim-2.4.9/include/galsim/BinomFact.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Bounds.h` & `GalSim-2.4.9/include/galsim/Bounds.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/CDModel.h` & `GalSim-2.4.9/include/galsim/CDModel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/CorrelatedNoise.h` & `GalSim-2.4.9/include/galsim/CorrelatedNoise.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/GSParams.h` & `GalSim-2.4.9/include/galsim/GSParams.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Image.h` & `GalSim-2.4.9/include/galsim/Image.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/ImageArith.h` & `GalSim-2.4.9/include/galsim/ImageArith.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Interpolant.h` & `GalSim-2.4.9/include/galsim/Interpolant.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/LRUCache.h` & `GalSim-2.4.9/include/galsim/LRUCache.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Laguerre.h` & `GalSim-2.4.9/include/galsim/Laguerre.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/OneDimensionalDeviate.h` & `GalSim-2.4.9/include/galsim/OneDimensionalDeviate.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/PhotonArray.h` & `GalSim-2.4.9/include/galsim/PhotonArray.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Polygon.h` & `GalSim-2.4.9/include/galsim/Polygon.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/ProbabilityTree.h` & `GalSim-2.4.9/include/galsim/ProbabilityTree.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Random.h` & `GalSim-2.4.9/include/galsim/Random.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/RealGalaxy.h` & `GalSim-2.4.9/include/galsim/RealGalaxy.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBAdd.h` & `GalSim-2.4.9/include/galsim/SBAdd.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBAddImpl.h` & `GalSim-2.4.9/include/galsim/SBAddImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBAiry.h` & `GalSim-2.4.9/include/galsim/SBAiry.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBAiryImpl.h` & `GalSim-2.4.9/include/galsim/SBAiryImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBBox.h` & `GalSim-2.4.9/include/galsim/SBBox.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBBoxImpl.h` & `GalSim-2.4.9/include/galsim/SBBoxImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBConvolve.h` & `GalSim-2.4.9/include/galsim/SBConvolve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBConvolveImpl.h` & `GalSim-2.4.9/include/galsim/SBConvolveImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBDeconvolve.h` & `GalSim-2.4.9/include/galsim/SBDeconvolve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBDeconvolveImpl.h` & `GalSim-2.4.9/include/galsim/SBDeconvolveImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBDeltaFunction.h` & `GalSim-2.4.9/include/galsim/SBDeltaFunction.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBDeltaFunctionImpl.h` & `GalSim-2.4.9/include/galsim/SBDeltaFunctionImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBExponential.h` & `GalSim-2.4.9/include/galsim/SBExponential.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBExponentialImpl.h` & `GalSim-2.4.9/include/galsim/SBExponentialImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBFourierSqrt.h` & `GalSim-2.4.9/include/galsim/SBFourierSqrt.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBFourierSqrtImpl.h` & `GalSim-2.4.9/include/galsim/SBFourierSqrtImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBGaussian.h` & `GalSim-2.4.9/include/galsim/SBGaussian.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBGaussianImpl.h` & `GalSim-2.4.9/include/galsim/SBGaussianImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBInclinedExponential.h` & `GalSim-2.4.9/include/galsim/SBInclinedExponential.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBInclinedExponentialImpl.h` & `GalSim-2.4.9/include/galsim/SBInclinedExponentialImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBInclinedSersic.h` & `GalSim-2.4.9/include/galsim/SBInclinedSersic.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBInclinedSersicImpl.h` & `GalSim-2.4.9/include/galsim/SBInclinedSersicImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBInterpolatedImage.h` & `GalSim-2.4.9/include/galsim/SBInterpolatedImage.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBInterpolatedImageImpl.h` & `GalSim-2.4.9/include/galsim/SBInterpolatedImageImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBKolmogorov.h` & `GalSim-2.4.9/include/galsim/SBKolmogorov.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBKolmogorovImpl.h` & `GalSim-2.4.9/include/galsim/SBKolmogorovImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBMoffat.h` & `GalSim-2.4.9/include/galsim/SBMoffat.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBMoffatImpl.h` & `GalSim-2.4.9/include/galsim/SBMoffatImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBProfile.h` & `GalSim-2.4.9/include/galsim/SBProfile.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBProfileImpl.h` & `GalSim-2.4.9/include/galsim/SBProfileImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBSecondKick.h` & `GalSim-2.4.9/include/galsim/SBSecondKick.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBSecondKickImpl.h` & `GalSim-2.4.9/include/galsim/SBSecondKickImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBSersic.h` & `GalSim-2.4.9/include/galsim/SBSersic.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBSersicImpl.h` & `GalSim-2.4.9/include/galsim/SBSersicImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBShapelet.h` & `GalSim-2.4.9/include/galsim/SBShapelet.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBShapeletImpl.h` & `GalSim-2.4.9/include/galsim/SBShapeletImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBSpergel.h` & `GalSim-2.4.9/include/galsim/SBSpergel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBSpergelImpl.h` & `GalSim-2.4.9/include/galsim/SBSpergelImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBTransform.h` & `GalSim-2.4.9/include/galsim/SBTransform.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBTransformImpl.h` & `GalSim-2.4.9/include/galsim/SBTransformImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBVonKarman.h` & `GalSim-2.4.9/include/galsim/SBVonKarman.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/SBVonKarmanImpl.h` & `GalSim-2.4.9/include/galsim/SBVonKarmanImpl.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Silicon.h` & `GalSim-2.4.9/include/galsim/Silicon.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Solve.h` & `GalSim-2.4.9/include/galsim/Solve.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Std.h` & `GalSim-2.4.9/include/galsim/Std.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Stopwatch.h` & `GalSim-2.4.9/include/galsim/Stopwatch.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Table.h` & `GalSim-2.4.9/include/galsim/Table.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/Version.h` & `GalSim-2.4.9/include/galsim/Version.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 // This file is auto-generated by setup.py.  Do not edit.
 #define GALSIM_MAJOR 2
 #define GALSIM_MINOR 4
-#define GALSIM_REVISION 11
+#define GALSIM_REVISION 9
 
 #include <string>
 #include <sstream>
 
 #if defined(__GNUC__)
 #define PUBLIC_API __attribute__ ((visibility ("default")))
 #else
```

### Comparing `GalSim-2.4.11/include/galsim/WCS.h` & `GalSim-2.4.9/include/galsim/WCS.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/assert.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/assert.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/config/suffix.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/config/suffix.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/current_function.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/current_function.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/binomial_distribution.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/binomial_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/chi_squared_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/detail/generator_seed_seq.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/detail/ptr_helper.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/detail/seed.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/detail/seed.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/detail/signed_unsigned_tools.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/exponential_distribution.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/exponential_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/gamma_distribution.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/gamma_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/mersenne_twister.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/mersenne_twister.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/normal_distribution.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/normal_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/poisson_distribution.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/poisson_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/uniform_01.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/uniform_01.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/uniform_real_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/boost1_48_0/random/weibull_distribution.hpp` & `GalSim-2.4.9/include/galsim/boost1_48_0/random/weibull_distribution.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/fmath/fmath.hpp` & `GalSim-2.4.9/include/galsim/fmath/fmath.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/fmath/include/cybozu/benchmark.hpp` & `GalSim-2.4.9/include/galsim/fmath/include/cybozu/benchmark.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/fmath/include/cybozu/inttype.hpp` & `GalSim-2.4.9/include/galsim/fmath/include/cybozu/inttype.hpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/hsm/PSFCorr.h` & `GalSim-2.4.9/include/galsim/hsm/PSFCorr.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/integ/Int.h` & `GalSim-2.4.9/include/galsim/integ/Int.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/integ/IntGKPData1.h` & `GalSim-2.4.9/include/galsim/integ/IntGKPData1.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/integ/IntGKPData10.h` & `GalSim-2.4.9/include/galsim/integ/IntGKPData10.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/integ/MoreFunctional.h` & `GalSim-2.4.9/include/galsim/integ/MoreFunctional.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/math/Angle.h` & `GalSim-2.4.9/include/galsim/math/Angle.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/math/Bessel.h` & `GalSim-2.4.9/include/galsim/math/Bessel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/math/Gamma.h` & `GalSim-2.4.9/include/galsim/math/Gamma.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/math/Hankel.h` & `GalSim-2.4.9/include/galsim/math/Hankel.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/math/Horner.h` & `GalSim-2.4.9/include/galsim/math/Horner.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/math/Nan.h` & `GalSim-2.4.9/include/galsim/math/Nan.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/math/Sinc.h` & `GalSim-2.4.9/include/galsim/math/Sinc.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/include/galsim/mmgr.h` & `GalSim-2.4.9/include/galsim/mmgr.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/Bessel.cpp` & `GalSim-2.4.9/pysrc/Bessel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/Bounds.cpp` & `GalSim-2.4.9/pysrc/Bounds.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/CDModel.cpp` & `GalSim-2.4.9/pysrc/CDModel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/HSM.cpp` & `GalSim-2.4.9/pysrc/HSM.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/Horner.cpp` & `GalSim-2.4.9/pysrc/Horner.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/Image.cpp` & `GalSim-2.4.9/pysrc/Image.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/Integ.cpp` & `GalSim-2.4.9/pysrc/Integ.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/Interpolant.cpp` & `GalSim-2.4.9/pysrc/Interpolant.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/PhotonArray.cpp` & `GalSim-2.4.9/pysrc/PhotonArray.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/PyBind11Helper.h` & `GalSim-2.4.9/pysrc/PyBind11Helper.h`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/Random.cpp` & `GalSim-2.4.9/pysrc/Random.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/RealGalaxy.cpp` & `GalSim-2.4.9/pysrc/RealGalaxy.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBAdd.cpp` & `GalSim-2.4.9/pysrc/SBAdd.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBAiry.cpp` & `GalSim-2.4.9/pysrc/SBAiry.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBBox.cpp` & `GalSim-2.4.9/pysrc/SBBox.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBConvolve.cpp` & `GalSim-2.4.9/pysrc/SBConvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBDeconvolve.cpp` & `GalSim-2.4.9/pysrc/SBDeconvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBDeltaFunction.cpp` & `GalSim-2.4.9/pysrc/SBDeltaFunction.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBExponential.cpp` & `GalSim-2.4.9/pysrc/SBExponential.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBFourierSqrt.cpp` & `GalSim-2.4.9/pysrc/SBFourierSqrt.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBGaussian.cpp` & `GalSim-2.4.9/pysrc/SBGaussian.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBInclinedExponential.cpp` & `GalSim-2.4.9/pysrc/SBInclinedExponential.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBInclinedSersic.cpp` & `GalSim-2.4.9/pysrc/SBInclinedSersic.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBInterpolatedImage.cpp` & `GalSim-2.4.9/pysrc/SBInterpolatedImage.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBKolmogorov.cpp` & `GalSim-2.4.9/pysrc/SBKolmogorov.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBMoffat.cpp` & `GalSim-2.4.9/pysrc/SBMoffat.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBProfile.cpp` & `GalSim-2.4.9/pysrc/SBProfile.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBSecondKick.cpp` & `GalSim-2.4.9/pysrc/SBSecondKick.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBSersic.cpp` & `GalSim-2.4.9/pysrc/SBSersic.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBShapelet.cpp` & `GalSim-2.4.9/pysrc/SBShapelet.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBSpergel.cpp` & `GalSim-2.4.9/pysrc/SBSpergel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBTransform.cpp` & `GalSim-2.4.9/pysrc/SBTransform.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/SBVonKarman.cpp` & `GalSim-2.4.9/pysrc/SBVonKarman.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/Silicon.cpp` & `GalSim-2.4.9/pysrc/Silicon.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/Table.cpp` & `GalSim-2.4.9/pysrc/Table.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/WCS.cpp` & `GalSim-2.4.9/pysrc/WCS.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/pysrc/module.cpp` & `GalSim-2.4.9/pysrc/module.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/setup.py` & `GalSim-2.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/SEDs/CWW_E_ext.sed` & `GalSim-2.4.9/share/SEDs/CWW_E_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/SEDs/CWW_E_ext_more.sed` & `GalSim-2.4.9/share/SEDs/CWW_E_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/SEDs/CWW_Im_ext.sed` & `GalSim-2.4.9/share/SEDs/CWW_Im_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/SEDs/CWW_Im_ext_more.sed` & `GalSim-2.4.9/share/SEDs/CWW_Im_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/SEDs/CWW_Sbc_ext.sed` & `GalSim-2.4.9/share/SEDs/CWW_Sbc_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/SEDs/CWW_Sbc_ext_more.sed` & `GalSim-2.4.9/share/SEDs/CWW_Sbc_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/SEDs/CWW_Scd_ext.sed` & `GalSim-2.4.9/share/SEDs/CWW_Scd_ext.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/SEDs/CWW_Scd_ext_more.sed` & `GalSim-2.4.9/share/SEDs/CWW_Scd_ext_more.sed`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/SEDs/vega.txt` & `GalSim-2.4.9/share/SEDs/vega.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/acs_I_unrot_sci_20_cf.fits` & `GalSim-2.4.9/share/acs_I_unrot_sci_20_cf.fits`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/ACS_wfc_F435W.dat` & `GalSim-2.4.9/share/bandpasses/ACS_wfc_F435W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/ACS_wfc_F606W.dat` & `GalSim-2.4.9/share/bandpasses/ACS_wfc_F606W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/ACS_wfc_F775W.dat` & `GalSim-2.4.9/share/bandpasses/ACS_wfc_F775W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/ACS_wfc_F814W.dat` & `GalSim-2.4.9/share/bandpasses/ACS_wfc_F814W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/ACS_wfc_F850LP.dat` & `GalSim-2.4.9/share/bandpasses/ACS_wfc_F850LP.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/LSST_g.dat` & `GalSim-2.4.9/share/bandpasses/LSST_g.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/LSST_i.dat` & `GalSim-2.4.9/share/bandpasses/LSST_i.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/LSST_r.dat` & `GalSim-2.4.9/share/bandpasses/LSST_r.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/LSST_u.dat` & `GalSim-2.4.9/share/bandpasses/LSST_u.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/LSST_y.dat` & `GalSim-2.4.9/share/bandpasses/LSST_y.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/LSST_z.dat` & `GalSim-2.4.9/share/bandpasses/LSST_z.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/WFC3_ir_F105W.dat` & `GalSim-2.4.9/share/bandpasses/WFC3_ir_F105W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/WFC3_ir_F125W.dat` & `GalSim-2.4.9/share/bandpasses/WFC3_ir_F125W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/WFC3_ir_F160W.dat` & `GalSim-2.4.9/share/bandpasses/WFC3_ir_F160W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/WFC3_uvis_F275W.dat` & `GalSim-2.4.9/share/bandpasses/WFC3_uvis_F275W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/bandpasses/WFC3_uvis_F336W.dat` & `GalSim-2.4.9/share/bandpasses/WFC3_uvis_F336W.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_01.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_01.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_02.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_02.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_03.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_03.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_04.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_04.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_05.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_05.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_06.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_06.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_07.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_07.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_08.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_08.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_09.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_09.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_10.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_10.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_11.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_11.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_12.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_12.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_13.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_13.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_14.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_14.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_15.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_15.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_16.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_16.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_17.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_17.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_18.txt` & `GalSim-2.4.9/share/roman/Roman_Phase-A_SRR_WFC_Zernike_and_Field_Data_170727_18.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz` & `GalSim-2.4.9/share/roman/Roman_SRR_WFC_Pupil_Mask_Longwave_2048_reformatted.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz` & `GalSim-2.4.9/share/roman/Roman_SRR_WFC_Pupil_Mask_Shortwave_2048_reformatted.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA10_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA10_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA10_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA10_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA11_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA11_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA11_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA11_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA12_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA12_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA12_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA12_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA13_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA13_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA13_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA13_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA14_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA14_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA14_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA14_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA15_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA15_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA15_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA15_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA16_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA16_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA16_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA16_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA17_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA17_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA17_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA17_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA18_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA18_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA18_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA18_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA1_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA1_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA1_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA1_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA2_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA2_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA2_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA2_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA3_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA3_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA3_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA3_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA4_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA4_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA4_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA4_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA5_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA5_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA5_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA5_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA6_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA6_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA6_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA6_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA7_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA7_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA7_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA7_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA8_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA8_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA8_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA8_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA9_full_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA9_full_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/SCA9_rim_mask.fits.gz` & `GalSim-2.4.9/share/roman/SCA9_rim_mask.fits.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/afta_throughput.txt` & `GalSim-2.4.9/share/roman/afta_throughput.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/roman_sky_backgrounds.txt` & `GalSim-2.4.9/share/roman/roman_sky_backgrounds.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/sca_positions_7_6_8.txt` & `GalSim-2.4.9/share/roman/sca_positions_7_6_8.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/roman/sip_7_6_8.txt` & `GalSim-2.4.9/share/roman/sip_7_6_8.txt`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/abs_length.dat` & `GalSim-2.4.9/share/sensors/abs_length.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_e2v_32.cfg` & `GalSim-2.4.9/share/sensors/lsst_e2v_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_e2v_32.dat` & `GalSim-2.4.9/share/sensors/lsst_e2v_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_e2v_50_32.cfg` & `GalSim-2.4.9/share/sensors/lsst_e2v_50_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_e2v_50_32.dat` & `GalSim-2.4.9/share/sensors/lsst_e2v_50_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_e2v_50_8.cfg` & `GalSim-2.4.9/share/sensors/lsst_e2v_50_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_e2v_50_8.dat` & `GalSim-2.4.9/share/sensors/lsst_e2v_50_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_e2v_8.cfg` & `GalSim-2.4.9/share/sensors/lsst_e2v_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_e2v_8.dat` & `GalSim-2.4.9/share/sensors/lsst_e2v_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_itl_32.cfg` & `GalSim-2.4.9/share/sensors/lsst_itl_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_itl_32.dat` & `GalSim-2.4.9/share/sensors/lsst_itl_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_itl_50_32.cfg` & `GalSim-2.4.9/share/sensors/lsst_itl_50_32.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_itl_50_32.dat` & `GalSim-2.4.9/share/sensors/lsst_itl_50_32.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_itl_50_8.cfg` & `GalSim-2.4.9/share/sensors/lsst_itl_50_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_itl_50_8.dat` & `GalSim-2.4.9/share/sensors/lsst_itl_50_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_itl_8.cfg` & `GalSim-2.4.9/share/sensors/lsst_itl_8.cfg`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/sensors/lsst_itl_8.dat` & `GalSim-2.4.9/share/sensors/lsst_itl_8.dat`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/share/wfc_F814W.dat.gz` & `GalSim-2.4.9/share/wfc_F814W.dat.gz`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/BinomFact.cpp` & `GalSim-2.4.9/src/BinomFact.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/CDModel.cpp` & `GalSim-2.4.9/src/CDModel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/CorrelatedNoise.cpp` & `GalSim-2.4.9/src/CorrelatedNoise.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/GSParams.cpp` & `GalSim-2.4.9/src/GSParams.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/Image.cpp` & `GalSim-2.4.9/src/Image.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/Image.inst` & `GalSim-2.4.9/src/Image.inst`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/Interpolant.cpp` & `GalSim-2.4.9/src/Interpolant.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/Laguerre.cpp` & `GalSim-2.4.9/src/Laguerre.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/OneDimensionalDeviate.cpp` & `GalSim-2.4.9/src/OneDimensionalDeviate.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/PhotonArray.cpp` & `GalSim-2.4.9/src/PhotonArray.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/Polygon.cpp` & `GalSim-2.4.9/src/Polygon.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/Random.cpp` & `GalSim-2.4.9/src/Random.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/RealGalaxy.cpp` & `GalSim-2.4.9/src/RealGalaxy.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/RealSpaceConvolve.cpp` & `GalSim-2.4.9/src/RealSpaceConvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBAdd.cpp` & `GalSim-2.4.9/src/SBAdd.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBAiry.cpp` & `GalSim-2.4.9/src/SBAiry.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBBox.cpp` & `GalSim-2.4.9/src/SBBox.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBConvolve.cpp` & `GalSim-2.4.9/src/SBConvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBDeconvolve.cpp` & `GalSim-2.4.9/src/SBDeconvolve.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBDeltaFunction.cpp` & `GalSim-2.4.9/src/SBDeltaFunction.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBExponential.cpp` & `GalSim-2.4.9/src/SBExponential.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBFourierSqrt.cpp` & `GalSim-2.4.9/src/SBFourierSqrt.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBGaussian.cpp` & `GalSim-2.4.9/src/SBGaussian.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBInclinedExponential.cpp` & `GalSim-2.4.9/src/SBInclinedExponential.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBInclinedSersic.cpp` & `GalSim-2.4.9/src/SBInclinedSersic.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBInterpolatedImage.cpp` & `GalSim-2.4.9/src/SBInterpolatedImage.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBKolmogorov.cpp` & `GalSim-2.4.9/src/SBKolmogorov.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBMoffat.cpp` & `GalSim-2.4.9/src/SBMoffat.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBProfile.cpp` & `GalSim-2.4.9/src/SBProfile.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBSecondKick.cpp` & `GalSim-2.4.9/src/SBSecondKick.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBSersic.cpp` & `GalSim-2.4.9/src/SBSersic.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBShapelet.cpp` & `GalSim-2.4.9/src/SBShapelet.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBSpergel.cpp` & `GalSim-2.4.9/src/SBSpergel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBTransform.cpp` & `GalSim-2.4.9/src/SBTransform.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/SBVonKarman.cpp` & `GalSim-2.4.9/src/SBVonKarman.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/Silicon.cpp` & `GalSim-2.4.9/src/Silicon.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -592,23 +592,15 @@
                                              double randomNumber) const
     {
         // Determine the distance the photon travels into the silicon
         double si_length;
         if (photons.hasAllocatedWavelengths()) {
             double lambda = photons.getWavelength(i); // in nm
             // Lookup the absorption length in the imported table
-            double abs_length;
-            try {
-                abs_length = _abs_length_table.lookup(lambda); // in microns
-            } catch (std::runtime_error) {
-                if (lambda <= _abs_length_table.argMin())
-                    abs_length = _abs_length_table.lookup(_abs_length_table.argMin());
-                else
-                    abs_length = _abs_length_table.lookup(_abs_length_table.argMax());
-            }
+            double abs_length = _abs_length_table.lookup(lambda); // in microns
             si_length = -abs_length * log(1.0 - randomNumber); // in microns
 #ifdef DEBUGLOGGING
             if (i % 1000 == 0) {
                 xdbg<<"lambda = "<<lambda<<std::endl;
                 xdbg<<"si_length = "<<si_length<<std::endl;
             }
 #endif
```

### Comparing `GalSim-2.4.11/src/Table.cpp` & `GalSim-2.4.9/src/Table.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/Version.cpp` & `GalSim-2.4.9/src/Version.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/WCS.cpp` & `GalSim-2.4.9/src/WCS.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/hsm/PSFCorr.cpp` & `GalSim-2.4.9/src/hsm/PSFCorr.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/Angle.cpp` & `GalSim-2.4.9/src/math/Angle.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/Bessel.cpp` & `GalSim-2.4.9/src/math/Bessel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/BesselI.cpp` & `GalSim-2.4.9/src/math/BesselI.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/BesselJ.cpp` & `GalSim-2.4.9/src/math/BesselJ.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/BesselK.cpp` & `GalSim-2.4.9/src/math/BesselK.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/BesselRoots.cpp` & `GalSim-2.4.9/src/math/BesselRoots.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/BesselY.cpp` & `GalSim-2.4.9/src/math/BesselY.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/Gamma.cpp` & `GalSim-2.4.9/src/math/Gamma.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/Hankel.cpp` & `GalSim-2.4.9/src/math/Hankel.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/Horner.cpp` & `GalSim-2.4.9/src/math/Horner.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/Nan.cpp` & `GalSim-2.4.9/src/math/Nan.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/math/Sinc.cpp` & `GalSim-2.4.9/src/math/Sinc.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/src/mmgr.cpp` & `GalSim-2.4.9/src/mmgr.cpp`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_airy.py` & `GalSim-2.4.9/tests/test_airy.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_bandpass.py` & `GalSim-2.4.9/tests/test_bandpass.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_bessel.py` & `GalSim-2.4.9/tests/test_bessel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_box.py` & `GalSim-2.4.9/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_calc.py` & `GalSim-2.4.9/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_catalog.py` & `GalSim-2.4.9/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_cdmodel.py` & `GalSim-2.4.9/tests/test_cdmodel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_celestial.py` & `GalSim-2.4.9/tests/test_celestial.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_chromatic.py` & `GalSim-2.4.9/tests/test_chromatic.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_config_gsobject.py` & `GalSim-2.4.9/tests/test_config_gsobject.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_config_image.py` & `GalSim-2.4.9/tests/test_config_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -2338,15 +2338,15 @@
     """
     # Use the multirng.yaml config file from the above test as a convenient template source
     config1 = {
         # This copies everything, but we'll override a few things
         "template" : "config_input/multirng.yaml",
 
         # Modules works differently from the others.  Here, we want to concatenate the lists.
-        "modules" : ["astropy.time"],
+        "modules" : ["astropy"],
 
         # Specific fields can be overridden
         "output" : { "file_name" : "test_template.fits" },
 
         # Can override non-top-level fields
         "gal.shear" : { "type" : "E1E2", "e1" : 0.2, "e2" : 0 },
 
@@ -2357,16 +2357,15 @@
         "gal.magnify" : { "type" : "PowerSpectrumMagnification", "num" : 1 },
 
         # Can use specific fields from the template file rather than the whole thing using :
         "gal.ellip" : { "template" : "config_input/multirng.yaml:psf.ellip" },
 
         # Using a zero-length string deletes an item
         "gal.half_light_radius" : "",
-        # Gratuitous use of astropy.time to test submodule inclusions.
-        "gal.scale_radius" : "$astropy.time.Time(1.6, format='jd').to_value('jd')",
+        "gal.scale_radius" : 1.6,
 
         # Check that template items work inside a list.
         "psf" : {
             "type" : "List",
             "items" : [
                 { "template" : "config_input/multirng.yaml:psf" },
                 { "type" : "Gaussian", "sigma" : 0.3 },
@@ -2395,46 +2394,42 @@
 
     assert config['gal']['type'] == 'Exponential'
     assert config['gal']['flux'] == 100
     assert config['gal']['shear'] == { "type" : "E1E2", "e1" : 0.2, "e2" : 0 }
     assert config['gal']['magnify'] == { "type" : "PowerSpectrumMagnification", "num" : 1 }
     assert config['gal']['ellip'] == { "type" : "PowerSpectrumShear", "num" : 0 }
     assert 'half_light_radius' not in config['gal']
-    assert config['gal']['scale_radius'] == "$astropy.time.Time(1.6, format='jd').to_value('jd')"
-
-    # Make sure that parses correctly.
-    sr = galsim.config.ParseValue(config['gal'].copy(), 'scale_radius', config.copy(), float)[0]
-    assert sr == 1.6
+    assert config['gal']['scale_radius'] == 1.6
 
     assert config['psf']['type'] == 'List'
     assert config['psf']['items'][0] == { "type": "Moffat", "beta": 2, "fwhm": 0.9,
                                           "ellip": { "type" : "PowerSpectrumShear", "num" : 0 } }
     assert config['psf']['items'][1] == { "type": "Gaussian", "sigma" : 0.3 }
     assert config['psf']['items'][2] == { "type": "Gaussian", "sigma" : 0.4 }
 
     assert config['input']['power_spectrum'][1]['grid_spacing'] == 2
     assert config['input']['power_spectrum'][0]['grid_spacing'] == 1
     assert config['input']['power_spectrum'][0]['ngrid'] == 50
     assert config['input']['power_spectrum'][0]['variance'] == 0.2
 
-    assert config['modules'] == ['numpy', 'astropy.time']
+    assert config['modules'] == ['numpy', 'astropy']
 
     # Test registering the template.
     galsim.config.RegisterTemplate('multirng', 'config_input/multirng.yaml')
     config3 = config1.copy()
     config3['template'] = 'multirng'
 
     galsim.config.ProcessAllTemplates(config3)
     assert config3 == config
 
     # Make sure template works when registered in a user module
     del galsim.config.process.valid_templates['multirng']
     config4 = config1.copy()
     config4['template'] = 'multirng'
-    config4['modules'] = ['template_register', 'astropy.time']
+    config4['modules'] = ['template_register']
     galsim.config.ImportModules(config4)
     galsim.config.ProcessAllTemplates(config4)
     for field in ['image', 'output', 'gal', 'psf']:
         assert config4[field] == config[field]
 
     # Check a simple Eval string
     config5 = config1.copy()
@@ -2456,37 +2451,14 @@
     with CaptureLog() as cl:
         galsim.config.ProcessAllTemplates(config7, cl.logger)
     assert config7['image']['random_seed'][0]['type'] == 'Eval'
     assert config7['image']['random_seed'][0]['str'] == '123 + (image_num//3) * @image.nobjects'
     print(cl.output)
     assert "Removing item 0 from image.random_seed." in cl.output
 
-    # Read a template config from a file
-    config8 = galsim.config.ReadConfig('config_input/template.yaml')[0]
-    galsim.config.ProcessAllTemplates(config8)
-    for key in config3:
-        print(key)
-        print(config4[key])
-        print(config8[key])
-        assert config8[key] == config4[key]
-    assert config8 == config4
-
-    # Make sure nested templating works
-    config9 = {
-        "template" : "config_input/template.yaml",
-        "gal.ellip.num" : 1,
-        "psf.items.0.beta" : 2.5,
-        "psf.items.2" : { "template" : "multirng:image.noise" },
-    }
-    galsim.config.ProcessAllTemplates(config9)
-    config8['gal']['ellip']['num'] = 1
-    config8['psf']['items'][0]['beta'] = 2.5
-    config8['psf']['items'][2] = config4['image']['noise']
-    assert config9 == config8
-
 
 @timer
 def test_variable_cat_size():
     """Test that some automatic nitems calculations work with variable input catalog sizes
     """
     config = {
         'gal': {
```

### Comparing `GalSim-2.4.11/tests/test_config_input.py` & `GalSim-2.4.9/tests/test_config_input.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_config_noise.py` & `GalSim-2.4.9/tests/test_config_noise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_config_output.py` & `GalSim-2.4.9/tests/test_config_output.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_config_value.py` & `GalSim-2.4.9/tests/test_config_value.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_convolve.py` & `GalSim-2.4.9/tests/test_convolve.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_correlatednoise.py` & `GalSim-2.4.9/tests/test_correlatednoise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_deltafunction.py` & `GalSim-2.4.9/tests/test_deltafunction.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_deprecated.py` & `GalSim-2.4.9/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_des.py` & `GalSim-2.4.9/tests/test_des.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_detectors.py` & `GalSim-2.4.9/tests/test_detectors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_download.py` & `GalSim-2.4.9/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_draw.py` & `GalSim-2.4.9/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_errors.py` & `GalSim-2.4.9/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_exponential.py` & `GalSim-2.4.9/tests/test_exponential.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_fitsheader.py` & `GalSim-2.4.9/tests/test_fitsheader.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_fouriersqrt.py` & `GalSim-2.4.9/tests/test_fouriersqrt.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_galaxy_sample.py` & `GalSim-2.4.9/tests/test_galaxy_sample.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_gaussian.py` & `GalSim-2.4.9/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_hsm.py` & `GalSim-2.4.9/tests/test_hsm.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_image.py` & `GalSim-2.4.9/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_inclined.py` & `GalSim-2.4.9/tests/test_inclined.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_integ.py` & `GalSim-2.4.9/tests/test_integ.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_interpolatedimage.py` & `GalSim-2.4.9/tests/test_interpolatedimage.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_knots.py` & `GalSim-2.4.9/tests/test_knots.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_kolmogorov.py` & `GalSim-2.4.9/tests/test_kolmogorov.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_lensing.py` & `GalSim-2.4.9/tests/test_lensing.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_main.py` & `GalSim-2.4.9/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_metacal.py` & `GalSim-2.4.9/tests/test_metacal.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_moffat.py` & `GalSim-2.4.9/tests/test_moffat.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_noise.py` & `GalSim-2.4.9/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_optics.py` & `GalSim-2.4.9/tests/test_optics.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_phase_psf.py` & `GalSim-2.4.9/tests/test_phase_psf.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_photon_array.py` & `GalSim-2.4.9/tests/test_photon_array.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_pse.py` & `GalSim-2.4.9/tests/test_pse.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_random.py` & `GalSim-2.4.9/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_real.py` & `GalSim-2.4.9/tests/test_real.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_roman.py` & `GalSim-2.4.9/tests/test_roman.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_second_kick.py` & `GalSim-2.4.9/tests/test_second_kick.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_sed.py` & `GalSim-2.4.9/tests/test_sed.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_sensor.py` & `GalSim-2.4.9/tests/test_sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -640,52 +640,14 @@
         # r4 should be greater than r1 with wavelengths and angles turned on.
         sigma_r = 1. / np.sqrt(obj.flux) * im1.scale
         print('check r4 > r1 due to added wavelengths and angles')
         print('r1 = %f, r4 = %f, 2*sigma_r = %f'%(r1,r4,2.*sigma_r))
         assert r4 > r1
 
 @timer
-def test_bad_wavelengths():
-    """If a wavelength is outside the valid range of our tabulated absorption length table,
-    make sure it does something reasonable, rather than abort.
-    """
-    rng = galsim.BaseDeviate(1234)
-
-    nphot = 7
-    x = rng.np.uniform(10,20, size=nphot)
-    y = rng.np.uniform(10,20, size=nphot)
-    flux = np.ones(nphot)
-    dxdz = rng.np.uniform(0,0.5, size=nphot)
-    dydz = rng.np.uniform(0,0.5, size=nphot)
-
-    # The original bug that triggered this test involved photons with wavelength=0.
-    # That's not physically possible, but now this works, using the min or max wavelength
-    # in the lookup table for any photons that are too blue or too red respectively.
-    # Note: the valid range is [255, 1450]
-    wave = [0.0, 55, 255., 800., 1450., 4000., np.inf]
-    photons = galsim.PhotonArray(nphot, x=x, y=y, flux=flux, dxdz=dxdz, dydz=dydz, wavelength=wave)
-
-    image = galsim.Image(32,32)
-    sensor = galsim.SiliconSensor(name='lsst_itl_50_8', rng=rng)
-    sensor.accumulate(photons, image)
-
-    # The real test is just that that didn't throw an exception.
-    # But check that all the photons were put somewhere.
-    assert np.sum(image.array) == nphot
-
-    # The original code that triggered this was actually putting flux=0 for the bad wavelengths,
-    # so let's do that too.
-    flux = [0, 0, 1, 1, 1, 0, 0]
-    photons = galsim.PhotonArray(nphot, x=x, y=y, flux=flux, dxdz=dxdz, dydz=dydz, wavelength=wave)
-    image.setZero()
-    sensor.accumulate(photons, image)
-    assert np.sum(image.array) == np.sum(flux)
-
-
-@timer
 def test_bf_slopes():
     """Test the brighter-fatter slopes
     with both the B-F effect and diffusion turned on and off.
     """
     from scipy.stats import linregress
 
     simple = galsim.Sensor()
```

### Comparing `GalSim-2.4.11/tests/test_sersic.py` & `GalSim-2.4.9/tests/test_sersic.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_shapelet.py` & `GalSim-2.4.9/tests/test_shapelet.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_shear.py` & `GalSim-2.4.9/tests/test_shear.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_shear_position.py` & `GalSim-2.4.9/tests/test_shear_position.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_spergel.py` & `GalSim-2.4.9/tests/test_spergel.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_sum.py` & `GalSim-2.4.9/tests/test_sum.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_table.py` & `GalSim-2.4.9/tests/test_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         assert tab2 == tab
 
 
 @timer
 def test_table2d():
     """Check LookupTable2D functionality.
     """
-    from scipy.interpolate import RectBivariateSpline
+    from scipy.interpolate import interp2d
 
     def f(x_, y_):
         return np.sin(x_) * np.cos(y_) + x_
 
     x = np.linspace(0.1, 3.3, 25)
     y = np.linspace(0.2, 10.4, 75)
     xx, yy = np.meshgrid(x, y)
@@ -433,16 +433,16 @@
     # Compare different ways of evaluating Table2D
     ref = tab2d(newxx, newyy)
     np.testing.assert_array_almost_equal(ref, tab2d(newx, newy, grid=True))
     np.testing.assert_array_almost_equal(ref, np.array([[tab2d(x0, y0)
                                                          for x0 in newx]
                                                         for y0 in newy]))
 
-    scitab2d = RectBivariateSpline(x, y, z.T, kx=1, ky=1)
-    np.testing.assert_array_almost_equal(ref, scitab2d(newx, newy).T)
+    scitab2d = interp2d(x, y, z)
+    np.testing.assert_array_almost_equal(ref, scitab2d(newx, newy))
 
     # Try using linear GSInterp
     tab2d2 = galsim.LookupTable2D(x, y, z, interpolant=galsim.Linear())
     np.testing.assert_array_almost_equal(tab2d(newxx, newyy), tab2d2(newxx, newyy))
     np.testing.assert_array_almost_equal(tab2d(newxx.T, newyy.T), tab2d2(newxx.T, newyy.T))
 
     # Try again using Nearest()
@@ -462,16 +462,16 @@
     z = f(xx, yy)
     tab2d = galsim.LookupTable2D(x, y, z)
     ref = tab2d(newxx, newyy)
     np.testing.assert_array_almost_equal(ref, tab2d(newx, newy, grid=True))
     np.testing.assert_array_almost_equal(ref, np.array([[tab2d(x0, y0)
                                                          for x0 in newx]
                                                         for y0 in newy]))
-    scitab2d = RectBivariateSpline(x, y, z.T, kx=1, ky=1)
-    np.testing.assert_array_almost_equal(ref, scitab2d(newx, newy).T)
+    scitab2d = interp2d(x, y, z)
+    np.testing.assert_array_almost_equal(ref, scitab2d(newx, newy))
 
     # Using a galsim.Interpolant should raise an exception if x/y are not equal spaced.
     with assert_raises(galsim.GalSimIncompatibleValuesError):
         tab2d2 = galsim.LookupTable2D(x, y, z, interpolant=galsim.Linear())
 
     # Try a simpler interpolation function.  We should be able to interpolate a (bi-)linear function
     # exactly with a linear interpolant.
```

### Comparing `GalSim-2.4.11/tests/test_transforms.py` & `GalSim-2.4.9/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_utilities.py` & `GalSim-2.4.9/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_vonkarman.py` & `GalSim-2.4.9/tests/test_vonkarman.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_wcs.py` & `GalSim-2.4.9/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `GalSim-2.4.11/tests/test_zernike.py` & `GalSim-2.4.9/tests/test_zernike.py`

 * *Files identical despite different names*

