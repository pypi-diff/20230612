# Comparing `tmp/mapchete-2023.6.1.tar.gz` & `tmp/mapchete-2023.6.2.tar.gz`

## Comparing `mapchete-2023.6.1.tar` & `mapchete-2023.6.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/__init__.py
--rw-r--r--   0        0        0    29098 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_core.py
--rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_executor.py
--rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_processing.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_registered.py
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_tasks.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_timer.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/_user_process.py
--rw-r--r--   0        0        0    48597 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/config.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/errors.py
--rw-r--r--   0        0        0    17748 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/index.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/log.py
--rw-r--r--   0        0        0    24483 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/path.py
--rw-r--r--   0        0        0    17481 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/stac.py
--rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/testing.py
--rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/tile.py
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/types.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/main.py
--rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     4995 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/__init__.py
--rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commons/contours.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    20802 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/loaders.py
--rw-r--r--   0        0        0    12520 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    15914 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/_json.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/_misc.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/_path.py
--rw-r--r--   0        0        0    44018 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/raster.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/settings.py
--rw-r--r--   0        0        0    21813 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/io/vector.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/static/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/static/index.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.1/mapchete/static/process_template.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.1/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.1/README.rst
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/__init__.py
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_core.py
+-rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_executor.py
+-rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_processing.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_registered.py
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_tasks.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_timer.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_user_process.py
+-rw-r--r--   0        0        0    48622 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/config.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/errors.py
+-rw-r--r--   0        0        0    17833 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/index.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/log.py
+-rw-r--r--   0        0        0    24958 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/path.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/stac.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/testing.py
+-rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/tile.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/types.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/main.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_convert.py
+-rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_cp.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_execute.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_index.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_rm.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commons/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commons/clip.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commons/contours.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commons/hillshade.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20760 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/geobuf.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/_path.py
+-rw-r--r--   0        0        0    44156 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/raster.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/settings.py
+-rw-r--r--   0        0        0    22010 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/static/index.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.2/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.2/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.2/README.rst
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.2/PKG-INFO
```

### Comparing `mapchete-2023.6.1/mapchete/__init__.py` & `mapchete-2023.6.2/mapchete/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     "ProcessInfo",
     "Timer",
     "Executor",
     "FakeFuture",
     "SkippedFuture",
     "Job",
 ]
-__version__ = "2023.6.1"
+__version__ = "2023.6.2"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `mapchete-2023.6.1/mapchete/_core.py` & `mapchete-2023.6.2/mapchete/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,19 +61,19 @@
     Returns
     -------
     Mapchete
         a Mapchete process object
     """
     # convert to MPath object if possible
     if isinstance(some_input, str):
-        some_input = MPath(some_input)
+        some_input = MPath.from_inp(some_input)
     # for TileDirectory inputs
     if isinstance(some_input, MPath) and some_input.suffix == "":
         logger.debug("assuming TileDirectory")
-        metadata_json = MPath(some_input).joinpath("metadata.json")
+        metadata_json = MPath.from_inp(some_input).joinpath("metadata.json")
         fs_kwargs = fs_kwargs or {}
         fs = fs or fs_from_path(metadata_json, **fs_kwargs)
         logger.debug("read metadata.json")
         metadata = read_output_metadata(metadata_json, fs=fs)
         config = dict(
             process=None,
             input=None,
@@ -703,15 +703,15 @@
                 zoom_levels=self.config.init_zoom_levels,
                 bounds=self.config.effective_bounds,
                 item_metadata=self.config.output.stac_item_metadata,
                 tile_pyramid=self.config.output_pyramid,
                 bands_type=self.config.output.stac_asset_type,
             )
             logger.debug("write STAC item JSON to %s", self.config.output.stac_path)
-            self.config.output.stac_path.makedirs()
+            self.config.output.stac_path.parent.makedirs()
             with self.config.output.stac_path.open("w") as dst:
                 dst.write(json.dumps(item.to_dict(), indent=indent))
         except ReprojectionFailed:
             logger.warning(
                 "cannot create STAC item because footprint cannot be reprojected into EPSG:4326"
             )
         except Exception as exc:  # pragma: no cover
```

### Comparing `mapchete-2023.6.1/mapchete/_executor.py` & `mapchete-2023.6.2/mapchete/_executor.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/_processing.py` & `mapchete-2023.6.2/mapchete/_processing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/_registered.py` & `mapchete-2023.6.2/mapchete/_registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/_tasks.py` & `mapchete-2023.6.2/mapchete/_tasks.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/_timer.py` & `mapchete-2023.6.2/mapchete/_timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/_user_process.py` & `mapchete-2023.6.2/mapchete/_user_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/config.py` & `mapchete-2023.6.2/mapchete/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,15 @@
             pixelbuffer=self.output_pyramid.pixelbuffer,
             metatiling=self.output_pyramid.metatiling,
             delimiters=self._delimiters,
             mode=self.mode,
         )
         if "path" in output_params:
             output_params.update(
-                path=MPath.from_dict(output_params).absolute_path(
+                path=MPath.from_inp(output_params).absolute_path(
                     base_dir=self.config_dir
                 )
             )
 
         if "format" not in output_params:
             raise MapcheteConfigError("output format not specified")
 
@@ -1042,15 +1042,15 @@
         elif isinstance(v, dict):
             logger.debug("load input reader for abstract input %s", v)
             try:
                 abstract = deepcopy(v)
                 # make path absolute and add filesystem options
                 if "path" in abstract:
                     abstract.update(
-                        path=MPath.from_dict(abstract).absolute_path(config_dir)
+                        path=MPath.from_inp(abstract).absolute_path(config_dir)
                     )
                 reader = load_input_reader(
                     dict(
                         abstract=abstract,
                         pyramid=pyramid,
                         pixelbuffer=pyramid.pixelbuffer,
                         delimiters=delimiters,
@@ -1074,23 +1074,23 @@
         initalized_inputs.keys(),
     )
     return initalized_inputs
 
 
 def _load_process_module(process=None, config_dir=None, run_compile=False):
     tmpfile = None
-    process = MPath(process) if isinstance(process, str) else process
+    process = MPath.from_inp(process) if isinstance(process, str) else process
     try:
         if isinstance(process, list):
             tmpfile = NamedTemporaryFile(suffix=".py")
             logger.debug(f"writing process code to temporary file {tmpfile.name}")
             with open(tmpfile.name, "w") as dst:
                 for line in process:
                     dst.write(line + "\n")
-            process = MPath(tmpfile.name)
+            process = MPath.from_inp(tmpfile.name)
         if process.suffix == ".py":
             module_path = absolute_path(path=process, base_dir=config_dir)
             if not module_path.exists():
                 raise MapcheteConfigError(f"{module_path} is not available")
             try:
                 if run_compile:
                     py_compile.compile(module_path, doraise=True)
@@ -1373,15 +1373,15 @@
     """
     crs = None
     # WKT or path:
     if isinstance(i, (str, MPath)):
         if str(i).upper().startswith(("POLYGON ", "MULTIPOLYGON ")):
             geom = wkt.loads(i)
         else:
-            path = MPath(i)
+            path = MPath.from_inp(i)
             with path.fio_env():
                 with fiona_open(str(path.absolute_path(base_dir))) as src:
                     geom = unary_union([shape(f["geometry"]) for f in src])
                     crs = src.crs
     # GeoJSON mapping
     elif isinstance(i, dict):
         geom = shape(i)
```

### Comparing `mapchete-2023.6.1/mapchete/errors.py` & `mapchete-2023.6.2/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/index.py` & `mapchete-2023.6.2/mapchete/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,34 +185,34 @@
                         index.write(output_tile, tile_path)
 
                 # yield tile for progress information
                 yield output_tile
 
 
 def _index_file_path(out_dir, zoom, ext):
-    return MPath(out_dir) / f"{str(zoom)}.{ext}"
+    return MPath.from_inp(out_dir) / f"{str(zoom)}.{ext}"
 
 
 def _tile_path(orig_path=None, basepath=None, for_gdal=True):
     path = (
-        MPath(basepath).joinpath(*orig_path.elements[-3:])
+        MPath.from_inp(basepath).joinpath(*orig_path.elements[-3:])
         if basepath
-        else MPath(orig_path)
+        else MPath.from_inp(orig_path)
     )
     if for_gdal:
         return path.as_gdal_str()
     else:
         return str(path)
 
 
 class VectorFileWriter:
     """Writes GeoJSON or GeoPackage files."""
 
     def __init__(self, out_path=None, crs=None, fieldname=None, driver=None):
-        self.path = MPath(out_path)
+        self.path = MPath.from_inp(out_path)
         self._append = (
             "a" in fiona.supported_drivers[driver] and not self.path.is_remote()
         )
         logger.debug("initialize %s writer with append %s", driver, self._append)
         self.driver = driver
         self.fieldname = fieldname
         self.new_entries = 0
@@ -352,15 +352,15 @@
         self._tp = out_pyramid
         self._output = output
         self.fs = fs_from_path(out_path)
         logger.debug("initialize VRT writer for %s", self.path)
         if path_exists(self.path):
             with self.fs.open(self.path) as src:
                 self._existing = {
-                    k: MPath(v) for k, v in self._xml_to_entries(src.read())
+                    k: MPath.from_inp(v) for k, v in self._xml_to_entries(src.read())
                 }
         else:
             self._existing = {}
         logger.debug("%s existing entries", len(self._existing))
         self.new_entries = 0
         self._new = {}
 
@@ -370,18 +370,20 @@
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def _path_to_tile(self, path):
-        return self._tp.tile(*map(int, MPath(path).without_suffix().elements[-3:]))
+        return self._tp.tile(
+            *map(int, MPath.from_inp(path).without_suffix().elements[-3:])
+        )
 
     def _add_entry(self, tile=None, path=None):
-        self._new[tile] = MPath(path)
+        self._new[tile] = MPath.from_inp(path)
 
     def _xml_to_entries(self, xml_string):
         for entry in next(
             ET.ElementTree(ET.fromstring(xml_string)).getroot().iter("VRTRasterBand")
         ).iter("ComplexSource"):
             path = next(entry.iter("SourceFilename")).text
             yield (self._path_to_tile(path), path)
```

### Comparing `mapchete-2023.6.1/mapchete/log.py` & `mapchete-2023.6.2/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/path.py` & `mapchete-2023.6.2/mapchete/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,27 @@
             )
         return MPath(
             path_str,
             storage_options=dictionary.get("storage_options", {}),
             fs=dictionary.get("fs"),
         )
 
+    @staticmethod
+    def from_inp(inp, **kwargs):
+        if isinstance(inp, dict):
+            return MPath.from_dict(inp)
+        elif isinstance(inp, str):
+            return MPath(inp, **kwargs)
+        elif isinstance(inp, MPath):
+            if kwargs:
+                return MPath(inp, **kwargs)
+            return inp
+        else:  # pragma: no cover
+            raise TypeError(f"cannot construct MPath object from {inp}")
+
     def to_dict(self) -> dict:
         return dict(
             path=self._path_str,
             storage_options=self._storage_options,
             fs=self.fs,
         )
 
@@ -262,18 +275,16 @@
             return src.read()
 
     def makedirs(self, exist_ok=True) -> None:
         """Create all parent directories for path."""
         # create parent directories on local filesystems
         if self.fs.protocol == "file":
             # if path has no suffix, assume a file path and only create parent directories
-            if self.suffix != "":
-                self.fs.makedirs(self.dirname, exist_ok=exist_ok)
-            else:
-                self.fs.makedirs(self, exist_ok=exist_ok)
+            logger.debug("create directory %s", str(self))
+            self.fs.makedirs(self, exist_ok=exist_ok)
 
     def ls(self, detail=False):
         if detail:
             # return as is but convert "name" from string to MPath instead
             return [
                 {k: (self.new(v) if k == "name" else v) for k, v in path_info.items()}
                 for path_info in self.fs.ls(self._path_str, detail=detail)
@@ -324,18 +335,21 @@
         """
         user_opts = {} if opts is None else dict(**opts)
         if self.is_remote():
             gdal_opts = GDAL_HTTP_OPTS.copy()
             if self.suffix == ".vrt":
                 # we cannot know at this point which file types the VRT is pointing to,
                 # so in order to play safe, we remove the extensions constraint here
-                gdal_opts.pop("CPL_VSIL_CURL_ALLOWED_EXTENSIONS")
+                try:
+                    gdal_opts.pop("CPL_VSIL_CURL_ALLOWED_EXTENSIONS")
+                except KeyError:  # pragma: no cover
+                    pass
             else:
                 default_remote_extensions = gdal_opts.get(
-                    "CPL_VSIL_CURL_ALLOWED_EXTENSIONS", []
+                    "CPL_VSIL_CURL_ALLOWED_EXTENSIONS", ""
                 ).split(", ")
                 if allowed_remote_extensions:
                     extensions = allowed_remote_extensions.split(",") + (
                         default_remote_extensions
                     )
                 extensions = default_remote_extensions + [self.suffix]
                 # make sure current path extension is added to allowed_remote_extensions
```

### Comparing `mapchete-2023.6.1/mapchete/stac.py` & `mapchete-2023.6.2/mapchete/stac.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,16 @@
     if item_id is None:
         raise ValueError("item_id must be set")
     if zoom_levels is None:
         raise ValueError("zoom_levels must be set")
     if tile_pyramid is None:
         raise ValueError("tile_pyramid must be set")
 
-    asset_basepath = MPath(asset_basepath) if asset_basepath else None
-    item_path = MPath(item_path) if item_path else None
+    asset_basepath = MPath.from_inp(asset_basepath) if asset_basepath else None
+    item_path = MPath.from_inp(item_path) if item_path else None
 
     item_metadata = _cleanup_datetime(item_metadata or {})
     timestamp = (
         item_metadata.get("properties", {}).get("start_datetime")
         or item_metadata.get("properties", {}).get("end_datetime")
         or str(datetime.datetime.utcnow())
     )
@@ -325,15 +325,15 @@
     crs_unit_to_meter : int or float
         Factor to convert CRS units to meter if tile pyramid grid is not "geodetic" or "mercator". (default: 1)
 
     Returns
     -------
     pystac.Item
     """
-    item_path = MPath(item_path) if item_path else None
+    item_path = MPath.from_inp(item_path) if item_path else None
     # from existing item
     if item is not None:
         zoom_levels = zoom_levels or []
         zoom_levels = sorted(list(set(zoom_levels + zoom_levels_from_item(item))))
         existing_tile_pyramid = tile_pyramid_from_item(item)
         if tile_pyramid and tile_pyramid != existing_tile_pyramid:
             raise TypeError(
@@ -449,15 +449,15 @@
         # if tile exists, skip
         if mp.config.output.tiles_exist(output_tile=prototype_tile):
             logger.debug("prototype tile %s already exists", tile_path)
         # if not, write empty tile
         else:
             logger.debug("creating prototype tile %s", tile_path)
             out_profile = mp.config.output.profile(prototype_tile)
-            tile_path.makedirs()
+            tile_path.parent.makedirs()
             write_raster_window(
                 in_tile=prototype_tile,
                 in_data=ma.masked_array(
                     data=np.full(
                         (out_profile["count"],) + prototype_tile.shape,
                         out_profile["nodata"],
                         dtype=out_profile["dtype"],
```

### Comparing `mapchete-2023.6.1/mapchete/testing.py` & `mapchete-2023.6.2/mapchete/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
 
 # helper functions
 def dict_from_mapchete(path):
     """
     Read mapchete configuration from file and return as dictionary.
     """
-    path = MPath(path)
+    path = MPath.from_inp(path)
     with path.open() as src:
         out = dict(yaml.safe_load(src.read()), config_dir=path.dirname)
         if "config_dir" in out:
-            out["config_dir"] = MPath(out["config_dir"])
+            out["config_dir"] = MPath.from_inp(out["config_dir"])
         elif "path" in out.get("output", {}):  # pragma: no cover
-            out["output"]["path"] = MPath.from_dict(out["output"])
+            out["output"]["path"] = MPath.from_inp(out["output"])
     return out
 
 
 def dict_to_yaml(dictionary):
     def _convert(vv):
         out = OrderedDict()
         for k, v in vv.items():
@@ -51,21 +51,21 @@
         self,
         path=None,
         tempdir=None,
         inp_cache_tempdir=None,
         output_suffix="",
         **kwargs,
     ):
-        self.path = MPath(path)
+        self.path = MPath.from_inp(path)
         self.basepath = MPath.parent
         self.output_path = None
         self.dict = None
         tempdir = tempdir or kwargs.get("output_tempdir")
         if tempdir:
-            self._tempdir = MPath(tempdir) / uuid.uuid4().hex
+            self._tempdir = MPath.from_inp(tempdir) / uuid.uuid4().hex
         else:  # pragma: no cover
             self._tempdir = None
         if inp_cache_tempdir:
             self._inp_cache_tempdir = inp_cache_tempdir / uuid.uuid4().hex
         else:
             self._inp_cache_tempdir = None
         self._out_fs = None
@@ -76,33 +76,33 @@
 
         # move all input/foo/cache/path paths to inp_cache_tempdir
         if self._inp_cache_tempdir:
             for key, val in self.dict.get("input", {}).items():
                 if isinstance(val, dict):
                     if "cache" in val:
                         if "path" in val["cache"]:
-                            path = MPath.from_dict(val["cache"])
+                            path = MPath.from_inp(val["cache"])
                             temp_path = (
                                 self._inp_cache_tempdir / key / "cache" / path.name
                             )
-                            temp_path.makedirs()
+                            temp_path.parent.makedirs()
                             val["cache"]["path"] = temp_path
         # replace output path with temporary path
         if self._tempdir:
             # set output directory
-            current_output_path = MPath.from_dict(self.dict["output"])
+            current_output_path = MPath.from_inp(self.dict["output"])
             if current_output_path.suffix:
                 self.dict["output"]["path"] = self._tempdir / current_output_path.name
             else:
                 self.dict["output"]["path"] = self._tempdir / "out"
 
             self.path = self._tempdir / self.path.name
 
             # dump modified mapchete config to temporary directory
-            self.path.makedirs()
+            self.path.parent.makedirs()
             with self.path.open("w") as dst:
                 dst.write(dict_to_yaml(self.dict))
 
         # shortcut to output path
         self.output_path = self.dict["output"]["path"]
         return self
 
@@ -116,15 +116,15 @@
         if self._tempdir:
             self._tempdir.rm(recursive=True, ignore_errors=True)
 
     def clear_output(self):
         # delete written output if any
         out_dir = (
             self._tempdir
-            or MPath(self.dict["config_dir"]) / self.dict["output"]["path"]
+            or MPath.from_inp(self.dict["config_dir"]) / self.dict["output"]["path"]
         )
         out_dir.rm(recursive=True, ignore_errors=True)
 
     def process_mp(self, tile=None, tile_zoom=None, batch_preprocess=True):
         """
         Return MapcheteProcess object used to test processes.
         """
@@ -140,19 +140,23 @@
             input=mp.config.get_inputs_for_tile(tile),
         )
 
     def mp(self, batch_preprocess=True):
         """
         Return Mapchete object from mapchete.open().
         """
-        if not self._mp:
-            self._mp = mapchete.open(self.dict)
-            if batch_preprocess:
-                self._mp.batch_preprocess()
-        return self._mp
+        from mapchete._executor import SequentialExecutor
+
+        with SequentialExecutor() as executor:
+            if not self._mp:
+                self._mp = mapchete.open(self.dict)
+                if batch_preprocess:
+                    self._mp.batch_preprocess(executor=executor)
+
+            return self._mp
 
     def first_process_tile(self, zoom=None):
         zoom = zoom or max(self.mp().config.zoom_levels)
         return next(self.mp().get_process_tiles(zoom))
 
 
 def get_process_mp(tile=None, zoom=0, input=None, params=None, metatiling=1, **kwargs):
```

### Comparing `mapchete-2023.6.1/mapchete/tile.py` & `mapchete-2023.6.2/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/types.py` & `mapchete-2023.6.2/mapchete/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/validate.py` & `mapchete-2023.6.2/mapchete/validate.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/cli/options.py` & `mapchete-2023.6.2/mapchete/cli/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import os
-from multiprocessing import cpu_count, get_all_start_methods
+from multiprocessing import get_all_start_methods
 
 import click
 import tilematrix
 from rasterio.enums import Resampling
 
 from mapchete.config import MULTIPROCESSING_DEFAULT_START_METHOD
 from mapchete.formats import available_output_formats
@@ -131,15 +131,15 @@
 
 
 # click options #
 #################
 opt_out_path = click.option(
     "--out-path",
     type=click.Path(),
-    default=MPath(os.getcwd()) / "output",
+    default=MPath.from_inp(os.getcwd()) / "output",
     help="Output path.",
 )
 opt_idx_out_dir = click.option(
     "--idx-out-dir", type=click.Path(), help="Index output directory."
 )
 opt_input_file = click.option(
     "--input-file",
```

### Comparing `mapchete-2023.6.1/mapchete/cli/default/convert.py` & `mapchete-2023.6.2/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/cli/default/cp.py` & `mapchete-2023.6.2/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/cli/default/create.py` & `mapchete-2023.6.2/mapchete/cli/default/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,26 @@
     process_file,
     out_format,
     out_path=None,
     pyramid_type=None,
     force=False,
 ):
     """Create an empty Mapchete and process file in a given directory."""
-    process_file = MPath(process_file)
-    mapchete_file = MPath(mapchete_file)
+    process_file = MPath.from_inp(process_file)
+    mapchete_file = MPath.from_inp(mapchete_file)
     if process_file.exists() or mapchete_file.exists():
         if not force:
             raise IOError("file(s) already exists")
 
-    out_path = out_path if out_path else MPath(os.getcwd()) / "output"
+    out_path = out_path if out_path else MPath.from_inp(os.getcwd()) / "output"
 
     # copy file template to target directory
     # Reads contents with UTF-8 encoding and returns str.
     process_template = str(files("mapchete.static").joinpath("process_template.py"))
-    process_file = MPath(os.getcwd()) / process_file
+    process_file = MPath.from_inp(os.getcwd()) / process_file
     copyfile(process_template, process_file)
 
     # modify and copy mapchete file template to target directory
     mapchete_template = str(
         files("mapchete.static").joinpath("mapchete_template.mapchete")
     )
```

### Comparing `mapchete-2023.6.1/mapchete/cli/default/execute.py` & `mapchete-2023.6.2/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/cli/default/formats.py` & `mapchete-2023.6.2/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/cli/default/index.py` & `mapchete-2023.6.2/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/cli/default/processes.py` & `mapchete-2023.6.2/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/cli/default/rm.py` & `mapchete-2023.6.2/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/cli/default/serve.py` & `mapchete-2023.6.2/mapchete/cli/default/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,17 @@
     debug=None,
 ):
     """Configure and create Flask app."""
     from flask import Flask, render_template_string
 
     app = Flask(__name__)
     mapchete_processes = {
-        str(MPath(MPath(mapchete_file).name).without_suffix()): mapchete.open(
+        str(
+            MPath.from_inp(MPath.from_inp(mapchete_file).name).without_suffix()
+        ): mapchete.open(
             mapchete_file,
             zoom=zoom,
             bounds=bounds,
             single_input_file=single_input_file,
             mode=mode,
             with_cache=True,
             debug=debug,
```

### Comparing `mapchete-2023.6.1/mapchete/cli/default/stac.py` & `mapchete-2023.6.2/mapchete/cli/default/stac.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import logging
-import os
 
 import click
 import fsspec
 import oyaml as yaml
 
 import mapchete
 from mapchete.cli import options
@@ -80,15 +79,15 @@
         with fsspec.open(item_metadata) as src:
             metadata = yaml.safe_load(src.read())
     else:
         metadata = default_item_metadata or {}
 
     item_id = item_id or metadata.get("id", default_id)
     logger.debug("use item ID %s", item_id)
-    item_path = item_path or MPath(default_basepath) / f"{item_id}.json"
+    item_path = item_path or MPath.from_inp(default_basepath) / f"{item_id}.json"
     item = tile_directory_stac_item(
         item_id=item_id,
         item_metadata=metadata,
         tile_pyramid=tile_pyramid,
         zoom_levels=zoom,
         bounds=bounds or default_bounds,
         bounds_crs=bounds_crs or default_bounds_crs,
@@ -103,18 +102,18 @@
     click.echo(item_json)
     if force or click.confirm(f"Write output to {item_path}?", abort=True):
         with fsspec.open(item_path, "w") as dst:
             dst.write(item_json)
 
 
 def output_info(inp):
-    path = MPath(inp)
+    path = MPath.from_inp(inp)
     if path.suffix == ".mapchete":
         conf = raw_conf(path)
-        default_basepath = MPath.from_dict(conf["output"])
+        default_basepath = MPath.from_inp(conf["output"])
         return (
             raw_conf_output_pyramid(conf),
             default_basepath,
             default_basepath.name,
             conf.get("bounds"),
             conf.get("bounds_crs"),
             conf.get("zoom_levels"),
```

### Comparing `mapchete-2023.6.1/mapchete/commands/_convert.py` & `mapchete-2023.6.2/mapchete/commands/_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,29 +172,29 @@
 
     msg_callback = msg_callback or _empty_callback
     if multi is not None:  # pragma: no cover
         warnings.warn("The 'multi' parameter is deprecated and is now named 'workers'")
     workers = workers or multi or cpu_count()
     creation_options = creation_options or {}
     bidx = [bidx] if isinstance(bidx, int) else bidx
-    tiledir = MPath(tiledir) if isinstance(tiledir, str) else tiledir
-    output = MPath(output)
+    tiledir = MPath.from_inp(tiledir) if isinstance(tiledir, str) else tiledir
+    output = MPath.from_inp(output)
     try:
         input_info = _get_input_info(tiledir)
         logger.debug("input params: %s", input_info)
         output_info = _get_output_info(output)
         logger.debug("output params: %s", output_info)
     except Exception as e:
         raise ValueError(e)
 
     if (
         isinstance(output_pyramid, (str, MPath))
         and output_pyramid not in tilematrix._conf.PYRAMID_PARAMS.keys()
     ):
-        output_pyramid = json.loads(MPath(output_pyramid).read_text())
+        output_pyramid = json.loads(MPath.from_inp(output_pyramid).read_text())
 
     # collect mapchete configuration
     mapchete_config = dict(
         process="mapchete.processes.convert",
         input=dict(inp=tiledir, clip=clip_geometry),
         pyramid=(
             dict(
```

### Comparing `mapchete-2023.6.1/mapchete/commands/_cp.py` & `mapchete-2023.6.2/mapchete/commands/_cp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Copy tiles between Tile Directories."""
 
 import logging
-import os
 import warnings
 from multiprocessing import cpu_count
 from typing import Callable, List, Tuple, Union
 
 from rasterio.crs import CRS
 from shapely.geometry import Point
 from shapely.geometry.base import BaseGeometry
@@ -109,16 +108,16 @@
         warnings.warn("The 'multi' parameter is deprecated and is now named 'workers'")
     workers = workers or multi or cpu_count()
     src_fs_opts = src_fs_opts or {}
     dst_fs_opts = dst_fs_opts or {}
     if zoom is None:  # pragma: no cover
         raise ValueError("zoom level(s) required")
 
-    src_tiledir = MPath(src_tiledir, **src_fs_opts)
-    dst_tiledir = MPath(dst_tiledir, **dst_fs_opts)
+    src_tiledir = MPath.from_inp(src_tiledir, **src_fs_opts)
+    dst_tiledir = MPath.from_inp(dst_tiledir, **dst_fs_opts)
     src_fs = src_tiledir.fs
     dst_fs = dst_tiledir.fs
 
     # open source tile directory
     with mapchete.open(
         src_tiledir,
         zoom=zoom,
```

### Comparing `mapchete-2023.6.1/mapchete/commands/_execute.py` & `mapchete-2023.6.2/mapchete/commands/_execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/commands/_index.py` & `mapchete-2023.6.2/mapchete/commands/_index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/commands/_rm.py` & `mapchete-2023.6.2/mapchete/commands/_rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/commons/clip.py` & `mapchete-2023.6.2/mapchete/commons/clip.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/commons/contours.py` & `mapchete-2023.6.2/mapchete/commons/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/commons/hillshade.py` & `mapchete-2023.6.2/mapchete/commons/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/__init__.py` & `mapchete-2023.6.2/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/base.py` & `mapchete-2023.6.2/mapchete/formats/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Main base classes for input and output formats.
 
 When writing a new driver, please inherit from these classes and implement the
 respective interfaces.
 """
 
 import logging
-import os
 import types
 import warnings
 from itertools import chain
 
 import numpy as np
 import numpy.ma as ma
 from shapely.geometry import shape
@@ -106,15 +105,14 @@
         -------
         file exists : bool
         """
         raise NotImplementedError
 
     def cleanup(self):
         """Optional cleanup function called when Mapchete exits."""
-        pass
 
     def add_preprocessing_task(
         self, func, fargs=None, fkwargs=None, key=None, geometry=None, bounds=None
     ):
         """
         Add longer running preprocessing function to be called right before processing.
 
@@ -226,15 +224,14 @@
 
     def __enter__(self):
         """Required for 'with' statement."""
         return self
 
     def __exit__(self, t, v, tb):
         """Clean up."""
-        pass
 
 
 class OutputDataBaseFunctions:
     write_in_parent_process = False
 
     def __init__(self, output_params, readonly=False, **kwargs):
         """Initialize."""
@@ -443,15 +440,15 @@
         Create directory and subdirectory if necessary.
 
         Parameters
         ----------
         tile : ``BufferedTile``
             must be member of output ``TilePyramid``
         """
-        self.get_path(tile).makedirs()
+        self.get_path(tile).parent.makedirs()
 
     def output_is_valid(self, process_data):
         """
         Check whether process output is allowed with output driver.
 
         Parameters
         ----------
@@ -504,15 +501,14 @@
         else:
             raise MapcheteProcessOutputError(
                 "invalid output type: %s" % type(process_data)
             )
 
     def close(self, exc_type=None, exc_value=None, exc_traceback=None):
         """Gets called if process is closed."""
-        pass
 
 
 class TileDirectoryOutputReader(OutputDataReader):
     def __init__(self, output_params, readonly=False):
         """Initialize."""
         super().__init__(output_params, readonly=readonly)
         if not readonly:
```

### Comparing `mapchete-2023.6.1/mapchete/formats/loaders.py` & `mapchete-2023.6.2/mapchete/formats/loaders.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/tools.py` & `mapchete-2023.6.2/mapchete/formats/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         fiona and rasterio. (default: True)
 
     Returns
     -------
     driver : string
         driver name
     """
-    input_file = MPath(input_file)
+    input_file = MPath.from_inp(input_file)
 
     # mapchete files can immediately be returned:
     if input_file.suffix == ".mapchete":
         return "Mapchete"
 
     # use the most common file extensions to quickly determine input driver for file:
     if quick:
@@ -309,15 +309,15 @@
 
     Parameters
     ----------
     output_params : dict
         Output parameters
     """
     if "path" in output_params:
-        metadata_path = MPath.from_dict(output_params) / "metadata.json"
+        metadata_path = MPath.from_inp(output_params) / "metadata.json"
         logger.debug("check for output %s", metadata_path)
         try:
             existing_params = read_output_metadata(metadata_path)
             logger.debug("%s exists", metadata_path)
             logger.debug("existing output parameters: %s", pformat(existing_params))
             current_params = dump_metadata(output_params)
             logger.debug("current output parameters: %s", pformat(current_params))
```

### Comparing `mapchete-2023.6.1/mapchete/formats/default/_fiona_base.py` & `mapchete-2023.6.2/mapchete/formats/default/_fiona_base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/default/flatgeobuf.py` & `mapchete-2023.6.2/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/default/geobuf.py` & `mapchete-2023.6.2/mapchete/formats/default/geobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/default/geojson.py` & `mapchete-2023.6.2/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/default/gtiff.py` & `mapchete-2023.6.2/mapchete/formats/default/gtiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,15 +503,14 @@
                 raise MapcheteConfigError(
                     "single GTiff file already exists, use overwrite mode to replace"
                 )
             elif not path_is_remote(self.path):
                 logger.debug("remove existing file: %s", self.path)
                 os.remove(self.path)
         # create output directory if necessary
-        self.path.makedirs()
         logger.debug("open output file: %s", self.path)
         self._ctx = ExitStack()
         self.dst = self._ctx.enter_context(
             rasterio_write(self.path, "w+", **self._profile)
         )
 
     def read(self, output_tile, **kwargs):
@@ -730,8 +729,7 @@
 
     def __enter__(self):
         """Enable context manager."""
         return self
 
     def __exit__(self, t, v, tb):
         """Clear cache on close."""
-        pass
```

### Comparing `mapchete-2023.6.1/mapchete/formats/default/mapchete_input.py` & `mapchete-2023.6.2/mapchete/formats/default/mapchete_input.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/default/png.py` & `mapchete-2023.6.2/mapchete/formats/default/png.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/default/png_hillshade.py` & `mapchete-2023.6.2/mapchete/formats/default/png_hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/formats/default/raster_file.py` & `mapchete-2023.6.2/mapchete/formats/default/raster_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 self._src_transform = src.transform
             self._src_bbox = box(*self._src_bounds)
 
         self._cache_task = f"cache_{self.path}"
         if "abstract" in input_params and "cache" in input_params["abstract"]:
             if isinstance(input_params["abstract"]["cache"], dict):
                 if "path" in input_params["abstract"]["cache"]:
-                    cached_path = MPath.from_dict(input_params["abstract"]["cache"])
+                    cached_path = MPath.from_inp(input_params["abstract"]["cache"])
                     if cached_path.is_absolute():
                         self._cached_path = cached_path
                     else:  # pragma: no cover
                         self._cached_path = cached_path.absolute_path(
                             base_dir=input_params["conf_dir"],
                         )
                 else:  # pragma: no cover
```

### Comparing `mapchete-2023.6.1/mapchete/formats/default/tile_directory.py` & `mapchete-2023.6.2/mapchete/formats/default/tile_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         super().__init__(input_params, **kwargs)
         self._read_as_tiledir_func = None
         logger.debug("InputData params: %s", input_params)
         # populate internal parameters initially depending on whether this input was
         # defined as simple or abstract input
         self._params = input_params.get("abstract") or dict(path=input_params["path"])
         # construct path and append optional filesystem options
-        self.path = MPath.from_dict(self._params).absolute_path(
+        self.path = MPath.from_inp(self._params).absolute_path(
             input_params.get("conf_dir")
         )
         if "abstract" in input_params:
             # define pyramid either by hardcoded given values or by existing metadata.json
             if "grid" in self._params:
                 self.td_pyramid = BufferedTilePyramid(
                     self._params["grid"],
```

### Comparing `mapchete-2023.6.1/mapchete/formats/default/vector_file.py` & `mapchete-2023.6.2/mapchete/formats/default/vector_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             if "abstract" in input_params
             else input_params["path"]
         )
         self._cache_task = f"cache_{self.path}"
         if "abstract" in input_params and "cache" in input_params["abstract"]:
             if isinstance(input_params["abstract"]["cache"], dict):
                 if "path" in input_params["abstract"]["cache"]:
-                    cached_path = MPath.from_dict(input_params["abstract"]["cache"])
+                    cached_path = MPath.from_inp(input_params["abstract"]["cache"])
                     if cached_path.is_absolute():
                         self._cached_path = cached_path
                     else:  # pragma: no cover
                         self._cached_path = cached_path.absolute_path(
                             base_dir=input_params["conf_dir"],
                         )
                 else:  # pragma: no cover
```

### Comparing `mapchete-2023.6.1/mapchete/io/__init__.py` & `mapchete-2023.6.2/mapchete/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/io/_geometry_operations.py` & `mapchete-2023.6.2/mapchete/io/_geometry_operations.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/io/_json.py` & `mapchete-2023.6.2/mapchete/io/_json.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 logger = logging.getLogger(__name__)
 
 
 def write_json(path, params, fs=None, **kwargs):
     """Write local or remote."""
     logger.debug(f"write {params} to {path}")
-    path = MPath(path, fs=fs, **kwargs)
-    path.makedirs()
+    path = MPath.from_inp(path, fs=fs, **kwargs)
+    path.parent.makedirs()
     with path.open(mode="w") as dst:
         json.dump(params, dst, sort_keys=True, indent=4)
 
 
 def read_json(path, fs=None, **kwargs):
     """Read local or remote."""
-    path = MPath(path, fs=fs, **kwargs)
+    path = MPath.from_inp(path, fs=fs, **kwargs)
     try:
         with path.open(mode="r") as src:
             return json.loads(src.read())
     except Exception as e:
         if path.exists():  # pragma: no cover
             logger.exception(e)
             raise e
```

### Comparing `mapchete-2023.6.1/mapchete/io/_misc.py` & `mapchete-2023.6.2/mapchete/io/_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,22 +172,22 @@
 def get_boto3_bucket(bucket_name):  # pragma: no cover
     """Return boto3.Bucket object from bucket name."""
     raise DeprecationWarning("get_boto3_bucket() is deprecated")
 
 
 def copy(src_path, dst_path, src_fs=None, dst_fs=None, overwrite=False):
     """Copy path from one place to the other."""
-    src_path = MPath(src_path, fs=src_fs)
-    dst_path = MPath(dst_path, fs=dst_fs)
+    src_path = MPath.from_inp(src_path, fs=src_fs)
+    dst_path = MPath.from_inp(dst_path, fs=dst_fs)
 
     if not overwrite and dst_path.fs.exists(dst_path):
         raise IOError(f"{dst_path} already exists")
 
     # create parent directories on local filesystems
-    dst_path.makedirs()
+    dst_path.parent.makedirs()
 
     # copy either within a filesystem or between filesystems
     if src_path.fs == dst_path.fs:
         src_path.fs.copy(str(src_path), str(dst_path))
     else:
         with src_path.open("rb") as src:
             with dst_path.open("wb") as dst:
```

### Comparing `mapchete-2023.6.1/mapchete/io/raster.py` & `mapchete-2023.6.2/mapchete/io/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 @contextmanager
 def rasterio_open(path, mode="r", **kwargs):
     """Call rasterio.open but set environment correctly and return custom writer if needed."""
-    path = MPath(path)
+    path = MPath.from_inp(path)
 
     if "w" in mode:
         with rasterio_write(path, mode=mode, **kwargs) as dst:
             yield dst
 
     else:
         with rasterio_read(path, mode=mode, **kwargs) as src:
@@ -49,14 +49,15 @@
 
 
 @contextmanager
 def rasterio_read(path, mode="r", **kwargs):
     """
     Wrapper around rasterio.open but rasterio.Env is set according to path properties.
     """
+    path = MPath.from_inp(path)
     with path.rio_env() as env:
         logger.debug("reading %s with GDAL options %s", str(path), env.options)
         with rasterio.open(path, mode=mode, **kwargs) as src:
             yield src
 
 
 @contextmanager
@@ -79,27 +80,30 @@
     kwargs : dict
         Keyword arguments to be passed on to rasterio.open()
 
     Returns
     -------
     RasterioRemoteWriter if target is remote, otherwise return rasterio.open().
     """
+    path = MPath.from_inp(path)
+
     if path.is_remote():
         if "s3" in path.protocols:  # pragma: no cover
             try:
                 import boto3
             except ImportError:
                 raise ImportError("please install [s3] extra to write remote files")
         with RasterioRemoteWriter(
             path, fs=fs, in_memory=in_memory, *args, **kwargs
         ) as dst:
             yield dst
     else:
         with path.rio_env() as env:
-            logger.debug("reading %s with GDAL options %s", str(path), env.options)
+            logger.debug("writing %s with GDAL options %s", str(path), env.options)
+            path.parent.makedirs(exist_ok=True)
             with rasterio.open(path, mode=mode, *args, **kwargs) as dst:
                 yield dst
 
 
 class ReferencedRaster:
     """
     A loose in-memory representation of a rasterio dataset.
@@ -248,15 +252,15 @@
         GDAL options passed on to rasterio.Env()
 
     Returns
     -------
     raster : MaskedArray
     """
     input_files = [
-        MPath(input_file)
+        MPath.from_inp(input_file)
         for input_file in (
             input_files if isinstance(input_files, list) else [input_files]
         )
     ]
     if len(input_files) == 0:  # pragma: no cover
         raise ValueError("no input given")
     try:
@@ -1267,37 +1271,36 @@
     overwrite : bool
         Overwrite output file. (default: False)
     skip_exists : bool
         Skip conversion if outpu already exists. (default: True)
     kwargs : mapping
         Creation parameters passed on to output file.
     """
-    inp = MPath(inp)
-    out = MPath(out)
+    inp = MPath.from_inp(inp)
+    out = MPath.from_inp(out)
     if out.exists():
         if not exists_ok:
             raise OSError(f"{str(out)} already exists")
         elif not overwrite:
             logger.debug("output %s already exists and will not be overwritten")
             return
     kwargs = kwargs or {}
     if kwargs:
         logger.debug("convert raster file %s to %s using %s", inp, out, kwargs)
         with rasterio_open(inp, "r") as src:
-            out.makedirs()
             with rasterio_open(out, mode="w", **{**src.meta, **kwargs}) as dst:
                 dst.write(src.read())
     else:
         logger.debug("copy %s to %s", inp, (out))
-        out.makedirs()
+        out.parent.makedirs()
         copy(inp, out, overwrite=overwrite)
 
 
 def read_raster(inp, **kwargs):
-    inp = MPath(inp)
+    inp = MPath.from_inp(inp)
     logger.debug(f"reading {str(inp)} into memory")
     with rasterio_open(inp, "r") as src:
         return ReferencedRaster(
             data=src.read(masked=True),
             affine=src.transform,
             bounds=src.bounds,
             crs=src.crs,
```

### Comparing `mapchete-2023.6.1/mapchete/io/vector.py` & `mapchete-2023.6.2/mapchete/io/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 @contextmanager
 def fiona_open(path, mode="r", **kwargs):
     """Call fiona.open but set environment correctly and return custom writer if needed."""
-    path = MPath(path)
+    path = MPath.from_inp(path)
 
     if "w" in mode:
         with fiona_write(path, mode=mode, **kwargs) as dst:
             yield dst
 
     else:
         with fiona_read(path, mode=mode, **kwargs) as src:
@@ -56,14 +56,16 @@
 
 
 @contextmanager
 def fiona_read(path, mode="r", **kwargs):
     """
     Wrapper around fiona.open but fiona.Env is set according to path properties.
     """
+    path = MPath.from_inp(path)
+
     with path.fio_env() as env:
         logger.debug("reading %s with GDAL options %s", str(path), env.options)
         with fiona.open(str(path), mode=mode, **kwargs) as src:
             yield src
 
 
 @contextmanager
@@ -86,27 +88,29 @@
     kwargs : dict
         Keyword arguments to be passed on to fiona.open()
 
     Returns
     -------
     FionaRemoteWriter if target is remote, otherwise return fiona.open().
     """
-    path = MPath(path)
+    path = MPath.from_inp(path)
     if path.is_remote():
         if "s3" in path.protocols:  # pragma: no cover
             try:
                 import boto3
             except ImportError:
                 raise ImportError("please install [s3] extra to write remote files")
         with FionaRemoteWriter(
             path, fs=fs, in_memory=in_memory, *args, **kwargs
         ) as dst:
             yield dst
     else:
-        with path.fio_env():
+        with path.fio_env() as env:
+            logger.debug("writing %s with GDAL options %s", str(path), env.options)
+            path.parent.makedirs(exist_ok=True)
             with fiona.open(str(path), mode=mode, *args, **kwargs) as dst:
                 yield dst
 
 
 def read_vector_window(
     inp, tile, validity_check=True, clip_to_crs_bounds=False, skip_missing_files=False
 ):
@@ -209,15 +213,15 @@
         output schema for fiona
     out_tile : ``BufferedTile``
         tile used for output extent
     out_path : string
         output path for file
     """
     # Delete existing file.
-    out_path = MPath(out_path)
+    out_path = MPath.from_inp(out_path)
     out_path.rm(ignore_errors=True)
     out_features = []
     for feature in in_data:
         try:
             # clip feature geometry to tile bounding box and append for writing
             clipped = clean_geometry_type(
                 to_shape(feature["geometry"]).intersection(out_tile.bbox),
@@ -584,34 +588,33 @@
     overwrite : bool
         Overwrite output file. (default: False)
     skip_exists : bool
         Skip conversion if outpu already exists. (default: True)
     kwargs : mapping
         Creation parameters passed on to output file.
     """
-    inp = MPath(inp)
-    out = MPath(out)
+    inp = MPath.from_inp(inp)
+    out = MPath.from_inp(out)
     if out.exists():
         if not exists_ok:
             raise IOError(f"{out} already exists")
         elif not overwrite:
             logger.debug("output %s already exists and will not be overwritten")
             return
         else:
             fs_from_path(out).rm(out)
     kwargs = kwargs or {}
     if kwargs:
         logger.debug("convert vector file %s to %s using %s", str(inp), out, kwargs)
         with fiona_open(inp, "r") as src:
-            out.makedirs()
             with fiona_open(out, mode="w", **{**src.meta, **kwargs}) as dst:
                 dst.writerecords(src)
     else:
         logger.debug("copy %s to %s", str(inp), str(out))
-        out.makedirs()
+        out.parent.makedirs()
         copy(inp, out, overwrite=overwrite)
 
 
 def read_vector(inp, index="rtree"):
     with fiona_open(inp, "r") as src:
         return IndexedFeatures(src, index=index)
```

### Comparing `mapchete-2023.6.1/mapchete/processes/__init__.py` & `mapchete-2023.6.2/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/processes/contours.py` & `mapchete-2023.6.2/mapchete/processes/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/processes/convert.py` & `mapchete-2023.6.2/mapchete/processes/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/processes/hillshade.py` & `mapchete-2023.6.2/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/processes/examples/example_process.py` & `mapchete-2023.6.2/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/static/index.html` & `mapchete-2023.6.2/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/mapchete/static/process_template.py` & `mapchete-2023.6.2/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/LICENSE` & `mapchete-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/README.rst` & `mapchete-2023.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/pyproject.toml` & `mapchete-2023.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.1/PKG-INFO` & `mapchete-2023.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapchete
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

