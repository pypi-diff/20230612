# Comparing `tmp/vasp_suite-1.2.1.tar.gz` & `tmp/vasp_suite-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.2.1.tar", last modified: Mon Jun  5 12:40:59 2023, max compression
+gzip compressed data, was "vasp_suite-1.2.2.tar", last modified: Mon Jun 12 18:13:35 2023, max compression
```

## Comparing `vasp_suite-1.2.1.tar` & `vasp_suite-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:40:59.956035 vasp_suite-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-05 12:40:59.956035 vasp_suite-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 12:40:59.956035 vasp_suite-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-06-05 12:40:57.000000 vasp_suite-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:40:59.955035 vasp_suite-1.2.1/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-05 12:40:57.000000 vasp_suite-1.2.1/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    16162 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4855 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/vasp_suite/core.py
--rwxrwxrwx   0 root         (0) root         (0)    17643 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     2936 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)    20176 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-05 12:40:46.000000 vasp_suite-1.2.1/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:40:59.956035 vasp_suite-1.2.1/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-05 12:40:59.000000 vasp_suite-1.2.1/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-05 12:40:59.000000 vasp_suite-1.2.1/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 12:40:59.000000 vasp_suite-1.2.1/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-05 12:40:59.000000 vasp_suite-1.2.1/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-05 12:40:59.000000 vasp_suite-1.2.1/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-05 12:40:59.000000 vasp_suite-1.2.1/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:13:35.490662 vasp_suite-1.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 18:13:35.490662 vasp_suite-1.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 18:13:35.490662 vasp_suite-1.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-06-12 18:13:33.000000 vasp_suite-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:13:35.489746 vasp_suite-1.2.2/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-12 18:13:33.000000 vasp_suite-1.2.2/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16153 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/vasp_suite/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    19084 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     3714 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)    20919 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-12 18:13:08.000000 vasp_suite-1.2.2/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:13:35.490662 vasp_suite-1.2.2/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 18:13:35.000000 vasp_suite-1.2.2/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-12 18:13:35.000000 vasp_suite-1.2.2/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 18:13:35.000000 vasp_suite-1.2.2/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-12 18:13:35.000000 vasp_suite-1.2.2/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-12 18:13:35.000000 vasp_suite-1.2.2/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 18:13:35.000000 vasp_suite-1.2.2/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.2.1/LICENSE` & `vasp_suite-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.1/PKG-INFO` & `vasp_suite-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.2.1
+Version: 1.2.2
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.2.1/README.md` & `vasp_suite-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.1/setup.py` & `vasp_suite-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.2.1/vasp_suite/cli.py` & `vasp_suite-1.2.2/vasp_suite/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,29 +277,29 @@
                     vasp_suite calculate_kpoints ...
                     vasp_suite generate_kpoints ...
                     vasp_suite generate_supercell ...
                     vasp_suite convert_cif ...
                     vasp_suite start_up ...
                     vasp_suite dope_structure ...
                     vasp_suite generate_defect ...
-                    vasp_suite asymmetric_unit ...
+                    vasp_suite molecular_qm ...
                     vasp_suite ewald ...
                     vasp_suite plot_potential ...
                     vasp_suite qm_region ...
                 '''
                 ),
             epilog=dedent(
                 '''
                 To display options for a specific programme, use vasp_suite <programme> -h
                 '''
                 ),
             formatter_class=argparse.RawDescriptionHelpFormatter
             )
 
-    # Subparsers 
+    # Subparsers
     subparsers = parser.add_subparsers(dest='prog')
 
     gen_inp = subparsers.add_parser(
             'generate_input',
             help='Generate input files for VASP calculations',
             description=dedent(
                 '''
@@ -421,15 +421,15 @@
             '''
             The expansion vector for the supercell, a b c
             '''
             ),
         )
 
     start_up = subparsers.add_parser(
-        'start_up',
+        'set_up',
         help='Generate the configuration files for the suite',
         formatter_class=argparse.RawDescriptionHelpFormatter
         )
 
     start_up.set_defaults(func=start_up_func)
 
     dope_struct = subparsers.add_parser(
@@ -486,15 +486,15 @@
             '--instances',
             help='The number of instances of defect',
             type=int,
             default=1,
             )
 
     asym = subparsers.add_parser(
-        'asymmetric_unit',
+        'molecular_qm',
         help='Generate the asymmetric unit of a structure',
         formatter_class=argparse.RawDescriptionHelpFormatter
         )
 
     asym.set_defaults(func=asymmetric_unit_func)
 
     asym.add_argument(
```

### Comparing `vasp_suite-1.2.1/vasp_suite/core.py` & `vasp_suite-1.2.2/vasp_suite/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Imports 
 import numpy as np 
 import os
 from . import structure 
 from . import input 
 from . import submission
 from . import ewald
-
+import socket
 # Functions 
 
 def generate_input(filename: str, calculation: str) -> None:
     '''
     Generates Input files for VASP Calculations.
     '''
     input_files = input.InputFileGenerator(filename, calculation)
@@ -36,14 +36,15 @@
 def generate_supercell(expansion: np.ndarray) -> None: 
     '''
     Generates a supercell from a given expansion matrix.
     '''
     _s = structure.Structure('POSCAR')
     _s.Vasp_reader()
     _s.Supercell(expansion)
+    _s.supercell_reorder()
     _s.write_poscar()
     return None
 
 def dope_structure(filename: str, dopant: str, replace: str, instances: int) -> None:
     '''
     Dopes a structure with a given dopant and generates all possible structures.
     '''
@@ -123,15 +124,27 @@
         r_cut: float,
         bound: float,
         verbose: int,
         ) -> None:
     '''
     Generates a xfield input file for molcas calulations using the Ewald summation.
     '''
-    _e = ewald.Ewald(qm_region, filename, charges, atom, n, r_cut, expansion, bound, verbose)
+    if 'csf' in socket.gethostname() and 'login' in socket.gethostname():
+        raise Warning('DO NOT run ewald on the CSF login node!!!')
+    _e = ewald.Ewald(
+            qm_region,
+            filename,
+            charges,
+            atom,
+            n,
+            r_cut,
+            expansion,
+            bound,
+            verbose
+            )
     _e.Calculate_Ewald()
     _e.Create_Zones()
     _e.Fitting()
 
 def potential_plot(
         filename: str,
         xy_grid: int,
```

### Comparing `vasp_suite-1.2.1/vasp_suite/ewald.py` & `vasp_suite-1.2.2/vasp_suite/ewald.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,21 +66,37 @@
         self.read_charges()
         self._s.bv = self._s.bv / (2 * np.pi)
         self.alpha = 0.2
         self.evconv = 1e10 * constants.e / (4 * np.pi * constants.epsilon_0)
         self.bound = bound
         self.verbose = verbose
 
+        # initial checks 
+        a1, a2, a3 = self._s.av
+        n1, n2, n3 = self._exp
+        a1, a2, a3 = a1 * n1, a2 * n2, a3 * n3
+        a_v = np.array([a1, a2, a3])
+        min = np.linalg.norm(np.min(a_v, axis=0))
+        if self._r_cut > min:
+            raise ValueError("Cutoff radius is larger than the smallest lattice vector")
+
+        # check unit cell charge
+        if np.sum(self._q) != 0:
+            raise ValueError("Unit cell is not charge neutral")
+
     def read_charges(self) -> None:
         '''
         Reads the charges from the file
         '''
         with open(self._charges, 'r') as f:
             _q = f.readlines()
         self._q = [float(i) for i in _q]
+        if len(self._q) != self._s._N:
+            raise ValueError(
+                    "Number of charges does not match number of atoms")
 
     def _uc_print(self) -> None:
         '''
         Creates a print out for the unit cell information
         '''
         print('''
 --------------------------------
@@ -100,21 +116,25 @@
         for i in range(len(self._s.bv)):
             print(f"{self._s.bv[i, 0]:.8f} {self._s.bv[i, 1]:.8f} {self._s.bv[i, 2]:.8f}")
 
     def _compute_n(self) -> None:
         _n1 = list(range(-self._n[0], self._n[0]+1))
         _n2 = list(range(-self._n[1], self._n[1]+1))
         _n3 = list(range(-self._n[2], self._n[2]+1))
-        self._n = np.array([[_n1[i], _n2[j], _n3[k]] for i in range(len(_n1)) for j in range(len(_n2)) for k in range(len(_n3))], dtype=int)
+        self._n = np.array([[_n1[i], _n2[j], _n3[k]]
+                            for i in range(len(_n1))
+                            for j in range(len(_n2))
+                            for k in range(len(_n3))], dtype=int)
 
     def _images(self):
         coords = self._s.coords
         _n = self._n
         _av = self._s.av
-        images = np.array([coord + _n[i] for i in range(len(_n)) for coord in coords], dtype=float)
+        images = np.array([coord + _n[i] for i in range(len(_n))
+                           for coord in coords], dtype=float)
         images = images @ _av
         self.images: np.ndarray = images
         self._num_images = len(images)
 
     def _ewald_recip(self) -> None:
         '''
         Calculates the reciprocal space contribution to the Ewald sum
@@ -227,34 +247,41 @@
 
         _dest = _dest.sum(axis=0)
         _vector = coords[location] - _dest
         coords = coords - _vector
         coords %= 1.0
         self._s.coords = coords
 
-    def _supercell(self):
+    def _build_supercell(self):
         '''
         Generates the _supercell
         '''
         _exp = self._exp
         _av = self._s.av
         coords = self._s.coords
         e_total = self.e_total
         atom_list = self._s._atom_list
 
         _n1 = list(range(_exp[0]))
         _n2 = list(range(_exp[1]))
         _n3 = list(range(_exp[2]))
-        _n = np.array([[_n1[i], _n2[j], _n3[k]] for i in range(len(_n1)) for j in range(len(_n2)) for k in range(len(_n3))], dtype=int)
-        coords = np.array([coord + _n[i] for i in range(len(_n)) for coord in coords], dtype=float) 
+
+        _n = np.array([[_n1[i], _n2[j], _n3[k]]
+                       for i in range(len(_n1))
+                       for j in range(len(_n2))
+                       for k in range(len(_n3))], dtype=int)
+
+        coords = np.array([coord + _n[i]
+                           for i in range(len(_n))
+                           for coord in coords], dtype=float)
 
         for i in range(len(coords)):
-            coords[i, 0] = coords[i, 0]/ _exp[0] - 0.5
-            coords[i, 1] = coords[i, 1]/ _exp[1] - 0.5
-            coords[i, 2] = coords[i, 2]/ _exp[2] - 0.5
+            coords[i, 0] = coords[i, 0] / _exp[0] - 0.5
+            coords[i, 1] = coords[i, 1] / _exp[1] - 0.5
+            coords[i, 2] = coords[i, 2] / _exp[2] - 0.5
 
         _av[0], _av[1], _av[2] = _av[0] * _exp[0], _av[1] * _exp[1], _av[2] * _exp[2]
         coords = coords @ _av
 
         e_total = [e_total] * (_exp[0] * _exp[1] * _exp[2])
         e_total = np.array(e_total, dtype=float).flatten()
 
@@ -279,17 +306,24 @@
 
         with open(file, 'r') as f:
             _qm = f.readlines()
         _qm = [line.strip().split() for line in _qm]
         _qm = np.array(_qm[2:])
         _qm = np.array(_qm[:, 1:], dtype=float)
 
-        _supercell = np.concatenate((coords, b[:,None], q[:,None], atom_list[:,None]), axis=1)
-        _sphere = np.array([coord for coord in _supercell if np.linalg.norm(coord[:3]) < rcut])
-        _param = np.array([coord for coord in _supercell if np.linalg.norm(coord[:3]) > rcut])
+        _supercell = np.concatenate((coords,
+                                     b[:, None],
+                                     q[:, None],
+                                     atom_list[:, None]), axis=1)
+
+        _sphere = np.array([coord for coord in _supercell
+                            if np.linalg.norm(coord[:3]) < rcut])
+
+        _param = np.array([coord for coord in _supercell
+                           if np.linalg.norm(coord[:3]) > rcut])
 
         self._sphere = _sphere
         self._param = _param
         self._qm = _qm
         self._supercell = _supercell
 
     def _drive_dipole(self) -> float:
@@ -298,16 +332,22 @@
         '''
         _sphere = self._sphere
         _param = self._param
 
         ind1, ind2, ind3 = np.random.choice(len(_param), 3, replace=True)
 
         r = np.array([_param[ind1], _param[ind2], _param[ind3]])
-        _r = np.array([_param[ind1, :3], _param[ind2, :3], _param[ind3, :3]], dtype=float)
-        q = np.array([_param[ind1, 4], _param[ind2, 4], _param[ind3, 4]], dtype=float)
+
+        _r = np.array([_param[ind1, :3],
+                       _param[ind2, :3],
+                       _param[ind3, :3]], dtype=float)
+
+        q = np.array([_param[ind1, 4],
+                      _param[ind2, 4],
+                      _param[ind3, 4]], dtype=float)
 
         # delete the three reandom charges
         np.delete(_param, [ind1, ind2, ind3], axis=0)
 
         # calculate the dipole moment
         dipole_sphere = np.array(_sphere[:, 4], dtype=float) @ np.array(_sphere[:, :3], dtype=float)
         dipole_param = np.array(_param[:, 4], dtype=float) @ np.array(_param[:, :3], dtype=float)
@@ -342,15 +382,15 @@
 
         # calculate the change in charge for each of the three charges so the total dipole moment is zero 
     def Create_Zones(self) -> None:
         '''
         Creates the zones for the Ewald sum
         '''
         self._vector()
-        self._supercell()
+        self._build_supercell()
         self._create_zones()
         print('''
 --------------------------------
 
      Driving Dipole Moment
            To Zero
 
@@ -393,46 +433,56 @@
 
         Q, R = np.linalg.qr(c.T, mode='complete')
 
         AQ = A @ Q
 
         b2 = bi - AQ[:, 0] * (1/R[0]).T * d
 
-        x2 = sp.optimize.lsq_linear(AQ[:, 1:], b2, bounds=(-15, 15), method='bvls', tol=1e-8, max_iter=10000, verbose=verbose)
+        x2 = sp.optimize.lsq_linear(AQ[:, 1:],
+                                    b2,
+                                    bounds=(-15, 15),
+                                    method='bvls',
+                                    tol=1e-8,
+                                    max_iter=10000,
+                                    verbose=verbose)
         x2 = x2.x
 
         x1 = (1/R[0]).T * d
         x = np.concatenate((x1, x2), axis=0)
         x = Q @ x
 
         x = x / self.evconv
         x = np.array(_param[:, 4], dtype=float) + x
 
         # calcualte rmsd
         q_total = np.concatenate((_sphere[:, 4], x), axis=0)
         coords = np.concatenate((_sphere_coords, _param_coords), axis=0)
-        rij = sp.spatial.distance.squareform(1/sp.spatial.distance.pdist(coords, 'euclidean'))
+        rij = sp.spatial.distance.squareform(
+                1/sp.spatial.distance.pdist(coords, 'euclidean'))
         rij[np.where(rij == np.inf)] = 0
 
         potential = self.evconv * np.array(q_total, dtype=float) @ rij
         ewald = np.array(_sphere[:, 3], dtype=float)
-        rmsd = np.sqrt(np.sum((potential[:len(_sphere)] - ewald)**2) / len(ewald))
+        rmsd = np.sqrt(np.sum(
+            (potential[:len(_sphere)] - ewald)**2) / len(ewald))
 
         self.rmsd = rmsd
         self.q_total = q_total
         self.coords = coords
         self._x = x
 
     def _outputs(self) -> None:
-        coords = np.array(np.hstack((self.coords, self.q_total[:, None])), dtype=str)
+        coords = np.array(np.hstack((self.coords,
+                                     self.q_total[:, None])), dtype=str)
         # remove _qm region
         _qm = np.array(self._qm[:, :3], dtype=float)
         for i in range(len(_qm)):
             for j in range(len(coords)-1):
-                if np.allclose(_qm[i, :3], np.array(coords[j, :3], dtype=float)):
+                if np.allclose(_qm[i, :3],
+                               np.array(coords[j, :3], dtype=float)):
                     coords = np.delete(coords, j, axis=0)
 
         with open('ewald.out', 'w') as f:
             for i in range(len(coords)):
                 f.write(f'{coords[i,0]} {coords[i,1]} {coords[i,2]} {coords[i,3]}\n')
 
     def Fitting(self) -> None:
@@ -509,8 +559,7 @@
         ax.contourf(self.X, self.Y, self.Z, self.n_contours, cmap='viridis')
         ax.set_xlabel('x/ Å')
         ax.set_ylabel('y/ Å')
         # show colorbar
         cbar = fig.colorbar(ax.contourf(self.X, self.Y, self.Z, self.n_contours, cmap='viridis'))
         cbar.set_label('Potential')
         plt.show()
-
```

### Comparing `vasp_suite-1.2.1/vasp_suite/input.py` & `vasp_suite-1.2.2/vasp_suite/input.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,31 +8,46 @@
 from .structure import Structure
 
 
 class InputFileGenerator():
     '''
     InputFileGenerator is a class which generates input files for VASP calculations.
     '''
+
     def __init__(self, filename: str, calculation: str):
         '''
         Initializes the class.
         '''
         self._s = Structure(filename)
         self._s.Vasp_reader()
         self.configuration = calculation
         hostname = socket.gethostname()
         if 'csf3' in hostname: 
             self.pseudopotentials = '/opt/apps/apps/intel-19.1/vasp/5.4.4/pseudopotentials/potpaw_PBE.54'
             self.module = 'apps/intel-19.1/vasp/5.4.4'
         elif 'csf4' in hostname: 
             self.pseudopotentials = '/opt/software/RI/apps/VASP/5.4.4-iomkl-2020.02/pseudopotentials/potpaw_PBE.54'
             self.module = 'VASP/5.4.4-iomkl-2020.02'
-        #else:
-        #    raise Warning('Unknown hostname. Generation of POTCAR file not possible.')
-
+        elif os.path.exists(
+                os.path.join(
+                    os.path.expanduser('~'),
+                    '.vasp_suite_configs/host.ini')):
+            config = cp.ConfigParser()
+            config.read(os.path.join(os.path.expanduser('~'), '.vasp_suite_configs/host.ini'))
+            try:
+                self.pseudopotentials = config['host']['pseudopotentials']
+                self.module = config['host']['module']
+            except KeyError:
+                print('''Create a host.ini file in ~/.vasp_suite_configs with the following format:
+                [host]
+                pseudopotentials = /path/to/pseudopotentials
+                module = module_name''')
+                raise KeyError(f'''No configuration found for {hostname}.''')
+        else:
+            raise Warning('Unable to generate POTCAR file. No configuration found for this host.')
 
     def _INCAR(self):
         config = cp.ConfigParser()
         input_file = os.path.join(os.path.expanduser('~'), '.vasp_suite_configs', f'''{self.configuration}.ini''')
         config.read(input_file)
         with open('INCAR', 'w') as f:
             for section in config.sections():
@@ -56,10 +71,7 @@
             os.chdir(pseudo)
             for file in files:
                 os.chdir(str(file))
                 with open('POTCAR', 'r') as g:
                     f.write(g.read()) 
                 os.chdir(pseudo)
             os.chdir(cwd)
-
-
-
```

### Comparing `vasp_suite-1.2.1/vasp_suite/structure.py` & `vasp_suite-1.2.2/vasp_suite/structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,277 +1,308 @@
 '''
 A module for the Structure class. Structure will perform operations structure data files.
 '''
  # Imports 
 import re
 import os
-import numpy as np 
-import scipy as sp 
-from functools import wraps 
+import numpy as np
+import scipy as sp
+from functools import wraps
 from time import perf_counter
 from ase import io
 
+
 def timer(func):
     '''
     A decorator function to time functions.
     '''
     @wraps(func)
     def wrapper(*args, **kwargs):
         start = perf_counter()
         print(f'Running {func.__name__}...')
         func(*args, *kwargs)
         end = perf_counter()
-        print(f"Time elapsed: {end - start}") 
+        print(f"Time elapsed: {end - start}")
     return wrapper
 
-class Structure(): 
+
+class Structure():
     '''
-    A class of functions for manipulating structure data files. 
+    A class of functions for manipulating structure data files.
     '''
+
     def __init__(self, filename: str):
         '''
         Initializes the Structure class.
         '''
         self.filename = filename
 
     def Vasp_reader(self):
-       '''
-       Reads and formats a .vasp, POSCAR or CONTCAR file. 
-       '''
-       # Obtain the data 
-       with open(self.filename) as f:
-           data = f.readlines()
-       data = [x.strip().split() for x in data]
-
-       self.name: str  = data[0][0]
-       self.scale: float = data[1][0]
-       self.av: np.ndarray = np.array(data[2:5], dtype=float)
-       self.atoms: list = data[5] 
-       self.natoms: list = [int(x) for x in data[6]]
-       self._N: int = sum(self.natoms)
-       self._type: str = data[7][0].lower()
-       self.coords: np.ndarray = np.array(data[8:8+self._N], dtype=float)
-
-       # Calculate reciprocal lattice vectors 
-       a1, a2, a3 = self.av 
-       b1 = 2 * np.pi * np.cross(a2, a3) / (a1@np.cross(a2, a3))
-       b2 = 2 * np.pi * np.cross(a3, a1) / (a2@np.cross(a3, a1))
-       b3 = 2 * np.pi * np.cross(a1, a2) / (a3@np.cross(a1, a2))
-       self.bv: np.ndarray = np.array([b1, b2, b3])
-
-       # Generate atom list 
-       atom_list = [f'{symbol} '*num for symbol, num in zip(self.atoms, self.natoms)]
-       atom_list = ' '.join(atom_list).split()
-       self._atom_list = atom_list
+        '''
+        Reads and formats a .vasp, POSCAR or CONTCAR file.
+        '''
+        with open(self.filename) as f:
+            data = f.readlines()
+        data = [x.strip().split() for x in data]
+
+        self.name: str = data[0][0]
+        self.scale: float = float(data[1][0])
+        self.av: np.ndarray = np.array(data[2:5], dtype=float)
+        self.atoms: list = data[5]
+        self.natoms: list = [int(x) for x in data[6]]
+        self._N: int = sum(self.natoms)
+        self._type: str = data[7][0].lower()
+        self.coords: np.ndarray = np.array(data[8:8+self._N], dtype=float)
+
+        # Calculate reciprocal lattice vectors
+        a1, a2, a3 = self.av
+        b1 = 2 * np.pi * np.cross(a2, a3) / (a1@np.cross(a2, a3))
+        b2 = 2 * np.pi * np.cross(a3, a1) / (a2@np.cross(a3, a1))
+        b3 = 2 * np.pi * np.cross(a1, a2) / (a3@np.cross(a1, a2))
+        self.bv: np.ndarray = np.array([b1, b2, b3])
 
-       # calculate the volume of the unit cell 
-       self.V = np.dot(a1, np.cross(a2, a3)) 
+        # Generate atom list
+        atom_list = [f'{symbol} '*num
+                     for symbol, num in zip(self.atoms, self.natoms)]
+
+        atom_list = ' '.join(atom_list).split()
+        self._atom_list = atom_list
+
+        # calculate the volume of the unit cell
+        self.V = np.dot(a1, np.cross(a2, a3))
 
     def CIF_reader(self) -> None:
         '''
         Reads a .cif file and initializes it into the structure class.
         '''
         data = io.read(self.filename) 
         self.name = data.get_chemical_formula()
         self.scale = 1
         self.av = data.cell.array
-        self._atom_list = data.get_chemical_symbols() 
+        self._atom_list = data.get_chemical_symbols()
         self._N = len(self._atom_list)
         self._type = 'direct'
         self.coords = data.get_scaled_positions()
 
-        # convert atom list into atoms and natoms 
-        atom_list = self._atom_list 
-        atoms = list(set(atom_list)) 
-        natoms = [atom_list.count(x) for x in atoms] 
-        self.atoms = atoms 
-        self.natoms = natoms 
+        # convert atom list into atoms and natoms
+        atom_list = self._atom_list
+        atoms = list(set(atom_list))
+        natoms = [atom_list.count(x) for x in atoms]
+        self.atoms = atoms
+        self.natoms = natoms
 
-        # Calculate reciprocal lattice vectors 
+        # Calculate reciprocal lattice vectors
         a1, a2, a3 = self.av 
         b1 = 2 * np.pi * np.cross(a2, a3) / (a1@np.cross(a2,a3))
         b2 = 2 * np.pi * np.cross(a3, a1) / (a2@np.cross(a3,a1))
-        b3 = 2 * np.pi * np.cross(a1, a2) / (a3@np.cross(a1,a2)) 
+        b3 = 2 * np.pi * np.cross(a1, a2) / (a3@np.cross(a1,a2))
         self.bv: np.ndarray = np.array([b1, b2, b3])
 
-        # calculate the volume of the unit cell 
+        # calculate the volume of the unit cell
         self.V = np.dot(a1, np.cross(a2, a3))
 
     @property
     def get_name(self):
         '''
         Getter for name
         '''
         print(f'Name: {self.name}')
         return self.name
 
-    @get_name.setter 
+    @get_name.setter
     def rename(self, new_name: str):
         '''
         Setter for name
         '''
         print(f'Name changed from "{self.name}" to "{new_name}"')
         self.name = new_name
 
-    @get_name.deleter 
-    def delete_name(self): 
+    @get_name.deleter
+    def delete_name(self):
         '''
-        Deleter for name 
+        Deleter for name
         '''
-        print(f'Name "{self.name}" deleted') 
+        print(f'Name "{self.name}" deleted')
         del self.name
 
     def Cart_coords(self) -> np.ndarray:
         '''
-        Converts fractional coordinates to cartesian coordinates. 
+        Converts fractional coordinates to cartesian coordinates.
         '''
         self._type = 'cartesian'
-        self.cart_coords =  self.coords @ self.av
+        self.cart_coords = self.coords @ self.av
 
-    def Supercell(self, n: list) -> None: 
+    def Supercell(self, n: list) -> None:
         '''
-        Creates a supercell of size n1 x n2 x n3. 
+        Creates a supercell of size n1 x n2 x n3.
         '''
         coords = self.coords
-        n1, n2, n3 = n 
         av = self.av
         self.orig_av = av
         atom_list = self._atom_list
 
         _n1 = list(range(n[0]))
         _n2 = list(range(n[1]))
         _n3 = list(range(n[2]))
-        _n = np.array([[_n1[i], _n2[j], _n3[k]] for i in range(len(_n1)) for j in range(len(_n2)) for k in range(len(_n3))])
-        coords = np.array([coord + _n[i] for i in range(len(_n)) for coord in coords], dtype=float)
+        _n = np.array([[_n1[i], _n2[j], _n3[k]]
+                       for i in range(len(_n1))
+                       for j in range(len(_n2))
+                       for k in range(len(_n3))])
+
+        coords = np.array([coord + _n[i]
+                           for i in range(len(_n))
+                           for coord in coords], dtype=float)
 
         for i in range(len(coords)):
             coords[i, 0] = coords[i, 0] / n[0]
             coords[i, 1] = coords[i, 1] / n[1]
             coords[i, 2] = coords[i, 2] / n[2]
 
         av[0], av[1], av[2] = av[0] * n[0], av[1] * n[1], av[2] * n[2]
         atom_list = [atom_list] * np.prod(n)
         atom_list = np.array(atom_list).flatten()
 
         self.coords = coords
-        self.av = av 
+        self.av = av
         self._atom_list = atom_list
 
+    def supercell_reorder(self):
+        coords = self.coords
+        _atom_list = self._atom_list
+        coords = np.concatenate((_atom_list.reshape(-1, 1), coords), axis=1)
+        coords = coords[coords[:, 0].argsort()]
+        self.coords = coords[:, 1:]
+        self._atom_list = coords[:, 0]
+
+        atoms = []
+        for i in self._atom_list:
+            if i not in atoms:
+                atoms.append(i)
+        
+        natoms = [list(self._atom_list).count(i) for i in atoms]
+
+        self.atoms = atoms
+        self.natoms = natoms
+
     def Const_shift(self, vector: np.ndarray) -> np.ndarray:
         '''
-        Shifts the structure by a constant vector. 
+        Shifts the structure by a constant vector.
         '''
-        coords = self.coords 
-        coords += vector 
+        coords = self.coords
+        coords += vector
         if self._type == 'direct':
-            coords %= 1 
-        else: 
+            coords %= 1
+        else:
             pass
-        return coords
+        self.coords = coords
 
-    def Calculate_mesh(self) -> np.ndarray: 
+    def Calculate_mesh(self) -> np.ndarray:
         '''
         Calculates K-point mesh.
         '''
         kpoint_mesh = []
         kspacing_min, kspacing_max = 0.05, 0.5
-        av = self.av 
-        bv = self.bv 
+        av = self.av
+        bv = self.bv
         bv_norm = np.array([np.linalg.norm(x) for x in bv], dtype=float)
 
-        temp = [(i,norm) for i, norm in enumerate(bv_norm)]
+        temp = [(i, norm) for i, norm in enumerate(bv_norm)]
         temp.sort(key=lambda x: x[1], reverse=True)
 
-        i1, i2, i3 = [i for i,_ in temp]
+        i1, i2, i3 = [i for i, _ in temp]
 
         # Calculate the number of subdivisions N1, N2, N3 in the reciprocal lattice vectors 
         N_max = max(1, int(np.ceil(bv_norm[i1] / kspacing_min)))
         N_min = max(1, int(np.ceil(bv_norm[i1] / kspacing_max)))
 
         for n1 in range(N_min, N_max):
             min_spacing = bv_norm[i1] / n1
             if np.fabs(bv_norm[i2] - bv_norm[i1]) < 1e-5:
-                n2 = n1 
+                n2 = n1
             else:
                 n2 = int(np.ceil(bv_norm[i2] / min_spacing))
-                n2 = max(n2, 1) 
+                n2 = max(n2, 1)
 
             if np.fabs(bv_norm[i3] - bv_norm[i2]) < 1e-5:
-                n3 = n2 
+                n3 = n2
             else:
                 n3 = int(np.ceil(bv_norm[i3] / min_spacing))
                 n3 = max(n3, 1)
 
             if bv_norm[i2] / n2 < kspacing_max and bv_norm[i3] / n3 < kspacing_max:
                 mesh = np.array([None, None, None])
             
             mesh[i1], mesh[i2], mesh[i3] = n1, n2, n3 
             kpoint_mesh.append(mesh)
 
-        # calculate kpoint density 
+        # calculate kpoint density
         volume = np.linalg.det(bv)
         density = np.array([[np.prod(mesh) / volume] for mesh in kpoint_mesh], dtype=float)
 
         return np.array(kpoint_mesh, dtype=int), density
 
     def _ENCUT(self) -> np.ndarray:
         '''
         Calculates possible ENCUT values to test for convergence.
         '''
-        # check if POTCAR file exits 
+        # check if POTCAR file exits
         if not os.path.isfile('POTCAR'):
-            raise Warning('POTCAR file not found. Please generate POTCAR file first.') 
+            raise Warning('POTCAR file not found. Please generate POTCAR file first.')
 
-        with open('POTCAR', 'r') as f: 
-            lines = f.readlines() 
-        enmax = [float(re.findall(r'ENMAX = ([0-9]+.[0-9]+)', x)[0]) for x in lines if 'ENMAX' in x] 
-        encut = max(enmax) * 1.3 
-        encut = round(encut / 50) * 50 
+        with open('POTCAR', 'r') as f:
+            lines = f.readlines()
+        enmax = [float(re.findall(r'ENMAX = ([0-9]+.[0-9]+)', x)[0]) for x in lines if 'ENMAX' in x]
+        encut = max(enmax) * 1.3
+        encut = round(encut / 50) * 50
         encut_list = [x for x in range(encut - 300, encut + 300, 50)]
         self.encut = encut_list
         return np.array(encut_list)
 
     def _find_index(self, atom: str):
         '''
-        finds the index of the supplied atom in the coords and then returns the index of the atom in the atom_list 
+        finds the index of the supplied atom in the coords
+        and then returns the index of the atom in the atom_list
         '''
         atom = re.split(r'(\d+)', atom)
         for ind, symb in enumerate(self.atoms):
             if symb == atom[0]:
                 atom_index = ind
 
         _prev = np.sum(self.natoms[:atom_index])
-        location = _prev + int(atom[1]) - 1
+        location = int(_prev) + int(atom[1]) - 1
         vector = - self.coords[location]
 
         self.vector = vector
 
     def _build_region(self):
         coords = self.cart_coords
         atom_list = self._atom_list
-        atom_list = np.array(atom_list).reshape(-1,1)
+        atom_list = np.array(atom_list).reshape(-1, 1)
         coords = np.concatenate((atom_list, coords), axis=1)
         a1, a2, a3 = self.orig_av
         a1, a2, a3 = np.linalg.norm(a1), np.linalg.norm(a2), np.linalg.norm(a3)
         a = np.min([a1, a2, a3])
 
         # build a region around the atom of shape a1 x a2 x a3
-        region = np.array([coords[i] for i in range(len(coords)) if np.linalg.norm(coords[i, 1:]) < a/2])
+        region = np.array([coords[i]
+                           for i in range(len(coords))
+                           if np.linalg.norm(coords[i, 1:]) < a/2])
+
         coords = np.array(region[:, 1:], dtype=float)
         atom_list = region[:, 0]
         self.cart_coords = coords
         self._atom_list = atom_list
         self.name = self.name + '_qm'
 
     def write_xyz(self):
         '''
         Writes an xyz file
         '''
         coords = self.cart_coords
-        atom_list = self._atom_list 
+        atom_list = self._atom_list
         name = self.name
 
         with open(f'{name}.xyz', 'w') as f:
             f.write(f'{len(coords)}\n\n')
             for i in range(len(coords)):
                 f.write(f'{atom_list[i]} {coords[i,0]} {coords[i,1]} {coords[i,2]}\n')
 
@@ -290,33 +321,33 @@
             f.write(f'{self._type}\n')
             for x in self.coords:
                 f.write(f'{" ".join([str(y) for y in x])}\n')
 
 
 class DOPE():
     """
-    A class doping materials. 
+    A class doping materials.
 
     Returns:
         POSCAR: POSCAR files containing the doped structures.
     """
     def __init__(
             self, 
-            filename: str, 
-            dopant: str, 
+            filename: str,
+            dopant: str,
             replace: str,
             instances: int):
         '''
         Initializes the DOPE class
         '''
         self.filename = filename
-        self.dopant = dopant 
+        self.dopant = dopant
         self.replace = replace
         self.instances = instances 
-        self._s = Structure(filename) 
+        self._s = Structure(filename)
         self._s.Vasp_reader()
 
     def Symbol_coords(self) -> np.ndarray: 
         '''
         Returns the symbol and coordinates of the atoms in the structure.
         '''
         return np.hstack((np.array(self._s._atom_list).reshape(-1,1), self._s.coords))
@@ -549,15 +580,15 @@
 
     def _origin_index(self) -> int:
         '''
         Finds the index of the origi atom.
         '''
         coords = self._s.coords
         for ind, val in enumerate(coords):
-            if np.allclose(val, [0,0,0]):
+            if np.allclose(val, [0, 0, 0]):
                 return ind
 
     def _nearest_neighbours(self, coords: np.ndarray, point: np.ndarray, bond_max: float) -> np.ndarray:
         neighbours = sp.spatial.KDTree(coords[:,1:], leafsize=10, compact_nodes=True, balanced_tree=True) 
         dist, ind = neighbours.query(point, k=10)
         ind = [ind[i] for i in range(len(ind)) if dist[i] < bond_max]
         coords = np.array([coords[i] for i in ind])
@@ -569,24 +600,24 @@
         '''
         with open(f'{self._s.name}_asymmetric_unit.xyz', 'w') as f:
             f.write(f'{len(self.asymm_unit)}\n')
             f.write(f'{self._s.name}\n') 
             for atom in self.asymm_unit: 
                 f.write(f'{atom[0]} {atom[1]} {atom[2]} {atom[3]}\n')
 
-
     @timer
     def find_unit(self) -> None:
         '''
         Finds the asymmetric unit.
         '''
         self._locate_atom()
         self._translate()
+        atom_list = np.array(self._s._atom_list).reshape(-1,1)
         origin = self._origin_index()
-        coords = np.hstack((self._s._atom_list, np.array(self._s.cart_coords, dtype=float)))
+        coords = np.concatenate((atom_list, self._s.cart_coords), axis=1)
 
         asymm_unit = np.array([coords[origin]])
         searching = True 
         while searching:
             total_coords = []
             for i in asymm_unit:
                 if not i[0] == 'H':
```

### Comparing `vasp_suite-1.2.1/vasp_suite/submission.py` & `vasp_suite-1.2.2/vasp_suite/submission.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.1/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.2.2/vasp_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.2.1
+Version: 1.2.2
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

