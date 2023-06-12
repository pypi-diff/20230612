# Comparing `tmp/v_quantum_annealing-0.0.6.tar.gz` & `tmp/v_quantum_annealing-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v_quantum_annealing-0.0.6.tar", last modified: Mon Jun 12 02:10:55 2023, max compression
+gzip compressed data, was "v_quantum_annealing-0.0.7.tar", last modified: Mon Jun 12 02:30:06 2023, max compression
```

## Comparing `v_quantum_annealing-0.0.6.tar` & `v_quantum_annealing-0.0.7.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.452574 v_quantum_annealing-0.0.6/
--rw-rw-rw-   0        0        0     9483 2023-06-10 04:35:48.000000 v_quantum_annealing-0.0.6/CMakeLists.txt
--rw-rw-rw-   0        0        0    11560 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1289 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1278 2023-06-12 02:10:55.457562 v_quantum_annealing-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     9339 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.124024 v_quantum_annealing-0.0.6/cmake/
--rw-rw-rw-   0        0        0     5390 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/FindGcov.cmake
--rw-rw-rw-   0        0        0    13074 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/FindLcov.cmake
--rw-rw-rw-   0        0        0     9299 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/Findcodecov.cmake
--rw-rw-rw-   0        0        0     4712 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/GenerateDocs.cmake
--rw-rw-rw-   0        0        0     2000 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/PythonAutoDetectOSX.cmake
--rw-rw-rw-   0        0        0     1129 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.6/cmake/llvm-cov-wrapper
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.159496 v_quantum_annealing-0.0.6/external/
--rw-rw-rw-   0        0        0     1025 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/external/cimod.cmake
--rw-rw-rw-   0        0        0     1976 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/external/eigen.cmake
--rw-rw-rw-   0        0        0     1043 2023-06-09 10:10:49.000000 v_quantum_annealing-0.0.6/external/googletest.cmake
--rw-rw-rw-   0        0        0      781 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/external/json.cmake
--rw-rw-rw-   0        0        0      465 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/external/pybind11-json.cmake
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.166440 v_quantum_annealing-0.0.6/include/
--rw-rw-rw-   0        0        0     2243 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:53.777366 v_quantum_annealing-0.0.6/include/v_quantum_annealing/
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.178408 v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/
--rw-rw-rw-   0        0        0     3244 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/algorithm.hpp
--rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/all.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.227277 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/
--rw-rw-rw-   0        0        0    45689 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0    68880 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/binary_quadratic_model.hpp
--rw-rw-rw-   0        0        0    42393 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp
--rw-rw-rw-   0        0        0     1158 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/disable_eigen_warning.hpp
--rw-rw-rw-   0        0        0     2684 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/hash.hpp
--rw-rw-rw-   0        0        0      654 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/json.hpp
--rw-rw-rw-   0        0        0     4884 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/utilities.hpp
--rw-rw-rw-   0        0        0     1624 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/vartypes.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.303066 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/
--rw-rw-rw-   0        0        0     1154 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/all.hpp
--rw-rw-rw-   0        0        0     9658 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0    15482 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/chimera.hpp
--rw-rw-rw-   0        0        0      899 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/converter.hpp
--rw-rw-rw-   0        0        0     5269 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/csr_sparse.hpp
--rw-rw-rw-   0        0        0     7702 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/dense.hpp
--rw-rw-rw-   0        0        0     2615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/graph.hpp
--rw-rw-rw-   0        0        0     9603 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/ising_polynomial_model.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.306057 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/json/
--rw-rw-rw-   0        0        0     4569 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/json/parse.hpp
--rw-rw-rw-   0        0        0    11286 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/polynomial.hpp
--rw-rw-rw-   0        0        0     8327 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/sparse.hpp
--rw-rw-rw-   0        0        0    10622 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/square.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.311045 v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/
--rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/all.hpp
--rw-rw-rw-   0        0        0     5217 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/get_solution.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.318049 v_quantum_annealing-0.0.6/include/v_quantum_annealing/sampler/
--rw-rw-rw-   0        0        0    10635 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/sampler/sa_sampler.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.406788 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/
--rw-rw-rw-   0        0        0     1410 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/all.hpp
--rw-rw-rw-   0        0        0     6308 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     7264 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/classical_ising.hpp
--rw-rw-rw-   0        0        0    21835 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/classical_ising_polynomial.hpp
--rw-rw-rw-   0        0        0    15181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/continuous_time_ising.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.423742 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.439710 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/
--rw-rw-rw-   0        0        0     5615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp
--rw-rw-rw-   0        0        0    14615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu
--rw-rw-rw-   0        0        0     1750 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp
--rw-rw-rw-   0        0        0     2898 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp
--rw-rw-rw-   0        0        0    16618 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp
--rw-rw-rw-   0        0        0     5502 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0    24738 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/k_local_polynomial.hpp
--rw-rw-rw-   0        0        0      856 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/sa_system.hpp
--rw-rw-rw-   0        0        0     3417 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/system.hpp
--rw-rw-rw-   0        0        0    19954 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/transverse_ising.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.603263 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/
--rw-rw-rw-   0        0        0     1089 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/all.hpp
--rw-rw-rw-   0        0        0    19616 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp
--rw-rw-rw-   0        0        0     5468 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/gpu.hpp
--rw-rw-rw-   0        0        0     3889 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/k_local.hpp
--rw-rw-rw-   0        0        0    13765 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/single_spin_flip.hpp
--rw-rw-rw-   0        0        0     6522 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/swendsen_wang.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.718960 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/
--rw-rw-rw-   0        0        0     1055 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/create_geometric_progression.hpp
--rw-rw-rw-   0        0        0     1179 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/disable_eigen_warning.hpp
--rw-rw-rw-   0        0        0     5958 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/eigen.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.728931 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/fmath/
--rw-rw-rw-   0        0        0    26304 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/fmath/fmath.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.763833 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/
--rw-rw-rw-   0        0        0     8427 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/cublas.hpp
--rw-rw-rw-   0        0        0     3061 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/handle_error.hpp
--rw-rw-rw-   0        0        0     2701 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/memory.hpp
--rw-rw-rw-   0        0        0     1102 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/index_type.hpp
--rw-rw-rw-   0        0        0     1337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/insert_or_assign.hpp
--rw-rw-rw-   0        0        0     1118 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/memory.hpp
--rw-rw-rw-   0        0        0     3673 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/pairhash.hpp
--rw-rw-rw-   0        0        0     4054 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/random.hpp
--rw-rw-rw-   0        0        0    10636 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/schedule_list.hpp
--rw-rw-rw-   0        0        0      853 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/thres_hold.hpp
--rw-rw-rw-   0        0        0     2444 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/type_traits.hpp
--rw-rw-rw-   0        0        0     2309 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/union_find.hpp
--rw-rw-rw-   0        0        0     4681 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1578 2023-06-12 02:10:55.501444 v_quantum_annealing-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1423 2023-06-12 02:10:11.000000 v_quantum_annealing-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.968287 v_quantum_annealing-0.0.6/tests/
--rw-rw-rw-   0        0        0     2064 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0        0 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.980254 v_quantum_annealing-0.0.6/tests/cxxtest/
--rw-rw-rw-   0        0        0     1979 2023-06-10 10:04:30.000000 v_quantum_annealing-0.0.6/tests/cxxtest/cxxtest.cpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.004190 v_quantum_annealing-0.0.6/tests/cxxtest/graph/
--rw-rw-rw-   0        0        0      809 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/all.hpp
--rw-rw-rw-   0        0        0     6134 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0     5917 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/ising_polynomial_model.hpp
--rw-rw-rw-   0        0        0     4663 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/polynomial.hpp
--rw-rw-rw-   0        0        0     7083 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/graph/quadratic.hpp
--rw-rw-rw-   0        0        0    39029 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/polynomial_test.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.062036 v_quantum_annealing-0.0.6/tests/cxxtest/result/
--rw-rw-rw-   0        0        0      700 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/result/all.hpp
--rw-rw-rw-   0        0        0     2777 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/result/result.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.103928 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/
--rw-rw-rw-   0        0        0      891 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/all.hpp
--rw-rw-rw-   0        0        0     2441 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     3200 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/gpu.hpp
--rw-rw-rw-   0        0        0     2429 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     4313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/k_local.hpp
--rw-rw-rw-   0        0        0     5337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/polynomial.hpp
--rw-rw-rw-   0        0        0     6406 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/quadraitc.hpp
--rw-rw-rw-   0        0        0     6808 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/sampler/swendsen_wang.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.185718 v_quantum_annealing-0.0.6/tests/cxxtest/system/
--rw-rw-rw-   0        0        0      861 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/all.hpp
--rw-rw-rw-   0        0        0     7840 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/binary_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     1390 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/classical_ising.hpp
--rw-rw-rw-   0        0        0     4090 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/classical_ising_polynomial.hpp
--rw-rw-rw-   0        0        0     9332 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/ising_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     2447 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/system/k_local.hpp
--rw-rw-rw-   0        0        0    15821 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.6/tests/cxxtest/testcase.hpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.296990 v_quantum_annealing-0.0.6/tests/cxxtest/utility/
--rw-rw-rw-   0        0        0      744 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/utility/all.hpp
--rw-rw-rw-   0        0        0     3829 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/utility/eigen.hpp
--rw-rw-rw-   0        0        0     6403 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/utility/gpu.hpp
--rw-rw-rw-   0        0        0     1965 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/cxxtest/utility/union_find.hpp
--rw-rw-rw-   0        0        0    28004 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_cxx.py
--rw-rw-rw-   0        0        0     5754 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_gpu.py
--rw-rw-rw-   0        0        0    60920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_hubo.py
--rw-rw-rw-   0        0        0     6313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_model.py
--rw-rw-rw-   0        0        0    10119 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_sampler.py
--rw-rw-rw-   0        0        0     1181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_sqa.py
--rw-rw-rw-   0        0        0     1973 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.341877 v_quantum_annealing-0.0.6/v_quantum_annealing/
--rw-rw-rw-   0        0        0     1086 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/__init__.py
--rw-rw-rw-   0        0        0     2988 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/compile_config.hpp
--rw-rw-rw-   0        0        0    44951 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/declare.hpp
--rw-rw-rw-   0        0        0    15576 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/main.cpp
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:53.972430 v_quantum_annealing-0.0.6/v_quantum_annealing/model/
--rw-rw-rw-   0        0        0      887 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/model/__init__.py
--rw-rw-rw-   0        0        0    14286 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/model/chimera_model.py
--rw-rw-rw-   0        0        0     9035 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/model/king_graph.py
--rw-rw-rw-   0        0        0    23582 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/model/model.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.042243 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/
--rw-rw-rw-   0        0        0      529 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/__init__.py
--rw-rw-rw-   0        0        0     4272 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/base_sa_sample_hubo.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.064189 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/
--rw-rw-rw-   0        0        0      320 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/__init__.py
--rw-rw-rw-   0        0        0     2363 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
--rw-rw-rw-   0        0        0     5010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
--rw-rw-rw-   0        0        0     5847 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
--rw-rw-rw-   0        0        0     5240 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/csqa_sampler.py
--rw-rw-rw-   0        0        0     1124 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/response.py
--rw-rw-rw-   0        0        0    25532 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sa_sampler.py
--rw-rw-rw-   0        0        0     8979 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sampler.py
--rw-rw-rw-   0        0        0    12920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sqa_sampler.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:54.098100 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/
--rw-rw-rw-   0        0        0      767 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/__init__.py
--rw-rw-rw-   0        0        0    10152 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/benchmark.py
--rw-rw-rw-   0        0        0     1283 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/cxx_cast.py
--rw-rw-rw-   0        0        0      855 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/decorator.py
--rw-rw-rw-   0        0        0      992 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/graph_utils.py
--rw-rw-rw-   0        0        0     2120 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/res_convertor.py
--rw-rw-rw-   0        0        0       36 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/utils/time_measure.py
--rw-rw-rw-   0        0        0     1010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.6/v_quantum_annealing/variable_type.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:10:55.403711 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/
--rw-rw-rw-   0        0        0     1278 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7360 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-12 02:10:08.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      130 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-12 02:10:53.000000 v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:06.177053 v_quantum_annealing-0.0.7/
+-rw-rw-rw-   0        0        0     9483 2023-06-10 04:35:48.000000 v_quantum_annealing-0.0.7/CMakeLists.txt
+-rw-rw-rw-   0        0        0    11560 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1289 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1278 2023-06-12 02:30:06.178031 v_quantum_annealing-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9339 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.366536 v_quantum_annealing-0.0.7/cmake/
+-rw-rw-rw-   0        0        0     5390 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.7/cmake/FindGcov.cmake
+-rw-rw-rw-   0        0        0    13074 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.7/cmake/FindLcov.cmake
+-rw-rw-rw-   0        0        0     9299 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.7/cmake/Findcodecov.cmake
+-rw-rw-rw-   0        0        0     4712 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.7/cmake/GenerateDocs.cmake
+-rw-rw-rw-   0        0        0     2000 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.7/cmake/PythonAutoDetectOSX.cmake
+-rw-rw-rw-   0        0        0     1129 2023-06-05 02:59:11.000000 v_quantum_annealing-0.0.7/cmake/llvm-cov-wrapper
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.393973 v_quantum_annealing-0.0.7/external/
+-rw-rw-rw-   0        0        0     1025 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/external/cimod.cmake
+-rw-rw-rw-   0        0        0     1976 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/external/eigen.cmake
+-rw-rw-rw-   0        0        0     1043 2023-06-09 10:10:49.000000 v_quantum_annealing-0.0.7/external/googletest.cmake
+-rw-rw-rw-   0        0        0      781 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/external/json.cmake
+-rw-rw-rw-   0        0        0      465 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/external/pybind11-json.cmake
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.399960 v_quantum_annealing-0.0.7/include/
+-rw-rw-rw-   0        0        0     2243 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.027010 v_quantum_annealing-0.0.7/include/v_quantum_annealing/
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.413917 v_quantum_annealing-0.0.7/include/v_quantum_annealing/algorithm/
+-rw-rw-rw-   0        0        0     3244 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/algorithm/algorithm.hpp
+-rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/algorithm/all.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.446118 v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/
+-rw-rw-rw-   0        0        0    45689 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0    68880 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/binary_quadratic_model.hpp
+-rw-rw-rw-   0        0        0    42393 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp
+-rw-rw-rw-   0        0        0     1158 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/disable_eigen_warning.hpp
+-rw-rw-rw-   0        0        0     2684 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/hash.hpp
+-rw-rw-rw-   0        0        0      654 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/json.hpp
+-rw-rw-rw-   0        0        0     4884 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/utilities.hpp
+-rw-rw-rw-   0        0        0     1624 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/vartypes.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.498834 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/
+-rw-rw-rw-   0        0        0     1154 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/all.hpp
+-rw-rw-rw-   0        0        0     9658 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0    15482 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/chimera.hpp
+-rw-rw-rw-   0        0        0      899 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/converter.hpp
+-rw-rw-rw-   0        0        0     5269 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/csr_sparse.hpp
+-rw-rw-rw-   0        0        0     7702 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/dense.hpp
+-rw-rw-rw-   0        0        0     2615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/graph.hpp
+-rw-rw-rw-   0        0        0     9603 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/ising_polynomial_model.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.500823 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/json/
+-rw-rw-rw-   0        0        0     4569 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/json/parse.hpp
+-rw-rw-rw-   0        0        0    11286 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     8327 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/sparse.hpp
+-rw-rw-rw-   0        0        0    10622 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/square.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.503815 v_quantum_annealing-0.0.7/include/v_quantum_annealing/result/
+-rw-rw-rw-   0        0        0      731 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/result/all.hpp
+-rw-rw-rw-   0        0        0     5217 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/result/get_solution.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.505809 v_quantum_annealing-0.0.7/include/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0    10635 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/sampler/sa_sampler.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.577176 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/
+-rw-rw-rw-   0        0        0     1410 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/all.hpp
+-rw-rw-rw-   0        0        0     6308 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     7264 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0    21835 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0    15181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/continuous_time_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.609079 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.634015 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_cuda/
+-rw-rw-rw-   0        0        0     5615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp
+-rw-rw-rw-   0        0        0    14615 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu
+-rw-rw-rw-   0        0        0     1750 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp
+-rw-rw-rw-   0        0        0     2898 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp
+-rw-rw-rw-   0        0        0    16618 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp
+-rw-rw-rw-   0        0        0     5502 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0    24738 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/k_local_polynomial.hpp
+-rw-rw-rw-   0        0        0      856 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/sa_system.hpp
+-rw-rw-rw-   0        0        0     3417 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/system.hpp
+-rw-rw-rw-   0        0        0    19954 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/transverse_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.680886 v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/
+-rw-rw-rw-   0        0        0     1089 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/all.hpp
+-rw-rw-rw-   0        0        0    19616 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp
+-rw-rw-rw-   0        0        0     5468 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/gpu.hpp
+-rw-rw-rw-   0        0        0     3889 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/k_local.hpp
+-rw-rw-rw-   0        0        0    13765 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/single_spin_flip.hpp
+-rw-rw-rw-   0        0        0     6522 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.741465 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/
+-rw-rw-rw-   0        0        0     1055 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/create_geometric_progression.hpp
+-rw-rw-rw-   0        0        0     1179 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/disable_eigen_warning.hpp
+-rw-rw-rw-   0        0        0     5958 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/eigen.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.743460 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/fmath/
+-rw-rw-rw-   0        0        0    26304 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/fmath/fmath.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.769390 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/gpu/
+-rw-rw-rw-   0        0        0     8427 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/gpu/cublas.hpp
+-rw-rw-rw-   0        0        0     3061 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/gpu/handle_error.hpp
+-rw-rw-rw-   0        0        0     2701 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/gpu/memory.hpp
+-rw-rw-rw-   0        0        0     1102 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/index_type.hpp
+-rw-rw-rw-   0        0        0     1337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/insert_or_assign.hpp
+-rw-rw-rw-   0        0        0     1118 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/memory.hpp
+-rw-rw-rw-   0        0        0     3673 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/pairhash.hpp
+-rw-rw-rw-   0        0        0     4054 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/random.hpp
+-rw-rw-rw-   0        0        0    10636 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/schedule_list.hpp
+-rw-rw-rw-   0        0        0      853 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/thres_hold.hpp
+-rw-rw-rw-   0        0        0     2444 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/type_traits.hpp
+-rw-rw-rw-   0        0        0     2309 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/union_find.hpp
+-rw-rw-rw-   0        0        0     4681 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1578 2023-06-12 02:30:06.221915 v_quantum_annealing-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1423 2023-06-12 02:29:48.000000 v_quantum_annealing-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.815270 v_quantum_annealing-0.0.7/tests/
+-rw-rw-rw-   0        0        0     2064 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0        0 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.843193 v_quantum_annealing-0.0.7/tests/cxxtest/
+-rw-rw-rw-   0        0        0     1979 2023-06-10 10:04:30.000000 v_quantum_annealing-0.0.7/tests/cxxtest/cxxtest.cpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.881091 v_quantum_annealing-0.0.7/tests/cxxtest/graph/
+-rw-rw-rw-   0        0        0      809 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/graph/all.hpp
+-rw-rw-rw-   0        0        0     6134 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     5917 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/graph/ising_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     4663 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/tests/cxxtest/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     7083 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/graph/quadratic.hpp
+-rw-rw-rw-   0        0        0    39029 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/polynomial_test.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.902592 v_quantum_annealing-0.0.7/tests/cxxtest/result/
+-rw-rw-rw-   0        0        0      700 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/result/all.hpp
+-rw-rw-rw-   0        0        0     2777 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/result/result.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.953643 v_quantum_annealing-0.0.7/tests/cxxtest/sampler/
+-rw-rw-rw-   0        0        0      891 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/sampler/all.hpp
+-rw-rw-rw-   0        0        0     2441 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     3200 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/sampler/gpu.hpp
+-rw-rw-rw-   0        0        0     2429 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     4313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/sampler/k_local.hpp
+-rw-rw-rw-   0        0        0     5337 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/sampler/polynomial.hpp
+-rw-rw-rw-   0        0        0     6406 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/sampler/quadraitc.hpp
+-rw-rw-rw-   0        0        0     6808 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/sampler/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.999520 v_quantum_annealing-0.0.7/tests/cxxtest/system/
+-rw-rw-rw-   0        0        0      861 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/system/all.hpp
+-rw-rw-rw-   0        0        0     7840 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     1390 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0     4090 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0     9332 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     2447 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/system/k_local.hpp
+-rw-rw-rw-   0        0        0    15821 2023-06-10 14:45:28.000000 v_quantum_annealing-0.0.7/tests/cxxtest/testcase.hpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:06.024444 v_quantum_annealing-0.0.7/tests/cxxtest/utility/
+-rw-rw-rw-   0        0        0      744 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/utility/all.hpp
+-rw-rw-rw-   0        0        0     3829 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/utility/eigen.hpp
+-rw-rw-rw-   0        0        0     6403 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/utility/gpu.hpp
+-rw-rw-rw-   0        0        0     1965 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/cxxtest/utility/union_find.hpp
+-rw-rw-rw-   0        0        0    28004 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/test_cxx.py
+-rw-rw-rw-   0        0        0     5754 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/test_gpu.py
+-rw-rw-rw-   0        0        0    60920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/test_hubo.py
+-rw-rw-rw-   0        0        0     6313 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/test_model.py
+-rw-rw-rw-   0        0        0    10119 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/test_sampler.py
+-rw-rw-rw-   0        0        0     1181 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/test_sqa.py
+-rw-rw-rw-   0        0        0     1973 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:06.084293 v_quantum_annealing-0.0.7/v_quantum_annealing/
+-rw-rw-rw-   0        0        0     1086 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/__init__.py
+-rw-rw-rw-   0        0        0     2988 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/compile_config.hpp
+-rw-rw-rw-   0        0        0    44951 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/declare.hpp
+-rw-rw-rw-   0        0        0    15576 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/main.cpp
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.173762 v_quantum_annealing-0.0.7/v_quantum_annealing/model/
+-rw-rw-rw-   0        0        0      887 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/model/__init__.py
+-rw-rw-rw-   0        0        0    14286 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/model/chimera_model.py
+-rw-rw-rw-   0        0        0     9035 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/model/king_graph.py
+-rw-rw-rw-   0        0        0    23582 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/model/model.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.208670 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0      529 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/__init__.py
+-rw-rw-rw-   0        0        0     4272 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/base_sa_sample_hubo.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.239594 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/chimera_gpu/
+-rw-rw-rw-   0        0        0      320 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/chimera_gpu/__init__.py
+-rw-rw-rw-   0        0        0     2363 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
+-rw-rw-rw-   0        0        0     5010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
+-rw-rw-rw-   0        0        0     5847 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
+-rw-rw-rw-   0        0        0     5240 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/csqa_sampler.py
+-rw-rw-rw-   0        0        0     1124 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/response.py
+-rw-rw-rw-   0        0        0    25532 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/sa_sampler.py
+-rw-rw-rw-   0        0        0     8979 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/sampler.py
+-rw-rw-rw-   0        0        0    12920 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/sqa_sampler.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:05.298439 v_quantum_annealing-0.0.7/v_quantum_annealing/utils/
+-rw-rw-rw-   0        0        0      767 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10152 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/utils/benchmark.py
+-rw-rw-rw-   0        0        0     1283 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/utils/cxx_cast.py
+-rw-rw-rw-   0        0        0      855 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/utils/decorator.py
+-rw-rw-rw-   0        0        0      992 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/utils/graph_utils.py
+-rw-rw-rw-   0        0        0     2120 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/utils/res_convertor.py
+-rw-rw-rw-   0        0        0       36 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/utils/time_measure.py
+-rw-rw-rw-   0        0        0     1010 2023-06-05 02:59:12.000000 v_quantum_annealing-0.0.7/v_quantum_annealing/variable_type.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:30:06.152100 v_quantum_annealing-0.0.7/v_quantum_annealing.egg-info/
+-rw-rw-rw-   0        0        0     1278 2023-06-12 02:30:04.000000 v_quantum_annealing-0.0.7/v_quantum_annealing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7360 2023-06-12 02:30:04.000000 v_quantum_annealing-0.0.7/v_quantum_annealing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 02:30:04.000000 v_quantum_annealing-0.0.7/v_quantum_annealing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-12 02:10:08.000000 v_quantum_annealing-0.0.7/v_quantum_annealing.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      130 2023-06-12 02:30:04.000000 v_quantum_annealing-0.0.7/v_quantum_annealing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-12 02:30:04.000000 v_quantum_annealing-0.0.7/v_quantum_annealing.egg-info/top_level.txt
```

### Comparing `v_quantum_annealing-0.0.6/CMakeLists.txt` & `v_quantum_annealing-0.0.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/LICENSE` & `v_quantum_annealing-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/MANIFEST.in` & `v_quantum_annealing-0.0.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/PKG-INFO` & `v_quantum_annealing-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v_quantum_annealing
-Version: 0.0.6
+Version: 0.0.7
 Summary: "Framework for the Ising model and QUBO."
 Home-page: https://v-quantum-technology.com
 Author: V-QUANTUM JSC
 Author-email: nqthinh@v-quantum-technology.com
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/v-quantum-jsc/V-QUANTUM-ANNEALING
 Project-URL: Documentation, https://v_quantum_annealing.github.io/v_quantum_annealing
```

### Comparing `v_quantum_annealing-0.0.6/README.md` & `v_quantum_annealing-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/cmake/FindGcov.cmake` & `v_quantum_annealing-0.0.7/cmake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/cmake/FindLcov.cmake` & `v_quantum_annealing-0.0.7/cmake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/cmake/Findcodecov.cmake` & `v_quantum_annealing-0.0.7/cmake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/cmake/GenerateDocs.cmake` & `v_quantum_annealing-0.0.7/cmake/GenerateDocs.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/cmake/PythonAutoDetectOSX.cmake` & `v_quantum_annealing-0.0.7/cmake/PythonAutoDetectOSX.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/cmake/llvm-cov-wrapper` & `v_quantum_annealing-0.0.7/cmake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/external/cimod.cmake` & `v_quantum_annealing-0.0.7/external/cimod.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/external/eigen.cmake` & `v_quantum_annealing-0.0.7/external/eigen.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/external/googletest.cmake` & `v_quantum_annealing-0.0.7/external/googletest.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/external/json.cmake` & `v_quantum_annealing-0.0.7/external/json.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/CMakeLists.txt` & `v_quantum_annealing-0.0.7/include/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/algorithm.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/algorithm/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/algorithm/all.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/algorithm/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/binary_quadratic_model.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/binary_quadratic_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/binary_quadratic_model_dict.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/disable_eigen_warning.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/disable_eigen_warning.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/hash.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/hash.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/json.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/json.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/utilities.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/utilities.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/cimod/vartypes.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/cimod/vartypes.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/all.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/chimera.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/chimera.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/converter.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/converter.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/csr_sparse.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/csr_sparse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/dense.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/dense.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/graph.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/graph.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/ising_polynomial_model.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/json/parse.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/json/parse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/polynomial.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/sparse.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/sparse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/graph/square.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/graph/square.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/all.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/result/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/result/get_solution.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/result/get_solution.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/sampler/sa_sampler.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/sampler/sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/all.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/classical_ising.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/classical_ising_polynomial.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/continuous_time_ising.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/continuous_time_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/k_local_polynomial.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/k_local_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/sa_system.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/system.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/system/transverse_ising.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/system/transverse_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/all.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/gpu.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/k_local.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/single_spin_flip.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/single_spin_flip.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/updater/swendsen_wang.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/updater/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/create_geometric_progression.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/create_geometric_progression.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/disable_eigen_warning.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/disable_eigen_warning.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/eigen.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/fmath/fmath.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/fmath/fmath.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/cublas.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/gpu/cublas.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/handle_error.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/gpu/handle_error.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/gpu/memory.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/gpu/memory.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/index_type.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/index_type.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/insert_or_assign.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/insert_or_assign.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/memory.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/memory.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/pairhash.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/pairhash.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/random.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/random.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/schedule_list.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/schedule_list.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/thres_hold.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/thres_hold.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/type_traits.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/include/v_quantum_annealing/utility/union_find.hpp` & `v_quantum_annealing-0.0.7/include/v_quantum_annealing/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/pyproject.toml` & `v_quantum_annealing-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/setup.cfg` & `v_quantum_annealing-0.0.7/setup.cfg`

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
-000001b0: 6e20 3d20 2230 2e30 2e36 220d 0a63 6c61  n = "0.0.6"..cla
+000001b0: 6e20 3d20 2230 2e30 2e37 220d 0a63 6c61  n = "0.0.7"..cla
 000001c0: 7373 6966 6965 7273 203d 200d 0a09 4c69  ssifiers = ...Li
 000001d0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
 000001e0: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
 000001f0: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
 00000200: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
 00000210: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
 00000220: 5265 7365 6172 6368 0d0a 0950 726f 6772  Research...Progr
@@ -78,15 +78,15 @@
 000004d0: 3c33 2e31 310d 0a69 6e73 7461 6c6c 5f72  <3.11..install_r
 000004e0: 6571 7569 7265 7320 3d20 0d0a 096e 756d  equires = ...num
 000004f0: 7079 203e 3d31 2e31 372e 332c 203c 2031  py >=1.17.3, < 1
 00000500: 2e32 352e 300d 0a09 6469 6d6f 6420 3c20  .25.0...dimod < 
 00000510: 302e 3133 2e30 0d0a 0973 6369 7079 203e  0.13.0...scipy >
 00000520: 3d20 312e 372e 332c 203c 2031 2e31 312e  = 1.7.3, < 1.11.
 00000530: 300d 0a09 7265 7175 6573 7473 203e 3d20  0...requests >= 
-00000540: 322e 3238 2e30 2c20 3c20 322e 3239 2e30  2.28.0, < 2.29.0
+00000540: 322e 3237 2e30 2c20 3c20 322e 3239 2e30  2.27.0, < 2.29.0
 00000550: 0d0a 096a 696a 2d63 696d 6f64 203e 3d20  ...jij-cimod >= 
 00000560: 312e 302e 302c 203c 2031 2e32 2e33 0d0a  1.0.0, < 1.2.3..
 00000570: 0974 7970 696e 672d 6578 7465 6e73 696f  .typing-extensio
 00000580: 6e73 203e 3d20 342e 322e 300d 0a74 6573  ns >= 4.2.0..tes
 00000590: 7473 5f72 6571 7569 7265 203d 200d 0a09  ts_require = ...
 000005a0: 7079 7465 7374 0d0a 0970 7974 6573 742d  pytest...pytest-
 000005b0: 6d6f 636b 0d0a 0970 7974 6573 742d 636f  mock...pytest-co
```

### Comparing `v_quantum_annealing-0.0.6/setup.py` & `v_quantum_annealing-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 setup_requires = [
     "numpy",
     "pybind11 >=2.10.0, < 2.11.0",
     "cmake > 3.20",
     "scikit-build > 0.16.0"
 ]
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 setup(
     name="v_quantum_annealing", 
     version=__version__,  
     author = "V-QUANTUM JSC",
     author_email = "nqthinh@v-quantum-technology.com",
     setup_requires=setup_requires,
```

### Comparing `v_quantum_annealing-0.0.6/tests/CMakeLists.txt` & `v_quantum_annealing-0.0.7/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/cxxtest.cpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/cxxtest.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/graph/all.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/graph/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/graph/ising_polynomial_model.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/graph/polynomial.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/graph/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/graph/quadratic.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/graph/quadratic.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/polynomial_test.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/polynomial_test.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/result/all.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/result/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/result/result.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/result/result.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/all.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/sampler/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/gpu.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/sampler/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/k_local.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/sampler/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/polynomial.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/sampler/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/quadraitc.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/sampler/quadraitc.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/sampler/swendsen_wang.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/sampler/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/system/all.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/system/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/system/binary_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/system/classical_ising.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/system/classical_ising_polynomial.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/system/ising_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/system/k_local.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/system/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/testcase.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/testcase.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/utility/all.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/utility/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/utility/eigen.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/utility/gpu.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/utility/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/cxxtest/utility/union_find.hpp` & `v_quantum_annealing-0.0.7/tests/cxxtest/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/test_cxx.py` & `v_quantum_annealing-0.0.7/tests/test_cxx.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/test_gpu.py` & `v_quantum_annealing-0.0.7/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/test_hubo.py` & `v_quantum_annealing-0.0.7/tests/test_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/test_model.py` & `v_quantum_annealing-0.0.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/test_sampler.py` & `v_quantum_annealing-0.0.7/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/test_sqa.py` & `v_quantum_annealing-0.0.7/tests/test_sqa.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/tests/test_utils.py` & `v_quantum_annealing-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/__init__.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/compile_config.hpp` & `v_quantum_annealing-0.0.7/v_quantum_annealing/compile_config.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/declare.hpp` & `v_quantum_annealing-0.0.7/v_quantum_annealing/declare.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/main.cpp` & `v_quantum_annealing-0.0.7/v_quantum_annealing/main.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/model/__init__.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/model/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/model/chimera_model.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/model/chimera_model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/model/king_graph.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/model/king_graph.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/model/model.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/model/model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/__init__.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/base_sa_sample_hubo.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/base_sa_sample_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/csqa_sampler.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/csqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/response.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/response.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sa_sampler.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sampler.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/sampler/sqa_sampler.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/sampler/sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/__init__.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/benchmark.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/cxx_cast.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/utils/cxx_cast.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/decorator.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/graph_utils.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/utils/res_convertor.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/utils/res_convertor.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing/variable_type.py` & `v_quantum_annealing-0.0.7/v_quantum_annealing/variable_type.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/PKG-INFO` & `v_quantum_annealing-0.0.7/v_quantum_annealing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v-quantum-annealing
-Version: 0.0.6
+Version: 0.0.7
 Summary: "Framework for the Ising model and QUBO."
 Home-page: https://v-quantum-technology.com
 Author: V-QUANTUM JSC
 Author-email: nqthinh@v-quantum-technology.com
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/v-quantum-jsc/V-QUANTUM-ANNEALING
 Project-URL: Documentation, https://v_quantum_annealing.github.io/v_quantum_annealing
```

### Comparing `v_quantum_annealing-0.0.6/v_quantum_annealing.egg-info/SOURCES.txt` & `v_quantum_annealing-0.0.7/v_quantum_annealing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

