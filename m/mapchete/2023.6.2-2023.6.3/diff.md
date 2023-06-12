# Comparing `tmp/mapchete-2023.6.2.tar.gz` & `tmp/mapchete-2023.6.3.tar.gz`

## Comparing `mapchete-2023.6.2.tar` & `mapchete-2023.6.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/__init__.py
--rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_core.py
--rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_executor.py
--rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_processing.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_registered.py
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_tasks.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_timer.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/_user_process.py
--rw-r--r--   0        0        0    48622 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/config.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/errors.py
--rw-r--r--   0        0        0    17833 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/index.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/log.py
--rw-r--r--   0        0        0    24958 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/path.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/stac.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/testing.py
--rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/tile.py
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/types.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/main.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/__init__.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commons/contours.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    20760 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/loaders.py
--rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/_json.py
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/_misc.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/_path.py
--rw-r--r--   0        0        0    44156 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/raster.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/settings.py
--rw-r--r--   0        0        0    22010 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/io/vector.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/static/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/static/index.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.2/mapchete/static/process_template.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.2/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.2/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.2/README.rst
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.2/pyproject.toml
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.2/PKG-INFO
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/__init__.py
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_core.py
+-rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_executor.py
+-rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_processing.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_registered.py
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_tasks.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_timer.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_user_process.py
+-rw-r--r--   0        0        0    48622 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/config.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/errors.py
+-rw-r--r--   0        0        0    17833 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/index.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/log.py
+-rw-r--r--   0        0        0    25097 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/path.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/stac.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/testing.py
+-rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/tile.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/types.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/main.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_convert.py
+-rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_cp.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_execute.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_index.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_rm.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commons/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commons/clip.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commons/contours.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commons/hillshade.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20760 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/geobuf.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/_path.py
+-rw-r--r--   0        0        0    44448 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/raster.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/settings.py
+-rw-r--r--   0        0        0    22010 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/static/index.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.3/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.3/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.3/README.rst
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.3/pyproject.toml
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.3/PKG-INFO
```

### Comparing `mapchete-2023.6.2/mapchete/__init__.py` & `mapchete-2023.6.3/mapchete/__init__.py`

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
-__version__ = "2023.6.2"
+__version__ = "2023.6.3"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `mapchete-2023.6.2/mapchete/_core.py` & `mapchete-2023.6.3/mapchete/_core.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/_executor.py` & `mapchete-2023.6.3/mapchete/_executor.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/_processing.py` & `mapchete-2023.6.3/mapchete/_processing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/_registered.py` & `mapchete-2023.6.3/mapchete/_registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/_tasks.py` & `mapchete-2023.6.3/mapchete/_tasks.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/_timer.py` & `mapchete-2023.6.3/mapchete/_timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/_user_process.py` & `mapchete-2023.6.3/mapchete/_user_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/config.py` & `mapchete-2023.6.3/mapchete/config.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/errors.py` & `mapchete-2023.6.3/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/index.py` & `mapchete-2023.6.3/mapchete/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/log.py` & `mapchete-2023.6.3/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/path.py` & `mapchete-2023.6.3/mapchete/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,18 @@
             return MPath.from_dict(inp)
         elif isinstance(inp, str):
             return MPath(inp, **kwargs)
         elif isinstance(inp, MPath):
             if kwargs:
                 return MPath(inp, **kwargs)
             return inp
+        elif hasattr(inp, "__fspath__"):  # pragma: no cover
+            return MPath(inp.__fspath__(), **kwargs)
         else:  # pragma: no cover
+            breakpoint()
             raise TypeError(f"cannot construct MPath object from {inp}")
 
     def to_dict(self) -> dict:
         return dict(
             path=self._path_str,
             storage_options=self._storage_options,
             fs=self.fs,
```

### Comparing `mapchete-2023.6.2/mapchete/stac.py` & `mapchete-2023.6.3/mapchete/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/testing.py` & `mapchete-2023.6.3/mapchete/testing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/tile.py` & `mapchete-2023.6.3/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/types.py` & `mapchete-2023.6.3/mapchete/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/validate.py` & `mapchete-2023.6.3/mapchete/validate.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/options.py` & `mapchete-2023.6.3/mapchete/cli/options.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/convert.py` & `mapchete-2023.6.3/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/cp.py` & `mapchete-2023.6.3/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/create.py` & `mapchete-2023.6.3/mapchete/cli/default/create.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/execute.py` & `mapchete-2023.6.3/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/formats.py` & `mapchete-2023.6.3/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/index.py` & `mapchete-2023.6.3/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/processes.py` & `mapchete-2023.6.3/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/rm.py` & `mapchete-2023.6.3/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/serve.py` & `mapchete-2023.6.3/mapchete/cli/default/serve.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/cli/default/stac.py` & `mapchete-2023.6.3/mapchete/cli/default/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/commands/_convert.py` & `mapchete-2023.6.3/mapchete/commands/_convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/commands/_cp.py` & `mapchete-2023.6.3/mapchete/commands/_cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/commands/_execute.py` & `mapchete-2023.6.3/mapchete/commands/_execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/commands/_index.py` & `mapchete-2023.6.3/mapchete/commands/_index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/commands/_rm.py` & `mapchete-2023.6.3/mapchete/commands/_rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/commons/clip.py` & `mapchete-2023.6.3/mapchete/commons/clip.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/commons/contours.py` & `mapchete-2023.6.3/mapchete/commons/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/commons/hillshade.py` & `mapchete-2023.6.3/mapchete/commons/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/__init__.py` & `mapchete-2023.6.3/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/base.py` & `mapchete-2023.6.3/mapchete/formats/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/loaders.py` & `mapchete-2023.6.3/mapchete/formats/loaders.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/tools.py` & `mapchete-2023.6.3/mapchete/formats/tools.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/_fiona_base.py` & `mapchete-2023.6.3/mapchete/formats/default/_fiona_base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/flatgeobuf.py` & `mapchete-2023.6.3/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/geobuf.py` & `mapchete-2023.6.3/mapchete/formats/default/geobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/geojson.py` & `mapchete-2023.6.3/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/gtiff.py` & `mapchete-2023.6.3/mapchete/formats/default/gtiff.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/mapchete_input.py` & `mapchete-2023.6.3/mapchete/formats/default/mapchete_input.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/png.py` & `mapchete-2023.6.3/mapchete/formats/default/png.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/png_hillshade.py` & `mapchete-2023.6.3/mapchete/formats/default/png_hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/raster_file.py` & `mapchete-2023.6.3/mapchete/formats/default/raster_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/tile_directory.py` & `mapchete-2023.6.3/mapchete/formats/default/tile_directory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/formats/default/vector_file.py` & `mapchete-2023.6.3/mapchete/formats/default/vector_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/io/__init__.py` & `mapchete-2023.6.3/mapchete/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/io/_geometry_operations.py` & `mapchete-2023.6.3/mapchete/io/_geometry_operations.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/io/_json.py` & `mapchete-2023.6.3/mapchete/io/_json.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/io/_misc.py` & `mapchete-2023.6.3/mapchete/io/_misc.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/io/raster.py` & `mapchete-2023.6.3/mapchete/io/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,34 +104,39 @@
                 yield dst
 
 
 class ReferencedRaster:
     """
     A loose in-memory representation of a rasterio dataset.
 
-    Useful to ship cached raster files between worker nodes.
+    Useful to ship cached raster files between dask worker nodes.
     """
 
     def __init__(
         self,
         data: Union[np.ndarray, ma.masked_array] = None,
         transform: Affine = None,
         bounds: Union[List[float], Tuple[float], Bounds] = None,
         crs: Union[str, rasterio.crs.CRS] = None,
         nodata: Union[int, float] = None,
         driver: str = None,
         **kwargs,
     ):
-        if data.ndim == 2:
+        if data.ndim == 1:  # pragma: no cover
+            raise TypeError("input array must have at least 2 dimensions")
+        elif data.ndim == 2:
             self.count = 1
             self.height, self.width = data.shape
         elif data.ndim == 3:
             self.count, self.height, self.width = data.shape
         else:  # pragma: no cover
-            raise TypeError("input array must be 2- or 3-dimensional")
+            # for arrays with more dimensions, the first axis is assumed to be
+            # the bands and the last two the width and height
+            self.count = data.shape[0]
+            self.height, self.width = data.shape[-2:]
         transform = transform or kwargs.get("affine")
         if transform is None:  # pragma: no cover
             raise ValueError("georeference given")
         self.data = data
         self.driver = driver
         self.dtype = self.data.dtype
         self.nodata = nodata
```

### Comparing `mapchete-2023.6.2/mapchete/io/settings.py` & `mapchete-2023.6.3/mapchete/io/settings.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/io/vector.py` & `mapchete-2023.6.3/mapchete/io/vector.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/processes/__init__.py` & `mapchete-2023.6.3/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/processes/contours.py` & `mapchete-2023.6.3/mapchete/processes/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/processes/convert.py` & `mapchete-2023.6.3/mapchete/processes/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/processes/hillshade.py` & `mapchete-2023.6.3/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/processes/examples/example_process.py` & `mapchete-2023.6.3/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/static/index.html` & `mapchete-2023.6.3/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/mapchete/static/process_template.py` & `mapchete-2023.6.3/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/LICENSE` & `mapchete-2023.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/README.rst` & `mapchete-2023.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/pyproject.toml` & `mapchete-2023.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.2/PKG-INFO` & `mapchete-2023.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapchete
-Version: 2023.6.2
+Version: 2023.6.3
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

