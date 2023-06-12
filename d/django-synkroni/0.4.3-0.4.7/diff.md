# Comparing `tmp/django-synkroni-0.4.3.tar.gz` & `tmp/django-synkroni-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-synkroni-0.4.3.tar", last modified: Mon Oct 17 07:40:11 2022, max compression
+gzip compressed data, was "django-synkroni-0.4.7.tar", last modified: Mon Jan  2 09:02:57 2023, max compression
```

## Comparing `django-synkroni-0.4.3.tar` & `django-synkroni-0.4.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-10-17 07:40:11.556915 django-synkroni-0.4.3/
--rw-r--r--   0 aha        (501) staff       (20)       75 2021-09-06 06:31:51.000000 django-synkroni-0.4.3/MANIFEST.in
--rw-r--r--   0 aha        (501) staff       (20)      242 2022-10-17 07:40:11.556741 django-synkroni-0.4.3/PKG-INFO
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-10-17 07:40:11.554721 django-synkroni-0.4.3/django_synkroni.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      242 2022-10-17 07:40:11.000000 django-synkroni-0.4.3/django_synkroni.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      592 2022-10-17 07:40:11.000000 django-synkroni-0.4.3/django_synkroni.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2022-10-17 07:40:11.000000 django-synkroni-0.4.3/django_synkroni.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)       47 2022-10-17 07:40:11.000000 django-synkroni-0.4.3/django_synkroni.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     7632 2022-10-17 07:40:11.000000 django-synkroni-0.4.3/django_synkroni.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        1 2021-09-06 06:32:14.000000 django-synkroni-0.4.3/django_synkroni.egg-info/not-zip-safe
--rw-r--r--   0 aha        (501) staff       (20)       27 2022-10-17 07:40:11.000000 django-synkroni-0.4.3/django_synkroni.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        9 2022-10-17 07:40:11.000000 django-synkroni-0.4.3/django_synkroni.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       72 2021-09-06 06:31:51.000000 django-synkroni-0.4.3/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2022-10-17 07:40:11.556959 django-synkroni-0.4.3/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      561 2021-09-06 06:31:51.000000 django-synkroni-0.4.3/setup.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-10-17 07:40:11.556176 django-synkroni-0.4.3/synkroni/
--rw-r--r--   0 aha        (501) staff       (20)      107 2021-04-07 18:03:12.000000 django-synkroni-0.4.3/synkroni/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      683 2021-09-20 10:38:01.000000 django-synkroni-0.4.3/synkroni/json.py
--rw-r--r--   0 aha        (501) staff       (20)      261 2021-09-20 10:38:01.000000 django-synkroni-0.4.3/synkroni/komennot.py
--rw-r--r--   0 aha        (501) staff       (20)      159 2021-04-08 18:06:03.000000 django-synkroni-0.4.3/synkroni/mallit.py
--rw-r--r--   0 aha        (501) staff       (20)       22 2021-04-08 17:56:03.000000 django-synkroni-0.4.3/synkroni/models.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-10-17 07:40:11.553205 django-synkroni-0.4.3/synkroni/static/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-10-17 07:40:11.553246 django-synkroni-0.4.3/synkroni/static/synkroni/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-10-17 07:40:11.556293 django-synkroni-0.4.3/synkroni/static/synkroni/js/
--rw-r--r--   0 aha        (501) staff       (20)     9447 2022-09-27 07:22:03.000000 django-synkroni-0.4.3/synkroni/static/synkroni/js/synkroni.js
--rw-r--r--   0 aha        (501) staff       (20)     2690 2021-10-08 10:27:09.000000 django-synkroni-0.4.3/synkroni/synkroni.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-10-17 07:40:11.553349 django-synkroni-0.4.3/synkroni/templates/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-10-17 07:40:11.556525 django-synkroni-0.4.3/synkroni/templates/synkroni/
--rw-r--r--   0 aha        (501) staff       (20)      859 2022-05-04 12:06:11.000000 django-synkroni-0.4.3/synkroni/templates/synkroni/synkroni.html
--rw-r--r--   0 aha        (501) staff       (20)     1954 2022-10-07 08:47:47.000000 django-synkroni-0.4.3/synkroni/toiminnot.py
--rw-r--r--   0 aha        (501) staff       (20)     5674 2022-10-03 05:46:48.000000 django-synkroni-0.4.3/synkroni/websocket.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 09:02:57.692524 django-synkroni-0.4.7/
+-rw-r--r--   0 aha        (501) staff       (20)       75 2021-09-06 06:31:51.000000 django-synkroni-0.4.7/MANIFEST.in
+-rw-r--r--   0 aha        (501) staff       (20)      242 2023-01-02 09:02:57.692364 django-synkroni-0.4.7/PKG-INFO
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 09:02:57.689529 django-synkroni-0.4.7/django_synkroni.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      242 2023-01-02 09:02:57.000000 django-synkroni-0.4.7/django_synkroni.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      592 2023-01-02 09:02:57.000000 django-synkroni-0.4.7/django_synkroni.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-01-02 09:02:57.000000 django-synkroni-0.4.7/django_synkroni.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)       47 2023-01-02 09:02:57.000000 django-synkroni-0.4.7/django_synkroni.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     8355 2023-01-02 09:02:57.000000 django-synkroni-0.4.7/django_synkroni.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        1 2021-09-06 06:32:14.000000 django-synkroni-0.4.7/django_synkroni.egg-info/not-zip-safe
+-rw-r--r--   0 aha        (501) staff       (20)       34 2023-01-02 09:02:57.000000 django-synkroni-0.4.7/django_synkroni.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        9 2023-01-02 09:02:57.000000 django-synkroni-0.4.7/django_synkroni.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       72 2021-09-06 06:31:51.000000 django-synkroni-0.4.7/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-01-02 09:02:57.692577 django-synkroni-0.4.7/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      568 2022-12-29 11:03:58.000000 django-synkroni-0.4.7/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 09:02:57.691564 django-synkroni-0.4.7/synkroni/
+-rw-r--r--   0 aha        (501) staff       (20)      107 2021-04-07 18:03:12.000000 django-synkroni-0.4.7/synkroni/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      683 2021-09-20 10:38:01.000000 django-synkroni-0.4.7/synkroni/json.py
+-rw-r--r--   0 aha        (501) staff       (20)      261 2021-09-20 10:38:01.000000 django-synkroni-0.4.7/synkroni/komennot.py
+-rw-r--r--   0 aha        (501) staff       (20)      159 2021-04-08 18:06:03.000000 django-synkroni-0.4.7/synkroni/mallit.py
+-rw-r--r--   0 aha        (501) staff       (20)       22 2021-04-08 17:56:03.000000 django-synkroni-0.4.7/synkroni/models.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 09:02:57.687128 django-synkroni-0.4.7/synkroni/static/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 09:02:57.687188 django-synkroni-0.4.7/synkroni/static/synkroni/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 09:02:57.691844 django-synkroni-0.4.7/synkroni/static/synkroni/js/
+-rw-r--r--   0 aha        (501) staff       (20)     9447 2022-09-27 07:22:03.000000 django-synkroni-0.4.7/synkroni/static/synkroni/js/synkroni.js
+-rw-r--r--   0 aha        (501) staff       (20)     2688 2022-11-18 14:29:51.000000 django-synkroni-0.4.7/synkroni/synkroni.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 09:02:57.687344 django-synkroni-0.4.7/synkroni/templates/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-02 09:02:57.692136 django-synkroni-0.4.7/synkroni/templates/synkroni/
+-rw-r--r--   0 aha        (501) staff       (20)      859 2022-05-04 12:06:11.000000 django-synkroni-0.4.7/synkroni/templates/synkroni/synkroni.html
+-rw-r--r--   0 aha        (501) staff       (20)     1905 2022-11-18 13:11:56.000000 django-synkroni-0.4.7/synkroni/toiminnot.py
+-rw-r--r--   0 aha        (501) staff       (20)     5565 2022-11-18 14:29:51.000000 django-synkroni-0.4.7/synkroni/websocket.py
```

### Comparing `django-synkroni-0.4.3/django_synkroni.egg-info/SOURCES.txt` & `django-synkroni-0.4.7/django_synkroni.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.3/django_synkroni.egg-info/historia.json` & `django-synkroni-0.4.7/django_synkroni.egg-info/historia.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {'insert': "[(0, OrderedDict([('tyyppi', 'muutos'), ('tunnus', "*

 * *           "'714853518997b43cf06476748b3ba035e4f844d2'), ('versio', '0.4.7'), ('kuvaus', "*

 * *           "'Django-pistoke 0.8 -yhteensopivuus')])), (1, OrderedDict([('tyyppi', 'muutos'), "*

 * *           "('tunnus', '09092c56648be319f77cb001f5789b862656e543'), ('versio', '0.4.6'), "*

 * *           "('kuvaus', 'Tulostetaan toiminnolla nouseva poikkeus heti')])), (2, "*

 * *           "OrderedDict([('tyyppi', 'muutos'), ('tunnus', "*

 * *           "'c7c687e437baa53 […]*

```diff
@@ -1,9 +1,33 @@
 [
     {
+        "kuvaus": "Django-pistoke 0.8 -yhteensopivuus",
+        "tunnus": "714853518997b43cf06476748b3ba035e4f844d2",
+        "tyyppi": "muutos",
+        "versio": "0.4.7"
+    },
+    {
+        "kuvaus": "Tulostetaan toiminnolla nouseva poikkeus heti",
+        "tunnus": "09092c56648be319f77cb001f5789b862656e543",
+        "tyyppi": "muutos",
+        "versio": "0.4.6"
+    },
+    {
+        "kuvaus": "Peitet\u00e4\u00e4n poikkeus toiminnon paluusanoman muodostuksessa",
+        "tunnus": "c7c687e437baa5387a2dcd43b185dae50693bebd",
+        "tyyppi": "muutos",
+        "versio": "0.4.5"
+    },
+    {
+        "kuvaus": "Lis\u00e4tietoa virheellisen toiminnon yhteydess\u00e4",
+        "tunnus": "d9996afffb86334cb32a5b5c0b0e51de0b72119f",
+        "tyyppi": "muutos",
+        "versio": "0.4.4"
+    },
+    {
         "kuvaus": "Lis\u00e4tty `toiminto{Suoritettu,Epaonnistui}`-metodit",
         "tunnus": "bbf063c36923d929c04ee4cc31b09900b14cc90a",
         "tyyppi": "muutos",
         "versio": "0.4.3"
     },
     {
         "kuvaus": "L\u00e4hetet\u00e4\u00e4n \"yhteys-virhe\", kun WS-yhteyden kautta palautuu HTTP-tilakoodi",
```

### Comparing `django-synkroni-0.4.3/setup.py` & `django-synkroni-0.4.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,13 +11,13 @@
   author_email='antti.hautaniemi@me.com',
   licence='MIT',
   packages=find_packages(),
   include_package_data=True,
   zip_safe=False,
   install_requires=[
     'django>=3.1',
-    'django-pistoke',
+    'django-pistoke>=0.8c1',
   ],
   entry_points={
     'django.sovellus': ['synkroni = synkroni.Synkroni'],
   }
 )
```

### Comparing `django-synkroni-0.4.3/synkroni/json.py` & `django-synkroni-0.4.7/synkroni/json.py`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.3/synkroni/static/synkroni/js/synkroni.js` & `django-synkroni-0.4.7/synkroni/static/synkroni/js/synkroni.js`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.3/synkroni/synkroni.py` & `django-synkroni-0.4.7/synkroni/synkroni.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     Tallenna data yhteyden katkettua.
     '''
     # pylint: disable=attribute-defined-outside-init
     # pylint: disable=no-member
     self.object = await sync_to_async(self.get_object)()
 
-    if self._websocket_kattely.get('uusi'):
+    if request._csrf_kattely.get('uusi'):
       await self.data_paivitetty(
         self.data_alkutilanne,
         self.data,
       )
 
     try:
       while True:
```

### Comparing `django-synkroni-0.4.3/synkroni/templates/synkroni/synkroni.html` & `django-synkroni-0.4.7/synkroni/templates/synkroni/synkroni.html`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.3/synkroni/toiminnot.py` & `django-synkroni-0.4.7/synkroni/toiminnot.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     # def _toiminto
 
   async def suorita_toiminto(self, **kwargs):
     if not kwargs:
       raise ValueError('Toiminnon tiedot puuttuvat: %r' % kwargs)
     _toiminto = self._toiminto(**kwargs)
     assert inspect.isawaitable(_toiminto)
-    print(f'Suoritetaan toiminto {_toiminto!r}')
     return await _toiminto
     # async def suorita_toiminto
 
   @toiminto
   async def yhteys_alustettu(self):
     ''' Yhteyskokeilu. '''
     return {}
```

### Comparing `django-synkroni-0.4.3/synkroni/websocket.py` & `django-synkroni-0.4.7/synkroni/websocket.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 
 from django.utils.functional import cached_property, classproperty
 from django.utils.html import escape
 
 from jsonpatch import JsonPatch, multidict
 
 from pistoke.nakyma import WebsocketNakyma
-from pistoke.tyokalut import csrf_tarkistus, json_viestiliikenne
+from pistoke.protokolla import WebsocketAliprotokolla
+from pistoke.tyokalut import (
+  CsrfKattely,
+  JsonLiikenne,
+)
 
 
 class WebsocketYhteys(WebsocketNakyma):
 
   # Datan alkutilanne sellaisena kuin sekä palvelin että selain
   # sen näkevät.
   data_alkutilanne = {}
@@ -63,23 +67,23 @@
 
     Alustetaan self.toimintojono: tyhjä joukko.
     '''
     # pylint: disable=unidiomatic-typecheck
     if type(self) is __class__:
       raise TypeError(f'{__class__} on abstrakti!')
     super().__init__(*args, **kwargs)
-    #self.toimintojono = set()
+    self.toimintojono = set()
     # def __init__
 
+  websocket_protokolla = 'django-synkroni'
+
   def websocket_protokolla_json(self):
     ''' Palauta JSON-muotoinen tuettujen protokollien luettelo. '''
-    if not getattr(self.websocket, 'protokolla', None):
-      return 'null'
     return escape(self.json_koodain().encode(
-      self.websocket.protokolla
+      [self.websocket_protokolla]
     ))
     # def websocket_protokolla_json
 
   async def data_paivitetty(self, vanha_data, uusi_data):
     ''' Vertaa vanhaa ja uutta dataa; lähetä muutokset selaimelle. '''
     # pylint: disable=no-member
     muutos = self.json_paikkain.from_diff(
@@ -89,38 +93,42 @@
     if muutos:
       await self.request.send(muutos)
     # async def data_paivitetty
 
   async def kasittele_toiminto(self, request, *, toiminto_id, **kwargs):
     try:
       vastaus = await self.suorita_toiminto(**kwargs)
-    # pylint: disable=broad-except
-    except BaseException as exc:
-      # Kuitataan toiminto suoritetuksi poikkeuksesta huolimatta.
       await request.send({
         'toiminto_id': toiminto_id,
+        **(vastaus or {})
       })
-      traceback.print_exception(exc)
-    else:
+    # pylint: disable=broad-except
+    except BaseException:
+      # Kuitataan toiminto suoritetuksi poikkeuksesta huolimatta.
       await request.send({
         'toiminto_id': toiminto_id,
-        **(vastaus or {})
       })
+      raise
     # async def kasittele_toiminto
 
   async def kasittele_saapuva_sanoma(self, request, sanoma):
     ''' Käsittele selaimelta saapuva sanoma. '''
     if 'toiminto_id' in sanoma:
       # Komento: suorita taustalla.
       # Useat peräkkäin saapuvat toiminnot ajetaan samanaikaisesti.
-      await self.kasittele_toiminto(request, **sanoma)
-      #toiminto = asyncio.ensure_future(
-      #  self.kasittele_toiminto(request, **sanoma)
-      #)
-      #self.toimintojono.add(toiminto)
+      toiminto = asyncio.ensure_future(
+        self.kasittele_toiminto(request, **sanoma)
+      )
+      self.toimintojono.add(toiminto)
+      @toiminto.add_done_callback
+      def done(task):
+        try:
+          task.result()
+        except BaseException:
+          traceback.print_exc()
 
     else:
       # Json-paikkaus: toteuta tässä.
       # Huomaa, että paikkaukset on toteutettava peräkkäin
       # saapumisjärjestyksessä, ei samanaikaisesti.
       sanoma = sanoma if isinstance(sanoma, list) else [sanoma]
       # pylint: disable=no-value-for-parameter
@@ -140,42 +148,35 @@
     '''
     try:
       while True:
         sanoma = await request.receive()
         await self.kasittele_saapuva_sanoma(request, sanoma)
         # while True
     finally:
-      pass
-      #for kesken in self.toimintojono:
-      #  kesken.cancel()
-      #tulokset = await asyncio.gather(
-      #  *self.toimintojono,
-      #  return_exceptions=True
-      #)
-      #for tulos in tulokset:
-      #  if isinstance(tulos, BaseException):
-      #    raise tulos
+      for kesken in self.toimintojono:
+        kesken.cancel()
+      await asyncio.gather(*self.toimintojono)
       # finally
     # async def _websocket
 
   async def websocket(self, request, *args, **kwargs):
     ''' JSON-ohjaimet valitaan pyyntökohtaisesti. '''
     # pylint: disable=no-self-argument, arguments-differ
-    @json_viestiliikenne(
+    @WebsocketAliprotokolla(self.websocket_protokolla)
+    @JsonLiikenne(
       # Käytetään luokkakohtaisesti määriteltyä JSON-protokollaa
       # viestinnässä selaimen kanssa.
       loads={'cls': self.json_latain},
       dumps={'cls': self.json_koodain},
     )
-    @csrf_tarkistus(
+    @CsrfKattely(
       csrf_avain='csrfmiddlewaretoken',
       virhe_avain='virhe'
     )
-    async def websocket(self, request, *args, **kwargs):
+    async def websocket(request, *args, **kwargs):
       # pylint: disable=protected-access
       return await self._websocket(request, *args, **kwargs)
       # async def websocket
-    return await websocket(self, request, *args, **kwargs)
+    return await websocket(request, *args, **kwargs)
     # def websocket
-  websocket.protokolla = 'django-synkroni'
 
   # class WebsocketYhteys
```

