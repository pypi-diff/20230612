# Comparing `tmp/atomcalc-0.1.0.tar.gz` & `tmp/atomcalc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomcalc-0.1.0.tar", max compression
+gzip compressed data, was "atomcalc-0.1.1.tar", max compression
```

## Comparing `atomcalc-0.1.0.tar` & `atomcalc-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      279 2023-06-03 16:12:35.652726 atomcalc-0.1.0/atomcalc/__init__.py
--rw-r--r--   0        0        0    27555 2023-06-07 12:25:50.128893 atomcalc-0.1.0/atomcalc/fidelity.py
--rw-r--r--   0        0        0      543 2023-06-07 13:15:21.392548 atomcalc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 11:10:34.022007 atomcalc-0.1.0/README.md
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 atomcalc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      279 2023-06-03 16:12:35.652726 atomcalc-0.1.1/atomcalc/__init__.py
+-rw-r--r--   0        0        0    27600 2023-06-12 18:09:46.970110 atomcalc-0.1.1/atomcalc/fidelity.py
+-rw-r--r--   0        0        0      526 2023-06-12 18:14:20.133388 atomcalc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-06 11:10:34.022007 atomcalc-0.1.1/README.md
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 atomcalc-0.1.1/PKG-INFO
```

### Comparing `atomcalc-0.1.0/atomcalc/fidelity.py` & `atomcalc-0.1.1/atomcalc/fidelity.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,28 @@
 
 
 class Level:
     """
     An object that describes an energy level.
 
     Args:
-        energy (list): value for :attr:`energy`
+        energy (number): value for :attr:`energy`
 
 
     Attributes:
-        energy (list): A list of a number that is the energy of the level.
+        energy (number): The energy of the level.
 
     Example:
 
-        >>> Level([5])
+        >>> Level(5)
         This is a Level object with an energy of 5.
     """
 
     def __init__(self, energy):
-        if type(energy) != list:
-            raise TypeError(
-                "Energy needs to be a list"
-            )  # meanwhile unnecessary to make this as a list
-        self.energy = energy[0]
+        self.energy = energy
 
 
 class Decay:
     """An object that describes the decay of the system with the decay rates and the respective transitions.
 
     Args:
         rates (list): value for :attr:`rates`
@@ -71,22 +67,25 @@
         frequency (number): value for :attr:`frequency`
         couple (list): value for :attr:`couple`
         pulse (None or function or list): value for :attr:`pulse`
 
 
     Attributes:
         rabifreq (number): Rabi frequency of the laser.
-        frequency (number): Frequency of the laser.
+        frequency (number): The to the frequency of the laser corresponding energy.
         couple (list): A tupel of :class:`Level` objects that assigns the laser to this transition.
         pulse (None or function or list): A time dependent function of the Rabi frequency of the laser OR a list of numbers describing a Rabi frequency pulse.
 
     Example:
 
         >>> Laser(1, 100, [Level([0]),Level([20])])
         The transition between Level([20]) and Level([0]) is assigned a laser with Rabi frequency of 1 and a frequency of 100.
+
+    Note:
+        Sort Level couples from low to high.
     """
 
     def __init__(self, rabifreq, frequency, couple, polarization=None, pulse=None):
         self.rabi = rabifreq
         self.couple = couple
         self.frequency = frequency
         self.polarization = polarization  # Not yet included. A list of a normalized E-field vector in the laser coordinate system, a theta_k and a theta_p (in degrees) and a pair [m_i,m_f].
@@ -114,15 +113,15 @@
         >>> level3 = Level([100])
         >>> laser1 = Laser(1, 120, [level1,level3])
         >>> laser2 = Laser(1, 100, [level2,level3])
         >>> decay = Decay([0],[[level3,level1]])
         >>> system = System([level1, level2, level3], [laser1,laser2], decay)
 
     Note:
-        Sort levels by energy in ascending order and Laser couples from low to high.
+        Sort levels by energy in ascending order.
     """
 
     def __init__(self, levels, lasers, decay):
         self.lasers = lasers
         self.levels = levels
         self.dim = len(levels)
         self.decay = decay
@@ -185,15 +184,15 @@
         delta_stark_shift=0,
         Diagonalization=True,
         plot_pop=True,
         Trotterintervals=500,
         resolution=250,
     ):
         """
-        An object that describes values for a laser: Rabi frequency, frequency, and coupled states.
+        A function to calculate the maximum population of the read_out_level
 
         Args:
             initial_state_index_list (list): value for :attr:`initial_state_index_list`
             read_out_level (number): value for :attr:`read_out_level`
             maxtime (integer): value for :attr:`maxtime`
             delta_stark_shift (number): value for :attr:`delta_stark_shift`
             Diagonalization (bool): value for :attr:`Diagonalization`
@@ -488,14 +487,15 @@
                             )
                         result[t + n * points_per_TI] = np.array(expect_value)
             result = np.array(
                 result
             )  # result[t] is a list of expectation values of all levels for the point of time that is indexed with t
             if plot_pop == True:
                 plot_population_diagonalization(tlist_ges[:], result[:], self.dim)
+            print("Maximum population of level {}:".format(read_out_level + 1))
             return np.real(np.amax(result[:, read_out_level]))
 
         elif Diagonalization == True:
             # Liouvillian
             L = qutip.liouvillian(H, c_ops)
             L = np.reshape(L, (self.dim**2, self.dim**2))
 
@@ -535,17 +535,18 @@
                     )
                 result[t] = np.array(np.reshape(expect_value, (self.dim,)))
             result = np.array(
                 result
             )  # result[t] is a list of expectation values of all levels for the point of time that is indexed with t
             if plot_pop == True:
                 plot_population_diagonalization(tlist, result, self.dim)
+            print("Maximum population of level {}:".format(read_out_level + 1))
             return np.real(np.amax(result[:, read_out_level]))
 
-        else:  # Integration-solver from QuTip
+        else:  # Integration-solver from QuTip. See QuTiP Documentation of the mesolve function.
             tlist = list(range(0, maxtime, int(41300000 / 100)))
             print("Length of tlist: {}".format(len(tlist)))
             # opts=Options(nsteps=1000)
             # print(options)
             # start = time.time()
             result = qutip.mesolve(H, initial_state_dm, tlist, c_ops, proj)
             # end = time.time()
```

### Comparing `atomcalc-0.1.0/pyproject.toml` & `atomcalc-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "atomcalc"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Moritz Wilke"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.5,<3.12"
 numpy = "^1.24.3"
 matplotlib = "^3.7.1"
-scipy = "1.9.1"
 qutip = "^4.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^6.2.1"
 sphinx-autobuild = "^2021.3.14"
 sphinx-rtd-theme = "^1.2.0"
```

