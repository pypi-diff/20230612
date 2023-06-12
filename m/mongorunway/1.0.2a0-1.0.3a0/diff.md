# Comparing `tmp/mongorunway-1.0.2a0.tar.gz` & `tmp/mongorunway-1.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongorunway-1.0.2a0.tar", max compression
+gzip compressed data, was "mongorunway-1.0.3a0.tar", max compression
```

## Comparing `mongorunway-1.0.2a0.tar` & `mongorunway-1.0.3a0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0   114798 2023-05-16 15:05:04.927930 mongorunway-1.0.2a0/assets/logo.jpg
--rw-r--r--   0        0        0     1083 2023-04-30 10:29:59.339256 mongorunway-1.0.2a0/LICENSE
--rw-r--r--   0        0        0     1545 2023-06-03 08:57:29.095661 mongorunway-1.0.2a0/mongorunway/__init__.py
--rw-r--r--   0        0        0    10084 2023-06-10 15:04:53.374709 mongorunway-1.0.2a0/mongorunway/api.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.634932 mongorunway-1.0.2a0/mongorunway/application/__init__.py
--rw-r--r--   0        0        0    16023 2023-06-03 10:45:51.886637 mongorunway-1.0.2a0/mongorunway/application/applications.py
--rw-r--r--   0        0        0     4722 2023-06-10 22:12:16.103130 mongorunway-1.0.2a0/mongorunway/application/config.py
--rw-r--r--   0        0        0     6635 2023-06-10 22:12:16.075499 mongorunway-1.0.2a0/mongorunway/application/event_manager.py
--rw-r--r--   0        0        0     1869 2023-06-10 22:12:16.143444 mongorunway-1.0.2a0/mongorunway/application/filesystem.py
--rw-r--r--   0        0        0     3754 2023-06-10 22:12:16.090515 mongorunway-1.0.2a0/mongorunway/application/output.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.653020 mongorunway-1.0.2a0/mongorunway/application/ports/__init__.py
--rw-r--r--   0        0        0     2367 2023-05-29 13:10:46.336291 mongorunway-1.0.2a0/mongorunway/application/ports/auditlog_journal.py
--rw-r--r--   0        0        0     1668 2023-06-03 08:16:22.923990 mongorunway-1.0.2a0/mongorunway/application/ports/config_reader.py
--rw-r--r--   0        0        0     1533 2023-05-29 12:25:19.814965 mongorunway-1.0.2a0/mongorunway/application/ports/filename_strategy.py
--rw-r--r--   0        0        0     3015 2023-06-03 06:50:09.695978 mongorunway-1.0.2a0/mongorunway/application/ports/repository.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.628311 mongorunway-1.0.2a0/mongorunway/application/services/__init__.py
--rw-r--r--   0        0        0     1583 2023-06-03 08:43:33.409655 mongorunway-1.0.2a0/mongorunway/application/services/checksum_service.py
--rw-r--r--   0        0        0     6885 2023-06-10 18:23:19.406553 mongorunway-1.0.2a0/mongorunway/application/services/migration_service.py
--rw-r--r--   0        0        0     2265 2023-06-10 22:12:16.130759 mongorunway-1.0.2a0/mongorunway/application/services/status_service.py
--rw-r--r--   0        0        0     3223 2023-06-03 08:55:00.830346 mongorunway-1.0.2a0/mongorunway/application/services/validation_service.py
--rw-r--r--   0        0        0     1537 2023-05-29 15:33:37.946295 mongorunway-1.0.2a0/mongorunway/application/services/versioning_service.py
--rw-r--r--   0        0        0    17828 2023-06-10 22:12:16.117969 mongorunway-1.0.2a0/mongorunway/application/session.py
--rw-r--r--   0        0        0     2744 2023-06-10 22:12:16.025624 mongorunway-1.0.2a0/mongorunway/application/traits.py
--rw-r--r--   0        0        0     8668 2023-06-09 20:59:37.635169 mongorunway-1.0.2a0/mongorunway/application/transactions.py
--rw-r--r--   0        0        0    13246 2023-06-10 22:06:28.197350 mongorunway-1.0.2a0/mongorunway/application/use_cases.py
--rw-r--r--   0        0        0    10438 2023-06-10 21:57:50.790123 mongorunway-1.0.2a0/mongorunway/application/ux.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.667525 mongorunway-1.0.2a0/mongorunway/domain/__init__.py
--rw-r--r--   0        0        0     5087 2023-06-03 08:42:10.654208 mongorunway-1.0.2a0/mongorunway/domain/migration.py
--rw-r--r--   0        0        0     2923 2023-06-10 22:12:16.063353 mongorunway-1.0.2a0/mongorunway/domain/migration_auditlog_entry.py
--rw-r--r--   0        0        0     2739 2023-06-02 07:43:28.451121 mongorunway-1.0.2a0/mongorunway/domain/migration_business_module.py
--rw-r--r--   0        0        0     2635 2023-06-03 08:55:00.817659 mongorunway-1.0.2a0/mongorunway/domain/migration_business_rule.py
--rw-r--r--   0        0        0     1882 2023-06-03 08:41:58.635457 mongorunway-1.0.2a0/mongorunway/domain/migration_command.py
--rw-r--r--   0        0        0     1550 2023-06-10 22:12:16.038377 mongorunway-1.0.2a0/mongorunway/domain/migration_context.py
--rw-r--r--   0        0        0     2588 2023-06-10 22:12:16.050671 mongorunway-1.0.2a0/mongorunway/domain/migration_event.py
--rw-r--r--   0        0        0     3390 2023-06-10 22:06:28.181157 mongorunway-1.0.2a0/mongorunway/domain/migration_event_manager.py
--rw-r--r--   0        0        0     3385 2023-06-03 10:37:53.057749 mongorunway-1.0.2a0/mongorunway/domain/migration_exception.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.622090 mongorunway-1.0.2a0/mongorunway/infrastructure/__init__.py
--rw-r--r--   0        0        0    18145 2023-06-04 06:30:35.981777 mongorunway-1.0.2a0/mongorunway/infrastructure/commands.py
--rw-r--r--   0        0        0    13603 2023-06-10 17:41:04.343321 mongorunway-1.0.2a0/mongorunway/infrastructure/config_readers.py
--rw-r--r--   0        0        0     4114 2023-06-10 21:42:09.715186 mongorunway-1.0.2a0/mongorunway/infrastructure/event_handlers.py
--rw-r--r--   0        0        0     2806 2023-06-10 13:40:29.075274 mongorunway-1.0.2a0/mongorunway/infrastructure/filename_strategies.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.659732 mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/__init__.py
--rw-r--r--   0        0        0     4536 2023-06-03 13:22:30.753303 mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/auditlog_journals.py
--rw-r--r--   0        0        0     6498 2023-06-03 13:24:34.707047 mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/repositories.py
--rw-r--r--   0        0        0     2874 2023-06-03 08:55:23.935731 mongorunway-1.0.2a0/mongorunway/mongo.py
--rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.640253 mongorunway-1.0.2a0/mongorunway/presentation/__init__.py
--rw-r--r--   0        0        0    15029 2023-06-10 22:18:47.959087 mongorunway-1.0.2a0/mongorunway/presentation/cli.py
--rw-r--r--   0        0        0     2324 2023-06-03 08:16:23.398941 mongorunway-1.0.2a0/mongorunway/presentation/formatters.py
--rw-r--r--   0        0        0     4141 2023-06-10 21:57:50.808767 mongorunway-1.0.2a0/mongorunway/presentation/presenters.py
--rw-r--r--   0        0        0    17080 2023-06-09 19:34:42.546670 mongorunway-1.0.2a0/mongorunway/util.py
--rw-r--r--   0        0        0     4589 2023-06-10 15:17:56.501111 mongorunway-1.0.2a0/PYPI_README.md
--rw-r--r--   0        0        0     2278 2023-06-10 22:18:55.635177 mongorunway-1.0.2a0/pyproject.toml
--rw-r--r--   0        0        0     5895 1970-01-01 00:00:00.000000 mongorunway-1.0.2a0/PKG-INFO
+-rw-r--r--   0        0        0   114798 2023-05-16 15:05:04.927930 mongorunway-1.0.3a0/assets/logo.jpg
+-rw-r--r--   0        0        0     1083 2023-04-30 10:29:59.339256 mongorunway-1.0.3a0/LICENSE
+-rw-r--r--   0        0        0     2141 2023-06-12 15:17:38.242879 mongorunway-1.0.3a0/mongorunway/__init__.py
+-rw-r--r--   0        0        0    10084 2023-06-10 15:04:53.374709 mongorunway-1.0.3a0/mongorunway/api.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.634932 mongorunway-1.0.3a0/mongorunway/application/__init__.py
+-rw-r--r--   0        0        0    16117 2023-06-12 12:11:31.173474 mongorunway-1.0.3a0/mongorunway/application/applications.py
+-rw-r--r--   0        0        0     4711 2023-06-12 12:11:31.188916 mongorunway-1.0.3a0/mongorunway/application/config.py
+-rw-r--r--   0        0        0     6627 2023-06-12 15:17:35.125378 mongorunway-1.0.3a0/mongorunway/application/event_manager.py
+-rw-r--r--   0        0        0     1869 2023-06-10 22:12:16.143444 mongorunway-1.0.3a0/mongorunway/application/filesystem.py
+-rw-r--r--   0        0        0     3754 2023-06-10 22:12:16.090515 mongorunway-1.0.3a0/mongorunway/application/output.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.653020 mongorunway-1.0.3a0/mongorunway/application/ports/__init__.py
+-rw-r--r--   0        0        0     2367 2023-05-29 13:10:46.336291 mongorunway-1.0.3a0/mongorunway/application/ports/auditlog_journal.py
+-rw-r--r--   0        0        0     1668 2023-06-03 08:16:22.923990 mongorunway-1.0.3a0/mongorunway/application/ports/config_reader.py
+-rw-r--r--   0        0        0     1533 2023-05-29 12:25:19.814965 mongorunway-1.0.3a0/mongorunway/application/ports/filename_strategy.py
+-rw-r--r--   0        0        0     3015 2023-06-03 06:50:09.695978 mongorunway-1.0.3a0/mongorunway/application/ports/repository.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.628311 mongorunway-1.0.3a0/mongorunway/application/services/__init__.py
+-rw-r--r--   0        0        0     1583 2023-06-03 08:43:33.409655 mongorunway-1.0.3a0/mongorunway/application/services/checksum_service.py
+-rw-r--r--   0        0        0     6885 2023-06-10 18:23:19.406553 mongorunway-1.0.3a0/mongorunway/application/services/migration_service.py
+-rw-r--r--   0        0        0     2265 2023-06-10 22:12:16.130759 mongorunway-1.0.3a0/mongorunway/application/services/status_service.py
+-rw-r--r--   0        0        0     3223 2023-06-03 08:55:00.830346 mongorunway-1.0.3a0/mongorunway/application/services/validation_service.py
+-rw-r--r--   0        0        0     1537 2023-05-29 15:33:37.946295 mongorunway-1.0.3a0/mongorunway/application/services/versioning_service.py
+-rw-r--r--   0        0        0    17817 2023-06-12 12:12:18.392506 mongorunway-1.0.3a0/mongorunway/application/session.py
+-rw-r--r--   0        0        0     2744 2023-06-10 22:12:16.025624 mongorunway-1.0.3a0/mongorunway/application/traits.py
+-rw-r--r--   0        0        0     8668 2023-06-11 20:46:29.271952 mongorunway-1.0.3a0/mongorunway/application/transactions.py
+-rw-r--r--   0        0        0    17308 2023-06-12 15:17:38.292466 mongorunway-1.0.3a0/mongorunway/application/use_cases.py
+-rw-r--r--   0        0        0    10438 2023-06-10 21:57:50.790123 mongorunway-1.0.3a0/mongorunway/application/ux.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.667525 mongorunway-1.0.3a0/mongorunway/domain/__init__.py
+-rw-r--r--   0        0        0     5087 2023-06-03 08:42:10.654208 mongorunway-1.0.3a0/mongorunway/domain/migration.py
+-rw-r--r--   0        0        0     2915 2023-06-12 15:17:35.044297 mongorunway-1.0.3a0/mongorunway/domain/migration_auditlog_entry.py
+-rw-r--r--   0        0        0     2739 2023-06-02 07:43:28.451121 mongorunway-1.0.3a0/mongorunway/domain/migration_business_module.py
+-rw-r--r--   0        0        0     2635 2023-06-03 08:55:00.817659 mongorunway-1.0.3a0/mongorunway/domain/migration_business_rule.py
+-rw-r--r--   0        0        0     1882 2023-06-03 08:41:58.635457 mongorunway-1.0.3a0/mongorunway/domain/migration_command.py
+-rw-r--r--   0        0        0     1550 2023-06-10 22:12:16.038377 mongorunway-1.0.3a0/mongorunway/domain/migration_context.py
+-rw-r--r--   0        0        0     2676 2023-06-12 09:02:48.786949 mongorunway-1.0.3a0/mongorunway/domain/migration_event.py
+-rw-r--r--   0        0        0     3382 2023-06-12 15:17:35.081376 mongorunway-1.0.3a0/mongorunway/domain/migration_event_manager.py
+-rw-r--r--   0        0        0     3596 2023-06-12 15:17:35.083879 mongorunway-1.0.3a0/mongorunway/domain/migration_exception.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.622090 mongorunway-1.0.3a0/mongorunway/infrastructure/__init__.py
+-rw-r--r--   0        0        0    18145 2023-06-04 06:30:35.981777 mongorunway-1.0.3a0/mongorunway/infrastructure/commands.py
+-rw-r--r--   0        0        0    13641 2023-06-12 15:17:35.213969 mongorunway-1.0.3a0/mongorunway/infrastructure/config_readers.py
+-rw-r--r--   0        0        0     4114 2023-06-10 21:42:09.715186 mongorunway-1.0.3a0/mongorunway/infrastructure/event_handlers.py
+-rw-r--r--   0        0        0     2806 2023-06-10 13:40:29.075274 mongorunway-1.0.3a0/mongorunway/infrastructure/filename_strategies.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.659732 mongorunway-1.0.3a0/mongorunway/infrastructure/persistence/__init__.py
+-rw-r--r--   0        0        0     4546 2023-06-12 13:59:52.705479 mongorunway-1.0.3a0/mongorunway/infrastructure/persistence/auditlog_journals.py
+-rw-r--r--   0        0        0     6466 2023-06-12 15:17:35.142513 mongorunway-1.0.3a0/mongorunway/infrastructure/persistence/repositories.py
+-rw-r--r--   0        0        0     2874 2023-06-03 08:55:23.935731 mongorunway-1.0.3a0/mongorunway/mongo.py
+-rw-r--r--   0        0        0     1225 2023-05-17 16:57:13.640253 mongorunway-1.0.3a0/mongorunway/presentation/__init__.py
+-rw-r--r--   0        0        0    18347 2023-06-12 15:17:35.257219 mongorunway-1.0.3a0/mongorunway/presentation/cli.py
+-rw-r--r--   0        0        0     2324 2023-06-03 08:16:23.398941 mongorunway-1.0.3a0/mongorunway/presentation/formatters.py
+-rw-r--r--   0        0        0     4028 2023-06-12 11:04:18.371307 mongorunway-1.0.3a0/mongorunway/presentation/presenters.py
+-rw-r--r--   0        0        0    17162 2023-06-11 20:46:29.255224 mongorunway-1.0.3a0/mongorunway/util.py
+-rw-r--r--   0        0        0     4589 2023-06-10 15:17:56.501111 mongorunway-1.0.3a0/PYPI_README.md
+-rw-r--r--   0        0        0     2278 2023-06-12 15:36:10.651277 mongorunway-1.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0     5895 1970-01-01 00:00:00.000000 mongorunway-1.0.3a0/PKG-INFO
```

### Comparing `mongorunway-1.0.2a0/assets/logo.jpg` & `mongorunway-1.0.3a0/assets/logo.jpg`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/LICENSE` & `mongorunway-1.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/api.py` & `mongorunway-1.0.3a0/mongorunway/api.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/__init__.py` & `mongorunway-1.0.3a0/mongorunway/application/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/applications.py` & `mongorunway-1.0.3a0/mongorunway/application/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,20 +185,23 @@
         ux.init_logging(configuration)
         ux.init_components(configuration)
 
         self._session = app_session = session.MigrationSessionImpl(self, configuration)
         self._migration_service = migration_service.MigrationService(app_session)
 
         self._event_manager = event_manager.MigrationEventManagerImpl()
-        for event_type, event_handlers in configuration.application.app_subscribed_events.items():
+        for event_type, event_handlers in configuration.application.app_events.items():
             for handler in event_handlers:
                 self._event_manager.subscribe_event_handler(handler, event_type)
 
         self._event_manager.dispatch(domain_event.StartingEvent(self))
 
+    def __del__(self) -> None:
+        self._event_manager.dispatch(domain_event.ClosingEvent(self))
+
     @property
     def name(self) -> str:
         return self._session.session_name
 
     @property
     def session(self) -> session.MigrationSession:
         return self._session
```

### Comparing `mongorunway-1.0.2a0/mongorunway/application/config.py` & `mongorunway-1.0.3a0/mongorunway/application/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         default="UTC",
         repr=True,
     )
     app_date_format: str = attr.field(
         default="%Y-%m-%d %H:%M:%S",
         validator=attr.validators.instance_of(str),
     )
-    app_subscribed_events: typing.Mapping[
+    app_events: typing.Mapping[
         typing.Type[domain_event.MigrationEvent],
         typing.Sequence[domain_event.EventHandlerProxyOr[domain_event.EventHandler]],
     ] = attr.field(factory=dict, repr=False)
     app_auditlog_limit: typing.Optional[int] = attr.field(
         default=None,
         validator=attr.validators.optional(attr.validators.instance_of(int)),
         converter=attr.converters.optional(int),
```

### Comparing `mongorunway-1.0.2a0/mongorunway/application/event_manager.py` & `mongorunway-1.0.3a0/mongorunway/application/event_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from __future__ import annotations
 
-__all__: typing.Sequence[str] = (
-    "MigrationEventManagerImpl",
-)
+__all__: typing.Sequence[str] = ("MigrationEventManagerImpl",)
 
 import collections
 import heapq
 import inspect
 import operator
 import typing
```

### Comparing `mongorunway-1.0.2a0/mongorunway/application/filesystem.py` & `mongorunway-1.0.3a0/mongorunway/application/filesystem.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/output.py` & `mongorunway-1.0.3a0/mongorunway/application/output.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/ports/__init__.py` & `mongorunway-1.0.3a0/mongorunway/application/ports/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/ports/auditlog_journal.py` & `mongorunway-1.0.3a0/mongorunway/application/ports/auditlog_journal.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/ports/config_reader.py` & `mongorunway-1.0.3a0/mongorunway/application/ports/config_reader.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/ports/filename_strategy.py` & `mongorunway-1.0.3a0/mongorunway/application/ports/filename_strategy.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/ports/repository.py` & `mongorunway-1.0.3a0/mongorunway/application/ports/repository.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/services/__init__.py` & `mongorunway-1.0.3a0/mongorunway/application/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/services/checksum_service.py` & `mongorunway-1.0.3a0/mongorunway/application/services/checksum_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/services/migration_service.py` & `mongorunway-1.0.3a0/mongorunway/application/services/migration_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/services/status_service.py` & `mongorunway-1.0.3a0/mongorunway/application/services/status_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/services/validation_service.py` & `mongorunway-1.0.3a0/mongorunway/application/services/validation_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/services/versioning_service.py` & `mongorunway-1.0.3a0/mongorunway/application/services/versioning_service.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/session.py` & `mongorunway-1.0.3a0/mongorunway/application/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
     @property
     def session_subscribed_events(
         self,
     ) -> typing.Mapping[
         typing.Type[domain_event.MigrationEvent],
         typing.Sequence[domain_event.EventHandlerProxyOr[domain_event.EventHandler]],
     ]:
-        return self._config.application.app_subscribed_events
+        return self._config.application.app_events
 
     @property
     def session_auditlog_limit(self) -> typing.Optional[int]:
         return self._config.application.app_auditlog_limit
 
     @property
     def session_config_dir(self) -> str:
```

### Comparing `mongorunway-1.0.2a0/mongorunway/application/traits.py` & `mongorunway-1.0.3a0/mongorunway/application/traits.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/application/transactions.py` & `mongorunway-1.0.3a0/mongorunway/application/transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
         except Exception as exc:
             _LOGGER.error(
                 "Transaction execution in MongoDB session (%s) ended with error %s.",
                 mongodb_session_id,
                 type(exc).__name__,
             )
-            _LOGGER.debug("Error details of transaction execution: %s", str(exc))
+            _LOGGER.error("Error details of transaction execution: %s", str(exc))
 
             self._exc_val = exc
             self.rollback(self._migration, session_context)
 
         if session_context.has_ended:
             _LOGGER.info("MongoDB session %s has ended.", mongodb_session_id)
```

### Comparing `mongorunway-1.0.2a0/mongorunway/application/use_cases.py` & `mongorunway-1.0.3a0/mongorunway/application/use_cases.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,30 +38,36 @@
     "render_downgrade_results",
     "render_error",
     "render_upgrade_results",
     "upgrade",
     "usecase",
     "walk",
     "refresh",
+    "safe_remove_migration",
+    "safe_remove_all_migrations",
+    "check_files",
+    "refresh_checksums",
 )
 
 import datetime
 import functools
+import os
 import sys
 import traceback
 import typing
 
 import typing_extensions
 
 from mongorunway import util
 from mongorunway.application import output
 from mongorunway.application import ux
 from mongorunway.application.ports import config_reader as config_reader_port
 from mongorunway.application.services import migration_service
 from mongorunway.application.services import status_service
+from mongorunway.domain import migration_exception as domain_exception
 
 if typing.TYPE_CHECKING:
     from mongorunway.application import applications
     from mongorunway.application import config
     from mongorunway.domain import migration_auditlog_entry as domain_auditlog_entry
 
 _T = typing.TypeVar("_T")
@@ -112,18 +118,18 @@
     has_verbose_exc: bool,
 ) -> typing.Callable[[typing.Callable[_P, _T]], typing.Callable[_P, ExitCode]]:
     def decorator(func: typing.Callable[_P, _T]) -> typing.Callable[_P, ExitCode]:
         @functools.wraps(func)
         def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> ExitCode:
             try:
                 func(*args, **kwargs)
-            except BaseException as exc:
+            except Exception as exc:
                 render_error(
                     exc,
-                    verbose=typing.cast(
+                    verbose_exc=typing.cast(
                         bool,
                         kwargs["verbose_exc"] if has_verbose_exc else False,
                     ),
                 )
                 return FAILURE
 
             return SUCCESS
@@ -138,18 +144,18 @@
     has_verbose_exc: bool,
 ) -> typing.Callable[[typing.Callable[_P, _T]], typing.Callable[_P, UseCaseFailedOr[_T]]]:
     def decorator(func: typing.Callable[_P, _T]) -> typing.Callable[_P, UseCaseFailedOr[_T]]:
         @functools.wraps(func)
         def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> UseCaseFailedOr[_T]:
             try:
                 callback = func(*args, **kwargs)
-            except BaseException as exc:
+            except Exception as exc:
                 render_error(
                     exc,
-                    verbose=typing.cast(
+                    verbose_exc=typing.cast(
                         bool,
                         kwargs["verbose_exc"] if has_verbose_exc else False,
                     ),
                 )
                 return UseCaseFailed
 
             return callback
@@ -159,15 +165,14 @@
     return decorator
 
 
 @usecase(has_verbose_exc=True)
 def downgrade(
     application: applications.MigrationApp,
     expression: str,
-    verbose: bool,
     verbose_exc: bool,
 ) -> ExitCode:
     func: typing.Optional[typing.Callable[..., ExitCode]] = None
     args: typing.Tuple[typing.Any, ...] = ()
 
     if expression.isdigit():
         func, args = application.downgrade_to, (int(expression),)
@@ -179,27 +184,23 @@
         )
     elif expression == ALL:
         func = application.downgrade_all
 
     if func is None:
         raise ValueError(f"The following expression cannot be applied: {expression!r}")
 
-    render_downgrade_results(
-        verbose,
-        *util.timeit_func(func, *args),
-    )
+    render_downgrade_results(*util.timeit_func(func, *args))
 
     return SUCCESS
 
 
 @usecase(has_verbose_exc=True)
 def upgrade(
     application: applications.MigrationApp,
     expression: str,
-    verbose: bool,
     verbose_exc: bool,
 ) -> ExitCode:
     func: typing.Optional[typing.Callable[..., ExitCode]] = None
     args: typing.Tuple[typing.Any, ...] = ()
 
     if expression.isdigit():
         func, args = application.upgrade_to, (int(expression),)
@@ -211,48 +212,42 @@
         )
     elif expression == ALL:
         func = application.upgrade_all
 
     if func is None:
         raise ValueError(f"The following expression cannot be applied: {expression!r}")
 
-    render_upgrade_results(
-        verbose,
-        *util.timeit_func(func, *args),
-    )
+    render_upgrade_results(*util.timeit_func(func, *args))
 
     return SUCCESS
 
 
 @usecase(has_verbose_exc=True)
 def walk(
     application: applications.MigrationApp,
     expression: str,
-    verbose: bool,
     verbose_exc: bool,
 ) -> ExitCode:
     if expression[0] not in {PLUS, MINUS}:
         raise ValueError(
             "This command can only go in positive or negative order. "
             "Therefore, the expression must begin with either the '+' "
             "or '-' character."
         )
 
     if expression.startswith(MINUS):
         return downgrade(
             application=application,
             expression=expression,
-            verbose=verbose,
             verbose_exc=verbose_exc,
         )
 
     return upgrade(
         application=application,
         expression=expression,
-        verbose=verbose,
         verbose_exc=verbose_exc,
     )
 
 
 @usecase(has_verbose_exc=True)
 def create_migration_file(
     application: applications.MigrationApp,
@@ -266,14 +261,130 @@
     service = migration_service.MigrationService(application.session)
     service.create_migration_file_template(migration_filename, migration_version)
 
     return SUCCESS
 
 
 @usecase(has_verbose_exc=True)
+def safe_remove_migration(
+    application: applications.MigrationApp,
+    migration_version: int,
+    verbose_exc: bool,
+) -> ExitCode:
+    migration = application.session.get_migration_model_by_version(migration_version)
+    output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
+
+    if migration is None:
+        output.print_error(f"Migration with version '{migration_version}' is not found.")
+        return FAILURE
+
+    latest, *_ = application.session.get_all_migration_models(ascending_id=False)
+    if migration.version != latest.version:
+        output.print_error(
+            f"Removing migrations must be sequential."
+            f" "
+            f"The currently available version for deletion is"
+            f" "
+            f"'{latest.version}'"
+        )
+        return FAILURE
+
+    application.session.remove_migration(migration_version)
+    output.print_success(
+        f"Migration with version {migration_version} has been successfully deleted."
+    )
+
+    directory = application.session.session_scripts_dir
+    if os.path.exists(fp := (directory + "\\" + migration.name + ".py")):
+        os.remove(fp)
+
+    return SUCCESS
+
+
+@usecase(has_verbose_exc=True)
+def check_files(
+    application: applications.MigrationApp,
+    raise_exc: bool,
+    verbose_exc: bool,
+) -> ExitCode:
+    service = migration_service.MigrationService(application.session)
+    failed_migrations = []
+    output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
+
+    for migration in application.session.get_all_migration_models():
+        current_migration_state = service.get_migration(migration.name, migration.version)
+        if current_migration_state.checksum != migration.checksum:
+            failed_migrations.append(current_migration_state)
+
+    if failed_migrations:
+        output.print_error(
+            f"'{', '.join(m.name for m in failed_migrations)}' migration file(s) are changed."
+        )
+        if raise_exc:
+            raise domain_exception.MigrationFilesChangedError(*[m.name for m in failed_migrations])
+
+        return FAILURE
+
+    output.print_success("All files remain in their previous state.")
+    return SUCCESS
+
+
+@usecase(has_verbose_exc=True)
+def refresh_checksums(application: applications.MigrationApp, verbose_exc: bool) -> ExitCode:
+    service = migration_service.MigrationService(application.session)
+    modified_files = []
+
+    for migration in application.session.get_all_migration_models():
+        current_migration_state = service.get_migration(migration.name, migration.version)
+
+        if current_migration_state.checksum != migration.checksum:
+            application.session.remove_migration(migration.version)
+            application.session.append_migration(current_migration_state)
+
+            modified_files.append(current_migration_state.name)
+
+    if modified_files:
+        output.print_success(
+            f"'{', '.join(modified_files)}' files have been modified, and their "
+            f"checksums have been successfully updated."
+        )
+    else:
+        output.print_info("All files remain in their previous state.")
+
+    return SUCCESS
+
+
+@usecase(has_verbose_exc=True)
+def safe_remove_all_migrations(
+    application: applications.MigrationApp,
+    verbose_exc: bool,
+) -> ExitCode:
+    migrations = application.session.get_all_migration_models()
+
+    output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
+    if not migrations:
+        output.print_error("There is no migrations.")
+        return FAILURE
+
+    for migration in migrations:
+        application.session.remove_migration(migration.version)
+
+    directory = application.session.session_scripts_dir
+    for file_name in os.listdir(directory):
+        if file_name.startswith("_") or not file_name.endswith(".py"):
+            continue
+
+        file_path = os.path.join(directory, file_name)
+        os.remove(file_path)
+
+    output.print_success(f"Successfully deleted {len(migrations)} migration(s).")
+    return SUCCESS
+
+
+@usecase(has_verbose_exc=True)
 def init(
     application: applications.MigrationApp,
     verbose_exc: bool,
     init_scripts_dir: bool,
     init_collection: bool,
     init_collection_indexes: bool,
     init_collection_schema_validation: bool,
@@ -295,17 +406,17 @@
 def refresh(
     application: applications.MigrationApp,
     verbose_exc: bool,
 ) -> ExitCode:
     synced_names = ux.sync_scripts_with_repository(application)
     output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
     if synced_names:
-        output.print_info(f"'{', '.join(synced_names)}' migrations was successfully synced.")
+        output.print_success(f"'{', '.join(synced_names)}' migration(s) was successfully synced.")
     else:
-        output.print_info("There is no unsynced migrations.")
+        output.print_error("There is no unsynced migrations.")
 
     return SUCCESS
 
 
 @query_usecase(has_verbose_exc=True)
 def get_auditlog_entries(
     application: applications.MigrationApp,
@@ -352,15 +463,19 @@
 def read_configuration(
     config_filepath: typing.Optional[str],
     *,
     app_name: str,
     verbose_exc: bool,
 ) -> UseCaseFailedOr[config.Config]:
     reader: typing.Optional[config_reader_port.ConfigReader] = None
-    if config_filepath is None or config_filepath.endswith(".yaml"):  # Default reader
+    if (
+        config_filepath is None
+        or config_filepath.endswith(".yaml")
+        or config_filepath.endswith(".yml")
+    ):  # Default reader
         reader = util.import_obj(
             "mongorunway.infrastructure.config_readers.YamlConfigReader",
             cast=config_reader_port.ConfigReader,
         ).from_application_name(app_name)
 
     if reader is None:
         output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
@@ -372,31 +487,28 @@
         output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
         output.print_error(f"Cannot find any configuration files in {config_filepath} directory.")
         return UseCaseFailed
 
     return configuration
 
 
-def render_error(exc: BaseException, verbose: bool = False) -> None:
+def render_error(exc: Exception, verbose_exc: bool = False) -> None:
     output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
     output.print_warning(type(exc).__name__ + " : " + str(exc))
 
-    if verbose:
+    if verbose_exc:
         exc_info = traceback.format_exception(*sys.exc_info())
         output.print_error("\n".join(exc_info))
 
 
-def render_downgrade_results(verbose: bool, downgraded_count: int, executed_in: float) -> None:
+def render_downgrade_results(downgraded_count: int, executed_in: float) -> None:
     output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
-    output.verbose_print(verbose, "Verbose mode enabled.")
     output.print_success(f"Successfully downgraded {downgraded_count} migration(s).")
-    output.verbose_print(
-        verbose,
+    output.print_info(
         f"Downgraded {downgraded_count} migration(s) in {executed_in}s.",
     )
 
 
-def render_upgrade_results(verbose: bool, upgraded_count: int, executed_in: float) -> None:
+def render_upgrade_results(upgraded_count: int, executed_in: float) -> None:
     output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
-    output.verbose_print(verbose, "Verbose mode enabled.")
     output.print_success(f"Successfully upgraded {upgraded_count} migration(s).")
-    output.verbose_print(verbose, f"Upgraded {upgraded_count} migration(s) in {executed_in}s.")
+    output.print_info(f"Upgraded {upgraded_count} migration(s) in {executed_in}s.")
```

### Comparing `mongorunway-1.0.2a0/mongorunway/application/ux.py` & `mongorunway-1.0.3a0/mongorunway/application/ux.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/__init__.py` & `mongorunway-1.0.3a0/mongorunway/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/migration.py` & `mongorunway-1.0.3a0/mongorunway/domain/migration.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/migration_auditlog_entry.py` & `mongorunway-1.0.3a0/mongorunway/domain/migration_auditlog_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from __future__ import annotations
 
-__all__: typing.Sequence[str] = (
-    "MigrationAuditlogEntry",
-)
+__all__: typing.Sequence[str] = ("MigrationAuditlogEntry",)
 
 import dataclasses
 import datetime
 import typing
 import zoneinfo
 
 import bson.binary
```

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/migration_business_module.py` & `mongorunway-1.0.3a0/mongorunway/domain/migration_business_module.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/migration_business_rule.py` & `mongorunway-1.0.3a0/mongorunway/domain/migration_business_rule.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/migration_command.py` & `mongorunway-1.0.3a0/mongorunway/domain/migration_command.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/migration_context.py` & `mongorunway-1.0.3a0/mongorunway/domain/migration_context.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/migration_event.py` & `mongorunway-1.0.3a0/mongorunway/domain/migration_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 __all__: typing.Sequence[str] = (
     "EventHandler",
     "EventHandlerProxy",
     "EventHandlerProxyOr",
     "EventHandlerT",
     "StartingEvent",
+    "ClosingEvent",
     "ApplicationEvent",
     "MigrationEvent",
 )
 
 import typing
 
 import attr
@@ -79,7 +80,12 @@
 class ApplicationEvent(MigrationEvent):
     application: applications.MigrationApp = attr.field()
 
 
 @attr.define
 class StartingEvent(ApplicationEvent):
     pass
+
+
+@attr.define
+class ClosingEvent(ApplicationEvent):
+    pass
```

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/migration_event_manager.py` & `mongorunway-1.0.3a0/mongorunway/domain/migration_event_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from __future__ import annotations
 
-__all__: typing.Sequence[str] = (
-    "MigrationEventManager",
-)
+__all__: typing.Sequence[str] = ("MigrationEventManager",)
 
 import abc
 import typing
 
 if typing.TYPE_CHECKING:
     from mongorunway.domain import migration_event as domain_event
```

### Comparing `mongorunway-1.0.2a0/mongorunway/domain/migration_exception.py` & `mongorunway-1.0.3a0/mongorunway/domain/migration_exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 __all__: typing.Sequence[str] = (
     "MigrationError",
     "MigrationFailedError",
     "MigrationTransactionFailedError",
     "NothingToUpgradeError",
     "NothingToDowngradeError",
-    "MigrationHookError",
+    "MigrationFilesChangedError",
     "MigrationFileChangedError",
 )
 
 import typing
 
 if typing.TYPE_CHECKING:
     from mongorunway.domain import migration as domain_migration
@@ -78,26 +78,29 @@
 class NothingToDowngradeError(MigrationFailedError):
     __slots__: typing.Sequence[str] = ()
 
     def __str__(self) -> str:
         return "There are currently no applied migrations."
 
 
-class MigrationHookError(MigrationError):
-    __slots__: typing.Sequence[str] = ()
-
-    pass
-
-
-class MigrationFileChangedError(MigrationHookError):
+class MigrationFileChangedError(BaseException):
     __slots__: typing.Sequence[str] = (
         "failed_migration_name",
         "failed_migration_version",
     )
 
     def __init__(self, migration_name: str, migration_version: int) -> None:
         self.failed_migration_name = migration_name
         self.failed_migration_version = migration_version
 
         super().__init__(
             f"Migration {migration_name!r} with version {migration_version!r} is changed."
         )
+
+
+class MigrationFilesChangedError(BaseException):
+    __slots__: typing.Sequence[str] = ("migration_names",)
+
+    def __init__(self, *migration_names: str) -> None:
+        self.migration_names = migration_names
+
+        super().__init__(f"{migration_names!r} migrations files have been modified.")
```

### Comparing `mongorunway-1.0.2a0/mongorunway/infrastructure/__init__.py` & `mongorunway-1.0.3a0/mongorunway/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/infrastructure/commands.py` & `mongorunway-1.0.3a0/mongorunway/infrastructure/commands.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/infrastructure/config_readers.py` & `mongorunway-1.0.3a0/mongorunway/infrastructure/config_readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from __future__ import annotations
 
 __all__: typing.Sequence[str] = (
-    "default_repository_reader",
-    "default_auditlog_journal_reader",
+    "default_mongo_repository_reader",
+    "default_mongo_auditlog_journal_reader",
     "read_repository",
     "read_events",
     "read_event_handlers",
     "read_auditlog_journal",
     "read_filename_strategy",
     "BaseConfigReader",
     "YamlConfigReader",
@@ -82,33 +82,33 @@
             "formatter": "simpleFormatter",
         }
     },
     "loggers": {"root": {"level": "INFO", "handlers": ["consoleHandler"], "propagate": 0}},
 }
 
 
-def default_repository_reader(
+def default_mongo_repository_reader(
     application_data: typing.Dict[str, typing.Any],
 ) -> repository_port.MigrationModelRepository:
     client = mongo.Client(**util.build_mapping_values(application_data["app_client"]))
     database = client.get_database(application_data["app_database"])
     collection = database.get_collection(application_data["app_repository"]["collection"])
     return repositories.MongoModelRepositoryImpl(collection)
 
 
-def default_auditlog_journal_reader(
+def default_mongo_auditlog_journal_reader(
     application_data: typing.Dict[str, typing.Any],
 ) -> typing.Optional[auditlog_journal_port.AuditlogJournal]:
     if (collection := application_data["app_auditlog_journal"].get("collection")) is None:
         return None
 
     client = mongo.Client(**util.build_mapping_values(application_data["app_client"]))
     database = client.get_database(application_data["app_database"])
     collection = database.get_collection(collection)
-    return auditlog_journals.AuditlogJournalImpl(collection)
+    return auditlog_journals.MongoAuditlogJournalImpl(collection)
 
 
 @typing.no_type_check
 def read_event_handlers(
     handler_name_seq: typing.Sequence[str],
 ) -> typing.List[domain_event.EventHandlerProxyOr[domain_event.EventHandler]]:
     handlers: typing.List[domain_event.EventHandlerProxyOr[domain_event.EventHandler]] = []
@@ -187,15 +187,15 @@
                     repository_port.MigrationModelRepository,
                 ],
             )
             return reader(application_data)
 
         if (repo_type := application_data.get("type")) is None:
             reader = util.import_obj(
-                "mongorunway.infrastructure.config_readers.default_repository_reader",
+                "mongorunway.infrastructure.config_readers.default_mongo_repository_reader",
                 cast=typing.Callable[
                     [typing.Dict[str, typing.Any]],
                     repository_port.MigrationModelRepository,
                 ],
             )
             return reader(application_data)
 
@@ -226,15 +226,15 @@
                     auditlog_journal_port.AuditlogJournal,
                 ],
             )
             return reader(application_data)
 
         if (audit_type := application_data.get("type")) is None:
             reader = util.import_obj(
-                "mongorunway.infrastructure.config_readers.default_auditlog_journal_reader",
+                "mongorunway.infrastructure.config_readers.default_mongo_auditlog_journal_reader",
                 cast=typing.Callable[
                     [typing.Dict[str, typing.Any]],
                     auditlog_journal_port.AuditlogJournal,
                 ],
             )
             return reader(application_data)
 
@@ -281,15 +281,15 @@
 
     @abc.abstractmethod
     def _read_config(self, config_filepath: str) -> typing.Optional[config.Config]:
         ...
 
 
 class YamlConfigReader(BaseConfigReader):
-    potential_config_filenames = ["mongorunway.yaml"]
+    potential_config_filenames = ["mongorunway.yaml", "mongorunway.yml"]
 
     def _read_config(self, config_filepath: str) -> typing.Optional[config.Config]:
         with open(config_filepath, "r") as config_file:
             configration_data = yaml.safe_load(config_file)["mongorunway"]
 
         return config.Config(
             filesystem=self._read_filesystem_config(
@@ -330,15 +330,15 @@
             app_name=self.application_name,
             app_client=(
                 client := mongo.Client(**util.build_mapping_values(application_data["app_client"]))
             ),
             app_database=client.get_database(application_data["app_database"]),
             app_repository=read_repository(application_data),
             app_auditlog_journal=read_auditlog_journal(application_data),
-            app_subscribed_events=read_events(application_data.get("app_subscribed_events", {})),
+            app_events=read_events(application_data.get("app_events", {})),
             **util.build_optional_kwargs(
                 (
                     "app_timezone",
                     "app_date_format",
                     "app_auditlog_limit",
                     "use_logging",
                     "use_auditlog",
```

### Comparing `mongorunway-1.0.2a0/mongorunway/infrastructure/event_handlers.py` & `mongorunway-1.0.3a0/mongorunway/infrastructure/event_handlers.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/infrastructure/filename_strategies.py` & `mongorunway-1.0.3a0/mongorunway/infrastructure/filename_strategies.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/__init__.py` & `mongorunway-1.0.3a0/mongorunway/infrastructure/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/auditlog_journals.py` & `mongorunway-1.0.3a0/mongorunway/infrastructure/persistence/auditlog_journals.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from __future__ import annotations
 
-__all__: typing.Sequence[str] = ("AuditlogJournalImpl",)
+__all__: typing.Sequence[str] = ("MongoAuditlogJournalImpl",)
 
 import dataclasses
 import datetime
 import typing
 
 import pymongo
 
@@ -32,15 +32,15 @@
 from mongorunway.domain import migration as domain_migration
 from mongorunway.domain import migration_auditlog_entry as domain_auditlog_entry
 
 if typing.TYPE_CHECKING:
     from mongorunway import mongo
 
 
-class AuditlogJournalImpl(auditlog_journal_port.AuditlogJournal):
+class MongoAuditlogJournalImpl(auditlog_journal_port.AuditlogJournal):
     __slots__: typing.Sequence[str] = ("_collection", "_max_records")
 
     def __init__(
         self,
         auditlog_collection: mongo.Collection,
         max_records: typing.Optional[int] = None,
     ) -> None:
```

### Comparing `mongorunway-1.0.2a0/mongorunway/infrastructure/persistence/repositories.py` & `mongorunway-1.0.3a0/mongorunway/infrastructure/persistence/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,15 @@
             return NotImplemented
 
         with self._lock:
             return self.has_migration_with_version(version)
 
     def has_migration_with_version(self, migration_version: int, /) -> bool:
         with self._lock:
-            return self._collection.count_documents(
-                {"_id": migration_version}
-            ) > 0
+            return self._collection.count_documents({"_id": migration_version}) > 0
 
     def has_migrations(self) -> bool:
         with self._lock:
             return bool(
                 self._collection.count_documents(
                     {},
                     limit=1,
```

### Comparing `mongorunway-1.0.2a0/mongorunway/mongo.py` & `mongorunway-1.0.3a0/mongorunway/mongo.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/presentation/__init__.py` & `mongorunway-1.0.3a0/mongorunway/presentation/__init__.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/presentation/cli.py` & `mongorunway-1.0.3a0/mongorunway/presentation/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     "status",
     "walk",
     "downgrade",
     "upgrade",
     "refresh",
     "version",
     "init",
+    "safe_remove",
+    "safe_remove_all",
+    "check_files",
+    "refresh_checksums",
 )
 
 import functools
 import sys
 import typing
 
 import click
@@ -75,22 +79,17 @@
 @click.group()
 def cli() -> None:
     pass
 
 
 @cli.command()
 @click.option(
-    "--verbose",
-    is_flag=True,
-    help="Enable verbose output during the upgrade process."
-)
-@click.option(
     "--verbose-exc",
     is_flag=True,
-    help="Enable verbose output for exceptions during the upgrade process."
+    help="Enable verbose output for exceptions during the upgrade process.",
 )
 @click.argument(
     "application_name",
     type=click.STRING,
     metavar="APPLICATION_NAME",
     required=True,
 )
@@ -101,44 +100,37 @@
     metavar="EXPRESSION",
     required=False,
 )
 @pass_application
 def upgrade(
     application: applications.MigrationApp,
     expression: str,
-    verbose: bool,
     verbose_exc: bool,
     **params: typing.Any,
 ) -> None:
     """Upgrade the specified application.
 
     This command allows you to upgrade the specified application using the
     given expression or additional arguments. Optionally, you can enable
     verbose output or verbose output for exceptions during the upgrade process.
     """
 
     exit_code = use_cases.upgrade(
         application=application,
         expression=expression,
-        verbose=verbose,
         verbose_exc=verbose_exc,
     )
     sys.exit(exit_code)
 
 
 @cli.command()
 @click.option(
-    "--verbose",
-    is_flag=True,
-    help="Enable verbose output during the downgrade process."
-)
-@click.option(
     "--verbose-exc",
     is_flag=True,
-    help="Enable verbose output for exceptions during the downgrade process."
+    help="Enable verbose output for exceptions during the downgrade process.",
 )
 @click.argument(
     "application_name",
     type=click.STRING,
     metavar="APPLICATION_NAME",
     required=True,
 )
@@ -149,44 +141,37 @@
     metavar="EXPRESSION",
     required=False,
 )
 @pass_application
 def downgrade(
     application: applications.MigrationApp,
     expression: str,
-    verbose: bool,
     verbose_exc: bool,
     **params: typing.Any,
 ) -> None:
     """Downgrade the specified application.
 
     This command allows you to downgrade the specified application using the
     given expression or additional arguments. Optionally, you can enable verbose
     output or verbose output for exceptions during the downgrade process.
     """
 
     exit_code = use_cases.downgrade(
         application=application,
         expression=expression,
-        verbose=verbose,
         verbose_exc=verbose_exc,
     )
     sys.exit(exit_code)
 
 
 @cli.command()
 @click.option(
-    "--verbose",
-    is_flag=True,
-    help="Enable verbose output during the walk process."
-)
-@click.option(
     "--verbose-exc",
     is_flag=True,
-    help="Enable verbose output for exceptions during the walk process."
+    help="Enable verbose output for exceptions during the walk process.",
 )
 @click.argument(
     "application_name",
     type=click.STRING,
     metavar="APPLICATION_NAME",
     required=True,
 )
@@ -196,15 +181,14 @@
     metavar="EXPRESSION",
     required=True,
 )
 @pass_application
 def walk(
     application: applications.MigrationApp,
     expression: str,
-    verbose: bool,
     verbose_exc: bool,
     **params: typing.Any,
 ) -> None:
     """
     Walk through the specified application.
 
     This command allows you to perform a walk operation on the specified
@@ -215,39 +199,35 @@
     Optionally, you can enable verbose output or verbose output for exceptions
     during the walk process.
     """
 
     exit_code = use_cases.walk(
         application=application,
         expression=expression,
-        verbose=verbose,
         verbose_exc=verbose_exc,
     )
     sys.exit(exit_code)
 
 
 @cli.command()
 @click.option(
-    "-n",
-    "--name",
-    type=click.STRING,
-    help="Specify the name of the migration template."
+    "-n", "--name", type=click.STRING, help="Specify the name of the migration template."
 )
 @click.option(
     "-v",
     "--version",
     type=click.INT,
     default=None,
     required=False,
-    help="Specify the version number of the migration template."
+    help="Specify the version number of the migration template.",
 )
 @click.option(
     "--verbose-exc",
     is_flag=True,
-    help="Enable verbose output for exceptions during the template creation process."
+    help="Enable verbose output for exceptions during the template creation process.",
 )
 @click.argument(
     "application_name",
     type=click.STRING,
     metavar="APPLICATION_NAME",
     required=True,
 )
@@ -307,42 +287,36 @@
         verbose_exc=verbose_exc,
     )
     sys.exit(exit_code)
 
 
 @cli.command()
 @click.option(
-    "--verbose",
-    is_flag=True,
-    help="Enable verbose output for the status command."
-)
-@click.option(
     "--verbose-exc",
     is_flag=True,
-    help="Enable verbose output for exceptions during the status command."
+    help="Enable verbose output for exceptions during the status command.",
 )
 @click.option(
     "-d",
     "--depth",
     type=click.INT,
     default=-1,
     required=False,
-    help="Specify the depth of the migration history to display."
+    help="Specify the depth of the migration history to display.",
 )
 @click.argument(
     "application_name",
     type=click.STRING,
     metavar="APPLICATION_NAME",
     required=True,
 )
 @pass_application
 def status(
     application: applications.MigrationApp,
     depth: int,
-    verbose: bool,
     verbose_exc: bool,
     **params: typing.Any,
 ) -> None:
     """Display the migration status for the specified application.
 
     This command allows you to view the migration status of the specified
     application. It shows the history of applied migrations up to the
@@ -351,53 +325,52 @@
     Optionally, you can enable verbose output for the status command and
     verbose output for exceptions that may occur during the status check.
     """
 
     presenters.show_status(
         application=application,
         pushed_depth=depth,
-        verbose=verbose,
         verbose_exc=verbose_exc,
     )
 
 
 @cli.command()
 @click.option(
     "-s",
     "--start",
     type=click.STRING,
     default=None,
     nargs="?",
-    help="Specify the start timestamp or date for filtering audit log entries."
+    help="Specify the start timestamp or date for filtering audit log entries.",
 )
 @click.option(
     "-e",
     "--end",
     type=click.STRING,
     default=None,
     nargs="?",
-    help="Specify the end timestamp or date for filtering audit log entries."
+    help="Specify the end timestamp or date for filtering audit log entries.",
 )
 @click.option(
     "-l",
     "--limit",
     type=click.INT,
     default=10,
-    help="Specify the maximum number of audit log entries to display."
+    help="Specify the maximum number of audit log entries to display.",
 )
 @click.option(
     "-a",
     "--ascending",
     is_flag=True,
-    help="Sort the audit log entries in ascending order by date."
+    help="Sort the audit log entries in ascending order by date.",
 )
 @click.option(
     "--verbose-exc",
     is_flag=True,
-    help="Enable verbose output for exceptions during the audit log command."
+    help="Enable verbose output for exceptions during the audit log command.",
 )
 @click.argument(
     "application_name",
     type=click.STRING,
     metavar="APPLICATION_NAME",
     required=True,
 )
@@ -431,69 +404,62 @@
         verbose_exc=verbose_exc,
         ascending_date=ascending,
     )
 
 
 @cli.command()
 @click.option(
-    "--verbose",
-    is_flag=True,
-    help="Enable verbose output for the version command."
-)
-@click.option(
     "--verbose-exc",
     is_flag=True,
-    help="Enable verbose output for exceptions during the version command."
+    help="Enable verbose output for exceptions during the version command.",
 )
 @click.argument(
     "application_name",
     type=click.STRING,
     metavar="APPLICATION_NAME",
     required=True,
 )
 @pass_application
-def version(application: applications.MigrationApp, verbose: bool, **params: typing.Any) -> None:
+def version(application: applications.MigrationApp, **params: typing.Any) -> None:
     """Display the version information for the specified application.
 
     This command allows you to view the version information of the
     specified application. It shows details such as the application's
     name, version number, and other relevant details.
 
     Optionally, you can enable verbose output for the version command
     to get more detailed information.
     """
 
-    presenters.show_version(application=application, verbose=verbose)
+    presenters.show_version(application=application)
 
 
 @cli.command()
 @click.option(
     "--verbose-exc",
     is_flag=True,
-    help="Enable verbose output for exceptions during the init command."
+    help="Enable verbose output for exceptions during the init command.",
 )
 @click.option(
     "--scripts-dir",
     is_flag=True,
-    help="Initialize the scripts directory for the specified application."
+    help="Initialize the scripts directory for the specified application.",
 )
 @click.option(
-    "--collection",
-    is_flag=True,
-    help="Initialize the collection for the specified application."
+    "--collection", is_flag=True, help="Initialize the collection for the specified application."
 )
 @click.option(
     "--indexes",
     is_flag=True,
-    help="Initialize the indexes for the specified application's collection."
+    help="Initialize the indexes for the specified application's collection.",
 )
 @click.option(
     "--schema-validation",
     is_flag=True,
-    help="Enable schema validation for the specified application's collection."
+    help="Enable schema validation for the specified application's collection.",
 )
 @click.argument(
     "application_name",
     type=click.STRING,
     metavar="APPLICATION_NAME",
     required=True,
 )
@@ -538,7 +504,160 @@
         verbose_exc=verbose_exc,
         init_scripts_dir=scripts_dir,
         init_collection=collection,
         init_collection_indexes=indexes,
         init_collection_schema_validation=schema_validation,
     )
     sys.exit(exit_code)
+
+
+@cli.command()
+@click.option(
+    "--verbose-exc",
+    is_flag=True,
+    help="Enable verbose exception output.",
+)
+@click.argument(
+    "application_name",
+    type=click.STRING,
+    metavar="APPLICATION_NAME",
+    required=True,
+)
+@click.argument(
+    "migration_version",
+    type=click.INT,
+    metavar="MIGRATION_VERSION",
+    required=True,
+)
+@pass_application
+def safe_remove(
+    application: applications.MigrationApp,
+    migration_version: int,
+    verbose_exc: bool,
+    **params: typing.Any,
+) -> None:
+    """Safely removes a migration from the specified application.
+
+    This command allows you to safely remove a migration from the
+    specified application. It ensures that the removal process is
+    handled securely and provides an option to enable verbose
+    exception output for detailed error messages.
+    """
+
+    exit_code = use_cases.safe_remove_migration(
+        application=application,
+        migration_version=migration_version,
+        verbose_exc=verbose_exc,
+    )
+    sys.exit(exit_code)
+
+
+@cli.command()
+@click.option(
+    "--verbose-exc",
+    is_flag=True,
+    help="Enable verbose exception output.",
+)
+@click.argument(
+    "application_name",
+    type=click.STRING,
+    metavar="APPLICATION_NAME",
+    required=True,
+)
+@pass_application
+def safe_remove_all(
+    application: applications.MigrationApp,
+    verbose_exc: bool,
+    **params: typing.Any,
+) -> None:
+    """Safely removes all migrations from the specified application.
+
+    This command allows you to safely remove all migrations from the
+    specified application. It ensures that the removal process is
+    handled securely and provides an option to enable verbose exception
+    output for detailed error messages.
+    """
+
+    exit_code = use_cases.safe_remove_all_migrations(
+        application=application,
+        verbose_exc=verbose_exc,
+    )
+    sys.exit(exit_code)
+
+
+@cli.command()
+@click.option(
+    "--verbose-exc",
+    is_flag=True,
+    help="Enable verbose exception output.",
+)
+@click.option(
+    "--raise-exc",
+    is_flag=True,
+    help="Throws an exception if a mismatch is found.",
+)
+@click.argument(
+    "application_name",
+    type=click.STRING,
+    metavar="APPLICATION_NAME",
+    required=True,
+)
+@pass_application
+def check_files(
+    application: applications.MigrationApp,
+    raise_exc: bool,
+    verbose_exc: bool,
+    **params: typing.Any,
+) -> None:
+    """Check the integrity of files in the specified application.
+
+    This command verifies the integrity of files in the specified
+    application. It compares the checksums of the files stored in
+    the repository with the checksums of the corresponding files
+    in the file system. If any differences are found, an appropriate
+    message is displayed.
+    """
+
+    exit_code = use_cases.check_files(
+        application=application,
+        raise_exc=raise_exc,
+        verbose_exc=verbose_exc,
+    )
+    sys.exit(exit_code)
+
+
+@cli.command()
+@click.option(
+    "--verbose-exc",
+    is_flag=True,
+    help="Enable verbose exception output.",
+)
+@click.argument(
+    "application_name",
+    type=click.STRING,
+    metavar="APPLICATION_NAME",
+    required=True,
+)
+@pass_application
+def refresh_checksums(
+    application: applications.MigrationApp,
+    verbose_exc: bool,
+    **params: typing.Any,
+) -> None:
+    """Refresh the checksums of files in the specified application.
+
+    This command updates the checksums of files in the specified
+    application. It recalculates the checksums of all files in the
+    repository and updates them accordingly. This can be useful when
+    the files in the application have been modified or when the
+    checksums need to be synchronized with the repository.
+    """
+
+    exit_code = use_cases.refresh_checksums(
+        application=application,
+        verbose_exc=verbose_exc,
+    )
+    sys.exit(exit_code)
+
+
+if __name__ == "__main__":
+    cli()
```

### Comparing `mongorunway-1.0.2a0/mongorunway/presentation/formatters.py` & `mongorunway-1.0.3a0/mongorunway/presentation/formatters.py`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/mongorunway/presentation/presenters.py` & `mongorunway-1.0.3a0/mongorunway/presentation/presenters.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,30 +62,28 @@
                     ["Date", "Is Failed", "Transaction Type", "Migration"],
                     *(formatters.format_auditlog_entry(entry) for entry in entries_result),
                 ]
             ).table
         )
 
 
-def show_version(application: applications.MigrationApp, verbose: bool) -> None:
+def show_version(application: applications.MigrationApp) -> None:
     version_result = application.session.get_current_version()
 
     if version_result is not use_cases.UseCaseFailed:
         presentation = f"Current applied version is {version_result}"
-        if verbose:
-            all_applied_migrations_len = len(list(application.session.get_all_migration_models()))
-            presentation += f" " + f"({version_result} of {all_applied_migrations_len})"
+        all_applied_migrations_len = len(list(application.session.get_all_migration_models()))
+        presentation += f" " + f"({version_result} of {all_applied_migrations_len})"
 
         output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
         output.print_success(presentation)
 
 
 def show_status(
     application: applications.MigrationApp,
-    verbose: bool,
     verbose_exc: bool,
     pushed_depth: int = -1,
 ) -> None:
     status_result = use_cases.get_status(
         application=application,
         verbose_exc=verbose_exc,
         pushed_depth=pushed_depth,
@@ -94,16 +92,15 @@
     if status_result is not use_cases.UseCaseFailed:
         all_pushed_successfully, pushed_depth = status_result
         if all_pushed_successfully:
             presentation = f"All migrations applied successfully in depth {pushed_depth!r}"
         else:
             presentation = f"Applying failed in depth {pushed_depth!r}"
 
-        if verbose:
-            presentation += f" " + (
-                f"({application.session.get_current_version()}"
-                f" "
-                f"of {len(list(application.session.get_all_migration_models()))})"
-            )
+        presentation += f" " + (
+            f"({application.session.get_current_version()}"
+            f" "
+            f"of {len(list(application.session.get_all_migration_models()))})"
+        )
 
-            output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
-            output.print_info(presentation)
+        output.print_heading(output.HEADING_LEVEL_ONE, output.TOOL_HEADING_NAME)
+        output.print_info(presentation)
```

### Comparing `mongorunway-1.0.2a0/mongorunway/util.py` & `mongorunway-1.0.3a0/mongorunway/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 import binascii
 import copy
 import distutils.util
 import importlib
 import importlib.util
 import os
 import re
+import sys
 import time
 import types
 import typing
 
 import bson
 import typing_extensions
 
@@ -308,26 +309,29 @@
     >>> assert isinstance(get_module("", "util"), ModuleType)
     ```
 
     See Also
     --------
     importlib.spec_from_file_location
     """
+    sys.path.append(os.getcwd())
     if not filename.endswith(".py"):
         filename += ".py"
 
     spec = importlib.util.spec_from_file_location(
         filename.rstrip(".py"), (path := os.path.join(directory, filename))
     )
     if spec is None:
         raise ModuleNotFoundError(f"Module {path!r} is not found.")
 
     module = importlib.util.module_from_spec(spec)
     assert spec.loader is not None  # For type checkers only
     spec.loader.exec_module(module)
+
+    sys.path.remove(os.getcwd())
     return module
 
 
 def import_obj(obj_path: str, /, cast: _TT) -> _TT:
     r"""Imports a class from the specified module.
 
     Imports a class from the specified module. The module path should
```

### Comparing `mongorunway-1.0.2a0/PYPI_README.md` & `mongorunway-1.0.3a0/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `mongorunway-1.0.2a0/pyproject.toml` & `mongorunway-1.0.3a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ["py39"]
 
 [tool.poetry]
 name = "mongorunway"
-version = "1.0.2a"
+version = "1.0.3a"
 description = "A MongoDB migration tool."
 authors = ["Animatea <animatea.programming@gmail.com>"]
 readme = "PYPI_README.md"
 license = "MIT"
 homepage = "https://github.com/Animatea/mongorunway"
 repository = "https://github.com/Animatea/mongorunway"
 documentation = "https://animatea.github.io/mongorunway/"
```

### Comparing `mongorunway-1.0.2a0/PKG-INFO` & `mongorunway-1.0.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongorunway
-Version: 1.0.2a0
+Version: 1.0.3a0
 Summary: A MongoDB migration tool.
 Home-page: https://github.com/Animatea/mongorunway
 License: MIT
 Keywords: migration,mongodb,mongo,mongorunway
 Author: Animatea
 Author-email: animatea.programming@gmail.com
 Requires-Python: >=3.9,<4.0
```

