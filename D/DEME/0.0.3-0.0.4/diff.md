# Comparing `tmp/DEME-0.0.3.tar.gz` & `tmp/deme-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DEME-0.0.3.tar", last modified: Sat Aug  5 09:54:40 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `DEME-0.0.3.tar` & `deme-0.0.4.tar`

### file list

```diff
@@ -1,172 +1,427 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.030583 DEME-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     8423 2023-08-05 09:40:20.000000 DEME-0.0.3/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2146 2023-08-05 09:40:13.000000 DEME-0.0.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       77 2023-08-05 09:40:20.000000 DEME-0.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      222 2023-08-05 09:54:40.030583 DEME-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18416 2023-08-05 09:40:20.000000 DEME-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.000583 DEME-0.0.3/cmake/
--rw-r--r--   0 root         (0) root         (0)     2106 2023-08-05 09:40:13.000000 DEME-0.0.3/cmake/CudaSupportedArchitectures.cmake
--rw-r--r--   0 root         (0) root         (0)     1895 2023-08-05 09:40:13.000000 DEME-0.0.3/cmake/CxxStdAutodetect.cmake
--rw-r--r--   0 root         (0) root         (0)     1387 2023-08-05 09:40:13.000000 DEME-0.0.3/cmake/FixNinjaColors.cmake
--rw-r--r--   0 root         (0) root         (0)     1296 2023-08-05 09:54:18.000000 DEME-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 09:54:40.030583 DEME-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5790 2023-08-05 09:54:23.000000 DEME-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:39.997250 DEME-0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.003916 DEME-0.0.3/src/DEM/
--rw-r--r--   0 root         (0) root         (0)    95272 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/API.h
--rw-r--r--   0 root         (0) root         (0)    92397 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/APIPrivate.cpp
--rw-r--r--   0 root         (0) root         (0)    80527 2023-08-05 09:40:20.000000 DEME-0.0.3/src/DEM/APIPublic.cpp
--rw-r--r--   0 root         (0) root         (0)    30242 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/AuxClasses.cpp
--rw-r--r--   0 root         (0) root         (0)    21225 2023-08-05 09:40:20.000000 DEME-0.0.3/src/DEM/AuxClasses.h
--rw-r--r--   0 root         (0) root         (0)    25283 2023-08-05 09:40:20.000000 DEME-0.0.3/src/DEM/BdrsAndObjs.h
--rw-r--r--   0 root         (0) root         (0)     3587 2023-08-05 09:40:20.000000 DEME-0.0.3/src/DEM/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    19426 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/Defines.h
--rw-r--r--   0 root         (0) root         (0)    24526 2023-08-05 09:40:20.000000 DEME-0.0.3/src/DEM/HostSideHelpers.hpp
--rw-r--r--   0 root         (0) root         (0)     6872 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/MeshUtils.cpp
--rw-r--r--   0 root         (0) root         (0)    17359 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/Models.h
--rw-r--r--   0 root         (0) root         (0)    51761 2023-08-05 09:40:20.000000 DEME-0.0.3/src/DEM/PyDEME.cpp
--rw-r--r--   0 root         (0) root         (0)    43207 2023-08-05 09:40:20.000000 DEME-0.0.3/src/DEM/Structs.h
--rw-r--r--   0 root         (0) root         (0)     2863 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/VariableTypes.h
--rw-r--r--   0 root         (0) root         (0)   137869 2023-08-05 09:40:20.000000 DEME-0.0.3/src/DEM/dT.cpp
--rw-r--r--   0 root         (0) root         (0)    35772 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/dT.h
--rw-r--r--   0 root         (0) root         (0)    47036 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/kT.cpp
--rw-r--r--   0 root         (0) root         (0)    19757 2023-08-05 09:40:13.000000 DEME-0.0.3/src/DEM/kT.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.003916 DEME-0.0.3/src/DEM/utils/
--rw-r--r--   0 root         (0) root         (0)    28271 2023-08-05 09:40:20.000000 DEME-0.0.3/src/DEM/utils/Samplers.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.007250 DEME-0.0.3/src/DEME.egg-info/
--rw-r--r--   0 root         (0) root         (0)      222 2023-08-05 09:54:39.000000 DEME-0.0.3/src/DEME.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5358 2023-08-05 09:54:39.000000 DEME-0.0.3/src/DEME.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 09:54:39.000000 DEME-0.0.3/src/DEME.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 09:42:09.000000 DEME-0.0.3/src/DEME.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       26 2023-08-05 09:54:39.000000 DEME-0.0.3/src/DEME.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-08-05 09:54:39.000000 DEME-0.0.3/src/DEME.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.007250 DEME-0.0.3/src/algorithms/
--rw-r--r--   0 root         (0) root         (0)     1736 2023-08-05 09:40:13.000000 DEME-0.0.3/src/algorithms/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7532 2023-08-05 09:40:13.000000 DEME-0.0.3/src/algorithms/DEMCubBasedSubroutines.h
--rw-r--r--   0 root         (0) root         (0)    57300 2023-08-05 09:40:13.000000 DEME-0.0.3/src/algorithms/DEMCubContactDetection.cu
--rw-r--r--   0 root         (0) root         (0)    10015 2023-08-05 09:40:13.000000 DEME-0.0.3/src/algorithms/DEMCubForceCollection.cu
--rw-r--r--   0 root         (0) root         (0)     8469 2023-08-05 09:40:13.000000 DEME-0.0.3/src/algorithms/DEMCubUtilities.cu
--rw-r--r--   0 root         (0) root         (0)     8277 2023-08-05 09:40:13.000000 DEME-0.0.3/src/algorithms/DEMCubWrappers.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.007250 DEME-0.0.3/src/core/
--rw-r--r--   0 root         (0) root         (0)     1163 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/ApiVersion.h.in
--rw-r--r--   0 root         (0) root         (0)     5071 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      544 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/DebugInfo.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.010583 DEME-0.0.3/src/core/utils/
--rw-r--r--   0 root         (0) root         (0)      996 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/DEMEPaths.cpp
--rw-r--r--   0 root         (0) root         (0)     1165 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/DEMEPaths.h
--rw-r--r--   0 root         (0) root         (0)     2878 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/GpuError.h
--rw-r--r--   0 root         (0) root         (0)     3887 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/GpuManager.cpp
--rw-r--r--   0 root         (0) root         (0)     1231 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/GpuManager.h
--rw-r--r--   0 root         (0) root         (0)      574 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/HeaderGenerator.h
--rw-r--r--   0 root         (0) root         (0)     2019 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/JitHelper.cpp
--rw-r--r--   0 root         (0) root         (0)     1748 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/JitHelper.h
--rw-r--r--   0 root         (0) root         (0)     3751 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/ManagedAllocator.hpp
--rw-r--r--   0 root         (0) root         (0)     3042 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/ManagedMemory.hpp
--rw-r--r--   0 root         (0) root         (0)      684 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/RuntimeData.cpp.in
--rw-r--r--   0 root         (0) root         (0)      360 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/RuntimeData.h
--rw-r--r--   0 root         (0) root         (0)     4065 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/ThreadManager.h
--rw-r--r--   0 root         (0) root         (0)     4611 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/Timer.hpp
--rw-r--r--   0 root         (0) root         (0)    21024 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/WavefrontMeshLoader.hpp
--rw-r--r--   0 root         (0) root         (0)    37737 2023-08-05 09:40:13.000000 DEME-0.0.3/src/core/utils/csv.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.017250 DEME-0.0.3/src/demo/
--rw-r--r--   0 root         (0) root         (0)     1578 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6473 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_BallDrop.cpp
--rw-r--r--   0 root         (0) root         (0)     9439 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_Centrifuge.cpp
--rw-r--r--   0 root         (0) root         (0)    13128 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_ConePenetration.cpp
--rw-r--r--   0 root         (0) root         (0)    20858 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_Electrostatic.cpp
--rw-r--r--   0 root         (0) root         (0)    15820 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_FlexibleMesh.cpp
--rw-r--r--   0 root         (0) root         (0)     8988 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_GRCPrep_Part1.cpp
--rw-r--r--   0 root         (0) root         (0)    13239 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_GRCPrep_Part2.cpp
--rw-r--r--   0 root         (0) root         (0)     6226 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_GameOfLife.cpp
--rw-r--r--   0 root         (0) root         (0)    11650 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_Indentation.cpp
--rw-r--r--   0 root         (0) root         (0)     6839 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_Mixer.cpp
--rw-r--r--   0 root         (0) root         (0)     7193 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_Repose.cpp
--rw-r--r--   0 root         (0) root         (0)     9600 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_RotatingDrum.cpp
--rw-r--r--   0 root         (0) root         (0)     7814 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_Shake.cpp
--rw-r--r--   0 root         (0) root         (0)     7715 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_Sieve.cpp
--rw-r--r--   0 root         (0) root         (0)     7667 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_SingleSphereCollide.cpp
--rw-r--r--   0 root         (0) root         (0)    10223 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_SolarSystem.cpp
--rw-r--r--   0 root         (0) root         (0)    13106 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_TestPack.cpp
--rw-r--r--   0 root         (0) root         (0)    15352 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_WheelDP.cpp
--rw-r--r--   0 root         (0) root         (0)    10608 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_WheelDPSimplified.cpp
--rw-r--r--   0 root         (0) root         (0)    15253 2023-08-05 09:40:13.000000 DEME-0.0.3/src/demo/DEMdemo_WheelSlopeSlip.cpp
--rw-r--r--   0 root         (0) root         (0)     5200 2023-08-05 09:40:20.000000 DEME-0.0.3/src/demo/pyDEME_BallDrop.py
--rw-r--r--   0 root         (0) root         (0)     7645 2023-08-05 09:40:20.000000 DEME-0.0.3/src/demo/pyDEME_Centrifuge.py
--rw-r--r--   0 root         (0) root         (0)    11311 2023-08-05 09:40:20.000000 DEME-0.0.3/src/demo/pyDEME_ConePenetration.py
--rw-r--r--   0 root         (0) root         (0)    19110 2023-08-05 09:40:20.000000 DEME-0.0.3/src/demo/pyDEME_Electrostatic.py
--rw-r--r--   0 root         (0) root         (0)    13738 2023-08-05 09:40:20.000000 DEME-0.0.3/src/demo/pyDEME_FlexibleMesh.py
--rw-r--r--   0 root         (0) root         (0)     6873 2023-08-05 09:40:20.000000 DEME-0.0.3/src/demo/pyDEME_GRCPrep_Part1.py
--rw-r--r--   0 root         (0) root         (0)     4997 2023-08-05 09:40:20.000000 DEME-0.0.3/src/demo/pyDEME_GameOfLife.py
--rw-r--r--   0 root         (0) root         (0)     8863 2023-08-05 09:40:20.000000 DEME-0.0.3/src/demo/pyDEME_WheelDPSimplified.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.020583 DEME-0.0.3/src/kernel/
--rw-r--r--   0 root         (0) root         (0)    10054 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/CUDAMathHelpers.cu
--rw-r--r--   0 root         (0) root         (0)    16691 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMBinSphereKernels.cu
--rw-r--r--   0 root         (0) root         (0)    12594 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMBinTriangleKernels.cu
--rw-r--r--   0 root         (0) root         (0)    13935 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCalcForceKernels.cu
--rw-r--r--   0 root         (0) root         (0)     5733 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCollectForceKernels.cu
--rw-r--r--   0 root         (0) root         (0)     4525 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCollectForceKernels_Compact.cu
--rw-r--r--   0 root         (0) root         (0)     8794 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCollisionKernels.cu
--rw-r--r--   0 root         (0) root         (0)    25399 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMContactKernels_SphereSphere.cu
--rw-r--r--   0 root         (0) root         (0)    26515 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMContactKernels_SphereTriangle.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.023916 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/
--rw-r--r--   0 root         (0) root         (0)      884 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/AnalyticalCompDefJitify.cu
--rw-r--r--   0 root         (0) root         (0)      187 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/ClumpCompAcqStratAllFlatten.cu
--rw-r--r--   0 root         (0) root         (0)      232 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/ClumpCompAcqStratAllJitify.cu
--rw-r--r--   0 root         (0) root         (0)      698 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/ClumpCompAcqStratPartialJitify.cu
--rw-r--r--   0 root         (0) root         (0)      286 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/ClumpCompDefJitify.cu
--rw-r--r--   0 root         (0) root         (0)      226 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/ContactInfoWriteBack.cu
--rw-r--r--   0 root         (0) root         (0)     1605 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/ForceInKernelReductionStrat.cu
--rw-r--r--   0 root         (0) root         (0)     1735 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/FrictionlessHertzianForceModel.cu
--rw-r--r--   0 root         (0) root         (0)     5275 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/FullHertzianForceModel.cu
--rw-r--r--   0 root         (0) root         (0)       77 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/IntegrationVelPassOnCenteredDiff.cu
--rw-r--r--   0 root         (0) root         (0)       91 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/IntegrationVelPassOnExtendedTaylor.cu
--rw-r--r--   0 root         (0) root         (0)       58 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/IntegrationVelPassOnForwardEuler.cu
--rw-r--r--   0 root         (0) root         (0)      107 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/MOIAcqStratFlatten.cu
--rw-r--r--   0 root         (0) root         (0)      164 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/MOIAcqStratJitify.cu
--rw-r--r--   0 root         (0) root         (0)      202 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/MOIDefJitify.cu
--rw-r--r--   0 root         (0) root         (0)       42 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/MassAcqStratFlatten.cu
--rw-r--r--   0 root         (0) root         (0)       63 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/MassAcqStratJitify.cu
--rw-r--r--   0 root         (0) root         (0)      122 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMCustomizablePolicies/MassDefJitify.cu
--rw-r--r--   0 root         (0) root         (0)    24775 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMHelperKernels.cu
--rw-r--r--   0 root         (0) root         (0)     4383 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMHistoryMappingKernels.cu
--rw-r--r--   0 root         (0) root         (0)    11129 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMIntegrationKernels.cu
--rw-r--r--   0 root         (0) root         (0)     3315 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMMiscKernels.cu
--rw-r--r--   0 root         (0) root         (0)     1633 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMModeratorKernels.cu
--rw-r--r--   0 root         (0) root         (0)     2398 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMOwnerQueryKernels.cu
--rw-r--r--   0 root         (0) root         (0)     3126 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMPrepForceKernels.cu
--rw-r--r--   0 root         (0) root         (0)     2295 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMSphereQueryKernels.cu
--rw-r--r--   0 root         (0) root         (0)    19116 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMTriangleBoxIntersect.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/src/kernel/DEMUserScripts/
--rw-r--r--   0 root         (0) root         (0)     5995 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMUserScripts/ForceModelWithCohesion.cu
--rw-r--r--   0 root         (0) root         (0)     8061 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMUserScripts/ForceModelWithElectrostatic.cu
--rw-r--r--   0 root         (0) root         (0)     2988 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/DEMUserScripts/ForceModelWithGravity.cu
--rw-r--r--   0 root         (0) root         (0)      113 2023-08-05 09:40:13.000000 DEME-0.0.3/src/kernel/hello.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:39.997250 DEME-0.0.3/thirdparty/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/
--rw-r--r--   0 root         (0) root         (0)    11983 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/tests/
--rw-r--r--   0 root         (0) root         (0)    21675 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/
--rw-r--r--   0 root         (0) root         (0)     2639 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 root         (0) root         (0)     1171 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 root         (0) root         (0)     1293 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 root         (0) root         (0)     1685 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 root         (0) root         (0)     1353 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 root         (0) root         (0)     1163 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 root         (0) root         (0)     1368 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.027250 DEME-0.0.3/thirdparty/pybind11/tests/test_embed/
--rw-r--r--   0 root         (0) root         (0)     1798 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:54:40.030583 DEME-0.0.3/thirdparty/pybind11/tools/
--rw-r--r--   0 root         (0) root         (0)     2350 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 root         (0) root         (0)     3105 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 root         (0) root         (0)    11190 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 root         (0) root         (0)      817 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 root         (0) root         (0)    14033 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 root         (0) root         (0)     8960 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 root         (0) root         (0)     8361 2023-08-05 09:54:03.000000 DEME-0.0.3/thirdparty/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 deme-0.0.4/.clang-format
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deme-0.0.4/.gitmodules
+-rw-r--r--   0        0        0     8423 2020-02-02 00:00:00.000000 deme-0.0.4/CMakeLists.txt
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 deme-0.0.4/CONTRIBUTORS.md
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 deme-0.0.4/MANIFEST.in
+-rw-r--r--   0        0        0    18416 2020-02-02 00:00:00.000000 deme-0.0.4/README.md
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 deme-0.0.4/DEME.egg-info/PKG-INFO
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 deme-0.0.4/DEME.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 deme-0.0.4/DEME.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 deme-0.0.4/DEME.egg-info/not-zip-safe
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 deme-0.0.4/DEME.egg-info/requires.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 deme-0.0.4/DEME.egg-info/top_level.txt
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 deme-0.0.4/PyDEME.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 deme-0.0.4/PyDEME.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 deme-0.0.4/PyDEME.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 deme-0.0.4/PyDEME.egg-info/not-zip-safe
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 deme-0.0.4/PyDEME.egg-info/requires.txt
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 deme-0.0.4/PyDEME.egg-info/top_level.txt
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 deme-0.0.4/cmake/CudaSupportedArchitectures.cmake
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 deme-0.0.4/cmake/CxxStdAutodetect.cmake
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 deme-0.0.4/cmake/DEMEConfig.cmake.in
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 deme-0.0.4/cmake/FixNinjaColors.cmake
+-rw-r--r--   0        0        0   461903 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/GPBR_Vessel_Fine.obj
+-rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/cone.obj
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/cube.obj
+-rw-r--r--   0        0        0    71306 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/cyl_r1_h2.obj
+-rw-r--r--   0        0        0    51398 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/funnel.obj
+-rw-r--r--   0        0        0    77565 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/hourglass.obj
+-rw-r--r--   0        0        0   123678 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/internal_mixer.obj
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/plane_20by20.obj
+-rw-r--r--   0        0        0    91981 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/silo.obj
+-rw-r--r--   0        0        0    21519 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/sphere.obj
+-rw-r--r--   0        0        0    56565 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/thin_plate.obj
+-rw-r--r--   0        0        0  9609852 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/rover_wheels/curiosity_wheel.obj
+-rw-r--r--   0        0        0  5442018 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/rover_wheels/curiosity_wheel_surface.obj
+-rw-r--r--   0        0        0  8660145 2020-02-02 00:00:00.000000 deme-0.0.4/data/mesh/rover_wheels/viper_wheel_right.obj
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 deme-0.0.4/recipe/meta.yaml
+-rw-r--r--   0        0        0    95272 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/API.h
+-rw-r--r--   0        0        0    92397 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/APIPrivate.cpp
+-rw-r--r--   0        0        0    80527 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/APIPublic.cpp
+-rw-r--r--   0        0        0    30242 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/AuxClasses.cpp
+-rw-r--r--   0        0        0    21225 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/AuxClasses.h
+-rw-r--r--   0        0        0    25283 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/BdrsAndObjs.h
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/CMakeLists.txt
+-rw-r--r--   0        0        0    19426 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/Defines.h
+-rw-r--r--   0        0        0    24526 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/HostSideHelpers.hpp
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/MeshUtils.cpp
+-rw-r--r--   0        0        0    17359 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/Models.h
+-rw-r--r--   0        0        0    51761 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/PyDEME.cpp
+-rw-r--r--   0        0        0    43207 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/Structs.h
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/VariableTypes.h
+-rw-r--r--   0        0        0   137869 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/dT.cpp
+-rw-r--r--   0        0        0    35772 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/dT.h
+-rw-r--r--   0        0        0    47036 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/kT.cpp
+-rw-r--r--   0        0        0    19757 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/kT.h
+-rw-r--r--   0        0        0    28271 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEM/utils/Samplers.hpp
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEME.egg-info/PKG-INFO
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEME.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEME.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEME.egg-info/not-zip-safe
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEME.egg-info/requires.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 deme-0.0.4/src/DEME.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 deme-0.0.4/src/algorithms/CMakeLists.txt
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 deme-0.0.4/src/algorithms/DEMCubBasedSubroutines.h
+-rw-r--r--   0        0        0    57300 2020-02-02 00:00:00.000000 deme-0.0.4/src/algorithms/DEMCubContactDetection.cu
+-rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 deme-0.0.4/src/algorithms/DEMCubForceCollection.cu
+-rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 deme-0.0.4/src/algorithms/DEMCubUtilities.cu
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 deme-0.0.4/src/algorithms/DEMCubWrappers.cu
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/ApiVersion.h.in
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/CMakeLists.txt
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/DebugInfo.cpp
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/DEMEPaths.cpp
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/DEMEPaths.h
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/GpuError.h
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/GpuManager.cpp
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/GpuManager.h
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/HeaderGenerator.h
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/JitHelper.cpp
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/JitHelper.h
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/ManagedAllocator.hpp
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/ManagedMemory.hpp
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/RuntimeData.cpp.in
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/RuntimeData.h
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/ThreadManager.h
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/Timer.hpp
+-rw-r--r--   0        0        0    21024 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/WavefrontMeshLoader.hpp
+-rw-r--r--   0        0        0    37737 2020-02-02 00:00:00.000000 deme-0.0.4/src/core/utils/csv.hpp
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/CMakeLists.txt
+-rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_BallDrop.cpp
+-rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_Centrifuge.cpp
+-rw-r--r--   0        0        0    13128 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_ConePenetration.cpp
+-rw-r--r--   0        0        0    20858 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_Electrostatic.cpp
+-rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_FlexibleMesh.cpp
+-rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_GRCPrep_Part1.cpp
+-rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_GRCPrep_Part2.cpp
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_GameOfLife.cpp
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_Indentation.cpp
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_Mixer.cpp
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_Repose.cpp
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_RotatingDrum.cpp
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_Shake.cpp
+-rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_Sieve.cpp
+-rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_SingleSphereCollide.cpp
+-rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_SolarSystem.cpp
+-rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_TestPack.cpp
+-rw-r--r--   0        0        0    15352 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_WheelDP.cpp
+-rw-r--r--   0        0        0    10608 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_WheelDPSimplified.cpp
+-rw-r--r--   0        0        0    15253 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/DEMdemo_WheelSlopeSlip.cpp
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/pyDEME_BallDrop.py
+-rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/pyDEME_Centrifuge.py
+-rw-r--r--   0        0        0    11311 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/pyDEME_ConePenetration.py
+-rw-r--r--   0        0        0    19110 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/pyDEME_Electrostatic.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/pyDEME_FlexibleMesh.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/pyDEME_GRCPrep_Part1.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/pyDEME_GameOfLife.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 deme-0.0.4/src/demo/pyDEME_WheelDPSimplified.py
+-rw-r--r--   0        0        0    10054 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/CUDAMathHelpers.cu
+-rw-r--r--   0        0        0    16691 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMBinSphereKernels.cu
+-rw-r--r--   0        0        0    12594 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMBinTriangleKernels.cu
+-rw-r--r--   0        0        0    13935 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCalcForceKernels.cu
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCollectForceKernels.cu
+-rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCollectForceKernels_Compact.cu
+-rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCollisionKernels.cu
+-rw-r--r--   0        0        0    25399 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMContactKernels_SphereSphere.cu
+-rw-r--r--   0        0        0    26515 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMContactKernels_SphereTriangle.cu
+-rw-r--r--   0        0        0    24775 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMHelperKernels.cu
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMHistoryMappingKernels.cu
+-rw-r--r--   0        0        0    11129 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMIntegrationKernels.cu
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMMiscKernels.cu
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMModeratorKernels.cu
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMOwnerQueryKernels.cu
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMPrepForceKernels.cu
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMSphereQueryKernels.cu
+-rw-r--r--   0        0        0    19116 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMTriangleBoxIntersect.cu
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/hello.cu
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/AnalyticalCompDefJitify.cu
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/ClumpCompAcqStratAllFlatten.cu
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/ClumpCompAcqStratAllJitify.cu
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/ClumpCompAcqStratPartialJitify.cu
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/ClumpCompDefJitify.cu
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/ContactInfoWriteBack.cu
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/ForceInKernelReductionStrat.cu
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/FrictionlessHertzianForceModel.cu
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/FullHertzianForceModel.cu
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/IntegrationVelPassOnCenteredDiff.cu
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/IntegrationVelPassOnExtendedTaylor.cu
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/IntegrationVelPassOnForwardEuler.cu
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/MOIAcqStratFlatten.cu
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/MOIAcqStratJitify.cu
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/MOIDefJitify.cu
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/MassAcqStratFlatten.cu
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/MassAcqStratJitify.cu
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMCustomizablePolicies/MassDefJitify.cu
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMUserScripts/ForceModelWithCohesion.cu
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMUserScripts/ForceModelWithElectrostatic.cu
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 deme-0.0.4/src/kernel/DEMUserScripts/ForceModelWithGravity.cu
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/.clang-format
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/.git
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/.gitignore
+-rw-r--r--   0        0        0   106196 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/Doxyfile
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/LICENSE
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/Makefile
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/README.md
+-rw-r--r--   0        0        0   166214 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/jitify.hpp
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/jitify_example.cpp
+-rw-r--r--   0        0        0    43886 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/jitify_test.cu
+-rw-r--r--   0        0        0    21615 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/nvrtc_cli.cpp
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/nvrtc_cli_test.sh
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/stringify.cpp
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/example_headers/class_arg_kernel.cuh
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/example_headers/constant_header.cuh
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/example_headers/my_header1.cuh
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/example_headers/my_header2.cuh
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/jitify/example_headers/my_header3.cuh
+-rw-r--r--   0        0        0    40591 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/nvidia_helper_math/nvmath/helper_math.cuh
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.appveyor.yml
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.clang-format
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.clang-tidy
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.cmake-format.yaml
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.codespell-ignore-lines
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.git
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.gitattributes
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.gitignore
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.readthedocs.yml
+-rw-r--r--   0        0        0    11983 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/LICENSE
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/MANIFEST.in
+-rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/README.rst
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/noxfile.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/pyproject.toml
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/setup.cfg
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/setup.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/CODEOWNERS
+-rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/dependabot.yml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/labeler.yml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/labeler_merged.yml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/pull_request_template.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0        0        0    32023 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/workflows/format.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/Doxyfile
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/Makefile
+-rw-r--r--   0        0        0     9240 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/basics.rst
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/benchmark.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/benchmark.rst
+-rw-r--r--   0        0        0   115476 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/changelog.rst
+-rw-r--r--   0        0        0    16380 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/classes.rst
+-rw-r--r--   0        0        0    25777 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/compiling.rst
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/conf.py
+-rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/faq.rst
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/index.rst
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/installing.rst
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/limitations.rst
+-rw-r--r--   0        0        0    61034 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0        0        0    44653 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0        0        0    87708 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0        0        0    41121 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0        0        0    85853 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/reference.rst
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/release.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/requirements.txt
+-rw-r--r--   0        0        0    23489 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/upgrade.rst
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    47796 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0        0        0    26729 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/misc.rst
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0        0        0    12371 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0        0        0    17161 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/docs/cmake/index.rst
+-rw-r--r--   0        0        0    23959 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/attr.h
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0        0        0    65660 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/cast.h
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/common.h
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/complex.h
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/embed.h
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/eval.h
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/functional.h
+-rw-r--r--   0        0        0     8262 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/gil.h
+-rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0        0        0    79416 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0        0        0     9103 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/operators.h
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/options.h
+-rw-r--r--   0        0        0   126420 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0        0        0    94641 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/stl.h
+-rw-r--r--   0        0        0    29747 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0        0        0    28518 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0        0        0    52930 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0        0        0    26305 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0        0        0    42613 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0        0        0    31450 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0        0        0    18140 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/pybind11/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/pybind11/__main__.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/pybind11/_version.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/pybind11/commands.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/pybind11/py.typed
+-rw-r--r--   0        0        0    17650 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0        0        0    21675 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/conftest.py
+-rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/constructor_stats.h
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/env.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/local_bindings.h
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/object.h
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/pytest.ini
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/requirements.txt
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_async.cpp
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_async.py
+-rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_buffers.py
+-rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0        0        0    17245 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_call_policies.py
+-rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_callbacks.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_chrono.py
+-rw-r--r--   0        0        0    24874 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_class.cpp
+-rw-r--r--   0        0        0    14814 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_class.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_const_name.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_copy_move.py
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0        0        0    19350 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0        0        0    28867 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0        0        0    10590 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_eigen_tensor.py
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_enum.cpp
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_enum.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_eval.cpp
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_eval.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_eval_call.py
+-rw-r--r--   0        0        0    11904 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_exceptions.h
+-rw-r--r--   0        0        0    12774 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_exceptions.py
+-rw-r--r--   0        0        0    18155 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_iostream.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0        0        0    13757 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0        0        0    21388 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0        0        0    18134 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_modules.cpp
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_modules.py
+-rw-r--r--   0        0        0    12305 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0        0        0    11874 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0        0        0    19861 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0        0        0    20356 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0        0        0    21114 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_pickling.py
+-rw-r--r--   0        0        0    30750 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0        0        0    23630 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_pytypes.py
+-rw-r--r--   0        0        0    21153 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0        0        0    18898 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0        0        0    21587 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_stl.cpp
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_stl.py
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_thread.cpp
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_thread.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_union.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_union.py
+-rw-r--r--   0        0        0    22991 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/valgrind-python.supp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/extra_python_package/test_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/embed.cpp
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/main.cpp
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0        0        0    16535 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0        0        0    11190 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/check-style.sh
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/libsize.py
+-rwxr-xr-x   0        0        0     1311 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/make_changelog.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0        0        0    14033 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/pyproject.toml
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/setup_global.py.in
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 deme-0.0.4/thirdparty/pybind11/tools/setup_main.py.in
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 deme-0.0.4/.gitignore
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 deme-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 deme-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 deme-0.0.4/PKG-INFO
```

### Comparing `DEME-0.0.3/CMakeLists.txt` & `deme-0.0.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/LICENSE.md` & `deme-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/README.md` & `deme-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/cmake/CudaSupportedArchitectures.cmake` & `deme-0.0.4/cmake/CudaSupportedArchitectures.cmake`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/cmake/CxxStdAutodetect.cmake` & `deme-0.0.4/cmake/CxxStdAutodetect.cmake`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/cmake/FixNinjaColors.cmake` & `deme-0.0.4/cmake/FixNinjaColors.cmake`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/pyproject.toml` & `deme-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 [build-system]
-requires = [
-    "setuptools>=61.0",
-    "wheel",
-    "ninja",
-    "cmake>=3.18",
-]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend= "hatchling.build"
 
 [project]
 name = "DEME"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 requires-python=">=3.8"
 
 [tool.mypy]
```

### Comparing `DEME-0.0.3/src/DEM/API.h` & `deme-0.0.4/src/DEM/API.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/APIPrivate.cpp` & `deme-0.0.4/src/DEM/APIPrivate.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/APIPublic.cpp` & `deme-0.0.4/src/DEM/APIPublic.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/AuxClasses.cpp` & `deme-0.0.4/src/DEM/AuxClasses.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/AuxClasses.h` & `deme-0.0.4/src/DEM/AuxClasses.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/BdrsAndObjs.h` & `deme-0.0.4/src/DEM/BdrsAndObjs.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/CMakeLists.txt` & `deme-0.0.4/src/DEM/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/Defines.h` & `deme-0.0.4/src/DEM/Defines.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/HostSideHelpers.hpp` & `deme-0.0.4/src/DEM/HostSideHelpers.hpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/MeshUtils.cpp` & `deme-0.0.4/src/DEM/MeshUtils.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/Models.h` & `deme-0.0.4/src/DEM/Models.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/PyDEME.cpp` & `deme-0.0.4/src/DEM/PyDEME.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/Structs.h` & `deme-0.0.4/src/DEM/Structs.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/VariableTypes.h` & `deme-0.0.4/src/DEM/VariableTypes.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/dT.cpp` & `deme-0.0.4/src/DEM/dT.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/dT.h` & `deme-0.0.4/src/DEM/dT.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/kT.cpp` & `deme-0.0.4/src/DEM/kT.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/kT.h` & `deme-0.0.4/src/DEM/kT.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEM/utils/Samplers.hpp` & `deme-0.0.4/src/DEM/utils/Samplers.hpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/DEME.egg-info/SOURCES.txt` & `deme-0.0.4/src/DEME.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/algorithms/CMakeLists.txt` & `deme-0.0.4/src/algorithms/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/algorithms/DEMCubBasedSubroutines.h` & `deme-0.0.4/src/algorithms/DEMCubBasedSubroutines.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/algorithms/DEMCubContactDetection.cu` & `deme-0.0.4/src/algorithms/DEMCubContactDetection.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/algorithms/DEMCubForceCollection.cu` & `deme-0.0.4/src/algorithms/DEMCubForceCollection.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/algorithms/DEMCubUtilities.cu` & `deme-0.0.4/src/algorithms/DEMCubUtilities.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/algorithms/DEMCubWrappers.cu` & `deme-0.0.4/src/algorithms/DEMCubWrappers.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/ApiVersion.h.in` & `deme-0.0.4/src/core/ApiVersion.h.in`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/CMakeLists.txt` & `deme-0.0.4/src/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/DebugInfo.cpp` & `deme-0.0.4/src/core/DebugInfo.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/DEMEPaths.cpp` & `deme-0.0.4/src/core/utils/DEMEPaths.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/DEMEPaths.h` & `deme-0.0.4/src/core/utils/DEMEPaths.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/GpuError.h` & `deme-0.0.4/src/core/utils/GpuError.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/GpuManager.cpp` & `deme-0.0.4/src/core/utils/GpuManager.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/GpuManager.h` & `deme-0.0.4/src/core/utils/GpuManager.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/HeaderGenerator.h` & `deme-0.0.4/src/core/utils/HeaderGenerator.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/JitHelper.cpp` & `deme-0.0.4/src/core/utils/JitHelper.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/JitHelper.h` & `deme-0.0.4/src/core/utils/JitHelper.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/ManagedAllocator.hpp` & `deme-0.0.4/src/core/utils/ManagedAllocator.hpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/ManagedMemory.hpp` & `deme-0.0.4/src/core/utils/ManagedMemory.hpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/RuntimeData.cpp.in` & `deme-0.0.4/src/core/utils/RuntimeData.cpp.in`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/ThreadManager.h` & `deme-0.0.4/src/core/utils/ThreadManager.h`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/Timer.hpp` & `deme-0.0.4/src/core/utils/Timer.hpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/WavefrontMeshLoader.hpp` & `deme-0.0.4/src/core/utils/WavefrontMeshLoader.hpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/core/utils/csv.hpp` & `deme-0.0.4/src/core/utils/csv.hpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/CMakeLists.txt` & `deme-0.0.4/src/demo/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_BallDrop.cpp` & `deme-0.0.4/src/demo/DEMdemo_BallDrop.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_Centrifuge.cpp` & `deme-0.0.4/src/demo/DEMdemo_Centrifuge.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_ConePenetration.cpp` & `deme-0.0.4/src/demo/DEMdemo_ConePenetration.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_Electrostatic.cpp` & `deme-0.0.4/src/demo/DEMdemo_Electrostatic.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_FlexibleMesh.cpp` & `deme-0.0.4/src/demo/DEMdemo_FlexibleMesh.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_GRCPrep_Part1.cpp` & `deme-0.0.4/src/demo/DEMdemo_GRCPrep_Part1.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_GRCPrep_Part2.cpp` & `deme-0.0.4/src/demo/DEMdemo_GRCPrep_Part2.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_GameOfLife.cpp` & `deme-0.0.4/src/demo/DEMdemo_GameOfLife.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_Indentation.cpp` & `deme-0.0.4/src/demo/DEMdemo_Indentation.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_Mixer.cpp` & `deme-0.0.4/src/demo/DEMdemo_Mixer.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_Repose.cpp` & `deme-0.0.4/src/demo/DEMdemo_Repose.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_RotatingDrum.cpp` & `deme-0.0.4/src/demo/DEMdemo_RotatingDrum.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_Shake.cpp` & `deme-0.0.4/src/demo/DEMdemo_Shake.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_Sieve.cpp` & `deme-0.0.4/src/demo/DEMdemo_Sieve.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_SingleSphereCollide.cpp` & `deme-0.0.4/src/demo/DEMdemo_SingleSphereCollide.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_SolarSystem.cpp` & `deme-0.0.4/src/demo/DEMdemo_SolarSystem.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_TestPack.cpp` & `deme-0.0.4/src/demo/DEMdemo_TestPack.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_WheelDP.cpp` & `deme-0.0.4/src/demo/DEMdemo_WheelDP.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_WheelDPSimplified.cpp` & `deme-0.0.4/src/demo/DEMdemo_WheelDPSimplified.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/DEMdemo_WheelSlopeSlip.cpp` & `deme-0.0.4/src/demo/DEMdemo_WheelSlopeSlip.cpp`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/pyDEME_BallDrop.py` & `deme-0.0.4/src/demo/pyDEME_BallDrop.py`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/pyDEME_Centrifuge.py` & `deme-0.0.4/src/demo/pyDEME_Centrifuge.py`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/pyDEME_ConePenetration.py` & `deme-0.0.4/src/demo/pyDEME_ConePenetration.py`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/pyDEME_Electrostatic.py` & `deme-0.0.4/src/demo/pyDEME_Electrostatic.py`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/pyDEME_FlexibleMesh.py` & `deme-0.0.4/src/demo/pyDEME_FlexibleMesh.py`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/pyDEME_GRCPrep_Part1.py` & `deme-0.0.4/src/demo/pyDEME_GRCPrep_Part1.py`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/pyDEME_GameOfLife.py` & `deme-0.0.4/src/demo/pyDEME_GameOfLife.py`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/demo/pyDEME_WheelDPSimplified.py` & `deme-0.0.4/src/demo/pyDEME_WheelDPSimplified.py`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/CUDAMathHelpers.cu` & `deme-0.0.4/src/kernel/CUDAMathHelpers.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMBinSphereKernels.cu` & `deme-0.0.4/src/kernel/DEMBinSphereKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMBinTriangleKernels.cu` & `deme-0.0.4/src/kernel/DEMBinTriangleKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMCalcForceKernels.cu` & `deme-0.0.4/src/kernel/DEMCalcForceKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMCollectForceKernels.cu` & `deme-0.0.4/src/kernel/DEMCollectForceKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMCollectForceKernels_Compact.cu` & `deme-0.0.4/src/kernel/DEMCollectForceKernels_Compact.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMCollisionKernels.cu` & `deme-0.0.4/src/kernel/DEMCollisionKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMContactKernels_SphereSphere.cu` & `deme-0.0.4/src/kernel/DEMContactKernels_SphereSphere.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMContactKernels_SphereTriangle.cu` & `deme-0.0.4/src/kernel/DEMContactKernels_SphereTriangle.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMCustomizablePolicies/AnalyticalCompDefJitify.cu` & `deme-0.0.4/src/kernel/DEMCustomizablePolicies/AnalyticalCompDefJitify.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMCustomizablePolicies/ClumpCompAcqStratPartialJitify.cu` & `deme-0.0.4/src/kernel/DEMCustomizablePolicies/ClumpCompAcqStratPartialJitify.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMCustomizablePolicies/ForceInKernelReductionStrat.cu` & `deme-0.0.4/src/kernel/DEMCustomizablePolicies/ForceInKernelReductionStrat.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMCustomizablePolicies/FrictionlessHertzianForceModel.cu` & `deme-0.0.4/src/kernel/DEMCustomizablePolicies/FrictionlessHertzianForceModel.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMCustomizablePolicies/FullHertzianForceModel.cu` & `deme-0.0.4/src/kernel/DEMCustomizablePolicies/FullHertzianForceModel.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMHelperKernels.cu` & `deme-0.0.4/src/kernel/DEMHelperKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMHistoryMappingKernels.cu` & `deme-0.0.4/src/kernel/DEMHistoryMappingKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMIntegrationKernels.cu` & `deme-0.0.4/src/kernel/DEMIntegrationKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMMiscKernels.cu` & `deme-0.0.4/src/kernel/DEMMiscKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMModeratorKernels.cu` & `deme-0.0.4/src/kernel/DEMModeratorKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMOwnerQueryKernels.cu` & `deme-0.0.4/src/kernel/DEMOwnerQueryKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMPrepForceKernels.cu` & `deme-0.0.4/src/kernel/DEMPrepForceKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMSphereQueryKernels.cu` & `deme-0.0.4/src/kernel/DEMSphereQueryKernels.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMTriangleBoxIntersect.cu` & `deme-0.0.4/src/kernel/DEMTriangleBoxIntersect.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMUserScripts/ForceModelWithCohesion.cu` & `deme-0.0.4/src/kernel/DEMUserScripts/ForceModelWithCohesion.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMUserScripts/ForceModelWithElectrostatic.cu` & `deme-0.0.4/src/kernel/DEMUserScripts/ForceModelWithElectrostatic.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/src/kernel/DEMUserScripts/ForceModelWithGravity.cu` & `deme-0.0.4/src/kernel/DEMUserScripts/ForceModelWithGravity.cu`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tests/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tests/test_embed/CMakeLists.txt` & `deme-0.0.4/thirdparty/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tools/FindCatch.cmake` & `deme-0.0.4/thirdparty/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tools/FindEigen3.cmake` & `deme-0.0.4/thirdparty/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tools/FindPythonLibsNew.cmake` & `deme-0.0.4/thirdparty/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tools/JoinPaths.cmake` & `deme-0.0.4/thirdparty/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tools/pybind11Common.cmake` & `deme-0.0.4/thirdparty/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tools/pybind11NewTools.cmake` & `deme-0.0.4/thirdparty/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `DEME-0.0.3/thirdparty/pybind11/tools/pybind11Tools.cmake` & `deme-0.0.4/thirdparty/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

