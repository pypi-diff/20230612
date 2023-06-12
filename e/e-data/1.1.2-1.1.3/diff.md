# Comparing `tmp/e-data-1.1.2.tar.gz` & `tmp/e-data-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-data-1.1.2.tar", last modified: Sun Jun 11 10:11:30 2023, max compression
+gzip compressed data, was "e-data-1.1.3.tar", last modified: Mon Jun 12 16:04:28 2023, max compression
```

## Comparing `e-data-1.1.2.tar` & `e-data-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.496630 e-data-1.1.2/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)      193 2023-06-11 10:01:58.000000 e-data-1.1.2/MANIFEST.in
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     6568 2023-06-11 10:11:30.496630 e-data-1.1.2/PKG-INFO
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     4860 2023-06-11 10:01:58.000000 e-data-1.1.2/README.md
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.484630 e-data-1.1.2/e_data.egg-info/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     6568 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/PKG-INFO
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)      499 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/SOURCES.txt
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        1 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/dependency_links.txt
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)      119 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/requires.txt
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        6 2023-06-11 10:11:30.000000 e-data-1.1.2/e_data.egg-info/top_level.txt
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.488630 e-data-1.1.2/edata/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/__init__.py
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.488630 e-data-1.1.2/edata/connectors/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/connectors/__init__.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)    15204 2023-06-11 10:10:24.000000 e-data-1.1.2/edata/connectors/datadis.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     1990 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/connectors/redata.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     3828 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/definitions.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)    22473 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/helpers.py
-drwxr-xr-x   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:11:30.492630 e-data-1.1.2/edata/processors/
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/__init__.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)      624 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/base.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     6224 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/billing.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     2330 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/consumption.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     1334 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/maximeter.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     5155 2023-06-11 10:01:58.000000 e-data-1.1.2/edata/processors/utils.py
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)       54 2023-06-11 10:11:30.496630 e-data-1.1.2/setup.cfg
--rw-r--r--   0 vmayor    (1000) vmayor    (1000)     4260 2023-06-11 10:10:34.000000 e-data-1.1.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.428333 e-data-1.1.3/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    35149 2023-06-11 10:01:58.000000 e-data-1.1.3/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      193 2023-06-11 10:01:58.000000 e-data-1.1.3/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-12 16:04:28.428333 e-data-1.1.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4860 2023-06-11 10:01:58.000000 e-data-1.1.3/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.392333 e-data-1.1.3/e_data.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-12 16:04:27.000000 e-data-1.1.3/e_data.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      507 2023-06-12 16:04:28.000000 e-data-1.1.3/e_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-12 16:04:27.000000 e-data-1.1.3/e_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      134 2023-06-12 16:04:27.000000 e-data-1.1.3/e_data.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-06-12 16:04:27.000000 e-data-1.1.3/e_data.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.396333 e-data-1.1.3/edata/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.3/edata/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.404333 e-data-1.1.3/edata/connectors/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 12:18:54.000000 e-data-1.1.3/edata/connectors/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15204 2023-06-12 15:54:38.000000 e-data-1.1.3/edata/connectors/datadis.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1990 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/connectors/redata.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3828 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/definitions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22473 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/helpers.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.428333 e-data-1.1.3/edata/processors/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.3/edata/processors/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6224 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/billing.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2330 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/consumption.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1334 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/maximeter.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5155 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       54 2023-06-12 16:04:28.436333 e-data-1.1.3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4283 2023-06-12 16:03:17.000000 e-data-1.1.3/setup.py
```

### Comparing `e-data-1.1.2/PKG-INFO` & `e-data-1.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,128 +1,128 @@
 Metadata-Version: 2.1
 Name: e-data
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python library for managing spanish energy data from various web providers
 Home-page: https://github.com/uvejota/python-edata
 Author: VMG
 Author-email: vmayorg@outlook.es
 License: GPLv3
-Description: 
-        [![Downloads](https://pepy.tech/badge/e-data)](https://pepy.tech/project/e-data)
-        [![Downloads](https://pepy.tech/badge/e-data/month)](https://pepy.tech/project/e-data)
-        [![Downloads](https://pepy.tech/badge/e-data/week)](https://pepy.tech/project/e-data)
-        
-        # python-edata
-        
-        Este paquete proporciona herramientas para la descarga de tus datos de consumo eléctrico (desde Datadis.es) y su posterior procesado. La motivación principal es que conocer el consumo puede ayudarnos a reducirlo, e incluso a elegir una tarifa que mejor se adapte a nuestras necesidades. A día de hoy sus capacidades de facturación (€) son limitadas, soporta PVPC (según disponibilidad de datos de REData) y tarificación fija por tramos. Es el corazón de la integración [homeassistant-edata](https://github.com/uvejota/homeassistant-edata).
-        
-        _**Esta herramienta no mantiene ningún tipo de vinculación con los proveedores de datos anteriormente mencionados, simplemente consulta la información disponible y facilita su posterior análisis.**_
-        
-        ## Instalación
-        
-        Puedes instalar la última versión estable mediante:
-        
-        ``` bash
-        pip install e-data
-        ```
-        
-        Si quieres probar la versión `dev` o contribuir a su desarrollo, clona este repositorio e instala manualmente las dependencias:
-        
-        ``` bash
-        pip install -r requirements.txt
-        ```
-        
-        ## Estructura
-        
-        El paquete consta de tres módulos diferenciados:
-        
-        * **Conectores** (módulo `connectors`), para definir los métodos de consulta a los diferentes proveedores: Datadis y REData.
-        * **Procesadores** (módulo `processors`), para procesar datos de consumo, maxímetro, o coste (tarificación). Ahora mismo consta de tres procesadores: `billing`, `consumption` y `maximeter`, además de algunas utilidades ubicadas en `utils`. Los procesadores deben heredar de la clase Processor definida en `base.py`
-        * **Ayudantes** (módulo `helpers`), para ayudar en el uso y gestión de los anteriores, presentando de momento un único ayudante llamado `EdataHelper` que te permite recopilar `X` días de datos (por defecto 365) y automáticamente procesarlos. Los datos son almacenados en la variable `data`, mientras que los atributos autocalculados son almacenados en la variable `attributes`. Por lo general, primero utilizan los conectores y luego procesan los datos, gestionando varias tareas de recuperación (principalmente para Datadis).
-        
-        Estos módulos corresponden a la siguiente estructura del paquete:
-        
-        ```
-        edata/
-            · __init__.py
-            · connectors/
-                · __init__.py
-                · datadis.py
-                · redata.py
-            · processors/
-                · __init__.py
-                · base.py
-                · billing.py
-                · consumption.py
-                · maximeter.py
-                · utils.py
-            · helpers.py
-        ```
-        
-        ## Ejemplo de uso
-        
-        Partimos de que tenemos credenciales en Datadis.es. Algunas aclaraciones:
-        * No es necesario solicitar API pública en el registro (se utilizará la API privada habilitada por defecto)
-        * El username suele ser el NIF del titular
-        * Copie el CUPS de la web de Datadis, algunas comercializadoras adhieren caracteres adicionales en el CUPS mostrado en su factura.
-        * La herramienta acepta el uso de NIF autorizado para consultar el suministro de otro titular.
-        
-        ``` python
-        from datetime import datetime
-        import json
-        
-        # importamos definiciones de datos que nos interesen
-        from edata.definitions import PricingRules
-        # importamos el ayudante
-        from edata.helpers import EdataHelper
-        # importamos el procesador de utilidades
-        from edata.processors import utils
-        
-        # Preparar reglas de tarificación (si se quiere)
-        PRICING_RULES_PVPC = PricingRules(
-            p1_kw_year_eur=30.67266,
-            p2_kw_year_eur=1.4243591,
-            meter_month_eur=0.81,
-            market_kw_year_eur=3.113,
-            electricity_tax=1.0511300560,
-            iva_tax=1.05,
-            # podemos rellenar los siguientes campos si quisiéramos precio fijo (y no pvpc)
-            p1_kwh_eur=None,
-            p2_kwh_eur=None,
-            p3_kwh_eur=None,
-        )
-        
-        # Instanciar el helper
-        # 'authorized_nif' permite indicar el NIF de la persona que nos autoriza a consultar su CUPS.
-        # 'data' permite "cargar" al helper datos anteriores (resultado edata.data de una ejecución anterior), para evitar volver a consultar los mismos.
-        edata = EdataHelper(
-                    "datadis_user",
-                    "datadis_password",
-                    "cups",
-                    datadis_authorized_nif=None,
-                    pricing_rules=PRICING_RULES_PVPC, # si se le pasa None, no aplica tarificación
-                    data=None, # aquí podríamos cargar datos anteriores
-                )
-        
-        # Solicitar actualización de todo el histórico (se almacena en edata.data)
-        edata.update(date_from=datetime(1970, 1, 1), date_to=datetime.today())
-        
-        # volcamos todo lo obtenido a un fichero
-        with open("backup.json", "w") as file:
-            json.dump(utils.serialize_dict(edata.data), file) # se puede utilizar deserialize_dict para la posterior lectura del backup
-        
-        # Imprimir atributos
-        print(edata.attributes)
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+[![Downloads](https://pepy.tech/badge/e-data)](https://pepy.tech/project/e-data)
+[![Downloads](https://pepy.tech/badge/e-data/month)](https://pepy.tech/project/e-data)
+[![Downloads](https://pepy.tech/badge/e-data/week)](https://pepy.tech/project/e-data)
+
+# python-edata
+
+Este paquete proporciona herramientas para la descarga de tus datos de consumo eléctrico (desde Datadis.es) y su posterior procesado. La motivación principal es que conocer el consumo puede ayudarnos a reducirlo, e incluso a elegir una tarifa que mejor se adapte a nuestras necesidades. A día de hoy sus capacidades de facturación (€) son limitadas, soporta PVPC (según disponibilidad de datos de REData) y tarificación fija por tramos. Es el corazón de la integración [homeassistant-edata](https://github.com/uvejota/homeassistant-edata).
+
+_**Esta herramienta no mantiene ningún tipo de vinculación con los proveedores de datos anteriormente mencionados, simplemente consulta la información disponible y facilita su posterior análisis.**_
+
+## Instalación
+
+Puedes instalar la última versión estable mediante:
+
+``` bash
+pip install e-data
+```
+
+Si quieres probar la versión `dev` o contribuir a su desarrollo, clona este repositorio e instala manualmente las dependencias:
+
+``` bash
+pip install -r requirements.txt
+```
+
+## Estructura
+
+El paquete consta de tres módulos diferenciados:
+
+* **Conectores** (módulo `connectors`), para definir los métodos de consulta a los diferentes proveedores: Datadis y REData.
+* **Procesadores** (módulo `processors`), para procesar datos de consumo, maxímetro, o coste (tarificación). Ahora mismo consta de tres procesadores: `billing`, `consumption` y `maximeter`, además de algunas utilidades ubicadas en `utils`. Los procesadores deben heredar de la clase Processor definida en `base.py`
+* **Ayudantes** (módulo `helpers`), para ayudar en el uso y gestión de los anteriores, presentando de momento un único ayudante llamado `EdataHelper` que te permite recopilar `X` días de datos (por defecto 365) y automáticamente procesarlos. Los datos son almacenados en la variable `data`, mientras que los atributos autocalculados son almacenados en la variable `attributes`. Por lo general, primero utilizan los conectores y luego procesan los datos, gestionando varias tareas de recuperación (principalmente para Datadis).
+
+Estos módulos corresponden a la siguiente estructura del paquete:
+
+```
+edata/
+    · __init__.py
+    · connectors/
+        · __init__.py
+        · datadis.py
+        · redata.py
+    · processors/
+        · __init__.py
+        · base.py
+        · billing.py
+        · consumption.py
+        · maximeter.py
+        · utils.py
+    · helpers.py
+```
+
+## Ejemplo de uso
+
+Partimos de que tenemos credenciales en Datadis.es. Algunas aclaraciones:
+* No es necesario solicitar API pública en el registro (se utilizará la API privada habilitada por defecto)
+* El username suele ser el NIF del titular
+* Copie el CUPS de la web de Datadis, algunas comercializadoras adhieren caracteres adicionales en el CUPS mostrado en su factura.
+* La herramienta acepta el uso de NIF autorizado para consultar el suministro de otro titular.
+
+``` python
+from datetime import datetime
+import json
+
+# importamos definiciones de datos que nos interesen
+from edata.definitions import PricingRules
+# importamos el ayudante
+from edata.helpers import EdataHelper
+# importamos el procesador de utilidades
+from edata.processors import utils
+
+# Preparar reglas de tarificación (si se quiere)
+PRICING_RULES_PVPC = PricingRules(
+    p1_kw_year_eur=30.67266,
+    p2_kw_year_eur=1.4243591,
+    meter_month_eur=0.81,
+    market_kw_year_eur=3.113,
+    electricity_tax=1.0511300560,
+    iva_tax=1.05,
+    # podemos rellenar los siguientes campos si quisiéramos precio fijo (y no pvpc)
+    p1_kwh_eur=None,
+    p2_kwh_eur=None,
+    p3_kwh_eur=None,
+)
+
+# Instanciar el helper
+# 'authorized_nif' permite indicar el NIF de la persona que nos autoriza a consultar su CUPS.
+# 'data' permite "cargar" al helper datos anteriores (resultado edata.data de una ejecución anterior), para evitar volver a consultar los mismos.
+edata = EdataHelper(
+            "datadis_user",
+            "datadis_password",
+            "cups",
+            datadis_authorized_nif=None,
+            pricing_rules=PRICING_RULES_PVPC, # si se le pasa None, no aplica tarificación
+            data=None, # aquí podríamos cargar datos anteriores
+        )
+
+# Solicitar actualización de todo el histórico (se almacena en edata.data)
+edata.update(date_from=datetime(1970, 1, 1), date_to=datetime.today())
+
+# volcamos todo lo obtenido a un fichero
+with open("backup.json", "w") as file:
+    json.dump(utils.serialize_dict(edata.data), file) # se puede utilizar deserialize_dict para la posterior lectura del backup
+
+# Imprimir atributos
+print(edata.attributes)
+```
```

### Comparing `e-data-1.1.2/README.md` & `e-data-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/e_data.egg-info/PKG-INFO` & `e-data-1.1.3/e_data.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,128 +1,128 @@
 Metadata-Version: 2.1
 Name: e-data
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python library for managing spanish energy data from various web providers
 Home-page: https://github.com/uvejota/python-edata
 Author: VMG
 Author-email: vmayorg@outlook.es
 License: GPLv3
-Description: 
-        [![Downloads](https://pepy.tech/badge/e-data)](https://pepy.tech/project/e-data)
-        [![Downloads](https://pepy.tech/badge/e-data/month)](https://pepy.tech/project/e-data)
-        [![Downloads](https://pepy.tech/badge/e-data/week)](https://pepy.tech/project/e-data)
-        
-        # python-edata
-        
-        Este paquete proporciona herramientas para la descarga de tus datos de consumo eléctrico (desde Datadis.es) y su posterior procesado. La motivación principal es que conocer el consumo puede ayudarnos a reducirlo, e incluso a elegir una tarifa que mejor se adapte a nuestras necesidades. A día de hoy sus capacidades de facturación (€) son limitadas, soporta PVPC (según disponibilidad de datos de REData) y tarificación fija por tramos. Es el corazón de la integración [homeassistant-edata](https://github.com/uvejota/homeassistant-edata).
-        
-        _**Esta herramienta no mantiene ningún tipo de vinculación con los proveedores de datos anteriormente mencionados, simplemente consulta la información disponible y facilita su posterior análisis.**_
-        
-        ## Instalación
-        
-        Puedes instalar la última versión estable mediante:
-        
-        ``` bash
-        pip install e-data
-        ```
-        
-        Si quieres probar la versión `dev` o contribuir a su desarrollo, clona este repositorio e instala manualmente las dependencias:
-        
-        ``` bash
-        pip install -r requirements.txt
-        ```
-        
-        ## Estructura
-        
-        El paquete consta de tres módulos diferenciados:
-        
-        * **Conectores** (módulo `connectors`), para definir los métodos de consulta a los diferentes proveedores: Datadis y REData.
-        * **Procesadores** (módulo `processors`), para procesar datos de consumo, maxímetro, o coste (tarificación). Ahora mismo consta de tres procesadores: `billing`, `consumption` y `maximeter`, además de algunas utilidades ubicadas en `utils`. Los procesadores deben heredar de la clase Processor definida en `base.py`
-        * **Ayudantes** (módulo `helpers`), para ayudar en el uso y gestión de los anteriores, presentando de momento un único ayudante llamado `EdataHelper` que te permite recopilar `X` días de datos (por defecto 365) y automáticamente procesarlos. Los datos son almacenados en la variable `data`, mientras que los atributos autocalculados son almacenados en la variable `attributes`. Por lo general, primero utilizan los conectores y luego procesan los datos, gestionando varias tareas de recuperación (principalmente para Datadis).
-        
-        Estos módulos corresponden a la siguiente estructura del paquete:
-        
-        ```
-        edata/
-            · __init__.py
-            · connectors/
-                · __init__.py
-                · datadis.py
-                · redata.py
-            · processors/
-                · __init__.py
-                · base.py
-                · billing.py
-                · consumption.py
-                · maximeter.py
-                · utils.py
-            · helpers.py
-        ```
-        
-        ## Ejemplo de uso
-        
-        Partimos de que tenemos credenciales en Datadis.es. Algunas aclaraciones:
-        * No es necesario solicitar API pública en el registro (se utilizará la API privada habilitada por defecto)
-        * El username suele ser el NIF del titular
-        * Copie el CUPS de la web de Datadis, algunas comercializadoras adhieren caracteres adicionales en el CUPS mostrado en su factura.
-        * La herramienta acepta el uso de NIF autorizado para consultar el suministro de otro titular.
-        
-        ``` python
-        from datetime import datetime
-        import json
-        
-        # importamos definiciones de datos que nos interesen
-        from edata.definitions import PricingRules
-        # importamos el ayudante
-        from edata.helpers import EdataHelper
-        # importamos el procesador de utilidades
-        from edata.processors import utils
-        
-        # Preparar reglas de tarificación (si se quiere)
-        PRICING_RULES_PVPC = PricingRules(
-            p1_kw_year_eur=30.67266,
-            p2_kw_year_eur=1.4243591,
-            meter_month_eur=0.81,
-            market_kw_year_eur=3.113,
-            electricity_tax=1.0511300560,
-            iva_tax=1.05,
-            # podemos rellenar los siguientes campos si quisiéramos precio fijo (y no pvpc)
-            p1_kwh_eur=None,
-            p2_kwh_eur=None,
-            p3_kwh_eur=None,
-        )
-        
-        # Instanciar el helper
-        # 'authorized_nif' permite indicar el NIF de la persona que nos autoriza a consultar su CUPS.
-        # 'data' permite "cargar" al helper datos anteriores (resultado edata.data de una ejecución anterior), para evitar volver a consultar los mismos.
-        edata = EdataHelper(
-                    "datadis_user",
-                    "datadis_password",
-                    "cups",
-                    datadis_authorized_nif=None,
-                    pricing_rules=PRICING_RULES_PVPC, # si se le pasa None, no aplica tarificación
-                    data=None, # aquí podríamos cargar datos anteriores
-                )
-        
-        # Solicitar actualización de todo el histórico (se almacena en edata.data)
-        edata.update(date_from=datetime(1970, 1, 1), date_to=datetime.today())
-        
-        # volcamos todo lo obtenido a un fichero
-        with open("backup.json", "w") as file:
-            json.dump(utils.serialize_dict(edata.data), file) # se puede utilizar deserialize_dict para la posterior lectura del backup
-        
-        # Imprimir atributos
-        print(edata.attributes)
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+[![Downloads](https://pepy.tech/badge/e-data)](https://pepy.tech/project/e-data)
+[![Downloads](https://pepy.tech/badge/e-data/month)](https://pepy.tech/project/e-data)
+[![Downloads](https://pepy.tech/badge/e-data/week)](https://pepy.tech/project/e-data)
+
+# python-edata
+
+Este paquete proporciona herramientas para la descarga de tus datos de consumo eléctrico (desde Datadis.es) y su posterior procesado. La motivación principal es que conocer el consumo puede ayudarnos a reducirlo, e incluso a elegir una tarifa que mejor se adapte a nuestras necesidades. A día de hoy sus capacidades de facturación (€) son limitadas, soporta PVPC (según disponibilidad de datos de REData) y tarificación fija por tramos. Es el corazón de la integración [homeassistant-edata](https://github.com/uvejota/homeassistant-edata).
+
+_**Esta herramienta no mantiene ningún tipo de vinculación con los proveedores de datos anteriormente mencionados, simplemente consulta la información disponible y facilita su posterior análisis.**_
+
+## Instalación
+
+Puedes instalar la última versión estable mediante:
+
+``` bash
+pip install e-data
+```
+
+Si quieres probar la versión `dev` o contribuir a su desarrollo, clona este repositorio e instala manualmente las dependencias:
+
+``` bash
+pip install -r requirements.txt
+```
+
+## Estructura
+
+El paquete consta de tres módulos diferenciados:
+
+* **Conectores** (módulo `connectors`), para definir los métodos de consulta a los diferentes proveedores: Datadis y REData.
+* **Procesadores** (módulo `processors`), para procesar datos de consumo, maxímetro, o coste (tarificación). Ahora mismo consta de tres procesadores: `billing`, `consumption` y `maximeter`, además de algunas utilidades ubicadas en `utils`. Los procesadores deben heredar de la clase Processor definida en `base.py`
+* **Ayudantes** (módulo `helpers`), para ayudar en el uso y gestión de los anteriores, presentando de momento un único ayudante llamado `EdataHelper` que te permite recopilar `X` días de datos (por defecto 365) y automáticamente procesarlos. Los datos son almacenados en la variable `data`, mientras que los atributos autocalculados son almacenados en la variable `attributes`. Por lo general, primero utilizan los conectores y luego procesan los datos, gestionando varias tareas de recuperación (principalmente para Datadis).
+
+Estos módulos corresponden a la siguiente estructura del paquete:
+
+```
+edata/
+    · __init__.py
+    · connectors/
+        · __init__.py
+        · datadis.py
+        · redata.py
+    · processors/
+        · __init__.py
+        · base.py
+        · billing.py
+        · consumption.py
+        · maximeter.py
+        · utils.py
+    · helpers.py
+```
+
+## Ejemplo de uso
+
+Partimos de que tenemos credenciales en Datadis.es. Algunas aclaraciones:
+* No es necesario solicitar API pública en el registro (se utilizará la API privada habilitada por defecto)
+* El username suele ser el NIF del titular
+* Copie el CUPS de la web de Datadis, algunas comercializadoras adhieren caracteres adicionales en el CUPS mostrado en su factura.
+* La herramienta acepta el uso de NIF autorizado para consultar el suministro de otro titular.
+
+``` python
+from datetime import datetime
+import json
+
+# importamos definiciones de datos que nos interesen
+from edata.definitions import PricingRules
+# importamos el ayudante
+from edata.helpers import EdataHelper
+# importamos el procesador de utilidades
+from edata.processors import utils
+
+# Preparar reglas de tarificación (si se quiere)
+PRICING_RULES_PVPC = PricingRules(
+    p1_kw_year_eur=30.67266,
+    p2_kw_year_eur=1.4243591,
+    meter_month_eur=0.81,
+    market_kw_year_eur=3.113,
+    electricity_tax=1.0511300560,
+    iva_tax=1.05,
+    # podemos rellenar los siguientes campos si quisiéramos precio fijo (y no pvpc)
+    p1_kwh_eur=None,
+    p2_kwh_eur=None,
+    p3_kwh_eur=None,
+)
+
+# Instanciar el helper
+# 'authorized_nif' permite indicar el NIF de la persona que nos autoriza a consultar su CUPS.
+# 'data' permite "cargar" al helper datos anteriores (resultado edata.data de una ejecución anterior), para evitar volver a consultar los mismos.
+edata = EdataHelper(
+            "datadis_user",
+            "datadis_password",
+            "cups",
+            datadis_authorized_nif=None,
+            pricing_rules=PRICING_RULES_PVPC, # si se le pasa None, no aplica tarificación
+            data=None, # aquí podríamos cargar datos anteriores
+        )
+
+# Solicitar actualización de todo el histórico (se almacena en edata.data)
+edata.update(date_from=datetime(1970, 1, 1), date_to=datetime.today())
+
+# volcamos todo lo obtenido a un fichero
+with open("backup.json", "w") as file:
+    json.dump(utils.serialize_dict(edata.data), file) # se puede utilizar deserialize_dict para la posterior lectura del backup
+
+# Imprimir atributos
+print(edata.attributes)
+```
```

### Comparing `e-data-1.1.2/edata/connectors/datadis.py` & `e-data-1.1.3/edata/connectors/datadis.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/edata/connectors/redata.py` & `e-data-1.1.3/edata/connectors/redata.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/edata/definitions.py` & `e-data-1.1.3/edata/definitions.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/edata/helpers.py` & `e-data-1.1.3/edata/helpers.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/edata/processors/base.py` & `e-data-1.1.3/edata/processors/base.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/edata/processors/billing.py` & `e-data-1.1.3/edata/processors/billing.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/edata/processors/consumption.py` & `e-data-1.1.3/edata/processors/consumption.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/edata/processors/maximeter.py` & `e-data-1.1.3/edata/processors/maximeter.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/edata/processors/utils.py` & `e-data-1.1.3/edata/processors/utils.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.2/setup.py` & `e-data-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 DESCRIPTION = (
     "Python library for managing spanish energy data from various web providers"
 )
 URL = "https://github.com/uvejota/python-edata"
 EMAIL = "vmayorg@outlook.es"
 AUTHOR = "VMG"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "dateparser>=1.1.2",
     "freezegun>=1.2.1",
     "holidays>=0.14.2",
-    "pandas<2.0.0",
+    "pandas==1.5.3",
+    "numpy==1.24.3",
     "pytest>=7.1.2",
     "python_dateutil>=2.8.2",
     "requests>=2.28.1",
 ]
 
 # What packages are optional?
 EXTRAS = {
```

