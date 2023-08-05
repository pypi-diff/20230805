# Comparing `tmp/volumizer-0.1.2.tar.gz` & `tmp/volumizer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volumizer-0.1.2.tar", max compression
+gzip compressed data, was "volumizer-0.1.3.tar", max compression
```

## Comparing `volumizer-0.1.2.tar` & `volumizer-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0     1076 2023-07-08 16:14:15.259791 volumizer-0.1.2/LICENSE
--rw-r--r--   0        0        0     7549 2023-07-15 16:57:40.640503 volumizer-0.1.2/README.md
--rw-r--r--   0        0        0      539 2023-07-15 17:11:32.583344 volumizer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-08 16:14:15.272791 volumizer-0.1.2/volumizer/__init__.py
--rw-r--r--   0        0        0      364 2023-07-13 02:14:29.115227 volumizer-0.1.2/volumizer/align.py
--rw-r--r--   0        0        0      814 2023-07-13 00:38:04.356379 volumizer-0.1.2/volumizer/constants.py
--rw-r--r--   0        0        0     6239 2023-07-08 16:14:15.273791 volumizer-0.1.2/volumizer/fib_sphere.py
--rw-r--r--   0        0        0      203 2023-07-09 18:40:05.790711 volumizer-0.1.2/volumizer/paths.py
--rw-r--r--   0        0        0     7624 2023-07-15 16:44:53.148182 volumizer-0.1.2/volumizer/pdb.py
--rw-r--r--   0        0        0     8393 2023-07-08 16:14:15.273791 volumizer-0.1.2/volumizer/protein_components.py
--rw-r--r--   0        0        0     1196 2023-07-14 01:49:45.715179 volumizer-0.1.2/volumizer/types.py
--rw-r--r--   0        0        0     6005 2023-07-15 16:33:07.883752 volumizer-0.1.2/volumizer/utils.py
--rw-r--r--   0        0        0     5620 2023-07-15 16:03:48.548894 volumizer-0.1.2/volumizer/volumizer.py
--rw-r--r--   0        0        0    25086 2023-07-14 02:13:44.025309 volumizer-0.1.2/volumizer/voxel.py
--rw-r--r--   0        0        0     8378 1970-01-01 00:00:00.000000 volumizer-0.1.2/setup.py
--rw-r--r--   0        0        0     8041 1970-01-01 00:00:00.000000 volumizer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-08 16:14:15.259791 volumizer-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7072 2023-08-05 04:17:13.959840 volumizer-0.1.3/README.md
+-rw-r--r--   0        0        0      539 2023-08-05 04:17:13.959840 volumizer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-08 16:14:15.272791 volumizer-0.1.3/volumizer/__init__.py
+-rw-r--r--   0        0        0      364 2023-07-13 02:14:29.115227 volumizer-0.1.3/volumizer/align.py
+-rw-r--r--   0        0        0      814 2023-07-13 00:38:04.356379 volumizer-0.1.3/volumizer/constants.py
+-rw-r--r--   0        0        0     6239 2023-07-08 16:14:15.273791 volumizer-0.1.3/volumizer/fib_sphere.py
+-rw-r--r--   0        0        0      203 2023-07-09 18:40:05.790711 volumizer-0.1.3/volumizer/paths.py
+-rw-r--r--   0        0        0     8364 2023-08-05 04:17:13.972841 volumizer-0.1.3/volumizer/pdb.py
+-rw-r--r--   0        0        0     1196 2023-07-14 01:49:45.715179 volumizer-0.1.3/volumizer/types.py
+-rw-r--r--   0        0        0     4925 2023-08-05 04:17:13.972841 volumizer-0.1.3/volumizer/utils.py
+-rw-r--r--   0        0        0     5620 2023-07-15 16:03:48.548894 volumizer-0.1.3/volumizer/volumizer.py
+-rw-r--r--   0        0        0    25086 2023-07-14 02:13:44.025309 volumizer-0.1.3/volumizer/voxel.py
+-rw-r--r--   0        0        0     7564 1970-01-01 00:00:00.000000 volumizer-0.1.3/PKG-INFO
```

### Comparing `volumizer-0.1.2/LICENSE` & `volumizer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.2/README.md` & `volumizer-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,35 +55,30 @@
 #  e.g. the default "END" allows Pymol to load the resulting PDB file as two separate objects, one for the cleaned input, and one for the volumes
 pdb_lines = pdb.make_volumized_pdb_lines([cleaned_structure, volumes_structure], deliminator="END")
 pdb.save_pdb_lines(pdb_lines, "volumized_pdb.pdb")
 
 volumes_df.to_json("volumized_df.json")
 ```
 
-## Changing Resolution, Modifying PDB Cleaning, and Beyond
-If you are interested in additional control over the volumizing method, the resolution of the voxels can be changed,
-you can skip cleaning, or modify which residues are kept/removed by the cleaning process
+## Changing Resolution, and Beyond
+If you are interested in additional control over the volumizing method:
+- the resolution of the voxels can be changed
+- cleaning can be skipped
 
 Note: the default voxel resolution is 3.0 Angstroms, which gives sensible results in the majority of cases.
 Higher resolutions especially < 2.0 Angstroms will often find small paths through a protein structure, making e.g. cavities look like pores, etc.
 Lower resolutions are faster to compute, but may begin to under-estimate the true volume of solvent occluded elements.
 
 Note: by default all residues that make L- or D- peptide bonds are retained through cleaning (e.g. Non-canonicals are kept, even if they are heteroatoms in PDB structure).
 By constrast all non-covalently attached residues are removed.  Currently glycan residues are also removed as they make non-peptide bonds, below is shown an example of how would would retain glycans.
 
 ```
 from volumizer import volumizer, pdb, utils
 
-# specify whichever residues you are interested in keeping during cleaning, or having additionally removed
-KEEP_RESIDUE_NAMES = {"GAL", "NAG", "MAN", "GLC"}  # some example sugar residues to keep when cleaning
-REMOVE_RESIDUE_NAMES = {"SME"}  # some example NCAAs to remove when cleaning
-
 utils.set_resolution(2.0)
-utils.add_protein_components(KEEP_RESIDUE_NAMES)
-utils.remove_protein_components(REMOVE_RESIDUE_NAMES)
 
 pdb_structure = pdb.load_structure("my_input.pdb")
 cleaned_structure = volumizer.prepare_pdb_structure(pdb_structure)  # skip this if you want to keep the exact input structure
 volumes_df, volumes_structure = volumizer.annotate_structure_volumes(cleaned_structure)
 
 # take the cleaned input and annotated volumes and convert them to a PDB format string and then save
 #  modify the `deliminator` to suit your visualization preference
```

### Comparing `volumizer-0.1.2/pyproject.toml` & `volumizer-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volumizer"
-version = "0.1.2"
+version = "0.1.3"
 description = "Search the RCSB for occluded volumes like cavities, pockets, and pores."
 authors = ["Aron Broom <broomsday@gmail.com>"]
 readme = "README.md"
 packages = [{include = "volumizer"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `volumizer-0.1.2/volumizer/constants.py` & `volumizer-0.1.3/volumizer/constants.py`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.2/volumizer/fib_sphere.py` & `volumizer-0.1.3/volumizer/fib_sphere.py`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.2/volumizer/pdb.py` & `volumizer-0.1.3/volumizer/pdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,51 @@
 """
 Functions for parsing, cleaning, and modifying PDBs.
 """
 
 from pathlib import Path
 
 import biotite.structure as bts
-from biotite.structure.io import load_structure  # in use by modules importing pdb.py
+from biotite.structure.io import load_structure as biotite_load_structure
+from biotite.structure.io import mmtf, pdbx, pdb
+from biotite import InvalidFileError
 from pyntcloud.structures.voxelgrid import VoxelGrid
 import pandas as pd
 import numpy as np
 
 from volumizer.constants import (
     VOXEL_TYPE_CHAIN_MAP,
     VOXEL_TYPE_ATOM_MAP,
     VOXEL_TYPE_ELEMENT_MAP,
 )
 from volumizer.types import VoxelGroup
 from volumizer import utils
 
 
+def load_structure(file_path: Path) -> bts.AtomArray:
+    """
+    Load various structure formats.
+    """
+    try:
+        if file_path.suffix == ".pdb":
+            file = pdb.PDBFile.read(file_path)
+            assembly = pdb.get_assembly(file, model=1)
+        elif file_path.suffix == ".cif":
+            file = pdbx.PDBxFile.read(file_path)
+            assembly = pdbx.get_assembly(file, model=1)
+        elif file_path.suffix == ".mmtf":
+            file = mmtf.MMTFFile.read(file_path)
+            assembly = mmtf.get_assembly(file, model=1)
+        else:
+            return biotite_load_structure(file_path)
+        return assembly
+    except InvalidFileError:
+        return biotite_load_structure(file_path)
+
+
 def save_pdb_lines(pdb_lines: list[str], output: Path | str) -> None:
     """
     Save individual pdb lines to a file.
     """
     if isinstance(output, (Path, str)):
         with open(output, mode="w", encoding="utf-8") as out_file:
             out_file.writelines("%s\n" % line for line in pdb_lines)
@@ -40,17 +63,15 @@
         elif structure.stack_depth() > 1:
             new_structure = structure[0]
             for model in structure[1:]:
                 new_structure += model
             structure = new_structure
 
     if not utils.KEEP_NON_PROTEIN:
-        structure = structure[
-            np.isin(structure.res_name, list(utils.get_protein_components()))
-        ]
+        structure = structure[bts.filter_amino_acids(structure)]
 
     if not utils.KEEP_HYDROGENS:
         structure = structure[~np.isin(structure.element, ["H"])]
 
     return structure
```

### Comparing `volumizer-0.1.2/volumizer/types.py` & `volumizer-0.1.3/volumizer/types.py`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.2/volumizer/utils.py` & `volumizer-0.1.3/volumizer/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,63 +4,26 @@
 
 
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
-from volumizer import constants, protein_components
+from volumizer import constants
 from volumizer.types import Annotation, VoxelGroup
 from volumizer.paths import C_CODE_DIR
 
 
 VOXEL_SIZE = constants.VOXEL_SIZE
 VOXEL_VOLUME = VOXEL_SIZE**3
 KEEP_MODELS = (
     True  # by default keep all models in case they are other biological assembly units
 )
 KEEP_NON_PROTEIN = False  # by default only keep protein residues
 KEEP_HYDROGENS = False  # by default remove hydrogens
-UTILS_PROTEIN_COMPONENTS = protein_components.PROTEIN_COMPONENTS
-
-
-def get_protein_components() -> set[str]:
-    """
-    Return the protein components definition currently in use.
-    """
-    return UTILS_PROTEIN_COMPONENTS
-
-
-def reset_protein_components():
-    """
-    Reset the protein components definition to the default.
-    """
-    global UTILS_PROTEIN_COMPONENTS
-
-    UTILS_PROTEIN_COMPONENTS = protein_components.PROTEIN_COMPONENTS
-
-
-def add_protein_components(additional_components: set[str]) -> None:
-    """
-    Extend the protein components definition currently in use with additional components
-    """
-    global UTILS_PROTEIN_COMPONENTS
-
-    UTILS_PROTEIN_COMPONENTS = UTILS_PROTEIN_COMPONENTS.union(
-        set(additional_components)
-    )
-
-
-def remove_protein_components(disallowed_components: set[str]) -> None:
-    """
-    Reduce the protein components definition currently in use with blacklisted components.
-    """
-    global UTILS_PROTEIN_COMPONENTS
-
-    UTILS_PROTEIN_COMPONENTS = UTILS_PROTEIN_COMPONENTS - set(disallowed_components)
 
 
 def set_resolution(resolution: float) -> None:
     """
     Set the value of the VOXEL_SIZE and VOXEL_VOLUME global constants.
     """
     global VOXEL_SIZE
```

### Comparing `volumizer-0.1.2/volumizer/volumizer.py` & `volumizer-0.1.3/volumizer/volumizer.py`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.2/volumizer/voxel.py` & `volumizer-0.1.3/volumizer/voxel.py`

 * *Files identical despite different names*

### Comparing `volumizer-0.1.2/setup.py` & `volumizer-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,148 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: volumizer
+Version: 0.1.3
+Summary: Search the RCSB for occluded volumes like cavities, pockets, and pores.
+Author: Aron Broom
+Author-email: broomsday@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: biotite (>=0.37.0,<0.38.0)
+Requires-Dist: pyntcloud (>=0.1.5,<0.2.0)
+Description-Content-Type: text/markdown
+
+`volumizer` discovers and annotates occluded volumes in proteins including:
+- `cavities`: Volumes within a protein that do not make any contacts with bulk solvent. Useful for e.g. carrying cargo.
+- `pockets`: Volumes on the protein surface that make a single contact with bulk solvent.  Useful for e.g. ligand binding or catalysis.
+- `pores`: Volumes connecting two bulk solvent surfaces.  Useful for e.g. filtering solutes.
+- `hubs`: Volumes connecting more than two bulk solvent surfaces.  Useful for e.g. containing a small reaction volume.
+
+# Example Identified Volume
+
+Here is shown an example pore identified and annotated (red) in PDB 4JPN (green).
+![image](images/pore_annotation.png)
+
+The same pore volume annotated (red) shown as a slice through the protein (grey).
+![image](images/pore_slice.png)
+
+The dataframe output shows volume/dimensinos of each occluded volume in the structure
+|    | id |  type  |  volume  |    x    |    y    |    z    |
+|----|----|--------|----------|---------|---------|---------|
+| 0  | 0  |   pore | 38286.0  | 108.221 |  38.574 |  36.310 |
+| 1  | 0  | pocket |   189.0  |   8.214 |   5.628 |   0.000 |
+| 2  | 1  | pocket |   162.0  |   6.635 |   3.843 |   2.840 |
+| 3  | 2  | pocket |   162.0  |   7.298 |   4.002 |   2.557 |
+| 4  | 3  | pocket |   162.0  |  10.757 |   2.701 |   0.000 |
+| 5  | 4  | pocket |   135.0  |   6.000 |   6.000 |   0.000 |
+
+# Installation
+The package is published on PyPi, `pip install volumizer`.
+
+## Developing the Volumizer Package
+If you want to develop the package, `poetry install` within the repository.
+Test with `pytest` within the repository base directory
+
+# Usage
+Using the test file `tests/pdbs/4jpn.pdb` try out the following:
+
+## Volumize a PDB and Save the Volumized PDB and DataFrame
+Performing end-to-end loading, cleaning, volumizing, and saving is done with a single convenience function:
+
+```
+from volumizer import volumizer
+
+volumizer.volumize_pdb_and_save("my_input.pdb", "volumized_pdb.pdb", "volumized_df.json")
+```
+
+## Load a PDB as a Biotite Structure, Clean, Volumize, and Save Output
+If you want access to the individual end-products: volume dataframe, the input structure after cleaning, and the structure of the volumes:
+
+```
+from volumizer import volumizer, pdb
+
+pdb_structure = pdb.load_structure("my_input.pdb")
+volumes_df, cleaned_structure, volumes_structure = volumizer.volumize_structure(pdb_structure)
+
+# take the cleaned input and annotated volumes and convert them to a PDB format string and then save
+#  modify the `deliminator` to suit your visualization preference
+#  e.g. the default "END" allows Pymol to load the resulting PDB file as two separate objects, one for the cleaned input, and one for the volumes
+pdb_lines = pdb.make_volumized_pdb_lines([cleaned_structure, volumes_structure], deliminator="END")
+pdb.save_pdb_lines(pdb_lines, "volumized_pdb.pdb")
+
+volumes_df.to_json("volumized_df.json")
+```
+
+## Changing Resolution, and Beyond
+If you are interested in additional control over the volumizing method:
+- the resolution of the voxels can be changed
+- cleaning can be skipped
+
+Note: the default voxel resolution is 3.0 Angstroms, which gives sensible results in the majority of cases.
+Higher resolutions especially < 2.0 Angstroms will often find small paths through a protein structure, making e.g. cavities look like pores, etc.
+Lower resolutions are faster to compute, but may begin to under-estimate the true volume of solvent occluded elements.
+
+Note: by default all residues that make L- or D- peptide bonds are retained through cleaning (e.g. Non-canonicals are kept, even if they are heteroatoms in PDB structure).
+By constrast all non-covalently attached residues are removed.  Currently glycan residues are also removed as they make non-peptide bonds, below is shown an example of how would would retain glycans.
+
+```
+from volumizer import volumizer, pdb, utils
+
+utils.set_resolution(2.0)
+
+pdb_structure = pdb.load_structure("my_input.pdb")
+cleaned_structure = volumizer.prepare_pdb_structure(pdb_structure)  # skip this if you want to keep the exact input structure
+volumes_df, volumes_structure = volumizer.annotate_structure_volumes(cleaned_structure)
+
+# take the cleaned input and annotated volumes and convert them to a PDB format string and then save
+#  modify the `deliminator` to suit your visualization preference
+#  e.g. the default "END" allows Pymol to load the resulting PDB file as two separate objects, one for the cleaned input, and one for the volumes
+pdb_lines = pdb.make_volumized_pdb_lines([cleaned_structure, volumes_structure], deliminator="END")
+pdb.save_pdb_lines(pdb_lines, "volumized_pdb.pdb")
+
+volumes_df.to_json("volumized_df.json")
+```
+
+# How It Works
+`volumizer` identifies hydrated volumes in a protein structure that are not fully solvent exposed, e.g. a binding pocket.
+It then computes the volume and dimensions of these and outputs that information along with an annotated 
+version of the input PDB showing where these volumes are (which can be visualized in e.g. Pymol, Chimerax, etc.).
+
+## Identifying hydrated volumes
+1. A large voxel-grid is built around the atoms of the protein or other structure supplied.
+2. All voxels within a van der Waals radius of a protein or other atom is flagged as being `non-solvent`
+3. Remaining `solvent` atoms are then broken into two groups: `bulk solvent` and `occluded volumes`
+   This is done by tracing a vector along each ordinal axis from a given voxel and if 2 or more of these vectors would
+   cross a `non-solvent` voxel, then the query voxel is identified as an `occluded volume` to be further analyzed
+   otherwise it is considered `bulk solvent`
+   The intention is to identify points on the grid that are outside the protein as `bulk solvent`
+4. All `occluded volume` voxels are then grouped into a number of continuous volumes
+5. For each continous volume the number of distinct surfaces that contact `bulk solvent` voxels is computed and used
+   to indicate the volume type:
+   0 surfaces interacting with solvent: `cavity`
+   1 surface interacting with solvent: `pocket`
+   2 surfaces interacting with solvent: `pore`
+   3+ surfaces interacting with solvent: `hub`
+
+## Annotations
+
+### Pandas DataFrame
+Annotations are given as a pandas data frame saved as a .json file.  The annotation lists all hydrated volumes ordered by
+total volume, giving the type of volume, and dimensions.
+
+### PDB File
+The input PDB file will be annotated by adding `atoms` to represent the hydrated volumes.  The ATOM entries
+contain several points of information about the volume from which they come:
+
+Type of volume: the residue name encodes the type of volume in 3-letter code
+- `OCC` for `occluded`
+- `CAV` for `cavity`
+- `POK` for `pocket`
+- `POR` for `pore`
+- `HUB` for `hub`
 
-packages = \
-['volumizer']
+Surface of the hydrated volume that interacts with bulk solvent: this is indicated by a B-factor of 50.0, whereas
+the remainder of the volume (that does not interact with the bulk solvent) has a value of 0.0.
 
-package_data = \
-{'': ['*']}
+All `atoms` of a particular volume are grouped under the same residue number.
 
-install_requires = \
-['biotite>=0.37.0,<0.38.0', 'pyntcloud>=0.1.5,<0.2.0']
-
-setup_kwargs = {
-    'name': 'volumizer',
-    'version': '0.1.2',
-    'description': 'Search the RCSB for occluded volumes like cavities, pockets, and pores.',
-    'long_description': '`volumizer` discovers and annotates occluded volumes in proteins including:\n- `cavities`: Volumes within a protein that do not make any contacts with bulk solvent. Useful for e.g. carrying cargo.\n- `pockets`: Volumes on the protein surface that make a single contact with bulk solvent.  Useful for e.g. ligand binding or catalysis.\n- `pores`: Volumes connecting two bulk solvent surfaces.  Useful for e.g. filtering solutes.\n- `hubs`: Volumes connecting more than two bulk solvent surfaces.  Useful for e.g. containing a small reaction volume.\n\n# Example Identified Volume\n\nHere is shown an example pore identified and annotated (red) in PDB 4JPN (green).\n![image](images/pore_annotation.png)\n\nThe same pore volume annotated (red) shown as a slice through the protein (grey).\n![image](images/pore_slice.png)\n\nThe dataframe output shows volume/dimensinos of each occluded volume in the structure\n|    | id |  type  |  volume  |    x    |    y    |    z    |\n|----|----|--------|----------|---------|---------|---------|\n| 0  | 0  |   pore | 38286.0  | 108.221 |  38.574 |  36.310 |\n| 1  | 0  | pocket |   189.0  |   8.214 |   5.628 |   0.000 |\n| 2  | 1  | pocket |   162.0  |   6.635 |   3.843 |   2.840 |\n| 3  | 2  | pocket |   162.0  |   7.298 |   4.002 |   2.557 |\n| 4  | 3  | pocket |   162.0  |  10.757 |   2.701 |   0.000 |\n| 5  | 4  | pocket |   135.0  |   6.000 |   6.000 |   0.000 |\n\n# Installation\nThe package is published on PyPi, `pip install volumizer`.\n\n## Developing the Volumizer Package\nIf you want to develop the package, `poetry install` within the repository.\nTest with `pytest` within the repository base directory\n\n# Usage\nUsing the test file `tests/pdbs/4jpn.pdb` try out the following:\n\n## Volumize a PDB and Save the Volumized PDB and DataFrame\nPerforming end-to-end loading, cleaning, volumizing, and saving is done with a single convenience function:\n\n```\nfrom volumizer import volumizer\n\nvolumizer.volumize_pdb_and_save("my_input.pdb", "volumized_pdb.pdb", "volumized_df.json")\n```\n\n## Load a PDB as a Biotite Structure, Clean, Volumize, and Save Output\nIf you want access to the individual end-products: volume dataframe, the input structure after cleaning, and the structure of the volumes:\n\n```\nfrom volumizer import volumizer, pdb\n\npdb_structure = pdb.load_structure("my_input.pdb")\nvolumes_df, cleaned_structure, volumes_structure = volumizer.volumize_structure(pdb_structure)\n\n# take the cleaned input and annotated volumes and convert them to a PDB format string and then save\n#  modify the `deliminator` to suit your visualization preference\n#  e.g. the default "END" allows Pymol to load the resulting PDB file as two separate objects, one for the cleaned input, and one for the volumes\npdb_lines = pdb.make_volumized_pdb_lines([cleaned_structure, volumes_structure], deliminator="END")\npdb.save_pdb_lines(pdb_lines, "volumized_pdb.pdb")\n\nvolumes_df.to_json("volumized_df.json")\n```\n\n## Changing Resolution, Modifying PDB Cleaning, and Beyond\nIf you are interested in additional control over the volumizing method, the resolution of the voxels can be changed,\nyou can skip cleaning, or modify which residues are kept/removed by the cleaning process\n\nNote: the default voxel resolution is 3.0 Angstroms, which gives sensible results in the majority of cases.\nHigher resolutions especially < 2.0 Angstroms will often find small paths through a protein structure, making e.g. cavities look like pores, etc.\nLower resolutions are faster to compute, but may begin to under-estimate the true volume of solvent occluded elements.\n\nNote: by default all residues that make L- or D- peptide bonds are retained through cleaning (e.g. Non-canonicals are kept, even if they are heteroatoms in PDB structure).\nBy constrast all non-covalently attached residues are removed.  Currently glycan residues are also removed as they make non-peptide bonds, below is shown an example of how would would retain glycans.\n\n```\nfrom volumizer import volumizer, pdb, utils\n\n# specify whichever residues you are interested in keeping during cleaning, or having additionally removed\nKEEP_RESIDUE_NAMES = {"GAL", "NAG", "MAN", "GLC"}  # some example sugar residues to keep when cleaning\nREMOVE_RESIDUE_NAMES = {"SME"}  # some example NCAAs to remove when cleaning\n\nutils.set_resolution(2.0)\nutils.add_protein_components(KEEP_RESIDUE_NAMES)\nutils.remove_protein_components(REMOVE_RESIDUE_NAMES)\n\npdb_structure = pdb.load_structure("my_input.pdb")\ncleaned_structure = volumizer.prepare_pdb_structure(pdb_structure)  # skip this if you want to keep the exact input structure\nvolumes_df, volumes_structure = volumizer.annotate_structure_volumes(cleaned_structure)\n\n# take the cleaned input and annotated volumes and convert them to a PDB format string and then save\n#  modify the `deliminator` to suit your visualization preference\n#  e.g. the default "END" allows Pymol to load the resulting PDB file as two separate objects, one for the cleaned input, and one for the volumes\npdb_lines = pdb.make_volumized_pdb_lines([cleaned_structure, volumes_structure], deliminator="END")\npdb.save_pdb_lines(pdb_lines, "volumized_pdb.pdb")\n\nvolumes_df.to_json("volumized_df.json")\n```\n\n# How It Works\n`volumizer` identifies hydrated volumes in a protein structure that are not fully solvent exposed, e.g. a binding pocket.\nIt then computes the volume and dimensions of these and outputs that information along with an annotated \nversion of the input PDB showing where these volumes are (which can be visualized in e.g. Pymol, Chimerax, etc.).\n\n## Identifying hydrated volumes\n1. A large voxel-grid is built around the atoms of the protein or other structure supplied.\n2. All voxels within a van der Waals radius of a protein or other atom is flagged as being `non-solvent`\n3. Remaining `solvent` atoms are then broken into two groups: `bulk solvent` and `occluded volumes`\n   This is done by tracing a vector along each ordinal axis from a given voxel and if 2 or more of these vectors would\n   cross a `non-solvent` voxel, then the query voxel is identified as an `occluded volume` to be further analyzed\n   otherwise it is considered `bulk solvent`\n   The intention is to identify points on the grid that are outside the protein as `bulk solvent`\n4. All `occluded volume` voxels are then grouped into a number of continuous volumes\n5. For each continous volume the number of distinct surfaces that contact `bulk solvent` voxels is computed and used\n   to indicate the volume type:\n   0 surfaces interacting with solvent: `cavity`\n   1 surface interacting with solvent: `pocket`\n   2 surfaces interacting with solvent: `pore`\n   3+ surfaces interacting with solvent: `hub`\n\n## Annotations\n\n### Pandas DataFrame\nAnnotations are given as a pandas data frame saved as a .json file.  The annotation lists all hydrated volumes ordered by\ntotal volume, giving the type of volume, and dimensions.\n\n### PDB File\nThe input PDB file will be annotated by adding `atoms` to represent the hydrated volumes.  The ATOM entries\ncontain several points of information about the volume from which they come:\n\nType of volume: the residue name encodes the type of volume in 3-letter code\n- `OCC` for `occluded`\n- `CAV` for `cavity`\n- `POK` for `pocket`\n- `POR` for `pore`\n- `HUB` for `hub`\n\nSurface of the hydrated volume that interacts with bulk solvent: this is indicated by a B-factor of 50.0, whereas\nthe remainder of the volume (that does not interact with the bulk solvent) has a value of 0.0.\n\nAll `atoms` of a particular volume are grouped under the same residue number.\n',
-    'author': 'Aron Broom',
-    'author_email': 'broomsday@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

