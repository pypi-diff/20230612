# Comparing `tmp/nexus_integra_api-1.0.1.tar.gz` & `tmp/nexus_integra_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus_integra_api-1.0.1.tar", max compression
+gzip compressed data, was "nexus_integra_api-1.0.2.tar", max compression
```

## Comparing `nexus_integra_api-1.0.1.tar` & `nexus_integra_api-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1089 2022-03-10 14:16:20.825000 nexus_integra_api-1.0.1/LICENSE.MD
--rw-r--r--   0        0        0        0 2022-09-19 08:17:11.475000 nexus_integra_api-1.0.1/nexus_api/__init__.py
--rw-r--r--   0        0        0    38210 2023-03-08 10:36:43.048000 nexus_integra_api-1.0.1/nexus_api/APINexus.py
--rw-r--r--   0        0        0     7953 2023-02-15 09:48:02.317000 nexus_integra_api-1.0.1/nexus_api/email_alerts.py
--rw-r--r--   0        0        0      943 2023-02-15 10:44:48.744000 nexus_integra_api-1.0.1/nexus_api/exceptions.py
--rw-r--r--   0        0        0      935 2022-09-19 08:17:11.457000 nexus_integra_api-1.0.1/nexus_api/NexusRequest.py
--rw-r--r--   0        0        0      370 2022-09-19 08:17:11.471000 nexus_integra_api-1.0.1/nexus_api/NexusValue.py
--rw-r--r--   0        0        0      594 2023-03-08 10:45:36.238000 nexus_integra_api-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    13745 2023-02-15 11:15:59.140000 nexus_integra_api-1.0.1/README.md
--rw-r--r--   0        0        0    14481 1970-01-01 00:00:00.000000 nexus_integra_api-1.0.1/setup.py
--rw-r--r--   0        0        0    14011 1970-01-01 00:00:00.000000 nexus_integra_api-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-14 02:02:18.000000 nexus_integra_api-1.0.2/LICENSE.MD
+-rw-r--r--   0        0        0        0 2023-04-14 02:02:18.000000 nexus_integra_api-1.0.2/nexus_api/__init__.py
+-rw-r--r--   0        0        0    38248 2023-06-12 07:52:04.251210 nexus_integra_api-1.0.2/nexus_api/APINexus.py
+-rw-r--r--   0        0        0     7953 2023-04-14 02:02:18.000000 nexus_integra_api-1.0.2/nexus_api/email_alerts.py
+-rw-r--r--   0        0        0      943 2023-04-14 02:02:18.000000 nexus_integra_api-1.0.2/nexus_api/exceptions.py
+-rw-r--r--   0        0        0      935 2023-04-14 02:02:18.000000 nexus_integra_api-1.0.2/nexus_api/NexusRequest.py
+-rw-r--r--   0        0        0      370 2023-04-14 02:02:18.000000 nexus_integra_api-1.0.2/nexus_api/NexusValue.py
+-rw-r--r--   0        0        0      594 2023-06-12 08:11:00.738374 nexus_integra_api-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13745 2023-04-14 02:02:18.000000 nexus_integra_api-1.0.2/README.md
+-rw-r--r--   0        0        0    14011 1970-01-01 00:00:00.000000 nexus_integra_api-1.0.2/PKG-INFO
```

### Comparing `nexus_integra_api-1.0.1/LICENSE.MD` & `nexus_integra_api-1.0.2/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `nexus_integra_api-1.0.1/nexus_api/APINexus.py` & `nexus_integra_api-1.0.2/nexus_api/APINexus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 APINexus
 Class definition
 """
+from __future__ import annotations
+
 import datetime
 import json
 
 import pandas
 import pandas as pd
 import requests
 import urllib3
```

### Comparing `nexus_integra_api-1.0.1/nexus_api/email_alerts.py` & `nexus_integra_api-1.0.2/nexus_api/email_alerts.py`

 * *Files identical despite different names*

### Comparing `nexus_integra_api-1.0.1/nexus_api/exceptions.py` & `nexus_integra_api-1.0.2/nexus_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `nexus_integra_api-1.0.1/nexus_api/NexusRequest.py` & `nexus_integra_api-1.0.2/nexus_api/NexusRequest.py`

 * *Files identical despite different names*

### Comparing `nexus_integra_api-1.0.1/pyproject.toml` & `nexus_integra_api-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "nexus_integra_api"
 packages = [
     {include = 'nexus_api'}
 ]
-version = "1.0.1"
+version = "1.0.2"
 authors = ["Nexus Integra"]
 description =" Nexus API connection methods and utilities"
 readme = "README.md"
 homepage = "https://nexusintegra.io"
 repository = 'https://github.com/NexusIntegra/NexusAPI'
 
 [tool.poetry.dependencies]
```

### Comparing `nexus_integra_api-1.0.1/README.md` & `nexus_integra_api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nexus_integra_api-1.0.1/setup.py` & `nexus_integra_api-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,424 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nexus-integra-api
+Version: 1.0.2
+Summary:  Nexus API connection methods and utilities
+Home-page: https://nexusintegra.io
+Author: Nexus Integra
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Repository, https://github.com/NexusIntegra/NexusAPI
+Description-Content-Type: text/markdown
 
-packages = \
-['nexus_api']
+# nexus_integra_api
+Este repositorio tiene como propósito reunir en una única libería todas las funciones necesarias para trabajar con la API de Nexus en Python.
+En lugar de importar los archivos a la carpeta del proyecto cada vez que se usan puede instalarse la librería en la PATH de Python 
 
-package_data = \
-{'': ['*']}
+## Table of Contents
 
-install_requires = \
-['pandas', 'requests>=2.28.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nexus-integra-api',
-    'version': '1.0.1',
-    'description': ' Nexus API connection methods and utilities',
-    'long_description': '# nexus_integra_api\nEste repositorio tiene como propósito reunir en una única libería todas las funciones necesarias para trabajar con la API de Nexus en Python.\nEn lugar de importar los archivos a la carpeta del proyecto cada vez que se usan puede instalarse la librería en la PATH de Python \n\n## Table of Contents\n\n* [Instalación](#instalacion)\n* [Uso](#uso)\n* [Ejemplos](#ejemplos)\n  * [Lectura de datos](#lectura)\n  * [Subida de datos](#subida)\n  * [Alarmas](#alarmas)\n  * [Email Alerts](#email)\n* [Contribuir](#contribuir)\n* [Change Log](#changelog)\n* [Contacto](#contacto)\n\n## Instalación <a class="anchor" id="instalacion"></a>\n\nUsa el package manager pip para instalar la librería. Puede instalarse de forma local o desde el repositorio de PyPi\n\n```\npip install nexus_integra_api\n```\n\n## Uso <a class="anchor" id="uso"></a>\nPara importar todo el contenido de la librería, una vez instalada hay que realizar el siguiente import:\n\n    import nexus_api\nSi únicamente se desea la clase en la que residen las funciones que trabajan con la API:\n\n    from nexus_api import APINexus\nLo que otorga acceso a la clase APINexus en la que residen todas las funciones necesarias.\n\n## Ejemplo de uso <a class="anchor" id="ejemplos"></a>\n\nEn primer lugar se especifican los parámetros de conexión y se crea el objeto Nexus, además de los imports necesarios\n```\nfrom nexus_api import APINexus\nimport pandas as pd\nimport datetime\n\nAPI_Host = \'nexus-cdi-demo.globalomnium.com\'  \nAPI_Port = 56000 \nNexusToken = \'xxxxxxxxxxxxxxxxx\' \nversion = \'v1\'\nlogger = [objeto logger - puede ser None]\nNX = APINexus.APINexus(API_Host, API_Port, NexusToken, version, logger)\n```\n\n### Lectura de datos <a class="anchor" id="lectura"></a>\n\n### filter_installation\n\n\nla funcion recibe como parametros la fecha ini, fecha fin, un df con los uid y\nlos nombres de las variables de la instalación y el filtro de texto aplicar (pueden ser varios)\n\nArgs:\n\n- Datefrom (datetime)\n- Dateto (datetime)\n- columnas (dataframe): df con los metadatos de los tags de Nexus \n- uids: (optional) (list): lista de los uids de las variables deseadas. No puede usarse con filter_txt\n- filter_txt (optional: list or str): lista de nombres de las variables deseadas. Si se deja en blanco o no se encuentran variables se devuelve toda la instalación. No puede usarse con uids\n- resolucion (int): de 0 a 10 [ RES_30_SEC, RES_1_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH, RES_1_YEAR, RES_5_MIN, RES_200_MIL, RES_500_MIL, RES_1_SEC ]\n- fuente (int): [0 -->RAW, 1 -->STATS_PER_HOUR, 2 -->STATS_PER_DAY, 3 -->STATS_PER_MONTH, 4 -->TRANSIENT]\n\nReturns:\n- filtered_hist (dataframe). Dataframe con los campos [index, timeStamp, name, value, uid]\n\nEjemplo:\n\n```\n# Lectura de loe metadatos de todos los tags contenidos en la API (necesario)\ndatos = self.NX.callGetTags()\ncolumnas = json_normalize(datos)\n\n# Profundidad del análisis en fechas desde hoy\ndelta_days = 3\ndate_to = datetime.datetime.now()\ndate_from = date_to - datetime.timedelta(days=delta_days)\n\nfiltered_hist = NX.filter_installation(date_from, date_to, columnas, resolucion=4)\n```\nSi quisiéramos filtrar las variables por texto o uids:\n```\n# Por uids:\nuids = [\'abc1\', \'abc2\', ...]\nfiltered_hist = NX.filter_installation(date_from, date_to, columnas, uids=uids, resolucion=4)\n# Por texto:\nfiltros = [\'var1\', \'var2\', ...]\nfiltered_hist = NX.filter_installation(date_from, date_to, columnas, filter_txt=filtros, resolucion=4)\n```\n\n### filter_tagview\n\nLa funcion recibe como parametros la fecha ini, fecha fin, un df con los uid y\nlos nombres de las variables de la instalación y el filtro de texto aplicar (pueden ser varios)\n\nArgs:\n- Datefrom (datetime)\n- Dateto (datetime)\n- columnas (dataframe)\n- filter_txt (optional: list or str)\n- resolucion (int): de 0 a 10 [ RES_30_SEC, RES_1_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH, RES_1_YEAR, RES_5_MIN, RES_200_MIL, RES_500_MIL, RES_1_SEC ]\n- fuente (int): [0 -->RAW, 1 -->STATS_PER_HOUR, 2 -->STATS_PER_DAY, 3 -->STATS_PER_MONTH, 4 -->TRANSIENT]\n\nReturns:\n- filtered_hist (dataframe). Dataframe con los campos [index, timeStamp, name, value, uid]\n\nExactamente igual que la anterior pero aplicable a vistas de variables (recomendado)\n\nPrimero hay que especificar el uid de la vista de variables deseada. Puede obtenerse desde Nexus o obtenerse a través de métodos de la API\n```\n# Leer vistas de variables asociadas al token  \ntagviews = NX.callGetDocuments()  \ntagviews = json_normalize(tagviews)  \n# Busqueda del uid de la vista\nuid_tagview = tagviews.uid[0]\n```\nSe especifica la ventana temporal deseada:\n```\n# Profundidad del análisis en fechas desde hoy  \ndelta_days = xxx  \ndate_format = \'%m/%d/%Y %H:%M:%S %Z\'  \ndate_to = datetime.datetime.now()  \ndate_from = date_to - datetime.timedelta(days=delta_days)\n```\nHay que especificar las variables deseadas de la vista de variables elegida. Con este código se obtienen todos los uids de las variables de la vista.\n```\n# Variables en la vista de variables  \nvbles = NX.callGetTagViews(uid_tagview)  \ndf = pd.DataFrame(vbles)  \ncolumnas = df[\'columns\']  \ncolumnas = json_normalize(columnas)  \n```\nFinalmente se obtiene el histórico llamando a la función:\n```\nfiltered_hist = NX.filter_tagview(date_from, date_to, columnas, uid_tagview)\n```\nTambién puede filtrarse por texto o uid dentro de la vista\n```\n# Por uids:\nuids = [\'abc1\', \'abc2\', ...]\nfiltered_hist = NX.filter_tagview(date_from, date_to, columnas, uid_vista, uids=uids, resolucion=4)\n# Por texto:\nfiltros = [\'var1\', \'var2\', ...]\nfiltered_hist = NX.filter_tagview(date_from, date_to, columnas, uid_vista, filter_txt=filtros, resolucion=4)\n```\n\n\n### Subida de datos <a class="anchor" id="subida"></a>\n\nLos datos que se suban a través de la API se encontrarán en la instalación habilitada para el token.\n\nEn primer lugar hay que asegurarse de crear las variables necesarias. Este paso puede omitirse si ya han sido creadas:\n\n### callPostTagInsert\nConsulta de tags con permisos de escritura. Si la variable no existe se crea\n\nArgs:\n- variable_name(str): nombre de la variable a consultar o crear\n\n### callPostValueHist\n\nFunción de escritura de variables en histórico.\n\nArgs:\n- df_value_timestamp: dataframe con las variables y sus valores y timestamp\n\nEjemplo:\n\nUna vez creadas las variables, pueden insertarse datos tanto en histórico como en tiempo real.\n**Importante**: para subir los datos se requiere un dataframe con la siguiente estructura:\n\n| timeStamp      \t| name      \t| value          \t|\n|----------------\t|-----------\t|----------------\t|\n| epoch time (s) \t| variable1 \t| valor numérico \t|\n| epoch time (s) \t| variable2 \t| valor numérico \t|\n\n```\ntest_df = pd.DataFrame({\'timeStamp\': [time.time()], \'name\': [\'api_test\'], \'value\': [1]})\nNX.callPostValueHist(test_df)\n```\n\nEl método acepta datetime64[ns] pero se recomienda pasar primero a epoch time. Para pasar de fecha en datetime a epoch se puede usar:\n```\ndf[\'timeStamp\'] = df[\'timeStamp\'].apply(lambda x: x.timestamp())\n```\n\n### callPostValueRTmult\nEscritura de variable en tiempo real.\n\nArgs:\n- df_variable_name_value: dataframe con las variables y valores a escribir\n\nEjemplo:\n```\ntest_df = pd.DataFrame({\'timeStamp\': [time.time()], \'name\': [\'api_test\'], \'value\': [1]})\nNX.callPostValueRTmult(test_df)\n```\nRealmente la columna timeStamp no es necesaria en este caso, pero se recomienda mantener la estructura común al resto de métodos\n\n### callPostValue_operate(self, variable_uid, variable_value)\nEscritura de variable sobre PLC\n\nArgs:\n- variable_uid: nombre de la variable a escribir en el PLC\n- variable_value: valor de la variable a escribir\n\n### Uso de alarmas <a class="anchor" id="alarmas"></a>\nDesde la versión **0.4** del encapsulado pueden modificarse alarmas en la API. Para ello se debe obtener el uid de la alarma a modificar y luego llamar a la función:\n#### Obtener uids de alarmas del token\n```\nalarmas = NX.callGetAlarms()\n```\n\n#### Obtener información de alarma por uid\n```\nalarma = NX.callGetAlarmByuid(uid)\n```\n\n#### Obtener uids de alarmas por nombres. Puede usarse una lista de nombres o un string con un nombre\n```\nuids_alarmas = NX.get_alarms_uids_by_names([names])\n```\n#### Obtener uids de alarmas por grupos de alarmas. Puede usarse una lista de grupos o un string con un grupo\n```\nuids_grupo = NX.get_alarms_uids_by_groups([groups])\n```\n\n#### Cambiar el estado de la alarma. Debe especificarse el uid de la alarma y el estado a cambiar (\'ARE\' o \'EXR\')\n```\nNX.callPostAckAlarm(uid, estado)\n```\n\n#### Cambiar el mensaje de estado de la alarma\n```\nNX.callPostAlarmEvent(uid, msg)\n```\n\n### Email Alerts <a class="anchor" id="email"></a>\nDesde la versión **0.5** se añade soporte para generar alarmas de correo eléctronico.\n\nPara usar la función debe crearse un objeto de tipo EmailAlerts. Deben proporcionarse los parámetros de conexión.\n```\nclass EmailAlerts:\n    """\n    Email management\n    Attributes:\n        attachments: list of files to add to message. See add_attachment for individual files\n        environment: name of the environment (used to identify application)\n        message: email\'s body\n        subject: email\'s subject\n        smtp_address: configuration parameter\n        email_password: password\n        email_port: port of server\n        email_sender: snder address\n        email_receiver: receiver address\n        cooldown (optional): time in hours to wait between two emails\n    """\n```\nSe recomienda usar variables de entorno para proteger las credenciales. En caso de no estar definidas se deben especificar (reemplazar las líneas de os.getenv()):\n\n```\nimport os\n\nsmtp_address = \'outlook.office365.com\'\nsmtp_port = 587\n# Tiempo en horas entre envíos sucesivos\ncooldown = 1\n\n# datos de la cuenta de envio\nsender_email_address = os.getenv("SENDER_EMAIL_ADDRESS")\nemail_password = os.getenv("EMAIL_PASSWORD")\nreceiver_email_address = os.getenv("RECEIVER_EMAIL_ADDRESS")\n\nemail_alerts = EmailAlerts(smtp_address, smtp_port, sender_email_address, email_password, receiver_email_address, cooldown=cooldown)\n```\n\nUna vez creado el objeto email_alerts puede usarse con libertad, bien con los parámetros predeterminados o moficiando los componentes del mensaje\n\nEl asunto y el cuerpo del mensaje tienen valores predeterminados en función del nombre del archivo, pero environment es una variable requerida con la que identificar el entorno de producción.\n```\nenviroment = \'NEXUS_PROD\'\nsubject = \'ALARMA\'\nbody = \'Alarma de \' + environment\n\nemail_alerts.set_email_alert_info(subject, body, environment)\n```\n\n\nSe puede usar la alerta de correo en cualquier función, sea de la API o no. Si la ejecución falla, \nse captura la excepción y se envía un correo con el error (mensaje predeterminado).\n\nSi se quiere incorporar a un script entero, debe usarse la función main()\n\n```\n# Uso del decorador para generar el correo\n\n@email_alerts.email_alert_decorator\ndef main():\n    # Aquí va todo el código del programa...\n    raise Exception(\'Error en la función\')\n    \nif __name__ == \'__main__\':\n    main() # Si aparece un error, se envía un correo con el error\n```\n\n## Contribuir <a class="anchor" id="contribuir"></a>\n\nCualquier función o sugerencia añadida es bien recibida.\n\nSugerencias:\n\n- Traducir documentación\n\n## Change log <a class="anchor" id="changelog"></a>\n\n###v0.9.0 - 15/02/2023\n**Added**\n- Operate method to write directly into PLC variables\n- NexusAPI custom exception\n- logging options\n\n###v0.8.0 - 04/11/2022\n**Added**\n- Support for cooldown options in email_alerts: pass time in hours as cooldown parameter in EmailAlerts\nclass to avoid sending more than 1 email in a given time\n\n###v0.7.0 - 20/09/2022\n**Important**\nThis update changes data structure of filter_tagview and filter_installation response. Please check your code before updating\n\n\n**Added**\n  - filter_tagview and filter_installation search by uid support\n  - filter_tagview and filter_installation match structure (index, uid, name, value, timeStamp (datetime))\n\n**Fix**\n  - Now filter_installation and filter_tagview will raise an error if API response is not valid\n\n**Updated**\n  - Better docs\n\n###v0.6.2 - 09/09/2022\n**Updated**\n- Better docs\n\n**Fix**\n- Now filter_installation/tagview raises an exception if dataframe structure is not correct\n\n###v0.6.0 - 10/05/2022\n**Added**\n- Email attachments\n\n###v0.5.0 - 12/04/2022\n\n**Added**\n\n - Email alerts functions\n\n**Changed**\n\n - Documentation\n\n###v0.4.0 - 30/03/2022\n\n**Added**\n  \n- API V2 alarm functions\n  * callPostAckAlarm(uid, status)\n  * callPostAlarmEvent(uid, msg)\n  * callGetAlarms()\n  * callGetAlarmByuid(uid)\n  * get_alarms_uids_by_names([names])\n  * get_alarms_uids_by_groups([groups])\n- Unit tests\n- .env file in order protect credentials\n- Bypassed 50k row limit in POST methods\n- Added support to datetime objects in callPostValueHist\n  \n**Modified**\n  \n- Unified callPostValueHist and callPostValueHistmult (deprecated)\n  \n###v0.3.2 - 11/03/2022\n**Added**\n- Add filter_installation and filter_tagview as replacement for GetFiltered\n- Add README.md\n\n## Contacto <a class="anchor" id="chapter6"></a>\n[**Pau Juan**](mailto:pau.juan@nexusintegra.io)\n*Operaciones*\n\n\n[**Laura Moreno**](mailto:laura.moreno@nexusintegra.io)\n*Operaciones*\n\n\n[**Ricardo Gómez**](mailto:ricardo.gomez.aldaravi@nexusintegra.io)\n*Operaciones*\n\n[Nexus Integra](https://nexusintegra.io/)\n',
-    'author': 'Nexus Integra',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://nexusintegra.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+* [Instalación](#instalacion)
+* [Uso](#uso)
+* [Ejemplos](#ejemplos)
+  * [Lectura de datos](#lectura)
+  * [Subida de datos](#subida)
+  * [Alarmas](#alarmas)
+  * [Email Alerts](#email)
+* [Contribuir](#contribuir)
+* [Change Log](#changelog)
+* [Contacto](#contacto)
 
+## Instalación <a class="anchor" id="instalacion"></a>
+
+Usa el package manager pip para instalar la librería. Puede instalarse de forma local o desde el repositorio de PyPi
+
+```
+pip install nexus_integra_api
+```
+
+## Uso <a class="anchor" id="uso"></a>
+Para importar todo el contenido de la librería, una vez instalada hay que realizar el siguiente import:
+
+    import nexus_api
+Si únicamente se desea la clase en la que residen las funciones que trabajan con la API:
+
+    from nexus_api import APINexus
+Lo que otorga acceso a la clase APINexus en la que residen todas las funciones necesarias.
+
+## Ejemplo de uso <a class="anchor" id="ejemplos"></a>
+
+En primer lugar se especifican los parámetros de conexión y se crea el objeto Nexus, además de los imports necesarios
+```
+from nexus_api import APINexus
+import pandas as pd
+import datetime
+
+API_Host = 'nexus-cdi-demo.globalomnium.com'  
+API_Port = 56000 
+NexusToken = 'xxxxxxxxxxxxxxxxx' 
+version = 'v1'
+logger = [objeto logger - puede ser None]
+NX = APINexus.APINexus(API_Host, API_Port, NexusToken, version, logger)
+```
+
+### Lectura de datos <a class="anchor" id="lectura"></a>
+
+### filter_installation
+
+
+la funcion recibe como parametros la fecha ini, fecha fin, un df con los uid y
+los nombres de las variables de la instalación y el filtro de texto aplicar (pueden ser varios)
+
+Args:
+
+- Datefrom (datetime)
+- Dateto (datetime)
+- columnas (dataframe): df con los metadatos de los tags de Nexus 
+- uids: (optional) (list): lista de los uids de las variables deseadas. No puede usarse con filter_txt
+- filter_txt (optional: list or str): lista de nombres de las variables deseadas. Si se deja en blanco o no se encuentran variables se devuelve toda la instalación. No puede usarse con uids
+- resolucion (int): de 0 a 10 [ RES_30_SEC, RES_1_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH, RES_1_YEAR, RES_5_MIN, RES_200_MIL, RES_500_MIL, RES_1_SEC ]
+- fuente (int): [0 -->RAW, 1 -->STATS_PER_HOUR, 2 -->STATS_PER_DAY, 3 -->STATS_PER_MONTH, 4 -->TRANSIENT]
+
+Returns:
+- filtered_hist (dataframe). Dataframe con los campos [index, timeStamp, name, value, uid]
+
+Ejemplo:
+
+```
+# Lectura de loe metadatos de todos los tags contenidos en la API (necesario)
+datos = self.NX.callGetTags()
+columnas = json_normalize(datos)
+
+# Profundidad del análisis en fechas desde hoy
+delta_days = 3
+date_to = datetime.datetime.now()
+date_from = date_to - datetime.timedelta(days=delta_days)
+
+filtered_hist = NX.filter_installation(date_from, date_to, columnas, resolucion=4)
+```
+Si quisiéramos filtrar las variables por texto o uids:
+```
+# Por uids:
+uids = ['abc1', 'abc2', ...]
+filtered_hist = NX.filter_installation(date_from, date_to, columnas, uids=uids, resolucion=4)
+# Por texto:
+filtros = ['var1', 'var2', ...]
+filtered_hist = NX.filter_installation(date_from, date_to, columnas, filter_txt=filtros, resolucion=4)
+```
+
+### filter_tagview
+
+La funcion recibe como parametros la fecha ini, fecha fin, un df con los uid y
+los nombres de las variables de la instalación y el filtro de texto aplicar (pueden ser varios)
+
+Args:
+- Datefrom (datetime)
+- Dateto (datetime)
+- columnas (dataframe)
+- filter_txt (optional: list or str)
+- resolucion (int): de 0 a 10 [ RES_30_SEC, RES_1_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH, RES_1_YEAR, RES_5_MIN, RES_200_MIL, RES_500_MIL, RES_1_SEC ]
+- fuente (int): [0 -->RAW, 1 -->STATS_PER_HOUR, 2 -->STATS_PER_DAY, 3 -->STATS_PER_MONTH, 4 -->TRANSIENT]
+
+Returns:
+- filtered_hist (dataframe). Dataframe con los campos [index, timeStamp, name, value, uid]
+
+Exactamente igual que la anterior pero aplicable a vistas de variables (recomendado)
+
+Primero hay que especificar el uid de la vista de variables deseada. Puede obtenerse desde Nexus o obtenerse a través de métodos de la API
+```
+# Leer vistas de variables asociadas al token  
+tagviews = NX.callGetDocuments()  
+tagviews = json_normalize(tagviews)  
+# Busqueda del uid de la vista
+uid_tagview = tagviews.uid[0]
+```
+Se especifica la ventana temporal deseada:
+```
+# Profundidad del análisis en fechas desde hoy  
+delta_days = xxx  
+date_format = '%m/%d/%Y %H:%M:%S %Z'  
+date_to = datetime.datetime.now()  
+date_from = date_to - datetime.timedelta(days=delta_days)
+```
+Hay que especificar las variables deseadas de la vista de variables elegida. Con este código se obtienen todos los uids de las variables de la vista.
+```
+# Variables en la vista de variables  
+vbles = NX.callGetTagViews(uid_tagview)  
+df = pd.DataFrame(vbles)  
+columnas = df['columns']  
+columnas = json_normalize(columnas)  
+```
+Finalmente se obtiene el histórico llamando a la función:
+```
+filtered_hist = NX.filter_tagview(date_from, date_to, columnas, uid_tagview)
+```
+También puede filtrarse por texto o uid dentro de la vista
+```
+# Por uids:
+uids = ['abc1', 'abc2', ...]
+filtered_hist = NX.filter_tagview(date_from, date_to, columnas, uid_vista, uids=uids, resolucion=4)
+# Por texto:
+filtros = ['var1', 'var2', ...]
+filtered_hist = NX.filter_tagview(date_from, date_to, columnas, uid_vista, filter_txt=filtros, resolucion=4)
+```
+
+
+### Subida de datos <a class="anchor" id="subida"></a>
+
+Los datos que se suban a través de la API se encontrarán en la instalación habilitada para el token.
+
+En primer lugar hay que asegurarse de crear las variables necesarias. Este paso puede omitirse si ya han sido creadas:
+
+### callPostTagInsert
+Consulta de tags con permisos de escritura. Si la variable no existe se crea
+
+Args:
+- variable_name(str): nombre de la variable a consultar o crear
+
+### callPostValueHist
+
+Función de escritura de variables en histórico.
+
+Args:
+- df_value_timestamp: dataframe con las variables y sus valores y timestamp
+
+Ejemplo:
+
+Una vez creadas las variables, pueden insertarse datos tanto en histórico como en tiempo real.
+**Importante**: para subir los datos se requiere un dataframe con la siguiente estructura:
+
+| timeStamp      	| name      	| value          	|
+|----------------	|-----------	|----------------	|
+| epoch time (s) 	| variable1 	| valor numérico 	|
+| epoch time (s) 	| variable2 	| valor numérico 	|
+
+```
+test_df = pd.DataFrame({'timeStamp': [time.time()], 'name': ['api_test'], 'value': [1]})
+NX.callPostValueHist(test_df)
+```
+
+El método acepta datetime64[ns] pero se recomienda pasar primero a epoch time. Para pasar de fecha en datetime a epoch se puede usar:
+```
+df['timeStamp'] = df['timeStamp'].apply(lambda x: x.timestamp())
+```
+
+### callPostValueRTmult
+Escritura de variable en tiempo real.
+
+Args:
+- df_variable_name_value: dataframe con las variables y valores a escribir
+
+Ejemplo:
+```
+test_df = pd.DataFrame({'timeStamp': [time.time()], 'name': ['api_test'], 'value': [1]})
+NX.callPostValueRTmult(test_df)
+```
+Realmente la columna timeStamp no es necesaria en este caso, pero se recomienda mantener la estructura común al resto de métodos
+
+### callPostValue_operate(self, variable_uid, variable_value)
+Escritura de variable sobre PLC
+
+Args:
+- variable_uid: nombre de la variable a escribir en el PLC
+- variable_value: valor de la variable a escribir
+
+### Uso de alarmas <a class="anchor" id="alarmas"></a>
+Desde la versión **0.4** del encapsulado pueden modificarse alarmas en la API. Para ello se debe obtener el uid de la alarma a modificar y luego llamar a la función:
+#### Obtener uids de alarmas del token
+```
+alarmas = NX.callGetAlarms()
+```
+
+#### Obtener información de alarma por uid
+```
+alarma = NX.callGetAlarmByuid(uid)
+```
+
+#### Obtener uids de alarmas por nombres. Puede usarse una lista de nombres o un string con un nombre
+```
+uids_alarmas = NX.get_alarms_uids_by_names([names])
+```
+#### Obtener uids de alarmas por grupos de alarmas. Puede usarse una lista de grupos o un string con un grupo
+```
+uids_grupo = NX.get_alarms_uids_by_groups([groups])
+```
+
+#### Cambiar el estado de la alarma. Debe especificarse el uid de la alarma y el estado a cambiar ('ARE' o 'EXR')
+```
+NX.callPostAckAlarm(uid, estado)
+```
+
+#### Cambiar el mensaje de estado de la alarma
+```
+NX.callPostAlarmEvent(uid, msg)
+```
+
+### Email Alerts <a class="anchor" id="email"></a>
+Desde la versión **0.5** se añade soporte para generar alarmas de correo eléctronico.
+
+Para usar la función debe crearse un objeto de tipo EmailAlerts. Deben proporcionarse los parámetros de conexión.
+```
+class EmailAlerts:
+    """
+    Email management
+    Attributes:
+        attachments: list of files to add to message. See add_attachment for individual files
+        environment: name of the environment (used to identify application)
+        message: email's body
+        subject: email's subject
+        smtp_address: configuration parameter
+        email_password: password
+        email_port: port of server
+        email_sender: snder address
+        email_receiver: receiver address
+        cooldown (optional): time in hours to wait between two emails
+    """
+```
+Se recomienda usar variables de entorno para proteger las credenciales. En caso de no estar definidas se deben especificar (reemplazar las líneas de os.getenv()):
+
+```
+import os
+
+smtp_address = 'outlook.office365.com'
+smtp_port = 587
+# Tiempo en horas entre envíos sucesivos
+cooldown = 1
+
+# datos de la cuenta de envio
+sender_email_address = os.getenv("SENDER_EMAIL_ADDRESS")
+email_password = os.getenv("EMAIL_PASSWORD")
+receiver_email_address = os.getenv("RECEIVER_EMAIL_ADDRESS")
+
+email_alerts = EmailAlerts(smtp_address, smtp_port, sender_email_address, email_password, receiver_email_address, cooldown=cooldown)
+```
+
+Una vez creado el objeto email_alerts puede usarse con libertad, bien con los parámetros predeterminados o moficiando los componentes del mensaje
+
+El asunto y el cuerpo del mensaje tienen valores predeterminados en función del nombre del archivo, pero environment es una variable requerida con la que identificar el entorno de producción.
+```
+enviroment = 'NEXUS_PROD'
+subject = 'ALARMA'
+body = 'Alarma de ' + environment
+
+email_alerts.set_email_alert_info(subject, body, environment)
+```
+
+
+Se puede usar la alerta de correo en cualquier función, sea de la API o no. Si la ejecución falla, 
+se captura la excepción y se envía un correo con el error (mensaje predeterminado).
+
+Si se quiere incorporar a un script entero, debe usarse la función main()
+
+```
+# Uso del decorador para generar el correo
+
+@email_alerts.email_alert_decorator
+def main():
+    # Aquí va todo el código del programa...
+    raise Exception('Error en la función')
+    
+if __name__ == '__main__':
+    main() # Si aparece un error, se envía un correo con el error
+```
+
+## Contribuir <a class="anchor" id="contribuir"></a>
+
+Cualquier función o sugerencia añadida es bien recibida.
+
+Sugerencias:
+
+- Traducir documentación
+
+## Change log <a class="anchor" id="changelog"></a>
+
+###v0.9.0 - 15/02/2023
+**Added**
+- Operate method to write directly into PLC variables
+- NexusAPI custom exception
+- logging options
+
+###v0.8.0 - 04/11/2022
+**Added**
+- Support for cooldown options in email_alerts: pass time in hours as cooldown parameter in EmailAlerts
+class to avoid sending more than 1 email in a given time
+
+###v0.7.0 - 20/09/2022
+**Important**
+This update changes data structure of filter_tagview and filter_installation response. Please check your code before updating
+
+
+**Added**
+  - filter_tagview and filter_installation search by uid support
+  - filter_tagview and filter_installation match structure (index, uid, name, value, timeStamp (datetime))
+
+**Fix**
+  - Now filter_installation and filter_tagview will raise an error if API response is not valid
+
+**Updated**
+  - Better docs
+
+###v0.6.2 - 09/09/2022
+**Updated**
+- Better docs
+
+**Fix**
+- Now filter_installation/tagview raises an exception if dataframe structure is not correct
+
+###v0.6.0 - 10/05/2022
+**Added**
+- Email attachments
+
+###v0.5.0 - 12/04/2022
+
+**Added**
+
+ - Email alerts functions
+
+**Changed**
+
+ - Documentation
+
+###v0.4.0 - 30/03/2022
+
+**Added**
+  
+- API V2 alarm functions
+  * callPostAckAlarm(uid, status)
+  * callPostAlarmEvent(uid, msg)
+  * callGetAlarms()
+  * callGetAlarmByuid(uid)
+  * get_alarms_uids_by_names([names])
+  * get_alarms_uids_by_groups([groups])
+- Unit tests
+- .env file in order protect credentials
+- Bypassed 50k row limit in POST methods
+- Added support to datetime objects in callPostValueHist
+  
+**Modified**
+  
+- Unified callPostValueHist and callPostValueHistmult (deprecated)
+  
+###v0.3.2 - 11/03/2022
+**Added**
+- Add filter_installation and filter_tagview as replacement for GetFiltered
+- Add README.md
+
+## Contacto <a class="anchor" id="chapter6"></a>
+[**Pau Juan**](mailto:pau.juan@nexusintegra.io)
+*Operaciones*
+
+
+[**Laura Moreno**](mailto:laura.moreno@nexusintegra.io)
+*Operaciones*
+
+
+[**Ricardo Gómez**](mailto:ricardo.gomez.aldaravi@nexusintegra.io)
+*Operaciones*
+
+[Nexus Integra](https://nexusintegra.io/)
 
-setup(**setup_kwargs)
```

