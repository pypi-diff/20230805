# Comparing `tmp/pynabi-0.1.1.tar.gz` & `tmp/pynabi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\feder\Documents\Scuola\Univerit\340\prova finale 3\nasello\dist\.tmp-x8rox8y2\pynabi-0.1.1.tar", last modified: Fri Jun 30 18:52:21 2023, max compression
+gzip compressed data, was "pynabi-0.1.2.tar", last modified: Sat Aug  5 13:42:52 2023, max compression
```

## Comparing `pynabi-0.1.1.tar` & `pynabi-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 18:52:21.183422 pynabi-0.1.1/
--rw-rw-rw-   0        0        0     1094 2023-06-14 17:22:45.000000 pynabi-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     8272 2023-06-30 18:52:21.183422 pynabi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5989 2023-06-30 17:30:56.000000 pynabi-0.1.1/README.md
--rw-rw-rw-   0        0        0     1084 2023-06-30 18:51:30.000000 pynabi-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 18:52:21.183422 pynabi-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 18:52:21.154502 pynabi-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 18:52:21.176444 pynabi-0.1.1/src/pynabi/
--rw-rw-rw-   0        0        0       47 2023-06-30 16:56:26.000000 pynabi-0.1.1/src/pynabi/__init__.py
--rw-rw-rw-   0        0        0     6042 2023-06-30 18:35:33.000000 pynabi-0.1.1/src/pynabi/_common.py
--rw-rw-rw-   0        0        0     9151 2023-06-30 18:45:35.000000 pynabi-0.1.1/src/pynabi/_dataset.py
--rw-rw-rw-   0        0        0     4204 2023-06-17 21:06:56.000000 pynabi-0.1.1/src/pynabi/calculation.py
--rw-rw-rw-   0        0        0     9529 2023-06-17 21:28:04.000000 pynabi-0.1.1/src/pynabi/crystal.py
--rw-rw-rw-   0        0        0    11672 2023-06-30 17:18:06.000000 pynabi-0.1.1/src/pynabi/kspace.py
--rw-rw-rw-   0        0        0     7844 2023-06-21 21:36:17.000000 pynabi-0.1.1/src/pynabi/occupation.py
--rw-rw-rw-   0        0        0    14540 2023-06-17 19:55:26.000000 pynabi-0.1.1/src/pynabi/relaxation.py
--rw-rw-rw-   0        0        0     3727 2023-06-17 21:24:10.000000 pynabi-0.1.1/src/pynabi/units.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:52:21.181456 pynabi-0.1.1/src/pynabi.egg-info/
--rw-rw-rw-   0        0        0     8272 2023-06-30 18:52:21.000000 pynabi-0.1.1/src/pynabi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-06-30 18:52:21.000000 pynabi-0.1.1/src/pynabi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 18:52:21.000000 pynabi-0.1.1/src/pynabi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 18:52:21.000000 pynabi-0.1.1/src/pynabi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:42:52.422598 pynabi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-05 13:42:43.000000 pynabi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-08-05 13:42:52.422598 pynabi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-08-05 13:42:43.000000 pynabi-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-05 13:42:43.000000 pynabi-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 13:42:52.422598 pynabi-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:42:52.418598 pynabi-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:42:52.422598 pynabi-0.1.2/src/pynabi/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 13:42:43.000000 pynabi-0.1.2/src/pynabi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-08-05 13:42:43.000000 pynabi-0.1.2/src/pynabi/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-08-05 13:42:43.000000 pynabi-0.1.2/src/pynabi/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-08-05 13:42:43.000000 pynabi-0.1.2/src/pynabi/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-08-05 13:42:43.000000 pynabi-0.1.2/src/pynabi/crystal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-08-05 13:42:43.000000 pynabi-0.1.2/src/pynabi/kspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-08-05 13:42:43.000000 pynabi-0.1.2/src/pynabi/occupation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-08-05 13:42:43.000000 pynabi-0.1.2/src/pynabi/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-05 13:42:43.000000 pynabi-0.1.2/src/pynabi/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:42:52.422598 pynabi-0.1.2/src/pynabi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-08-05 13:42:52.000000 pynabi-0.1.2/src/pynabi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-05 13:42:52.000000 pynabi-0.1.2/src/pynabi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:42:52.000000 pynabi-0.1.2/src/pynabi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 13:42:52.000000 pynabi-0.1.2/src/pynabi.egg-info/top_level.txt
```

### Comparing `pynabi-0.1.1/PKG-INFO` & `pynabi-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,222 +1,225 @@
-Metadata-Version: 2.1
-Name: pynabi
-Version: 0.1.1
-Summary: A package to easily create Abinit input files
-Author: Federico Guglielmi
-License: MIT License
-        
-        Copyright (c) 2023 Federico Guglielmi
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/Fedesky25/pynabi
-Project-URL: Bug Tracker, https://github.com/Fedesky25/pynabi/issues
-Project-URL: Documentation, https://github.com/Fedesky25/pynabi/wiki
-Project-URL: Repository, https://github.com/Fedesky25/pynabi.git
-Project-URL: Changelog, https://github.com/Fedesky25/pynabi/blob/master/CHANGELOG.md
-Keywords: abinit
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PynAbi
-
-Python package to easily create [Abinit](https://www.abinit.org/) input files.
-
-```cmd
-pip install pynabi
-```
-
-## Example
-
-```python
-from pynabi import createAbi, DataSet, AbIn, AbOut
-from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
-from pynabi.calculation import ToleranceOn, EnergyCutoff, MaxSteps, SCFMixing, NonSelfConsistentCalc
-from pynabi.crystal import Atom, FluoriteLike
-from pynabi.occupation import OccupationPerBand
-from pynabi.units import eV, nm
-
-# create manually an atom -> Atom(<Z>, <pseudo potential name>)
-# or using sensible defaults as follows
-Zr = Atom.of("Zr")  # Z=40 and pseudos located at "Zr.psp8"
-Oxy = Atom.of("O")  # Z=8 and pseudos located at "O.psp8"
-
-# base dataset with common variables
-base = DataSet(
-    AbOut("./scf/scf"),                             # prefix for output files
-    AbIn().PseudoPotentials("./pseudos/PBE-SR"),    # folder with pseudo potentials
-
-    FluoriteLike(Zr, Oxy, 0.5135*nm),               # creates AtomBasis and Lattice of a crystal like fluorite
-                                                    # with lattice constant 0.5135nm
-
-    SymmetricGrid(BZ.Irreducible, UsualKShifts.FCC) # easily define kptopt, ngkpt, nshiftk, kpt
-        .ofMonkhorstPack(4),
-
-    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density 
-                                                    # based on the last 10 iteration
-
-    ToleranceOn.EnergyDifference(1e-6),             # expressively define the tolerance
-    MaxSteps(30)                                    # nstep
-)
-
-# set the default energy unit in eV (from now on)
-eV.setAsReference()
-
-# datasets to see the convergenge as a function of energy
-sets = [DataSet(EnergyCutoff(8.0 + i*0.25)) for i in range(0,17)]
-
-# final non-self-consistent round to find bands 
-bands = DataSet(
-    NonSelfConsistentCalc(),
-    ToleranceOn.WavefunctionSquaredResidual(1e-12),
-    AbIn().ElectronDensity(sets[-1]),                   # get the electron density from the last dataset
-    OccupationPerBand(2.0, repeat=8),                   # same number of bands (max 8) for each k point
-    Path.auto(10, "GXWKGLUWLK", CriticalPointsOf.FCC)   # easily define a path in the k-space   
-)
-
-with open("./out.txt", 'w') as f:
-    f.write(createAbi(base, *sets, bands))
-```
-
-<details>
-<summary><b>Output</b></summary>
-
-```txt
-ndtset 18
-
-# Atoms definition
-ntypat 2
-znucl 8 40
-pseudos "O.psp8, Zr.psp8"
-
-# Common DataSet
-natoms 3
-typeat 2 1 1
-xred 0 0 0   0.3333333333333333 0.3333333333333333 0.3333333333333333   0.6666666666666666 0.6666666666666666 0.6666666666666666
-outdata_prefix "./scf/scf"
-pp_dirpath "./pseudos/PBE-SR"
-scalecart 0.5135 0.5135 0.5135 nm
-rprim 0.5 0.5 0.0   0.0 0.5 0.5   0.5 0.0 0.5
-ngkpt 4 4 4
-iscf 17
-npulayit 10
-toldfe 1e-06
-nstep 30
-
-# DataSet 1
-ecut1 8.0 eV
-
-# DataSet 2
-ecut2 8.25 eV
-
-# DataSet 3
-ecut3 8.5 eV
-
-# DataSet 4
-ecut4 8.75 eV
-
-# DataSet 5
-ecut5 9.0 eV
-
-# DataSet 6
-ecut6 9.25 eV
-
-# DataSet 7
-ecut7 9.5 eV
-
-# DataSet 8
-ecut8 9.75 eV
-
-# DataSet 9
-ecut9 10.0 eV
-
-# DataSet 10
-ecut10 10.25 eV
-
-# DataSet 11
-ecut11 10.5 eV
-
-# DataSet 12
-ecut12 10.75 eV
-
-# DataSet 13
-ecut13 11.0 eV
-
-# DataSet 14
-ecut14 11.25 eV
-
-# DataSet 15
-ecut15 11.5 eV
-
-# DataSet 16
-ecut16 11.75 eV
-
-# DataSet 17
-ecut17 12.0 eV
-
-# DataSet 18
-iscf18 -2
-tolwfr18 1e-12
-getden18 17
-occopt18 0
-occ18 8*2.0
-bands18 8
-kptopt18 -9
-kptbounds18 0 0 0  0.0 0.5 0.5  0.25 0.75 0.5  0.375 0.75 0.375  0 0 0  0.5 0.5 0.5  0.25 0.625 0.625  0.25 0.75 0.5  0.5 0.5 0.5  0.375 0.75 0.375
-ndivsm18 10
-```
-
-</details>
-
-## Features
-
- - Multi dataset support
- - Helper functions for common crystal structures (caesium chloride, rock-salt, fluorite, zincblende, wurtzite, nickeline, HCP)
- - Registered critical points of and methodsto create lattices of CUB, BCC, FCC, HEX, TET, BCT, ORC, ORCC
- - Smooth experience in defining the k-points
- - Handy management of [file handling variables](https://docs.abinit.org/variables/files/)
- - Almost full covarage of [basic input variables](https://docs.abinit.org/variables/basic/) (missing nbandhf, symrel, tnons, wvl_hgrid)
- - Partial coverage of [ground state variables](https://docs.abinit.org/variables/gstate/)
- - Partial coverage of [relaxation variables](https://docs.abinit.org/variables/rlx/)
- - _More to come..._
-
-## Why PynAbi over pure Abinit files?
-
-If you're a very experienced Abinit user who knows its variables and their possible values (and associated meaning), then this package probably isn't for you.
-For all other users, on top of all the aforementioned features, here's a list of reasons why you could find PynAbi useful:
-
- 1. You have all the power of coding to generate Abinit instructions, e.g. reusability, loops to generate datasets programmatically
- 2. It provides some useful presets and helper functions/methods that allows you to skip to the fun part of the simulation
- 3. Under the hood, it checks for the validity of variable values *before* starting Abinit
- 4. It makes use of expressive declarations and definition, leading to readable and comprehensible istructions
- 5. If you're using a code editor (with autocompletition), you'll get suggetions of all the possible options in a more natural language 
-
-Some prior knowledge of Abinit (and DFT in general) is nonetheless needed to fully understand what actually is to be simulated: this package only provides a handier way to generate the required files.
-
-## Documentation
-
-Although currently severely incomplete, a wiki is available on the [GitHub repository Wiki](https://github.com/Fedesky25/pynabi/wiki). Ideally a wiki for this package shouldn't be needed if your editor has some autocompletition: the aim is to document every class and function with a detailed description taken from the relevant parts of ABINIT documentation. 
+Metadata-Version: 2.1
+Name: pynabi
+Version: 0.1.2
+Summary: A package to easily create Abinit input files
+Author: Federico Guglielmi
+License: MIT License
+        
+        Copyright (c) 2023 Federico Guglielmi
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/Fedesky25/pynabi
+Project-URL: Bug Tracker, https://github.com/Fedesky25/pynabi/issues
+Project-URL: Documentation, https://github.com/Fedesky25/pynabi/wiki
+Project-URL: Repository, https://github.com/Fedesky25/pynabi.git
+Project-URL: Changelog, https://github.com/Fedesky25/pynabi/blob/master/CHANGELOG.md
+Keywords: abinit
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PynAbi
+
+Python package to easily create [Abinit](https://www.abinit.org/) input files.
+
+```cmd
+pip install pynabi
+```
+
+## Example
+
+```python
+from pynabi import createAbi, DataSet, AbIn, AbOut
+from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
+from pynabi.calculation import ToleranceOn, EnergyCutoff, MaxSteps, SCFMixing, NonSelfConsistentCalc
+from pynabi.crystal import Atom, FluoriteLike
+from pynabi.occupation import OccupationPerBand
+from pynabi.units import eV, nm
+
+# create manually an atom -> Atom(<Z>, <pseudo potential name>)
+# or using sensible defaults as follows
+Zr = Atom.of("Zr")  # Z=40 and pseudos located at "Zr.psp8"
+Oxy = Atom.of("O")  # Z=8 and pseudos located at "O.psp8"
+
+# base dataset with common variables
+base = DataSet(
+    AbOut("./scf/scf"),                             # prefix for output files
+    AbIn().PseudoPotentials("./pseudos/PBE-SR"),    # folder with pseudo potentials
+
+    FluoriteLike(Zr, Oxy, 0.5135*nm),               # creates AtomBasis and Lattice of a crystal like fluorite
+                                                    # with lattice constant 0.5135nm
+
+    SymmetricGrid(BZ.Irreducible, UsualKShifts.FCC) # easily define kptopt, ngkpt, nshiftk, kpt
+        .ofMonkhorstPack(4),
+
+    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density 
+                                                    # based on the last 10 iteration
+
+    ToleranceOn.EnergyDifference(1e-6),             # expressively define the tolerance
+    MaxSteps(30)                                    # nstep
+)
+
+# set the default energy unit in eV (from now on)
+eV.setAsReference()
+
+# datasets to see the convergenge as a function of energy
+sets = [DataSet(EnergyCutoff(8.0 + i*0.25)) for i in range(0,17)]
+
+# final non-self-consistent round to find bands 
+bands = DataSet(
+    NonSelfConsistentCalc(),
+    ToleranceOn.WavefunctionSquaredResidual(1e-12),
+    AbIn().ElectronDensity(sets[-1]),                   # get the electron density from the last dataset
+    OccupationPerBand(2.0, repeat=8),                   # same number of bands (max 8) for each k point
+    Path.auto(10, "GXWKGLUWLK", CriticalPointsOf.FCC)   # easily define a path in the k-space   
+)
+
+with open("./out.txt", 'w') as f:
+    f.write(createAbi(base, *sets, bands))
+```
+
+<details>
+<summary><b>Output</b></summary>
+
+```txt
+ndtset 18
+
+# Atoms definition
+ntypat 2
+znucl 40 8
+pseudos "Zr.psp8, O.psp8"
+
+# Common DataSet
+natom 3
+typat 1 2 2
+xred 0 0 0   0.3333333333333333 0.3333333333333333 0.3333333333333333   0.6666666666666666 0.6666666666666666 0.6666666666666666
+outdata_prefix "./scf/scf"
+pp_dirpath "./pseudos/PBE-SR"
+scalecart 0.5135 0.5135 0.5135 nm
+rprim 0.5 0.5 0.0   0.0 0.5 0.5   0.5 0.0 0.5
+kptopt 1
+nshiftk 4
+shiftk 0.5 0.5 0.5 0.5 0.0 0.0 0.0 0.5 0.0 0.0 0.0 0.5
+ngkpt 4 4 4
+iscf 17
+npulayit 10
+toldfe 1e-06
+nstep 30
+
+# DataSet 1
+ecut1 8.0 eV
+
+# DataSet 2
+ecut2 8.25 eV
+
+# DataSet 3
+ecut3 8.5 eV
+
+# DataSet 4
+ecut4 8.75 eV
+
+# DataSet 5
+ecut5 9.0 eV
+
+# DataSet 6
+ecut6 9.25 eV
+
+# DataSet 7
+ecut7 9.5 eV
+
+# DataSet 8
+ecut8 9.75 eV
+
+# DataSet 9
+ecut9 10.0 eV
+
+# DataSet 10
+ecut10 10.25 eV
+
+# DataSet 11
+ecut11 10.5 eV
+
+# DataSet 12
+ecut12 10.75 eV
+
+# DataSet 13
+ecut13 11.0 eV
+
+# DataSet 14
+ecut14 11.25 eV
+
+# DataSet 15
+ecut15 11.5 eV
+
+# DataSet 16
+ecut16 11.75 eV
+
+# DataSet 17
+ecut17 12.0 eV
+
+# DataSet 18
+iscf18 -2
+tolwfr18 1e-12
+getden18 17
+occopt18 0
+occ18 8*2.0
+band18 8
+kptopt18 -9
+kptbounds18 0 0 0  0.0 0.5 0.5  0.25 0.75 0.5  0.375 0.75 0.375  0 0 0  0.5 0.5 0.5  0.25 0.625 0.625  0.25 0.75 0.5  0.5 0.5 0.5  0.375 0.75 0.375
+ndivsm18 10
+```
+
+</details>
+
+## Features
+
+ - Multi dataset support
+ - Helper functions for common crystal structures (caesium chloride, rock-salt, fluorite, zincblende, wurtzite, nickeline, HCP)
+ - Registered critical points of and methodsto create lattices of CUB, BCC, FCC, HEX, TET, BCT, ORC, ORCC
+ - Smooth experience in defining the k-points
+ - Handy management of [file handling variables](https://docs.abinit.org/variables/files/)
+ - Almost full covarage of [basic input variables](https://docs.abinit.org/variables/basic/) (missing nbandhf, symrel, tnons, wvl_hgrid)
+ - Partial coverage of [ground state variables](https://docs.abinit.org/variables/gstate/)
+ - Partial coverage of [relaxation variables](https://docs.abinit.org/variables/rlx/)
+ - _More to come..._
+
+## Why PynAbi over pure Abinit files?
+
+If you're a very experienced Abinit user who knows its variables and their possible values (and associated meaning), then this package probably isn't for you.
+For all other users, on top of all the aforementioned features, here's a list of reasons why you could find PynAbi useful:
+
+ 1. You have all the power of coding to generate Abinit instructions, e.g. reusability, loops to generate datasets programmatically
+ 2. It provides some useful presets and helper functions/methods that allows you to skip to the fun part of the simulation
+ 3. Under the hood, it checks for the validity of variable values *before* starting Abinit
+ 4. It makes use of expressive declarations and definition, leading to readable and comprehensible istructions
+ 5. If you're using a code editor (with autocompletition), you'll get suggetions of all the possible options in a more natural language 
+
+Some prior knowledge of Abinit (and DFT in general) is nonetheless needed to fully understand what actually is to be simulated: this package only provides a handier way to generate the required files.
+
+## Documentation
+
+Although currently severely incomplete, a wiki is available on the [GitHub repository Wiki](https://github.com/Fedesky25/pynabi/wiki). Ideally a wiki for this package shouldn't be needed if your editor has some autocompletition: the aim is to document every class and function with a detailed description taken from the relevant parts of ABINIT documentation.
```

### Comparing `pynabi-0.1.1/README.md` & `pynabi-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,178 +1,181 @@
-# PynAbi
-
-Python package to easily create [Abinit](https://www.abinit.org/) input files.
-
-```cmd
-pip install pynabi
-```
-
-## Example
-
-```python
-from pynabi import createAbi, DataSet, AbIn, AbOut
-from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
-from pynabi.calculation import ToleranceOn, EnergyCutoff, MaxSteps, SCFMixing, NonSelfConsistentCalc
-from pynabi.crystal import Atom, FluoriteLike
-from pynabi.occupation import OccupationPerBand
-from pynabi.units import eV, nm
-
-# create manually an atom -> Atom(<Z>, <pseudo potential name>)
-# or using sensible defaults as follows
-Zr = Atom.of("Zr")  # Z=40 and pseudos located at "Zr.psp8"
-Oxy = Atom.of("O")  # Z=8 and pseudos located at "O.psp8"
-
-# base dataset with common variables
-base = DataSet(
-    AbOut("./scf/scf"),                             # prefix for output files
-    AbIn().PseudoPotentials("./pseudos/PBE-SR"),    # folder with pseudo potentials
-
-    FluoriteLike(Zr, Oxy, 0.5135*nm),               # creates AtomBasis and Lattice of a crystal like fluorite
-                                                    # with lattice constant 0.5135nm
-
-    SymmetricGrid(BZ.Irreducible, UsualKShifts.FCC) # easily define kptopt, ngkpt, nshiftk, kpt
-        .ofMonkhorstPack(4),
-
-    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density 
-                                                    # based on the last 10 iteration
-
-    ToleranceOn.EnergyDifference(1e-6),             # expressively define the tolerance
-    MaxSteps(30)                                    # nstep
-)
-
-# set the default energy unit in eV (from now on)
-eV.setAsReference()
-
-# datasets to see the convergenge as a function of energy
-sets = [DataSet(EnergyCutoff(8.0 + i*0.25)) for i in range(0,17)]
-
-# final non-self-consistent round to find bands 
-bands = DataSet(
-    NonSelfConsistentCalc(),
-    ToleranceOn.WavefunctionSquaredResidual(1e-12),
-    AbIn().ElectronDensity(sets[-1]),                   # get the electron density from the last dataset
-    OccupationPerBand(2.0, repeat=8),                   # same number of bands (max 8) for each k point
-    Path.auto(10, "GXWKGLUWLK", CriticalPointsOf.FCC)   # easily define a path in the k-space   
-)
-
-with open("./out.txt", 'w') as f:
-    f.write(createAbi(base, *sets, bands))
-```
-
-<details>
-<summary><b>Output</b></summary>
-
-```txt
-ndtset 18
-
-# Atoms definition
-ntypat 2
-znucl 8 40
-pseudos "O.psp8, Zr.psp8"
-
-# Common DataSet
-natoms 3
-typeat 2 1 1
-xred 0 0 0   0.3333333333333333 0.3333333333333333 0.3333333333333333   0.6666666666666666 0.6666666666666666 0.6666666666666666
-outdata_prefix "./scf/scf"
-pp_dirpath "./pseudos/PBE-SR"
-scalecart 0.5135 0.5135 0.5135 nm
-rprim 0.5 0.5 0.0   0.0 0.5 0.5   0.5 0.0 0.5
-ngkpt 4 4 4
-iscf 17
-npulayit 10
-toldfe 1e-06
-nstep 30
-
-# DataSet 1
-ecut1 8.0 eV
-
-# DataSet 2
-ecut2 8.25 eV
-
-# DataSet 3
-ecut3 8.5 eV
-
-# DataSet 4
-ecut4 8.75 eV
-
-# DataSet 5
-ecut5 9.0 eV
-
-# DataSet 6
-ecut6 9.25 eV
-
-# DataSet 7
-ecut7 9.5 eV
-
-# DataSet 8
-ecut8 9.75 eV
-
-# DataSet 9
-ecut9 10.0 eV
-
-# DataSet 10
-ecut10 10.25 eV
-
-# DataSet 11
-ecut11 10.5 eV
-
-# DataSet 12
-ecut12 10.75 eV
-
-# DataSet 13
-ecut13 11.0 eV
-
-# DataSet 14
-ecut14 11.25 eV
-
-# DataSet 15
-ecut15 11.5 eV
-
-# DataSet 16
-ecut16 11.75 eV
-
-# DataSet 17
-ecut17 12.0 eV
-
-# DataSet 18
-iscf18 -2
-tolwfr18 1e-12
-getden18 17
-occopt18 0
-occ18 8*2.0
-bands18 8
-kptopt18 -9
-kptbounds18 0 0 0  0.0 0.5 0.5  0.25 0.75 0.5  0.375 0.75 0.375  0 0 0  0.5 0.5 0.5  0.25 0.625 0.625  0.25 0.75 0.5  0.5 0.5 0.5  0.375 0.75 0.375
-ndivsm18 10
-```
-
-</details>
-
-## Features
-
- - Multi dataset support
- - Helper functions for common crystal structures (caesium chloride, rock-salt, fluorite, zincblende, wurtzite, nickeline, HCP)
- - Registered critical points of and methodsto create lattices of CUB, BCC, FCC, HEX, TET, BCT, ORC, ORCC
- - Smooth experience in defining the k-points
- - Handy management of [file handling variables](https://docs.abinit.org/variables/files/)
- - Almost full covarage of [basic input variables](https://docs.abinit.org/variables/basic/) (missing nbandhf, symrel, tnons, wvl_hgrid)
- - Partial coverage of [ground state variables](https://docs.abinit.org/variables/gstate/)
- - Partial coverage of [relaxation variables](https://docs.abinit.org/variables/rlx/)
- - _More to come..._
-
-## Why PynAbi over pure Abinit files?
-
-If you're a very experienced Abinit user who knows its variables and their possible values (and associated meaning), then this package probably isn't for you.
-For all other users, on top of all the aforementioned features, here's a list of reasons why you could find PynAbi useful:
-
- 1. You have all the power of coding to generate Abinit instructions, e.g. reusability, loops to generate datasets programmatically
- 2. It provides some useful presets and helper functions/methods that allows you to skip to the fun part of the simulation
- 3. Under the hood, it checks for the validity of variable values *before* starting Abinit
- 4. It makes use of expressive declarations and definition, leading to readable and comprehensible istructions
- 5. If you're using a code editor (with autocompletition), you'll get suggetions of all the possible options in a more natural language 
-
-Some prior knowledge of Abinit (and DFT in general) is nonetheless needed to fully understand what actually is to be simulated: this package only provides a handier way to generate the required files.
-
-## Documentation
-
+# PynAbi
+
+Python package to easily create [Abinit](https://www.abinit.org/) input files.
+
+```cmd
+pip install pynabi
+```
+
+## Example
+
+```python
+from pynabi import createAbi, DataSet, AbIn, AbOut
+from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
+from pynabi.calculation import ToleranceOn, EnergyCutoff, MaxSteps, SCFMixing, NonSelfConsistentCalc
+from pynabi.crystal import Atom, FluoriteLike
+from pynabi.occupation import OccupationPerBand
+from pynabi.units import eV, nm
+
+# create manually an atom -> Atom(<Z>, <pseudo potential name>)
+# or using sensible defaults as follows
+Zr = Atom.of("Zr")  # Z=40 and pseudos located at "Zr.psp8"
+Oxy = Atom.of("O")  # Z=8 and pseudos located at "O.psp8"
+
+# base dataset with common variables
+base = DataSet(
+    AbOut("./scf/scf"),                             # prefix for output files
+    AbIn().PseudoPotentials("./pseudos/PBE-SR"),    # folder with pseudo potentials
+
+    FluoriteLike(Zr, Oxy, 0.5135*nm),               # creates AtomBasis and Lattice of a crystal like fluorite
+                                                    # with lattice constant 0.5135nm
+
+    SymmetricGrid(BZ.Irreducible, UsualKShifts.FCC) # easily define kptopt, ngkpt, nshiftk, kpt
+        .ofMonkhorstPack(4),
+
+    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density 
+                                                    # based on the last 10 iteration
+
+    ToleranceOn.EnergyDifference(1e-6),             # expressively define the tolerance
+    MaxSteps(30)                                    # nstep
+)
+
+# set the default energy unit in eV (from now on)
+eV.setAsReference()
+
+# datasets to see the convergenge as a function of energy
+sets = [DataSet(EnergyCutoff(8.0 + i*0.25)) for i in range(0,17)]
+
+# final non-self-consistent round to find bands 
+bands = DataSet(
+    NonSelfConsistentCalc(),
+    ToleranceOn.WavefunctionSquaredResidual(1e-12),
+    AbIn().ElectronDensity(sets[-1]),                   # get the electron density from the last dataset
+    OccupationPerBand(2.0, repeat=8),                   # same number of bands (max 8) for each k point
+    Path.auto(10, "GXWKGLUWLK", CriticalPointsOf.FCC)   # easily define a path in the k-space   
+)
+
+with open("./out.txt", 'w') as f:
+    f.write(createAbi(base, *sets, bands))
+```
+
+<details>
+<summary><b>Output</b></summary>
+
+```txt
+ndtset 18
+
+# Atoms definition
+ntypat 2
+znucl 40 8
+pseudos "Zr.psp8, O.psp8"
+
+# Common DataSet
+natom 3
+typat 1 2 2
+xred 0 0 0   0.3333333333333333 0.3333333333333333 0.3333333333333333   0.6666666666666666 0.6666666666666666 0.6666666666666666
+outdata_prefix "./scf/scf"
+pp_dirpath "./pseudos/PBE-SR"
+scalecart 0.5135 0.5135 0.5135 nm
+rprim 0.5 0.5 0.0   0.0 0.5 0.5   0.5 0.0 0.5
+kptopt 1
+nshiftk 4
+shiftk 0.5 0.5 0.5 0.5 0.0 0.0 0.0 0.5 0.0 0.0 0.0 0.5
+ngkpt 4 4 4
+iscf 17
+npulayit 10
+toldfe 1e-06
+nstep 30
+
+# DataSet 1
+ecut1 8.0 eV
+
+# DataSet 2
+ecut2 8.25 eV
+
+# DataSet 3
+ecut3 8.5 eV
+
+# DataSet 4
+ecut4 8.75 eV
+
+# DataSet 5
+ecut5 9.0 eV
+
+# DataSet 6
+ecut6 9.25 eV
+
+# DataSet 7
+ecut7 9.5 eV
+
+# DataSet 8
+ecut8 9.75 eV
+
+# DataSet 9
+ecut9 10.0 eV
+
+# DataSet 10
+ecut10 10.25 eV
+
+# DataSet 11
+ecut11 10.5 eV
+
+# DataSet 12
+ecut12 10.75 eV
+
+# DataSet 13
+ecut13 11.0 eV
+
+# DataSet 14
+ecut14 11.25 eV
+
+# DataSet 15
+ecut15 11.5 eV
+
+# DataSet 16
+ecut16 11.75 eV
+
+# DataSet 17
+ecut17 12.0 eV
+
+# DataSet 18
+iscf18 -2
+tolwfr18 1e-12
+getden18 17
+occopt18 0
+occ18 8*2.0
+band18 8
+kptopt18 -9
+kptbounds18 0 0 0  0.0 0.5 0.5  0.25 0.75 0.5  0.375 0.75 0.375  0 0 0  0.5 0.5 0.5  0.25 0.625 0.625  0.25 0.75 0.5  0.5 0.5 0.5  0.375 0.75 0.375
+ndivsm18 10
+```
+
+</details>
+
+## Features
+
+ - Multi dataset support
+ - Helper functions for common crystal structures (caesium chloride, rock-salt, fluorite, zincblende, wurtzite, nickeline, HCP)
+ - Registered critical points of and methodsto create lattices of CUB, BCC, FCC, HEX, TET, BCT, ORC, ORCC
+ - Smooth experience in defining the k-points
+ - Handy management of [file handling variables](https://docs.abinit.org/variables/files/)
+ - Almost full covarage of [basic input variables](https://docs.abinit.org/variables/basic/) (missing nbandhf, symrel, tnons, wvl_hgrid)
+ - Partial coverage of [ground state variables](https://docs.abinit.org/variables/gstate/)
+ - Partial coverage of [relaxation variables](https://docs.abinit.org/variables/rlx/)
+ - _More to come..._
+
+## Why PynAbi over pure Abinit files?
+
+If you're a very experienced Abinit user who knows its variables and their possible values (and associated meaning), then this package probably isn't for you.
+For all other users, on top of all the aforementioned features, here's a list of reasons why you could find PynAbi useful:
+
+ 1. You have all the power of coding to generate Abinit instructions, e.g. reusability, loops to generate datasets programmatically
+ 2. It provides some useful presets and helper functions/methods that allows you to skip to the fun part of the simulation
+ 3. Under the hood, it checks for the validity of variable values *before* starting Abinit
+ 4. It makes use of expressive declarations and definition, leading to readable and comprehensible istructions
+ 5. If you're using a code editor (with autocompletition), you'll get suggetions of all the possible options in a more natural language 
+
+Some prior knowledge of Abinit (and DFT in general) is nonetheless needed to fully understand what actually is to be simulated: this package only provides a handier way to generate the required files.
+
+## Documentation
+
 Although currently severely incomplete, a wiki is available on the [GitHub repository Wiki](https://github.com/Fedesky25/pynabi/wiki). Ideally a wiki for this package shouldn't be needed if your editor has some autocompletition: the aim is to document every class and function with a detailed description taken from the relevant parts of ABINIT documentation.
```

### Comparing `pynabi-0.1.1/pyproject.toml` & `pynabi-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "pynabi"
-version = "0.1.1"
-description = "A package to easily create Abinit input files"
-keywords = [ "abinit" ]
-license = { file = "LICENSE" }
-readme = "README.md"
-authors = [
-  { name="Federico Guglielmi" }
-]
-requires-python = ">=3.11"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Science/Research",
-    "Topic :: Scientific/Engineering :: Physics",
-    "Topic :: Scientific/Engineering :: Chemistry",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/Fedesky25/pynabi"
-"Bug Tracker" = "https://github.com/Fedesky25/pynabi/issues"
-"Documentation" = "https://github.com/Fedesky25/pynabi/wiki"
-"Repository" = "https://github.com/Fedesky25/pynabi.git"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pynabi"
+version = "0.1.2"
+description = "A package to easily create Abinit input files"
+keywords = [ "abinit" ]
+license = { file = "LICENSE" }
+readme = "README.md"
+authors = [
+  { name="Federico Guglielmi" }
+]
+requires-python = ">=3.11"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Science/Research",
+    "Topic :: Scientific/Engineering :: Physics",
+    "Topic :: Scientific/Engineering :: Chemistry",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/Fedesky25/pynabi"
+"Bug Tracker" = "https://github.com/Fedesky25/pynabi/issues"
+"Documentation" = "https://github.com/Fedesky25/pynabi/wiki"
+"Repository" = "https://github.com/Fedesky25/pynabi.git"
 "Changelog" = "https://github.com/Fedesky25/pynabi/blob/master/CHANGELOG.md"
```

### Comparing `pynabi-0.1.1/src/pynabi/_common.py` & `pynabi-0.1.2/src/pynabi/_common.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-from typing import TypeVar, Type, Tuple, Callable, Any, TypeGuard
-
-
-__all__ = ["Vec3D"]
-
-
-class Singleton(object):
-    _instance = None
-    def __new__(cls):
-        if cls._instance is None:
-            cls._instance = object.__new__(cls)
-        return cls._instance
-    
-    @classmethod
-    def eq(cls, value):
-        return type(value) is cls or value is cls
-
-
-class Vec3D:
-    def __init__(self, x: float, y: float, z: float) -> None:
-        self.x = x
-        self.y = y
-        self.z = z
-    
-    def __str__(self) -> str:
-        return "{} {} {}".format(self.x, self.y, self.z)
-    
-    @staticmethod
-    def uniform(v: float = 1.0):
-        return Vec3D(v,v,v)
-    
-    @staticmethod
-    def zero():
-        return Vec3D(0,0,0)
-
- 
-S = TypeVar("S", bound="Stampable")
-
-class StampCollection:
-    def __init__(self, siblings: 'dict[type,Stampable]', base: 'dict[type,Stampable]') -> None:
-        self._s = siblings
-        self._b = base
-    
-    def get(self, t: Type[S]) -> S | None:
-        s = self._s.get(t);
-        if s is None:
-            s = self._b.get(t)
-        return s # type: ignore
-    
-    def nextto(self, t: Type['Stampable']):
-        return t in self._s
-
-
-class Stampable:
-    def stamp(self, index: int):
-        raise NotImplementedError(f"{type(self).__name__} has not implemented stamp")
-    
-    def compatible(self, coll: 'StampCollection'):
-        pass
-    
-    def __str__(self):
-        return self.stamp(0)
-
-
-class OneLineStamp(Stampable):
-    name = ''
-    
-    def __init__(self, value, suffix: str = '') -> None:
-        super().__init__()
-        self.value = value
-        self.suffix = suffix
-
-    def stamp(self, index: int):
-        t = type(self)
-        return f"{t.name}{self.suffix}{index or ''} {self.value}"
-
-
-class Later(Singleton):
-    pass
-
-
-class DelayedInfo:
-    def __init__(self, prop: str, name: str) -> None:
-        self.prop = prop
-        self.name = name
-
-    def sanitize(self, value):
-        raise NotImplementedError()
-    
-    def laterOrSanitized(self, value):
-        return value if value is Later._instance else self.sanitize(value)
-    
-    def stamp(self, suffix, value):
-        return f"{self.prop}{suffix} {value}"
-    
-    @staticmethod
-    def basic(fn: Callable[[Any],bool], msg: str):
-        class Child(DelayedInfo):
-            def sanitize(self, value):
-                assert fn(value), f"{self.name} {msg}"
-                return value
-        return Child
-
-
-class CanDelay(Stampable): 
-    _delayables: Tuple[DelayedInfo,...] = ()
-
-    def __init__(self, *values):
-        self._dv = tuple(self._delayables[i].laterOrSanitized(v) for i,v in enumerate(values))
-
-    def _doesDelay(self, i: int):
-        return self._dv[i] is Later._instance
-    
-    def stamp(self, index: int):
-        res: list[str] = []
-        s = index or ''
-        for i,v in enumerate(self._dv):
-            if v is not Later._instance:
-                res.append(self._delayables[i].stamp(s,v))
-        return '\n'.join(res)
-    
-    info = DelayedInfo # for ease of access
-
-
-class Delayed(Stampable):
-    def __init__(self, cls: Type[CanDelay], index: int, value) -> None:
-        super().__init__()
-        self.c = cls
-        self.i = index
-        self.d = cls._delayables[index]
-        self.v = self.d.sanitize(value)
-    
-    def compatible(self, coll: StampCollection):
-        v = coll.get(self.c)
-        if v is None:
-            raise TypeError(f"{self.d.name} definition requires also a {self.c.__name__} definition in the base or current dataset")
-        if coll.nextto(self.c):
-            assert v._doesDelay(self.i), f"Adjacent {self.c.__name__} does not delay {self.d.name}"
-    
-    def stamp(self, index: int):
-        return self.d.stamp(index or '', self.v)
-
-
-def delayer(index: int, T: Type, use: Type[Delayed] = Delayed):
-    @classmethod
-    def fn(cls, value: T):
-        return use(cls, index, value)
-    return fn
-
-
-class SKO:
-    """Single K Occupation"""
-    def __init__(self, k: Vec3D, *occupations: float) -> None:
-        self.k = k
-        self.occ = occupations
-
-
-def sectionTitle(index: int, name: str):
-    if index > 0:
-        return f"\n# DS{index} - {name}"
-    else:
-        return f"\n# {name}"
-    
-
-def decorate_IWD_method(fn):
-    def method(self: 'IndexedWithDefault', *args):
-        assert self._index is None, f"Multiple definitions for {type(self).__name__}"
-        return fn(self, *args)
-    return method
-
-
-class IndexedWithDefault(Stampable):
-    _default: str = ""
-    _prop: str = ""
-    
-    def __init__(self) -> None:
-        super().__init__()
-        self._index: int|None = None
-        self._extra: dict[str, Any] = {}
-    
-    def __init_subclass__(cls, default: str, prop: str = "") -> None:
-        super().__init_subclass__()
-        cls._prop = prop
-        if not callable(getattr(cls, default, 0)): # 0 is not callable
-            raise AttributeError(f"Property {default} of {cls.__name__} is not callable")
-        for (name,method) in cls.__dict__.items():
-            if callable(method) and not hasattr(IndexedWithDefault, name):
-                setattr(cls, name, decorate_IWD_method(method))
-    
-    def stamp(self, index: int):
-        s = index or ''
-        if self._index is None:
-            getattr(self,self._default)()
-        res = f"{self._prop}{s} {self._index}"
-        extra = '\n'.join(f"{k}{s} {v}" for (k,v) in self._extra.items())
-        if len(extra) > 0:
-            res += '\n' + extra
-        return res
-
-
-def _pos_int(v) -> TypeGuard[int]:
-    return type(v) is int and v > 0
-
-
-def _pos0_int(v) -> TypeGuard[int]:
-    return type(v) is int and v >= 0
-
-
-def _pos_num(v) -> TypeGuard[float|int]:
-    return type(v) is float or type(v) is int and v > 0
-
-
-def _pos0_num(v) -> TypeGuard[float|int]:
+from typing import TypeVar, Type, Tuple, Callable, Any, TypeGuard
+
+
+__all__ = ["Vec3D"]
+
+
+class Singleton(object):
+    _instance = None
+    def __new__(cls):
+        if cls._instance is None:
+            cls._instance = object.__new__(cls)
+        return cls._instance
+    
+    @classmethod
+    def eq(cls, value):
+        return type(value) is cls or value is cls
+
+
+class Vec3D:
+    def __init__(self, x: float, y: float, z: float) -> None:
+        self.x = x
+        self.y = y
+        self.z = z
+    
+    def __str__(self) -> str:
+        return "{} {} {}".format(self.x, self.y, self.z)
+    
+    @staticmethod
+    def uniform(v: float = 1.0):
+        return Vec3D(v,v,v)
+    
+    @staticmethod
+    def zero():
+        return Vec3D(0,0,0)
+
+ 
+S = TypeVar("S", bound="Stampable")
+
+class StampCollection:
+    def __init__(self, siblings: 'dict[type,Stampable]', base: 'dict[type,Stampable]') -> None:
+        self._s = siblings
+        self._b = base
+    
+    def get(self, t: Type[S]) -> S | None:
+        s = self._s.get(t);
+        if s is None:
+            s = self._b.get(t)
+        return s # type: ignore
+    
+    def nextto(self, t: Type['Stampable']):
+        return t in self._s
+
+
+class Stampable:
+    def stamp(self, index: int):
+        raise NotImplementedError(f"{type(self).__name__} has not implemented stamp")
+    
+    def compatible(self, coll: 'StampCollection'):
+        pass
+    
+    def __str__(self):
+        return self.stamp(0)
+
+
+class OneLineStamp(Stampable):
+    name = ''
+    
+    def __init__(self, value, suffix: str = '') -> None:
+        super().__init__()
+        self.value = value
+        self.suffix = suffix
+
+    def stamp(self, index: int):
+        t = type(self)
+        return f"{t.name}{self.suffix}{index or ''} {self.value}"
+
+
+class Later(Singleton):
+    pass
+
+
+class DelayedInfo:
+    def __init__(self, prop: str, name: str) -> None:
+        self.prop = prop
+        self.name = name
+
+    def sanitize(self, value):
+        raise NotImplementedError()
+    
+    def laterOrSanitized(self, value):
+        return value if value is Later._instance else self.sanitize(value)
+    
+    def stamp(self, suffix, value):
+        return f"{self.prop}{suffix} {value}"
+    
+    @staticmethod
+    def basic(fn: Callable[[Any],bool], msg: str):
+        class Child(DelayedInfo):
+            def sanitize(self, value):
+                assert fn(value), f"{self.name} {msg}"
+                return value
+        return Child
+
+
+class CanDelay(Stampable): 
+    _delayables: Tuple[DelayedInfo,...] = ()
+
+    def __init__(self, *values):
+        self._dv = tuple(self._delayables[i].laterOrSanitized(v) for i,v in enumerate(values))
+
+    def _doesDelay(self, i: int):
+        return self._dv[i] is Later._instance
+    
+    def stamp(self, index: int):
+        res: list[str] = []
+        s = index or ''
+        for i,v in enumerate(self._dv):
+            if v is not Later._instance:
+                res.append(self._delayables[i].stamp(s,v))
+        return '\n'.join(res)
+    
+    info = DelayedInfo # for ease of access
+
+
+class Delayed(Stampable):
+    def __init__(self, cls: Type[CanDelay], index: int, value) -> None:
+        super().__init__()
+        self.c = cls
+        self.i = index
+        self.d = cls._delayables[index]
+        self.v = self.d.sanitize(value)
+    
+    def compatible(self, coll: StampCollection):
+        v = coll.get(self.c)
+        if v is None:
+            raise TypeError(f"{self.d.name} definition requires also a {self.c.__name__} definition in the base or current dataset")
+        if coll.nextto(self.c):
+            assert v._doesDelay(self.i), f"Adjacent {self.c.__name__} does not delay {self.d.name}"
+    
+    def stamp(self, index: int):
+        return self.d.stamp(index or '', self.v)
+
+
+def delayer(index: int, T: Type, use: Type[Delayed] = Delayed):
+    @classmethod
+    def fn(cls, value: T):
+        return use(cls, index, value)
+    return fn
+
+
+class SKO:
+    """Single K Occupation"""
+    def __init__(self, k: Vec3D, *occupations: float) -> None:
+        self.k = k
+        self.occ = occupations
+
+
+def sectionTitle(index: int, name: str):
+    if index > 0:
+        return f"\n# DS{index} - {name}"
+    else:
+        return f"\n# {name}"
+    
+
+def decorate_IWD_method(fn):
+    def method(self: 'IndexedWithDefault', *args):
+        assert self._index is None, f"Multiple definitions for {type(self).__name__}"
+        return fn(self, *args)
+    return method
+
+
+class IndexedWithDefault(Stampable):
+    _default: str = ""
+    _prop: str = ""
+    
+    def __init__(self) -> None:
+        super().__init__()
+        self._index: int|None = None
+        self._extra: dict[str, Any] = {}
+    
+    def __init_subclass__(cls, default: str, prop: str = "") -> None:
+        super().__init_subclass__()
+        cls._prop = prop
+        if not callable(getattr(cls, default, 0)): # 0 is not callable
+            raise AttributeError(f"Property {default} of {cls.__name__} is not callable")
+        for (name,method) in cls.__dict__.items():
+            if callable(method) and not hasattr(IndexedWithDefault, name):
+                setattr(cls, name, decorate_IWD_method(method))
+    
+    def stamp(self, index: int):
+        s = index or ''
+        if self._index is None:
+            getattr(self,self._default)()
+        res = f"{self._prop}{s} {self._index}"
+        extra = '\n'.join(f"{k}{s} {v}" for (k,v) in self._extra.items())
+        if len(extra) > 0:
+            res += '\n' + extra
+        return res
+
+
+def _pos_int(v) -> TypeGuard[int]:
+    return type(v) is int and v > 0
+
+
+def _pos0_int(v) -> TypeGuard[int]:
+    return type(v) is int and v >= 0
+
+
+def _pos_num(v) -> TypeGuard[float|int]:
+    return type(v) is float or type(v) is int and v > 0
+
+
+def _pos0_num(v) -> TypeGuard[float|int]:
     return type(v) is float or type(v) is int and v >= 0
```

### Comparing `pynabi-0.1.1/src/pynabi/_dataset.py` & `pynabi-0.1.2/src/pynabi/_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,257 +1,272 @@
-from typing import Union, List, Iterable, Literal, Callable, Optional, Type, TypeVar
-from ._common import Stampable, Singleton, Delayed, StampCollection
-from .crystal import AtomBasis, Atom
-from inspect import stack
-
-from .occupation import _exclusives as _ex1
-from .calculation import _exclusives as _ex2
-from .kspace import _exclusives as _ex3
-
-_excl = [_ex1, _ex2, _ex3]
-
-
-__all__ = ["DataSet", "PreviousRun", "AbIn", "AbOut", "createAbi", "append"]
-
-
-_RS = Union[Stampable,Iterable['_RS']]
-
-
-def splat(i: Iterable[_RS]) -> Iterable[Stampable]:
-    for v in i:
-        if isinstance(v,Stampable):
-            yield v
-        else:
-            try:
-                yield from splat(v)
-            except:
-                raise TypeError("Arguments provided to dataset must be DataSet stampables of iterables of them")
-
-
-class DataSet:
-    def __init__(self, *stampables: _RS) -> None:
-        self.index = 0
-        self.atoms: Union[AtomBasis,None] = None
-        self.stamps: list[Stampable] = []
-        self.map: dict[Type[Stampable], Stampable] = {}
-        self.delayeds = set()
-        self._append(stampables)
-            
-    def _append(self, *stampables: _RS):
-        for s in splat(stampables):
-            if not isinstance(s, Stampable):
-                raise TypeError(f"{s.__class__.__name__} is not a valid type for a dataset")
-            if isinstance(s, Delayed):
-                p = s.d.prop
-                if p in self.delayeds:
-                    raise ValueError(f"Multiple {s.d.name} definition are present")
-                self.delayeds.add(p)
-                self.stamps.append(s)
-            else:
-                t = type(s)
-                if t in self.map:
-                    raise ValueError(f"Multiple {s.__class__.__name__} given")
-                self.map[t] = s
-                if t is AtomBasis:
-                    self.atoms = s # type: ignore
-                else:
-                    self.stamps.append(s) # type: ignore
-        s = set(self.map.keys())
-        for excl in _excl:
-            inters = s.intersection(excl)
-            if len(inters) > 1:
-                raise ValueError(', '.join(c.__name__ for c in inters) + " are mutually incompatible: please specify only one of them") 
-    
-    def stamp(self, atompool: List[Atom]):
-        res: list[str] = []
-        if self.atoms is not None:
-            res.append(self.atoms.stamp(self.index, atompool))
-        for s in self.stamps:
-            res.append(s.stamp(self.index))
-        return '\n'.join(res)
-    
-T = TypeVar("T", bound=Iterable[DataSet])
-def append(what: _RS, to: T) -> T:
-    for d in to:
-        d._append(what)
-    return to
-
-
-class PreviousRun(Singleton):
-    pass
-
-
-def _AbInMethod(prop: str, sel: Literal[0,1,2] = 0):
-    def method(self: 'AbIn', value: Union['DataSet', str, PreviousRun]): 
-        if type(value) is str:
-            assert sel != 0, f"{method._name} cannot be read from a file"
-        else:
-            assert sel < 2, f"{method._name} can only be read from a file"
-        self._d[method] = value
-        return self
-    method._name = ""
-    method._prop = prop
-    return method
-
-
-class AbIn(Stampable):
-    def __init__(self, prefix: Optional[str] = None):
-        self._p = prefix
-        self._d: dict[Callable, Union['DataSet', str, PreviousRun]] = dict()
-        self._ppd: Optional[str] = None
-    
-    def stamp(self, index: int):
-        res: list[str] = []
-        if self._ppd is not None:
-            res.append(f"pp_dirpath{index or ''} \"{self._ppd}\"")
-        if self._p is not None:
-            res.append(f"indata_prefix{index or ''} \"{self._p}\"")
-        body = '\n'.join(AbIn._print_helper(k,v,index) for k, v in self._d.items())
-        if len(body) > 0:
-            res.append(body)
-        return '\n'.join(res);
-    
-    @staticmethod
-    def _print_helper(m: Callable, v: Union['DataSet', str, PreviousRun], i: int):
-        if type(v) is DataSet:
-            assert v.index < i, f"Cannot read {m._name} for {i}-th dataset from the {v.index}-th dataset"
-            return f"get{m._prop}{i or ''} {v.index}"
-        elif type(v) is PreviousRun:
-            return f"ird{m._prop}{i or ''} 1"
-        else:
-            return f"get{m._prop}_filepath{i or ''} \"{v}\""
-    
-    def PseudoPotentials(self, path: str):
-        self._ppd = path;
-        return self
-            
-    FirstOrderDensity = _AbInMethod("1den")
-    FirstOrderWavefunction = _AbInMethod("1wf")
-    BetheSalpeterCouplingBlock = _AbInMethod("bscoup")
-    BetheSalpeterEigenstates = _AbInMethod("bseig")
-    BetheSalpeterResonantBlock = _AbInMethod("bsreso")
-    DDB = _AbInMethod("ddb",1)
-    DDKWavefunctions = _AbInMethod("ddk")
-    dE = _AbInMethod("delfd")
-    ElectronDensity = _AbInMethod("den",1)
-    dkdE = _AbInMethod("dkde")
-    dkdk = _AbInMethod("dkdk")
-    PotentialDerivative = _AbInMethod("dvdb",1)
-    EffectiveMasses = _AbInMethod("efmas")
-    HaydockRestartFile = _AbInMethod("haydock")
-    OccupationNumbers = _AbInMethod("occ")
-    KSPotential = _AbInMethod("pot",2)
-    QuasiParticleStructure = _AbInMethod("qps")
-    Screening = _AbInMethod("scr",1)
-    SIGEPH = _AbInMethod("sigeph",2)
-    Susceptibility = _AbInMethod("suscep")
-    WavefunctionsK = _AbInMethod("wfk",1)
-    FineWavefunctionsK = _AbInMethod("wfkfine",2)
-    WavefunctionsQ = _AbInMethod("wfq",1)
-
-
-for k,v in AbIn.__dict__.items():
-    if callable(v) and hasattr(v,"_name"):
-        v._name = k
-
-
-def _os(name: str):
-    def method(self: 'AbOut', flag: bool = True):
-        self._d[name] = int(flag)
-        return self
-    return method
-
-
-def _om(name: str, max: int, min: int = 0):
-    def method(self: 'AbOut', value: int):
-        assert type(value) is int and min <= value <= max, f"Value of {stack()[0][3]} must be integer between {min} and {max}"
-        self._d[name] = value
-        return self
-    return method
-
-
-class AbOut(Stampable):
-    def __init__(self, prefix: Union[str,None] = None):
-        self._p = prefix
-        self._d: dict[str, int] = {}
-
-    def stamp(self, index: int):
-        s = index or ''
-        body = '\n'.join(f"prt{k}{s} {v}" for k,v in self._d.items())
-        if self._p is None:
-            return body
-        elif len(body) == 0:
-            return f"outdata_prefix \"{self._p}\""
-        else:
-            return f"outdata_prefix \"{self._p}\"\n{body}"
-
-    PotentialAndDensity1D = _os("1dm")
-    CheckPoint = _os("chkprdm")
-    ElectronDensity = _os("den")
-    DensityOfStates = _om("dos", 5)
-    MResolvedPartialDOS = _os("dosm")
-    EigenEnergies = _os("eig")
-    ElectronLocalizedFunction = _os("elf")
-    FermiSurface = _os("surf")
-    ElectronDensityGradient = _os("gden")
-    GeometryAnalysis = _os("geo")
-    MatrixGKK = _os("gkk")
-    GSR = _os("gsr")
-    KleynmanBylanderFormFactors = _os("kbff")
-    KineticEnergyDensity = _os("kden")
-    KPointsSets = _os("kpt")
-    ElectronDensityLaplacian = _os("lden")
-    Potential = _os("pot")
-    PSPS = _os("psps")
-    SpinCurrentDensity = _os("spcur")
-    STMDensity = _os("stm")
-    Susceptibility = _os("suscep")
-    CoulombPotential = _os("vclmb")
-    HartreePotential = _os("vha")
-    HartreeANdExchangeCorrelationPotential = _os("vhxc")
-    Volume = _om("vol", 11, -10)
-    ImagesVolume = _os("volimg")
-    LocalPseudoPotential = _os("vpsp")
-    ExchangeCorrelationPotential = _os("vxc")
-    UseWanTInterface = _om("want", 3)
-    Wavefunction = _om("wf", 2, -1)
-    FullMeshWavefunction = _os("wf_full")
-    XML = _os("xml")
-
-
-def createAbi(setup: Union[DataSet,None], *datasets: DataSet) -> str:
-    """Given one optional base dataset and multiple subsequent datasets, it constructs the abinit input file and returns it as a string"""
-    n = len(datasets)
-    if setup is None:
-        if n == 0:
-            return ''
-        elif n == 1:
-            return createAbi(datasets[0])
-        else:
-            setup = DataSet()
-    elif len(datasets) == 1:
-        raise ValueError("Cannot use a single dataset")
-    
-    res: list[str] = [f"ndtset {len(datasets)}\n"]
-
-    atomSet = set() if setup.atoms is None else set(setup.atoms.getAtoms())
-    initialAtomCount = len(atomSet)
-    base_coll = {} if setup is None else setup.map
-    for (i,d) in enumerate(datasets):
-        d.index = i+1
-        coll = StampCollection(d.map, base_coll)
-        for s in d.stamps:
-            s.compatible(coll)
-        if d.atoms is not None:
-            atomSet = atomSet.union(d.atoms.getAtoms())
-        elif initialAtomCount == 0:
-            raise ValueError(f"All datasets (in particular the {i+1}-th one) must define the atom basis since no common one was defined")
-    
-    atomPool = list(atomSet)
-    res.append(Atom.poolstr(atomPool))
-    res.append("\n# Common DataSet")
-    res.append(setup.stamp(atomPool))
-    for d in datasets:
-        res.append(f"\n# DataSet {d.index}")
-        res.append(d.stamp(atomPool))
-    return '\n'.join(res)
-    
+from typing import Union, List, Iterable, Literal, Callable, Optional, Type, TypeVar
+from ._common import Stampable, Singleton, Delayed, StampCollection
+from .crystal import AtomBasis, Atom
+from .calculation import NonSelfConsistentCalc, Tolerance
+from inspect import stack
+
+from .occupation import _exclusives as _ex1
+from .calculation import _exclusives as _ex2
+from .kspace import _exclusives as _ex3
+
+_excl = [_ex1, _ex2, _ex3]
+
+
+__all__ = ["DataSet", "PreviousRun", "AbIn", "AbOut", "createAbi", "append"]
+
+
+_RS = Union[Stampable,Iterable['_RS']]
+
+
+def splat(i: Iterable[_RS]) -> Iterable[Stampable]:
+    for v in i:
+        if isinstance(v,Stampable):
+            yield v
+        else:
+            try:
+                yield from splat(v)
+            except:
+                raise TypeError("Arguments provided to dataset must be DataSet stampables of iterables of them")
+
+
+class DataSet:
+    def __init__(self, *stampables: _RS) -> None:
+        self.index = 0
+        self.atoms: Union[AtomBasis,None] = None
+        self.stamps: list[Stampable] = []
+        self.map: dict[Type[Stampable], Stampable] = {}
+        self.delayeds = set()
+        self._append(stampables)
+            
+    def _append(self, *stampables: _RS):
+        for s in splat(stampables):
+            if not isinstance(s, Stampable):
+                raise TypeError(f"{s.__class__.__name__} is not a valid type for a dataset")
+            if isinstance(s, Delayed):
+                p = s.d.prop
+                if p in self.delayeds:
+                    raise ValueError(f"Multiple {s.d.name} definition are present")
+                self.delayeds.add(p)
+                self.stamps.append(s)
+            else:
+                t = type(s)
+                if t in self.map:
+                    raise ValueError(f"Multiple {s.__class__.__name__} given")
+                self.map[t] = s
+                if t is AtomBasis:
+                    self.atoms = s # type: ignore
+                else:
+                    self.stamps.append(s) # type: ignore
+        s = set(self.map.keys())
+        for excl in _excl:
+            inters = s.intersection(excl)
+            if len(inters) > 1:
+                raise ValueError(', '.join(c.__name__ for c in inters) + " are mutually incompatible: please specify only one of them") 
+    
+    def stamp(self, atompool: List[Atom]):
+        res: list[str] = []
+        if self.atoms is not None:
+            res.append(self.atoms.stamp(self.index, atompool))
+        for s in self.stamps:
+            res.append(s.stamp(self.index))
+        return '\n'.join(res)
+    
+T = TypeVar("T", bound=Iterable[DataSet])
+def append(what: _RS, to: T) -> T:
+    for d in to:
+        d._append(what)
+    return to
+
+
+class PreviousRun(Singleton):
+    pass
+
+
+def _AbInMethod(prop: str, sel: Literal[0,1,2] = 0):
+    def method(self: 'AbIn', value: Union['DataSet', str, PreviousRun]): 
+        if type(value) is str:
+            assert sel != 0, f"{method._name} cannot be read from a file"
+        else:
+            assert sel < 2, f"{method._name} can only be read from a file"
+        self._d[method] = value
+        return self
+    method._name = ""
+    method._prop = prop
+    return method
+
+
+class AbIn(Stampable):
+    def __init__(self, prefix: Optional[str] = None):
+        self._p = prefix
+        self._d: dict[Callable, Union['DataSet', str, PreviousRun]] = dict()
+        self._ppd: Optional[str] = None
+    
+    def stamp(self, index: int):
+        res: list[str] = []
+        if self._ppd is not None:
+            res.append(f"pp_dirpath{index or ''} \"{self._ppd}\"")
+        if self._p is not None:
+            res.append(f"indata_prefix{index or ''} \"{self._p}\"")
+        body = '\n'.join(AbIn._print_helper(k,v,index) for k, v in self._d.items())
+        if len(body) > 0:
+            res.append(body)
+        return '\n'.join(res);
+    
+    @staticmethod
+    def _print_helper(m: Callable, v: Union['DataSet', str, PreviousRun], i: int):
+        if type(v) is DataSet:
+            assert v.index < i, f"Cannot read {m._name} for {i}-th dataset from the {v.index}-th dataset"
+            return f"get{m._prop}{i or ''} {v.index}"
+        elif type(v) is PreviousRun:
+            return f"ird{m._prop}{i or ''} 1"
+        else:
+            return f"get{m._prop}_filepath{i or ''} \"{v}\""
+    
+    def PseudoPotentials(self, directory_path: str):
+        self._ppd = directory_path;
+        return self
+            
+    FirstOrderDensity = _AbInMethod("1den")
+    FirstOrderWavefunction = _AbInMethod("1wf")
+    BetheSalpeterCouplingBlock = _AbInMethod("bscoup")
+    BetheSalpeterEigenstates = _AbInMethod("bseig")
+    BetheSalpeterResonantBlock = _AbInMethod("bsreso")
+    DDB = _AbInMethod("ddb",1)
+    DDKWavefunctions = _AbInMethod("ddk")
+    dE = _AbInMethod("delfd")
+    ElectronDensity = _AbInMethod("den",1)
+    dkdE = _AbInMethod("dkde")
+    dkdk = _AbInMethod("dkdk")
+    PotentialDerivative = _AbInMethod("dvdb",1)
+    EffectiveMasses = _AbInMethod("efmas")
+    HaydockRestartFile = _AbInMethod("haydock")
+    OccupationNumbers = _AbInMethod("occ")
+    KSPotential = _AbInMethod("pot",2)
+    QuasiParticleStructure = _AbInMethod("qps")
+    Screening = _AbInMethod("scr",1)
+    SIGEPH = _AbInMethod("sigeph",2)
+    Susceptibility = _AbInMethod("suscep")
+    WavefunctionsK = _AbInMethod("wfk",1)
+    FineWavefunctionsK = _AbInMethod("wfkfine",2)
+    WavefunctionsQ = _AbInMethod("wfq",1)
+
+
+for k,v in AbIn.__dict__.items():
+    if callable(v) and hasattr(v,"_name"):
+        v._name = k
+
+
+def _os(name: str):
+    def method(self: 'AbOut', flag: bool = True):
+        self._d[name] = int(flag)
+        return self
+    return method
+
+
+def _om(name: str, max: int, min: int = 0):
+    def method(self: 'AbOut', value: int):
+        assert type(value) is int and min <= value <= max, f"Value of {stack()[0][3]} must be integer between {min} and {max}"
+        self._d[name] = value
+        return self
+    return method
+
+
+class AbOut(Stampable):
+    def __init__(self, prefix: Union[str,None] = None):
+        self._p = prefix
+        self._d: dict[str, int] = {}
+
+    def stamp(self, index: int):
+        s = index or ''
+        body = '\n'.join(f"prt{k}{s} {v}" for k,v in self._d.items())
+        if self._p is None:
+            return body
+        elif len(body) == 0:
+            return f"outdata_prefix \"{self._p}\""
+        else:
+            return f"outdata_prefix \"{self._p}\"\n{body}"
+
+    PotentialAndDensity1D = _os("1dm")
+    CheckPoint = _os("chkprdm")
+    ElectronDensity = _os("den")
+    DensityOfStates = _om("dos", 5)
+    MResolvedPartialDOS = _os("dosm")
+    EigenEnergies = _os("eig")
+    ElectronLocalizedFunction = _os("elf")
+    FermiSurface = _os("fsurf")
+    ElectronDensityGradient = _os("gden")
+    GeometryAnalysis = _os("geo")
+    MatrixGKK = _os("gkk")
+    GSR = _os("gsr")
+    KleynmanBylanderFormFactors = _os("kbff")
+    KineticEnergyDensity = _os("kden")
+    KPointsSets = _os("kpt")
+    ElectronDensityLaplacian = _os("lden")
+    Potential = _os("pot")
+    PSPS = _os("psps")
+    SpinCurrentDensity = _os("spcur")
+    STMDensity = _os("stm")
+    Susceptibility = _os("suscep")
+    CoulombPotential = _os("vclmb")
+    HartreePotential = _os("vha")
+    HartreeANdExchangeCorrelationPotential = _os("vhxc")
+    Volume = _om("vol", 11, -10)
+    ImagesVolume = _os("volimg")
+    LocalPseudoPotential = _os("vpsp")
+    ExchangeCorrelationPotential = _os("vxc")
+    UseWanTInterface = _om("want", 3)
+    Wavefunction = _om("wf", 2, -1)
+    FullMeshWavefunction = _os("wf_full")
+    XML = _os("xml")
+
+
+def createAbi(setup: Union[DataSet,None], *datasets: DataSet) -> str:
+    """Given one optional base dataset and multiple subsequent datasets, it constructs the abinit input file and returns it as a string"""
+    n = len(datasets)
+    if n == 1 and setup is None:
+        raise ValueError("Cannot use a single dataset")
+     
+    res: list[str] = [f"ndtset {n}\n"]
+    atomSet = set()
+    base_coll = {} if setup is None else setup.map
+
+    # check base dataset
+    no_base_tol = True
+    if setup is not None:
+        coll = StampCollection(setup.map, {});
+        for s in setup.stamps:
+            s.compatible(coll)
+        if setup.atoms is not None:
+            atomSet = set(setup.atoms.getAtoms())
+        # check that user sets tolerance when no SCF is specified
+        no_base_tol = setup.map.get(Tolerance) is None and setup.map.get(NonSelfConsistentCalc) is None
+        if n == 0 and no_base_tol:
+            raise ValueError("The dataset must specify a Tolerance, since Abinit will implictly assume a SCF calculation")
+
+    # check compatibility
+    initialAtomCount = len(atomSet)
+    for (i,d) in enumerate(datasets):
+        d.index = i+1
+        coll = StampCollection(d.map, base_coll)
+        for s in d.stamps:
+            s.compatible(coll)
+        if d.atoms is not None:
+            atomSet = atomSet.union(d.atoms.getAtoms())
+        elif initialAtomCount == 0:
+            raise ValueError(f"All datasets (in particular the {i+1}-th one) must define the atom basis since no common one was defined")
+    
+    # if no tolerance on base set
+    if no_base_tol:
+        for ds in datasets:
+            if ds.map.get(Tolerance) is None and ds.map.get(NonSelfConsistentCalc) is None:
+                raise ValueError("All numbered datasets without explicit Non SCF calculation must specify a Tolerance, since Abinit will implicitly assume a SFC calculation")
+
+    atomPool = list(atomSet)
+    res.append(Atom.poolstr(atomPool))
+    if setup is not None:
+        res.append("\n# Common DataSet")
+        res.append(setup.stamp(atomPool))
+    for d in datasets:
+        res.append(f"\n# DataSet {d.index}")
+        res.append(d.stamp(atomPool))
+    return '\n'.join(res)
+
```

### Comparing `pynabi-0.1.1/src/pynabi/calculation.py` & `pynabi-0.1.2/src/pynabi/calculation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,109 @@
-from typing import Literal as _L, Union as _U
-from ._common import Stampable as _S, _pos_int, OneLineStamp as _OLS, IndexedWithDefault as _IWD
-from .units import Energy as _En
-from enum import Enum as _E
-
-
-__all__ = ["SCFDirectMinimization", "SCFMixing", "NonSelfConsistentCalc", "ToleranceOn", "EnergyCutoff", "MaxSteps"]
-
-
-class SCFDirectMinimization(_S):
-    def __init__(self) -> None:
-        super().__init__()
-    
-    def stamp(self, index: int):
-        return f"iscf{index or ''} 0"
-
-
-class SCFMixing(_IWD, default="Pulay", prop="iscf"):
-    """Usual ground state (GS) calculations or for structural relaxations, where the potential has to be determined self-consistently"""
-
-    def __init__(self, density: bool = False) -> None:
-        super().__init__()
-        self._den = density
-    
-    def Simple(self):
-        self._index = 2 + 10*int(self._den)
-        return self
-
-    def Anderson(self, onPrevious: bool = False):
-        """Anderson mixing of the potential/density.\n
-        If `onPrevious` is True, the mixing is based on the two previous iterations"""
-        self._index = (4 if onPrevious else 3) + 10*int(self._den)
-        return self
-
-    def CGBased(self, alt: bool = False):
-        """CG based on the minimum of the energy with respect to the potential/density.\n
-        If `alt` is True, it uses an alternative implementation (still in development)"""
-        self._index = (6 if alt else 5) + 10*int(self._den)
-        return self
-
-    def Pulay(self, iterations: int = 7):
-        """Pulay mixing of the potential/density based on the `iterations` previous iterations"""
-        assert _pos_int(iterations), "Number of iterations used in Pulay mixing must be a positive integer"
-        self._index = 7 + 10*int(self._den)
-        self._extra = { "npulayit": iterations }
-        return self
-
-
-class NonSelfConsistentCalc(_S):
-    def __init__(self, i: _L[-1,-2,-3] = -2) -> None:
-        assert type(i) is int and -3 <= i <= -1, "Non self consistend calculation index must be -1, -2, or -3"
-        self._i = i
-    
-    def stamp(self, index: int):
-        return f"iscf{index or ''} {self._i}"
-    
-
-class ToleranceOn(_E):
-    EnergyDifference = "dfe"
-    ForceDifference = "dff"
-    ForceRelativeDifference = "drff"
-    PotentialResidual = "vrs"
-    WavefunctionSquaredResidual = "wfr"
-
-    def __call__(self, value: float):
-        return Tolerance(value, self.value)
-
-
-class Tolerance(_OLS):
-    """Do not use this class directly: prefer ToleranceOn"""
-    name = "tol"
-
-
-class EnergyCutoff(_OLS):
-    """Used to define the kinetic energy cutoff which controls the number of planewaves at given k point. The allowed plane waves are those with kinetic energy lower than ecut, which translates to the following constraint on the planewave vector G in reciprocal space"""
-    name = "ecut"
-    def __init__(self, value: _U[float,_En]) -> None:
-        e = _En.sanitize(value);
-        assert e._v > 0, "cutoff energy must be positive"
-        super().__init__(str(e))
-
-
-class MaxSteps(_OLS):
-    """The maximum number of cycles (or “iterations”) in a SCF or non-SCF run. 
-    
-    Full convergence from random numbers is usually achieved in 12-20 SCF iterations. Each can take from minutes to hours. In certain difficult cases, usually related to a small or zero band gap or magnetism, convergence performance may be much worse
-    
-    For non-self-consistent runs, it governs the number of cycles of convergence for the wavefunctions for a fixed density and Hamiltonian.
-
-    NOTE that a choice of nstep = 0 is permitted; this will either read wavefunctions from disk and compute the density, the total energy and stop, or else will initialize randomly the wavefunctions and compute the resulting density and total energy. This is provided for testing purposes.
-    """
-
-    name = "nstep"
-    def __init__(self, value: int) -> None:
-        assert type(value) is int and value >= 0, "Number of steps must be an integer greater than or equal to 0"
-        super().__init__(value)
-
-
+from typing import Literal as _L, Union as _U
+
+from pynabi._common import StampCollection
+from ._common import Stampable as _S, _pos_int, OneLineStamp as _OLS, IndexedWithDefault as _IWD
+from .units import Energy as _En
+from enum import Enum as _E
+
+
+__all__ = ["SCFDirectMinimization", "SCFMixing", "NonSelfConsistentCalc", "ToleranceOn", "EnergyCutoff", "MaxSteps"]
+
+
+class SCFDirectMinimization(_S):
+    def __init__(self) -> None:
+        super().__init__()
+    
+    def stamp(self, index: int):
+        return f"iscf{index or ''} 0"
+    
+    def compatible(self, coll: StampCollection):
+        tol = coll.get(Tolerance)
+        assert tol is not None, "SCF direct minimization requires one tolerance to be spcified"
+
+
+class SCFMixing(_IWD, default="Pulay", prop="iscf"):
+    """Usual ground state (GS) calculations or for structural relaxations, where the potential has to be determined self-consistently"""
+
+    def __init__(self, density: bool = False) -> None:
+        super().__init__()
+        self._den = density
+    
+    def Simple(self):
+        self._index = 2 + 10*int(self._den)
+        return self
+
+    def Anderson(self, onPrevious: bool = False):
+        """Anderson mixing of the potential/density.\n
+        If `onPrevious` is True, the mixing is based on the two previous iterations"""
+        self._index = (4 if onPrevious else 3) + 10*int(self._den)
+        return self
+
+    def CGBased(self, alt: bool = False):
+        """CG based on the minimum of the energy with respect to the potential/density.\n
+        If `alt` is True, it uses an alternative implementation (still in development)"""
+        self._index = (6 if alt else 5) + 10*int(self._den)
+        return self
+
+    def Pulay(self, iterations: int = 7):
+        """Pulay mixing of the potential/density based on the `iterations` previous iterations"""
+        assert _pos_int(iterations), "Number of iterations used in Pulay mixing must be a positive integer"
+        self._index = 7 + 10*int(self._den)
+        self._extra = { "npulayit": iterations }
+        return self
+    
+    def compatible(self, coll: StampCollection):
+        tol = coll.get(Tolerance)
+        assert tol is not None, "SCF mixing requires one tolerance to be specified"
+
+
+class NonSelfConsistentCalc(_S):
+    def __init__(self, i: _L[-1,-2,-3] = -2) -> None:
+        assert type(i) is int and -3 <= i <= -1, "Non self consistend calculation index must be -1, -2, or -3"
+        self._i = i
+    
+    def stamp(self, index: int):
+        return f"iscf{index or ''} {self._i}"
+    
+
+class ToleranceOn(_E):
+    EnergyDifference = "dfe"
+    ForceDifference = "dff"
+    ForceRelativeDifference = "drff"
+    PotentialResidual = "vrs"
+    WavefunctionSquaredResidual = "wfr"
+
+    def __call__(self, value: float):
+        return Tolerance(value, self.value)
+
+
+class Tolerance(_OLS):
+    """Do not use this class directly: prefer ToleranceOn"""
+    name = "tol"
+
+
+class EnergyCutoff(_OLS):
+    """Used to define the kinetic energy cutoff which controls the number of planewaves at given k point. The allowed plane waves are those with kinetic energy lower than ecut, which translates to the following constraint on the planewave vector G in reciprocal space"""
+    name = "ecut"
+    def __init__(self, value: _U[float,_En]) -> None:
+        e = _En.sanitize(value);
+        assert e._v > 0, "cutoff energy must be positive"
+        super().__init__(str(e))
+
+
+class MaxSteps(_OLS):
+    """The maximum number of cycles (or “iterations”) in a SCF or non-SCF run. 
+    
+    Full convergence from random numbers is usually achieved in 12-20 SCF iterations. Each can take from minutes to hours. In certain difficult cases, usually related to a small or zero band gap or magnetism, convergence performance may be much worse
+    
+    For non-self-consistent runs, it governs the number of cycles of convergence for the wavefunctions for a fixed density and Hamiltonian.
+
+    NOTE that a choice of nstep = 0 is permitted; this will either read wavefunctions from disk and compute the density, the total energy and stop, or else will initialize randomly the wavefunctions and compute the resulting density and total energy. This is provided for testing purposes.
+    """
+
+    name = "nstep"
+    def __init__(self, value: int) -> None:
+        assert type(value) is int and value >= 0, "Number of steps must be an integer greater than or equal to 0"
+        super().__init__(value)
+
+
 _exclusives = set((SCFMixing, SCFDirectMinimization, NonSelfConsistentCalc))
```

### Comparing `pynabi-0.1.1/src/pynabi/crystal.py` & `pynabi-0.1.2/src/pynabi/crystal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,279 +1,279 @@
-from ._common import Vec3D as _V, Stampable as _S, _pos_int
-from typing import Optional as _O, Union as _U
-from .units import Length as _L, Pos3D as _P
-
-__all__ = ["Atom", "AtomBasis", "Lattice", "HCP", "CsClLike", "RockSaltLike", "FluoriteLike", "ZincBlendeLike", "HCP", "WurtziteLike", "NiAsLike"]
-
-_atom_symbols = ["H","He","Li","Be","B","C","N","O","F","Ne","Na","Mg","Al","Si","P","S","Cl","Ar","K","Ca","Sc","Ti","V","Cr","Mn","Fe","Co","Ni","Cu","Zn","Ga","Ge","As","Se","Br","Kr","Rb","Sr","Y","Zr","Nb","Mo","Tc","Ru","Rh","Pd","Ag","Cd","In","Sn","Sb","Te","I","Xe","Cs","Ba","La","Ce","Pr","Nd","Pm","Sm","Eu","Gd","Tb","Dy","Ho","Er","Tm","Yb","Lu","Hf","Ta","W","Re","Os","Ir","Pt","Au","Hg","Tl","Pb","Bi","Po","At","Rn","Fr","Ra","Ac","Th","Pa","U ","Np","Pu","Am","Cm","Bk","Cf","Es","F","Md","No","Lr","Rf","Db","Sg","Bh","Hs","Mt","Ds","Rg","Cn","Nh","Fl","Mc","Lv","Ts","Og"]
-
-class Atom:
-    def __init__(self, Z: int, file: str):
-        assert _pos_int(Z), "Atomic number must be a positive integer"
-        self.num = Z
-        self.file = file
-        assert self.file.find(",") == -1, "File name cannot contain ','"
-    
-    def __str__(self) -> str:
-        return f"{_atom_symbols[self.num-1]} atom (located at {self.file})"
-    
-    # def __eq__(self, __value: object) -> bool:
-    #     return (self is __value) or (type(__value) is Atom and __value.num == self.num and __value.file == self.file)
-
-    @staticmethod
-    def of(name: str):
-        """Constructs an atom using default filenaming
-        
-        returns Atom(Z of element, element name + '.psp8')
-        """
-        try:
-            Z = _atom_symbols.index(name) + 1;
-            return Atom(Z, name + '.psp8')
-        except:
-            raise ValueError(name + " is not a valid atom type")
-    
-    @staticmethod
-    def poolstr(atoms: 'list[Atom]'):
-        return f"""# Atoms definition
-ntypat {len(atoms)}
-znucl {' '.join(str(a.num) for a in atoms)}
-pseudos \"{', '.join(a.file for a in atoms)}\""""
-
-
-class AtomBasis(_S):
-    def __init__(self, *atoms: 'tuple[Atom,_V]', cartesian: bool = False) -> None:
-        """Construct an atom basis given a sequence of tuples containing an atom and a position (Vec3D)\n
-        If `cartesian` is True, the coordinates of the atoms' position are cartesian instead of reduced."""
-        assert len(atoms) > 0, "There must be at least one atom in basis"
-        self.atoms = atoms
-        self.cartesian = cartesian
-    
-    def add(self, atom: Atom, where: _V):
-        if type(self.atoms) is tuple:
-            self.atoms = list(self.atoms)
-        self.atoms.append((atom, where)) # type: ignore
-    
-    def getAtoms(self):
-        return (a[0] for a in self.atoms)
-    
-    def stamp(self, index: int, pool: 'list[Atom]'):
-        indexes = [pool.index(a[0]) for a in self.atoms]
-        suffix = str(index or '');
-        x_type = "xcart" if self.cartesian else "xred";
-        return f"""natoms{suffix} {len(indexes)}
-typeat{suffix} {' '.join(str(i+1) for i in indexes)}
-{x_type}{suffix} {'   '.join(str(a[1]) for a in self.atoms)}"""
-
-    @staticmethod
-    def ofOne(atom: Atom):
-        """Construct an atom basis with only one atom (placed at Vec3D(0,0,0))"""
-        return AtomBasis((atom, _V.zero()))
-
-
-def _2uni(v: _U[float,_L]):
-    t = type(v)
-    if t is _L:
-        return _P.uniform(v) # type: ignore
-    elif t is float:
-        return _V.uniform(v) # type: ignore
-    else:
-        raise TypeError(f"Lattice constant is of wrong value (got {t} instead of float or Length)")
-
-
-class Lattice(_S):
-    def __init__(self, **props):
-        """Do not use directly: prefer static methods like fromAngle, fromPrimitives"""
-        self._p = props
-
-    def stamp(self, index: int):
-        suffix = index if index > 0 else ''
-        return '\n'.join(f"{k}{suffix} {v}" for k,v in self._p.items())
-    
-    @staticmethod
-    def fromAngles(angles: _V, scaling: _U[_V,_P]):
-        """
-        Constructs lattice from angles [&alpha;, &beta;, &gamma;]\n
-        Scaling is defined per primitive vector (e.g. a is multiplied by scaling[0])
-
-        Angles are defined between vectors as follows:
-        | angle | from | to |
-        | :---: | :----------: | :-----------: |
-        | &alpha;(1) | b(2) | c(3) |
-        | &beta;(2) | a(1) | c(3) |
-        | &gamma;(3) | a(1) | b(2) |
-        """
-        assert type(angles) is _V, "Angles must be of type Vec3D"
-        return Lattice(acell=_P.sanitize(scaling), angdeg=angles)
-    
-    @staticmethod
-    def fromPrimitives(a: _V, b: _V, c: _V, scaling: _U[_V,_P]):
-        """
-        Construct lattice from primitives [a, b, c]\n
-        Scaling is applied to the cartesian axis
-        """
-        assert type(a) is _V and type(b) is _V and type(c) is _V, "Primitive vectors must be of type Vec3D"
-        return Lattice(scalecart=_P.sanitize(scaling), rprim=f"{a}   {b}   {c}")
-    
-    @staticmethod
-    def CUB(a: _U[float,_L]):
-        return Lattice.fromAngles(_V.uniform(90),_2uni(a))
-
-    @staticmethod
-    def BCC(a: _U[float,_L]):
-        return Lattice.fromPrimitives(
-            _V(-0.5,0.5,0.5),
-            _V(0.5,-0.5,0.5),
-            _V(0.5,0.5,-0.5),
-            _2uni(a)
-        )
-
-    @staticmethod
-    def FCC(a: _U[float,_L]):
-        """Rhombohedral primitive cell of the FCC lattice"""
-        return Lattice.fromPrimitives(
-            _V(0.5, 0.5, 0.0),
-            _V(0.0, 0.5, 0.5),
-            _V(0.5, 0.0, 0.5),
-            _2uni(a)
-        )
-
-    @staticmethod
-    def HEX(a: float, c: float, unit: _O[_L] = None):
-        return Lattice.fromPrimitives(
-            _V(-1.0,0.0,0.0),
-            _V(-0.5,0.8660254037844386,0.0),
-            _V(0.0,0.0,1.0),
-            _P(a,a,c,unit)
-        )
-
-    @staticmethod
-    def TET(a: float, c: float, unit: _O[_L] = None):
-        """Simple tetragonal"""
-        return Lattice.fromAngles(
-            _V.uniform(90),
-            _P(a,a,c,unit)
-        )
-    
-    @staticmethod
-    def BCT(a: float, c: float, unit: _O[_L] = None):
-        """Body-centered tetragonal"""
-        return Lattice.fromPrimitives(
-            _V(-0.5,0.5,0.5),
-            _V(0.5,-0.5,0.5),
-            _V(0.5,0.5,-0.5),
-            _P(a,a,c,unit)
-        )
-
-    @staticmethod
-    def ORC(dimensions: _U[_V,_P]):
-        """Simple orthorhombic"""
-        return Lattice.fromAngles(_V.uniform(90),dimensions)
-    
-    @staticmethod
-    def ORCC(dimensions: _U[_V,_P]):
-        """Base-centered orthorhombic"""
-        return Lattice.fromPrimitives(
-            _V(0.5,-0.5,0.0),
-            _V(0.5,0.5,0.0),
-            _V(0.0,0.0,1.0),
-            dimensions
-        )
-
-
-def CsClLike(atomA: Atom, atomB: Atom, a: _U[float,_L]):
-    """Two interpenetrating primitive cubic structure"""
-    l = Lattice.CUB(a)
-    b = AtomBasis(
-        (atomA, _V.zero()),
-        (atomB, _V.uniform(0.5))
-    )
-    return (b,l)
-
-
-def RockSaltLike(atomA: Atom, atomB: Atom, a: _U[float,_L]):
-    """
-    Two interpenetrating FCC that form a chessboard like crystal\n
-    Examples: NaCl, PbS
-    """
-    l = Lattice.FCC(a)
-    b = AtomBasis(
-        (atomA, _V.zero()),
-        (atomB, _V.uniform(0.5))
-    )
-    return (b,l)
-
-
-def FluoriteLike(Ca: Atom, F: Atom, a: _U[float,_L]):
-    """
-    FCC crystal with stechiometric ration of 1:2 between atoms\n
-    Examples: BaF2, β-PbF2, PuO2, SrF2, UO2, CaF2, ZrO2, K2O , K2S , Li2O, Na2O, Na2S, Rb2O, Mg2Si
-    """
-    l = Lattice.FCC(a)
-    b = AtomBasis(
-        (Ca, _V.zero()),
-        (F, _V.uniform(1/3)),
-        (F, _V.uniform(2/3)),
-    )
-    return (b,l)
-
-
-def ZincBlendeLike(atomA: Atom, atomB: Atom, a: _U[float,_L]):
-    """
-    Two interpenetrating FCC crystal\n
-    Examples:
-     - Diamond: both atoms are C
-     - Zincblende: basis of Zn & S
-    """
-    l = Lattice.FCC(a)
-    b = AtomBasis(
-        (atomA, _V.zero()),
-        (atomB, _V.uniform(0.25))
-    )
-    return (b,l)
-
-
-def HCP(atomA: Atom, atomB: Atom, a: float, c: float, unit: _O[_L] = None):
-    """Hexagonal Close Packet crystal"""
-    l = Lattice.HEX(a,c,unit)
-    b = AtomBasis(
-        (atomA, _V.zero()),
-        (atomB, _V(2/3, 1/3, 0.5)),
-    )
-    return (b,l)
-
-
-def WurtziteLike(atomA: Atom, atomB: Atom, a: float, c: float, unit: _O[_L] = None):
-    """
-    Two interpenetrating HCP crystal\n
-    Examples: wurtzite (ZnS), silver iodide (AgI), zinc oxide (ZnO), cadmium sulfide (CdS), cadmium selenide (CdSe), silicon carbide (α-SiC), gallium nitride (GaN), aluminium nitride (AlN), boron nitride (w-BN)
-    """
-    l = Lattice.HEX(a,c,unit)
-    b = AtomBasis(
-        (atomA, _V.zero()),
-        (atomB, _V(2/3, 1/3, 0.25)),
-        (atomA, _V(2/3, 1/3, 0.5)),
-        (atomB, _V(0.0,0.0,0.75))
-    )
-    return (b,l)
-
-
-def NiAsLike(Ni: Atom, As: Atom, a: float, c: float, unit: _O[_L] = None):
-    """
-    Iterpenetrating HEX and HCP\n
-    Examples: 
-     - Achavalite: FeSe
-     - Breithauptite: NiSb
-     - Freboldite: CoSe
-     - Kotulskite: Pd(Te,Bi)
-     - Langistite: (Co,Ni)As
-     - Nickeline: NiAs
-     - Sobolevskite: Pd(Bi,Te)
-     - Sudburyite: (Pd,Ni)Sb
-    """
-    l = Lattice.HEX(a,c,unit)
-    b = AtomBasis(
-        (Ni, _V.zero()),
-        (As, _V(2/3, 1/3, 0.25)),
-        (Ni, _V(0.0,0.0,0.5)),
-        (As, _V(1/3, 2/3, 0.75))
-    )
+from ._common import Vec3D as _V, Stampable as _S, _pos_int
+from typing import Optional as _O, Union as _U
+from .units import Length as _L, Pos3D as _P
+
+__all__ = ["Atom", "AtomBasis", "Lattice", "HCP", "CsClLike", "RockSaltLike", "FluoriteLike", "ZincBlendeLike", "HCP", "WurtziteLike", "NiAsLike"]
+
+_atom_symbols = ["H","He","Li","Be","B","C","N","O","F","Ne","Na","Mg","Al","Si","P","S","Cl","Ar","K","Ca","Sc","Ti","V","Cr","Mn","Fe","Co","Ni","Cu","Zn","Ga","Ge","As","Se","Br","Kr","Rb","Sr","Y","Zr","Nb","Mo","Tc","Ru","Rh","Pd","Ag","Cd","In","Sn","Sb","Te","I","Xe","Cs","Ba","La","Ce","Pr","Nd","Pm","Sm","Eu","Gd","Tb","Dy","Ho","Er","Tm","Yb","Lu","Hf","Ta","W","Re","Os","Ir","Pt","Au","Hg","Tl","Pb","Bi","Po","At","Rn","Fr","Ra","Ac","Th","Pa","U ","Np","Pu","Am","Cm","Bk","Cf","Es","F","Md","No","Lr","Rf","Db","Sg","Bh","Hs","Mt","Ds","Rg","Cn","Nh","Fl","Mc","Lv","Ts","Og"]
+
+class Atom:
+    def __init__(self, Z: int, file: str):
+        assert _pos_int(Z), "Atomic number must be a positive integer"
+        self.num = Z
+        self.file = file
+        assert self.file.find(",") == -1, "File name cannot contain ','"
+    
+    def __str__(self) -> str:
+        return f"{_atom_symbols[self.num-1]} atom (located at {self.file})"
+    
+    # def __eq__(self, __value: object) -> bool:
+    #     return (self is __value) or (type(__value) is Atom and __value.num == self.num and __value.file == self.file)
+
+    @staticmethod
+    def of(name: str):
+        """Constructs an atom using default filenaming
+        
+        returns Atom(Z of element, element name + '.psp8')
+        """
+        try:
+            Z = _atom_symbols.index(name) + 1;
+            return Atom(Z, name + '.psp8')
+        except:
+            raise ValueError(name + " is not a valid atom type")
+    
+    @staticmethod
+    def poolstr(atoms: 'list[Atom]'):
+        return f"""# Atoms definition
+ntypat {len(atoms)}
+znucl {' '.join(str(a.num) for a in atoms)}
+pseudos \"{', '.join(a.file for a in atoms)}\""""
+
+
+class AtomBasis(_S):
+    def __init__(self, *atoms: 'tuple[Atom,_V]', cartesian: bool = False) -> None:
+        """Construct an atom basis given a sequence of tuples containing an atom and a position (Vec3D)\n
+        If `cartesian` is True, the coordinates of the atoms' position are cartesian instead of reduced."""
+        assert len(atoms) > 0, "There must be at least one atom in basis"
+        self.atoms = atoms
+        self.cartesian = cartesian
+    
+    def add(self, atom: Atom, where: _V):
+        if type(self.atoms) is tuple:
+            self.atoms = list(self.atoms)
+        self.atoms.append((atom, where)) # type: ignore
+    
+    def getAtoms(self):
+        return (a[0] for a in self.atoms)
+    
+    def stamp(self, index: int, pool: 'list[Atom]'):
+        indexes = [pool.index(a[0]) for a in self.atoms]
+        suffix = str(index or '');
+        x_type = "xcart" if self.cartesian else "xred";
+        return f"""natom{suffix} {len(indexes)}
+typat{suffix} {' '.join(str(i+1) for i in indexes)}
+{x_type}{suffix} {'   '.join(str(a[1]) for a in self.atoms)}"""
+
+    @staticmethod
+    def ofOne(atom: Atom):
+        """Construct an atom basis with only one atom (placed at Vec3D(0,0,0))"""
+        return AtomBasis((atom, _V.zero()))
+
+
+def _2uni(v: _U[float,_L]):
+    t = type(v)
+    if t is _L:
+        return _P.uniform(v) # type: ignore
+    elif t is float:
+        return _V.uniform(v) # type: ignore
+    else:
+        raise TypeError(f"Lattice constant is of wrong value (got {t} instead of float or Length)")
+
+
+class Lattice(_S):
+    def __init__(self, **props):
+        """Do not use directly: prefer static methods like fromAngle, fromPrimitives"""
+        self._p = props
+
+    def stamp(self, index: int):
+        suffix = index if index > 0 else ''
+        return '\n'.join(f"{k}{suffix} {v}" for k,v in self._p.items())
+    
+    @staticmethod
+    def fromAngles(angles: _V, scaling: _U[_V,_P]):
+        """
+        Constructs lattice from angles [&alpha;, &beta;, &gamma;]\n
+        Scaling is defined per primitive vector (e.g. a is multiplied by scaling[0])
+
+        Angles are defined between vectors as follows:
+        | angle | from | to |
+        | :---: | :----------: | :-----------: |
+        | &alpha;(1) | b(2) | c(3) |
+        | &beta;(2) | a(1) | c(3) |
+        | &gamma;(3) | a(1) | b(2) |
+        """
+        assert type(angles) is _V, "Angles must be of type Vec3D"
+        return Lattice(acell=_P.sanitize(scaling), angdeg=angles)
+    
+    @staticmethod
+    def fromPrimitives(a: _V, b: _V, c: _V, scaling: _U[_V,_P]):
+        """
+        Construct lattice from primitives [a, b, c]\n
+        Scaling is applied to the cartesian axis
+        """
+        assert type(a) is _V and type(b) is _V and type(c) is _V, "Primitive vectors must be of type Vec3D"
+        return Lattice(scalecart=_P.sanitize(scaling), rprim=f"{a}   {b}   {c}")
+    
+    @staticmethod
+    def CUB(a: _U[float,_L]):
+        return Lattice.fromAngles(_V.uniform(90),_2uni(a))
+
+    @staticmethod
+    def BCC(a: _U[float,_L]):
+        return Lattice.fromPrimitives(
+            _V(-0.5,0.5,0.5),
+            _V(0.5,-0.5,0.5),
+            _V(0.5,0.5,-0.5),
+            _2uni(a)
+        )
+
+    @staticmethod
+    def FCC(a: _U[float,_L]):
+        """Rhombohedral primitive cell of the FCC lattice"""
+        return Lattice.fromPrimitives(
+            _V(0.5, 0.5, 0.0),
+            _V(0.0, 0.5, 0.5),
+            _V(0.5, 0.0, 0.5),
+            _2uni(a)
+        )
+
+    @staticmethod
+    def HEX(a: float, c: float, unit: _O[_L] = None):
+        return Lattice.fromPrimitives(
+            _V(-1.0,0.0,0.0),
+            _V(-0.5,0.8660254037844386,0.0),
+            _V(0.0,0.0,1.0),
+            _P(a,a,c,unit)
+        )
+
+    @staticmethod
+    def TET(a: float, c: float, unit: _O[_L] = None):
+        """Simple tetragonal"""
+        return Lattice.fromAngles(
+            _V.uniform(90),
+            _P(a,a,c,unit)
+        )
+    
+    @staticmethod
+    def BCT(a: float, c: float, unit: _O[_L] = None):
+        """Body-centered tetragonal"""
+        return Lattice.fromPrimitives(
+            _V(-0.5,0.5,0.5),
+            _V(0.5,-0.5,0.5),
+            _V(0.5,0.5,-0.5),
+            _P(a,a,c,unit)
+        )
+
+    @staticmethod
+    def ORC(dimensions: _U[_V,_P]):
+        """Simple orthorhombic"""
+        return Lattice.fromAngles(_V.uniform(90),dimensions)
+    
+    @staticmethod
+    def ORCC(dimensions: _U[_V,_P]):
+        """Base-centered orthorhombic"""
+        return Lattice.fromPrimitives(
+            _V(0.5,-0.5,0.0),
+            _V(0.5,0.5,0.0),
+            _V(0.0,0.0,1.0),
+            dimensions
+        )
+
+
+def CsClLike(atomA: Atom, atomB: Atom, a: _U[float,_L]):
+    """Two interpenetrating primitive cubic structure"""
+    l = Lattice.CUB(a)
+    b = AtomBasis(
+        (atomA, _V.zero()),
+        (atomB, _V.uniform(0.5))
+    )
+    return (b,l)
+
+
+def RockSaltLike(atomA: Atom, atomB: Atom, a: _U[float,_L]):
+    """
+    Two interpenetrating FCC that form a chessboard like crystal\n
+    Examples: NaCl, PbS
+    """
+    l = Lattice.FCC(a)
+    b = AtomBasis(
+        (atomA, _V.zero()),
+        (atomB, _V.uniform(0.5))
+    )
+    return (b,l)
+
+
+def FluoriteLike(Ca: Atom, F: Atom, a: _U[float,_L]):
+    """
+    FCC crystal with stechiometric ration of 1:2 between atoms\n
+    Examples: BaF2, β-PbF2, PuO2, SrF2, UO2, CaF2, ZrO2, K2O , K2S , Li2O, Na2O, Na2S, Rb2O, Mg2Si
+    """
+    l = Lattice.FCC(a)
+    b = AtomBasis(
+        (Ca, _V.zero()),
+        (F, _V.uniform(1/3)),
+        (F, _V.uniform(2/3)),
+    )
+    return (b,l)
+
+
+def ZincBlendeLike(atomA: Atom, atomB: Atom, a: _U[float,_L]):
+    """
+    Two interpenetrating FCC crystal\n
+    Examples:
+     - Diamond: both atoms are C
+     - Zincblende: basis of Zn & S
+    """
+    l = Lattice.FCC(a)
+    b = AtomBasis(
+        (atomA, _V.zero()),
+        (atomB, _V.uniform(0.25))
+    )
+    return (b,l)
+
+
+def HCP(atomA: Atom, atomB: Atom, a: float, c: float, unit: _O[_L] = None):
+    """Hexagonal Close Packet crystal"""
+    l = Lattice.HEX(a,c,unit)
+    b = AtomBasis(
+        (atomA, _V.zero()),
+        (atomB, _V(2/3, 1/3, 0.5)),
+    )
+    return (b,l)
+
+
+def WurtziteLike(atomA: Atom, atomB: Atom, a: float, c: float, unit: _O[_L] = None):
+    """
+    Two interpenetrating HCP crystal\n
+    Examples: wurtzite (ZnS), silver iodide (AgI), zinc oxide (ZnO), cadmium sulfide (CdS), cadmium selenide (CdSe), silicon carbide (α-SiC), gallium nitride (GaN), aluminium nitride (AlN), boron nitride (w-BN)
+    """
+    l = Lattice.HEX(a,c,unit)
+    b = AtomBasis(
+        (atomA, _V.zero()),
+        (atomB, _V(2/3, 1/3, 0.25)),
+        (atomA, _V(2/3, 1/3, 0.5)),
+        (atomB, _V(0.0,0.0,0.75))
+    )
+    return (b,l)
+
+
+def NiAsLike(Ni: Atom, As: Atom, a: float, c: float, unit: _O[_L] = None):
+    """
+    Iterpenetrating HEX and HCP\n
+    Examples: 
+     - Achavalite: FeSe
+     - Breithauptite: NiSb
+     - Freboldite: CoSe
+     - Kotulskite: Pd(Te,Bi)
+     - Langistite: (Co,Ni)As
+     - Nickeline: NiAs
+     - Sobolevskite: Pd(Bi,Te)
+     - Sudburyite: (Pd,Ni)Sb
+    """
+    l = Lattice.HEX(a,c,unit)
+    b = AtomBasis(
+        (Ni, _V.zero()),
+        (As, _V(2/3, 1/3, 0.25)),
+        (Ni, _V(0.0,0.0,0.5)),
+        (As, _V(1/3, 2/3, 0.75))
+    )
     return (b,l)
```

### Comparing `pynabi-0.1.1/src/pynabi/kspace.py` & `pynabi-0.1.2/src/pynabi/kspace.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,311 +1,316 @@
-from ._common import Vec3D as _V, Stampable as _Stmp, _pos_int, _pos_num, CanDelay as _CD, Delayed as _D, Later as _L
-from enum import Enum as _E
-from typing import Dict as _dict, Any as _any, Union as _union, Tuple as _tuple, Iterable as _iter
-
-
-__all__ = ["BZ", "CriticalPointsOf", "ManualGrid", "SymmetricGrid", "UsualKShifts", "Path"]
-
-
-class BZ(_E):
-    """Brillouin Zone symmetries required to setup a symmetric grid"""
-    Irreducible = 1
-    Half = 2
-    Full = 3
-    NoTimeReversal = 4
-
-
-class CriticalPointsOf(_E):
-    """
-    Critical points of (some) Brillouin zones\n
-    Taken from http://lampx.tugraz.at/~hadley/ss1/bzones/
-    """
-    CUB = {
-        'R': _V(0.5, 0.5, 0.5),
-        'X': _V(0.0, 0.5, 0.0),
-        'M': _V(0.5, 0.5, 0.0)
-    }
-    BCC = {
-        'H': _V(-0.5, 0.5, 0.5),
-        'P': _V.uniform(0.25),
-        'N': _V(0.0, 0.5, 0.0)
-    }
-    FCC = {
-        'X': _V(0.0, 0.5, 0.5),
-        'L': _V.uniform(0.5),
-        'W': _V(0.25, 0.75, 0.5),
-        'U': _V(0.25, 0.625, 0.625),
-        'K': _V(0.375, 0.75, 0.375)
-    }
-    HEX = {
-        'A': _V(0,0,1/2),
-        'K': _V(2/3,1/3,0),
-        'H': _V(2/3,1/3,1/2),
-        'M': _V(1/2,0,0),
-        'L': _V(1/2,0,1/2)
-    }
-    TET = {
-        'X': _V(0.5,0.0,0.0),
-        'M': _V(0.5,0.5,0.0),
-        'Z': _V(0.0,0.0,0.5),
-        'R': _V(0.5,0.0,0.5),
-        'A': _V.uniform(0.5)
-    }
-    BCT = {
-        'X': _V(0.5,0.0,0.0),
-        'Z': _V(0.5,0.5,-0.5),
-        'N': _V(0.0,0.5,0.0),
-        'P': _V.uniform(0.25)
-    }
-    ORC = {
-        'X': _V(0.5,0.0,0.0),
-        'Y': _V(0.0,0.5,0.0),
-        'Z': _V(0.0,0.0,0.5),
-        'T': _V(0.0,0.5,0.5),
-        'U': _V(0.5,0.0,0.5),
-        'S': _V(0.5,0.5,0.5),
-        'R': _V.uniform(0.5)
-    }
-    ORCC = {
-        'Y': _V(0.5,0.5,0.0),
-        'Y': _V(-0.5,0.5,0.0),
-        'Z': _V(0.0,0.0,0.5),
-        'T': _V.uniform(0.5),
-        'T': _V(-0.5,0.5,0.5),
-        'S': _V(0.0,0.5,0.0),
-        'R': _V(0.0,0.5,0.5),
-    }
-
-
-class UsualKShifts(_E):
-    Unshifted = (_V.zero(),)
-    Default = (_V.uniform(0.5),)
-    BCC = (_V.uniform(0.25), _V.uniform(-0.25))
-    FCC = (_V.uniform(0.5), _V(0.5,0.0,0.0), _V(0.0,0.5,0.0), _V(0.0,0.0,0.5))
-    HEX = (_V(1.0,0.0,0.0), _V(-0.5,0.8660254037844386,0.0), _V(0.0,0.0,1.0))
-
-
-class ManualGrid(_Stmp):
-    def __init__(self, *points: _V, normalize: float = 1.0) -> None:
-        assert all(type(v) is _V for v in points), "Points of the manual grid must be Vec3D"
-        assert normalize >= 1, "k-points normalization faction cannot be lower than 1"
-        self.p = points
-        self.n = normalize
-    
-    def stamp(self, index: int):
-        s = index or ''
-        kpt = "   ".join(str(v) for v in self.p)
-        return f"kptopt{s} 0\nnkpt{s} {len(self.p)}\nkpt{s} {kpt}\nkptnrm{s} {self.n}"
-
-
-def _parse_shifts(value: _tuple[_V,...]|UsualKShifts) -> _tuple[_V,...]:
-    if type(value) is UsualKShifts:
-        return value.value
-    elif type(value) is tuple:
-        assert all(type(v) is _V for v in value), "K Shifts must be vectors"
-        return value
-    else:
-        raise TypeError("Invalid type of k shifts")
-
-
-class _D_grid_points(_CD.info):
-    def sanitize(self, value):
-        t = type(value)
-        if t is int:
-            assert value > 0, f"{self.name} must be positive (if integer)"
-            return (value,value,value)
-        elif t is tuple:
-            assert len(value) == 3 and all(_pos_int(v) for v in value), f"{self.name} must be a tuple of three positive integers"
-            return value
-        else:
-            raise TypeError(f"{self.name} must be either a positive integer or a tuple of 3 positive integers")
-
-    def stamp(self, suffix, value):
-        return f"{self.prop}{suffix} {value[0]} {value[1]} {value[2]}"
-
-
-class _D_super_lattice(_CD.info):
-    def sanitize(self, value):
-        try:
-            assert type(value) is tuple and len(value) == 3
-            assert all(type(v) is _V for v in value) 
-            return value
-        except:
-            raise TypeError(f"{self.name} must be three Vec3D")
-    
-    def stamp(self, suffix, value):
-        s = '  '.join(str(v) for v in value)
-        return f"{self.prop}{suffix} {s}"
-
-
-class SymmetricGrid(_CD):
-    """Constructs a grid of k-points in the reciprocal space leveraging a symmetry of the Brillouin Zone"""
-
-    _delayables = (
-        _D_grid_points("ngkpt", "Number of grid points"),
-        _D_super_lattice("kptrlatt", "Super lattice vectors")
-    )
-
-    def __init__(self, symmetry: BZ, shifts: _union[_tuple[_V,...], UsualKShifts] = ()):
-        super().__init__(_L(),_L())
-        assert type(symmetry) is BZ, "Symmetry must one of the entries of BZ"
-        self.sym = symmetry
-        self.shi = _parse_shifts(shifts)
-        self.type = -1
-    
-    def _doesDelay(self, i: int):
-        return self.type == i and super()._doesDelay(i)
-    
-    def ofMonkhorstPack(self, gridPointsNumber: int|tuple[int,int,int]|_L = _L()):
-        assert self.type == -1, "Symmetric grid type redefined"
-        self.type = 0
-        self._dv = (self._delayables[0].laterOrSanitized(gridPointsNumber), _L())
-        return self
-    
-    def fromSuperLattice(self, a: _V, b: _V, c: _V):
-        assert self.type == -1, "Symmetric grid type redefined"
-        self.type = 1
-        self._dv = (_L(), self._delayables[1].laterOrSanitized((a,b,c)))
-        return self
-    
-    @classmethod
-    def setMPgridPointNumber(cls, num: int|tuple[int,int,int]):
-        """Sets the number of k points in the Monkhorst-Pack grid"""
-        return _D(cls, 0, num)
-    
-    @classmethod
-    def setSuperLatticeVectors(cls, a: _V, b: _V, c: _V):
-        """Sets the vectors of the super lattice"""
-        return _D(cls, 1, (a,b,c))
-
-
-class AutomaticGrid(_Stmp):
-    """ABINIT will automatically generate a large set of possible k point grids, and select among this set, the grids that give a length of smallest vector larger than the provided lenght.
-    
-    Note that this procedure can be time-consuming. It is worth doing it once for a given unit cell and set of symmetries, but not use this procedure by default. The best is then to use `AbOut().KPointsSets()`, in order to get a detailed analysis of the set of grids."""
-
-    def __init__(self, symmetry: BZ, length: float = 30.0):
-        self.sym = symmetry
-        self.len = length
-    
-    def stamp(self, index: int):
-        s = index or ''
-        return f"kptopt{s} {self.sym.value}\nkptrlen{s} {self.len}"
-
-
-def _parse_crit_point(c: str, s: dict[str,_V]):
-    if c == 'G':
-        return _V.zero()
-    else:
-        assert c in s, f"(critical) point '{c}' is not defined"
-        assert type(s[c]) is _V, f"type of critial point '{c}' is not Vec3D"
-        return s[c]
-
-
-class Path(_Stmp):
-    """A path though points in the reciprocal space"""
-
-    def __init__(self, points: list[_V]|tuple[_V], prop: str, val: str) -> None:
-        """DO NOT USE this constructor"""
-        super().__init__()
-        self.points = points
-        self.prop = prop
-        self.val = val
-    
-    def stamp(self, index: int):
-        s = index or ''
-        bounds = '  '.join(str(v) for v in self.points)
-        return f"kptopt{s} {1-len(self.points)}\nkptbounds{s} {bounds}\n{self.prop}{s} {self.val}"
-
-    @staticmethod
-    def auto(minDivisions: int, points: str|_iter[_union[str,_V]], pointSet: CriticalPointsOf|_dict[str,_V] = {}):
-        """Path through k points. The number of division for each segment is scaled based on the length and `minDivisions`, the number of division of the smallest segment.
-        
-        ## Example
-        ```python
-        # this path
-        p1 = Path.auto(10, (
-            V.zero(),
-            V(0.0, 0.5, 0.5),
-            V.uniform(0.5),
-            V(0.25, 0.75, 0.5)
-        ))
-        # is equivalent to
-        p2 = Path.auto(10, "GXLW", CriticalPointsOf.FCC)
-
-        # You don't have to sacrifice the comfort of strings 
-        # to pass through non critical points
-        p3 = Path.auto(10, ("GX", V(0.25,0.5,0.4), "LW"), CriticalPointsOf.FCC)
-
-        # For some application, it could be useful to define
-        # custom critical points and use them
-        ccp = {
-            'A': V(0.25,0.5,0.75),
-            'B': V(0.75,0.5,0.25),
-            'C': V(-0.5,0.25,0.4)
-        }
-        p4 = Path.auto(10, "GABGC", ccp) # note that 'G' is always (0,0,0)
-        ```"""
-        assert _pos_int(minDivisions), "Smallest division must be a positive integer"
-        s: dict[str,_V] = pointSet.value if type(pointSet) is CriticalPointsOf else pointSet  # type: ignore
-        b: list[_V] = []
-        for p in points:
-            if type(p) is str:
-                for c in p:
-                    b.append(_parse_crit_point(c,s))
-            elif type(p) is _V:
-                b.append(p)
-            else:
-                raise TypeError(f"Invalid type of k-path point (got {type(p)})")
-        assert len(b) > 1, "Number of boundaries must be at least 2 (i.e. one segment)"
-        return Path(b, "ndivsm", str(minDivisions))
-    
-    @staticmethod
-    def manual(*args: int|_V|str, pointSet: CriticalPointsOf|_dict[str,_V] = {}):
-        """Path though k points where each segment has its own number of divisions. To specify points and divisions, the arguments must be a sequence of alternating positive integers and k points, starting and eending in a k point.
-
-        ## Example
-        ```python
-        # this path
-        p1 = Path.manual( V.zero(), 10, V(0.0, 0.5, 0.5), 15, V.uniform(0.5), 20, V(0.25, 0.75, 0.5))
-        # is equivalent to
-        p2 = Path.auto('G',10,'X',15,'L',20,'W', pointSet=CriticalPointsOf.FCC)
-
-        # You don't have to sacrifice the comfort of strings 
-        # to pass through non critical points
-        p3 = Path.auto('G',10,'X',18,V(0.25,0.5,0.4),12,'L',15,'W', pointSet=CriticalPointsOf.FCC)
-
-        # For some application, it could be useful to define
-        # custom critical points and use them
-        ccp = {
-            'A': V(0.25,0.5,0.75),
-            'B': V(0.75,0.5,0.25),
-            'C': V(-0.5,0.25,0.4)
-        }
-        p4 = Path.auto('G',7,'A',8,'B',16'G',10,'C', pointSet=ccp) # note that 'G' is always (0,0,0)
-        ```"""
-        s: dict[str,_V] = pointSet.value if type(pointSet) is CriticalPointsOf else pointSet  # type: ignore
-        p: list[_V] = []
-        d: list[int] = []
-        assert len(args) & 1, "Invalid path sequence"
-        for i in range(0, len(args)-1, 2):
-            t = type(args[i])
-            if t is str:
-                p.append(_parse_crit_point(args[i],s)) # type: ignore
-            elif t is _V:
-                p.append(args[i]) # type: ignore
-            else:
-                raise TypeError(f"Element number {i+1} must be a vector or a critical point name")
-            assert _pos_int(args[i+1]), f"Number of divisions must be a positive integer (at position {i+2})"
-            d.append(args[i+1]) # type: ignore
-        last = args[len(args)-1]
-        t = type(last)
-        if t is str:
-            p.append(_parse_crit_point(last,s)) # type: ignore
-        elif t is _V:
-            p.append(last) # type: ignore
-        else:
-            raise TypeError(f"Last element must be a vector or a critical point name")
-        return Path(p, "ndivk", ' '.join(str(v) for v in d))
-
-
+from ._common import Vec3D as _V, Stampable as _Stmp, _pos_int, _pos_num, CanDelay as _CD, Delayed as _D, Later as _L
+from enum import Enum as _E
+from typing import Dict as _dict, Any as _any, Union as _union, Tuple as _tuple, Iterable as _iter
+
+
+__all__ = ["BZ", "CriticalPointsOf", "ManualGrid", "SymmetricGrid", "UsualKShifts", "Path"]
+
+
+class BZ(_E):
+    """Brillouin Zone symmetries required to setup a symmetric grid"""
+    Irreducible = 1
+    Half = 2
+    Full = 3
+    NoTimeReversal = 4
+
+
+class CriticalPointsOf(_E):
+    """
+    Critical points of (some) Brillouin zones\n
+    Taken from http://lampx.tugraz.at/~hadley/ss1/bzones/
+    """
+    CUB = {
+        'R': _V(0.5, 0.5, 0.5),
+        'X': _V(0.0, 0.5, 0.0),
+        'M': _V(0.5, 0.5, 0.0)
+    }
+    BCC = {
+        'H': _V(-0.5, 0.5, 0.5),
+        'P': _V.uniform(0.25),
+        'N': _V(0.0, 0.5, 0.0)
+    }
+    FCC = {
+        'X': _V(0.0, 0.5, 0.5),
+        'L': _V.uniform(0.5),
+        'W': _V(0.25, 0.75, 0.5),
+        'U': _V(0.25, 0.625, 0.625),
+        'K': _V(0.375, 0.75, 0.375)
+    }
+    HEX = {
+        'A': _V(0,0,1/2),
+        'K': _V(2/3,1/3,0),
+        'H': _V(2/3,1/3,1/2),
+        'M': _V(1/2,0,0),
+        'L': _V(1/2,0,1/2)
+    }
+    TET = {
+        'X': _V(0.5,0.0,0.0),
+        'M': _V(0.5,0.5,0.0),
+        'Z': _V(0.0,0.0,0.5),
+        'R': _V(0.5,0.0,0.5),
+        'A': _V.uniform(0.5)
+    }
+    BCT = {
+        'X': _V(0.5,0.0,0.0),
+        'Z': _V(0.5,0.5,-0.5),
+        'N': _V(0.0,0.5,0.0),
+        'P': _V.uniform(0.25)
+    }
+    ORC = {
+        'X': _V(0.5,0.0,0.0),
+        'Y': _V(0.0,0.5,0.0),
+        'Z': _V(0.0,0.0,0.5),
+        'T': _V(0.0,0.5,0.5),
+        'U': _V(0.5,0.0,0.5),
+        'S': _V(0.5,0.5,0.5),
+        'R': _V.uniform(0.5)
+    }
+    ORCC = {
+        'Y': _V(0.5,0.5,0.0),
+        'Y': _V(-0.5,0.5,0.0),
+        'Z': _V(0.0,0.0,0.5),
+        'T': _V.uniform(0.5),
+        'T': _V(-0.5,0.5,0.5),
+        'S': _V(0.0,0.5,0.0),
+        'R': _V(0.0,0.5,0.5),
+    }
+
+
+class UsualKShifts(_E):
+    Unshifted = (_V.zero(),)
+    Default = (_V.uniform(0.5),)
+    BCC = (_V.uniform(0.25), _V.uniform(-0.25))
+    FCC = (_V.uniform(0.5), _V(0.5,0.0,0.0), _V(0.0,0.5,0.0), _V(0.0,0.0,0.5))
+    HEX = (_V(1.0,0.0,0.0), _V(-0.5,0.8660254037844386,0.0), _V(0.0,0.0,1.0))
+
+
+class ManualGrid(_Stmp):
+    def __init__(self, *points: _V, normalize: float = 1.0) -> None:
+        assert all(type(v) is _V for v in points), "Points of the manual grid must be Vec3D"
+        assert normalize >= 1, "k-points normalization faction cannot be lower than 1"
+        self.p = points
+        self.n = normalize
+    
+    def stamp(self, index: int):
+        s = index or ''
+        kpt = "   ".join(str(v) for v in self.p)
+        return f"kptopt{s} 0\nnkpt{s} {len(self.p)}\nkpt{s} {kpt}\nkptnrm{s} {self.n}"
+
+
+def _parse_shifts(value: _tuple[_V,...]|UsualKShifts) -> _tuple[_V,...]:
+    if type(value) is UsualKShifts:
+        return value.value
+    elif type(value) is tuple:
+        assert all(type(v) is _V for v in value), "K Shifts must be vectors"
+        return value
+    else:
+        raise TypeError("Invalid type of k shifts")
+
+
+class _D_grid_points(_CD.info):
+    def sanitize(self, value):
+        t = type(value)
+        if t is int:
+            assert value > 0, f"{self.name} must be positive (if integer)"
+            return (value,value,value)
+        elif t is tuple:
+            assert len(value) == 3 and all(_pos_int(v) for v in value), f"{self.name} must be a tuple of three positive integers"
+            return value
+        else:
+            raise TypeError(f"{self.name} must be either a positive integer or a tuple of 3 positive integers")
+
+    def stamp(self, suffix, value):
+        return f"{self.prop}{suffix} {value[0]} {value[1]} {value[2]}"
+
+
+class _D_super_lattice(_CD.info):
+    def sanitize(self, value):
+        try:
+            assert type(value) is tuple and len(value) == 3
+            assert all(type(v) is _V for v in value) 
+            return value
+        except:
+            raise TypeError(f"{self.name} must be three Vec3D")
+    
+    def stamp(self, suffix, value):
+        s = '  '.join(str(v) for v in value)
+        return f"{self.prop}{suffix} {s}"
+
+
+class SymmetricGrid(_CD):
+    """Constructs a grid of k-points in the reciprocal space leveraging a symmetry of the Brillouin Zone"""
+
+    _delayables = (
+        _D_grid_points("ngkpt", "Number of grid points"),
+        _D_super_lattice("kptrlatt", "Super lattice vectors")
+    )
+
+    def __init__(self, symmetry: BZ, shifts: _union[_tuple[_V,...], UsualKShifts] = ()):
+        super().__init__(_L(),_L())
+        assert type(symmetry) is BZ, "Symmetry must one of the entries of BZ"
+        self.sym = symmetry
+        self.shi = _parse_shifts(shifts)
+        self.type = -1
+    
+    def _doesDelay(self, i: int):
+        return self.type == i and super()._doesDelay(i)
+    
+    def ofMonkhorstPack(self, gridPointsNumber: int|tuple[int,int,int]|_L = _L()):
+        assert self.type == -1, "Symmetric grid type redefined"
+        self.type = 0
+        self._dv = (self._delayables[0].laterOrSanitized(gridPointsNumber), _L())
+        return self
+    
+    def fromSuperLattice(self, a: _V, b: _V, c: _V):
+        assert self.type == -1, "Symmetric grid type redefined"
+        self.type = 1
+        self._dv = (_L(), self._delayables[1].laterOrSanitized((a,b,c)))
+        return self
+    
+    def stamp(self, index: int):
+        s = index or ''
+        shift = " ".join(str(t) for t in self.shi)
+        return f"kptopt{s} {self.sym.value}\nnshiftk{s} {len(self.shi)}\nshiftk{s} {shift}\n{super().stamp(index)}"
+    
+    @classmethod
+    def setMPgridPointNumber(cls, num: int|tuple[int,int,int]):
+        """Sets the number of k points in the Monkhorst-Pack grid"""
+        return _D(cls, 0, num)
+    
+    @classmethod
+    def setSuperLatticeVectors(cls, a: _V, b: _V, c: _V):
+        """Sets the vectors of the super lattice"""
+        return _D(cls, 1, (a,b,c))
+
+
+class AutomaticGrid(_Stmp):
+    """ABINIT will automatically generate a large set of possible k point grids, and select among this set, the grids that give a length of smallest vector larger than the provided lenght.
+    
+    Note that this procedure can be time-consuming. It is worth doing it once for a given unit cell and set of symmetries, but not use this procedure by default. The best is then to use `AbOut().KPointsSets()`, in order to get a detailed analysis of the set of grids."""
+
+    def __init__(self, symmetry: BZ, length: float = 30.0):
+        self.sym = symmetry
+        self.len = length
+    
+    def stamp(self, index: int):
+        s = index or ''
+        return f"kptopt{s} {self.sym.value}\nkptrlen{s} {self.len}"
+
+
+def _parse_crit_point(c: str, s: dict[str,_V]):
+    if c == 'G':
+        return _V.zero()
+    else:
+        assert c in s, f"(critical) point '{c}' is not defined"
+        assert type(s[c]) is _V, f"type of critial point '{c}' is not Vec3D"
+        return s[c]
+
+
+class Path(_Stmp):
+    """A path though points in the reciprocal space"""
+
+    def __init__(self, points: list[_V]|tuple[_V], prop: str, val: str) -> None:
+        """DO NOT USE this constructor"""
+        super().__init__()
+        self.points = points
+        self.prop = prop
+        self.val = val
+    
+    def stamp(self, index: int):
+        s = index or ''
+        bounds = '  '.join(str(v) for v in self.points)
+        return f"kptopt{s} {1-len(self.points)}\nkptbounds{s} {bounds}\n{self.prop}{s} {self.val}"
+
+    @staticmethod
+    def auto(minDivisions: int, points: str|_iter[_union[str,_V]], pointSet: CriticalPointsOf|_dict[str,_V] = {}):
+        """Path through k points. The number of division for each segment is scaled based on the length and `minDivisions`, the number of division of the smallest segment.
+        
+        ## Example
+        ```python
+        # this path
+        p1 = Path.auto(10, (
+            V.zero(),
+            V(0.0, 0.5, 0.5),
+            V.uniform(0.5),
+            V(0.25, 0.75, 0.5)
+        ))
+        # is equivalent to
+        p2 = Path.auto(10, "GXLW", CriticalPointsOf.FCC)
+
+        # You don't have to sacrifice the comfort of strings 
+        # to pass through non critical points
+        p3 = Path.auto(10, ("GX", V(0.25,0.5,0.4), "LW"), CriticalPointsOf.FCC)
+
+        # For some application, it could be useful to define
+        # custom critical points and use them
+        ccp = {
+            'A': V(0.25,0.5,0.75),
+            'B': V(0.75,0.5,0.25),
+            'C': V(-0.5,0.25,0.4)
+        }
+        p4 = Path.auto(10, "GABGC", ccp) # note that 'G' is always (0,0,0)
+        ```"""
+        assert _pos_int(minDivisions), "Smallest division must be a positive integer"
+        s: dict[str,_V] = pointSet.value if type(pointSet) is CriticalPointsOf else pointSet  # type: ignore
+        b: list[_V] = []
+        for p in points:
+            if type(p) is str:
+                for c in p:
+                    b.append(_parse_crit_point(c,s))
+            elif type(p) is _V:
+                b.append(p)
+            else:
+                raise TypeError(f"Invalid type of k-path point (got {type(p)})")
+        assert len(b) > 1, "Number of boundaries must be at least 2 (i.e. one segment)"
+        return Path(b, "ndivsm", str(minDivisions))
+    
+    @staticmethod
+    def manual(*args: int|_V|str, pointSet: CriticalPointsOf|_dict[str,_V] = {}):
+        """Path though k points where each segment has its own number of divisions. To specify points and divisions, the arguments must be a sequence of alternating positive integers and k points, starting and eending in a k point.
+
+        ## Example
+        ```python
+        # this path
+        p1 = Path.manual( V.zero(), 10, V(0.0, 0.5, 0.5), 15, V.uniform(0.5), 20, V(0.25, 0.75, 0.5))
+        # is equivalent to
+        p2 = Path.auto('G',10,'X',15,'L',20,'W', pointSet=CriticalPointsOf.FCC)
+
+        # You don't have to sacrifice the comfort of strings 
+        # to pass through non critical points
+        p3 = Path.auto('G',10,'X',18,V(0.25,0.5,0.4),12,'L',15,'W', pointSet=CriticalPointsOf.FCC)
+
+        # For some application, it could be useful to define
+        # custom critical points and use them
+        ccp = {
+            'A': V(0.25,0.5,0.75),
+            'B': V(0.75,0.5,0.25),
+            'C': V(-0.5,0.25,0.4)
+        }
+        p4 = Path.auto('G',7,'A',8,'B',16'G',10,'C', pointSet=ccp) # note that 'G' is always (0,0,0)
+        ```"""
+        s: dict[str,_V] = pointSet.value if type(pointSet) is CriticalPointsOf else pointSet  # type: ignore
+        p: list[_V] = []
+        d: list[int] = []
+        assert len(args) & 1, "Invalid path sequence"
+        for i in range(0, len(args)-1, 2):
+            t = type(args[i])
+            if t is str:
+                p.append(_parse_crit_point(args[i],s)) # type: ignore
+            elif t is _V:
+                p.append(args[i]) # type: ignore
+            else:
+                raise TypeError(f"Element number {i+1} must be a vector or a critical point name")
+            assert _pos_int(args[i+1]), f"Number of divisions must be a positive integer (at position {i+2})"
+            d.append(args[i+1]) # type: ignore
+        last = args[len(args)-1]
+        t = type(last)
+        if t is str:
+            p.append(_parse_crit_point(last,s)) # type: ignore
+        elif t is _V:
+            p.append(last) # type: ignore
+        else:
+            raise TypeError(f"Last element must be a vector or a critical point name")
+        return Path(p, "ndivk", ' '.join(str(v) for v in d))
+
+
 _exclusives = (ManualGrid, SymmetricGrid, AutomaticGrid, Path)
```

### Comparing `pynabi-0.1.1/src/pynabi/relaxation.py` & `pynabi-0.1.2/src/pynabi/relaxation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,278 +1,288 @@
-from ._common import Stampable as _S, StampCollection as _SC, _pos_num, _pos0_num, IndexedWithDefault as _IWD
-from .units import Energy as _En
-from typing import Literal as _L, Tuple as _T
-
-
-# TODO: missing ionmov 20, 28
-
-
-# class FixedAtoms(_S):
-#     pass
-
-
-def _check_co(coll: _SC, name: str):
-    coov = coll.get(CellOptimizationOnVector)
-    if coov is not None:
-        raise ValueError(f"{name} is not compatible with cell optimization on vector")
-    co = coll.get(CellOptimization)
-    if co is not None:
-        raise ValueError(f"{name} is not compatible with cell optimization")
-
-
-def _mdtemp(v):
-    assert type(v) is tuple and len(v) == 2 and _pos_num(v[0]) and _pos_num(v[1]), "Temperatures must be a tuple of to positive numbers"
-    return f"[{v[0]},{v[1]}]"
-
-
-class _MD_SO(_IWD, default="__init__", prop="ionmov"):
-    def __init__(self, timeStep: float = 100, maxSteps: int = 1000) -> None:
-        super().__init__()
-        assert _pos_num(timeStep), "time step (for molecular dynamics or structural optimization) must be a positive number"
-        assert type(maxSteps) is int and maxSteps > 0, "number of maximum steps (for molecular dynamics or structural optimization) must be a positive integer"
-        self._dt = timeStep
-        self._ms = maxSteps
-    
-    def stamp(self, index: int):
-        s = index or ''
-        return super().stamp(index) + f"\ndtion{s} {self._dt}\nntime{s} {self._ms}"
-
-
-class MolecularDynamics(_MD_SO, default="basic"):
-    """Move atoms using molecular dynamics"""
-
-    def compatible(self, coll: _SC):
-        if self._index != 13: # isoenthaplic is the only one that accept cell optimization
-            _check_co(coll, "Molecular dynamics")
-    
-    def basic(self):
-        """Move atoms using undumped molecular dynamics\n
-        For viscous damping use `StructuralOptimization(...).damping(...)`"""
-        self._index = 1
-        self._extra = {"vis": 0}
-        return self
-
-    def Verlet(self):
-        """Molecular dynamics using the Verlet algorithm, see [[Allen1987a]](https://docs.abinit.org/theory/bibliography#allen1987a) p 81"""
-        self._index = 6
-        return self
-
-    def quenchedVerlet(self):
-        """Quenched Molecular dynamics using the Verlet algorithm, and stopping each atom for which the scalar product of velocity and force is negative.\n
-        The goal is not to produce a realistic dynamics, but to go as fast as possible to the minimum. For this purpose, it is advised to set all the masses to the same value"""
-        self._index = 7
-        return self
-    
-    def NoseHoover(self, inertia: float = 100, temperatures: _T[float, float] = (200,300)):
-        """
-        Molecular dynamics with Nose-Hoover thermostat, using the Verlet algorithm
-        
-        `inertia` is the inertia factor WT of the thermostat in atomic units (see [the docs](https://docs.abinit.org/variables/rlx/#noseinert))
-
-        `temperatures` is a tuple of floats who represent the initial and final temperatures of the thermostat
-        """
-        assert _pos_num(inertia), "thermostat intertia must a positive number"
-        self._index = 8
-        self._extra = { "mdtemp": _mdtemp(temperatures), "noseinert": inertia }
-        return self
-
-    def Langevin(self, friction: float, temperatures: _T[float, float] = (200,300)):
-        """
-        Langevin molecular dynamics
-
-        `friction` is friction coefficient for Langevin dynamics with units Hartree*Electronic mass*(atomic unit of Time)/Bohr^2
-
-        `temperatures` is a tuple of floats who represent the initial and final temperatures of the dynamics
-        """
-        assert _pos_num(friction), "thermostat intertia must a positive number"
-        self._index = 9
-        self._extra = { "mdtemp": _mdtemp(temperatures), "friction": friction }
-        return self
-    
-    def isokinetic(self, temperature: float = 200):
-        """
-        Isokinetic ensemble molecular dynamics\n
-        The velocity is initialized from the given temperature (in Kelvin)
-        """
-        assert _pos_num(temperature), "The temperature must be a positive number"
-        self._index = 12
-        self._extra = { "mdtemp": f"[{temperature},{temperature+1}]" }
-        return self
-
-    def SRKNa14(self):
-        """Simple molecular dynamics with a symplectic algorithm proposed in [[Blanes2002]](https://docs.abinit.org/theory/bibliography#blanes2002) (called SRKNa14) of the kind first published in [[Yoshida1990]](https://docs.abinit.org/theory/bibliography#bitzek2006). This algorithm requires at least 14 evaluation of the forces (actually 15 are done within Abinit) per time step. At this cost it usually gives much better energy conservation than the verlet algorithm for a 30 times bigger value of time step.\n
-        NOTE: the potential energy of the initial atomic configuration is never evaluated using this algorithm."""
-        self._index = 14
-        return self
-
-    def learnOnTheFly(self, iterations: int = 10):
-        """Use of Learn on The Fly method (LOTF) for Molecular Dynamics. In the framework of isokinetic MD, the atomic forces and positions are computed by using LOTF interpolation. A SCF computation is performed only _A `iterations` steps. The results of the SCF are used to compute the parameters of a short range classical potential (for the moment only the glue potential for gold is implemented). Then these parameters are continuously tuned to compute atomic trajectories.\n
-        The LOTF cycle is divided in the following steps: 
-         1. Initialization (SFC at t=0) and computation of potential parameters. 
-         2. Extrapolation of the atomic forces and positions for `iterations` time step. To perform this extrapolation, the potential computed in 1 is used (Verlet algorithm). 
-         3. SFC at t=`iterations`. Computation of the potential parameters. 
-         4. LOTF interpolation, linear interpolation of the potential parameters and computation of the atomic forces and positions between t=0 and t=`iterations`.
-        
-        NOTE: LOTF has to be enabled at configure time. If LOTF is not enabled, abinit will set automatically isokinetic MD.\n
-         """
-        assert type(iterations) is int and iterations > 0, "Number of LOTF iterations must be a positive integer"
-        self._index = 23
-        self._extra = {"lotf_nitex": iterations }
-        return self
-
-    def constantEnergy(self):
-        """Simple constant energy molecular dynamics using the velocity Verlet symplectic algorithm (second order), see [[Hairer2003]](https://docs.abinit.org/theory/bibliography#hairer2003)."""
-        self._index = 24
-        return self
-
-
-class StructuralOptimization(_MD_SO, default="BFGS"):
-    def compatible(self, coll: _SC):
-        if self._index not in (2, 3, 22):
-            _check_co(coll, "Structural optimization")
-
-    def damping(self, viscosity: float = 100):
-        """Move atoms using molecular dynamics with viscous damping (friction linearly proportional to velocity). \n
-        The implemented algorithm is the generalisation of the Numerov technique (6th order), but is NOT invariant upon time-reversal, so that the energy is not conserved."""
-        assert _pos_num(viscosity), "Viscosity must be a positive number"
-        self._index = 1
-        self._extra = {"vis": viscosity}
-        return self
-
-    def BFGS(self, delocalizedCoordinates: bool = False, withEnergy: bool = False):
-        """Conduct structural optimization using the Broyden-Fletcher-Goldfarb-Shanno minimization (BFGS)\n
-         - `withEnergy` determines whether to take into account the total energy or not (can be very unstable)
-         - `delocalizedCoordinates` detemines whether to use delocalized coordinates or not (if true, no cell optimization can be done) 
-        """
-        assert type(delocalizedCoordinates) is bool, "delocalizedCoordinates must be a bool"
-        assert type(withEnergy) is bool, "withEnergy must be a bool"
-        self._index = 2 + 8*int(delocalizedCoordinates) + int(withEnergy)
-        return self
-    
-    def conjugateGradient(self):
-        """Conjugate gradient algorithm for simultaneous optimization of potential and ionic degrees of freedom.\n
-        WARNING: this is under development, and does not work very well in m_A cases"""
-        self._index = 4
-        return self
-
-    def simpleRelaxation(self, preconditioning: _L[-1, 0, 1, 2] = 0):
-        """Simple relaxation of ionic positions according to (converged) forces\n
-        `preconditioning` is an integer between -1 and 2 and describes the way a change of force is derived from a change of atomic position. 
-        In particular: hessian is 2^(-preconditioning) times the identity matrix
-        """
-        assert type(preconditioning) is int and -1 <= preconditioning <= 2, "preconditioning must a integer between -1 and 2"
-        self._index = 5
-        self._extra = { "iprcfc": preconditioning }
-        return self
-
-    # def directInversion(self):
-    #     self._n = 20
-    #     self._d = {}
-    #     return self
-
-    def LBFGS(self):
-        """Conduct structural optimization using the Limited-memory Broyden-Fletcher-Goldfarb-Shanno minimization (L-BFGS) [[Nocedal1980]](https://docs.abinit.org/theory/bibliography#nocedal1980). 
-        The routines are based on the original implementation by J. Nocedal available on netlib.org. 
-        This algorithm can be much better than the native implementation of BFGS in ABINIT"""
-        self._index = 22
-        return self
-
-
-class FIRE(_S):
-    """Fast inertial relaxation engine (FIRE) algorithm proposed by Erik Bitzek, Pekka Koskinen, Franz Gähler, Michael Moseler, and Peter Gumbsch in [[Bitzek2006]](https://docs.abinit.org/theory/bibliography#bitzek2006). According to the authors, the efficiency of this method is nearly the same as L-BFGS. It is based on conventional molecular dynamics with additional velocity modifications and adaptive time steps. The purpose of this algorithm is relaxation, not molecular dynamics. \n
-    The initial time step is set with `initialTimeStep`: it governs the ion position changes, but the cell parameter changes as well. The suggested first guess is 0.03.\n
-    The positions are in reduced coordinates instead of in cartesian coordinates."""
-    def __init__(self, initialTimeStep: float = 0.03) -> None:
-        super().__init__()
-        assert _pos_num(initialTimeStep), "The initial time step must be a positive number"
-        self.t = initialTimeStep
-    
-    def stamp(self, index: int):
-        s = index or ''
-        return f"ionmov{s} 15\ndtion{s} {self.t}"
-
-
-class MonteCarloSampling(_S):
-    """Hybrid Monte Carlo sampling of the ionic positions at fixed temperature and unit cell geometry (NVT ensemble). 
-    The underlying molecular dynamics corresponds to the constant energy one. \n
-    Within the HMC algorithm [[Duane1987]](https://docs.abinit.org/theory/bibliography#duane1987), the trial states are generated via short trajectories (ten steps in current implementation). The initial momenta for each trial are randomly sampled from Boltzmann distribution, and the final trajectory state is either accepted or rejected based on the Metropolis criterion. Such strategy allows to simultaneously update all reduced coordinates, achieve higher acceptance ratio than classical Metropolis Monte Carlo and better sampling efficiency for shallow energy landscapes [[Prokhorenko2018]](https://docs.abinit.org/theory/bibliography#prokhorenko2018)"""
-
-    def __init__(self, temperatures: _T[float, float] = (200,300), timeStep: float = 100) -> None:
-        assert _pos_num(timeStep)
-        self.t = _mdtemp(temperatures)
-        self.s = timeStep
-    
-    def stamp(self, index: int):
-        s = index or ''
-        return f"ionmov{s} 24\ndtion{s} {self.s}\nmdtemp{s} {self.t}"
-
-    def compatible(self, coll: _SC):
-        _check_co(coll, "Monte Carlo Sampling")
-
-
-def _CO_method(n: int):
-    def fn(self: 'CellOptimization'):
-        assert self.n == 0, "Cell optimization defined multiple times"
-        self.n = n
-        return self
-    return fn
-
-
-class CellOptimization(_S):
-    def __init__(self, energyCutoffSmearing: _En|float) -> None:
-        super().__init__()
-        self.s = _En.sanitize(energyCutoffSmearing)
-        self.n = 0
-    
-    def stamp(self, index: int):
-        s = index or ''
-        return f"optcell{s} {self.n}\necutsm{s} {self.s}"
-    
-    def compatible(self, coll: _SC):
-        assert self.n != 0, "Cell optimization not fully defined"
-    
-    OnVolumeOnly = _CO_method(1)
-    Full = _CO_method(2)
-    ConstantVolume = _CO_method(3)
-
-
-class CellOptimizationOnVector(_S):
-    def __init__(self, energyCutoffSmearing: _En|float, axis: _L[1,2,3,'x','y','z','X','Y','Z'], keep: bool) -> None:
-        super().__init__()
-        self.s = _En.sanitize(energyCutoffSmearing)
-        if type(axis) is int:
-            assert 1 <= axis <= 3, "Axis index must be between 1 and 3"
-            self._a = axis
-        elif type(axis) is str:
-            n = ('x','y','z')
-            s = axis.lower()
-            assert s in n, "Axis name can only be one of the following charachters: xyxXYZ"
-            self._a = n.index(n)
-        else:
-            raise TypeError("Invalid type for axis argument")
-        assert type(keep) is bool, "Argument keeep must be a bool"
-        self._k = keep
-    
-    def stamp(self, index: int):
-        s = index or ''
-        return f"optcell{s} {4 + self._a + 3*int(self._k)}\necutsm{s} {self.s}"
-
-
-class MaxLatticeDilatation(_S):
-    def __init__(self, additional: float = 0, exceed: bool = False) -> None:
-        super().__init__()
-        assert _pos0_num(additional), "Additional percentage of memory must be a positive number"
-        if not exceed:
-            assert additional <= 15, "Additional percentage of memory must be less than or equal to 15 (when exceed is False)"
-        self.a = additional
-        self.x = exceed
-    
-    def stamp(self, index: int):
-        s = index or ''
-        return f"dilatmx{s} {1 + self.a*0.01}\nchkdilatmx{s} {int(not self.x)}"
-
-
-_ex1 = set((MolecularDynamics, StructuralOptimization, FIRE, MonteCarloSampling))
-_ex2 = set((CellOptimization, CellOptimizationOnVector))
-
-
+from ._common import Stampable as _S, StampCollection as _SC, _pos_num, _pos0_num, IndexedWithDefault as _IWD
+from .units import Energy as _En
+from typing import Literal as _L, Tuple as _T
+
+
+# TODO: missing ionmov 20, 28
+
+
+# class FixedAtoms(_S):
+#     pass
+
+
+def _check_co(coll: _SC, name: str):
+    coov = coll.get(CellOptimizationOnVector)
+    if coov is not None:
+        raise ValueError(f"{name} is not compatible with cell optimization on vector")
+    co = coll.get(CellOptimization)
+    if co is not None:
+        raise ValueError(f"{name} is not compatible with cell optimization")
+
+
+def _mdtemp(v):
+    assert type(v) is tuple and len(v) == 2 and _pos_num(v[0]) and _pos_num(v[1]), "Temperatures must be a tuple of to positive numbers"
+    return f"[{v[0]},{v[1]}]"
+
+
+class _MD_SO(_IWD, default="__init__", prop="ionmov"):
+    def __init__(self, timeStep: float = 100, maxSteps: int = 1000) -> None:
+        super().__init__()
+        assert _pos_num(timeStep), "time step (for molecular dynamics or structural optimization) must be a positive number"
+        assert type(maxSteps) is int and maxSteps > 0, "number of maximum steps (for molecular dynamics or structural optimization) must be a positive integer"
+        self._dt = timeStep
+        self._ms = maxSteps
+    
+    def stamp(self, index: int):
+        s = index or ''
+        return super().stamp(index) + f"\ndtion{s} {self._dt}\nntime{s} {self._ms}"
+
+
+class MolecularDynamics(_MD_SO, default="basic"):
+    """Move atoms using molecular dynamics"""
+
+    def compatible(self, coll: _SC):
+        if self._index != 13: # isoenthaplic is the only one that accept cell optimization
+            _check_co(coll, "Molecular dynamics")
+    
+    def basic(self):
+        """Move atoms using undumped molecular dynamics\n
+        For viscous damping use `StructuralOptimization(...).damping(...)`"""
+        self._index = 1
+        self._extra = {"vis": 0}
+        return self
+
+    def Verlet(self):
+        """Molecular dynamics using the Verlet algorithm, see [[Allen1987a]](https://docs.abinit.org/theory/bibliography#allen1987a) p 81"""
+        self._index = 6
+        return self
+
+    def quenchedVerlet(self):
+        """Quenched Molecular dynamics using the Verlet algorithm, and stopping each atom for which the scalar product of velocity and force is negative.\n
+        The goal is not to produce a realistic dynamics, but to go as fast as possible to the minimum. For this purpose, it is advised to set all the masses to the same value"""
+        self._index = 7
+        return self
+    
+    def NoseHoover(self, inertia: float = 100, temperatures: _T[float, float] = (200,300)):
+        """
+        Molecular dynamics with Nose-Hoover thermostat, using the Verlet algorithm
+        
+        `inertia` is the inertia factor WT of the thermostat in atomic units (see [the docs](https://docs.abinit.org/variables/rlx/#noseinert))
+
+        `temperatures` is a tuple of floats who represent the initial and final temperatures of the thermostat
+        """
+        assert _pos_num(inertia), "thermostat intertia must a positive number"
+        self._index = 8
+        self._extra = { "mdtemp": _mdtemp(temperatures), "noseinert": inertia }
+        return self
+
+    def Langevin(self, friction: float, temperatures: _T[float, float] = (200,300)):
+        """
+        Langevin molecular dynamics
+
+        `friction` is friction coefficient for Langevin dynamics with units Hartree*Electronic mass*(atomic unit of Time)/Bohr^2
+
+        `temperatures` is a tuple of floats who represent the initial and final temperatures of the dynamics
+        """
+        assert _pos_num(friction), "thermostat intertia must a positive number"
+        self._index = 9
+        self._extra = { "mdtemp": _mdtemp(temperatures), "friction": friction }
+        return self
+    
+    def isokinetic(self, temperature: float = 200):
+        """
+        Isokinetic ensemble molecular dynamics\n
+        The velocity is initialized from the given temperature (in Kelvin)
+        """
+        assert _pos_num(temperature), "The temperature must be a positive number"
+        self._index = 12
+        self._extra = { "mdtemp": f"[{temperature},{temperature+1}]" }
+        return self
+
+    def SRKNa14(self):
+        """Simple molecular dynamics with a symplectic algorithm proposed in [[Blanes2002]](https://docs.abinit.org/theory/bibliography#blanes2002) (called SRKNa14) of the kind first published in [[Yoshida1990]](https://docs.abinit.org/theory/bibliography#bitzek2006). This algorithm requires at least 14 evaluation of the forces (actually 15 are done within Abinit) per time step. At this cost it usually gives much better energy conservation than the verlet algorithm for a 30 times bigger value of time step.\n
+        NOTE: the potential energy of the initial atomic configuration is never evaluated using this algorithm."""
+        self._index = 14
+        return self
+
+    def learnOnTheFly(self, iterations: int = 10):
+        """Use of Learn on The Fly method (LOTF) for Molecular Dynamics. In the framework of isokinetic MD, the atomic forces and positions are computed by using LOTF interpolation. A SCF computation is performed only _A `iterations` steps. The results of the SCF are used to compute the parameters of a short range classical potential (for the moment only the glue potential for gold is implemented). Then these parameters are continuously tuned to compute atomic trajectories.\n
+        The LOTF cycle is divided in the following steps: 
+         1. Initialization (SFC at t=0) and computation of potential parameters. 
+         2. Extrapolation of the atomic forces and positions for `iterations` time step. To perform this extrapolation, the potential computed in 1 is used (Verlet algorithm). 
+         3. SFC at t=`iterations`. Computation of the potential parameters. 
+         4. LOTF interpolation, linear interpolation of the potential parameters and computation of the atomic forces and positions between t=0 and t=`iterations`.
+        
+        NOTE: LOTF has to be enabled at configure time. If LOTF is not enabled, abinit will set automatically isokinetic MD.\n
+         """
+        assert type(iterations) is int and iterations > 0, "Number of LOTF iterations must be a positive integer"
+        self._index = 23
+        self._extra = {"lotf_nitex": iterations }
+        return self
+
+    def constantEnergy(self):
+        """Simple constant energy molecular dynamics using the velocity Verlet symplectic algorithm (second order), see [[Hairer2003]](https://docs.abinit.org/theory/bibliography#hairer2003)."""
+        self._index = 24
+        return self
+
+
+class StructuralOptimization(_MD_SO, default="BFGS"):
+    def compatible(self, coll: _SC):
+        if self._index not in (2, 3, 22):
+            _check_co(coll, "Structural optimization")
+
+    def damping(self, viscosity: float = 100):
+        """Move atoms using molecular dynamics with viscous damping (friction linearly proportional to velocity). \n
+        The implemented algorithm is the generalisation of the Numerov technique (6th order), but is NOT invariant upon time-reversal, so that the energy is not conserved."""
+        assert _pos_num(viscosity), "Viscosity must be a positive number"
+        self._index = 1
+        self._extra = {"vis": viscosity}
+        return self
+
+    def BFGS(self, delocalizedCoordinates: bool = False, withEnergy: bool = False):
+        """Conduct structural optimization using the Broyden-Fletcher-Goldfarb-Shanno minimization (BFGS)\n
+         - `withEnergy` determines whether to take into account the total energy or not (can be very unstable)
+         - `delocalizedCoordinates` detemines whether to use delocalized coordinates or not (if true, no cell optimization can be done) 
+        """
+        assert type(delocalizedCoordinates) is bool, "delocalizedCoordinates must be a bool"
+        assert type(withEnergy) is bool, "withEnergy must be a bool"
+        self._index = 2 + 8*int(delocalizedCoordinates) + int(withEnergy)
+        return self
+    
+    def conjugateGradient(self):
+        """Conjugate gradient algorithm for simultaneous optimization of potential and ionic degrees of freedom.\n
+        WARNING: this is under development, and does not work very well in m_A cases"""
+        self._index = 4
+        return self
+
+    def simpleRelaxation(self, preconditioning: _L[-1, 0, 1, 2] = 0):
+        """Simple relaxation of ionic positions according to (converged) forces\n
+        `preconditioning` is an integer between -1 and 2 and describes the way a change of force is derived from a change of atomic position. 
+        In particular: hessian is 2^(-preconditioning) times the identity matrix
+        """
+        assert type(preconditioning) is int and -1 <= preconditioning <= 2, "preconditioning must a integer between -1 and 2"
+        self._index = 5
+        self._extra = { "iprcfc": preconditioning }
+        return self
+
+    # def directInversion(self):
+    #     self._n = 20
+    #     self._d = {}
+    #     return self
+
+    def LBFGS(self):
+        """Conduct structural optimization using the Limited-memory Broyden-Fletcher-Goldfarb-Shanno minimization (L-BFGS) [[Nocedal1980]](https://docs.abinit.org/theory/bibliography#nocedal1980). 
+        The routines are based on the original implementation by J. Nocedal available on netlib.org. 
+        This algorithm can be much better than the native implementation of BFGS in ABINIT"""
+        self._index = 22
+        return self
+
+
+class FIRE(_S):
+    """Fast inertial relaxation engine (FIRE) algorithm proposed by Erik Bitzek, Pekka Koskinen, Franz Gähler, Michael Moseler, and Peter Gumbsch in [[Bitzek2006]](https://docs.abinit.org/theory/bibliography#bitzek2006). According to the authors, the efficiency of this method is nearly the same as L-BFGS. It is based on conventional molecular dynamics with additional velocity modifications and adaptive time steps. The purpose of this algorithm is relaxation, not molecular dynamics. \n
+    The initial time step is set with `initialTimeStep`: it governs the ion position changes, but the cell parameter changes as well. The suggested first guess is 0.03.\n
+    The positions are in reduced coordinates instead of in cartesian coordinates."""
+    def __init__(self, initialTimeStep: float = 0.03) -> None:
+        super().__init__()
+        assert _pos_num(initialTimeStep), "The initial time step must be a positive number"
+        self.t = initialTimeStep
+    
+    def stamp(self, index: int):
+        s = index or ''
+        return f"ionmov{s} 15\ndtion{s} {self.t}"
+
+
+class MonteCarloSampling(_S):
+    """Hybrid Monte Carlo sampling of the ionic positions at fixed temperature and unit cell geometry (NVT ensemble). 
+    The underlying molecular dynamics corresponds to the constant energy one. \n
+    Within the HMC algorithm [[Duane1987]](https://docs.abinit.org/theory/bibliography#duane1987), the trial states are generated via short trajectories (ten steps in current implementation). The initial momenta for each trial are randomly sampled from Boltzmann distribution, and the final trajectory state is either accepted or rejected based on the Metropolis criterion. Such strategy allows to simultaneously update all reduced coordinates, achieve higher acceptance ratio than classical Metropolis Monte Carlo and better sampling efficiency for shallow energy landscapes [[Prokhorenko2018]](https://docs.abinit.org/theory/bibliography#prokhorenko2018)"""
+
+    def __init__(self, temperatures: _T[float, float] = (200,300), timeStep: float = 100) -> None:
+        assert _pos_num(timeStep)
+        self.t = _mdtemp(temperatures)
+        self.s = timeStep
+    
+    def stamp(self, index: int):
+        s = index or ''
+        return f"ionmov{s} 24\ndtion{s} {self.s}\nmdtemp{s} {self.t}"
+
+    def compatible(self, coll: _SC):
+        _check_co(coll, "Monte Carlo Sampling")
+
+
+def _CO_method(n: int):
+    def fn(self: 'CellOptimization'):
+        assert self.n == 0, "Cell optimization defined multiple times"
+        self.n = n
+        return self
+    return fn
+
+
+class CellOptimization(_S):
+    def __init__(self, energyCutoffSmearing: _En|float|None = None) -> None:
+        """
+        `energyCutoffSmearing` regulates the smoothing the total energy curve (as a function of the energy cutoff), in order to keep consistency with the stress (and automatically including the Pulay stress).
+
+        If none is provided, 0.5 Hatree is used as default value (it is the recommended one). If you want to optimize cell shape and size without smoothing the total energy curve (a dangerous thing to do), use a very small value, on the order of one microHartree, but never zero.
+        """
+        super().__init__()
+        if energyCutoffSmearing is None:
+            self.s = _En(0.5,0)
+        else:
+            self.s = _En.sanitize(energyCutoffSmearing)
+            assert self.s._v > 0, "Energy cutoff smearing must be positive"
+        self.n = 0
+
+    
+    def stamp(self, index: int):
+        s = index or ''
+        return f"optcell{s} {self.n}\necutsm{s} {self.s}"
+    
+    def compatible(self, coll: _SC):
+        assert self.n != 0, "Cell optimization not fully defined"
+    
+    OnVolumeOnly = _CO_method(1)
+    Full = _CO_method(2)
+    ConstantVolume = _CO_method(3)
+
+
+class CellOptimizationOnVector(_S):
+    def __init__(self, energyCutoffSmearing: _En|float, axis: _L[1,2,3,'x','y','z','X','Y','Z'], keep: bool) -> None:
+        super().__init__()
+        self.s = _En.sanitize(energyCutoffSmearing)
+        if type(axis) is int:
+            assert 1 <= axis <= 3, "Axis index must be between 1 and 3"
+            self._a = axis
+        elif type(axis) is str:
+            n = ('x','y','z')
+            s = axis.lower()
+            assert s in n, "Axis name can only be one of the following charachters: xyxXYZ"
+            self._a = n.index(n)
+        else:
+            raise TypeError("Invalid type for axis argument")
+        assert type(keep) is bool, "Argument keeep must be a bool"
+        self._k = keep
+    
+    def stamp(self, index: int):
+        s = index or ''
+        return f"optcell{s} {4 + self._a + 3*int(self._k)}\necutsm{s} {self.s}"
+
+
+class MaxLatticeDilatation(_S):
+    def __init__(self, additional: float = 0, exceed: bool = False) -> None:
+        super().__init__()
+        assert _pos0_num(additional), "Additional percentage of memory must be a positive number"
+        if not exceed:
+            assert additional <= 15, "Additional percentage of memory must be less than or equal to 15 (when exceed is False)"
+        self.a = additional
+        self.x = exceed
+    
+    def stamp(self, index: int):
+        s = index or ''
+        return f"dilatmx{s} {1 + self.a*0.01}\nchkdilatmx{s} {int(not self.x)}"
+
+
+_ex1 = set((MolecularDynamics, StructuralOptimization, FIRE, MonteCarloSampling))
+_ex2 = set((CellOptimization, CellOptimizationOnVector))
+
+
 # check se non SCF che bande siano specificate
```

### Comparing `pynabi-0.1.1/src/pynabi.egg-info/PKG-INFO` & `pynabi-0.1.2/src/pynabi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,222 +1,225 @@
-Metadata-Version: 2.1
-Name: pynabi
-Version: 0.1.1
-Summary: A package to easily create Abinit input files
-Author: Federico Guglielmi
-License: MIT License
-        
-        Copyright (c) 2023 Federico Guglielmi
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/Fedesky25/pynabi
-Project-URL: Bug Tracker, https://github.com/Fedesky25/pynabi/issues
-Project-URL: Documentation, https://github.com/Fedesky25/pynabi/wiki
-Project-URL: Repository, https://github.com/Fedesky25/pynabi.git
-Project-URL: Changelog, https://github.com/Fedesky25/pynabi/blob/master/CHANGELOG.md
-Keywords: abinit
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PynAbi
-
-Python package to easily create [Abinit](https://www.abinit.org/) input files.
-
-```cmd
-pip install pynabi
-```
-
-## Example
-
-```python
-from pynabi import createAbi, DataSet, AbIn, AbOut
-from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
-from pynabi.calculation import ToleranceOn, EnergyCutoff, MaxSteps, SCFMixing, NonSelfConsistentCalc
-from pynabi.crystal import Atom, FluoriteLike
-from pynabi.occupation import OccupationPerBand
-from pynabi.units import eV, nm
-
-# create manually an atom -> Atom(<Z>, <pseudo potential name>)
-# or using sensible defaults as follows
-Zr = Atom.of("Zr")  # Z=40 and pseudos located at "Zr.psp8"
-Oxy = Atom.of("O")  # Z=8 and pseudos located at "O.psp8"
-
-# base dataset with common variables
-base = DataSet(
-    AbOut("./scf/scf"),                             # prefix for output files
-    AbIn().PseudoPotentials("./pseudos/PBE-SR"),    # folder with pseudo potentials
-
-    FluoriteLike(Zr, Oxy, 0.5135*nm),               # creates AtomBasis and Lattice of a crystal like fluorite
-                                                    # with lattice constant 0.5135nm
-
-    SymmetricGrid(BZ.Irreducible, UsualKShifts.FCC) # easily define kptopt, ngkpt, nshiftk, kpt
-        .ofMonkhorstPack(4),
-
-    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density 
-                                                    # based on the last 10 iteration
-
-    ToleranceOn.EnergyDifference(1e-6),             # expressively define the tolerance
-    MaxSteps(30)                                    # nstep
-)
-
-# set the default energy unit in eV (from now on)
-eV.setAsReference()
-
-# datasets to see the convergenge as a function of energy
-sets = [DataSet(EnergyCutoff(8.0 + i*0.25)) for i in range(0,17)]
-
-# final non-self-consistent round to find bands 
-bands = DataSet(
-    NonSelfConsistentCalc(),
-    ToleranceOn.WavefunctionSquaredResidual(1e-12),
-    AbIn().ElectronDensity(sets[-1]),                   # get the electron density from the last dataset
-    OccupationPerBand(2.0, repeat=8),                   # same number of bands (max 8) for each k point
-    Path.auto(10, "GXWKGLUWLK", CriticalPointsOf.FCC)   # easily define a path in the k-space   
-)
-
-with open("./out.txt", 'w') as f:
-    f.write(createAbi(base, *sets, bands))
-```
-
-<details>
-<summary><b>Output</b></summary>
-
-```txt
-ndtset 18
-
-# Atoms definition
-ntypat 2
-znucl 8 40
-pseudos "O.psp8, Zr.psp8"
-
-# Common DataSet
-natoms 3
-typeat 2 1 1
-xred 0 0 0   0.3333333333333333 0.3333333333333333 0.3333333333333333   0.6666666666666666 0.6666666666666666 0.6666666666666666
-outdata_prefix "./scf/scf"
-pp_dirpath "./pseudos/PBE-SR"
-scalecart 0.5135 0.5135 0.5135 nm
-rprim 0.5 0.5 0.0   0.0 0.5 0.5   0.5 0.0 0.5
-ngkpt 4 4 4
-iscf 17
-npulayit 10
-toldfe 1e-06
-nstep 30
-
-# DataSet 1
-ecut1 8.0 eV
-
-# DataSet 2
-ecut2 8.25 eV
-
-# DataSet 3
-ecut3 8.5 eV
-
-# DataSet 4
-ecut4 8.75 eV
-
-# DataSet 5
-ecut5 9.0 eV
-
-# DataSet 6
-ecut6 9.25 eV
-
-# DataSet 7
-ecut7 9.5 eV
-
-# DataSet 8
-ecut8 9.75 eV
-
-# DataSet 9
-ecut9 10.0 eV
-
-# DataSet 10
-ecut10 10.25 eV
-
-# DataSet 11
-ecut11 10.5 eV
-
-# DataSet 12
-ecut12 10.75 eV
-
-# DataSet 13
-ecut13 11.0 eV
-
-# DataSet 14
-ecut14 11.25 eV
-
-# DataSet 15
-ecut15 11.5 eV
-
-# DataSet 16
-ecut16 11.75 eV
-
-# DataSet 17
-ecut17 12.0 eV
-
-# DataSet 18
-iscf18 -2
-tolwfr18 1e-12
-getden18 17
-occopt18 0
-occ18 8*2.0
-bands18 8
-kptopt18 -9
-kptbounds18 0 0 0  0.0 0.5 0.5  0.25 0.75 0.5  0.375 0.75 0.375  0 0 0  0.5 0.5 0.5  0.25 0.625 0.625  0.25 0.75 0.5  0.5 0.5 0.5  0.375 0.75 0.375
-ndivsm18 10
-```
-
-</details>
-
-## Features
-
- - Multi dataset support
- - Helper functions for common crystal structures (caesium chloride, rock-salt, fluorite, zincblende, wurtzite, nickeline, HCP)
- - Registered critical points of and methodsto create lattices of CUB, BCC, FCC, HEX, TET, BCT, ORC, ORCC
- - Smooth experience in defining the k-points
- - Handy management of [file handling variables](https://docs.abinit.org/variables/files/)
- - Almost full covarage of [basic input variables](https://docs.abinit.org/variables/basic/) (missing nbandhf, symrel, tnons, wvl_hgrid)
- - Partial coverage of [ground state variables](https://docs.abinit.org/variables/gstate/)
- - Partial coverage of [relaxation variables](https://docs.abinit.org/variables/rlx/)
- - _More to come..._
-
-## Why PynAbi over pure Abinit files?
-
-If you're a very experienced Abinit user who knows its variables and their possible values (and associated meaning), then this package probably isn't for you.
-For all other users, on top of all the aforementioned features, here's a list of reasons why you could find PynAbi useful:
-
- 1. You have all the power of coding to generate Abinit instructions, e.g. reusability, loops to generate datasets programmatically
- 2. It provides some useful presets and helper functions/methods that allows you to skip to the fun part of the simulation
- 3. Under the hood, it checks for the validity of variable values *before* starting Abinit
- 4. It makes use of expressive declarations and definition, leading to readable and comprehensible istructions
- 5. If you're using a code editor (with autocompletition), you'll get suggetions of all the possible options in a more natural language 
-
-Some prior knowledge of Abinit (and DFT in general) is nonetheless needed to fully understand what actually is to be simulated: this package only provides a handier way to generate the required files.
-
-## Documentation
-
-Although currently severely incomplete, a wiki is available on the [GitHub repository Wiki](https://github.com/Fedesky25/pynabi/wiki). Ideally a wiki for this package shouldn't be needed if your editor has some autocompletition: the aim is to document every class and function with a detailed description taken from the relevant parts of ABINIT documentation. 
+Metadata-Version: 2.1
+Name: pynabi
+Version: 0.1.2
+Summary: A package to easily create Abinit input files
+Author: Federico Guglielmi
+License: MIT License
+        
+        Copyright (c) 2023 Federico Guglielmi
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/Fedesky25/pynabi
+Project-URL: Bug Tracker, https://github.com/Fedesky25/pynabi/issues
+Project-URL: Documentation, https://github.com/Fedesky25/pynabi/wiki
+Project-URL: Repository, https://github.com/Fedesky25/pynabi.git
+Project-URL: Changelog, https://github.com/Fedesky25/pynabi/blob/master/CHANGELOG.md
+Keywords: abinit
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PynAbi
+
+Python package to easily create [Abinit](https://www.abinit.org/) input files.
+
+```cmd
+pip install pynabi
+```
+
+## Example
+
+```python
+from pynabi import createAbi, DataSet, AbIn, AbOut
+from pynabi.kspace import CriticalPointsOf, BZ, SymmetricGrid, UsualKShifts, Path
+from pynabi.calculation import ToleranceOn, EnergyCutoff, MaxSteps, SCFMixing, NonSelfConsistentCalc
+from pynabi.crystal import Atom, FluoriteLike
+from pynabi.occupation import OccupationPerBand
+from pynabi.units import eV, nm
+
+# create manually an atom -> Atom(<Z>, <pseudo potential name>)
+# or using sensible defaults as follows
+Zr = Atom.of("Zr")  # Z=40 and pseudos located at "Zr.psp8"
+Oxy = Atom.of("O")  # Z=8 and pseudos located at "O.psp8"
+
+# base dataset with common variables
+base = DataSet(
+    AbOut("./scf/scf"),                             # prefix for output files
+    AbIn().PseudoPotentials("./pseudos/PBE-SR"),    # folder with pseudo potentials
+
+    FluoriteLike(Zr, Oxy, 0.5135*nm),               # creates AtomBasis and Lattice of a crystal like fluorite
+                                                    # with lattice constant 0.5135nm
+
+    SymmetricGrid(BZ.Irreducible, UsualKShifts.FCC) # easily define kptopt, ngkpt, nshiftk, kpt
+        .ofMonkhorstPack(4),
+
+    SCFMixing(density=True).Pulay(10),              # scf cycle with Pulay mixing of the density 
+                                                    # based on the last 10 iteration
+
+    ToleranceOn.EnergyDifference(1e-6),             # expressively define the tolerance
+    MaxSteps(30)                                    # nstep
+)
+
+# set the default energy unit in eV (from now on)
+eV.setAsReference()
+
+# datasets to see the convergenge as a function of energy
+sets = [DataSet(EnergyCutoff(8.0 + i*0.25)) for i in range(0,17)]
+
+# final non-self-consistent round to find bands 
+bands = DataSet(
+    NonSelfConsistentCalc(),
+    ToleranceOn.WavefunctionSquaredResidual(1e-12),
+    AbIn().ElectronDensity(sets[-1]),                   # get the electron density from the last dataset
+    OccupationPerBand(2.0, repeat=8),                   # same number of bands (max 8) for each k point
+    Path.auto(10, "GXWKGLUWLK", CriticalPointsOf.FCC)   # easily define a path in the k-space   
+)
+
+with open("./out.txt", 'w') as f:
+    f.write(createAbi(base, *sets, bands))
+```
+
+<details>
+<summary><b>Output</b></summary>
+
+```txt
+ndtset 18
+
+# Atoms definition
+ntypat 2
+znucl 40 8
+pseudos "Zr.psp8, O.psp8"
+
+# Common DataSet
+natom 3
+typat 1 2 2
+xred 0 0 0   0.3333333333333333 0.3333333333333333 0.3333333333333333   0.6666666666666666 0.6666666666666666 0.6666666666666666
+outdata_prefix "./scf/scf"
+pp_dirpath "./pseudos/PBE-SR"
+scalecart 0.5135 0.5135 0.5135 nm
+rprim 0.5 0.5 0.0   0.0 0.5 0.5   0.5 0.0 0.5
+kptopt 1
+nshiftk 4
+shiftk 0.5 0.5 0.5 0.5 0.0 0.0 0.0 0.5 0.0 0.0 0.0 0.5
+ngkpt 4 4 4
+iscf 17
+npulayit 10
+toldfe 1e-06
+nstep 30
+
+# DataSet 1
+ecut1 8.0 eV
+
+# DataSet 2
+ecut2 8.25 eV
+
+# DataSet 3
+ecut3 8.5 eV
+
+# DataSet 4
+ecut4 8.75 eV
+
+# DataSet 5
+ecut5 9.0 eV
+
+# DataSet 6
+ecut6 9.25 eV
+
+# DataSet 7
+ecut7 9.5 eV
+
+# DataSet 8
+ecut8 9.75 eV
+
+# DataSet 9
+ecut9 10.0 eV
+
+# DataSet 10
+ecut10 10.25 eV
+
+# DataSet 11
+ecut11 10.5 eV
+
+# DataSet 12
+ecut12 10.75 eV
+
+# DataSet 13
+ecut13 11.0 eV
+
+# DataSet 14
+ecut14 11.25 eV
+
+# DataSet 15
+ecut15 11.5 eV
+
+# DataSet 16
+ecut16 11.75 eV
+
+# DataSet 17
+ecut17 12.0 eV
+
+# DataSet 18
+iscf18 -2
+tolwfr18 1e-12
+getden18 17
+occopt18 0
+occ18 8*2.0
+band18 8
+kptopt18 -9
+kptbounds18 0 0 0  0.0 0.5 0.5  0.25 0.75 0.5  0.375 0.75 0.375  0 0 0  0.5 0.5 0.5  0.25 0.625 0.625  0.25 0.75 0.5  0.5 0.5 0.5  0.375 0.75 0.375
+ndivsm18 10
+```
+
+</details>
+
+## Features
+
+ - Multi dataset support
+ - Helper functions for common crystal structures (caesium chloride, rock-salt, fluorite, zincblende, wurtzite, nickeline, HCP)
+ - Registered critical points of and methodsto create lattices of CUB, BCC, FCC, HEX, TET, BCT, ORC, ORCC
+ - Smooth experience in defining the k-points
+ - Handy management of [file handling variables](https://docs.abinit.org/variables/files/)
+ - Almost full covarage of [basic input variables](https://docs.abinit.org/variables/basic/) (missing nbandhf, symrel, tnons, wvl_hgrid)
+ - Partial coverage of [ground state variables](https://docs.abinit.org/variables/gstate/)
+ - Partial coverage of [relaxation variables](https://docs.abinit.org/variables/rlx/)
+ - _More to come..._
+
+## Why PynAbi over pure Abinit files?
+
+If you're a very experienced Abinit user who knows its variables and their possible values (and associated meaning), then this package probably isn't for you.
+For all other users, on top of all the aforementioned features, here's a list of reasons why you could find PynAbi useful:
+
+ 1. You have all the power of coding to generate Abinit instructions, e.g. reusability, loops to generate datasets programmatically
+ 2. It provides some useful presets and helper functions/methods that allows you to skip to the fun part of the simulation
+ 3. Under the hood, it checks for the validity of variable values *before* starting Abinit
+ 4. It makes use of expressive declarations and definition, leading to readable and comprehensible istructions
+ 5. If you're using a code editor (with autocompletition), you'll get suggetions of all the possible options in a more natural language 
+
+Some prior knowledge of Abinit (and DFT in general) is nonetheless needed to fully understand what actually is to be simulated: this package only provides a handier way to generate the required files.
+
+## Documentation
+
+Although currently severely incomplete, a wiki is available on the [GitHub repository Wiki](https://github.com/Fedesky25/pynabi/wiki). Ideally a wiki for this package shouldn't be needed if your editor has some autocompletition: the aim is to document every class and function with a detailed description taken from the relevant parts of ABINIT documentation.
```

