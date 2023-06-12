# Comparing `tmp/databudgie-2.8.1.tar.gz` & `tmp/databudgie-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databudgie-2.8.1.tar", max compression
+gzip compressed data, was "databudgie-2.8.2.tar", max compression
```

## Comparing `databudgie-2.8.1.tar` & `databudgie-2.8.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     5139 2023-06-08 20:35:22.217064 databudgie-2.8.1/CHANGELOG.md
--rw-r--r--   0        0        0     1973 2023-06-08 20:35:22.217064 databudgie-2.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1053 2023-06-08 20:35:22.217064 databudgie-2.8.1/LICENSE
--rw-r--r--   0        0        0     1310 2023-06-08 20:35:22.217064 databudgie-2.8.1/README.md
--rw-r--r--   0        0        0     2883 2023-06-08 20:35:22.221064 databudgie-2.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/__init__.py
--rw-r--r--   0        0        0       69 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/__main__.py
--rw-r--r--   0        0        0       74 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/adapter/__init__.py
--rw-r--r--   0        0        0     7162 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/adapter/base.py
--rw-r--r--   0        0        0    10638 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/adapter/postgres.py
--rw-r--r--   0        0        0     7361 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/backup.py
--rw-r--r--   0        0        0      105 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/cli/__init__.py
--rw-r--r--   0        0        0     2896 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/cli/base.py
--rw-r--r--   0        0        0     6733 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/cli/commands.py
--rw-r--r--   0        0        0     4696 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/cli/config.py
--rw-r--r--   0        0        0     1112 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/compression.py
--rw-r--r--   0        0        0    11307 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/config.py
--rw-r--r--   0        0        0      105 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/manifest/__init__.py
--rw-r--r--   0        0        0     2348 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/manifest/manager.py
--rw-r--r--   0        0        0     1602 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/manifest/sqlalchemy.py
--rw-r--r--   0        0        0      565 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/match.py
--rw-r--r--   0        0        0     1564 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/output.py
--rw-r--r--   0        0        0        0 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/py.typed
--rw-r--r--   0        0        0     8408 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/restore.py
--rw-r--r--   0        0        0     1948 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/s3.py
--rw-r--r--   0        0        0    11806 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/storage.py
--rw-r--r--   0        0        0     4586 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/table_op.py
--rw-r--r--   0        0        0     2462 2023-06-08 20:35:22.225065 databudgie-2.8.1/src/databudgie/utils.py
--rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 databudgie-2.8.1/setup.py
--rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 databudgie-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0     5139 2023-06-12 14:36:28.294923 databudgie-2.8.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1973 2023-06-12 14:36:28.294923 databudgie-2.8.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1053 2023-06-12 14:36:28.294923 databudgie-2.8.2/LICENSE
+-rw-r--r--   0        0        0     1310 2023-06-12 14:36:28.294923 databudgie-2.8.2/README.md
+-rw-r--r--   0        0        0     2883 2023-06-12 14:36:28.298923 databudgie-2.8.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/__init__.py
+-rw-r--r--   0        0        0       69 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/__main__.py
+-rw-r--r--   0        0        0       74 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/adapter/__init__.py
+-rw-r--r--   0        0        0     7162 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/adapter/base.py
+-rw-r--r--   0        0        0    10638 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/adapter/postgres.py
+-rw-r--r--   0        0        0     7361 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/backup.py
+-rw-r--r--   0        0        0      105 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/cli/__init__.py
+-rw-r--r--   0        0        0     3071 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/cli/base.py
+-rw-r--r--   0        0        0     6728 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/cli/commands.py
+-rw-r--r--   0        0        0     4730 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/cli/config.py
+-rw-r--r--   0        0        0     1112 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/compression.py
+-rw-r--r--   0        0        0    11753 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/config.py
+-rw-r--r--   0        0        0      105 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/manifest/__init__.py
+-rw-r--r--   0        0        0     2348 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/manifest/manager.py
+-rw-r--r--   0        0        0     1602 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/manifest/sqlalchemy.py
+-rw-r--r--   0        0        0      565 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/match.py
+-rw-r--r--   0        0        0     1564 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/output.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/py.typed
+-rw-r--r--   0        0        0     8408 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/restore.py
+-rw-r--r--   0        0        0     1948 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/s3.py
+-rw-r--r--   0        0        0    11806 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/storage.py
+-rw-r--r--   0        0        0     4586 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/table_op.py
+-rw-r--r--   0        0        0     2462 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/utils.py
+-rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 databudgie-2.8.2/setup.py
+-rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 databudgie-2.8.2/PKG-INFO
```

### Comparing `databudgie-2.8.1/CHANGELOG.md` & `databudgie-2.8.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/CONTRIBUTING.md` & `databudgie-2.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/LICENSE` & `databudgie-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/README.md` & `databudgie-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/pyproject.toml` & `databudgie-2.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databudgie"
-version = "2.8.1"
+version = "2.8.2"
 packages = [
     { include = "databudgie", from = "src" },
 ]
 
 authors = [
   "Andrew Sosa <andrewso@known.is>",
   "Dan Cardin <ddcardin@gmail.com>",
```

### Comparing `databudgie-2.8.1/src/databudgie/adapter/base.py` & `databudgie-2.8.2/src/databudgie/adapter/base.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/adapter/postgres.py` & `databudgie-2.8.2/src/databudgie/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/backup.py` & `databudgie-2.8.2/src/databudgie/backup.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/cli/base.py` & `databudgie-2.8.2/src/databudgie/cli/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-from typing import Callable, Optional, Union
+from __future__ import annotations
+
+from typing import Callable
 
 import click
 import sqlalchemy
 import sqlalchemy.engine.url
 import sqlalchemy.orm
 import strapp.click
 
-from databudgie.config import BackupConfig, RestoreConfig, RootConfig
+from databudgie.config import BackupConfig, Connection, RestoreConfig, RootConfig
 from databudgie.output import Console
 
 version = getattr(sqlalchemy, "__version__", "")
 
 URLType = Callable[..., sqlalchemy.engine.url.URL]
 
 if version.startswith("1.4") or version.startswith("2."):
     create_url: URLType = sqlalchemy.engine.url.URL.create
 else:
     create_url = sqlalchemy.engine.url.URL
 
 
-def _create_postgres_session(config: Union[BackupConfig, RestoreConfig], connection_name: Optional[str] = None):
-    if connection_name:
-        connection = config.connections.get(connection_name)
-        if connection is None:
-            raise click.UsageError(f"Connection '{connection_name}' not found")
-    else:
-        connection = config.connection
-        if connection is None:
-            raise click.UsageError("No config found for 'url' field. Either a 'connection' or a 'url' is required")
+def _create_postgres_session(config: BackupConfig | RestoreConfig):
+    connection: str | Connection = config.connection
+    if isinstance(config.connection, str):
+        if config.connection in config.connections:
+            # `connection` can either be a connection's name, or a literal connection string. We need
+            # to only overwrite the `connection` value if there is a correspondingly named connection
+            connection = config.connections[config.connection]
+        else:
+            raise click.UsageError(
+                f"'{config.connection}' did not resolve to a connection. 'url' or 'connection' must "
+                "resolve to a named connection or connection details."
+            )
 
+    assert isinstance(connection, Connection)
     url = connection.url
+
     if isinstance(url, dict):
         url_obj = create_url(**url)
     else:
         url_obj = sqlalchemy.engine.url.make_url(url)
 
     engine = sqlalchemy.create_engine(url_obj)
     return sqlalchemy.orm.scoping.scoped_session(sqlalchemy.orm.session.sessionmaker(bind=engine))()
@@ -47,35 +54,35 @@
 
 def restore_config(root_config: RootConfig, console: Console):
     if not root_config.restore:
         raise click.UsageError("No restore config found. Run 'databudgie config' to see your current configuration.")
     return root_config.restore
 
 
-def backup_db(backup_config: BackupConfig, connection_name: Optional[str] = None):
-    return _create_postgres_session(backup_config, connection_name)
+def backup_db(backup_config: BackupConfig):
+    return _create_postgres_session(backup_config)
 
 
-def restore_db(restore_config: RestoreConfig, connection_name: Optional[str] = None):
-    return _create_postgres_session(restore_config, connection_name)
+def restore_db(restore_config: RestoreConfig):
+    return _create_postgres_session(restore_config)
 
 
 def backup_manifest(backup_config: BackupConfig, backup_db):
     from databudgie.manifest.manager import BackupManifest
 
-    table_name: Optional[str] = backup_config.manifest
+    table_name: str | None = backup_config.manifest
     if table_name:
         return BackupManifest(backup_db, table_name)
     return None
 
 
 def restore_manifest(restore_config: RestoreConfig, restore_db):
     from databudgie.manifest.manager import RestoreManifest
 
-    table_name: Optional[str] = restore_config.manifest
+    table_name: str | None = restore_config.manifest
     if table_name:
         return RestoreManifest(restore_db, table_name)
     return None
 
 
 resolver = strapp.click.Resolver(
     backup_config=backup_config,
```

### Comparing `databudgie-2.8.1/src/databudgie/cli/commands.py` & `databudgie-2.8.2/src/databudgie/cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
         ddl=ddl,
         tables=list(table) if table else None,
         exclude=list(exclude) if exclude else None,
         url=url,
         location=location,
         adapter=adapter,
         strict=strict,
+        connection=conn,
     )
 
     try:
         root_config = collect_config(
             cli_config=cli_config,
             file_names=config,
             raw_config=raw_config,
@@ -127,15 +128,14 @@
     except ConfigError as e:
         raise click.UsageError(*e.args)
 
     resolver.register_values(
         root_config=root_config,
         verbosity=verbose,
         console=Console(verbosity=verbose),
-        connection_name=conn,
         dry_run=bool(dry_run),
         stats=stats if stats is not None else dry_run,
     )
 
 
 @resolver.command(cli, "backup")
 @click.option("--backup-id", default=None, help="Backup manifest id.")
```

### Comparing `databudgie-2.8.1/src/databudgie/cli/config.py` & `databudgie-2.8.2/src/databudgie/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     tables: list[str] | None = None
     exclude: list[str] | None = None
     ddl: bool | None = None
     url: str | dict | None = None
     location: str | None = None
     adapter: str | None = None
     strict: bool | None = None
+    connection: str | None = None
 
     def to_dict(self) -> dict:
         config = asdict(self)
         return {k: v for k, v in config.items() if v is not None}
 
 
 def collect_config(
```

### Comparing `databudgie-2.8.1/src/databudgie/compression.py` & `databudgie-2.8.2/src/databudgie/compression.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/config.py` & `databudgie-2.8.2/src/databudgie/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,32 +124,32 @@
         restore = RestoreConfig.from_stack(stack.push(restore_config))
         return cls(backup=backup, restore=restore)
 
 
 @dataclass
 class TableParentConfig(typing.Generic[T], Config):
     tables: list[T]
-    connections: dict[str, Connection]
+    connections: dict[str, Connection | str]
     ddl: DDLConfig
 
-    connection: Connection | None = None
+    connection: Connection | str = "default"
     manifest: str | None = None
 
     s3: S3Config | None = None
     root_location: str | None = None
     adapter: str | None = None
 
     @classmethod
     @abc.abstractmethod
     def get_child_class(cls):
         pass
 
     @classmethod
     def from_stack(cls, stack: ConfigStack):
-        connection = Connection.from_raw(stack.get("url") or stack.get("connection"), name="default")
+        connection = Connection.from_raw(stack.get("url") or stack.get("connection"), name="default") or "default"
         root_location = stack.get("root_location")
 
         tables_config: list = normalize_table_config(stack.get("tables", []))
         table_class = cls.get_child_class()
         tables = [table_class.from_stack(stack.push(tbl_conf), root_location) for tbl_conf in tables_config]
 
         # manifest defauls to None
@@ -178,19 +178,22 @@
 
 @dataclass
 class Connection(Config):
     name: str
     url: str | dict
 
     @classmethod
-    def from_raw(cls, raw: str | dict | None, *, name: str | None = None):
+    def from_raw(cls, raw: str | dict | None, *, name: str | None = None) -> Connection | str | None:
         if raw is None:
             return None
 
         if isinstance(raw, str):
+            if "://" not in raw:
+                return raw
+
             if name is None:
                 raise ConfigError(f"Connection '{raw}' requires a name")
             return cls(name="default", url=raw)
 
         if name is None:
             raise ConfigError(f"Connection '{raw}' requires a name")
 
@@ -198,33 +201,41 @@
             url = raw["url"]
         else:
             url = {k: v for k, v in raw.items() if k != "name"}
 
         return cls(name=name or "default", url=url)
 
     @classmethod
-    def from_collection(cls, collection: list | dict | None) -> dict[str, Connection]:
+    def from_collection(cls, collection: list | dict | None) -> dict[str, Connection | str]:
         if collection is None:
             return {}
 
         if isinstance(collection, list):
             connections = []
             names = set()
             for c in collection:
                 connection = Connection.from_raw(c, name=c.get("name"))
-                assert connection is not None
+                if not isinstance(connection, Connection):
+                    raise ConfigError(
+                        "Connections must be a database connection string or a mapping of individual connection fields."
+                    )
 
                 if connection.name in names:
                     raise ConfigError(f"Detected more than one connection with the same name: {connection.name}")
                 names.add(connection.name)
                 connections.append(connection)
 
             return {c.name: c for c in connections}
 
-        return {k: Connection.from_raw(c, name=k) for k, c in collection.items()}
+        result = {}
+        for k, c in collection.items():
+            connection = Connection.from_raw(c, name=k)
+            if connection is not None:
+                result[k] = connection
+        return result
 
 
 @dataclass
 class BackupTableConfig(Config):
     name: str
     location: str = "backups/{table}"
     query: str = "select * from {table}"
```

### Comparing `databudgie-2.8.1/src/databudgie/manifest/manager.py` & `databudgie-2.8.2/src/databudgie/manifest/manager.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/manifest/sqlalchemy.py` & `databudgie-2.8.2/src/databudgie/manifest/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/match.py` & `databudgie-2.8.2/src/databudgie/match.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/output.py` & `databudgie-2.8.2/src/databudgie/output.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/restore.py` & `databudgie-2.8.2/src/databudgie/restore.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/s3.py` & `databudgie-2.8.2/src/databudgie/s3.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/storage.py` & `databudgie-2.8.2/src/databudgie/storage.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/table_op.py` & `databudgie-2.8.2/src/databudgie/table_op.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/src/databudgie/utils.py` & `databudgie-2.8.2/src/databudgie/utils.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.1/setup.py` & `databudgie-2.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  's3': ['boto3']}
 
 entry_points = \
 {'console_scripts': ['databudgie = databudgie.__main__:run']}
 
 setup_kwargs = {
     'name': 'databudgie',
-    'version': '2.8.1',
+    'version': '2.8.2',
     'description': 'Ergonomic and flexible tool for database backup and restore',
     'long_description': '# Databudgie\n\n![Github Actions Build](https://github.com/schireson/databudgie/actions/workflows/build.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/schireson/databudgie/badge.svg?branch=main&t=6I0aU6)](https://coveralls.io/github/schireson/databudgie?branch=main)\n[![Documentation\nStatus](https://readthedocs.org/projects/databudgie/badge/?version=latest)](https://databudgie.readthedocs.io)\n\n![](docs/source/_static/databudgie.png)\n\nDatabudgie is a CLI & library for database performing targeted backup and\nrestore of database tables or arbitrary queries against database tables.\n\n# Usage\n\nA minimal config file might look like:\n\n```yaml\n# databudgie.yml or config.databudgie.yml\nbackup:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      query: "select * from {table} where store_id > 4"\n      location: s3://my-s3-bucket/databudgie/public.product\nrestore:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      location: s3://my-s3-bucket/databudgie/public.product\n```\n\nWith that config in place, backing up the defined tables (using the specified\nconfig) is as simple as `databudgie backup`; and restore `databudgie restore`.\n\n## Installation\n\n```bash\npip install databudgie\n```\n',
     'author': 'Andrew Sosa',
     'author_email': 'andrewso@known.is',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/databudgie',
```

### Comparing `databudgie-2.8.1/PKG-INFO` & `databudgie-2.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databudgie
-Version: 2.8.1
+Version: 2.8.2
 Summary: Ergonomic and flexible tool for database backup and restore
 Home-page: https://github.com/schireson/databudgie
 License: MIT
 Keywords: sqlalchemy,postgres,database,etl,s3
 Author: Andrew Sosa
 Author-email: andrewso@known.is
 Requires-Python: >=3.7,<4
```

