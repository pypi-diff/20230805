# Comparing `tmp/expectra-0.1.0.tar.gz` & `tmp/expectra-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/expectra-0.1.0.tar", last modified: Tue Sep  6 01:07:31 2016, max compression
+gzip compressed data, was "expectra-1.0.5.tar", last modified: Sat Aug  5 00:37:17 2023, max compression
```

## Comparing `expectra-0.1.0.tar` & `expectra-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 chill     (1000) chill     (1000)        0 2016-09-06 01:07:30.000000 expectra-0.1.0/
--rw-rw-r--   0 chill     (1000) chill     (1000)     3769 2016-09-06 01:07:30.000000 expectra-0.1.0/PKG-INFO
-drwxrwxr-x   0 chill     (1000) chill     (1000)        0 2016-09-06 01:07:30.000000 expectra-0.1.0/expectra/
--rw-rw-r--   0 chill     (1000) chill     (1000)      974 2015-05-19 15:24:06.000000 expectra-0.1.0/expectra/fft.py
--rw-rw-r--   0 chill     (1000) chill     (1000)        0 2015-05-19 15:24:06.000000 expectra-0.1.0/expectra/__init__.py
--rw-rw-r--   0 chill     (1000) chill     (1000)     5769 2016-09-02 04:53:46.000000 expectra-0.1.0/expectra/exafs.py
--rw-rw-r--   0 chill     (1000) chill     (1000)     6961 2016-09-02 04:54:15.000000 expectra-0.1.0/expectra/feff.py
--rw-rw-r--   0 chill     (1000) chill     (1000)     6871 2016-09-02 05:23:00.000000 expectra-0.1.0/expectra/io.py
-drwxrwxr-x   0 chill     (1000) chill     (1000)        0 2016-09-06 01:07:30.000000 expectra-0.1.0/bin/
--rwxrwxr-x   0 chill     (1000) chill     (1000)     4321 2015-08-04 16:03:40.000000 expectra-0.1.0/bin/expectra
--rwxrwxr-x   0 chill     (1000) chill     (1000)     5526 2016-09-02 04:55:51.000000 expectra-0.1.0/bin/pdfstats
--rwxrwxr-x   0 chill     (1000) chill     (1000)     1607 2015-05-19 15:24:06.000000 expectra-0.1.0/bin/xafsft
--rwxrwxr-x   0 chill     (1000) chill     (1000)     2796 2016-09-02 05:06:53.000000 expectra-0.1.0/bin/harmonic-sampler
--rwxrwxr-x   0 chill     (1000) chill     (1000)     1232 2016-09-06 01:06:44.000000 expectra-0.1.0/setup.py
-drwxrwxr-x   0 chill     (1000) chill     (1000)        0 2016-09-06 01:07:30.000000 expectra-0.1.0/feff/
--rw-rw-r--   0 chill     (1000) chill     (1000)      240 2016-09-01 23:00:26.000000 expectra-0.1.0/feff/Makefile
--rw-rw-r--   0 chill     (1000) chill     (1000)   403643 2016-09-01 23:00:23.000000 expectra-0.1.0/feff/feff6l.f
--rw-rw-r--   0 chill     (1000) chill     (1000)     1023 2015-05-19 15:24:06.000000 expectra-0.1.0/LICENSE.txt
--rw-rw-r--   0 chill     (1000) chill     (1000)       92 2016-09-01 23:39:37.000000 expectra-0.1.0/MANIFEST.in
--rw-rw-r--   0 chill     (1000) chill     (1000)     2654 2016-09-06 01:03:27.000000 expectra-0.1.0/README.md
-drwxrwxr-x   0 chill     (1000) chill     (1000)        0 2016-09-06 01:07:30.000000 expectra-0.1.0/expectra.egg-info/
--rw-rw-r--   0 chill     (1000) chill     (1000)        9 2016-09-06 01:07:30.000000 expectra-0.1.0/expectra.egg-info/top_level.txt
--rw-rw-r--   0 chill     (1000) chill     (1000)     3769 2016-09-06 01:07:30.000000 expectra-0.1.0/expectra.egg-info/PKG-INFO
--rw-rw-r--   0 chill     (1000) chill     (1000)        1 2016-09-06 01:07:30.000000 expectra-0.1.0/expectra.egg-info/dependency_links.txt
--rw-rw-r--   0 chill     (1000) chill     (1000)       43 2016-09-06 01:07:30.000000 expectra-0.1.0/expectra.egg-info/requires.txt
--rw-rw-r--   0 chill     (1000) chill     (1000)      374 2016-09-06 01:07:30.000000 expectra-0.1.0/expectra.egg-info/SOURCES.txt
--rw-rw-r--   0 chill     (1000) chill     (1000)       59 2016-09-06 01:07:30.000000 expectra-0.1.0/setup.cfg
+drwxrwxr-x   0 sung      (1120) sung      (1120)        0 2023-08-05 00:37:17.398795 expectra-1.0.5/
+-rw-rw-r--   0 sung      (1120) sung      (1120)     1023 2023-08-05 00:00:26.000000 expectra-1.0.5/LICENSE.txt
+-rw-rw-r--   0 sung      (1120) sung      (1120)       92 2023-08-05 00:00:26.000000 expectra-1.0.5/MANIFEST.in
+-rw-rw-r--   0 sung      (1120) sung      (1120)     4113 2023-08-05 00:37:17.398795 expectra-1.0.5/PKG-INFO
+-rw-rw-r--   0 sung      (1120) sung      (1120)     3609 2023-08-05 00:00:26.000000 expectra-1.0.5/README.md
+drwxrwxr-x   0 sung      (1120) sung      (1120)        0 2023-08-05 00:37:17.397796 expectra-1.0.5/bin/
+-rwxrwxr-x   0 sung      (1120) sung      (1120)     4325 2023-08-05 00:00:26.000000 expectra-1.0.5/bin/expectra
+-rwxrwxr-x   0 sung      (1120) sung      (1120)      460 2023-08-05 00:00:26.000000 expectra-1.0.5/bin/feff
+-rwxrwxr-x   0 sung      (1120) sung      (1120)     2794 2023-08-05 00:00:26.000000 expectra-1.0.5/bin/harmonic-sampler
+-rwxrwxr-x   0 sung      (1120) sung      (1120)     5597 2023-08-05 00:00:26.000000 expectra-1.0.5/bin/pdfstats
+-rwxrwxr-x   0 sung      (1120) sung      (1120)     1607 2023-08-05 00:00:26.000000 expectra-1.0.5/bin/xafsft
+drwxrwxr-x   0 sung      (1120) sung      (1120)        0 2023-08-05 00:37:17.397796 expectra-1.0.5/expectra/
+-rw-rw-r--   0 sung      (1120) sung      (1120)        0 2023-08-05 00:00:26.000000 expectra-1.0.5/expectra/__init__.py
+-rw-rw-r--   0 sung      (1120) sung      (1120)     5769 2023-08-05 00:00:26.000000 expectra-1.0.5/expectra/exafs.py
+-rw-rw-r--   0 sung      (1120) sung      (1120)     6985 2023-08-05 00:00:26.000000 expectra-1.0.5/expectra/feff.py
+-rw-rw-r--   0 sung      (1120) sung      (1120)      973 2023-08-05 00:00:26.000000 expectra-1.0.5/expectra/fft.py
+-rw-rw-r--   0 sung      (1120) sung      (1120)     6913 2023-08-05 00:00:26.000000 expectra-1.0.5/expectra/io.py
+drwxrwxr-x   0 sung      (1120) sung      (1120)        0 2023-08-05 00:37:17.398795 expectra-1.0.5/expectra.egg-info/
+-rw-rw-r--   0 sung      (1120) sung      (1120)     4113 2023-08-05 00:37:17.000000 expectra-1.0.5/expectra.egg-info/PKG-INFO
+-rw-rw-r--   0 sung      (1120) sung      (1120)      383 2023-08-05 00:37:17.000000 expectra-1.0.5/expectra.egg-info/SOURCES.txt
+-rw-rw-r--   0 sung      (1120) sung      (1120)        1 2023-08-05 00:37:17.000000 expectra-1.0.5/expectra.egg-info/dependency_links.txt
+-rw-rw-r--   0 sung      (1120) sung      (1120)       37 2023-08-05 00:37:17.000000 expectra-1.0.5/expectra.egg-info/requires.txt
+-rw-rw-r--   0 sung      (1120) sung      (1120)        9 2023-08-05 00:37:17.000000 expectra-1.0.5/expectra.egg-info/top_level.txt
+drwxrwxr-x   0 sung      (1120) sung      (1120)        0 2023-08-05 00:37:17.398795 expectra-1.0.5/feff/
+-rw-rw-r--   0 sung      (1120) sung      (1120)      240 2023-08-05 00:00:26.000000 expectra-1.0.5/feff/Makefile
+-rw-rw-r--   0 sung      (1120) sung      (1120)   403643 2023-08-05 00:00:26.000000 expectra-1.0.5/feff/feff6l.f
+-rw-rw-r--   0 sung      (1120) sung      (1120)       38 2023-08-05 00:37:17.398795 expectra-1.0.5/setup.cfg
+-rwxrwxr-x   0 sung      (1120) sung      (1120)     1524 2023-08-05 00:10:32.000000 expectra-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `expectra-0.1.0/PKG-INFO` & `expectra-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,93 +1,134 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: expectra
-Version: 0.1.0
+Version: 1.0.5
 Summary: Code for simulating EXAFS calculations from molecular dynamics trajectories or normal modes using FEFF
 Home-page: https://github.com/SamChill/expectra
 Author: Samuel T. Chill
 Author-email: samchill@gmail.com
 License: LICENSE.txt
-Description: Expectra
-        ========
-        
-        Introduction
-        ------------
-        
-        Expectra is program to simulate EXAFS from the outputs of molecular
-        dynamics simulations. It also has the ability to to sample structures
-        based on a harmonic potential generated from a normal modes calculation.
-        
-        The EXAFS multiple scattering calculations are performed using
-        `FEFF6-lite <http://www.feffproject.org/>`__, which was written at the
-        University of Washington by J.J. Rehr and co-workers.1
-        
-        1. J.J. Rehr, S.I. Zabinsky and R.C. Albers, "High-order multiple
-           scattering calculations of x-ray-absorption fine structure", *Phys.
-           Rev. Lett.* **69**, 3397 (1992).
-        
-        Requirements
-        ------------
-        
-        -  gfortran
-        -  MPI (e.g. OpenMPI or MPICH)
-        -  Python
-        -  numpy
-        -  mpi4py
-        
-        Installation
-        ------------
-        
-        This program is distributed as a Python package. It requires a Fortran
-        compiler (e.g. gfortran) to build the FEFF6-lite program that is
-        redistributed with the code. A MPI library (e.g. OpenMPI) is also
-        required.
-        
-        The first step is to install Python, GFortran, and MPICH. On Ubuntu this
-        can be accomplished like so:
-        
-        ::
-        
-            $ sudo apt-get install build-essential gfortran mpich python python-pip
-        
-        Once the dependencies are installed expectra (and the Python packages it
-        depends on) can be installed using pip:
-        
-        ::
-        
-            $ pip install --user expectra
-        
-        Usage
-        -----
-        
-        ::
-        
-            usage: expectra [-h] [--first-shell] [--neighbor-cutoff DISTANCE]
-                            [--multiple-scattering] [--rmax DISTANCE] [--S02 FACTOR]
-                            [--energy-shift ENERGY] [--absorber ELEMENT]
-                            [--ignore-elements ELEMENTS] [--edge EDGE] [--skip SKIP]
-                            [--every EVERY]
-                            TRAJ [TRAJ ...]
-        
-            positional arguments:
-              TRAJ                  trajectory file (POSCAR, con, xyz)
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              --first-shell         a single scattering calculation that uses an
-                                    automatically calculated reference path (default:
-                                    True)
-              --neighbor-cutoff DISTANCE
-                                    1st neighbor cutoff distance (default: 3.4)
-              --multiple-scattering
-              --rmax DISTANCE       maximum scattering half-path length
-              --S02 FACTOR          amplitude reduction factor
-              --energy-shift ENERGY
-                                    energy shift to apply in eV
-              --absorber ELEMENT    atomic symbol of the xray absorber
-              --ignore-elements ELEMENTS
-                                    comma delimited list of elements to ignore in the
-                                    scattering calculation
-              --edge EDGE           one of K, L1, L2, L3
-              --skip SKIP           number of frames to skip at the beginning
-              --every EVERY         number of frames to between each step
-        
-Platform: UNKNOWN
+License-File: LICENSE.txt
+
+Expectra
+========
+
+Introduction
+------------
+
+Expectra is program to simulate EXAFS from the outputs of molecular
+dynamics simulations. It also has the ability to to sample structures
+based on a harmonic potential generated from a normal modes calculation.
+
+The EXAFS multiple scattering calculations are performed using
+`FEFF6-lite <http://www.feffproject.org/>`__, which was written at the
+University of Washington by J.J. Rehr and co-workers.1
+
+1. J.J. Rehr, S.I. Zabinsky and R.C. Albers, “High-order multiple
+   scattering calculations of x-ray-absorption fine structure”, *Phys.
+   Rev. Lett.* **69**, 3397 (1992).
+
+Requirements
+------------
+
+-  gfortran
+-  MPI (e.g. OpenMPI or MPICH)
+-  Python
+
+   -  numpy
+   -  mpi4py
+   -  `ASE <https://wiki.fysik.dtu.dk/ase/>`__
+
+Installation
+------------
+
+This program is distributed as a Python package. It requires a Fortran
+compiler (e.g. gfortran) to build the FEFF6-lite program that is
+redistributed with the code. A MPI library (e.g. OpenMPI) is also
+required.
+
+The first step is to install Python, GFortran, and MPICH. On Ubuntu this
+can be accomplished like so:
+
+::
+
+   $ sudo apt-get install build-essential gfortran mpich python python-pip
+
+Once the dependencies are installed expectra (and the Python packages it
+depends on) can be installed using pip:
+
+::
+
+   $ pip install --user expectra
+
+Usage
+-----
+
+::
+
+   usage: expectra [-h] [--first-shell] [--neighbor-cutoff DISTANCE]
+                   [--multiple-scattering] [--rmax DISTANCE] [--S02 FACTOR]
+                   [--energy-shift ENERGY] [--absorber ELEMENT]
+                   [--ignore-elements ELEMENTS] [--edge EDGE] [--skip SKIP]
+                   [--every EVERY]
+                   TRAJ [TRAJ ...]
+
+   positional arguments:
+     TRAJ                  trajectory file (POSCAR, con, xyz)
+
+   optional arguments:
+     -h, --help            show this help message and exit
+     --first-shell         a single scattering calculation that uses an
+                           automatically calculated reference path (default:
+                           True)
+     --neighbor-cutoff DISTANCE
+                           1st neighbor cutoff distance (default: 3.4)
+     --multiple-scattering
+     --rmax DISTANCE       maximum scattering half-path length
+     --S02 FACTOR          amplitude reduction factor
+     --energy-shift ENERGY
+                           energy shift to apply in eV
+     --absorber ELEMENT    atomic symbol of the xray absorber
+     --ignore-elements ELEMENTS
+                           comma delimited list of elements to ignore in the
+                           scattering calculation
+     --edge EDGE           one of K, L1, L2, L3
+     --skip SKIP           number of frames to skip at the beginning
+     --every EVERY         number of frames to between each step
+
+Installing from source
+----------------------
+
+If installing Expectra from source instead of ``pip``, clone the source
+code from `GitHub <https://github.com/SamChill/expectra>`__:
+
+::
+
+   git clone https://github.com/SamChill/expectra.git
+
+After all the dependency requirements have been satisfied, build the
+``feff`` binary, and move it to ``expectra/expectra/``:
+
+::
+
+   cd expectra/feff
+
+   # To use ifort instead of gfortran, set FC=ifort in ./Makefile
+
+   make clean
+   make  # should create the feff binary
+
+   mv ./feff ../expectra
+
+Finally, set relevant environmental variables (assuming Expectra was
+installed at ``$HOME``):
+
+::
+
+   # consider including these in ~/.bash_profile, ~/.profile, or ~/.bashrc
+   export PATH=$HOME/expectra/bin:$PATH
+   export PYTHONPATH=$HOME/expectra:$PYTHONPATH
+
+Note from developers
+--------------------
+
+Expectra was recently migrated from Python2 to Python3. Please report
+any bugs to `sunghjung3@utexas.edu <sunghjung3@utexas.edu>`__.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `expectra-0.1.0/expectra/fft.py` & `expectra-1.0.5/expectra/fft.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,12 +17,12 @@
     ccpath *= xk**kweight
     delta_k = 0.05
     nfft = 2048
     cnorm = delta_k * 1.0/np.sqrt(np.pi) 
     chi_r = np.fft.fft(cnorm*ccpath, n=nfft)
 
     delta_r = np.pi/(nfft*delta_k)                                              
-    r = np.array([ i*delta_r for i in xrange(len(chi_r)) ])
+    r = np.array([ i*delta_r for i in range(len(chi_r)) ])
     ir_min = np.argmin(np.abs(r_min-r))
     ir_max = np.argmin(np.abs(r_max-r))
 
     return r[ir_min:ir_max], chi_r[ir_min:ir_max]
```

### Comparing `expectra-0.1.0/expectra/exafs.py` & `expectra-1.0.5/expectra/exafs.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,26 +87,26 @@
     counter = -1
     interactions = 0
     nl = None
 
     for step, atoms in enumerate(trajectory):
         if COMM_WORLD.rank == 0:
             time_stamp = strftime("%F %T")
-            print '[%s] step %i/%i' % (time_stamp, step+1, len(trajectory))
+            print('[%s] step %i/%i' % (time_stamp, step+1, len(trajectory)))
         atoms = atoms.copy()
         if ignore_elements:
             ignore_indicies = [atom.index for atom in atoms
                                if atom.symbol in ignore_elements]
             del atoms[ignore_indicies]
         if nl is None:
             nl = NeighborList(len(atoms)*[neighbor_cutoff], skin=0.3,
                     self_interaction=False)
         nl.update(atoms)
 
-        for i in xrange(len(atoms)):
+        for i in range(len(atoms)):
             if atoms[i].symbol != absorber:
                 continue
             indicies, offsets = nl.get_neighbors(i)
             for j, offset in zip(indicies, offsets):
                 counter += 1
                 if counter % COMM_WORLD.size != COMM_WORLD.rank:
                     continue
@@ -137,22 +137,22 @@
 
     k = None
     chi_total = None
     counter = -1
     for step, atoms in enumerate(trajectory):
         if COMM_WORLD.rank == 0:
             time_stamp = strftime("%F %T")
-            print '[%s] step %i/%i' % (time_stamp, step+1, len(trajectory))
+            print('[%s] step %i/%i' % (time_stamp, step+1, len(trajectory)))
         atoms = atoms.copy()
         if ignore_elements:
             ignore_indicies = [atom.index for atom in atoms
                                if atom.symbol in ignore_elements]
             del atoms[ignore_indicies]
 
-        for i in xrange(len(atoms)):
+        for i in range(len(atoms)):
             counter += 1
             if counter % COMM_WORLD.size != COMM_WORLD.rank:
                 continue
 
             if atoms[i].symbol != absorber:
                 continue
```

### Comparing `expectra-0.1.0/expectra/feff.py` & `expectra-1.0.5/expectra/feff.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
              "xlam":xlam,
              "rep":rep,
            }
 
 def write_feff(filename, atoms, absorber, feff_options={}):
     f = open(filename, "w")
     f.write("TITLE %s\n" % str(atoms))
-    for key, value in feff_options.iteritems():
+    for key, value in feff_options.items():
         f.write("%s %s\n" % (key, value))
     f.write("\nPOTENTIALS\n")
     absorber_z = atoms[absorber].number
     f.write("%i %i\n" % (0, absorber_z))
 
     unique_z = list(set(atoms.get_atomic_numbers()))
     pot_map = {}
@@ -157,15 +157,15 @@
 
 def absorber_sphere(atoms, absorber, radius):
     box = atoms.get_cell()
     ibox = numpy.linalg.inv(box)
     pos = atoms.get_positions()
     elements = atoms.get_chemical_symbols()
     atoms_sphere = [Atom(elements[absorber], (0.,0.,0.))]
-    for i in xrange(len(atoms)):
+    for i in range(len(atoms)):
         if i == absorber: continue
         r = pbc(pos[i] - pos[absorber], box, ibox)
         d = numpy.linalg.norm(r)
         if d <= radius:
             atoms_sphere.append(Atom(elements[i], r))
     return Atoms(atoms_sphere)
 
@@ -179,26 +179,27 @@
         atoms = absorber_sphere(atoms, absorber, radius=float(feff_options['RMAX'])+0.01)
         absorber = 0
 
     write_feff(feff_inp_path, atoms, absorber, feff_options)
 
     try:
         p = subprocess.Popen(["feff"], cwd=tmp_dir_path,
-                stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                stdout=subprocess.PIPE, stderr=subprocess.PIPE,
+                text=True)
     except OSError:
         from sys import exit, stderr
         stderr.write('unable to locate feff executable in PATH\n')
         exit(1)
     retval = p.wait()
 
     #function to deal with errors
     def feff_error():
-        print 'Problem with feff calculation in %s' % tmp_dir_path
+        print('Problem with feff calculation in %s' % tmp_dir_path)
         tmp_f = tempfile.NamedTemporaryFile(dir='.', prefix='feff.inp.')
-        print 'feff.inp saved to:', tmp_f.name
+        print('feff.inp saved to:', tmp_f.name)
         tmp_f.close()
         write_feff(tmp_f.name, atoms, absorber, feff_options)
         shutil.rmtree(tmp_dir_path)
 
     if retval != 0:
         feff_error()
         return
```

### Comparing `expectra-0.1.0/expectra/io.py` & `expectra-1.0.5/expectra/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -70,50 +70,50 @@
             a.set_positions(positions)
             a.set_masses(masses)
             a.set_constraint(FixAtoms(frozen))
         except:
             if len(trajectory) == 1:
                 return trajectory[0]
             if len(trajectory) == 0:
-                raise IOError, "Could not read con file."
+                raise IOError("Could not read con file.")
             return trajectory
         trajectory.append(a)
 
 
 def write_con(filename, p, w = 'w'):
     con = open(filename, w)
-    print >> con, "Generated by tsase"
-    print >> con
+    print("Generated by tsase", file=con)
+    print(file=con)
     lengths, angles = box_to_length_angle(p.cell)
-    print >> con, " ".join(['%12.6f' % s for s in lengths])
-    print >> con, " ".join(['%12.6f' % s for s in angles])
-    print >> con
-    print >> con
+    print(" ".join(['%12.6f' % s for s in lengths]), file=con)
+    print(" ".join(['%12.6f' % s for s in angles]), file=con)
+    print(file=con)
+    print(file=con)
     atom_count = {}
     name_order = []
     for i in range(len(p)):
         name = p[i].symbol
         if name not in name_order:
             name_order.append(name)
         if name in atom_count:
             atom_count[name] += 1
         else:
             atom_count[name] = 1
-    print >> con, len(name_order)
-    print >> con, " ".join([str(atom_count[i]) for i in name_order])
+    print(len(name_order), file=con)
+    print(" ".join([str(atom_count[i]) for i in name_order]), file=con)
     printmasses = []
     index = 0
     for i in range(len(name_order)):
         printmasses.append(p[index].mass)
         index += atom_count[name_order[i]]
-    print >> con, " ".join(["%12.6f"% i for i in printmasses])
+    print(" ".join(["%12.6f"% i for i in printmasses]), file=con)
     index = 0
     for i in range(len(name_order)):
-        print >> con, name_order[i]
-        print >> con, "Coordinates of Component", i+1
+        print(name_order[i], file=con)
+        print("Coordinates of Component", i+1, file=con)
         for j in range(atom_count[name_order[i]]):
             free = 0
             if len(p.constraints) > 0:
                 if index in p.constraints[0].index:
                     free = 1
             con.write("%12.6f %12.6f %12.6f %d %d\n" % (p[index].position[0],
                       p[index].position[1], p[index].position[2], free, index))
@@ -131,30 +131,30 @@
     while True:
         try:
             data.append(ase.io.read(f, format='vasp'))
         except:
             f.close()
             break
     if len(data) < 1:
-        raise IOError, "Could not read file %s as vasp file." % filename
+        raise IOError("Could not read file %s as vasp file." % filename)
     if len(data) < 2:
         return data[0]
     return data
 
 def read_xdatcar(filename, skip=0, every=1):
     f = open(filename, 'r')
     lines = f.readlines()
     f.close()
     lattice_constant = float(lines[1].strip())
     cell = numpy.array([[float(x) * lattice_constant for x in lines[2].split()],
                         [float(x) * lattice_constant for x in lines[3].split()],
                         [float(x) * lattice_constant for x in lines[4].split()]])
     elements = lines[5].split()
     natoms = [int(x) for x in lines[6].split()]
-    nframes = (len(lines)-7)/(sum(natoms) + 1)
+    nframes = int(round(len(lines)-7)/(sum(natoms) + 1))
     trajectory = []
     for i in range(skip, nframes, every):
         a = Atoms('H'*sum(natoms))
         a.masses = [1.0] * len(a)
         a.set_chemical_symbols(''.join([n*e for (n, e) in zip(natoms, elements)]))
         a.cell = cell.copy()
         a.set_pbc((True, True, True))
@@ -173,15 +173,15 @@
 
     if type(comments) == str:
         f.write('#%s\n' % comments)
     elif type(comments) == list or type(comments) == tuple:
         for comment in comments:
             f.write('#%s\n' % comment)
 
-    for i in xrange(len(r)):
+    for i in range(len(r)):
         f.write('%e %e\n' % (r[i], chir[i]))
 
     f.close()
 
 def read_chi(filename):
     f = open(filename)
     ks = []
```

### Comparing `expectra-0.1.0/bin/expectra` & `expectra-1.0.5/bin/expectra`

 * *Files 2% similar despite different names*

```diff
@@ -60,51 +60,51 @@
 
     if args.multiple_scattering == True:
         args.first_shell = False
 
     trajectory = []
     if COMM_WORLD.rank == 0:
         for filename in args.trajectories:
-            print 'reading', filename
+            print('reading', filename)
             if filename[-3:] == 'con':
                 trajectory_part = read_con(filename)[args.skip::args.every]
             else:
                 trajectory_part = read_xdatcar(filename, args.skip, args.every)
             n = len(trajectory_part)
-            print 'read %4i configurations from %s' % (n, filename)
+            print('read %4i configurations from %s' % (n, filename))
             trajectory += trajectory_part
     trajectory = COMM_WORLD.bcast(trajectory)
 
     args.absorber = get_default_absorber(trajectory[0], args)
 
     k, chi = exafs_trajectory(args, trajectory)
     save_result(k, chi)
 
 def save_result(k, chi):
     if COMM_WORLD.rank != 0: return
-    print 'saving result to chi.dat'
+    print('saving result to chi.dat')
     f = open('chi.dat', 'w')
-    for i in xrange(len(k)):
+    for i in range(len(k)):
         f.write("%6.3f %16.8e\n" % (k[i], chi[i]))
     f.close()
 
 def get_default_absorber(atoms, args):
     symbols = set(atoms.get_chemical_symbols())
     if args.absorber:
         if args.absorber not in symbols:
-            print 'ERROR: --absorber %s is not in the system' % args.absorber
+            print('ERROR: --absorber %s is not in the system' % args.absorber)
             sys.exit(2)
         else:
             return args.absorber
     if args.ignore_elements:
         symbols -= set(args.ignore_elements)
     if len(symbols) == 1:
         return list(symbols)[0]
     else:
-        print 'ERROR: must specify --absorber if more than one chemical specie'
+        print('ERROR: must specify --absorber if more than one chemical specie')
         sys.exit(2)
 
 def exafs_trajectory(args, trajectory):
     if args.multiple_scattering:
         k, chi = exafs_multiple_scattering(args.S02, args.energy_shift, 
                 args.absorber, args.ignore_elements, args.edge, args.rmax, 
                 trajectory)
```

### Comparing `expectra-0.1.0/bin/pdfstats` & `expectra-1.0.5/bin/pdfstats`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             self.min = x
 
         if self.max == None:
             self.max = x
         elif x > self.max:
             self.max = x
 
-        for i in xrange(1,5):
+        for i in range(1,5):
             self.sums[i] += x**float(i)
 
     def mean(self):
         return self.sums[1]/self.N
 
     def sem(self):
         return self.stddev()/(self.N**0.5)
@@ -111,35 +111,35 @@
             r -= 3*(self.sums[2]/self.N)**2
             r += 12*self.sums[2]/self.N*self.mean()**2
             r -= 6*self.mean()**4
 
         return r
 
     def describe_short(self):
-        print 'min: %.3f' % self.min,
-        print 'max: %.3f' % self.max,
-        print 'avg: %.3f' % self.mean(),
-        print 'var: %.5f' % self.var(),
-        print 'c3: %.3e' % self.cumulant(3),
-        print 'c4: %.3e' % self.cumulant(4),
-        print
+        print('min: %.3f' % self.min, end=' ')
+        print('max: %.3f' % self.max, end=' ')
+        print('avg: %.3f' % self.mean(), end=' ')
+        print('var: %.5f' % self.var(), end=' ')
+        print('c3: %.3e' % self.cumulant(3), end=' ')
+        print('c4: %.3e' % self.cumulant(4), end=' ')
+        print()
 
     def describe(self):
-        print 'min:          %f' % self.min
-        print 'max:          %f' % self.max
-        print 'mean:         %f' % self.mean()
-        print 'variance:     %f' % self.var()
-        print '3rd cumulant: %f' % self.cumulant(3)
-        print '4th cumulant: %f' % self.cumulant(4)
+        print('min:          %f' % self.min)
+        print('max:          %f' % self.max)
+        print('mean:         %f' % self.mean())
+        print('variance:     %f' % self.var())
+        print('3rd cumulant: %f' % self.cumulant(3))
+        print('4th cumulant: %f' % self.cumulant(4))
 
 def snapshots_command(args):
     trajectory = []
-    print 'neighbor-cutoff of %.2f Angstrom' % args.neighbor_cutoff
+    print('neighbor-cutoff of %.2f Angstrom' % args.neighbor_cutoff)
     for filename in args.trajectories:
-        print 'reading', filename
+        print('reading', filename)
         if filename[-3:] == 'con':
             trajectory += read_con(filename)[args.skip::args.every]
         elif filename.startswith('POSCAR') or filename.startswith('CONTCAR'):
             trajectory = [ase.io.read(filename, format='vasp')]
         else:
             trajectory += read_xdatcar(filename, args.skip, args.every)
 
@@ -152,25 +152,25 @@
                                if atom.symbol in args.ignore_elements]
             del atoms[ignore_indicies]
         if nl == None:
             nl = NeighborList(len(atoms)*[args.neighbor_cutoff/2.0], skin=0.3, 
                     self_interaction=False, bothways=False)
         nl.update(atoms)
 
-        for j in xrange(len(atoms)):
+        for j in range(len(atoms)):
             indicies, offsets = nl.get_neighbors(j)
             for k, offset in zip(indicies, offsets):
                 r = numpy.linalg.norm(atoms.positions[j] - (atoms.positions[k] + numpy.dot(offset, atoms.get_cell())))
 
                 #r = atoms.get_distance(j,k,True)
                 if r >= args.neighbor_cutoff: continue
                 if r <= args.neighbor_cutoff_min: continue
                 acc.push(r)
 
-        print '%4i/%i: N: %.2f' % (i+1,len(trajectory),2*acc.N/(float(i+1)*len(atoms))),
+        print('%4i/%i: N: %.2f' % (i+1,len(trajectory),2*acc.N/(float(i+1)*len(atoms))), end=' ')
         try:
             acc.describe_short()
         except:
             pass
 
 
     f = open('bonds.dat', 'w')
```

### Comparing `expectra-0.1.0/bin/xafsft` & `expectra-1.0.5/bin/xafsft`

 * *Files identical despite different names*

### Comparing `expectra-0.1.0/bin/harmonic-sampler` & `expectra-1.0.5/bin/harmonic-sampler`

 * *Files 5% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 
     atoms = atoms.copy()
     r0 = atoms.get_positions()
 
     hbar = pq.constants.hbar
     kB = pq.constants.Boltzmann_constant
 
-    for iter in xrange(iters):
+    for iter in range(iters):
         r = r0.copy()
-        for j in xrange(len(ews)):
+        for j in range(len(ews)):
             # Ignore negative and small modes.
             if ews[j] < 1e-2: continue
 
             beta = 1.0/(kB*temperature)
             mass = masses[j]
             # Vibrational frequency.
             omega = numpy.sqrt(ews[j]/mass)
```

### Comparing `expectra-0.1.0/setup.py` & `expectra-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 #!/usr/bin/env python
 from setuptools import setup
 from distutils.command.build import build
-import subprocess
+import subprocess, os, stat, shutil
+
 
 class build_feff(build):
     def run(self):
         subprocess.call('make -C feff', shell=True)
+        # ensure the binary is executable
+        st = os.stat('feff/feff')
+        os.chmod('feff/feff', st.st_mode | stat.S_IEXEC)
+        # move to package dir
+        shutil.move('feff/feff', 'expectra/feff')
 
 class build_custom(build):
     def run(self):
         self.run_command('build_feff')
         build.run(self)
 
 try:
    import pypandoc
-   long_description = pypandoc.convert('README.md', 'rst')
+   long_description = pypandoc.convert_file('README.md', 'rst')
 except (IOError, ImportError):
    long_description = ''
 
 description = 'Code for simulating EXAFS calculations from molecular ' \
               'dynamics trajectories or normal modes using FEFF'
 
 setup(
     name='expectra',
-    version='0.1.0',
+    version='1.0.5',
     author='Samuel T. Chill',
     author_email='samchill@gmail.com',
     url='https://github.com/SamChill/expectra',
     packages=['expectra'],
     scripts=[
         'bin/expectra',
         'bin/xafsft',
         'bin/harmonic-sampler',
         'bin/pdfstats',
-        'feff/feff',
+        'bin/feff',
     ],
+    package_data={
+        'expectra': ['feff'],
+    },
     license='LICENSE.txt',
     description=description,
     long_description=long_description,
     install_requires=[
         'numpy >= 1.5.0',
         'mpi4py >= 1.3',
         'ase >= 3.11.0',
```

### Comparing `expectra-0.1.0/feff/feff6l.f` & `expectra-1.0.5/feff/feff6l.f`

 * *Files identical despite different names*

### Comparing `expectra-0.1.0/LICENSE.txt` & `expectra-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `expectra-0.1.0/README.md` & `expectra-1.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 ## Requirements
 
 * gfortran
 * MPI (e.g. OpenMPI or MPICH)
 * Python
   * numpy
   * mpi4py
+  * [ASE](https://wiki.fysik.dtu.dk/ase/)
 
 ## Installation
 
 This program is distributed as a Python package. It requires a Fortran
 compiler (e.g. gfortran) to build the FEFF6-lite program that is redistributed with the code. A MPI library (e.g. OpenMPI) is also required.
 
 The first step is to install Python, GFortran, and MPICH. On Ubuntu this can be accomplished like so:
@@ -71,7 +72,43 @@
   --ignore-elements ELEMENTS
                         comma delimited list of elements to ignore in the
                         scattering calculation
   --edge EDGE           one of K, L1, L2, L3
   --skip SKIP           number of frames to skip at the beginning
   --every EVERY         number of frames to between each step
 ```
+
+## Installing from source
+
+If installing Expectra from source instead of `pip`, clone the source code
+from [GitHub](https://github.com/SamChill/expectra):
+
+```
+git clone https://github.com/SamChill/expectra.git
+```
+
+After all the dependency requirements have been satisfied, build the `feff` binary,
+and move it to `expectra/expectra/`:
+
+```
+cd expectra/feff
+
+# To use ifort instead of gfortran, set FC=ifort in ./Makefile
+
+make clean
+make  # should create the feff binary
+
+mv ./feff ../expectra
+```
+
+Finally, set relevant environmental variables (assuming Expectra was installed at `$HOME`):
+
+```
+# consider including these in ~/.bash_profile, ~/.profile, or ~/.bashrc
+export PATH=$HOME/expectra/bin:$PATH
+export PYTHONPATH=$HOME/expectra:$PYTHONPATH
+```
+
+## Note from developers
+
+Expectra was recently migrated from Python2 to Python3.
+Please report any bugs to [sunghjung3@utexas.edu](sunghjung3@utexas.edu).
```

### Comparing `expectra-0.1.0/expectra.egg-info/PKG-INFO` & `expectra-1.0.5/expectra.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,93 +1,134 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: expectra
-Version: 0.1.0
+Version: 1.0.5
 Summary: Code for simulating EXAFS calculations from molecular dynamics trajectories or normal modes using FEFF
 Home-page: https://github.com/SamChill/expectra
 Author: Samuel T. Chill
 Author-email: samchill@gmail.com
 License: LICENSE.txt
-Description: Expectra
-        ========
-        
-        Introduction
-        ------------
-        
-        Expectra is program to simulate EXAFS from the outputs of molecular
-        dynamics simulations. It also has the ability to to sample structures
-        based on a harmonic potential generated from a normal modes calculation.
-        
-        The EXAFS multiple scattering calculations are performed using
-        `FEFF6-lite <http://www.feffproject.org/>`__, which was written at the
-        University of Washington by J.J. Rehr and co-workers.1
-        
-        1. J.J. Rehr, S.I. Zabinsky and R.C. Albers, "High-order multiple
-           scattering calculations of x-ray-absorption fine structure", *Phys.
-           Rev. Lett.* **69**, 3397 (1992).
-        
-        Requirements
-        ------------
-        
-        -  gfortran
-        -  MPI (e.g. OpenMPI or MPICH)
-        -  Python
-        -  numpy
-        -  mpi4py
-        
-        Installation
-        ------------
-        
-        This program is distributed as a Python package. It requires a Fortran
-        compiler (e.g. gfortran) to build the FEFF6-lite program that is
-        redistributed with the code. A MPI library (e.g. OpenMPI) is also
-        required.
-        
-        The first step is to install Python, GFortran, and MPICH. On Ubuntu this
-        can be accomplished like so:
-        
-        ::
-        
-            $ sudo apt-get install build-essential gfortran mpich python python-pip
-        
-        Once the dependencies are installed expectra (and the Python packages it
-        depends on) can be installed using pip:
-        
-        ::
-        
-            $ pip install --user expectra
-        
-        Usage
-        -----
-        
-        ::
-        
-            usage: expectra [-h] [--first-shell] [--neighbor-cutoff DISTANCE]
-                            [--multiple-scattering] [--rmax DISTANCE] [--S02 FACTOR]
-                            [--energy-shift ENERGY] [--absorber ELEMENT]
-                            [--ignore-elements ELEMENTS] [--edge EDGE] [--skip SKIP]
-                            [--every EVERY]
-                            TRAJ [TRAJ ...]
-        
-            positional arguments:
-              TRAJ                  trajectory file (POSCAR, con, xyz)
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              --first-shell         a single scattering calculation that uses an
-                                    automatically calculated reference path (default:
-                                    True)
-              --neighbor-cutoff DISTANCE
-                                    1st neighbor cutoff distance (default: 3.4)
-              --multiple-scattering
-              --rmax DISTANCE       maximum scattering half-path length
-              --S02 FACTOR          amplitude reduction factor
-              --energy-shift ENERGY
-                                    energy shift to apply in eV
-              --absorber ELEMENT    atomic symbol of the xray absorber
-              --ignore-elements ELEMENTS
-                                    comma delimited list of elements to ignore in the
-                                    scattering calculation
-              --edge EDGE           one of K, L1, L2, L3
-              --skip SKIP           number of frames to skip at the beginning
-              --every EVERY         number of frames to between each step
-        
-Platform: UNKNOWN
+License-File: LICENSE.txt
+
+Expectra
+========
+
+Introduction
+------------
+
+Expectra is program to simulate EXAFS from the outputs of molecular
+dynamics simulations. It also has the ability to to sample structures
+based on a harmonic potential generated from a normal modes calculation.
+
+The EXAFS multiple scattering calculations are performed using
+`FEFF6-lite <http://www.feffproject.org/>`__, which was written at the
+University of Washington by J.J. Rehr and co-workers.1
+
+1. J.J. Rehr, S.I. Zabinsky and R.C. Albers, “High-order multiple
+   scattering calculations of x-ray-absorption fine structure”, *Phys.
+   Rev. Lett.* **69**, 3397 (1992).
+
+Requirements
+------------
+
+-  gfortran
+-  MPI (e.g. OpenMPI or MPICH)
+-  Python
+
+   -  numpy
+   -  mpi4py
+   -  `ASE <https://wiki.fysik.dtu.dk/ase/>`__
+
+Installation
+------------
+
+This program is distributed as a Python package. It requires a Fortran
+compiler (e.g. gfortran) to build the FEFF6-lite program that is
+redistributed with the code. A MPI library (e.g. OpenMPI) is also
+required.
+
+The first step is to install Python, GFortran, and MPICH. On Ubuntu this
+can be accomplished like so:
+
+::
+
+   $ sudo apt-get install build-essential gfortran mpich python python-pip
+
+Once the dependencies are installed expectra (and the Python packages it
+depends on) can be installed using pip:
+
+::
+
+   $ pip install --user expectra
+
+Usage
+-----
+
+::
+
+   usage: expectra [-h] [--first-shell] [--neighbor-cutoff DISTANCE]
+                   [--multiple-scattering] [--rmax DISTANCE] [--S02 FACTOR]
+                   [--energy-shift ENERGY] [--absorber ELEMENT]
+                   [--ignore-elements ELEMENTS] [--edge EDGE] [--skip SKIP]
+                   [--every EVERY]
+                   TRAJ [TRAJ ...]
+
+   positional arguments:
+     TRAJ                  trajectory file (POSCAR, con, xyz)
+
+   optional arguments:
+     -h, --help            show this help message and exit
+     --first-shell         a single scattering calculation that uses an
+                           automatically calculated reference path (default:
+                           True)
+     --neighbor-cutoff DISTANCE
+                           1st neighbor cutoff distance (default: 3.4)
+     --multiple-scattering
+     --rmax DISTANCE       maximum scattering half-path length
+     --S02 FACTOR          amplitude reduction factor
+     --energy-shift ENERGY
+                           energy shift to apply in eV
+     --absorber ELEMENT    atomic symbol of the xray absorber
+     --ignore-elements ELEMENTS
+                           comma delimited list of elements to ignore in the
+                           scattering calculation
+     --edge EDGE           one of K, L1, L2, L3
+     --skip SKIP           number of frames to skip at the beginning
+     --every EVERY         number of frames to between each step
+
+Installing from source
+----------------------
+
+If installing Expectra from source instead of ``pip``, clone the source
+code from `GitHub <https://github.com/SamChill/expectra>`__:
+
+::
+
+   git clone https://github.com/SamChill/expectra.git
+
+After all the dependency requirements have been satisfied, build the
+``feff`` binary, and move it to ``expectra/expectra/``:
+
+::
+
+   cd expectra/feff
+
+   # To use ifort instead of gfortran, set FC=ifort in ./Makefile
+
+   make clean
+   make  # should create the feff binary
+
+   mv ./feff ../expectra
+
+Finally, set relevant environmental variables (assuming Expectra was
+installed at ``$HOME``):
+
+::
+
+   # consider including these in ~/.bash_profile, ~/.profile, or ~/.bashrc
+   export PATH=$HOME/expectra/bin:$PATH
+   export PYTHONPATH=$HOME/expectra:$PYTHONPATH
+
+Note from developers
+--------------------
+
+Expectra was recently migrated from Python2 to Python3. Please report
+any bugs to `sunghjung3@utexas.edu <sunghjung3@utexas.edu>`__.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

