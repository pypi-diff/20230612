# Comparing `tmp/abics-2.0.1.tar.gz` & `tmp/abics-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abics-2.0.1.tar", max compression
+gzip compressed data, was "abics-2.1.0.tar", max compression
```

## Comparing `abics-2.0.1.tar` & `abics-2.1.0.tar`

### file list

```diff
@@ -1,36 +1,52 @@
--rw-r--r--   0        0        0     2318 2022-06-24 12:51:30.301926 abics-2.0.1/README.md
--rw-r--r--   0        0        0        7 2022-06-24 01:22:15.000000 abics-2.0.1/abics/.gitignore
--rw-r--r--   0        0        0       22 2022-11-04 11:26:55.374361 abics-2.0.1/abics/__init__.py
--rw-r--r--   0        0        0        0 2022-06-24 01:22:15.000000 abics-2.0.1/abics/applications/__init__.py
--rw-r--r--   0        0        0      819 2022-08-23 04:46:23.000000 abics-2.0.1/abics/applications/latgas_abinitio_interface/__init__.py
--rw-r--r--   0        0        0     9635 2022-11-04 11:26:55.375297 abics-2.0.1/abics/applications/latgas_abinitio_interface/aenet.py
--rw-r--r--   0        0        0     6701 2022-06-24 12:51:05.836773 abics-2.0.1/abics/applications/latgas_abinitio_interface/aenet_trainer.py
--rw-r--r--   0        0        0     4747 2022-11-04 11:26:55.377085 abics-2.0.1/abics/applications/latgas_abinitio_interface/base_solver.py
--rw-r--r--   0        0        0     5817 2022-11-04 11:26:55.377941 abics-2.0.1/abics/applications/latgas_abinitio_interface/default_observer.py
--rw-r--r--   0        0        0     3348 2022-11-04 11:26:55.379070 abics-2.0.1/abics/applications/latgas_abinitio_interface/defect.py
--rw-r--r--   0        0        0     1310 2022-11-04 11:26:55.380339 abics-2.0.1/abics/applications/latgas_abinitio_interface/map2perflat.py
--rw-r--r--   0        0        0     5017 2022-11-04 07:40:38.000000 abics-2.0.1/abics/applications/latgas_abinitio_interface/mocksolver.py
--rw-r--r--   0        0        0    29595 2022-11-04 11:26:55.381883 abics-2.0.1/abics/applications/latgas_abinitio_interface/model_setup.py
--rw-r--r--   0        0        0      912 2022-11-04 11:26:55.382453 abics-2.0.1/abics/applications/latgas_abinitio_interface/naive_matcher.py
--rw-r--r--   0        0        0    13732 2022-06-24 12:51:05.838467 abics-2.0.1/abics/applications/latgas_abinitio_interface/openmx.py
--rw-r--r--   0        0        0     6338 2022-07-20 07:01:45.954566 abics-2.0.1/abics/applications/latgas_abinitio_interface/params.py
--rw-r--r--   0        0        0    15542 2022-09-26 01:57:58.049733 abics-2.0.1/abics/applications/latgas_abinitio_interface/qe.py
--rw-r--r--   0        0        0    29352 2022-11-04 11:26:55.383234 abics-2.0.1/abics/applications/latgas_abinitio_interface/run_base_mpi.py
--rw-r--r--   0        0        0     7831 2022-06-24 12:51:05.839751 abics-2.0.1/abics/applications/latgas_abinitio_interface/vasp.py
--rw-r--r--   0        0        0     1245 2022-11-04 11:26:55.384313 abics-2.0.1/abics/exception.py
--rw-r--r--   0        0        0    13840 2022-11-04 11:26:55.384608 abics-2.0.1/abics/mc.py
--rw-r--r--   0        0        0    31255 2022-11-04 11:26:55.384994 abics-2.0.1/abics/mc_mpi.py
--rw-r--r--   0        0        0     9307 2022-11-04 11:26:55.386448 abics-2.0.1/abics/replica_params.py
--rw-r--r--   0        0        0        0 2022-06-24 01:22:15.000000 abics-2.0.1/abics/scripts/__init__.py
--rw-r--r--   0        0        0     3296 2022-11-04 11:26:55.387587 abics-2.0.1/abics/scripts/abicsRXsepT.py
--rw-r--r--   0        0        0    21349 2022-11-04 11:26:55.388692 abics-2.0.1/abics/scripts/activelearn.py
--rw-r--r--   0        0        0     8501 2022-11-04 11:26:55.388941 abics-2.0.1/abics/scripts/activelearn_spawn.py
--rw-r--r--   0        0        0      384 2022-06-24 12:51:05.842275 abics-2.0.1/abics/scripts/input_template.toml
--rw-r--r--   0        0        0    14181 2022-11-04 11:26:55.395053 abics-2.0.1/abics/scripts/main.py
--rw-r--r--   0        0        0     1091 2022-06-24 12:51:06.073466 abics-2.0.1/abics/scripts/mocksolver.py
--rw-r--r--   0        0        0     6247 2022-06-24 12:51:05.843039 abics-2.0.1/abics/scripts/st2abics_config.py
--rw-r--r--   0        0        0     8689 2022-11-04 11:26:55.396034 abics-2.0.1/abics/scripts/train.py
--rw-r--r--   0        0        0     5367 2022-11-04 11:26:55.396536 abics-2.0.1/abics/util.py
--rw-r--r--   0        0        0      939 2022-11-04 11:26:55.411831 abics-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 abics-2.0.1/setup.py
--rw-r--r--   0        0        0     3236 1970-01-01 00:00:00.000000 abics-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2334 2023-06-12 13:48:54.574760 abics-2.1.0/README.md
+-rw-r--r--   0        0        0        7 2023-06-12 13:48:54.574760 abics-2.1.0/abics/.gitignore
+-rw-r--r--   0        0        0       22 2023-06-12 13:48:54.574760 abics-2.1.0/abics/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 13:48:54.574760 abics-2.1.0/abics/applications/__init__.py
+-rw-r--r--   0        0        0     1041 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/__init__.py
+-rw-r--r--   0        0        0    10112 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/aenet.py
+-rw-r--r--   0        0        0     6832 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/aenet_pylammps.py
+-rw-r--r--   0        0        0     8306 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/aenet_trainer.py
+-rw-r--r--   0        0        0     6362 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/base_solver.py
+-rw-r--r--   0        0        0    10626 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/default_observer.py
+-rw-r--r--   0        0        0     8105 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/defect.py
+-rw-r--r--   0        0        0     1422 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/map2perflat.py
+-rw-r--r--   0        0        0    57122 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/model_setup.py
+-rw-r--r--   0        0        0      923 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/naive_matcher.py
+-rw-r--r--   0        0        0    14007 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/openmx.py
+-rw-r--r--   0        0        0     6890 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/params.py
+-rw-r--r--   0        0        0    16067 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/qe.py
+-rw-r--r--   0        0        0    28755 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/run_base_mpi.py
+-rw-r--r--   0        0        0     5590 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/user_function_solver.py
+-rw-r--r--   0        0        0     8063 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/latgas_abinitio_interface/vasp.py
+-rw-r--r--   0        0        0        0 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/lattice_model/__init__.py
+-rw-r--r--   0        0        0     3575 2023-06-12 13:48:54.578760 abics-2.1.0/abics/applications/lattice_model/potts.py
+-rw-r--r--   0        0        0     1255 2023-06-12 13:48:54.578760 abics-2.1.0/abics/exception.py
+-rw-r--r--   0        0        0      368 2023-06-12 13:48:54.578760 abics-2.1.0/abics/loggers/README.txt
+-rw-r--r--   0        0        0      113 2023-06-12 13:48:54.578760 abics-2.1.0/abics/loggers/__init__.py
+-rw-r--r--   0        0        0    13407 2023-06-12 13:48:54.578760 abics-2.1.0/abics/loggers/loggers.py
+-rw-r--r--   0        0        0      909 2023-06-12 13:48:54.578760 abics-2.1.0/abics/mc.py
+-rw-r--r--   0        0        0     1043 2023-06-12 13:48:54.578760 abics-2.1.0/abics/mc_mpi.py
+-rw-r--r--   0        0        0     2715 2023-06-12 13:48:54.578760 abics-2.1.0/abics/mlref.py
+-rw-r--r--   0        0        0     2967 2023-06-12 13:48:54.578760 abics-2.1.0/abics/model.py
+-rw-r--r--   0        0        0     7052 2023-06-12 13:48:54.578760 abics-2.1.0/abics/observer.py
+-rw-r--r--   0        0        0     8319 2023-06-12 13:48:54.578760 abics-2.1.0/abics/replica_params.py
+-rw-r--r--   0        0        0        0 2023-06-12 13:48:54.578760 abics-2.1.0/abics/sampling/__init__.py
+-rw-r--r--   0        0        0     8543 2023-06-12 13:48:54.578760 abics-2.1.0/abics/sampling/mc.py
+-rw-r--r--   0        0        0     8365 2023-06-12 13:48:54.578760 abics-2.1.0/abics/sampling/mc_mpi.py
+-rw-r--r--   0        0        0    18028 2023-06-12 13:48:54.578760 abics-2.1.0/abics/sampling/pamc.py
+-rw-r--r--   0        0        0     4587 2023-06-12 13:48:54.578760 abics-2.1.0/abics/sampling/resampling.py
+-rw-r--r--   0        0        0    19739 2023-06-12 13:48:54.578760 abics-2.1.0/abics/sampling/rxmc.py
+-rw-r--r--   0        0        0    12340 2023-06-12 13:48:54.578760 abics-2.1.0/abics/sampling/simple_parallel.py
+-rw-r--r--   0        0        0        0 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/__init__.py
+-rw-r--r--   0        0        0     4070 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/abicsRXsepT.py
+-rw-r--r--   0        0        0    21158 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/activelearn.py
+-rw-r--r--   0        0        0      384 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/input_template.toml
+-rw-r--r--   0        0        0     1821 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/main.py
+-rw-r--r--   0        0        0    14843 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/main_dft_latgas.py
+-rw-r--r--   0        0        0     7174 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/main_potts.py
+-rw-r--r--   0        0        0     1091 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/mocksolver.py
+-rw-r--r--   0        0        0     6252 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/st2abics_config.py
+-rw-r--r--   0        0        0    10449 2023-06-12 13:48:54.578760 abics-2.1.0/abics/scripts/train.py
+-rw-r--r--   0        0        0     5770 2023-06-12 13:48:54.578760 abics-2.1.0/abics/util.py
+-rw-r--r--   0        0        0     1008 2023-06-12 13:48:54.622760 abics-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 abics-2.1.0/PKG-INFO
```

### Comparing `abics-2.0.1/README.md` & `abics-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 ## Official page
 
 https://www.pasums.issp.u-tokyo.ac.jp/abics
 
 ## Author
 
-Shusuke Kasamatsu, Yuichi Motoyama, Kazuyoshi Yoshimi
+Shusuke Kasamatsu, Yuichi Motoyama, Tatsumi Aoyama, Kazuyoshi Yoshimi
 
 ## Manual
 
 [English online manual](https://issp-center-dev.github.io/abICS/docs/master/en/html/index.html)
 
 [Japnese online manual](https://issp-center-dev.github.io/abICS/docs/master/ja/html/index.html)
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/__init__.py` & `abics-2.1.0/abics/mc_mpi.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,10 +10,12 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
-from .default_observer import *
-from .map2perflat import *
-from .aenet_trainer import *
+from abics.mlref import RefParams
+from abics.sampling.mc_mpi import ParallelMC, RX_MPI_init
+from abics.sampling.pamc import PopulationAnnealing, PAMCParams
+from abics.sampling.rxmc import RXParams, TemperatureRX_MPI
+from abics.sampling.simple_parallel import EmbarrassinglyParallelSampling, ParallelRandomParams
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/aenet.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/aenet.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,33 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
-from .base_solver import SolverBase
-from collections import namedtuple
-import numpy as np
-from pymatgen.core import Structure
-import os
-import sys, shutil, io
-
-
 """
 Adapted from pymatgen.io.xcrysden distributed under the MIT License
 # Copyright (c) Pymatgen Development Team.
 # Distributed under the terms of the MIT License.
 """
 
+from __future__ import annotations
+
+import os
+import sys, shutil, io
+from collections import namedtuple
+import numpy as np
+from pymatgen.core import Structure
+
+from .base_solver import SolverBase, register_solver
+from .params import ALParams, DFTParams
+
 
-def to_XSF(structure, write_force_zero=False):
+def to_XSF(structure: Structure, write_force_zero=False):
     """
     Returns a string with the structure in XSF format
     See http://www.xcrysden.org/doc/XSF.html
     """
     lines = []
     app = lines.append
 
@@ -46,37 +49,38 @@
 
     cart_coords = structure.cart_coords
     app("# Cartesian coordinates in Angstrom.")
     app("PRIMCOORD")
     app(" %d 1" % len(cart_coords))
     species = structure.species
     site_properties = structure.site_properties
-    if 'forces' not in site_properties.keys():
+    if "forces" not in site_properties.keys():
         write_force_zero = True
     else:
-        forces = site_properties['forces']
+        forces = site_properties["forces"]
 
     if write_force_zero:
         for a in range(len(cart_coords)):
             app(
                 str(species[a])
                 + " %20.14f %20.14f %20.14f" % tuple(cart_coords[a])
                 + " 0.0 0.0 0.0"
             )
     else:
         for a in range(len(cart_coords)):
-            app(str(species[a]) 
+            app(
+                str(species[a])
                 + " %20.14f %20.14f %20.14f" % tuple(cart_coords[a])
                 + " %20.14f %20.14f %20.14f" % tuple(forces[a])
             )
 
     return "\n".join(lines)
 
 
-def from_XSF(input_string):
+def from_XSF(input_string: str):
     """
     Initialize a `Structure` object from a string with data in XSF format.
 
     Args:
         input_string: String with the structure in XSF format.
             See http://www.xcrysden.org/doc/XSF.html
         cls_: Structure class to be created. default: pymatgen structure
@@ -120,58 +124,58 @@
     else:
         raise ValueError("Invalid XSF data")
 
     s = Structure(lattice, species, coords, coords_are_cartesian=True)
     return s
 
 
-class aenetSolver(SolverBase):
+class AenetSolver(SolverBase):
     """
     This class defines the aenet solver.
     """
 
-    def __init__(self, path_to_solver, ignore_species=None, run_scheme="subprocess"):
+    def __init__(self, path_to_solver: os.PathLike, ignore_species=None, run_scheme="subprocess"):
         """
         Initialize the solver.
 
         Parameters
         ----------
         path_to_solver : str
                       Path to the solver.
         """
-        super(aenetSolver, self).__init__(path_to_solver)
+        super(AenetSolver, self).__init__(path_to_solver)
         self.path_to_solver = path_to_solver
-        self.input = aenetSolver.Input(ignore_species, run_scheme)
-        self.output = aenetSolver.Output()
+        self.input = AenetSolver.Input(ignore_species, run_scheme)
+        self.output = AenetSolver.Output()
 
     def name(self):
         return "aenet"
 
     class Input(object):
-        def __init__(self, ignore_species, run_scheme="subprocess"):
+        def __init__(self, ignore_species : str | None, run_scheme="subprocess"):
             self.base_info = None
             self.pos_info = None
             self.ignore_species = ignore_species
             self.run_scheme = run_scheme
 
-        def from_directory(self, base_input_dir):
+        def from_directory(self, base_input_dir: os.PathLike):
             """
             Initialize information from files in base_input_dir.
 
             Parameters
             ----------
             base_input_dir : str
                 Path to the directory including base input files.
             """
 
             # set information of base_input and pos_info from files in base_input_dir
             self.base_info = os.path.abspath(base_input_dir)
             # self.pos_info = open('{}/structure.xsf'.format(base_input_dir), 'r').read()
 
-        def update_info_by_structure(self, structure):
+        def update_info_by_structure(self, structure: Structure):
             """
             Update information by atomic structure.
 
             Parameters
             ----------
             structure : pymatgen.Structure
                 Atomic structure
@@ -184,21 +188,21 @@
         def update_info_from_files(self, output_dir, rerun):
             """
             Do nothing.
             """
             print("rerun not implemented. Something has gone wrong")
             sys.exit(1)
 
-        def write_input(self, output_dir):
+        def write_input(self, output_dir: os.PathLike):
             """
             Generate input files of the solver program.
 
             Parameters
             ----------
-            output_dir : str
+            output_dir : os.PathLike
                 Path to working directory.
             """
             # Write input files
             if self.base_info is None:
                 raise AttributeError("Fail to set base_info.")
             os.makedirs(output_dir, exist_ok=True)
             for fname in os.listdir(self.base_info):
@@ -252,15 +256,15 @@
             phys : named_tuple("energy", "structure")
                 Total energy and atomic structure.
                 The energy is measured in the units of eV
                 and coordinates is measured in the units of Angstrom.
 
             """
             # Read results from files in output_dir and calculate values
-            Phys = namedtuple("PhysVaules", ("energy", "structure"))
+            Phys = namedtuple("PhysValues", ("energy", "structure"))
             with open(os.path.join(output_dir, "structure.xsf")) as f:
                 structure = from_XSF(f.read())
             with open(os.path.join(output_dir, "stdout")) as f:
                 lines = f.read()
                 fi_io = io.StringIO(lines)
                 line = fi_io.readline()
             if "optimized" in lines:
@@ -276,7 +280,16 @@
             while "Total energy" not in line:
                 line = fi_io.readline()
             energy = line.split()[-2]
             return Phys(np.float64(energy), structure)
 
     def solver_run_schemes(self):
         return ("subprocess", "mpi_spawn_ready")
+
+    @classmethod
+    def create(cls, params: ALParams | DFTParams):
+        path = params.path
+        ignore_species = params.ignore_species
+        run_scheme = params.solver_run_scheme
+        return cls(path, ignore_species, run_scheme)
+
+register_solver("aenet", AenetSolver)
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/aenet_trainer.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/aenet_trainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-from abics.applications.latgas_abinitio_interface import aenet
+from __future__ import annotations
+from typing import Sequence
+
 import numpy as np
-import os, pathlib, shutil, subprocess
+import os, pathlib, shutil, subprocess, shlex
 import time
 
+from pymatgen.core import Structure
+
+from abics.util import expand_cmd_path
+from abics.applications.latgas_abinitio_interface import aenet
 
 class aenet_trainer:
     def __init__(
         self,
-        structures,
-        energies,
-        generate_inputdir,
-        train_inputdir,
-        predict_inputdir,
-        generate_exe,
-        train_exe,
+        structures: Sequence[Structure],
+        energies: Sequence[float],
+        generate_inputdir: os.PathLike,
+        train_inputdir: os.PathLike,
+        predict_inputdir: os.PathLike,
+        generate_exe: str,
+        train_exe: str,
     ):
         self.structures = structures
         self.energies = energies
         self.generate_inputdir = generate_inputdir
         self.train_inputdir = train_inputdir
         self.predict_inputdir = predict_inputdir
-        self.generate_exe = generate_exe
-        self.train_exe = train_exe
+        self.generate_exe = [expand_cmd_path(e) for e in shlex.split(generate_exe)]
+        self.generate_exe.append("generate.in")
+        self.train_exe = [expand_cmd_path(e) for e in shlex.split(train_exe)]
+        self.train_exe.append("train.in")
+        # self.generate_exe = generate_exe
+        # self.train_exe = train_exe
         assert len(self.structures) == len(self.energies)
         self.numdata = len(self.structures)
         self.is_prepared = False
         self.is_trained = False
         self.generate_outputdir = None
 
     def prepare(self, latgas_mode = True, st_dir = "aenetXSF"):
@@ -57,14 +67,15 @@
 
     def generate_run(self, xsfdir="aenetXSF", generate_dir="generate"):
         # prepare generate
         xsfdir = str(pathlib.Path(xsfdir).resolve())
         if os.path.exists(generate_dir):
             shutil.rmtree(generate_dir)
         shutil.copytree(self.generate_inputdir, generate_dir)
+        self.generate_dir = generate_dir
         os.chdir(generate_dir)
         with open("generate.in.head", "r") as fi:
             generate_head = fi.read()
             xsf_paths = [
                 os.path.join(xsfdir, "structure.{}.xsf".format(i))
                 for i in range(self.numdata)
             ]
@@ -76,49 +87,68 @@
                 + "\n"
                 + "\n".join(xsf_paths)
                 + "\n"
             )
             with open("generate.in", "w") as fi_in:
                 fi_in.write(generate)
 
-        command = self.generate_exe + " generate.in"
+        # command = self.generate_exe + " generate.in"
         with open(os.path.join(os.getcwd(), "stdout"), "w") as fi:
             #subprocess.run(
             self.gen_proc = subprocess.Popen(
-                command, shell=True, stdout=fi, stderr=subprocess.STDOUT,#, check=True
+                self.generate_exe, stdout=fi, stderr=subprocess.STDOUT,#, check=True
                 )
         self.generate_outputdir = os.getcwd()
         os.chdir(pathlib.Path(os.getcwd()).parent)
         #self.is_prepared = True
         
     def generate_wait(self):
         self.gen_proc.wait()
-        self.is_prepared = True
+        timeout = 5.0 # sec
+        interval = 0.1 # sec
+        t = 0.0
+        self.is_prepared = False
+        while t < timeout:
+            if os.path.exists(os.path.join(self.generate_outputdir, "aenet.train")):
+                self.is_prepared = True
+                break
+            time.sleep(interval)
+        if not self.is_prepared:
+            raise RuntimeError(f"{self.generate_outputdir}")
 
     def train(self, train_dir = "train"):
-        try:
-            assert self.is_prepared
-        except AssertionError as e:
-            e.args += "you have to prepare the trainer before training!"
+        if not self.is_prepared:
+            raise RuntimeError("you have to prepare the trainer before training!")
         if os.path.exists(train_dir):
             shutil.rmtree(train_dir)
         shutil.copytree(self.train_inputdir, train_dir)
         os.chdir(train_dir)
         os.rename(
             os.path.join(self.generate_outputdir, "aenet.train"),
             os.path.join(os.getcwd(), "aenet.train"),
         )
-        command = self.train_exe + " train.in"
+        # command = self.train_exe + " train.in"
+        # print(os.getcwd())
+        # print(command)
+        # print(os.path.exists("train.in"))
 
         while True:
             # Repeat until test set error begins to rise
             with open(os.path.join(os.getcwd(), "stdout"), "w") as fi:
                 subprocess.run(
-                    command, shell=True, stdout=fi, stderr=subprocess.STDOUT, check=True
+                    self.train_exe, stdout=fi, stderr=subprocess.STDOUT, check=True
                 )
+                # try:
+                #     subprocess.run(
+                #         self.train_exe, stdout=fi, stderr=subprocess.STDOUT, check=True
+                #     )
+                # except subprocess.CalledProcessError as e:
+                #     print(e.stdout)
+                #     print(e.stderr)
+                #     raise
             with open("stdout", "r") as trainout:
                 fullout = trainout.readlines()
                 epoch_data = []
                 for li in fullout:
                     if "<" in li:
                         epoch_data.append(li)
             with open("epochdat", "w") as epochdatfi:
@@ -153,18 +183,26 @@
         # `baseinput_dir` is removed after `os.rename`.
         if os.path.exists(baseinput_dir):
             os.rename(baseinput_dir, baseinput_dir + "_temporary")
             shutil.rmtree(baseinput_dir + "_temporary")
         os.makedirs(baseinput_dir, exist_ok=False)
         while not os.path.exists(baseinput_dir):
             time.sleep(0.1)
-        shutil.copyfile(
-            os.path.join(self.predict_inputdir, "predict.in"),
-            os.path.join(baseinput_dir, "predict.in"),
-        )
+
+        iflg = False
+        for name in ["predict.in", "in.lammps"]:
+            if os.path.isfile(os.path.join(self.predict_inputdir, name)):
+                iflg = True
+                shutil.copyfile(
+                    os.path.join(self.predict_inputdir, name),
+                    os.path.join(baseinput_dir, name),
+                )
+        if iflg is False:
+            print("Warning: predict.in or in.lammps should be in the predict directory.")
+
 
         NNPid_str = "{:05d}".format(self.train_minID)
         NNPfiles = [fi for fi in os.listdir(self.train_outputdir) if NNPid_str in fi]
         for fi in NNPfiles:
             shutil.copyfile(
                 os.path.join(self.train_outputdir, fi),
                 os.path.join(baseinput_dir, fi),
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/base_solver.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/user_function_solver.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,99 +10,129 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
+"""
+User-defined function as energy calculator
+"""
+
+from __future__ import annotations
+
 from collections import namedtuple
+import os
+import sys
+import importlib
+
+from pymatgen.core import Structure
+
+from .base_solver import SolverBase, register_solver
+from .params import ALParams, DFTParams
 
 
-class SolverBase(object):
+class UserFunctionSolver(SolverBase):
     """
-    Base class defining the common interface of solvers.
+    UserFunction solver
 
     Attributes
     ----------
-    path_to_solver : str
-        Path to solver program.
-    input : SolverBase.Input
-        Input manager.
-    output : SolverBase.Output
-        Output manager.
+    path_to_solver : function(st) -> float
+    input : SimpleFunctionSolver.Input
+        Input manager
+    output : SimpleFunctionSolver.Output
+        Output manager
     """
 
+    def __init__(self, function = None):
+        """
+        Initialize the solver.
+
+        """
+        super(UserFunctionSolver, self).__init__("")
+        self.input = UserFunctionSolver.Input()
+        self.output = UserFunctionSolver.Output()
+        self.path_to_solver = self.__call__
+        self.__fn = function
+
+    def __call__(self, fi, output_dir):
+        st = self.input.st
+        if self.__fn is None:
+            raise ValueError("Function is not set")
+        ene = self.__fn(st)
+        with open(os.path.join(output_dir, "energy.dat"), "w") as f:
+            f.write("{:.15f}\n".format(ene))
+
+    def name(self):
+        return "UserFunction"
+
+    def set_function(self, fn):
+        self.__fn = fn
+
     class Input(object):
         """
-        Input manager.
+        Input manager for SimpleFunction
 
         Attributes
         ----------
-        base_info : Any
-            Common parameter.
-        pos_info : Any
-            Information of position.
+        st : pymatgen.Structure
+            structure
         """
 
+        st: Structure
+
         def __init__(self):
-            self.base_info = None
-            self.pos_info = None
+            # self.st = Structure()
+            pass
 
-        def update_info_by_structure(self, structure):
+        def from_directory(self, base_input_dir):
             """
-            Update information by structure.
 
             Parameters
             ----------
-            structure : pymatgen.Structure
-                Atomic structure.
-
+            base_input_dir : str
+                Path to the directory including base input files.
             """
-            return None
+            pass
 
-        def update_info_from_files(self, workdir, rerun):
+        def update_info_by_structure(self, structure):
             """
-            Update information by result files.
+            Update information by structure file
 
             Parameters
             ----------
-            workdir : str
-                Path to working directory.
-            rerun : int
+            structure : pymatgen.Structure
+                Atomic structure
             """
+            self.st = structure
 
-            return None
+        def update_info_from_files(self, workdir, rerun):
+            """
+            Do nothing
+            """
+            pass
 
-        def write_input(self, workdir):
+        def write_input(self, output_dir):
             """
             Generate input files of the solver program.
 
             Parameters
             ----------
             workdir : str
                 Path to working directory.
             """
-            return None
-
-        def from_directory(self, base_input_dir):
-            """
-            Set information, base_input and pos_info, from files in the base_input_dir
-
-            Parameters
-            ----------
-            base_input_dir : str
-                Path to the directory including base input files.
-            """
-            # set information of base_input and pos_info from files in base_input_dir
-            self.base_info = {}
-            self.pos_info = {}
+            os.makedirs(output_dir, exist_ok=True)
+            self.st.to(
+                fmt="POSCAR", filename=os.path.join(output_dir, "structure.vasp")
+            )
 
         def cl_args(self, nprocs, nthreads, workdir):
             """
-            Generate command line arguments of the solver program.
+            Generate command line argument of the solver program.
 
             Parameters
             ----------
             nprocs : int
                 The number of processes.
             nthreads : int
                 The number of threads.
@@ -110,20 +140,24 @@
                 Path to the working directory.
 
             Returns
             -------
             args : list[str]
                 Arguments of command
             """
-            return []
+            return [workdir]
 
     class Output(object):
         """
         Output manager.
         """
+
+        def __init__(self):
+            pass
+
         def get_results(self, workdir):
             """
             Get energy and structure obtained by the solver program.
 
             Parameters
             ----------
             workdir : str
@@ -132,44 +166,34 @@
             Returns
             -------
             phys : named_tuple("energy", "structure")
                 Total energy and atomic structure.
                 The energy is measured in the units of eV
                 and coodinates is measured in the units of Angstrom.
             """
-            Phys = namedtuple("PhysVaules", ("energy", "structure"))
-            # Read results from files in workdir and calculate values
-            phys = Phys(0.0, None)
-            return phys
+            # Read results from files in output_dir and calculate values
+            Phys = namedtuple("PhysValues", ("energy", "structure"))
+            with open(os.path.join(workdir, "energy.dat")) as f:
+                ene = float(f.read())
+            st = Structure.from_file(os.path.join(workdir, "structure.vasp"))
+            return Phys(ene, st)
 
-    def __init__(self, path_to_solver):
-        """
-        Initialize the solver.
+    def solver_run_schemes(self):
+        return ("function",)
 
-        Parameters
-        ----------
-        solver_name : str
-            Solver name.
-        path_to_solver : str
-            Path to the solver.
-        """
-        self.path_to_solver = path_to_solver
-        self.input = SolverBase.Input
-        self.output = SolverBase.Output
+    @classmethod
+    def create(cls, params: ALParams | DFTParams):
+        fn = None
+        if params.function_module:
+            sys.path.append(os.getcwd())
+            pkg = params.function_module.split('.')
+            modname = '.'.join(pkg[:-1])
+            funcname = pkg[-1]
+            try:
+                mod = importlib.import_module(modname)
+                fn = getattr(mod, funcname)
+            except ImportError:
+                raise ImportError(f"Cannot import module {modname}")
+        return cls(fn)
 
-    def name(self):
-        """
-        Returns
-        -------
-        name : str
-            Name of solver.
-        """
-        return "Base solver"
 
-    def solver_run_schemes(self):
-        """
-        Returns
-        -------
-        schemes : tuple[str]
-            Implemented runner schemes.
-        """
-        return ()
+register_solver("User", UserFunctionSolver)
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/default_observer.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/base_solver.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,179 +10,231 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
-from abics.mc import observer_base
-from ...util import expand_path
+from __future__ import annotations
 
-import os
-import numpy as np
+from collections import namedtuple
 
+from pymatgen.core.structure import Structure
 
-class default_observer(observer_base):
+from .params import ALParams, DFTParams
+
+class SolverBase(object):
     """
-    Default observer.
+    Base class defining the common interface of solvers.
 
     Attributes
     ----------
-    minE : float
-        Minimum of energy
+    path_to_solver : str
+        Path to solver program.
+    input : SolverBase.Input
+        Input manager.
+    output : SolverBase.Output
+        Output manager.
     """
-    def __init__(self, comm, Lreload=False):
-        """
-
-        Parameters
-        ----------
-        comm: mpi4py.MPI.Intracomm
-            MPI communicator
-        Lreload: bool
-            Reload or not
-        """
-        super(default_observer, self).__init__()
-        self.minE = 100000.0
-        myrank = comm.Get_rank()
-        if Lreload:
-            with open(os.path.join(str(myrank), "minEfi.dat"), "r") as f:
-                self.minE = float(f.readlines()[-1])
-            with open(os.path.join(str(myrank), "obs.dat"), "r") as f:
-                self.lprintcount = int(f.readlines()[-1].split()[0]) + 1
 
-    def logfunc(self, calc_state):
+    class Input(object):
         """
+        Input manager.
 
-        Parameters
+        Attributes
         ----------
-        calc_state: MCalgo
-        Object of Monte Carlo algorithm
-        Returns
-        -------
-        calc_state.energy : float
-        Minimum energy
+        base_info : Any
+            Common parameter.
+        pos_info : Any
+            Information of position.
         """
-        if calc_state.energy < self.minE:
-            self.minE = calc_state.energy
-            with open("minEfi.dat", "a") as f:
-                f.write(str(self.minE) + "\n")
-            calc_state.config.structure.to(fmt="POSCAR", filename="minE.vasp")
-        return calc_state.energy
 
-    def writefile(self, calc_state):
-        """
+        def __init__(self) -> None:
+            self.base_info = None
+            self.pos_info = None
 
-        Parameters
-        ----------
-        calc_state: MCalgo
-        Object of Monte Carlo algorithm
+        def update_info_by_structure(self, structure: Structure) -> None:
+            """
+            Update information by structure.
 
-        """
-        calc_state.config.structure.to(
-            fmt="POSCAR", filename="structure." + str(self.lprintcount) + ".vasp"
-        )
-        calc_state.config.structure_norel.to(
-            fmt="POSCAR", filename="structure_norel." + str(self.lprintcount) + ".vasp"
-        )
+            Parameters
+            ----------
+            structure : pymatgen.Structure
+                Atomic structure.
 
-class ensemble_error_observer(default_observer):
-    def __init__(self, comm, energy_calculators, Lreload=False):
-        """
+            """
+            return None
 
-        Parameters
-        ----------
-        comm: mpi4py.MPI.Intracomm
-            MPI communicator
-        energy_calculators: abics.applications.latgas_abinitio_interface.run_base_mpi.runner
-            setup of the energy calculator
-        Lreload: bool
-            Reload or not
-        """
-        super(ensemble_error_observer, self).__init__(comm, Lreload)
-        self.calculators = energy_calculators
-        self.comm = comm
-
-    def logfunc(self, calc_state):
-        if calc_state.energy < self.minE:
-            self.minE = calc_state.energy
-            with open("minEfi.dat", "a") as f:
-                f.write(str(self.minE) + "\n")
-            calc_state.config.structure.to(fmt="POSCAR", filename="minE.vasp")
-        energies = [calc_state.energy]
-        npar = self.comm.Get_size()
-        if npar > 1:
-            assert(npar == len(self.calculators))
-            myrank = self.comm.Get_rank()
-            energy, _ = self.calculators[myrank].submit(calc_state.config.structure, os.path.join(os.getcwd(),"ensemble{}".format(myrank)))
-            energies_tmp = self.comm.allgather(energy)
-            std = np.std(energies_tmp, ddof=1)
-
-        else:
-            energies_tmp = []
-            for i, calculator in enumerate(self.calculators):
-                energy, _ = calculator.submit(
-                        calc_state.config.structure, os.path.join(os.getcwd(), "ensemble{}".format(i))
-                )
-                energies_tmp.append(energy)
-            std = np.std(energies_tmp, ddof=1)
-        energies.extend(energies_tmp)
-        energies.append(std)
-        return np.asarray(energies)
+        def update_info_from_files(self, workdir, rerun) -> None:
+            """
+            Update information by result files.
+
+            Parameters
+            ----------
+            workdir : str
+                Path to working directory.
+            rerun : int
+            """
 
+            return None
 
+        def write_input(self, workdir) -> None:
+            """
+            Generate input files of the solver program.
+
+            Parameters
+            ----------
+            workdir : str
+                Path to working directory.
+            """
+            return None
 
-class EnsembleParams:
-    @classmethod
-    def from_dict(cls, d):
-        """
-        Read information from dictionary
-
-        Parameters
-        ----------
-        d: dict
-            Dictionary
+        def from_directory(self, base_input_dir) -> None:
+            """
+            Set information, base_input and pos_info, from files in the base_input_dir
+
+            Parameters
+            ----------
+            base_input_dir : str
+                Path to the directory including base input files.
+            """
+            # set information of base_input and pos_info from files in base_input_dir
+            self.base_info = {}
+            self.pos_info = {}
+
+        def cl_args(self, nprocs, nthreads, workdir) -> list[str]:
+            """
+            Generate command line arguments of the solver program.
+
+            Parameters
+            ----------
+            nprocs : int
+                The number of processes.
+            nthreads : int
+                The number of threads.
+            workdir : str
+                Path to the working directory.
+
+            Returns
+            -------
+            args : list[str]
+                Arguments of command
+            """
+            ret: list[str] = []
+            return ret
+
+    class Output(object):
+        """
+        Output manager.
+        """
+        def get_results(self, workdir):
+            """
+            Get energy and structure obtained by the solver program.
+
+            Parameters
+            ----------
+            workdir : str
+                Path to the working directory.
+
+            Returns
+            -------
+            phys : named_tuple("energy", "structure")
+                Total energy and atomic structure.
+                The energy is measured in the units of eV
+                and coodinates is measured in the units of Angstrom.
+            """
+            Phys = namedtuple("PhysValues", ("energy", "structure"))
+            # Read results from files in workdir and calculate values
+            phys = Phys(0.0, None)
+            return phys
+
+    def __init__(self, path_to_solver):
+        """
+        Initialize the solver.
+
+        Parameters
+        ----------
+        solver_name : str
+            Solver name.
+        path_to_solver : str
+            Path to the solver.
+        """
+        self.path_to_solver = path_to_solver
+        self.input = SolverBase.Input
+        self.output = SolverBase.Output
 
+    def name(self):
+        """
         Returns
         -------
-        params: EnsembleParams object
-            self
+        name : str
+            Name of solver.
         """
-        if "ensemble" in d:
-            d = d["ensemble"]
-        else:
-            return None
+        return "Base solver"
 
-        params = cls()
-        base_input_dirs = d.get("base_input_dirs", ["./baseinput"])
-        if isinstance(base_input_dirs, str):
-            base_input_dirs = [base_input_dirs]
-        params.base_input_dirs = base_input_dirs = list(
-            map(lambda x: expand_path(x, os.getcwd()), base_input_dirs)
-        )
-        params.solver = d["type"]
-        params.path = expand_path(d["path"], os.getcwd())
-        params.perturb = d.get("perturb", 0.1)
-        params.solver_run_scheme = d.get("run_scheme", "mpi_spawn_ready")
-        params.ignore_species = d.get("ignore_species", None)
-        params.constraint_module = d.get("constraint_module", None)
-        params.properties = d
-
-        return params
+    def solver_run_schemes(self):
+        """
+        Returns
+        -------
+        schemes : tuple[str]
+            Implemented runner schemes.
+        """
+        return ()
 
     @classmethod
-    def from_toml(cls, f):
+    def create(cls, params: ALParams | DFTParams) -> SolverBase:
         """
-        Read information from toml file
+        Create solver instance.
 
         Parameters
         ----------
-        f: str
-            Name of input toml File
+        params : ALParams or DFTParams
+            Parameters.
 
         Returns
         -------
-        oDFTParams: DFTParams object
-            self
+        solver : SolverBase
+            Solver instance.
         """
-        import toml
+        raise NotImplementedError()
+
 
-        return cls.from_dict(toml.load(f))
+__solver_table = {}
+
+def register_solver(solver_name: str, solver_class) -> None:
+    """
+    Register solver class.
+
+    Parameters
+    ----------
+    solver_name : str
+        Solver name (case insensible).
+    solver_class : SolverBase
+        Solver class, which should be a subclass of SolverBase.
+    """
+
+    if SolverBase not in solver_class.mro():
+        raise TypeError("solver_class must be a subclass of SolverBase")
+    __solver_table[solver_name.lower()] = solver_class
+
+
+def create_solver(solver_name, params: ALParams | DFTParams) -> SolverBase:
+    """
+    Create solver instance.
+
+    Parameters
+    ----------
+    solver_name : str
+        Solver name (case insensible).
+    params : ALParams or DFTParams
+        Parameters.
+
+    Returns
+    -------
+    solver : SolverBase
+        Solver instance.
+    """
+    sn = solver_name.lower()
+    if sn not in __solver_table:
+        raise ValueError(f"Unknown solver: {solver_name}")
+    solver_class = __solver_table[sn]
+    return solver_class.create(params)
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/defect.py` & `abics-2.1.0/abics/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,108 +10,99 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
-from pymatgen.core import Lattice
+from __future__ import annotations
 
-from .model_setup import config, defect_sublattice, base_structure
+from typing import Any
 
-from abics.exception import InputError
-from abics.util import read_matrix
+from abc import ABCMeta, abstractmethod
 
+import sys
 
-class DFTConfigParams:
-    def __init__(self, dconfig):
+from abics import __version__
+
+"""Defines base classes for Monte Carlo simulations"""
+
+
+class Model(metaclass=ABCMeta):
+    """This class defines a model whose energy equals 0 no matter the configuration, and the configuration
+    never changes.
+    This is a base template for building useful models."""
+
+    model_name = ""
+
+    # def __init__(self):
+
+    @abstractmethod
+    def energy(self, config) -> float:
         """
-        Get information from dictionary
+        Calculate energy of configuration: input: config
 
         Parameters
         ----------
-        dconfig: dict
-            Dictionary
-        """
-
-        if "config" in dconfig:
-            dconfig = dconfig["config"]
+        config: config object
+            configuration
 
-        if "unitcell" not in dconfig:
-            raise InputError('"unitcell" is not found in the "config" section.')
-        self.lat = Lattice(read_matrix(dconfig["unitcell"]))
-
-        self.supercell = dconfig.get("supercell", [1, 1, 1])
-
-        constraint_module = dconfig.get("constraint_module", False)
-        if constraint_module:
-            import os, sys
-
-            sys.path.append(os.getcwd())
-            from constraint_module import constraint_func
-
-            self.constraint_func = constraint_func
-        else:
-            self.constraint_func = bool
-
-        if "base_structure" not in dconfig:
-            raise InputError('"base_structure" is not found in the "config" section.')
-        self.base_structure = base_structure(self.lat, dconfig["base_structure"])
-
-        if "defect_structure" not in dconfig:
-            raise InputError('"defect_structure" is not found in the "config" section.')
-        self.defect_sublattices = [
-            defect_sublattice.from_dict(ds) for ds in dconfig["defect_structure"]
-        ]
-        self.num_defects = [
-            {g["name"]: g["num"] for g in ds["groups"]}
-            for ds in dconfig["defect_structure"]
-        ]
-
-    @classmethod
-    def from_dict(cls, d):
-        return cls(d)
+        Returns
+        -------
+        energy: float
 
-    @classmethod
-    def from_toml(cls, f):
         """
+        ...
 
-        Get information from toml file.
+    @abstractmethod
+    def trialstep(self, config, energy: float) -> tuple[Any, float]:
+        """Define a trial step on config
+
+        Returns dconfig, which can contain the minimal information for
+        constructing the trial configuration from config to be used in newconfig().
+        Make sure that config is unchanged.
 
         Parameters
         ----------
-        f: str
-            Name of input toml File
+        config: config object
+            current configuration
+
+        energy: float
+            current energy
 
         Returns
         -------
-        cls.from_dict: DFTConfigParams object
-            Parameters for DFT solver
+        dconfig: config object
+            The minimal information for constructing the trial configuration
+            from config to be used in newconfig()
+        dE: float
+            Energy difference
         """
-        import toml
 
-        return cls(toml.load(f))
+        # Return only change in configuration dconfig so that
+        # you don't have to copy entire configurations,
+        # which can sometimes be costly
+        ...
+
+    @abstractmethod
+    def newconfig(self, config, dconfig):
+        """
+        Update config by using the trial step, dconfig
 
+        Parameters
+        ----------
+        config: config object
+            Original configuration
+            This may be mutated through this function
+        dconfig: config object
+            Difference of configuration
+
+        Returns
+        -------
+        config: config object
+            updated configuration
+        """
+        return config
 
-def defect_config(cparam: DFTConfigParams):
-    """
-    Get configuration information
-
-    Parameters
-    ----------
-    cparam: DFTConfigParams object
-        Parameters for DFT solver
-
-    Returns
-    -------
-    spinel_config: config object
-        spinel configure object
-    """
-    spinel_config = config(
-        cparam.base_structure,
-        cparam.defect_sublattices,
-        cparam.num_defects,
-        cparam.supercell,
-        cparam.constraint_func,
-    )
-    spinel_config.shuffle()
-    return spinel_config
+# For backward compatibility
+if __version__ < "3":
+    model = Model
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/map2perflat.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/map2perflat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-# from mpi4py import MPI
+from __future__ import annotations
+
 import numpy as np
-from typing import Dict
 from pymatgen.core import Structure
+# pymatgen 2019.12.22 does not have SpeciesLike
+# from pymatgen.util.typing import SpeciesLike
+
 from abics.applications.latgas_abinitio_interface.naive_matcher import naive_mapping
 
 
 def map2perflat(
-    perf_st: Structure, st: Structure, vac_spaceholder: Dict[str, str] = {}
+    perf_st: Structure, st: Structure,
+    vac_spaceholder = {} #: dict[SpeciesLike, SpeciesLike] = {}
 ) -> Structure:
     """
 
     Arguments
     =========
     perf_st: Structure
         reference structure
@@ -22,15 +26,15 @@
         - value
             - virtual specy implying vacancy of 'A'
 
     """
     perf_st = perf_st.copy()
     N = perf_st.num_sites
     seldyn = np.array(
-        perf_st.site_properties.get("seldyn", np.ones((N, 3))), dtype=np.float
+        perf_st.site_properties.get("seldyn", np.ones((N, 3))), dtype=np.float64
     )
     perf_st.replace_species(vac_spaceholder)
     mapping = naive_mapping(st, perf_st)
     for i, j in enumerate(mapping):
         perf_st.replace(j, st[i].species_string, properties={"seldyn": seldyn[j]})
     perf_st.sort(key=lambda site: site.species_string)
     return perf_st
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/naive_matcher.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/naive_matcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import List
+from __future__ import annotations
 
 import numpy as np
 from pymatgen.core import Structure
 
 
-def naive_mapping(st0: Structure, st1: Structure) -> List[int]:
+def naive_mapping(st0: Structure, st1: Structure) -> list[int]:
     """
 
     Arguments
     =========
     st0: Structure
     st1: Structure
 
     Returns
     =======
-    mapping: List[int]
+    mapping: list[int]
         mapping atoms from st0 to st1.
         st0[i] corresponds to st1[mapping[i]]
     """
     coords0 = st0.frac_coords
     coords1 = st1.frac_coords
     D = st1.lattice.get_all_distances(coords0, coords1)
     rows = D.min(axis=1).argsort()
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/openmx.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/openmx.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
-from .base_solver import SolverBase
+from __future__ import annotations
+
 from collections import namedtuple
-import numpy as np
 import os
-import scipy.constants as spc
 import subprocess
+
+import numpy as np
+import scipy.constants as spc
+
 from pymatgen.core import Structure
 
+from .base_solver import SolverBase, register_solver
+from .params import ALParams, DFTParams
+
 hartree2eV = spc.value("Hartree energy in eV")
 Bohr2AA = spc.value("Bohr radius") * 1e10
 
 
 class OpenMXInputFile(dict):
     """ OpenMX Input
 
@@ -253,15 +259,15 @@
             try:
                 os.makedirs(output_dir)
             except:
                 pass
             output_file = os.path.join(
                 output_dir, "{}.dat".format(self.base_openmx_input["System.Name"][0])
             )
-            self.base_openmx_input['System.CurrrentDirectory'] = [output_dir + '/']
+            self.base_openmx_input["System.CurrrentDirectory"] = [output_dir + "/"]
             with open(output_file, "w") as f:
                 for key, values in self.base_openmx_input.items():
                     if key in self.base_openmx_input.vec_list:
                         print_stamp = "<{}\n".format(key)
                         for value_list in values:
                             for value in value_list:
                                 print_stamp += " {}".format(value)
@@ -390,7 +396,15 @@
                     positions.append([float(s) for s in line[1:4]])
             structure = Structure(A, species, positions, coords_are_cartesian=True)
             Phys = namedtuple("PhysValues", ("energy", "structure"))
             return Phys(np.float64(Utot), structure)
 
     def solver_run_schemes(self):
         return ("mpi_spawn_ready", "mpi_spawn_wrapper")
+
+    # -- factory
+    @classmethod
+    def create(cls, params: ALParams | DFTParams):
+        path = params.path
+        return cls(path)
+
+register_solver("openmx", OpenMXSolver)
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/params.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/params.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         self.solver = ""
         self.path = ""
         self.perturb = 0.0
         self.solver_run_scheme = ""
         self.properties = {}
         self.ignore_species = None
         self.constraint_module = None
+        self.function_module = None
         self.ensemble = False
         self.par_ensemble = False
         self.use_tmpdir = False
 
     @classmethod
     def from_dict(cls, d):
         """
@@ -52,22 +53,25 @@
         base_input_dir = d.get("base_input_dir", ["./baseinput"])
         if isinstance(base_input_dir, str):
             base_input_dir = [base_input_dir]
         params.base_input_dir = base_input_dir = list(
             map(lambda x: expand_path(x, os.getcwd()), base_input_dir)
         )
         params.solver = d["type"]
+        params.solver_run_scheme = d.get("run_scheme", "function")
 
-        #params.path = expand_path(d["path"], os.getcwd())
-        params.path = expand_cmd_path(d["path"])
+        if params.solver_run_scheme != "function":
+            params.path = expand_cmd_path(d["path"])
+        else:
+            params.path = ""
 
         params.perturb = d.get("perturb", 0.1)
-        params.solver_run_scheme = d.get("run_scheme", "mpi_spawn_ready")
         params.ignore_species = d.get("ignore_species", None)
         params.constraint_module = d.get("constraint_module", None)
+        params.function_module = d.get("function", None)
         params.ensemble = d.get("ensemble", False)
         params.par_ensemble = d.get("par_ensemble", False)
         params.use_tmpdir = d.get("use_tmpdir", True)
         params.properties = d
 
         return params
 
@@ -98,14 +102,15 @@
         self.solver = ""
         self.path = ""
         self.perturb = 0.0
         self.solver_run_scheme = ""
         self.properties = {}
         self.ignore_species = None
         self.constraint_module = None
+        self.function_module = None
         self.only_input = False
         self.vac_space_holder = []
 
     @classmethod
     def from_dict(cls, d):
         """
         Read information from dictionary
@@ -129,17 +134,23 @@
         )
         params.solver = d["type"]
 
         # the current version of abics_mlref does not invoke solver
         # params.path = expand_path(d["path"], os.getcwd())
 
         params.perturb = d.get("perturb", 0.1)
-        params.solver_run_scheme = d.get("run_scheme", "mpi_spawn_ready")
+        params.solver_run_scheme = d.get("run_scheme", "function")
+        if params.solver_run_scheme != "function":
+            params.path = expand_cmd_path(d["path"])
+        else:
+            params.path = ""
+
         params.ignore_species = d.get("ignore_species", None)
         params.constraint_module = d.get("constraint_module", None)
+        params.function_module = d.get("function", None)
         params.only_input = d.get("only_input", False)
         params.vac_space_holder = d.get("vac_convert", [])
 
         params.properties = d
 
         return params
 
@@ -169,14 +180,15 @@
         self.solver = ""
         self.path = ""
         self.solver_run_scheme = ""
         self.ignore_species = None
         self.properties = {}
         self.exe_command = []
         self.vac_map = []
+        self.previous_dir = []
 
     @classmethod
     def from_dict(cls, d):
         """
         Read information from dictionary
 
         Parameters
@@ -200,14 +212,17 @@
         exe_command = d["exe_command"]
         if isinstance(exe_command, str):
             exe_command = [exe_command]
         params.exe_command = exe_command
         params.solver_run_scheme = d.get("run_scheme", "subprocess")
         params.ignore_species = d.get("ignore_species", None)
         params.vac_map = d.get("vac_map", [])
+        params.previous_dir = d.get("previous_dirs", [])
+        if isinstance(params.previous_dir, str):
+            params.previous_dir = [params.previous_dir]
 
         params.properties = d
 
         return params
 
     @classmethod
     def from_toml(cls, f):
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/qe.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/qe.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,29 @@
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
 """
 To deal with QuantumESPRESSO
 
 """
 
+from __future__ import annotations
+
 from collections import namedtuple
 import xml.etree.ElementTree as ET
 import operator
 import os
 import os.path
 
 import numpy as np
 import scipy.constants as spc
 from pymatgen.core import Structure
 from qe_tools.parsers import PwInputFile
 
-from .base_solver import SolverBase
+from .params import ALParams, DFTParams
+from .base_solver import SolverBase, register_solver
 from ...util import expand_path
 from ...exception import InputError
 
 
 hartree2eV = spc.value("Hartree energy in eV")
 Bohr2AA = spc.value("Bohr radius") * 1e10
 
@@ -176,15 +179,16 @@
             if calculation not in ("scf", "relax"):
                 raise InputError("Sorry, {} is not yet supported".format(calculation))
             for name in ["ELECTRONS", "IONS", "CELL"]:
                 if name not in self.pwi.namelists:
                     self.pwi.namelists[name] = {}
             self.pwi.namelists["CONTROL"]["prefix"] = "pwscf"
             self.pwi.namelists["CONTROL"]["pseudo_dir"] = expand_path(
-                self.pwi.namelists["CONTROL"]["pseudo_dir"], base_input_dir
+                self.pwi.namelists["CONTROL"]["pseudo_dir"],
+                base_input_dir
                 # self.pwi.namelists["CONTROL"]["pseudo_dir"], os.getcwd()
             )
 
         def update_info_by_structure(self, structure):
             """
             Update information by atomic structure.
 
@@ -392,15 +396,19 @@
             -------
             phys : named_tuple("energy", "structure")
                 Total energy and atomic structure.
                 The energy is measured in the units of eV
                 and coordinates is measured in the units of Angstrom.
             """
             # Read results from files in output_dir and calculate values
-            tree = ET.parse(os.path.join(workdir, "pwscf.save", "data-file-schema.xml"))
+            try:
+                tree = ET.parse(os.path.join(workdir, "pwscf.save", "data-file-schema.xml"))
+            except Exception as e:
+                print("ERROR: QESolver.Output.get_results:", e)
+                exit(1)
             root = tree.getroot()
             A = np.zeros((3, 3))
             child = root.find("input").find("atomic_structure").find("cell")
             for i in range(3):
                 A[:, i] = list(map(float, child.find("a{}".format(i + 1)).text.split()))
             A *= Bohr2AA
 
@@ -425,7 +433,17 @@
         Returns
         -------
         schemes : tuple[str]
             Implemented runner schemes.
         """
         return "mpi_spawn"
 
+    # -- factory
+
+    @classmethod
+    def create(cls, params: ALParams | DFTParams):
+        path = params.path
+        parallel_level = params.properties.get("parallel_level", {})
+        return cls(path, parallel_level=parallel_level)
+
+
+register_solver("qe", QESolver)
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/run_base_mpi.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/run_base_mpi.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,341 +10,61 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
+from __future__ import annotations
+
+from typing import Type
+from abc import ABCMeta, abstractmethod
+
 import copy
 import os
 import shlex
 import subprocess
 import sys
 import time
 from timeit import default_timer as timer
 
 from mpi4py import MPI
 
 import numpy as np
 
+from abics import __version__
 from .model_setup import perturb_structure
 
 
-class runner(object):
-    """
-    Base class of runner (manager) of external solver program
-
-    Attributes
-    ----------
-    solver_name : str
-        Name of solver program
-    path_to_solver : str
-        Path to solver program
-    run : Any
-        Runner object
-    nprocs_per_solver : int
-        Number of processes which solver program uses
-    nthreads_per_proc : int
-        Number of threads which a solver process uses
-    comm : MPI.Comm
-        MPI Communicator
-    perturb : float
-        perturbation of atom position for structure optimization
-    base_solver_input : Solver.Input
-        Input manager
-    output : Solver.Output
-        Output manager
-    """
-
-    def __init__(
-        self,
-        base_input_dir,
-        Solver,
-        nprocs_per_solver,
-        comm,
-        perturb=0,
-        nthreads_per_proc=1,
-        solver_run_scheme="mpi_spawn_ready",
-        use_tmpdir=False,
-    ):
-        """
-        Parameters
-        -----------
-        base_input_dir : str
-            Path to the directory including input file templates
-        Solver : SolverBase
-            Solver
-        nprocs_per_solver : int
-            Number of processes which one solver program uses
-        comm : MPI.Comm
-            MPI Communicator
-        perturb : float, default 0.0
-            Perturbation of atom position
-        nthreads_per_proc : int, default 1
-            Number of threads which one solver process uses
-        solver_run_scheme : str, default "mpi_spawn_ready"
-            Scheme how to invoke a solver program
-        use_tmpdir : bool, default False
-            Whether to use temporary directory for solver run
-
-        Raises
-        ------
-        ValueError
-            Raises ValueError if unknown `solver_run_scheme` is passed
-        """
-        self.solver_name = Solver.name()
-        self.path_to_solver = Solver.path_to_solver
-        self.base_solver_input = Solver.input
-        self.base_solver_input.from_directory(base_input_dir)
-        self.nprocs_per_solver = nprocs_per_solver
-        self.nthreads_per_proc = nthreads_per_proc
-        self.output = Solver.output
-        self.comm = comm
-        self.use_tmpdir = use_tmpdir
-
-        if self.use_tmpdir:
-            import tempfile
-            self.tmpdir = tempfile.TemporaryDirectory()
-        #    import shutil
-        #    shutil.copy(self.path_to_solver, self.tmpdir.name)
-        #    self.path_to_solver = os.path.join(self.tmpdir.name, os.path.basename(self.path_to_solver))
-        if solver_run_scheme not in Solver.solver_run_schemes():
-            print(
-                "{scheme} not implemented for {solver}".format(
-                    scheme=solver_run_scheme, solver=Solver.name()
-                )
-            )
-            sys.exit(1)
-        if solver_run_scheme == "mpi_spawn_ready":
-            self.run = run_mpispawn_ready(
-                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
-            )
-        elif solver_run_scheme == "mpi_spawn":
-            self.run = run_mpispawn(
-                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
-            )
-        elif solver_run_scheme == "mpi_spawn_wrapper":
-            self.run = run_mpispawn_wrapper(
-                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
-            )
-        elif solver_run_scheme == "subprocess":
-            self.run = run_subprocess(
-                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
-            )
-        elif solver_run_scheme == "function":
-            self.run = run_function(
-                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
-            )
-        else:
-            msg = "Unknown scheme: {}".format(solver_run_scheme)
-            raise ValueError(msg)
-        self.perturb = perturb
-
-    def submit(self, structure, output_dir):
+class Run(metaclass=ABCMeta):
+    @abstractmethod
+    def submit(self, solver_name, solverinput, output_dir, rerun=0) -> int:
         """
-        Run a solver program and return results
+        Run solver
 
         Parameters
         ----------
-        structure : pymatgen.Structure
-            Structure of compounds
+        solver_name : str
+            Name of solver (e.g., VASP)
+        solverinput : Solver.Input
+            Input manager
         output_dir : str
-            Name of directory where solver program saves output files
+            Path to directory where a solver saves output
+        rerun : int, default = 2
+            How many times to restart solver on failed
 
         Returns
         -------
-        energy : float
-            Total energy
-        structure : pymatgen.Structure
-            Structure of compounds after optimization
-        """
-        if self.perturb:
-            perturb_structure(structure, self.perturb)
-        solverinput = self.base_solver_input
-        solverinput.update_info_by_structure(structure)
-        if self.use_tmpdir:
-            if output_dir[0] == "/":
-                output_dir = output_dir[1:]
-            output_dir = os.path.join(self.tmpdir.name, output_dir)
-        self.run.submit(self.solver_name, solverinput, output_dir)
-        results = self.output.get_results(output_dir)
-        return np.float64(results.energy), results.structure
-
-
-class runner_multistep(object):
-    """
-    Sequential runner
-
-    Attributes
-    ----------
-    runners : list[runner]
-        Runners
-    """
-
-    def __init__(
-        self,
-        base_input_dirs,
-        Solver,
-        runner,
-        nprocs_per_solver,
-        comm,
-        perturb=0,
-        nthreads_per_proc=1,
-        solver_run_scheme="mpi_spawn_ready",
-        use_tmpdir=False,
-    ):
-        """
-        Parameters
-        ----------
-        base_input_dirs : list[str]
-            List of paths to directories including base input files
-        Solver : SolverBase
-            Solver
-        nprocs_per_solver : int
-            Number of processes which one solver program uses
-        comm : MPI.Comm
-            MPI Communicator
-        perturb : float, default 0.0
-            Perturbation of atom position
-        nthreads_per_proc : int, default 1
-            Number of threads which one solver process uses
-        solver_run_scheme : str, default "mpi_spawn_ready"
-            Scheme how to invoke a solver program
-        use_tmpdir : bool, default False
-            Whether to use temporary directory for solver run
-        """
-
-        self.runners = []
-        assert len(base_input_dirs) > 1
-        self.runners.append(
-            runner(
-                base_input_dirs[0],
-                copy.deepcopy(Solver),
-                nprocs_per_solver,
-                comm,
-                perturb,
-                nthreads_per_proc,
-                solver_run_scheme,
-                use_tmpdir,
-            )
-        )
-        for i in range(1, len(base_input_dirs)):
-            self.runners.append(
-                runner(
-                    base_input_dirs[i],
-                    copy.deepcopy(Solver),
-                    nprocs_per_solver,
-                    comm,
-                    perturb=0,
-                    nthreads_per_proc=nthreads_per_proc,
-                    solver_run_scheme=solver_run_scheme,
-                    use_tmpdir=use_tmpdir,
-                )
-            )
-
-    def submit(self, structure, output_dir):
-        site_properties = structure.site_properties
-        energy, newstructure = self.runners[0].submit(structure, output_dir)
-        newstructure = newstructure.copy(site_properties)
-        for i in range(1, len(self.runners)):
-            energy, newstructure = self.runners[i].submit(newstructure, output_dir)
-            newstructure = newstructure.copy(site_properties)
-        return energy, newstructure
-
-class runner_ensemble(object):
-    """
-    Ensemble runner
-
-    Attributes
-    ----------
-    runners : list[runner]
-        Runners
-    """
-
-    def __init__(
-        self,
-        base_input_dirs,
-        Solver,
-        runner,
-        nprocs_per_solver,
-        comm,
-        perturb=0,
-        nthreads_per_proc=1,
-        solver_run_scheme="mpi_spawn_ready",
-        use_tmpdir=False,
-    ):
-        """
-        Parameters
-        ----------
-        base_input_dirs : list[str]
-            List of paths to directories including base input files
-        Solver : SolverBase
-            Solver
-        nprocs_per_solver : int
-            Number of processes which one solver program uses
-        comm : MPI.Comm
-            MPI Communicator
-        perturb : float, default 0.0
-            Perturbation of atom position
-        nthreads_per_proc : int, default 1
-            Number of threads which one solver process uses
-        solver_run_scheme : str, default "mpi_spawn_ready"
-            Scheme how to invoke a solver program
-        use_tmpdir : bool, default False
-            Whether to use temporary directory for solver run
+        status : int
+            Always returns 0
         """
+        ...
 
-        self.runners = []
-        assert len(base_input_dirs) > 1
-        self.runners.append(
-            runner(
-                base_input_dirs[0],
-                copy.deepcopy(Solver),
-                nprocs_per_solver,
-                comm,
-                perturb,
-                nthreads_per_proc,
-                solver_run_scheme,
-                use_tmpdir=use_tmpdir,
-            )
-        )
-        for i in range(1, len(base_input_dirs)):
-            self.runners.append(
-                runner(
-                    base_input_dirs[i],
-                    copy.deepcopy(Solver),
-                    nprocs_per_solver,
-                    comm,
-                    perturb=0,
-                    nthreads_per_proc=nthreads_per_proc,
-                    solver_run_scheme=solver_run_scheme,
-                    use_tmpdir=use_tmpdir,
-                )
-            )
-        self.comm = comm
-
-    def submit(self, structure, output_dir):
-        
-        npar = self.comm.Get_size()
-        if npar > 1:
-            assert(npar == len(self.runners))
-            myrank = self.comm.Get_rank()
-            energy, _ = self.runners[myrank].submit(structure, os.path.join(output_dir,"ensemble{}".format(myrank)))
-            energies = self.comm.allgather(energy)
-        else:
-            energies = []
-            for i in range(len(self.runners)):
-                energy, _ = self.runners[i].submit(structure, os.path.join(output_dir,"ensemble{}".format(i)))
-                energies.append(energy)
-
-        return np.mean(energies), structure
 
-
-
-class run_mpispawn:
+class RunMpispawn(Run):
     """
     Invoker via mpi_comm_spawn
 
     Attributes
     ----------
     path_to_solver : str
         Path to solver program
@@ -401,54 +121,23 @@
 
         Returns
         -------
         status : int
             Always returns 0
         """
         solverinput.write_input(output_dir)
-
-        # Barrier so that spawn is atomic between processes.
-        # This is to make sure that vasp processes are spawned one by one according to
-        # MPI policy (hopefully on adjacent nodes)
-        # (might be MPI implementation dependent...)
-
-        # for i in range(self.commsize):
-        #    self.comm.Barrier()
-        #    if i == self.commrank:
-        failed_dir = []
         cl_argslist = self.comm.gather(
             solverinput.cl_args(self.nprocs, self.nthreads, output_dir), root=0
         )
         solverrundirs = self.comm.gather(output_dir, root=0)
 
-        # checkfilename = "abacus_solver_finished"
-
         if self.commrank == 0:
             for rundir in solverrundirs:
                 solverinput.cleanup(rundir)
 
-            # wrappers = [
-            #     "rm -f {checkfile}; {solvername} {cl_args}; echo $? > {checkfile}".format(
-            #         checkfile=shlex.quote(
-            #             os.path.join(rundir, checkfilename)
-            #         ),
-            #         solvername=self.path_to_solver,
-            #         cl_args=" ".join(map(shlex.quote, cl_args)),
-            #     )
-            #     for cl_args in cl_argslist
-            # ]
-            #
-            # start = timer()
-            # commspawn = [
-            #     MPI.COMM_SELF.Spawn(
-            #         os.getenv('SHELL'), args=["-c", wrapper], maxprocs=self.nprocs
-            #     )
-            #     for wrapper in wrappers
-            # ]
-
             start = timer()
             commspawn = [
                 MPI.COMM_SELF.Spawn(
                     self.path_to_solver, args=cl_args, maxprocs=self.nprocs
                 )
                 for cl_args in cl_argslist
             ]
@@ -466,35 +155,19 @@
             print(
                 "rank ",
                 self.worldrank,
                 " took ",
                 end - start,
                 " for " + solver_name + "execution",
             )
-
-            # if len(failed_dir) != 0:
-            #     print(
-            #         solver_name + " failed in directories: \n " + "\n".join(failed_dir)
-            #     )
-            #     sys.stdout.flush()
-            #     if rerun == 0:
-            #         MPI.COMM_WORLD.Abort()
         self.comm.Barrier()
-
-        # Rerun if Solver failed
-        # failed_dir = self.comm.bcast(failed_dir, root=0)
-        # if len(failed_dir) != 0:
-        #     solverinput.update_info_from_files(output_dir, rerun)
-        #     rerun -= 1
-        #     self.submit(solverinput, output_dir, rerun)
-
         return 0
 
 
-class run_mpispawn_ready:
+class RunMpispawnReady(Run):
     """
     Invoker via mpi_comm_spawn for solvers which is MPI_Comm_spawn-ready
 
     Attributes
     ----------
     path_to_solver : str
         Path to solver program
@@ -634,15 +307,15 @@
         #        commspawn.Bcast([sendbuffer, 255, MPI.CHAR], root=MPI.ROOT)
         # commspawn.Barrier()
         # commspawn.Disconnect()
         # os.chdir(cwd)
         return 0
 
 
-class run_mpispawn_wrapper:
+class RunMpispawnWrapper(Run):
     """
     Invoker via mpi_comm_spawn
 
     Attributes
     ----------
     path_to_solver : str
         Path to solver program
@@ -771,15 +444,15 @@
         #     solverinput.update_info_from_files(output_dir, rerun)
         #     rerun -= 1
         #     self.submit(solverinput, output_dir, rerun)
 
         return 0
 
 
-class run_subprocess:
+class RunSubprocess(Run):
     """
     Invoker via subprocess
 
     Attributes
     ----------
     path_to_solver : str
         Path to solver program
@@ -852,15 +525,15 @@
         if to_rerun:
             self.submit(solver_name, solverinput, output_dir, rerun - 1)
 
         os.chdir(cwd)
         return 0
 
 
-class run_function:
+class RunFunction(Run):
     """
     Invoker via function call
 
     Attributes
     ----------
     path_to_solver : str
         function name
@@ -911,21 +584,350 @@
             Raises RuntimeError when solver failed.
         """
         solverinput.write_input(output_dir=output_dir)
         cwd = os.getcwd()
         os.chdir(output_dir)
         args = solverinput.cl_args(self.nprocs, self.nthreads, output_dir)
         to_rerun = False
-        # print(' '.join(command))
         with open(os.path.join(output_dir, "stdout"), "w") as fi:
             try:
                 self.path_to_solver(fi, *args)
             except RuntimeError as e:
                 if rerun > 0:
                     to_rerun = True
                 else:
                     raise
         if to_rerun:
             self.submit(solver_name, solverinput, output_dir, rerun - 1)
 
         os.chdir(cwd)
         return 0
+
+
+## Runners ##################################
+class Runner:
+    """
+    Base class of runner (manager) of external solver program
+
+    Attributes
+    ----------
+    solver_name : str
+        Name of solver program
+    path_to_solver : str
+        Path to solver program
+    run : Any
+        Runner object
+    nprocs_per_solver : int
+        Number of processes which solver program uses
+    nthreads_per_proc : int
+        Number of threads which a solver process uses
+    comm : MPI.Comm
+        MPI Communicator
+    perturb : float
+        perturbation of atom position for structure optimization
+    base_solver_input : Solver.Input
+        Input manager
+    output : Solver.Output
+        Output manager
+    """
+
+    run: Run
+
+    def __init__(
+        self,
+        base_input_dir,
+        Solver,
+        nprocs_per_solver,
+        comm,
+        perturb=0.0,
+        nthreads_per_proc=1,
+        solver_run_scheme="mpi_spawn_ready",
+        use_tmpdir=False,
+    ):
+        """
+        Parameters
+        -----------
+        base_input_dir : str
+            Path to the directory including input file templates
+        Solver : SolverBase
+            Solver
+        nprocs_per_solver : int
+            Number of processes which one solver program uses
+        comm : MPI.Comm
+            MPI Communicator
+        perturb : float, default 0.0
+            Perturbation of atom position
+        nthreads_per_proc : int, default 1
+            Number of threads which one solver process uses
+        solver_run_scheme : str, default "mpi_spawn_ready"
+            Scheme how to invoke a solver program
+        use_tmpdir : bool, default False
+            Whether to use temporary directory for solver run
+
+        Raises
+        ------
+        ValueError
+            Raises ValueError if unknown `solver_run_scheme` is passed
+        """
+        self.solver_name = Solver.name()
+        self.path_to_solver = Solver.path_to_solver
+        self.base_solver_input = Solver.input
+        self.base_solver_input.from_directory(base_input_dir)
+        self.nprocs_per_solver = nprocs_per_solver
+        self.nthreads_per_proc = nthreads_per_proc
+        self.output = Solver.output
+        self.comm = comm
+        self.use_tmpdir = use_tmpdir
+
+        if self.use_tmpdir:
+            import tempfile
+
+            self.tmpdir = tempfile.TemporaryDirectory()
+        #    import shutil
+        #    shutil.copy(self.path_to_solver, self.tmpdir.name)
+        #    self.path_to_solver = os.path.join(self.tmpdir.name, os.path.basename(self.path_to_solver))
+        if solver_run_scheme not in Solver.solver_run_schemes():
+            print(
+                "{scheme} not implemented for {solver}".format(
+                    scheme=solver_run_scheme, solver=Solver.name()
+                )
+            )
+            sys.exit(1)
+        if solver_run_scheme == "mpi_spawn_ready":
+            self.run = RunMpispawnReady(
+                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
+            )
+        elif solver_run_scheme == "mpi_spawn":
+            self.run = RunMpispawn(
+                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
+            )
+        elif solver_run_scheme == "mpi_spawn_wrapper":
+            self.run = RunMpispawnWrapper(
+                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
+            )
+        elif solver_run_scheme == "subprocess":
+            self.run = RunSubprocess(
+                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
+            )
+        elif solver_run_scheme == "function":
+            self.run = RunFunction(
+                self.path_to_solver, nprocs_per_solver, nthreads_per_proc, comm
+            )
+        else:
+            msg = "Unknown scheme: {}".format(solver_run_scheme)
+            raise ValueError(msg)
+        self.perturb = perturb
+
+    def submit(self, structure, output_dir):
+        """
+        Run a solver program and return results
+
+        Parameters
+        ----------
+        structure : pymatgen.Structure
+            Structure of compounds
+        output_dir : str
+            Name of directory where solver program saves output files
+
+        Returns
+        -------
+        energy : float
+            Total energy
+        structure : pymatgen.Structure
+            Structure of compounds after optimization
+        """
+        if self.perturb:
+            perturb_structure(structure, self.perturb)
+        solverinput = self.base_solver_input
+        solverinput.update_info_by_structure(structure)
+        if self.use_tmpdir:
+            if output_dir[0] == "/":
+                output_dir = output_dir[1:]
+            output_dir = os.path.join(self.tmpdir.name, output_dir)
+        self.run.submit(self.solver_name, solverinput, output_dir)
+        results = self.output.get_results(output_dir)
+        return float(results.energy), results.structure
+
+
+class RunnerMultistep:
+    """
+    Sequential runner
+
+    Attributes
+    ----------
+    runners : list[Runner]
+        Runners
+    """
+
+    def __init__(
+        self,
+        base_input_dirs,
+        Solvers,
+        runner: Type[Runner],
+        nprocs_per_solver,
+        comm,
+        perturb=0.0,
+        nthreads_per_proc=1,
+        solver_run_scheme="mpi_spawn_ready",
+        use_tmpdir=False,
+    ):
+        """
+        Parameters
+        ----------
+        base_input_dirs : list[str]
+            List of paths to directories including base input files
+        Solver : SolverBase
+            Solver
+        nprocs_per_solver : int
+            Number of processes which one solver program uses
+        comm : MPI.Comm
+            MPI Communicator
+        perturb : float, default 0.0
+            Perturbation of atom position
+        nthreads_per_proc : int, default 1
+            Number of threads which one solver process uses
+        solver_run_scheme : str, default "mpi_spawn_ready"
+            Scheme how to invoke a solver program
+        use_tmpdir : bool, default False
+            Whether to use temporary directory for solver run
+        """
+
+        self.runners = []
+        assert len(base_input_dirs) > 1
+        self.runners.append(
+            runner(
+                base_input_dirs[0],
+                Solvers[0],
+                nprocs_per_solver,
+                comm,
+                perturb,
+                nthreads_per_proc,
+                solver_run_scheme,
+                use_tmpdir,
+            )
+        )
+        for i in range(1, len(base_input_dirs)):
+            self.runners.append(
+                runner(
+                    base_input_dirs[i],
+                    Solvers[i],
+                    nprocs_per_solver,
+                    comm,
+                    perturb=0,
+                    nthreads_per_proc=nthreads_per_proc,
+                    solver_run_scheme=solver_run_scheme,
+                    use_tmpdir=use_tmpdir,
+                )
+            )
+
+    def submit(self, structure, output_dir):
+        site_properties = structure.site_properties
+        energy, newstructure = self.runners[0].submit(structure, output_dir)
+        newstructure = newstructure.copy(site_properties)
+        for i in range(1, len(self.runners)):
+            energy, newstructure = self.runners[i].submit(newstructure, output_dir)
+            newstructure = newstructure.copy(site_properties)
+        return energy, newstructure
+
+
+class RunnerEnsemble:
+    """
+    Ensemble runner
+
+    Attributes
+    ----------
+    runners : list[Runner]
+        Runners
+    """
+
+    def __init__(
+        self,
+        base_input_dirs,
+        Solvers,
+        runner: Type[Runner],
+        nprocs_per_solver,
+        comm,
+        perturb=0.0,
+        nthreads_per_proc=1,
+        solver_run_scheme="mpi_spawn_ready",
+        use_tmpdir=False,
+    ):
+        """
+        Parameters
+        ----------
+        base_input_dirs : list[str]
+            List of paths to directories including base input files
+        Solvers : list[SolverBase]
+            list of Solvers
+        nprocs_per_solver : int
+            Number of processes which one solver program uses
+        comm : MPI.Comm
+            MPI Communicator
+        perturb : float, default 0.0
+            Perturbation of atom position
+        nthreads_per_proc : int, default 1
+            Number of threads which one solver process uses
+        solver_run_scheme : str, default "mpi_spawn_ready"
+            Scheme how to invoke a solver program
+        use_tmpdir : bool, default False
+            Whether to use temporary directory for solver run
+        """
+
+        self.runners = []
+        assert len(base_input_dirs) > 1
+        self.runners.append(
+            runner(
+                base_input_dirs[0],
+                Solvers[0],
+                nprocs_per_solver,
+                comm,
+                perturb,
+                nthreads_per_proc,
+                solver_run_scheme,
+                use_tmpdir=use_tmpdir,
+            )
+        )
+        for i in range(1, len(base_input_dirs)):
+            self.runners.append(
+                runner(
+                    base_input_dirs[i],
+                    Solvers[i],
+                    nprocs_per_solver,
+                    comm,
+                    perturb=0,
+                    nthreads_per_proc=nthreads_per_proc,
+                    solver_run_scheme=solver_run_scheme,
+                    use_tmpdir=use_tmpdir,
+                )
+            )
+        self.comm = comm
+
+    def submit(self, structure, output_dir):
+
+        npar = self.comm.Get_size()
+        if npar > 1:
+            assert npar == len(self.runners)
+            myrank = self.comm.Get_rank()
+            energy, structure_new = self.runners[myrank].submit(
+                structure, os.path.join(output_dir, "ensemble{}".format(myrank))
+            )
+            energies = self.comm.allgather(energy)
+        else:
+            energies = []
+            for i in range(len(self.runners)):
+                energy, structure_new = self.runners[i].submit(
+                    structure, os.path.join(output_dir, "ensemble{}".format(i))
+                )
+                energies.append(energy)
+
+        return np.mean(energies), structure_new
+
+
+if __version__ < "3":
+    runner = Runner
+    runner_multistep = RunnerMultistep
+    runner_ensemble = RunnerEnsemble
+    run_mpispawn = RunMpispawn
+    run_mpispawn_ready = RunMpispawnReady
+    run_mpispawn_wrapper = RunMpispawnWrapper
+    run_subprocess = RunSubprocess
+    run_function = RunFunction
```

### Comparing `abics-2.0.1/abics/applications/latgas_abinitio_interface/vasp.py` & `abics-2.1.0/abics/applications/latgas_abinitio_interface/vasp.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,28 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
 """
 To deal with VASP
 """
 
+from __future__ import annotations
 
-from .base_solver import SolverBase
+import os, os.path
+import time
 from collections import namedtuple
+
+import numpy as np
 from pymatgen.io.vasp.inputs import Poscar, VaspInput
 from pymatgen.io.vasp.outputs import Oszicar
 from pymatgen.core import Structure
-#from pymatgen.apps.borg.hive import SimpleVaspToComputedEntryDrone
-#from pymatgen.apps.borg.queen import BorgQueen
-import numpy as np
-import os, os.path
-import time
+
+from .params import ALParams, DFTParams
+from .base_solver import SolverBase, register_solver
+
 
 class VASPSolver(SolverBase):
     """
     VASP solver
 
     Attributes
     ----------
@@ -180,15 +183,15 @@
             return [workdir]
 
     class Output(object):
         """
         Output manager.
         """
 
-        #def __init__(self):
+        # def __init__(self):
         #    self.drone = SimpleVaspToComputedEntryDrone(inc_structure=True)
         #    self.queen = BorgQueen(self.drone)
 
         def get_results(self, workdir):
             """
             Get energy and structure obtained by the solver program.
 
@@ -217,19 +220,30 @@
                     break
                 elif counter > 10:
                     raise TimeoutError(
                         "VASP OSZICAR is older than INCAR and no update was seen for 1 minute. "
                         "If VASP was actually run, then this might be due to a very slow file system."
                     )
                 else:
-                    print("VASP OSZICAR is older than INCAR; waiting for file system update")
+                    print(
+                        "VASP OSZICAR is older than INCAR; waiting for file system update"
+                    )
                     counter += 1
                     time.sleep(10)
-                    
+
             energy = Oszicar(os.path.join(workdir, "OSZICAR")).final_energy
             structure = Structure.from_file(os.path.join(workdir, "CONTCAR"))
-            
 
             return Phys(np.float64(energy), structure)
 
     def solver_run_schemes(self):
         return ("mpi_spawn_ready",)
+
+    # -- factory
+
+    @classmethod
+    def create(cls, params: ALParams | DFTParams):
+        path = params.path
+        ignore_species = params.ignore_species
+        return cls(path, ignore_species)
+
+register_solver("vasp", VASPSolver)
```

### Comparing `abics-2.0.1/abics/exception.py` & `abics-2.1.0/abics/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     """Exception raised for errors in the input
 
     Attributes
     ----------
     message: str
         explanation
     """
-    def __init__(self, message):
+    def __init__(self, message: str):
         self.message = message
 
 
 class MatrixParseError(Error):
     """Exception raised for matrix parse errors
 
     Attributes
     ----------
     message: str
         explanation
     """
-    def __init__(self, message):
+    def __init__(self, message: str):
         self.message = message
```

### Comparing `abics-2.0.1/abics/replica_params.py` & `abics-2.1.0/abics/replica_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+from __future__ import annotations
+
+from typing import Any
+from collections.abc import MutableMapping
+
 class SamplerParams:
     """Parameter set for specifying sampling algorithm
 
     Attributes
     ----------
     sampler : str
         Sampler name
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.sampler = "RXMC"
 
     @classmethod
-    def from_dict(cls, d):
+    def from_dict(cls, d: MutableMapping[str, Any]) -> "SamplerParams":
         """
         Read information from dictionary
 
         Parameters
         ----------
         d: dict
             Dictionary including parameters for specifying sampling algorithm
@@ -28,15 +33,15 @@
         if "sampler" in d:
             d = d["sampler"]
         params = cls()
         params.sampler = d.get("sampler", "RXMC")
         return params
 
     @classmethod
-    def from_toml(cls, fname):
+    def from_toml(cls, fname: str) -> "SamplerParams":
         """
         Read information from toml file
 
         Parameters
         ----------
         f: str
             The name of input toml File
@@ -47,73 +52,14 @@
             self
         """
         import toml
 
         return cls.from_dict(toml.load(fname))
 
 
-# class TrainParams:
-#     """Parameter set for reference calculations in active learning run
-#
-#     Attributes
-#     ----------
-#     nreplicas : int
-#         The number of replicas
-#     nprocs_per_replica : int
-#         The number of processes which a replica uses
-#     """
-#
-#     def __init__(self):
-#         self.nreplicas = None
-#         self.nprocs_per_replica = 1
-#         self.seed = 0
-#
-#     @classmethod
-#     def from_dict(cls, d):
-#         """
-#         Read information from dictionary
-#
-#         Parameters
-#         ----------
-#         d: dict
-#             Dictionary including parameters for parallel random sampling
-#
-#         Returns
-#         -------
-#         params: DFTParams object
-#             self
-#         """
-#         if "replicaRef" in d:
-#             d = d["replicaRef"]
-#         params = cls()
-#         params.nreplicas = d["nreplicas"]
-#         params.nprocs_per_replica = d.get("nprocs_per_replica", 1)
-#         return params
-#
-#     @classmethod
-#     def from_toml(cls, fname):
-#         """
-#         Read information from toml file
-#
-#         Parameters
-#         ----------
-#         f: str
-#             The name of input toml File
-#
-#         Returns
-#         -------
-#         DFTParams: DFTParams object
-#             self
-#         """
-#         import toml
-#
-#         d = toml.load(fname)
-#         return cls.from_dict(d["train"])
-
-
 class ParallelRandomParams:
     """Parameter set for parallel random sampling
 
     Attributes
     ----------
     nreplicas : int
         The number of replicas
@@ -128,25 +74,25 @@
     reload : bool
         Whether to restart simulation or not
     seed : int
         The seed of the random number generator
         If 0, some random number is used (e.g., system time or some random noise).
     """
 
-    def __init__(self):
-        self.nreplicas = None
+    def __init__(self) -> None:
+        self.nreplicas = 1
         self.nprocs_per_replica = 1
         self.nsteps = None
         self.sample_frequency = 1
         self.print_frequency = 1
         self.reload = False
         self.seed = 0
 
     @classmethod
-    def from_dict(cls, d):
+    def from_dict(cls, d: MutableMapping[str, Any]) -> "ParallelRandomParams":
         """
         Read information from dictionary
 
         Parameters
         ----------
         d: dict
             Dictionary including parameters for parallel random sampling
@@ -165,15 +111,15 @@
         params.sample_frequency = d.get("sample_frequency", 1)
         params.print_frequency = d.get("print_frequency", 1)
         params.reload = d.get("reload", False)
         params.seed = d.get("seed", 0)
         return params
 
     @classmethod
-    def from_toml(cls, fname):
+    def from_toml(cls, fname: str) -> "ParallelRandomParams":
         """
         Read information from toml file
 
         Parameters
         ----------
         f: str
             The name of input toml File
@@ -184,15 +130,15 @@
             self
         """
         import toml
 
         return cls.from_dict(toml.load(fname))
 
 
-class ParalleMCParams:
+class ParallelMCParams:
     """Parameter set for embarrasingly parallel Monte Carlo
 
     Attributes
     ----------
     nreplicas : int
         The number of replicas
     nprocs_per_replica : int
@@ -210,27 +156,27 @@
     reload : bool
         Whether to restart simulation or not
     seed : int
         The seed of the random number generator
         If 0, some random number is used (e.g., system time or some random noise).
     """
 
-    def __init__(self):
-        self.nreplicas = None
+    def __init__(self) -> None:
+        self.nreplicas = -1
         self.nprocs_per_replica = 1
-        self.kTstart = None
-        self.kTend = None
-        self.nsteps = None
+        self.kTstart = -1.0
+        self.kTend = -1.0
+        self.nsteps = -1
         self.sample_frequency = 1
         self.print_frequency = 1
         self.reload = False
         self.seed = 0
 
     @classmethod
-    def from_dict(cls, d):
+    def from_dict(cls, d: MutableMapping[str, Any]) -> "ParallelMCParams":
         """
         Read information from dictionary
 
         Parameters
         ----------
         d: dict
             Dictionary including parameters for embarrassingly parallel Monte Carlo method
@@ -251,15 +197,15 @@
         params.sample_frequency = d.get("sample_frequency", 1)
         params.print_frequency = d.get("print_frequency", 1)
         params.reload = d.get("reload", False)
         params.seed = d.get("seed", 0)
         return params
 
     @classmethod
-    def from_toml(cls, fname):
+    def from_toml(cls, fname: str) -> "ParallelMCParams":
         """
         Read information from toml file
 
         Parameters
         ----------
         f: str
             The name of input toml File
@@ -298,28 +244,28 @@
     reload : bool
         Whether to restart simulation or not
     seed : int
         The seed of the random number generator
         If 0, some random number is used (e.g., system time or some random noise).
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.nreplicas = None
         self.nprocs_per_replica = 1
         self.kTstart = None
         self.kTend = None
         self.nsteps = None
         self.RXtrial_frequency = 1
         self.sample_frequency = 1
         self.print_frequency = 1
         self.reload = False
         self.seed = 0
 
     @classmethod
-    def from_dict(cls, d):
+    def from_dict(cls, d: MutableMapping[str, Any]) -> "RXParams":
         """
         Read information from dictionary
 
         Parameters
         ----------
         d: dict
             Dictionary including parameters for replica exchange Monte Carlo method
@@ -341,15 +287,15 @@
         params.sample_frequency = d.get("sample_frequency", 1)
         params.print_frequency = d.get("print_frequency", 1)
         params.reload = d.get("reload", False)
         params.seed = d.get("seed", 0)
         return params
 
     @classmethod
-    def from_toml(cls, fname):
+    def from_toml(cls, fname: str) -> "RXParams":
         """
         Read information from toml file
 
         Parameters
         ----------
         f: str
             The name of input toml File
```

### Comparing `abics-2.0.1/abics/scripts/abicsRXsepT.py` & `abics-2.1.0/abics/scripts/abicsRXsepT.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
 from mpi4py import MPI
+
 import shutil
 import os, sys
 import datetime
 import argparse
-from abics.mc_mpi import RXParams, RX_MPI_init
+
 import numpy as np
 import scipy.constants as constants
+import toml
+
+from abics.sampling.mc_mpi import RX_MPI_init
+from abics.sampling.rxmc import RXParams
 
 
 def main():
     # Input parser
     parser = argparse.ArgumentParser(
         description="Reorganize abICS RXMC results by temperature"
     )
@@ -33,47 +38,56 @@
     parser.add_argument("inputfi", help="toml input file used for abICS run")
 
     parser.add_argument(
         "skipsteps",
         nargs="?",
         type=int,
         default=0,
-        help="number of thermalization steps to skip in energy averaging." + " Default: 0",
+        help="number of thermalization steps to skip in energy averaging."
+        + " Default: 0",
     )
 
     args = parser.parse_args()
     inputfi = args.inputfi
     nskip = args.skipsteps
     rxparams = RXParams.from_toml(inputfi)
     nreplicas = rxparams.nreplicas
-    comm = RX_MPI_init(rxparams)
+    comm = RX_MPI_init(rxparams.nreplicas, rxparams.seed)
+
+    param = toml.load(inputfi)
+    solver_type = param["sampling"]["solver"]["type"]
 
     myreplica = comm.Get_rank()
 
     if myreplica == 0:
         if os.path.exists("Tseparate"):
             shutil.move("Tseparate", "Tseparate.bak.{}".format(datetime.datetime.now()))
         os.mkdir("Tseparate")
     comm.Barrier()
 
     # Separate structure files
     os.mkdir(os.path.join("Tseparate", str(myreplica)))
     Trank_hist = np.load(os.path.join(str(myreplica), "Trank_hist.npy"))
     os.chdir(str(myreplica))
     for j in range(len(Trank_hist)):
-        shutil.copy(
-            "structure.{}.vasp".format(j),
-            os.path.join(os.pardir, "Tseparate", str(Trank_hist[j])),
-        )
+        str_file = f"structure.{j}.vasp"
+        if os.path.exists(str_file):
+            shutil.copy(
+                str_file,
+                os.path.join(os.pardir, "Tseparate", str(Trank_hist[j])),
+            )
 
     # Separate energies
-    myreplica_energies = np.load("obs_save.npy")[:, 0]
+    myreplica_energies = np.load("obs_save.npy")
     for Tid in range(nreplicas):
-        T_energies = np.where(Trank_hist == Tid, myreplica_energies, 0)
-        T_energies_rcvbuf = np.zeros(T_energies.shape[0], "d")
+        mask = Trank_hist == Tid
+        if myreplica_energies.ndim == 2:
+            mask = np.repeat(mask.reshape(-1,1), myreplica_energies.shape[1], axis=1)
+        T_energies = np.where(mask, myreplica_energies, 0)
+        T_energies_rcvbuf = np.zeros(T_energies.shape, "d")
         comm.Reduce(
             [T_energies, MPI.DOUBLE],
             [T_energies_rcvbuf, MPI.DOUBLE],
             op=MPI.SUM,
             root=Tid,
         )
         if myreplica == Tid:
@@ -84,17 +98,28 @@
 
     comm.Barrier()
 
     if myreplica == 0:
         os.chdir(os.path.join(os.pardir, "Tseparate"))
         with open("energies_T.dat", "w") as fi:
             kTs = np.load(os.path.join(os.pardir, "kTs.npy"))
-            Ts = kTs / constants.value(u"Boltzmann constant in eV/K")
+            if solver_type != "potts":
+                Ts = kTs / constants.value("Boltzmann constant in eV/K")
+            else:
+                Ts = kTs
             for Tid in range(nreplicas):
-                energy_mean = np.mean(
-                    np.loadtxt(os.path.join(str(Tid), "energies.dat"))[nskip:]
-                )
-                fi.write("{}\t{}\n".format(Ts[Tid], energy_mean))
+                energies_data = np.loadtxt(os.path.join(str(Tid), "energies.dat"))
+                if energies_data.ndim == 1:
+                    energy_mean = [np.mean(energies_data[nskip:])]
+                else:
+                    energy_mean = np.mean(energies_data[nskip:,:],
+                                          axis = 0
+                    )
+
+                fi.write(f"{Ts[Tid]}")
+                for en in energy_mean:
+                    fi.write(f"\t{en}")
+                fi.write("\n")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `abics-2.0.1/abics/scripts/activelearn.py` & `abics-2.1.0/abics/scripts/activelearn.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,85 +10,62 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
-from mpi4py import MPI
+from typing import MutableMapping
 
 import sys
-import os, copy
+import os
 import glob
 import datetime
 
 import numpy as np
 
 from abics import __version__
 
-from abics.mc import RandomSampling
-
 from abics.mc_mpi import (
     RX_MPI_init,
     RefParams,
-    EmbarrassinglyParallelSampling,
 )
 from abics.applications.latgas_abinitio_interface import map2perflat
-from abics.applications.latgas_abinitio_interface import default_observer
 from abics.applications.latgas_abinitio_interface.model_setup import (
-    dft_latgas,
-    ObserverParams,
     perturb_structure,
 )
 from abics.applications.latgas_abinitio_interface.defect import (
     defect_config,
     DFTConfigParams,
 )
-from abics.applications.latgas_abinitio_interface.run_base_mpi import (
-    runner,
-    runner_multistep,
-)
-from abics.applications.latgas_abinitio_interface.vasp import VASPSolver
-from abics.applications.latgas_abinitio_interface.qe import QESolver
-from abics.applications.latgas_abinitio_interface.aenet import aenetSolver
-from abics.applications.latgas_abinitio_interface.openmx import OpenMXSolver
-from abics.applications.latgas_abinitio_interface.mocksolver import MockSolver
-from abics.applications.latgas_abinitio_interface.params import ALParams
+from abics.applications.latgas_abinitio_interface.base_solver import SolverBase, create_solver
+from abics.applications.latgas_abinitio_interface.params import ALParams, DFTParams
 
 from abics.util import exists_on_all_nodes
 from pymatgen.core import Structure
 
+import logging
+import abics.loggers as loggers
+
+logger = logging.getLogger("main")
 
-def main_impl(tomlfile):
-    rxparams = RefParams.from_toml(tomlfile)
+
+def main_impl(params_root: MutableMapping):
+    rxparams = RefParams.from_dict(params_root["mlref"])
     # nprocs_per_replica = rxparams.nprocs_per_replica
     # nreplicas = rxparams.nreplicas
     # nsteps = rxparams.nsteps
     # sample_frequency = rxparams.sample_frequency
     ndata = rxparams.ndata
-    comm = RX_MPI_init(rxparams)
-    alparams = ALParams.from_toml(tomlfile)
-    configparams = DFTConfigParams.from_toml(tomlfile)
-
-    if alparams.solver == "vasp":
-        solver = VASPSolver(alparams.path, alparams.ignore_species)
-    elif alparams.solver == "qe":
-        parallel_level = alparams.properties.get("parallel_level", {})
-        solver = QESolver(alparams.path, parallel_level=parallel_level)
-    elif alparams.solver == "aenet":
-        solver = aenetSolver(
-            alparams.path, alparams.ignore_species, alparams.solver_run_scheme
-        )
-    elif alparams.solver == "openmx":
-        solver = OpenMXSolver(alparams.path)
-    elif alparams.solver == "mock":
-        solver = MockSolver()
-    else:
-        print("unknown solver: {}".format(alparams.solver))
-        sys.exit(1)
+    comm = RX_MPI_init(rxparams.nreplicas, rxparams.seed)
+    alparams = ALParams.from_dict(params_root["mlref"]["solver"])
+    mcparams = DFTParams.from_dict(params_root["sampling"]["solver"])
+    configparams = DFTConfigParams.from_dict(params_root["config"])
+
+    solver: SolverBase = create_solver(alparams.solver, alparams)
 
     perturb = alparams.perturb
     solver_output = solver.output
     solver_input = solver.input
 
     myreplica = comm.Get_rank()
 
@@ -101,17 +78,15 @@
     if nextMC_index == 0:  # "MC0" does not exist
         # Random sampling!
         ndigits = len(str(ndata))
         fmtstr = "input{:0>" + str(ndigits) + "d}"
 
         if exists_on_all_nodes(comm, "AL0"):
             if exists_on_all_nodes(comm, "ALloop.progress"):
-                print(
-                    "It seems you've already run the first active learning step. You should train now."
-                )
+                logger.error("It seems you've already run the first active learning step. You should train now.")
                 sys.exit(1)
             os.chdir("AL0")
 
             # attempting post processing of ALed output
             if not exists_on_all_nodes(comm, "baseinput.progress"):  # 1st step
                 runstep = 0
 
@@ -124,45 +99,48 @@
                 finalrun = True
             else:
                 finalrun = False
                 solver_input.from_directory(alparams.base_input_dir[runstep + 1])
             energies = []
 
             # Preparing ignored species structure to add in postprocess
-            config = defect_config(configparams)
-            if alparams.ignore_species:
-                ignore_structure = config.dummy_structure()
-                remove_sp = filter(
-                    lambda sp: sp not in alparams.ignore_species,
-                    ignore_structure.symbol_set,
-                )
-                ignore_structure.remove_species(remove_sp)
-            rundir_list = []
+            #config = defect_config(configparams)
             
-            if myreplica == 0:
-                print(f"-Parsing {alparams.solver} results in AL0/*/input*/baseinput{runstep}...")
-                if finalrun:
-                    print(f"--This is the final {alparams.solver} calculation step for AL0")
-                else:
-                    print("--Input files for the next calculation step will be",
-                          f"---prepared in AL{nextMC_index}/*/input*/baseinput{runstep+1}",
-                          sep = os.linesep
-                    )
+            rundir_list = []
+
+            logger.info(f"-Parsing {alparams.solver} results in AL0/*/input*/baseinput{runstep}...")
+            if finalrun:
+                logger.info(f"--This is the final {alparams.solver} calculation step for AL0")
+            else:
+                logger.info("--Input files for the next calculation step will be")
+                logger.info(f"---prepared in AL{nextMC_index}/*/input*/baseinput{runstep+1}")
+
             for i in range(ndata):
                 energy, st = solver_output.get_results(
                     os.path.join(
                         str(myreplica), fmtstr.format(i), f"baseinput{runstep}"
                     )
                 )
                 if finalrun:
                     # energy_calculator may return the structure w/o ignored structure
                     if alparams.ignore_species:
+                        # Get original structure for calculating relaxation magnitude
+                        ignore_structure = Structure.from_file(
+                            os.path.join(str(myreplica),fmtstr.format(i), "initial.vasp")
+                        )
+                        remove_sp = filter(
+                            lambda sp: sp not in alparams.ignore_species,
+                            ignore_structure.symbol_set,
+                        )
+                        ignore_structure.remove_species(remove_sp)
+                    
                         for site in ignore_structure:
                             st.append(site.species_string, site.frac_coords)
 
+                    st.sort(key=lambda site: site.species_string)
                     st.to(
                         fmt="POSCAR",
                         filename=os.path.join(str(myreplica), f"structure.{i}.vasp"),
                     )
                     energies.append([energy])
                 else:
                     solver_input.update_info_by_structure(st)
@@ -188,192 +166,186 @@
                     for i in range(len(energies)):
                         energy = energies[i][0]
                         fi.write(f"NaN {energy} {i}\n")
                 os.chdir(rootdir)
                 comm.Barrier()
                 if myreplica == 0:
                     with open("ALloop.progress", "a") as fi:
-                        print("-Writing ALloop.progress")
+                        logger.info("-Writing ALloop.progress")
                         fi.write("AL0\n")
                         fi.flush()
                         os.fsync(fi.fileno())
                     now = datetime.datetime.now()
-                    print("--Done. Please run abics_train next.",
-                          f"Exiting normally on {now}.\n",
-                          sep = os.linesep)
+                    logger.info("--Done. Please run abics_train next.")
+                    logger.info(f"Exiting normally on {now}.\n")
                 sys.exit(0)
             else:
                 comm.Barrier()
                 if myreplica == 0:
                     with open("baseinput.progress", "a") as fi:
                         fi.write(str(runstep) + "\n")
                         fi.flush()
                         os.fsync(fi.fileno())
 
-                    print(f"-Finished preparing {alparams.solver} input in AL0/*/input*/baseinput{runstep+1}.",
-                          "--See rundirs.txt for a full list of the directories.", sep = os.linesep)
-                    print("-Please perform the calculations in those directories before running abics_mlref again.")
+                    logger.info(f"-Finished preparing {alparams.solver} input in AL0/*/input*/baseinput{runstep+1}.")
+                    logger.info("--See rundirs.txt for a full list of the directories.")
+                    logger.info("-Please perform the calculations in those directories before running abics_mlref again.")
                     now = datetime.datetime.now()
-                    print(f"Exiting normally on {now}.\n")
+                    logger.info(f"Exiting normally on {now}.\n")
                 sys.exit(0)
         else:
             # "AL0" nor "MC0" does not exist:
             # this should be the first time running this script
             if myreplica == 0:
-                print("-No preceding MC or AL runs exist. Preparing {} input by random sampling".format(alparams.solver))
-                print("--Input files will be prepared in AL0/*/input*/baseinput0")
+                logger.info("-No preceding MC or AL runs exist. Preparing {} input by random sampling".format(alparams.solver))
+                logger.info("--Input files will be prepared in AL0/*/input*/baseinput0")
 
-            configparams = DFTConfigParams.from_toml(tomlfile)
+            configparams = DFTConfigParams.from_dict(params_root["config"])
             config = defect_config(configparams)
             comm.Barrier()
             if myreplica == 0:
                 os.mkdir("AL0")
 
             # Wait until the new directory is visible from all ranks
             if not exists_on_all_nodes(comm, "AL0"):
-                print("Failed to create AL0 directory.")
+                logger.error("Failed to create AL0 directory.")
                 sys.exit(1)
 
             os.chdir("AL0")
             rundir_list = []
             solver_input = solver.input
             solver_input.from_directory(alparams.base_input_dir[0])
             for i in range(ndata):
-                config.shuffle()
-                perturb_structure(config.structure, perturb)
+                config.shuffle() # randomize config
                 config.structure.sort(key=lambda site: site.species_string)
+                structure0 = config.structure.copy()  
+                perturb_structure(config.structure, perturb)
                 solver_input.update_info_by_structure(config.structure)
                 inputfile = os.path.abspath(
                     os.path.join(str(myreplica), fmtstr.format(i), "baseinput0")
                 )
                 solver_input.write_input(inputfile)
                 rundir_list.append(inputfile)
+
+                # save structure before running through solver (contains ignored species)
+                structure0.to(
+                    fmt='POSCAR',
+                    filename=os.path.abspath(
+                        os.path.join(str(myreplica), fmtstr.format(i), "initial.vasp")
+                        ),
+                )
             rundir_list = comm.gather(rundir_list, root=0)
             if myreplica == 0:
                 rundir_list = [rundir for sublist in rundir_list for rundir in sublist]
                 with open(os.path.join(rootdir, "rundirs.txt"), "w") as fi:
                     fi.write("\n".join(rundir_list))
                     fi.write("\n")
                     fi.flush()
                     os.fsync(fi.fileno())
 
-                print(f"-Finished preparing {alparams.solver} input in AL0/*/input*/baseinput0.",
-                      "--See rundirs.txt for a full list of the directories.",
-                      sep = os.linesep)
-                print("--Please perform the calculations in those directories before running abics_mlref again.")
+                logger.info(f"-Finished preparing {alparams.solver} input in AL0/*/input*/baseinput0.")
+                logger.info("--See rundirs.txt for a full list of the directories.")
+                logger.info("--Please perform the calculations in those directories before running abics_mlref again.")
                 now = datetime.datetime.now()
-                print(f"Exiting normally on {now}.\n")
+                logger.info(f"Exiting normally on {now}.\n")
 
                 sys.exit(0)
 
     else:  # "MC*" exists
         # Active learning!
         MCdirname = f"MC{nextMC_index-1}"
         MCdir = os.path.join(os.getcwd(), MCdirname)
         nsamples = 0
         with open(os.path.join(MCdir, str(myreplica), "obs.dat")) as f:
-            for _ in f:
+            for line in f:
+                line = line.strip()
+                if line.startswith("#"):
+                    continue
                 nsamples += 1
         ndigits = len(str(nsamples))
         fmtstr = "input{:0>" + str(ndigits) + "d}"
         with open("ALloop.progress", "r") as fi:
             last_li = fi.readlines()[-1].strip()
         if last_li != MCdirname:
-            print("The last action:")
-            print(f"  expected: {MCdirname}")
-            print(f"  actual:   {last_li}")
-            print("You shouldn't run activelearn now.")
-            print("Either train (abics_train) or MC (abics_sampling) first.")
+            logger.error("The last action:")
+            logger.error(f"  expected: {MCdirname}")
+            logger.error(f"  actual:   {last_li}")
+            logger.error("You shouldn't run activelearn now.")
+            logger.error("Either train (abics_train) or MC (abics_sampling) first.")
             sys.exit(1)
         obs = np.load(os.path.join(MCdir, str(myreplica), "obs_save.npy"))
         energy_ref = obs[:, 0]
         ALstep = nextMC_index
         ALdir = os.path.join(os.getcwd(), f"AL{ALstep}", str(myreplica))
         config = defect_config(configparams)
-        perf_st = config.dummy_structure()
-        if alparams.ignore_species:
-            ignore_structure = perf_st.copy()
-            remove_sp = filter(
-                lambda sp: sp not in alparams.ignore_species, perf_st.symbol_set
-            )
-            ignore_structure.remove_species(remove_sp)
 
         if exists_on_all_nodes(comm, ALdir):  # We're going to read solver results
             os.chdir(ALdir)
 
             if not exists_on_all_nodes(
                 comm, os.path.join(os.path.pardir, "baseinput.progress")
             ):
                 # 1st runner step
                 runstep = 0
             else:
                 # 2nd or later runner step
                 with open(os.path.join(os.pardir, "baseinput.progress"), "r") as fi:
                     runstep = int(fi.readlines()[-1]) + 1
-                
+
             if runstep + 1 == len(alparams.base_input_dir):
                 # This is the last run for this AL step
                 finalrun = True
 
             else:
                 finalrun = False
                 solver_input.from_directory(alparams.base_input_dir[runstep + 1])
 
-            if myreplica == 0:
-                print(f"-Parsing {alparams.solver} results in AL{nextMC_index}/*/input*/baseinput{runstep}...")
-                if finalrun:
-                    print(f"--This is the final {alparams.solver} calculation step for AL{nextMC_index}")
-                else:
-                    print("--Input files for the next calculation step will be",
-                          f"---prepared in AL{nextMC_index}/*/input*/baseinput{runstep+1}",
-                          sep = os.linesep
-                    )
+            logger.info(f"-Parsing {alparams.solver} results in AL{nextMC_index}/*/input*/baseinput{runstep}...")
+            if finalrun:
+                logger.info(f"--This is the final {alparams.solver} calculation step for AL{nextMC_index}")
+            else:
+                logger.info("--Input files for the next calculation step will be")
+                logger.info(f"---prepared in AL{nextMC_index}/*/input*/baseinput{runstep+1}")
 
             energy_corrlist = []
             relax_max = []
             rundir_list = []
             sample_list = []
-            for f in glob.iglob(
-                os.path.join(ALdir, "input*")
-            ):
-                sample_list.append(int(os.path.basename(f).split("t")[1]))
+            for path in glob.iglob(os.path.join(ALdir, "input*")):
+                sample_list.append(int(os.path.basename(path).split("t")[1]))
             sample_list.sort()
             for i in sample_list:
                 energy, st_rel = solver_output.get_results(
                     os.path.join(fmtstr.format(i), f"baseinput{runstep}")
                 )
                 if finalrun:
                     # Get original structure for calculating relaxation magnitude
-                    # In st_in, used for aenet,
-                    # (i)  "Ignore species" are omitted and should be added.
-                    # (ii) "Vacancy element" is included and should be removed.
                     st_in = Structure.from_file(
-                        os.path.join(MCdir, str(myreplica), f"structure.{i}.vasp")
+                        os.path.join(fmtstr.format(i), "initial.vasp")
                     )
-
-                    # (i)
-                    st = map2perflat(perf_st, st_in)
-                    st.remove_species(["X"])
-                    # (ii)
-                    if alparams.vac_space_holder:
-                        st.remove_species(alparams.vac_space_holder)
-                    stbak = st.copy()
-
+                    
                     # energy_calculator may return the structure w/o ignored structure
+                    # so we need to add them
                     if alparams.ignore_species:
+                        # initial.vasp contains full structure with ignored atoms
+                        ignore_structure = st_in.copy()
+                        remove_sp = filter(
+                            lambda sp: sp not in alparams.ignore_species, ignore_structure.symbol_set
+                            )
+                        ignore_structure.remove_species(remove_sp)
                         for site in ignore_structure:
                             st_rel.append(site.species_string, site.frac_coords)
 
                     st_rel.to(fmt="POSCAR", filename=f"structure.{i}.vasp")
                     energy_corrlist.append([energy_ref[i], energy, i])
 
                     # Examine relaxation
                     dmax = 0
                     dmax_id = 0
-                    for j, site in enumerate(stbak):
+                    for j, site in enumerate(st_in):
                         d = site.distance(st_rel[j])
                         if d > dmax:
                             dmax = d
                             dmax_id = j
                     relax_max.append([dmax_id, dmax])
 
                 else:
@@ -389,106 +361,117 @@
                 with open(os.path.join(rootdir, "rundirs.txt"), "w") as fi:
                     fi.write("\n".join(rundir_list))
                     fi.write("\n")
                     fi.flush()
                     os.fsync(fi.fileno())
 
             if finalrun:
-                # np.savetxt("energy_corr.dat", energy_corrlist)
                 with open("energy_corr.dat", "w") as fi:
                     for i in range(len(energy_corrlist)):
                         ene_nn, ene_ref, step = energy_corrlist[i]
                         fi.write(f"{ene_nn} {ene_ref} {step}\n")
                 with open("relax_max.dat", "w") as fi:
                     for row in relax_max:
                         fi.write("{} \t {}\n".format(row[0], row[1]))
                 os.chdir(rootdir)
                 comm.Barrier()
                 if myreplica == 0:
                     with open("ALloop.progress", "a") as fi:
-                        print("-Writing ALloop.progress")
+                        logger.info("-Writing ALloop.progress")
                         fi.write("AL{}\n".format(ALstep))
                         fi.flush()
                         os.fsync(fi.fileno())
                     now = datetime.datetime.now()
-                    print("--Done. Please run abics_train next.",
-                          f"Exiting normally on {now}.\n",
-                          sep = os.linesep)
+                    logger.info("--Done. Please run abics_train next.")
+                    logger.info(f"Exiting normally on {now}.\n")
                 sys.exit(0)
             else:
                 comm.Barrier()
                 if myreplica == 0:
                     with open(
                         os.path.join(os.path.pardir, "baseinput.progress"), "a"
                     ) as fi:
                         fi.write(str(runstep) + "\n")
                         fi.flush()
                         os.fsync(fi.fileno())
-                    print(f"-Finished preparing {alparams.solver} input in AL{nextMC_index}/*/input*/baseinput{runstep+1}.",
-                          "--See rundirs.txt for a full list of the directories.", sep = os.linesep)
-                    print("--Please perform the calculations in those directories before running abics_mlref again.")
+                    logger.info(f"-Finished preparing {alparams.solver} input in AL{nextMC_index}/*/input*/baseinput{runstep+1}.")
+                    logger.info("--See rundirs.txt for a full list of the directories.")
+                    logger.info("--Please perform the calculations in those directories before running abics_mlref again.")
                     now = datetime.datetime.now()
-                    print(f"Exiting normally on {now}.\n")
+                    logger.info(f"Exiting normally on {now}.\n")
                 sys.exit(0)
 
         else:  # Create first input for this AL step
-            if myreplica == 0:
-                print(f"-This is the first run for AL{nextMC_index}")
-                print(f"--Configurations from MC{nextMC_index-1} will be converted to {alparams.solver} input")
+            logger.info(f"-This is the first run for AL{nextMC_index}")
+            logger.info(f"--Configurations from MC{nextMC_index-1} will be converted to {alparams.solver} input")
             os.makedirs(ALdir, exist_ok=False)
             solver_input.from_directory(alparams.base_input_dir[0])
             os.chdir(ALdir)
             sample_list = rxparams.sampling(nsamples)
             rundir_list = []
             for i in sample_list:
-                # In st_in, used for aenet,
-                # (i)  "Ignore species" are omitted and should be added.
-                # (ii) "Vacancy element" is included and should be removed.
-
-                st_in = Structure.from_file(
+                # We read structures from MC, but we also need to add ignored species.
+                # We utilize structure_norel.*.vasp, which is the structure before solver run
+                # in MC with ignored species.
+                st = Structure.from_file(
                     os.path.join(MCdir, str(myreplica), f"structure.{i}.vasp")
                 )
+                ignore_structure = Structure.from_file(
+                    os.path.join(MCdir, str(myreplica), f"structure_norel.{i}.vasp")
+                )
 
-                # (i)
-                st = map2perflat(perf_st, st_in)
-                st.remove_species(["X"])
-                # (ii)
-                if alparams.vac_space_holder:
-                    st.remove_species(alparams.vac_space_holder)
+                if mcparams.ignore_species:
+                    remove_sp = filter(
+                        lambda sp: sp not in mcparams.ignore_species, ignore_structure.symbol_set
+                        )
+                    ignore_structure.remove_species(remove_sp)
+                    for site in ignore_structure:
+                        st.append(site.species_string, site.frac_coords)
+                st.sort(key=lambda site: site.species_string)
+                st0 = st.copy()
+                
                 perturb_structure(st, perturb)
                 solver_input.update_info_by_structure(st)
                 solver_input.write_input(
                     os.path.abspath(os.path.join(fmtstr.format(i), "baseinput0"))
                 )
+                st0.to(fmt='POSCAR',filename=os.path.abspath(os.path.join(fmtstr.format(i), "initial.vasp")))
                 rundir_list.append(
                     os.path.abspath(os.path.join(fmtstr.format(i), "baseinput0"))
                 )
             rundir_list = comm.gather(rundir_list, root=0)
             if myreplica == 0:
                 rundir_list = [rundir for sublist in rundir_list for rundir in sublist]
                 with open(os.path.join(rootdir, "rundirs.txt"), "w") as fi:
                     fi.write("\n".join(rundir_list))
                     fi.write("\n")
                     fi.flush()
                     os.fsync(fi.fileno())
-                print(f"-Finished preparing {alparams.solver} input in AL{nextMC_index}/*/input*/baseinput0.",
-                      "--See rundirs.txt for a full list of the directories.",
-                      sep = os.linesep)
-                print("--Please perform the calculations in those directories before running abics_mlref again.")
+                logger.info(f"-Finished preparing {alparams.solver} input in AL{nextMC_index}/*/input*/baseinput0.")
+                logger.info("--See rundirs.txt for a full list of the directories.")
+                logger.info("--Please perform the calculations in those directories before running abics_mlref again.")
                 now = datetime.datetime.now()
-                print(f"Exiting normally on {now}.\n")
+                logger.info(f"Exiting normally on {now}.\n")
             sys.exit(0)
 
 
 def main():
+
     now = datetime.datetime.now()
-    if MPI.COMM_WORLD.Get_rank() == 0:
-        print("Running abics_mlref (abICS v{}) on {}".format(__version__, now))
 
+    import toml
     tomlfile = sys.argv[1] if len(sys.argv) > 1 else "input.toml"
-    if MPI.COMM_WORLD.Get_rank() == 0:
-        print("-Reading input from: {}".format(tomlfile))
-    main_impl(tomlfile)
+    params_root = toml.load(tomlfile)
+
+    loggers.set_log_handles(
+        app_name="activelearn",
+        level=logging.INFO,
+        params=params_root.get("log", {}))
+
+    logger.info(f"Running abics_mlref (abICS v{__version__}) on {now}")
+    logger.info(f"-Reading input from: {tomlfile}")
+
+    main_impl(params_root)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `abics-2.0.1/abics/scripts/main.py` & `abics-2.1.0/abics/scripts/main_dft_latgas.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,391 +10,394 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
+from typing import MutableMapping, Union
+
 from mpi4py import MPI
 import copy
 import sys, os, shutil
 import datetime
 
 import numpy as np
 import scipy.constants as constants
 
 from abics import __version__
-from abics.mc import CanonicalMonteCarlo, RandomSampling
-from abics.mc_mpi import (
-    RX_MPI_init,
-    TemperatureRX_MPI,
-    RXParams,
-    SamplerParams,
-    ParallelRandomParams,
-    EmbarrassinglyParallelSampling,
-)
-from abics.applications.latgas_abinitio_interface import (
-    default_observer,
+from abics.mc import CanonicalMonteCarlo, WeightedCanonicalMonteCarlo, RandomSampling
+from abics.observer import ObserverParams
+
+from abics.sampling.mc_mpi import RX_MPI_init
+from abics.sampling.rxmc import TemperatureRX_MPI, RXParams
+from abics.sampling.pamc import PopulationAnnealing, PAMCParams
+from abics.sampling.simple_parallel import EmbarrassinglyParallelSampling, ParallelRandomParams
+
+from abics.applications.latgas_abinitio_interface.default_observer import (
+    DefaultObserver,
     EnsembleParams,
-    ensemble_error_observer,
+    EnsembleErrorObserver,
 )
 from abics.applications.latgas_abinitio_interface.model_setup import (
-    dft_latgas,
-    ObserverParams,
+    DFTLatticeGas,
 )
 from abics.applications.latgas_abinitio_interface.defect import (
     defect_config,
     DFTConfigParams,
 )
 from abics.applications.latgas_abinitio_interface.run_base_mpi import (
-    runner,
-    runner_ensemble,
-    runner_multistep,
+    Runner,
+    RunnerEnsemble,
+    RunnerMultistep,
 )
-from abics.applications.latgas_abinitio_interface.vasp import VASPSolver
-from abics.applications.latgas_abinitio_interface.qe import QESolver
-from abics.applications.latgas_abinitio_interface.aenet import aenetSolver
-from abics.applications.latgas_abinitio_interface.openmx import OpenMXSolver
-from abics.applications.latgas_abinitio_interface.mocksolver import MockSolver
+from abics.applications.latgas_abinitio_interface.base_solver import SolverBase, create_solver
 from abics.applications.latgas_abinitio_interface.params import DFTParams
 
 from abics.util import exists_on_all_nodes
 
+import logging
+logger = logging.getLogger("main")
 
-def main_impl(tomlfile):
-    dftparams = DFTParams.from_toml(tomlfile)
-    samplerparams = SamplerParams.from_toml(tomlfile)
-    if samplerparams.sampler == "RXMC":
-        rxparams = RXParams.from_toml(tomlfile)
+def main_dft_latgas(params_root: MutableMapping):
+    params_sampling = params_root.get("sampling", None)
+    if not params_sampling:
+        logger.error("sampling section is missing in parameters")
+        sys.exit(1)
+    dftparams = DFTParams.from_dict(params_sampling["solver"])
+    sampler_type = params_sampling.get("sampler", "RXMC")
+    params_observer = params_root.get("observer", {})
+
+    if sampler_type == "RXMC":
+        rxparams = RXParams.from_dict(params_sampling)
         nreplicas = rxparams.nreplicas
         nprocs_per_replica = rxparams.nprocs_per_replica
 
         kB = constants.value("Boltzmann constant in eV/K")
 
-        comm, commEnsemble, commAll = RX_MPI_init(rxparams, dftparams)
+        nensemble = len(dftparams.base_input_dir)
+        comm, commEnsemble, commAll = RX_MPI_init(rxparams.nreplicas, rxparams.seed, nensemble)
 
         # RXMC parameters
         # specify temperatures for each replica, number of steps, etc.
-        kTstart = rxparams.kTstart
-        kTend = rxparams.kTend
-        kTs = kB * np.linspace(kTstart, kTend, nreplicas)
+        kTs = kB * rxparams.kTs
+        kTstart = rxparams.kTs[0]
+        kTend = rxparams.kTs[-1]
 
         # Set Lreload to True when restarting
         Lreload = rxparams.reload
 
         nsteps = rxparams.nsteps
         RXtrial_frequency = rxparams.RXtrial_frequency
         sample_frequency = rxparams.sample_frequency
         print_frequency = rxparams.print_frequency
 
-        if commAll.Get_rank() == 0:
-            print(f"-Running RXMC calculation with {nreplicas} replicas")
-            print(f"--Temperatures are linearly spaced from {kTstart} K to {kTend} K")
-            sys.stdout.flush()
+        logger.info(f"-Running RXMC calculation with {nreplicas} replicas")
+        logger.info(f"--Temperature varies from {kTstart} K to {kTend} K")
+
+    elif sampler_type == "PAMC":
+        pamcparams = PAMCParams.from_dict(params_sampling)
+        nreplicas = pamcparams.nreplicas
+        nprocs_per_replica = pamcparams.nprocs_per_replica
+
+        kB = constants.value("Boltzmann constant in eV/K")
+
+        nensemble = len(dftparams.base_input_dir)
+        comm, commEnsemble, commAll = RX_MPI_init(pamcparams.nreplicas, pamcparams.seed, nensemble)
+
+        # RXMC parameters
+        # specify temperatures for each replica, number of steps, etc.
+        kTstart = pamcparams.kTs[0]
+        kTend = pamcparams.kTs[-1]
+        if kTstart < kTend:
+            kTstart, kTend = kTend, kTstart
+        kTs = kB * pamcparams.kTs
+
+        # Set Lreload to True when restarting
+        Lreload = pamcparams.reload
+
+        nsteps = pamcparams.nsteps
+        resample_frequency = pamcparams.resample_frequency
+        sample_frequency = pamcparams.sample_frequency
+        print_frequency = pamcparams.print_frequency
 
-    elif samplerparams.sampler == "parallelRand":
-        rxparams = ParallelRandomParams.from_toml(tomlfile)
+        logger.info(f"-Running PAMC calculation with {nreplicas} replicas")
+        logger.info(f"--Anneal from {kTstart} K to {kTend} K")
+
+    elif sampler_type == "parallelRand":
+        rxparams = ParallelRandomParams.from_dict(params_sampling)
         nreplicas = rxparams.nreplicas
         nprocs_per_replica = rxparams.nprocs_per_replica
-        comm, commEnsemble, commAll = RX_MPI_init(rxparams, dftparams)
+        nensemble = len(dftparams.base_input_dir)
+        comm, commEnsemble, commAll = RX_MPI_init(rxparams.nreplicas, rxparams.seed, nensemble)
 
         # Set Lreload to True when restarting
         Lreload = rxparams.reload
 
         nsteps = rxparams.nsteps
         sample_frequency = rxparams.sample_frequency
         print_frequency = rxparams.print_frequency
-        if commAll.Get_rank() == 0:
-            print(f"-Running parallel random sampling")
-            sys.stdout.flush()
-    elif samplerparams.sampler == "parallelMC":
-        rxparams = RXParams.from_toml(tomlfile)
+        logger.info(f"-Running parallel random sampling")
+
+    elif sampler_type == "parallelMC":
+        rxparams = RXParams.from_dict(params_sampling)
         nreplicas = rxparams.nreplicas
         nprocs_per_replica = rxparams.nprocs_per_replica
 
         kB = constants.value("Boltzmann constant in eV/K")
 
-        comm, commEnsemble, commAll = RX_MPI_init(rxparams, dftparams)
+        nensemble = len(dftparams.base_input_dir)
+        comm, commEnsemble, commAll = RX_MPI_init(rxparams.nreplicas, rxparams.seed, nensemble)
 
         # RXMC parameters
         # specify temperatures for each replica, number of steps, etc.
-        kTstart = rxparams.kTstart
-        kTend = rxparams.kTend
-        kTs = kB * np.linspace(kTstart, kTend, nreplicas)
+        kTstart = rxparams.kTs[0]
+        kTend = rxparams.kTs[-1]
+        kTs = kB * rxparams.kTs
 
         # Set Lreload to True when restarting
         Lreload = rxparams.reload
 
         nsteps = rxparams.nsteps
         sample_frequency = rxparams.sample_frequency
         print_frequency = rxparams.print_frequency
-        if commAll.Get_rank() == 0:
-            print(f"-Running parallel MC sampling")
-            sys.stdout.flush()
-    else:
-        print("Unknown sampler. Exiting...")
-        sys.exit(1)
+        logger.info(f"-Running parallel MC sampling")
 
-    if dftparams.solver == "vasp":
-        solver = VASPSolver(dftparams.path)
-    elif dftparams.solver == "qe":
-        parallel_level = dftparams.properties.get("parallel_level", {})
-        solver = QESolver(dftparams.path, parallel_level=parallel_level)
-    elif dftparams.solver == "aenet":
-        solver = aenetSolver(
-            dftparams.path, dftparams.ignore_species, dftparams.solver_run_scheme
-        )
-    elif dftparams.solver == "openmx":
-        solver = OpenMXSolver(dftparams.path)
-    elif dftparams.solver == "mock":
-        solver = MockSolver()
     else:
-        print("unknown solver: {}".format(dftparams.solver))
+        logger.error("Unknown sampler. Exiting...")
         sys.exit(1)
-    if commAll.Get_rank() == 0:
-        print(f"-Setting up {dftparams.solver} solver for configuration energies")
-        print("--Base input is taken from {}".format(",".join(dftparams.base_input_dir)))
-        sys.stdout.flush()
+
+
+    solvers = []
+    for i in range(len(dftparams.base_input_dir)):
+        solver: SolverBase = create_solver(dftparams.solver, dftparams)
+        solvers.append(solver)
+    
+    logger.info(f"-Setting up {dftparams.solver} solver for configuration energies")
+    logger.info("--Base input is taken from {}".format(",".join(dftparams.base_input_dir)))
+
     # model setup
     # we first choose a "model" defining how to perform energy calculations and trial steps
     # on the "configuration" defined below
+    energy_calculator: Union[Runner, RunnerEnsemble, RunnerMultistep]
     if dftparams.ensemble:
         if len(dftparams.base_input_dir) == 1:
-            print(
-                "You must specify more than one base_input_dir for ensemble calculator"
-            )
+            logger.error("You must specify more than one base_input_dir for ensemble calculator")
             sys.exit(1)
-        energy_calculator = runner_ensemble(
+        energy_calculator = RunnerEnsemble(
             base_input_dirs=dftparams.base_input_dir,
-            Solver=solver,
-            runner=runner,
+            Solvers=solvers,
+            runner=Runner,
             nprocs_per_solver=nprocs_per_replica,
             comm=commEnsemble,
             perturb=dftparams.perturb,
             solver_run_scheme=dftparams.solver_run_scheme,
             use_tmpdir=dftparams.use_tmpdir,
         )
     else:
         if len(dftparams.base_input_dir) == 1:
-            energy_calculator = runner(
+            energy_calculator = Runner(
                 base_input_dir=dftparams.base_input_dir[0],
-                Solver=solver,
+                Solver=solvers[0],
                 nprocs_per_solver=nprocs_per_replica,
                 comm=MPI.COMM_SELF,
                 perturb=dftparams.perturb,
                 solver_run_scheme=dftparams.solver_run_scheme,
                 use_tmpdir=dftparams.use_tmpdir,
             )
         else:
-            energy_calculator = runner_multistep(
+            energy_calculator = RunnerMultistep(
                 base_input_dirs=dftparams.base_input_dir,
-                Solver=solver,
-                runner=runner,
+                Solvers=solvers,
+                runner=Runner,
                 nprocs_per_solver=nprocs_per_replica,
                 comm=MPI.COMM_SELF,
                 perturb=dftparams.perturb,
                 solver_run_scheme=dftparams.solver_run_scheme,
                 use_tmpdir=dftparams.use_tmpdir,
             )
-    model = dft_latgas(energy_calculator, save_history=False)
-    if commAll.Get_rank() == 0:
-        print("--Success.")
-
-    # defect sublattice setup
-    if commAll.Get_rank() == 0:
-        print("-Setting up the on-lattice model.")
 
-    sys.stdout.flush()
+    gc_flag  = params_sampling.get("enable_grandcanonical", False)
+    gc_ratio = params_sampling.get("gc_ratio", 0.3)
+
+    model = DFTLatticeGas(energy_calculator,
+                          save_history=False,
+                          enable_grandcanonical=gc_flag,
+                          gc_ratio=gc_ratio,
+    )
+
+    logger.info("--Success.")
+    logger.info("-Setting up the on-lattice model.")
     
-    configparams = DFTConfigParams.from_toml(tomlfile)
+    configparams = DFTConfigParams.from_dict(params_root["config"])
 
     spinel_config = defect_config(configparams)
+    if configparams.init_structure is None:
+        exit_code, msg = spinel_config.shuffle()
+        logger.info("--Rank {}: {}".format(commAll.Get_rank(), msg))
+        exit_code = commAll.allgather(exit_code)
+        if np.sum(exit_code) != 0:
+            logger.error("Failed to initialize configuration. Exiting.")
+            sys.exit(1)
+    else:
+        logger.info("--Initial structure will be set to 'config.init_structure'.")
+        spinel_config.reset_from_structure(configparams.init_structure)
 
     # configs = []
     # for i in range(nreplicas):
     #    configs.append(copy.deepcopy(spinel_config))
     configs = [spinel_config] * nreplicas
 
-    obsparams = ObserverParams.from_toml(tomlfile)
+    obsparams = ObserverParams.from_dict(params_observer)
 
-    if commAll.Get_rank() == 0:
-        print("--Success.")
+    logger.info("--Success.")
 
-    
     # NNP ensemble error estimation
-    ensembleparams = EnsembleParams.from_toml(tomlfile)
-    if ensembleparams:
-        if ensembleparams.solver == "vasp":
-            solver = VASPSolver(ensembleparams.path)
-        elif ensembleparams.solver == "qe":
-            parallel_level = ensembleparams.properties.get("parallel_level", {})
-            solver = QESolver(ensembleparams.path, parallel_level=parallel_level)
-        elif ensembleparams.solver == "aenet":
-            solver = aenetSolver(
-                ensembleparams.path,
-                ensembleparams.ignore_species,
-                ensembleparams.solver_run_scheme,
-            )
-        elif ensembleparams.solver == "openmx":
-            solver = OpenMXSolver(ensembleparams.path)
-        elif ensembleparams.solver == "mock":
-            solver = MockSolver()
-        else:
-            print("unknown solver: {}".format(ensembleparams.solver))
-            sys.exit(1)
+    if "ensemble" in params_root:
+        ensembleparams = EnsembleParams.from_dict(params_root["ensemble"])
+        solver = create_solver(ensembleparams.solver, ensembleparams)
 
         energy_calculators = [
-            runner(
+            Runner(
                 base_input_dir=base_input_dir,
                 Solver=copy.deepcopy(solver),
                 nprocs_per_solver=nprocs_per_replica,
                 comm=MPI.COMM_SELF,
                 perturb=ensembleparams.perturb,
                 solver_run_scheme=ensembleparams.solver_run_scheme,
                 use_tmpdir=dftparams.use_tmpdir,
             )
             for base_input_dir in ensembleparams.base_input_dirs
         ]
-        observer = ensemble_error_observer(commEnsemble, energy_calculators, Lreload)
+        observer: DefaultObserver = EnsembleErrorObserver(commEnsemble, energy_calculators, Lreload)
     else:
-        observer = default_observer(comm, Lreload)
+        observer = DefaultObserver(comm, Lreload, params_observer)
 
     ALrun = exists_on_all_nodes(commAll, "ALloop.progress")
 
     # Active learning mode
     if ALrun:
-        if commAll.Get_rank() == 0:
-            print(f"-Running in active learning mode.")
+        logger.info(f"-Running in active learning mode.")
 
         if "train0" in os.listdir():
             # Check how many AL iterations have been performed
             i = 0
             while exists_on_all_nodes(commAll, "MC{}".format(i)):
                 i += 1
             with open("ALloop.progress", "r") as fi:
                 last_li = fi.readlines(-1)[-1]
             if "train" not in last_li:
-                print("You should train before next MC sampling.")
+                logger.error("You should train before next MC sampling.")
                 sys.exit(1)
             if Lreload:
-                if commAll.Get_rank() == 0:
-                    print(f"--Restarting run in MC{i-1}")
-                    sys.stdout.flush()
+                logger.info(f"--Restarting run in MC{i-1}")
                 rootdir = os.getcwd()
                 os.chdir("MC{}".format(i - 1))
                 MCid = i - 1
             else:
                 # Make new directory and perform sampling there
                 if commAll.Get_rank() == 0:
-                    print(f"--MC sampling will be run in MC{i}")
+                    logger.info(f"--MC sampling will be run in MC{i}")
                     os.mkdir("MC{}".format(i))
                     if dftparams.use_tmpdir:
-                        print(f"---Will use local tmpdir for {dftparams.solver} run")
+                        logger.info(f"---Will use local tmpdir for {dftparams.solver} run")
                         # backup baseinput for this AL step
                         for j, d in enumerate(dftparams.base_input_dir):
                             shutil.copytree(d, "MC{}/baseinput{}".format(i, j))
                     sys.stdout.flush()
                 commAll.Barrier()
                 rootdir = os.getcwd()
                 while not exists_on_all_nodes(commAll, "MC{}".format(i)):
                     pass
                 os.chdir("MC{}".format(i))
                 MCid = i
         else:
-            print("You should train before MC sampling in AL mode.")
+            logger.error("You should train before MC sampling in AL mode.")
             sys.exit(1)
 
+    if gc_flag == True:
+        mc_class = WeightedCanonicalMonteCarlo
+    else:
+        mc_class = CanonicalMonteCarlo
+
     if commEnsemble.Get_rank() == 0:
         write_node = True
     else:
         write_node = False
-    if samplerparams.sampler == "RXMC":
+    if sampler_type == "RXMC":
         # RXMC calculation
         RXcalc = TemperatureRX_MPI(
-            comm, CanonicalMonteCarlo, model, configs, kTs, write_node=write_node
+            comm, mc_class, model, configs, kTs, write_node=write_node
         )
         if Lreload:
-            if commAll.Get_rank() == 0:
-                print("-Reloading from previous calculation")
+            logger.info("-Reloading from previous calculation")
             RXcalc.reload()
 
-        if commAll.Get_rank() == 0:
-            print("-Starting RXMC calculation")
-            sys.stdout.flush()
+        logger.info("-Starting RXMC calculation")
             
         obs = RXcalc.run(
             nsteps,
             RXtrial_frequency,
-            sample_frequency,
-            print_frequency,
+            sample_frequency=sample_frequency,
+            print_frequency=print_frequency,
             observer=observer,
             subdirs=True,
         )
 
-        #if comm.Get_rank() == 0 and write_node:
-        #    print(obs)
+    elif sampler_type == "PAMC":
+        # PAMC calculation
+        PAcalc = PopulationAnnealing(
+            comm, mc_class, model, configs, kTs, write_node=write_node
+        )
+        if Lreload:
+            logger.info("-Reloading from previous calculation")
+            PAcalc.reload()
 
-    elif samplerparams.sampler == "parallelRand":
+        logger.info("-Starting PAMC calculation")
+            
+        obs = PAcalc.run(
+            nsteps,
+            resample_frequency,
+            sample_frequency=sample_frequency,
+            print_frequency=print_frequency,
+            observer=observer,
+            subdirs=True,
+        )
+
+    elif sampler_type == "parallelRand":
         calc = EmbarrassinglyParallelSampling(
             comm, RandomSampling, model, configs, write_node=write_node
         )
         if Lreload:
             calc.reload()
         obs = calc.run(
             nsteps,
-            sample_frequency,
-            print_frequency,
+            sample_frequency=sample_frequency,
+            print_frequency=print_frequency,
             observer=observer,
             subdirs=True,
         )
 
-        #if comm.Get_rank() == 0 and write_node:
-        #    print(obs)
-
-    elif samplerparams.sampler == "parallelMC":
+    elif sampler_type == "parallelMC":
         calc = EmbarrassinglyParallelSampling(
-            comm, CanonicalMonteCarlo, model, configs, kTs, write_node=write_node
+            comm, mc_class, model, configs, kTs, write_node=write_node
         )
         if Lreload:
             calc.reload()
         obs = calc.run(
             nsteps,
-            sample_frequency,
-            print_frequency,
+            sample_frequency=sample_frequency,
+            print_frequency=print_frequency,
             observer=observer,
             subdirs=True,
         )
+    logger.info("--Sampling completed sucessfully.")
 
-        #if comm.Get_rank() == 0 and write_node:
-        #    print(obs)
-
-    if commAll.Get_rank() == 0:
-        print("--Sampling completed sucessfully.")
     if ALrun:
         os.chdir(rootdir)
         if comm.Get_rank() == 0 and write_node:
-            print("-Writing ALloop.progress")
+            logger.info("-Writing ALloop.progress")
             with open("ALloop.progress", "a") as fi:
                 fi.write("MC{}\n".format(MCid))
                 fi.flush()
                 os.fsync(fi.fileno())
-
-    if commAll.Get_rank() == 0:
-        now = datetime.datetime.now()
-        print(f"Exiting normally on {now}\n")
-
-
-def main():
-    now = datetime.datetime.now()
-    
-    if MPI.COMM_WORLD.Get_rank() == 0:
-        print("Running abics_sampling (abICS v{}) on {}".format(__version__, now))
-        
-    tomlfile = sys.argv[1] if len(sys.argv) > 1 else "input.toml"
-    if MPI.COMM_WORLD.Get_rank() == 0:
-        print("-Reading input from: {}".format(tomlfile))
-
-    main_impl(tomlfile)
-
-
-if __name__ == "__main__":
-    main()
+    logger.info("Exiting normally on {}\n".format(datetime.datetime.now()))
```

### Comparing `abics-2.0.1/abics/scripts/mocksolver.py` & `abics-2.1.0/abics/scripts/mocksolver.py`

 * *Files identical despite different names*

### Comparing `abics-2.0.1/abics/scripts/st2abics_config.py` & `abics-2.1.0/abics/scripts/st2abics_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,20 +141,20 @@
             config.append("[[config.defect_structure.groups]]")
             config.append('name = "{}"'.format(group["name"]))
             config.append("species = {}".format(group["species"]))
             config.append("coords = [")
             for coord in group["coords"]:
                 if len(coord) == 1:
                     c = coord[0]
-                    config.append('"{} {} {}"'.format(c[0], c[1], c[2]))
+                    config.append('[[{}, {}, {}]]'.format(c[0], c[1], c[2]))
                 else:
-                    config.append('"""')
+                    config.append('[')
                     for c in coord:
-                        config.append("{} {} {}".format(c[0], c[1], c[2]))
-                    config.append('""",')
+                        config.append("[{}, {}, {}],".format(c[0], c[1], c[2]))
+                    config.append('],')
             config.append("]")
             config.append("num = {}".format(group["num"]))
             config.append("")
 
     # config = toml.dumps(abics_input_dict)
     with open(
         os.path.join(os.path.dirname(__file__), "input_template.toml"), "r"
```

### Comparing `abics-2.0.1/abics/scripts/train.py` & `abics-2.1.0/abics/scripts/train.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,167 +10,202 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
+from __future__ import annotations
+from typing import MutableMapping, Any
+
 import sys, datetime
 
+import os, sys
+import itertools
+
+import numpy as np
+import networkx as nx
+from pymatgen.core import Structure
+
 from abics import __version__
 from abics.applications.latgas_abinitio_interface.params import DFTParams, TrainerParams
 from abics.applications.latgas_abinitio_interface import aenet_trainer
 from abics.applications.latgas_abinitio_interface import map2perflat
-from abics.applications.latgas_abinitio_interface.naive_matcher import naive_mapping
 from abics.applications.latgas_abinitio_interface.defect import (
     defect_config,
     DFTConfigParams,
 )
 
-from pymatgen.core import Structure
-import numpy as np
-import os, sys
-import threading
-import networkx as nx
-import itertools
+import logging
+import abics.loggers as loggers
+
+logger = logging.getLogger("main")
 
 
-def main_impl(tomlfile):
+def main_impl(params_root: MutableMapping):
     if not os.path.exists("ALloop.progress"):
-        print("abics_mlref has not run yet.")
+        logger.error("abics_mlref has not run yet.")
         sys.exit(1)
     ALdirs = []
     with open("ALloop.progress", "r") as fi:
         lines = fi.readlines()
         for line in lines:
             line = line.strip()
             if line.startswith("AL"):
                 ALdirs.append(line)
         last_li = lines[-1].strip()
     if not last_li.startswith("AL"):
-        print("You shouldn't run train now.")
-        print("Either abics_sampling or abics_mlref first.")
+        logger.error("You shouldn't run train now.")
+        logger.error("Either abics_sampling or abics_mlref first.")
         sys.exit(1)
 
-    dftparams = DFTParams.from_toml(tomlfile)
+    dftparams = DFTParams.from_dict(params_root["sampling"]["solver"])
     ensemble = dftparams.ensemble
     base_input_dir = dftparams.base_input_dir
 
-    trainerparams = TrainerParams.from_toml(tomlfile)
+    trainerparams = TrainerParams.from_dict(params_root["train"])
     ignore_species = trainerparams.ignore_species
     trainer_commands = trainerparams.exe_command
     trainer_type = trainerparams.solver
     trainer_input_dirs = trainerparams.base_input_dir
+    previous_dirs = trainerparams.previous_dir
 
-    configparams = DFTConfigParams.from_toml(tomlfile)
+    configparams = DFTConfigParams.from_dict(params_root["config"])
     config = defect_config(configparams)
     species = config.structure.symbol_set
     dummy_sts = {sp: config.dummy_structure_sp(sp) for sp in species}
 
     if trainer_type != "aenet":
-        print("Unknown trainer: ", trainer_type)
+        logger.error("Unknown trainer: ", trainer_type)
         sys.exit(1)
 
     rootdir = os.getcwd()
     structures = []
     energies = []
+    if len(previous_dirs) > 0:
+        logger.info("-Adding data in previous_dirs to data set")
 
+        for dir in previous_dirs:
+            os.chdir(dir)
+            num_st = len(os.listdir())
+            st_fis = ["structure.{}.xsf".format(i) for i in range(num_st)]
+            for fi in st_fis:
+                structures.append(Structure.from_file(fi))
+                with open(fi) as f:
+                    li = f.readline()
+                    e = float(li.split()[4])
+                energies.append(e)
+        os.chdir(rootdir)
+        logger.info("--Done")
+
+
+    logger.info("-Mapping relaxed structures in AL* to on-lattice model...")
 
-    print("-Mapping relaxed structures in AL* to on-lattice model...")
-    sys.stdout.flush()
     # val_map is a list of list [[sp0, vac0], [sp1, vac1], ...]
     # if vac_map:
     #    vac_map = {specie: vacancy for specie, vacancy in vac_map}
     # else:
     #    vac_map = {}
 
     # we first group species that share sublattices together
-
     G = nx.Graph()
     G.add_nodes_from(species)
     for sublattice in config.defect_sublattices:
         groups = sublattice.groups
         sp_list = []
         for group in groups:
             sp_list.extend(group.species)
         for pair in itertools.combinations(sp_list, 2):
             G.add_edge(*pair)
     sp_groups = nx.connected_components(G)
-    # print(list(sp_groups))
-    # sys.exit(0)
-    dummy_sts_share = []
+    dummy_sts_share : list[tuple[Structure, list]] = []
     for c in nx.connected_components(G):
         # merge dummy structures for species that share sublattices
         sps = list(c)
 
         coords = np.concatenate([dummy_sts[sp].frac_coords for sp in sps], axis=0)
         st_tmp = Structure(
             dummy_sts[sps[0]].lattice,
             species=["X"] * coords.shape[0],
             coords=coords,
         )
-        st_tmp.merge_sites(mode="del")
-        dummy_sts_share.append([st_tmp, sps])
-
-    # for i,st in enumerate(dummy_sts_share):
-    #    st.to(fmt="POSCAR", filename="{}.dummy.vasp".format(i))
-
-    for dir in ALdirs:
-        rpl = 0
-        while os.path.isdir(os.path.join(dir, str(rpl))):
-            os.chdir(os.path.join(dir, str(rpl)))
-            energies_ref = []
-            step_ids = []
-            with open("energy_corr.dat") as fi:
-                for line in fi:
-                    words = line.split()
-                    energies_ref.append(float(words[1]))
-                    step_ids.append(int(words[2]))
-            for step_id, energy in zip(step_ids, energies_ref):
-                structure = Structure.from_file(f"structure.{step_id}.vasp")
-                mapped_sts = []
-                mapping_success = True
-                for dummy_st, specs in dummy_sts_share:
-                    # perform sublattice by sublattice mapping
-                    sp_rm = filter(lambda s: s not in specs, species)
-                    st_tmp = structure.copy()
-                    st_tmp.remove_species(sp_rm)
-                    num_sp = len(st_tmp)
-                    # map to perfect lattice for this species
-                    st_tmp = map2perflat(dummy_st, st_tmp)
-                    st_tmp.remove_species(["X"])
-                    mapped_sts.append(st_tmp)
-                    if num_sp != len(st_tmp):
-                        print(
-                            f"--mapping failed for structure {step_id} in replica {rpl}"
-                        )
-                        mapping_success = False
-
-                for sts in mapped_sts[1:]:
-                    for i in range(len(sts)):
-                        mapped_sts[0].append(sts[i].species_string, sts[i].frac_coords)
-                if ignore_species:
-                    mapped_sts[0].remove_species(ignore_species)
-                if mapping_success:
-                    structures.append(mapped_sts[0])
-                    energies.append(energy)
-            rpl += 1
-            os.chdir(rootdir)
-    print("--Finished mapping")
-    sys.stdout.flush()
+        st_tmp.merge_sites(mode="delete")
+        dummy_sts_share.append((st_tmp, sps))
+    if len(ALdirs) > 1:
+        logger.info(f"-Reading previously mapped structures up to {ALdirs[-2]}")
+        for dir in ALdirs[:-1]:
+            rpl = 0
+            while os.path.isdir(os.path.join(dir, str(rpl))):
+                os.chdir(os.path.join(dir, str(rpl)))
+                energies_ref = []
+                step_ids = []
+                with open("energy_corr.dat") as fi:
+                    for line in fi:
+                        words = line.split()
+                        energies_ref.append(float(words[1]))
+                        step_ids.append(int(words[2]))
+                for step_id, energy in zip(step_ids, energies_ref):
+                    if os.path.exists(f"structure.{step_id}_mapped.vasp"):
+                        structures.append(Structure.from_file(f"structure.{step_id}_mapped.vasp"))
+                        energies.append(energy)
+                rpl += 1
+                os.chdir(rootdir)
+
+        logger.info("--Finished reading previously mapped structures")
+
+    logger.info(f"-Mapping structures in {ALdirs[-1]}")
+    dir = ALdirs[-1]
+    rpl = 0
+    while os.path.isdir(os.path.join(dir, str(rpl))):
+        os.chdir(os.path.join(dir, str(rpl)))
+        energies_ref = []
+        step_ids = []
+        with open("energy_corr.dat") as fi:
+            for line in fi:
+                words = line.split()
+                energies_ref.append(float(words[1]))
+                step_ids.append(int(words[2]))
+        for step_id, energy in zip(step_ids, energies_ref):
+            structure: Structure = Structure.from_file(f"structure.{step_id}.vasp")
+            mapped_sts = []
+            mapping_success = True
+            for dummy_st, specs in dummy_sts_share:
+                # perform sublattice by sublattice mapping
+                sp_rm = list(filter(lambda s: s not in specs, species))
+                st_tmp = structure.copy()
+                st_tmp.remove_species(sp_rm)
+                num_sp = len(st_tmp)
+                # map to perfect lattice for this species
+                st_tmp = map2perflat(dummy_st, st_tmp)
+                st_tmp.remove_species(["X"])
+                mapped_sts.append(st_tmp)
+                if num_sp != len(st_tmp):
+                    logger.info(f"--mapping failed for structure {step_id} in replica {rpl}")
+                    mapping_success = False
+
+            for sts in mapped_sts[1:]:
+                for i in range(len(sts)):
+                    mapped_sts[0].append(sts[i].species_string, sts[i].frac_coords)
+            if ignore_species:
+                mapped_sts[0].remove_species(ignore_species)
+            if mapping_success:
+                structures.append(mapped_sts[0])
+                mapped_sts[0].to(filename=f"structure.{step_id}_mapped.vasp", fmt="POSCAR")
+                energies.append(energy)
+        rpl += 1
+        os.chdir(rootdir)
+    logger.info("--Finished mapping")
     
     generate_input_dirs = []
     train_input_dirs = []
     predict_input_dirs = []
 
     if dftparams.ensemble:
         if len(trainer_input_dirs) != len(base_input_dir):
-            print(
-                "You must set the number of trainer input dirs equal to baseinput dirs for ensemble NNP"
-            )
+            logger.error("You must set the number of trainer input dirs equal to baseinput dirs for ensemble NNP")
             sys.exit(1)
     for d in trainer_input_dirs:
         generate_input_dirs.append(os.path.join(d, "generate"))
         train_input_dirs.append(os.path.join(d, "train"))
         predict_input_dirs.append(os.path.join(d, "predict"))
 
     generate_exe = trainer_commands[0]
@@ -188,58 +223,66 @@
                 generate_exe,
                 train_exe,
             )
         )
 
     trainers[0].prepare()
     # We use threads to parallelize generate.x over ensemble members
-    """threads = []
-    for i, trainer in enumerate(trainers):
-        threads.append(
-            threading.Thread(
-                target=trainer.generate(generate_dir="generate{}".format(i))
-                )
-            )
-        threads[-1].start()
-    for t in threads:
-        t.join()
-    """
+    # threads = []
+    # for i, trainer in enumerate(trainers):
+    #     threads.append(
+    #         threading.Thread(
+    #             target=trainer.generate(generate_dir="generate{}".format(i))
+    #             )
+    #         )
+    #     threads[-1].start()
+    # for t in threads:
+    #     t.join()
+
     for i, trainer in enumerate(trainers):
-        print(f"-Running generate run in generate{i}")
-        sys.stdout.flush()
+        logger.info(f"-Running generate run in generate{i}")
         trainer.generate_run(generate_dir="generate{}".format(i))
 
     for trainer in trainers:
         trainer.generate_wait()
-    print(f"--Finished generate run(s)")
+    logger.info(f"--Finished generate run(s)")
     
     # We use MPI version of train.x so no need to write parallel code here
     for i, trainer in enumerate(trainers):
-        print(f"-Training run in train{i}")
-        sys.stdout.flush()
+        logger.info(f"-Training run in train{i}")
         trainer.train(train_dir="train{}".format(i))
-        print(f"--Training run finished in train{i}")
-        print(f"-Preparing NN model for abics_sampling in {base_input_dir[i]}")
-        sys.stdout.flush()
+        logger.info(f"--Training run finished in train{i}")
+        logger.info(f"-Preparing NN model for abics_sampling in {base_input_dir[i]}")
         trainer.new_baseinput(base_input_dir[i])
-        print(f"--Success.")
+        logger.info(f"--Success.")
 
     with open("ALloop.progress", "a") as fi:
-        print("-Writing ALloop.progress")
+        logger.info("-Writing ALloop.progress")
         fi.write("train\n")
         fi.flush()
         os.fsync(fi.fileno())
     now = datetime.datetime.now()
-    print("-Let's run abics_sampling next!")
-    print(f"Exiting normally on {now}.\n")
+    logger.info("-Let's run abics_sampling next!")
+    logger.info(f"Exiting normally on {now}.\n")
 
 
 def main():
     now = datetime.datetime.now()
-    print("Running abics_train (abICS v{}) on {}".format(__version__, now))
+
+    import toml
     tomlfile = sys.argv[1] if len(sys.argv) > 1 else "input.toml"
-    print("-Reading input from: {}".format(tomlfile))
-    main_impl(tomlfile)
+    params_root = toml.load(tomlfile)
+
+    loggers.set_log_handles(
+        app_name = "train",
+        level = logging.INFO,
+        console = "serial",
+        params=params_root.get("log", {}))
+
+    logger.info(f"Running abics_train (abICS v{__version__}) on {now}")
+    logger.info(f"-Reading input from: {tomlfile}")
+
+    main_impl(params_root)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `abics-2.0.1/abics/util.py` & `abics-2.1.0/abics/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,43 +10,48 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see http://www.gnu.org/licenses/.
 
+from __future__ import annotations
+
 import os.path
 import pickle
 import time
 from itertools import groupby
 
 import numpy as np
+from numpy.typing import DTypeLike
 
 from .exception import InputError
 
 
-def read_vector(v, *, dtype=np.float):
+def read_vector(v: str | list[float] | np.ndarray, *, dtype: DTypeLike = np.float64) -> np.ndarray:
     return read_tensor(v, rank=1, dtype=dtype)
 
 
-def read_matrix(v, *, dtype=np.float):
+def read_matrix(v: str | list[float] | np.ndarray, *, dtype: DTypeLike = np.float64) -> np.ndarray:
     return read_tensor(v, rank=2, dtype=dtype)
 
 
-def read_tensor(v, *, rank=2, dtype=np.float):
+def read_tensor(
+    v: str | list[float] | list[list] | np.ndarray, *, rank: int = 2, dtype: DTypeLike = np.float64
+) -> np.ndarray:
     """
     Read tensor
 
     Parameters
     ----------
     v: str or list or np.ndarray
         tensor
 
     dtype: type
-        type of elements, default: np.float
+        type of elements, default: np.float64
 
     Returns
     -------
     v: numpy array
         tensor
     """
 
@@ -68,15 +73,15 @@
             ret = []
             lines = list(filter(lambda l: bool(l.strip()), v.splitlines()))
             n = len(lines)
             if n > 1:
                 ret = [parse(x, dtype) for x in lines]
             else:
                 ret = [parse(x, dtype) for x in lines[0].split()]
-            return ret
+            return np.array(ret)
         elif rank == 2:
             ret = []
             m0 = -1
             for line in v.splitlines():
                 try:
                     row = [parse(x, dtype) for x in line.strip().split()]
                 except ValueError as e:
@@ -94,18 +99,20 @@
                 return np.zeros((0, 0), dtype=dtype)
             return np.array(ret, dtype=dtype)
         else:
             raise InputError("read_tensor(rank>2) requires list-type argument")
     elif isinstance(v, list):
         if rank == 1:
             return np.array(v, dtype=dtype)
+        if not isinstance(v[0], list):
+            raise InputError("")
         m0 = -1
         ret = []
         for vv in v:
-            child = read_tensor(vv, rank=rank-1, dtype=dtype)
+            child = read_tensor(vv, rank=rank - 1, dtype=dtype)
             m = child.shape[0]
             if m0 < 0:
                 m0 = m
             if m != m0:
                 raise InputError("Dimension mismatch in {}".format(v))
             ret.append(child)
         return np.array(ret, dtype=dtype)
@@ -128,60 +135,68 @@
     Returns
     -------
     path: str
         path combined basedir with path (absolute path)
     """
     path = os.path.expanduser(path)
     path = os.path.expandvars(path)
-    if not path.startswith('/'):
+    if not path.startswith("/"):
         path = os.path.join(basedir, path)
     return path
 
+
 def expand_cmd_path(path):
     path = os.path.expanduser(path)
     path = os.path.expandvars(path)
     return path
 
+
 def pickle_dump(data, filename):
-    with open(filename, 'wb') as f:
+    with open(filename, "wb") as f:
         pickle.dump(data, f)
 
 
 def pickle_load(filename):
-    with open(filename, 'rb') as f:
+    with open(filename, "rb") as f:
         return pickle.load(f)
 
+
 def numpy_save(data, filename, allow_pickle=False):
-    with open(filename, 'wb') as f:
+    with open(filename, "wb") as f:
         np.save(f, data, allow_pickle)
 
 
 def numpy_load(filename):
-    with open(filename, 'rb') as f:
+    with open(filename, "rb") as f:
         return np.load(f)
 
+
 # all_equal function by kennytm
 # CC-BY-SA 4.0 https://stackoverflow.com/a/3844832
 def all_equal(iterable):
     g = groupby(iterable)
     return next(g, True) and not next(g, False)
 
-def exists_on_all_nodes(comm, path, check_interval = 1, max_wait = 30):
-    """ check ``path`` file is visible from all procs
-    """
+
+def exists_on_all_nodes(comm, path, check_interval=1, max_wait=30):
+    """check ``path`` file is visible from all procs"""
 
     counter = 0
     while True:
         exists = os.path.exists(path)
         exists_gather = comm.allgather(exists)
         # make sure all procs return same result
         if all_equal(exists_gather):
             break
         counter += 1
         if counter == max_wait:
-            raise TimeoutError("File system has been out of sync as seen from each process"
-                               " for {} seconds. Aborting.". format(check_interval * max_wait))
+            raise TimeoutError(
+                "File system has been out of sync as seen from each process"
+                " for {} seconds. Aborting.".format(check_interval * max_wait)
+            )
         if comm.Get_rank() == 0:
-            print("File system seems to be out of sync as seen from each process."
-                  " Waiting for sync. (Don't worry, this happens often on network file systems)")
+            print(
+                "File system seems to be out of sync as seen from each process."
+                " Waiting for sync. (Don't worry, this happens often on network file systems)"
+            )
         time.sleep(check_interval)
     return exists_gather[0]
```

### Comparing `abics-2.0.1/pyproject.toml` & `abics-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abics"
-version = "2.0.1"
+version = "2.1.0"
 description = "ab-Initio Configuration Sampling tool kit"
 authors = ["abICS developers <abics-dev@issp.u-tokyo.ac.jp>"]
 license = "GPL-3.0-or-later"
 
 readme = "README.md"
 repository = "https://github.com/issp-center-dev/abICS"
 
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 numpy = "^1.20"
 toml = ">=0.10"
 scipy = "^1"
 mpi4py = "^3"
-pymatgen = ">=2019.12.3"
+pymatgen = ">=2019.12.3 <2023.5.8"
 qe_tools = "^1.1"
 
 [tool.poetry.extras]
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.5.0"
 sphinx-rtd-theme = "^1.0.0"
@@ -32,10 +32,14 @@
 [tool.poetry.scripts]
 abics_sampling = "abics.scripts.main:main"
 st2abics = "abics.scripts.st2abics_config:main"
 abicsRXsepT = "abics.scripts.abicsRXsepT:main"
 abics_mlref = "abics.scripts.activelearn:main"
 abics_train = "abics.scripts.train:main"
 
+[tool.mypy]
+files = "abics"
+ignore_missing_imports = true
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `abics-2.0.1/PKG-INFO` & `abics-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: abics
-Version: 2.0.1
+Version: 2.1.0
 Summary: ab-Initio Configuration Sampling tool kit
 Home-page: https://github.com/issp-center-dev/abICS
 License: GPL-3.0-or-later
 Author: abICS developers
 Author-email: abics-dev@issp.u-tokyo.ac.jp
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mpi4py (>=3,<4)
 Requires-Dist: numpy (>=1.20,<2.0)
-Requires-Dist: pymatgen (>=2019.12.3)
+Requires-Dist: pymatgen (>=2019.12.3,<2023.5.8)
 Requires-Dist: qe_tools (>=1.1,<2.0)
 Requires-Dist: scipy (>=1,<2)
 Requires-Dist: toml (>=0.10)
 Project-URL: Repository, https://github.com/issp-center-dev/abICS
 Description-Content-Type: text/markdown
 
 # abICS
@@ -85,15 +86,15 @@
 
 ## Official page
 
 https://www.pasums.issp.u-tokyo.ac.jp/abics
 
 ## Author
 
-Shusuke Kasamatsu, Yuichi Motoyama, Kazuyoshi Yoshimi
+Shusuke Kasamatsu, Yuichi Motoyama, Tatsumi Aoyama, Kazuyoshi Yoshimi
 
 ## Manual
 
 [English online manual](https://issp-center-dev.github.io/abICS/docs/master/en/html/index.html)
 
 [Japnese online manual](https://issp-center-dev.github.io/abICS/docs/master/ja/html/index.html)
```

