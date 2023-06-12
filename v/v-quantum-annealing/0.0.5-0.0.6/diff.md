# Comparing `tmp/v_quantum_annealing-0.0.5.tar.gz` & `tmp/v_quantum_annealing-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v_quantum_annealing-0.0.5.tar", last modified: Fri Jun  2 10:03:10 2023, max compression
+gzip compressed data, was "v_quantum_annealing-0.0.6.tar", last modified: Mon Jun 12 02:10:55 2023, max compression
```

## Comparing `v_quantum_annealing-0.0.5.tar` & `v_quantum_annealing-0.0.6.tar`

### file list

```diff
@@ -1,188 +1,183 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:10.143260 v_quantum_annealing-0.0.5/
--rw-rw-rw-   0        0        0     8974 2023-06-02 04:03:00.000000 v_quantum_annealing-0.0.5/CMakeLists.txt
--rw-rw-rw-   0        0        0       72 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11560 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1289 2023-05-27 18:46:55.000000 v_quantum_annealing-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1285 2023-06-02 10:03:10.144264 v_quantum_annealing-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     9339 2023-06-02 03:17:12.000000 v_quantum_annealing-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.547531 v_quantum_annealing-0.0.5/cmake/
--rw-rw-rw-   0        0        0     5390 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/cmake/FindGcov.cmake
--rw-rw-rw-   0        0        0    13074 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/cmake/FindLcov.cmake
--rw-rw-rw-   0        0        0     9299 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/cmake/Findcodecov.cmake
--rw-rw-rw-   0        0        0     4712 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.5/cmake/GenerateDocs.cmake
--rw-rw-rw-   0        0        0     2000 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/cmake/PythonAutoDetectOSX.cmake
--rw-rw-rw-   0        0        0     1129 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/cmake/llvm-cov-wrapper
--rw-rw-rw-   0        0        0     1257 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/doc-requirements.in
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.572465 v_quantum_annealing-0.0.5/external/
--rw-rw-rw-   0        0        0     1037 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/external/cimod.cmake
--rw-rw-rw-   0        0        0     1704 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.5/external/eigen.cmake
--rw-rw-rw-   0        0        0      724 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/external/googletest.cmake
--rw-rw-rw-   0        0        0      781 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/external/json.cmake
--rw-rw-rw-   0        0        0      465 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/external/pybind11-json.cmake
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.608370 v_quantum_annealing-0.0.5/include/
--rw-rw-rw-   0        0        0     2163 2023-06-01 15:38:26.000000 v_quantum_annealing-0.0.5/include/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.340085 v_quantum_annealing-0.0.5/include/v_quantum_annealing/
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.612359 v_quantum_annealing-0.0.5/include/v_quantum_annealing/algorithm/
--rw-rw-rw-   0        0        0     3244 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/algorithm/algorithm.hpp
--rw-rw-rw-   0        0        0      731 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/algorithm/all.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.638289 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/
--rw-rw-rw-   0        0        0     1154 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/all.hpp
--rw-rw-rw-   0        0        0     9658 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0    15482 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/chimera.hpp
--rw-rw-rw-   0        0        0      899 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/converter.hpp
--rw-rw-rw-   0        0        0     5269 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/csr_sparse.hpp
--rw-rw-rw-   0        0        0     7702 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/dense.hpp
--rw-rw-rw-   0        0        0     2615 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/graph.hpp
--rw-rw-rw-   0        0        0     9603 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/ising_polynomial_model.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.640284 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/json/
--rw-rw-rw-   0        0        0     4480 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/json/parse.hpp
--rw-rw-rw-   0        0        0    11232 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/polynomial.hpp
--rw-rw-rw-   0        0        0     8327 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/sparse.hpp
--rw-rw-rw-   0        0        0    10622 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/square.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.644272 v_quantum_annealing-0.0.5/include/v_quantum_annealing/result/
--rw-rw-rw-   0        0        0      731 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/result/all.hpp
--rw-rw-rw-   0        0        0     5217 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/result/get_solution.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.647264 v_quantum_annealing-0.0.5/include/v_quantum_annealing/sampler/
--rw-rw-rw-   0        0        0    10635 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/sampler/sa_sampler.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.718075 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/
--rw-rw-rw-   0        0        0     1152 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/CMakeLists.txt
--rw-rw-rw-   0        0        0     1410 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/all.hpp
--rw-rw-rw-   0        0        0     6308 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     7212 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/classical_ising.hpp
--rw-rw-rw-   0        0        0    21835 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/classical_ising_polynomial.hpp
--rw-rw-rw-   0        0        0    15181 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/continuous_time_ising.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.737028 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.743009 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_cuda/
--rw-rw-rw-   0        0        0     5615 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp
--rw-rw-rw-   0        0        0    14615 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu
--rw-rw-rw-   0        0        0     1750 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp
--rw-rw-rw-   0        0        0     2898 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp
--rw-rw-rw-   0        0        0    16618 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp
--rw-rw-rw-   0        0        0     5502 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0    24738 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/k_local_polynomial.hpp
--rw-rw-rw-   0        0        0      856 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/sa_system.hpp
--rw-rw-rw-   0        0        0     3417 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/system.hpp
--rw-rw-rw-   0        0        0    19954 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/transverse_ising.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.777915 v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/
--rw-rw-rw-   0        0        0     1089 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/all.hpp
--rw-rw-rw-   0        0        0    19616 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp
--rw-rw-rw-   0        0        0     5468 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/gpu.hpp
--rw-rw-rw-   0        0        0     3889 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/k_local.hpp
--rw-rw-rw-   0        0        0    13765 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/single_spin_flip.hpp
--rw-rw-rw-   0        0        0     6522 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/swendsen_wang.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.831771 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/
--rw-rw-rw-   0        0        0     1055 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/create_geometric_progression.hpp
--rw-rw-rw-   0        0        0     1179 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/disable_eigen_warning.hpp
--rw-rw-rw-   0        0        0     5958 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/eigen.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.835765 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/fmath/
--rw-rw-rw-   0        0        0    26304 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/fmath/fmath.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.854714 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/gpu/
--rw-rw-rw-   0        0        0     8427 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/gpu/cublas.hpp
--rw-rw-rw-   0        0        0     3061 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/gpu/handle_error.hpp
--rw-rw-rw-   0        0        0     2701 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/gpu/memory.hpp
--rw-rw-rw-   0        0        0     1102 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/index_type.hpp
--rw-rw-rw-   0        0        0     1337 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/insert_or_assign.hpp
--rw-rw-rw-   0        0        0     1118 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/memory.hpp
--rw-rw-rw-   0        0        0     3673 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/pairhash.hpp
--rw-rw-rw-   0        0        0     4054 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/random.hpp
--rw-rw-rw-   0        0        0    10636 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/schedule_list.hpp
--rw-rw-rw-   0        0        0      853 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/thres_hold.hpp
--rw-rw-rw-   0        0        0     2444 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/type_traits.hpp
--rw-rw-rw-   0        0        0     2309 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/union_find.hpp
--rw-rw-rw-   0        0        0     4681 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0     1578 2023-06-02 10:03:10.147251 v_quantum_annealing-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1423 2023-06-02 10:02:37.000000 v_quantum_annealing-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.877648 v_quantum_annealing-0.0.5/tests/
--rw-rw-rw-   0        0        0     1756 2023-05-28 17:40:55.000000 v_quantum_annealing-0.0.5/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0        0 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.5/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.928835 v_quantum_annealing-0.0.5/tests/__pycache__/
--rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.5/tests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    13004 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.5/tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.5/tests/__pycache__/test_gpu.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    34580 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.5/tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     5551 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.5/tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     8200 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.5/tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     1848 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.5/tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     2147 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.5/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.948780 v_quantum_annealing-0.0.5/tests/cxxtest/
--rw-rw-rw-   0        0        0     1979 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/cxxtest.cpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.957756 v_quantum_annealing-0.0.5/tests/cxxtest/graph/
--rw-rw-rw-   0        0        0      809 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/graph/all.hpp
--rw-rw-rw-   0        0        0     6134 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/graph/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0     5917 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/graph/ising_polynomial_model.hpp
--rw-rw-rw-   0        0        0     4604 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/graph/polynomial.hpp
--rw-rw-rw-   0        0        0     7083 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/graph/quadratic.hpp
--rw-rw-rw-   0        0        0    39029 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/polynomial_test.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.961745 v_quantum_annealing-0.0.5/tests/cxxtest/result/
--rw-rw-rw-   0        0        0      700 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/result/all.hpp
--rw-rw-rw-   0        0        0     2777 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/result/result.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:10.029563 v_quantum_annealing-0.0.5/tests/cxxtest/sampler/
--rw-rw-rw-   0        0        0      891 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/sampler/all.hpp
--rw-rw-rw-   0        0        0     2441 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     3200 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/sampler/gpu.hpp
--rw-rw-rw-   0        0        0     2429 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     4313 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/sampler/k_local.hpp
--rw-rw-rw-   0        0        0     5337 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/sampler/polynomial.hpp
--rw-rw-rw-   0        0        0     6406 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/sampler/quadraitc.hpp
--rw-rw-rw-   0        0        0     6808 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/sampler/swendsen_wang.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:10.059485 v_quantum_annealing-0.0.5/tests/cxxtest/system/
--rw-rw-rw-   0        0        0      861 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/system/all.hpp
--rw-rw-rw-   0        0        0     7840 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/system/binary_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     1390 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/system/classical_ising.hpp
--rw-rw-rw-   0        0        0     4090 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/system/classical_ising_polynomial.hpp
--rw-rw-rw-   0        0        0     9332 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/system/ising_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     2447 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/system/k_local.hpp
--rw-rw-rw-   0        0        0    15804 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/testcase.hpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:10.066470 v_quantum_annealing-0.0.5/tests/cxxtest/utility/
--rw-rw-rw-   0        0        0      744 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/utility/all.hpp
--rw-rw-rw-   0        0        0     3829 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/utility/eigen.hpp
--rw-rw-rw-   0        0        0     6403 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/utility/gpu.hpp
--rw-rw-rw-   0        0        0     1965 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/tests/cxxtest/utility/union_find.hpp
--rw-rw-rw-   0        0        0    28004 2023-05-29 03:26:14.000000 v_quantum_annealing-0.0.5/tests/test_cxx.py
--rw-rw-rw-   0        0        0     5754 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.5/tests/test_gpu.py
--rw-rw-rw-   0        0        0    60920 2023-05-29 03:36:19.000000 v_quantum_annealing-0.0.5/tests/test_hubo.py
--rw-rw-rw-   0        0        0     6313 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.5/tests/test_model.py
--rw-rw-rw-   0        0        0    10119 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.5/tests/test_sampler.py
--rw-rw-rw-   0        0        0     1181 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.5/tests/test_sqa.py
--rw-rw-rw-   0        0        0     1973 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.5/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:10.075441 v_quantum_annealing-0.0.5/v_quantum_annealing/
--rw-rw-rw-   0        0        0     2240 2023-05-28 17:40:55.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/CMakeLists.txt
--rw-rw-rw-   0        0        0     1086 2023-06-01 15:38:26.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/__init__.py
--rw-rw-rw-   0        0        0      215 2023-06-01 10:54:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/_version.py
--rw-rw-rw-   0        0        0     2988 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/compile_config.hpp
--rw-rw-rw-   0        0        0    44951 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/declare.hpp
--rw-rw-rw-   0        0        0    15576 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/main.cpp
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.426854 v_quantum_annealing-0.0.5/v_quantum_annealing/model/
--rw-rw-rw-   0        0        0      887 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/model/__init__.py
--rw-rw-rw-   0        0        0    14286 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/model/chimera_model.py
--rw-rw-rw-   0        0        0     9035 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/model/king_graph.py
--rw-rw-rw-   0        0        0    23582 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/model/model.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.463755 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/
--rw-rw-rw-   0        0        0      529 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/__init__.py
--rw-rw-rw-   0        0        0     4272 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/base_sa_sample_hubo.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.498662 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/chimera_gpu/
--rw-rw-rw-   0        0        0      320 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/chimera_gpu/__init__.py
--rw-rw-rw-   0        0        0     2363 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
--rw-rw-rw-   0        0        0     5010 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
--rw-rw-rw-   0        0        0     5847 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
--rw-rw-rw-   0        0        0     5240 2023-05-28 14:52:35.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/csqa_sampler.py
--rw-rw-rw-   0        0        0     1124 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/response.py
--rw-rw-rw-   0        0        0    25532 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/sa_sampler.py
--rw-rw-rw-   0        0        0     8979 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/sampler.py
--rw-rw-rw-   0        0        0    12920 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/sqa_sampler.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:09.534566 v_quantum_annealing-0.0.5/v_quantum_annealing/utils/
--rw-rw-rw-   0        0        0      767 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/utils/__init__.py
--rw-rw-rw-   0        0        0    10152 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/utils/benchmark.py
--rw-rw-rw-   0        0        0     1283 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/utils/cxx_cast.py
--rw-rw-rw-   0        0        0      855 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/utils/decorator.py
--rw-rw-rw-   0        0        0      992 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/utils/graph_utils.py
--rw-rw-rw-   0        0        0     2120 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/utils/res_convertor.py
--rw-rw-rw-   0        0        0       36 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/utils/time_measure.py
--rw-rw-rw-   0        0        0     1010 2023-06-02 03:16:31.000000 v_quantum_annealing-0.0.5/v_quantum_annealing/variable_type.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:03:10.135281 v_quantum_annealing-0.0.5/v_quantum_annealing.egg-info/
--rw-rw-rw-   0        0        0     1285 2023-06-02 10:03:09.000000 v_quantum_annealing-0.0.5/v_quantum_annealing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7553 2023-06-02 10:03:09.000000 v_quantum_annealing-0.0.5/v_quantum_annealing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 10:03:09.000000 v_quantum_annealing-0.0.5/v_quantum_annealing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 08:08:59.000000 v_quantum_annealing-0.0.5/v_quantum_annealing.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      130 2023-06-02 10:03:09.000000 v_quantum_annealing-0.0.5/v_quantum_annealing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-02 10:03:09.000000 v_quantum_annealing-0.0.5/v_quantum_annealing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.452574 v_quantum_annealing-0.0.6/
+-rw-rw-rw-   0        0        0     9483 2023-06-10 04:35:48.000000 v_quantum_annealing-0.0.6/CMakeLists.txt
+-rw-rw-rw-   0        0        0    11560 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1289 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1278 2023-06-12 02:10:55.457562 v_quantum_annealing-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9339 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.124024 v_quantum_annealing-0.0.6/cmake/
+-rw-rw-rw-   0        0        0     5390 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/FindGcov.cmake
+-rw-rw-rw-   0        0        0    13074 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/FindLcov.cmake
+-rw-rw-rw-   0        0        0     9299 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/Findcodecov.cmake
+-rw-rw-rw-   0        0        0     4712 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/GenerateDocs.cmake
+-rw-rw-rw-   0        0        0     2000 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/PythonAutoDetectOSX.cmake
+-rw-rw-rw-   0        0        0     1129 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/llvm-cov-wrapper
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.159496 v_quantum_annealing-0.0.6/external/
+-rw-rw-rw-   0        0        0     1025 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/external/cimod.cmake
+-rw-rw-rw-   0        0        0     1976 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/external/eigen.cmake
+-rw-rw-rw-   0        0        0     1043 2023-06-09 10:10:49.000000 v_quantum_annealing-0.0.6/external/googletest.cmake
+-rw-rw-rw-   0        0        0      781 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/external/json.cmake
+-rw-rw-rw-   0        0        0      465 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/external/pybind11-json.cmake
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.166440 v_quantum_annealing-0.0.6/include/
+-rw-rw-rw-   0        0        0     2243 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:53.777366 v_quantum_annealing-0.0.6/include/v_quantum_annealing/
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.178408 v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/
+-rw-rw-rw-   0        0        0     3244 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/algorithm.hpp
+-rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/all.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.227277 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/
+-rw-rw-rw-   0        0        0    45689 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0    68880 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/binary_quadratic_model.hpp
+-rw-rw-rw-   0        0        0    42393 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp
+-rw-rw-rw-   0        0        0     1158 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/disable_eigen_warning.hpp
+-rw-rw-rw-   0        0        0     2684 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/hash.hpp
+-rw-rw-rw-   0        0        0      654 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/json.hpp
+-rw-rw-rw-   0        0        0     4884 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/utilities.hpp
+-rw-rw-rw-   0        0        0     1624 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/vartypes.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.303066 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/
+-rw-rw-rw-   0        0        0     1154 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/all.hpp
+-rw-rw-rw-   0        0        0     9658 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0    15482 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/chimera.hpp
+-rw-rw-rw-   0        0        0      899 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/converter.hpp
+-rw-rw-rw-   0        0        0     5269 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/csr_sparse.hpp
+-rw-rw-rw-   0        0        0     7702 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/dense.hpp
+-rw-rw-rw-   0        0        0     2615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/graph.hpp
+-rw-rw-rw-   0        0        0     9603 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/ising_polynomial_model.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.306057 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/json/
+-rw-rw-rw-   0        0        0     4569 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/json/parse.hpp
+-rw-rw-rw-   0        0        0    11286 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     8327 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/sparse.hpp
+-rw-rw-rw-   0        0        0    10622 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/square.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.311045 v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/
+-rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/all.hpp
+-rw-rw-rw-   0        0        0     5217 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/get_solution.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.318049 v_quantum_annealing-0.0.6/include/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0    10635 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/sampler/sa_sampler.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.406788 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/
+-rw-rw-rw-   0        0        0     1410 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/all.hpp
+-rw-rw-rw-   0        0        0     6308 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     7264 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0    21835 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0    15181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/continuous_time_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.423742 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.439710 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/
+-rw-rw-rw-   0        0        0     5615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp
+-rw-rw-rw-   0        0        0    14615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu
+-rw-rw-rw-   0        0        0     1750 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp
+-rw-rw-rw-   0        0        0     2898 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp
+-rw-rw-rw-   0        0        0    16618 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp
+-rw-rw-rw-   0        0        0     5502 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0    24738 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/k_local_polynomial.hpp
+-rw-rw-rw-   0        0        0      856 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/sa_system.hpp
+-rw-rw-rw-   0        0        0     3417 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/system.hpp
+-rw-rw-rw-   0        0        0    19954 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/transverse_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.603263 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/
+-rw-rw-rw-   0        0        0     1089 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/all.hpp
+-rw-rw-rw-   0        0        0    19616 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp
+-rw-rw-rw-   0        0        0     5468 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/gpu.hpp
+-rw-rw-rw-   0        0        0     3889 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/k_local.hpp
+-rw-rw-rw-   0        0        0    13765 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/single_spin_flip.hpp
+-rw-rw-rw-   0        0        0     6522 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.718960 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/
+-rw-rw-rw-   0        0        0     1055 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/create_geometric_progression.hpp
+-rw-rw-rw-   0        0        0     1179 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/disable_eigen_warning.hpp
+-rw-rw-rw-   0        0        0     5958 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/eigen.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.728931 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/fmath/
+-rw-rw-rw-   0        0        0    26304 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/fmath/fmath.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.763833 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/
+-rw-rw-rw-   0        0        0     8427 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/cublas.hpp
+-rw-rw-rw-   0        0        0     3061 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/handle_error.hpp
+-rw-rw-rw-   0        0        0     2701 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/memory.hpp
+-rw-rw-rw-   0        0        0     1102 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/index_type.hpp
+-rw-rw-rw-   0        0        0     1337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/insert_or_assign.hpp
+-rw-rw-rw-   0        0        0     1118 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/memory.hpp
+-rw-rw-rw-   0        0        0     3673 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/pairhash.hpp
+-rw-rw-rw-   0        0        0     4054 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/random.hpp
+-rw-rw-rw-   0        0        0    10636 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/schedule_list.hpp
+-rw-rw-rw-   0        0        0      853 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/thres_hold.hpp
+-rw-rw-rw-   0        0        0     2444 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/type_traits.hpp
+-rw-rw-rw-   0        0        0     2309 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/union_find.hpp
+-rw-rw-rw-   0        0        0     4681 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1578 2023-06-12 02:10:55.501444 v_quantum_annealing-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1423 2023-06-12 02:10:11.000000 v_quantum_annealing-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.968287 v_quantum_annealing-0.0.6/tests/
+-rw-rw-rw-   0        0        0     2064 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.980254 v_quantum_annealing-0.0.6/tests/cxxtest/
+-rw-rw-rw-   0        0        0     1979 2023-06-10 10:04:30.000000 v_quantum_annealing-0.0.6/tests/cxxtest/cxxtest.cpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.004190 v_quantum_annealing-0.0.6/tests/cxxtest/graph/
+-rw-rw-rw-   0        0        0      809 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/all.hpp
+-rw-rw-rw-   0        0        0     6134 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     5917 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/ising_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     4663 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     7083 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/quadratic.hpp
+-rw-rw-rw-   0        0        0    39029 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/polynomial_test.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.062036 v_quantum_annealing-0.0.6/tests/cxxtest/result/
+-rw-rw-rw-   0        0        0      700 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/result/all.hpp
+-rw-rw-rw-   0        0        0     2777 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/result/result.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.103928 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/
+-rw-rw-rw-   0        0        0      891 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/all.hpp
+-rw-rw-rw-   0        0        0     2441 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     3200 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/gpu.hpp
+-rw-rw-rw-   0        0        0     2429 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     4313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/k_local.hpp
+-rw-rw-rw-   0        0        0     5337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/polynomial.hpp
+-rw-rw-rw-   0        0        0     6406 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/quadraitc.hpp
+-rw-rw-rw-   0        0        0     6808 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.185718 v_quantum_annealing-0.0.6/tests/cxxtest/system/
+-rw-rw-rw-   0        0        0      861 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/all.hpp
+-rw-rw-rw-   0        0        0     7840 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     1390 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0     4090 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0     9332 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     2447 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/k_local.hpp
+-rw-rw-rw-   0        0        0    15821 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/tests/cxxtest/testcase.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.296990 v_quantum_annealing-0.0.6/tests/cxxtest/utility/
+-rw-rw-rw-   0        0        0      744 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/utility/all.hpp
+-rw-rw-rw-   0        0        0     3829 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/utility/eigen.hpp
+-rw-rw-rw-   0        0        0     6403 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/utility/gpu.hpp
+-rw-rw-rw-   0        0        0     1965 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/utility/union_find.hpp
+-rw-rw-rw-   0        0        0    28004 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_cxx.py
+-rw-rw-rw-   0        0        0     5754 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_gpu.py
+-rw-rw-rw-   0        0        0    60920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_hubo.py
+-rw-rw-rw-   0        0        0     6313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_model.py
+-rw-rw-rw-   0        0        0    10119 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_sampler.py
+-rw-rw-rw-   0        0        0     1181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_sqa.py
+-rw-rw-rw-   0        0        0     1973 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.341877 v_quantum_annealing-0.0.6/v_quantum_annealing/
+-rw-rw-rw-   0        0        0     1086 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/__init__.py
+-rw-rw-rw-   0        0        0     2988 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/compile_config.hpp
+-rw-rw-rw-   0        0        0    44951 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/declare.hpp
+-rw-rw-rw-   0        0        0    15576 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/main.cpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:53.972430 v_quantum_annealing-0.0.6/v_quantum_annealing/model/
+-rw-rw-rw-   0        0        0      887 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/model/__init__.py
+-rw-rw-rw-   0        0        0    14286 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/model/chimera_model.py
+-rw-rw-rw-   0        0        0     9035 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/model/king_graph.py
+-rw-rw-rw-   0        0        0    23582 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/model/model.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.042243 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0      529 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/__init__.py
+-rw-rw-rw-   0        0        0     4272 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/base_sa_sample_hubo.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.064189 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/
+-rw-rw-rw-   0        0        0      320 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/__init__.py
+-rw-rw-rw-   0        0        0     2363 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
+-rw-rw-rw-   0        0        0     5010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
+-rw-rw-rw-   0        0        0     5847 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
+-rw-rw-rw-   0        0        0     5240 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/csqa_sampler.py
+-rw-rw-rw-   0        0        0     1124 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/response.py
+-rw-rw-rw-   0        0        0    25532 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sa_sampler.py
+-rw-rw-rw-   0        0        0     8979 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sampler.py
+-rw-rw-rw-   0        0        0    12920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sqa_sampler.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.098100 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/
+-rw-rw-rw-   0        0        0      767 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10152 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/benchmark.py
+-rw-rw-rw-   0        0        0     1283 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/cxx_cast.py
+-rw-rw-rw-   0        0        0      855 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/decorator.py
+-rw-rw-rw-   0        0        0      992 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/graph_utils.py
+-rw-rw-rw-   0        0        0     2120 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/res_convertor.py
+-rw-rw-rw-   0        0        0       36 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/time_measure.py
+-rw-rw-rw-   0        0        0     1010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/variable_type.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.403711 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/
+-rw-rw-rw-   0        0        0     1278 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7360 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-12 02:10:08.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      130 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/top_level.txt
```

### Comparing `v_quantum_annealing-0.0.5/CMakeLists.txt` & `v_quantum_annealing-0.0.6/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,34 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-cmake_minimum_required(VERSION 3.22 FATAL_ERROR)
+cmake_minimum_required(VERSION 3.26 FATAL_ERROR)
 project(v_quantum_annealing
     DESCRIPTION "Framework for the Ising model and QUBO."
     HOMEPAGE_URL "https://v-quantum-technology.com"
 )
+cmake_minimum_required(VERSION 3.0)
+project(myproject)
+
+cmake_policy(SET CMP0079 NEW)
+cmake_policy(SET CMP0002 NEW)
+
+find_package(Eigen3 REQUIRED)
+if(Eigen3_FOUND)
+    message("Eigen3 found")
+    include_directories(${Eigen3_INCLUDE_DIRS})
+    # ...
+else()
+    message("Eigen3 not found")
+endif()
+
 
 # Standard includes
 include(CheckLanguage)
 
 set(V_QUANTUM_ANNEALING_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/include)
 
 if (CMAKE_CURRENT_SOURCE_DIR STREQUAL CMAKE_SOURCE_DIR)
@@ -192,41 +207,51 @@
   else() 
     message(STATUS "OMP_FOUND = NO")
     message(STATUS "USE_OMP = OFF")
     set(USE_OMP OFF)
   endif()
 endif()
 
-find_package(Eigen3 CONFIG)
 
-if(EIGEN3_FOUND)
-  message(STATUS "Skip Download eigen3")
-else() 
-  message(STATUS "Downlod eigen3")
-  include(external/eigen.cmake)
-endif() 
+
+# find_package(Eigen3 CONFIG)
+# if(EIGEN3_FOUND)
+#   message(STATUS "Skip Download eigen3")
+# else() 
+#   message(STATUS "Downlod eigen3")
+#   include(external/eigen.cmake)
+# endif() 
+
+
+
 
 find_package(nlohmann_json CONFIG)
 if(TARGET nlohmann_json::nlohmann_json)
   message(STATUS "Skip Download nlohmann_json")
 else()
   message(STATUS "Downlod nlohmann_json")
   set(JSON_BuildTests OFF CACHE INTERNAL "")
   include(external/json.cmake)
 endif()
 
+
+
+
 find_package(cxxcimod_header_only CONFIG)
 if(TARGET cxxcimod_header_only)
   message(STATUS "Skip Download cimod")
 else()
   message(STATUS "Fetch cimod")
   include(external/cimod.cmake)
 endif()
 
+
 add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/include)
+message(STATUS "------------End check error here----------------------------")
+
 
 # Build Python Extension 
 if(SKBUILD AND V_QUANTUM_ANNEALING_MAIN_PROJECT)
   message(STATUS "Build Python Extension.")
   option(WITH_THREAD "Compile in rudimentary thread support" ON)
   option(BUILD_TESTING "Enable CTest support." OFF)
   find_package(Python3 COMPONENTS Interpreter Development NumPy)
@@ -263,15 +288,18 @@
   endif()
   
   message(STATUS "Use Googletest") 
   message(STATUS "Downlod Googletest")
   include(external/googletest.cmake)
   
   enable_testing()
-  
+
+  message(STATUS "End Downlod Googletest")
+  message(STATUS "End Use Googletest")
+
   add_subdirectory(tests)
   
   if(ENABLE_COVERAGE AND (NOT MSVC))
      coverage_evaluate()
   endif()
 endif()
```

### Comparing `v_quantum_annealing-0.0.5/LICENSE` & `v_quantum_annealing-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/MANIFEST.in` & `v_quantum_annealing-0.0.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/PKG-INFO` & `v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
-Name: v_quantum_annealing
-Version: 0.0.5
+Name: v-quantum-annealing
+Version: 0.0.6
 Summary: "Framework for the Ising model and QUBO."
 Home-page: https://v-quantum-technology.com
 Author: V-QUANTUM JSC
 Author-email: nqthinh@v-quantum-technology.com
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/v-quantum-jsc/V-QUANTUM-ANNEALING
 Project-URL: Documentation, https://v_quantum_annealing.github.io/v_quantum_annealing
 Project-URL: Reference, https://ref.v_quantum_annealing.org/index.html
-Description: "file: README.md"
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,7 +20,10 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+"file: README.md"
```

### Comparing `v_quantum_annealing-0.0.5/README.md` & `v_quantum_annealing-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/cmake/FindGcov.cmake` & `v_quantum_annealing-0.0.6/cmake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/cmake/FindLcov.cmake` & `v_quantum_annealing-0.0.6/cmake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/cmake/Findcodecov.cmake` & `v_quantum_annealing-0.0.6/cmake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/cmake/GenerateDocs.cmake` & `v_quantum_annealing-0.0.6/cmake/GenerateDocs.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/cmake/PythonAutoDetectOSX.cmake` & `v_quantum_annealing-0.0.6/cmake/PythonAutoDetectOSX.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/cmake/llvm-cov-wrapper` & `v_quantum_annealing-0.0.6/cmake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/external/cimod.cmake` & `v_quantum_annealing-0.0.6/external/cimod.cmake`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 set(FETCHCONTENT_QUIET OFF)
 
 
 #### Cimod ####
 FetchContent_Declare(
     cimod
-    GIT_REPOSITORY  https://github.com/v_quantum_annealing/cimod
+    GIT_REPOSITORY  https://github.com/openjij/cimod
     GIT_TAG         v1.4.54
     GIT_SHALLOW     TRUE
     )
 
 FetchContent_MakeAvailable(cimod)
```

### Comparing `v_quantum_annealing-0.0.5/external/eigen.cmake` & `v_quantum_annealing-0.0.6/external/eigen.cmake`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #set(EIGEN_BUILD_SHARED_LIBS OFF CACHE BOOL "" FORCE)
 
 if(MSVC)
   set(EIGEN_Fortran_COMPILER_WORKS OFF CACHE BOOL "" FORCE)
 endif()
 
 if(BLAS_FOUND) 
+  message(STATUS "------FOUND BLAS PACKAGE -------------")
   set(EIGEN_USE_BLAS ON) 
 endif()
 
 if(LAPACK_FOUND) 
   set(EIGEN_USE_LAPACKE ON)
 endif()
 
@@ -35,14 +36,20 @@
     GIT_REPOSITORY  https://gitlab.com/libeigen/eigen
     GIT_TAG         3.4.0
     GIT_SHALLOW     TRUE
     )
 
 FetchContent_MakeAvailable(eigen3)
 
+
+
+#TUDN CHANGE add_library = add_subdirectory
+message(STATUS  "-----eigen_source_dir= ${EIGEN3_SOURCE_DIR} --------")
+message(STATUS  "-----CMAKE_CURRENT_BINARY_DIR= ${CMAKE_CURRENT_BINARY_DIR} --------")
+
 add_library(v_quantum_annealing-eigen_lib INTERFACE)
 target_include_directories(v_quantum_annealing-eigen_lib INTERFACE ${eigen_SOURCE_DIR})
 target_compile_definitions(v_quantum_annealing-eigen_lib INTERFACE 
     EIGEN_MPL2_ONLY
     BUILD_TESTING=OFF
     TEST_LIB=OFF
     EIGEN_BUILD_PKGCONFIG=OFF
```

### Comparing `v_quantum_annealing-0.0.5/external/googletest.cmake` & `v_quantum_annealing-0.0.6/external/googletest.cmake`

 * *Files 21% similar despite different names*

```diff
@@ -16,17 +16,28 @@
 
 if(WIN32)
   set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
 endif()
 
 FetchContent_MakeAvailable(googletest)
 
+
+#set gtest library
+set(GTEST_INCLUDE_DIR ${gtest_SOURCE_DIR}/include)
+set(GTEST_LIBRARY ${CMAKE_CURRENT_SOURCE_DIR}/lib/gtest.lib)
+set(GTEST_MAIN_LIBRARY ${CMAKE_CURRENT_SOURCE_DIR}/lib/gtest_main.lib)
+
+# message(STATUS "CMAKE_CURRENT_SOURCE_DIR = ${CMAKE_CURRENT_SOURCE_DIR}")
+#end set gtest library
+
 find_package(GTest)
 
-#FetchContent_GetProperties(googletest)
+# FetchContent_GetProperties(googletest)
+
+# message(STATUS "gtest_SOURCE_DIR = ${gtest_SOURCE_DIR}")
+# message(STATUS "gmock_SOURCE_DIR = ${gmock_SOURCE_DIR}")
+
 
-#message(STATUS "gtest_SOURCE_DIR = ${gtest_SOURCE_DIR}")
-#message(STATUS "gmock_SOURCE_DIR = ${gmock_SOURCE_DIR}")
 
 
 list(POP_BACK CMAKE_MESSAGE_INDENT)
 message(CHECK_PASS "fetched")
```

### Comparing `v_quantum_annealing-0.0.5/external/json.cmake` & `v_quantum_annealing-0.0.6/external/json.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/CMakeLists.txt` & `v_quantum_annealing-0.0.6/include/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 #) 
 
 #for GPU
 if(CUDAToolkit_FOUND)
     add_subdirectory(openjij/system)
 endif()
 
+#TUDN CHANGE OPENJIJ_INCLUDE_DIR = V_QUANTUM_ANNEALING_INCLUDE_DIR
 target_include_directories(cxxjij_header_only INTERFACE 
-  $<BUILD_INTERFACE:${OPENJIJ_INCLUDE_DIR}>
+  $<BUILD_INTERFACE:${V_QUANTUM_ANNEALING_INCLUDE_DIR}>
   $<INSTALL_INTERFACE:include>
 )
 
 target_link_libraries(cxxjij_header_only INTERFACE 
     cxxcimod_header_only
     nlohmann_json::nlohmann_json
     $<IF:$<TARGET_EXISTS:Eigen3::Eigen>,Eigen3::Eigen,openjij-eigen_lib>
```

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/algorithm/algorithm.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/algorithm/all.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/all.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/chimera.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/chimera.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/converter.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/converter.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/csr_sparse.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/csr_sparse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/dense.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/dense.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/graph.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/graph.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/ising_polynomial_model.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/json/parse.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/json/parse.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 #include <exception>
 #include <tuple>
 #include <vector>
 #include <numeric>
 
 #include <nlohmann/json.hpp>
-
-#include <cimod/binary_polynomial_model.hpp>
-#include <cimod/binary_quadratic_model.hpp>
-#include <cimod/binary_quadratic_model_dict.hpp>
+// TUDN Fix loi include cimod
+#include <v_quantum_annealing/cimod/binary_polynomial_model.hpp>
+#include <v_quantum_annealing/cimod/binary_quadratic_model.hpp>
+#include <v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp>
 
 #include "v_quantum_annealing/graph/graph.hpp"
 
 namespace v_quantum_annealing {
 namespace graph {
 
 using json = nlohmann::json;
```

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/polynomial.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/polynomial.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 #include <algorithm>
 #include <cassert>
 #include <cstddef>
 #include <type_traits>
 #include <unordered_map>
 #include <utility>
 
-#include <cimod/binary_polynomial_model.hpp>
+// tudn add v_quantum_annealing/
+#include <v_quantum_annealing/cimod/binary_polynomial_model.hpp>
 
 #include "v_quantum_annealing/graph/graph.hpp"
 #include "v_quantum_annealing/graph/json/parse.hpp"
 #include "v_quantum_annealing/utility/index_type.hpp"
 #include "v_quantum_annealing/utility/pairhash.hpp"
 
 namespace v_quantum_annealing {
```

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/sparse.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/sparse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/graph/square.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/square.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/result/all.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/result/get_solution.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/get_solution.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/sampler/sa_sampler.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/sampler/sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/all.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/classical_ising.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/classical_ising.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 #include <cassert>
 #include <type_traits>
 #include <utility>
 
 #include <Eigen/Dense>
 #include <Eigen/Sparse>
-
-#include <cimod/utilities.hpp>
+// TUDN add v_quantum_annealing/
+#include <v_quantum_annealing/cimod/utilities.hpp>
 
 #include "v_quantum_annealing/graph/all.hpp"
 #include "v_quantum_annealing/system/system.hpp"
 #include "v_quantum_annealing/utility/eigen.hpp"
 
 namespace v_quantum_annealing {
 namespace system {
```

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/classical_ising_polynomial.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/continuous_time_ising.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/continuous_time_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/k_local_polynomial.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/k_local_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/sa_system.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/system.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/system/transverse_ising.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/transverse_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/all.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/gpu.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/k_local.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/single_spin_flip.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/single_spin_flip.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/updater/swendsen_wang.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/create_geometric_progression.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/create_geometric_progression.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/disable_eigen_warning.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/disable_eigen_warning.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/eigen.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/fmath/fmath.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/fmath/fmath.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/gpu/cublas.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/cublas.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/gpu/handle_error.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/handle_error.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/gpu/memory.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/memory.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/index_type.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/index_type.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/insert_or_assign.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/insert_or_assign.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/memory.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/memory.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/pairhash.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/pairhash.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/random.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/random.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/schedule_list.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/schedule_list.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/thres_hold.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/thres_hold.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/type_traits.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/include/v_quantum_annealing/utility/union_find.hpp` & `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/pyproject.toml` & `v_quantum_annealing-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/setup.cfg` & `v_quantum_annealing-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 00000140: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000150: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
 00000160: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
 00000170: 0a6c 6963 656e 7365 5f66 696c 6573 203d  .license_files =
 00000180: 204c 4943 454e 5345 0d0a 6c69 6365 6e73   LICENSE..licens
 00000190: 6520 3d20 2241 7061 6368 6520 4c69 6365  e = "Apache Lice
 000001a0: 6e73 6520 322e 3022 0d0a 7665 7273 696f  nse 2.0"..versio
-000001b0: 6e20 3d20 2230 2e30 2e35 220d 0a63 6c61  n = "0.0.5"..cla
+000001b0: 6e20 3d20 2230 2e30 2e36 220d 0a63 6c61  n = "0.0.6"..cla
 000001c0: 7373 6966 6965 7273 203d 200d 0a09 4c69  ssifiers = ...Li
 000001d0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
 000001e0: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
 000001f0: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
 00000200: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
 00000210: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
 00000220: 5265 7365 6172 6368 0d0a 0950 726f 6772  Research...Progr
```

### Comparing `v_quantum_annealing-0.0.5/setup.py` & `v_quantum_annealing-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 setup_requires = [
     "numpy",
     "pybind11 >=2.10.0, < 2.11.0",
     "cmake > 3.20",
     "scikit-build > 0.16.0"
 ]
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 setup(
     name="v_quantum_annealing", 
     version=__version__,  
     author = "V-QUANTUM JSC",
     author_email = "nqthinh@v-quantum-technology.com",
     setup_requires=setup_requires,
```

### Comparing `v_quantum_annealing-0.0.5/tests/CMakeLists.txt` & `v_quantum_annealing-0.0.6/tests/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 #include(GoogleTest)
 
+
+
+# target_include_directories(cxxvqa_test PUBLIC ${V_QUANTUM_ANNEALING_INCLUDE_DIR})
+
 add_executable(cxxvqa_test
     cxxtest/cxxtest.cpp
 )
+# TUDN add target include directory to fix issue of not found library
+target_include_directories(cxxvqa_test PUBLIC
+  ${CMAKE_SOURCE_DIR}/src
+  ${CMAKE_SOURCE_DIR}/include
+ )
 
 if(ENABLE_COVERAGE AND (NOT MSVC))
   add_coverage(cxxvqa_test)
 endif()
 
 if(CUDAToolkit_FOUND)
     set_target_properties(cxxvqa_test PROPERTIES
@@ -38,15 +47,16 @@
 
 target_compile_definitions(cxxvqa_test PRIVATE
     BUILD_TESTING=OFF
 )
 
 target_link_libraries(cxxvqa_test PRIVATE
     nlohmann_json::nlohmann_json
-    cxxvqa_header_only
+    # #tudn remove header onlylib
+    # cxxvqa_header_only
     $<IF:$<TARGET_EXISTS:Eigen3::Eigen>,Eigen3::Eigen,openjij-eigen_lib>
     $<IF:$<TARGET_EXISTS:GTest::gtest>,GTest::gtest,gtest>
     $<IF:$<TARGET_EXISTS:GTest::gtest_main>,GTest::gtest_main,gtest_main>
     $<IF:$<TARGET_EXISTS:GTest::gmock>,GTest::gmock,gmock>
     $<IF:$<TARGET_EXISTS:GTest::gmock_main>,GTest::gmock_main,gmock_main>
     $<$<TARGET_EXISTS:cxxvqa_chimera_gpu_kernel>:cxxvqa_chimera_gpu_kernel>
 )
```

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/cxxtest.cpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/cxxtest.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/graph/all.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/graph/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/graph/ising_polynomial_model.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/graph/polynomial.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/graph/polynomial.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 //    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 
 
 #pragma once
-
+// tudn add test include
+#include "../polynomial_test.hpp"
 
 namespace v_quantum_annealing {
 namespace test {
 
 
 TEST(PolyGraph, ConstructorCimodDenseInt) {
    TestPolyGraphConstructorCimodDense<v_quantum_annealing::graph::Index, double>(GeneratePolynomialInteractionsDenseInt<double>());
```

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/graph/quadratic.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/graph/quadratic.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/polynomial_test.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/polynomial_test.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/result/all.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/result/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/result/result.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/result/result.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/sampler/all.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/sampler/gpu.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/sampler/k_local.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/sampler/polynomial.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/sampler/quadraitc.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/quadraitc.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/sampler/swendsen_wang.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/system/all.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/system/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/system/binary_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/system/classical_ising.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/system/classical_ising_polynomial.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/system/ising_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/system/k_local.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/system/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/testcase.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/testcase.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 //    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 
 #pragma once
 
-#include "v_quantum_annealing/graph/all.hpp"
+//v_quantum_annealing/graph/all.hpp
+#include "graph/all.hpp"
 #include <iostream>
 #include <bitset>
 
 static constexpr std::size_t num_system_size = 8;
 
 static v_quantum_annealing::utility::ClassicalScheduleList generate_schedule_list(){
     return v_quantum_annealing::utility::make_classical_schedule_list(0.1, 100.0, 100, 100);
```

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/utility/all.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/utility/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/utility/eigen.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/utility/gpu.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/utility/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/cxxtest/utility/union_find.hpp` & `v_quantum_annealing-0.0.6/tests/cxxtest/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/test_cxx.py` & `v_quantum_annealing-0.0.6/tests/test_cxx.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/test_gpu.py` & `v_quantum_annealing-0.0.6/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/test_hubo.py` & `v_quantum_annealing-0.0.6/tests/test_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/test_model.py` & `v_quantum_annealing-0.0.6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/test_sampler.py` & `v_quantum_annealing-0.0.6/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/test_sqa.py` & `v_quantum_annealing-0.0.6/tests/test_sqa.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/tests/test_utils.py` & `v_quantum_annealing-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/__init__.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/compile_config.hpp` & `v_quantum_annealing-0.0.6/v_quantum_annealing/compile_config.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/declare.hpp` & `v_quantum_annealing-0.0.6/v_quantum_annealing/declare.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/main.cpp` & `v_quantum_annealing-0.0.6/v_quantum_annealing/main.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/model/__init__.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/model/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/model/chimera_model.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/model/chimera_model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/model/king_graph.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/model/king_graph.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/model/model.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/model/model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/__init__.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/base_sa_sample_hubo.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/base_sa_sample_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/csqa_sampler.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/csqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/response.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/response.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/sa_sampler.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/sampler.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/sampler/sqa_sampler.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/utils/__init__.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/utils/benchmark.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/utils/cxx_cast.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/cxx_cast.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/utils/decorator.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/utils/graph_utils.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/utils/res_convertor.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/res_convertor.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing/variable_type.py` & `v_quantum_annealing-0.0.6/v_quantum_annealing/variable_type.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing.egg-info/PKG-INFO` & `v_quantum_annealing-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
-Name: v-quantum-annealing
-Version: 0.0.5
+Name: v_quantum_annealing
+Version: 0.0.6
 Summary: "Framework for the Ising model and QUBO."
 Home-page: https://v-quantum-technology.com
 Author: V-QUANTUM JSC
 Author-email: nqthinh@v-quantum-technology.com
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/v-quantum-jsc/V-QUANTUM-ANNEALING
 Project-URL: Documentation, https://v_quantum_annealing.github.io/v_quantum_annealing
 Project-URL: Reference, https://ref.v_quantum_annealing.org/index.html
-Description: "file: README.md"
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,7 +20,10 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+"file: README.md"
```

### Comparing `v_quantum_annealing-0.0.5/v_quantum_annealing.egg-info/SOURCES.txt` & `v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 CMakeLists.txt
-CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
-doc-requirements.in
 pyproject.toml
 setup.cfg
 setup.py
 ./v_quantum_annealing/__init__.py
-./v_quantum_annealing/_version.py
 ./v_quantum_annealing/variable_type.py
 ./v_quantum_annealing/model/__init__.py
 ./v_quantum_annealing/model/chimera_model.py
 ./v_quantum_annealing/model/king_graph.py
 ./v_quantum_annealing/model/model.py
 ./v_quantum_annealing/sampler/__init__.py
 ./v_quantum_annealing/sampler/base_sa_sample_hubo.py
@@ -42,14 +39,22 @@
 external/eigen.cmake
 external/googletest.cmake
 external/json.cmake
 external/pybind11-json.cmake
 include/CMakeLists.txt
 include/v_quantum_annealing/algorithm/algorithm.hpp
 include/v_quantum_annealing/algorithm/all.hpp
+include/v_quantum_annealing/cimod/binary_polynomial_model.hpp
+include/v_quantum_annealing/cimod/binary_quadratic_model.hpp
+include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp
+include/v_quantum_annealing/cimod/disable_eigen_warning.hpp
+include/v_quantum_annealing/cimod/hash.hpp
+include/v_quantum_annealing/cimod/json.hpp
+include/v_quantum_annealing/cimod/utilities.hpp
+include/v_quantum_annealing/cimod/vartypes.hpp
 include/v_quantum_annealing/graph/all.hpp
 include/v_quantum_annealing/graph/binary_polynomial_model.hpp
 include/v_quantum_annealing/graph/chimera.hpp
 include/v_quantum_annealing/graph/converter.hpp
 include/v_quantum_annealing/graph/csr_sparse.hpp
 include/v_quantum_annealing/graph/dense.hpp
 include/v_quantum_annealing/graph/graph.hpp
@@ -57,15 +62,14 @@
 include/v_quantum_annealing/graph/polynomial.hpp
 include/v_quantum_annealing/graph/sparse.hpp
 include/v_quantum_annealing/graph/square.hpp
 include/v_quantum_annealing/graph/json/parse.hpp
 include/v_quantum_annealing/result/all.hpp
 include/v_quantum_annealing/result/get_solution.hpp
 include/v_quantum_annealing/sampler/sa_sampler.hpp
-include/v_quantum_annealing/system/CMakeLists.txt
 include/v_quantum_annealing/system/all.hpp
 include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
 include/v_quantum_annealing/system/classical_ising.hpp
 include/v_quantum_annealing/system/classical_ising_polynomial.hpp
 include/v_quantum_annealing/system/continuous_time_ising.hpp
 include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
 include/v_quantum_annealing/system/k_local_polynomial.hpp
@@ -104,22 +108,14 @@
 tests/test_cxx.py
 tests/test_gpu.py
 tests/test_hubo.py
 tests/test_model.py
 tests/test_sampler.py
 tests/test_sqa.py
 tests/test_utils.py
-tests/__pycache__/__init__.cpython-39.pyc
-tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc
-tests/__pycache__/test_gpu.cpython-39-pytest-7.3.1.pyc
-tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc
-tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc
-tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc
-tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc
-tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc
 tests/cxxtest/cxxtest.cpp
 tests/cxxtest/polynomial_test.hpp
 tests/cxxtest/testcase.hpp
 tests/cxxtest/graph/all.hpp
 tests/cxxtest/graph/binary_polynomial_model.hpp
 tests/cxxtest/graph/ising_polynomial_model.hpp
 tests/cxxtest/graph/polynomial.hpp
@@ -140,17 +136,15 @@
 tests/cxxtest/system/classical_ising_polynomial.hpp
 tests/cxxtest/system/ising_polynomial_sa_system.hpp
 tests/cxxtest/system/k_local.hpp
 tests/cxxtest/utility/all.hpp
 tests/cxxtest/utility/eigen.hpp
 tests/cxxtest/utility/gpu.hpp
 tests/cxxtest/utility/union_find.hpp
-v_quantum_annealing/CMakeLists.txt
 v_quantum_annealing/__init__.py
-v_quantum_annealing/_version.py
 v_quantum_annealing/compile_config.hpp
 v_quantum_annealing/declare.hpp
 v_quantum_annealing/main.cpp
 v_quantum_annealing/variable_type.py
 v_quantum_annealing.egg-info/PKG-INFO
 v_quantum_annealing.egg-info/SOURCES.txt
 v_quantum_annealing.egg-info/dependency_links.txt
```

