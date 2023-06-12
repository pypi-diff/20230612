# Comparing `tmp/phidata-1.6.9.tar.gz` & `tmp/phidata-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-1.6.9.tar", last modified: Tue May 23 01:53:19 2023, max compression
+gzip compressed data, was "phidata-1.7.0.tar", last modified: Mon Jun 12 21:23:33 2023, max compression
```

## Comparing `phidata-1.6.9.tar` & `phidata-1.7.0.tar`

### file list

```diff
@@ -1,513 +1,527 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.962381 phidata-1.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-23 01:52:54.000000 phidata-1.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-23 01:53:19.962381 phidata-1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-23 01:52:54.000000 phidata-1.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.870379 phidata-1.6.9/phidata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.870379 phidata-1.6.9/phidata/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.874379 phidata-1.6.9/phidata/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.874379 phidata-1.6.9/phidata/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.874379 phidata-1.6.9/phidata/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.874379 phidata-1.6.9/phidata/app/alertmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/amundsen/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/amundsen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/amundsen/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/amundsen/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/amundsen/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/assistant/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/cadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/databox/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/databox/databox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/db/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/db/base_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/django/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/django/django_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18443 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/grafana/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/k8s/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/k8s/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/k8s/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/nodeexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    37973 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/phidata_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/redis/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/redis/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/server/api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58714 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/server/server_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.890380 phidata-1.6.9/phidata/app/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/spark/spark_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.890380 phidata-1.6.9/phidata/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.890380 phidata-1.6.9/phidata/app/superset/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/asset/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/data_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/asset/local/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/local/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/create/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/create/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/resource/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.902380 phidata-1.6.9/phidata/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.902380 phidata-1.6.9/phidata/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.902380 phidata-1.6.9/phidata/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/iam/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/checks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/checks/not_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/decorators/validate_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.914380 phidata-1.6.9/phidata/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.914380 phidata-1.6.9/phidata/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.918380 phidata-1.6.9/phidata/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.918380 phidata-1.6.9/phidata/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/exceptions/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/exceptions/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/exceptions/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.918380 phidata-1.6.9/phidata/infra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.934381 phidata-1.6.9/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.934381 phidata-1.6.9/phidata/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/utils/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/llm/duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/product/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/product/data_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/table/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/local/local_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/local/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/table/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/s3/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/s3/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/table/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/sql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/aws/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/aws/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/download/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/download/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/url/to_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/url/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/plot/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/plot/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/python_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/run/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/run/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/run/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/task_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/upload/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/upload/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.954381 phidata-1.6.9/phidata/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/phidata_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.958381 phidata-1.6.9/phidata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/prep_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/workspace_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.958381 phidata-1.6.9/phidata/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.962381 phidata-1.6.9/phidata/workflow/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.962381 phidata-1.6.9/phidata/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.870379 phidata-1.6.9/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-23 01:52:54.000000 phidata-1.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:53:19.962381 phidata-1.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 01:52:54.000000 phidata-1.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.962381 phidata-1.6.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 01:52:54.000000 phidata-1.6.9/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.288650 phidata-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-12 21:23:12.000000 phidata-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-12 21:23:33.288650 phidata-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-12 21:23:12.000000 phidata-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.244650 phidata-1.7.0/phidata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.244650 phidata-1.7.0/phidata/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.244650 phidata-1.7.0/phidata/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.244650 phidata-1.7.0/phidata/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.244650 phidata-1.7.0/phidata/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.244650 phidata-1.7.0/phidata/app/alertmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.244650 phidata-1.7.0/phidata/app/amundsen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/amundsen/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20467 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/aws_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/base_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/cadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/databox/databox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/db/base_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/django/django_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/docker_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20089 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/fastapi/fastapi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/grafana/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/jupyter/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/k8s/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/k8s/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/k8s/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37744 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.248650 phidata-1.7.0/phidata/app/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/app/nodeexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/phidata_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/app/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/redis/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/redis/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/server/api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58714 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/server/server_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/app/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/spark/spark_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/streamlit/streamlit_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/superset/superset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/superset/superset_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.252650 phidata-1.7.0/phidata/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/asset/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/asset/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24787 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/asset/data_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/asset/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/asset/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/asset/local/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/create/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/create/iam/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/resource/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.256650 phidata-1.7.0/phidata/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20513 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ec2/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.260650 phidata-1.7.0/phidata/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.260650 phidata-1.7.0/phidata/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.260650 phidata-1.7.0/phidata/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.260650 phidata-1.7.0/phidata/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.260650 phidata-1.7.0/phidata/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.260650 phidata-1.7.0/phidata/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.260650 phidata-1.7.0/phidata/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.260650 phidata-1.7.0/phidata/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36056 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34552 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.260650 phidata-1.7.0/phidata/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.264650 phidata-1.7.0/phidata/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/secret/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.264650 phidata-1.7.0/phidata/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/s3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/s3/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22470 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/aws/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.264650 phidata-1.7.0/phidata/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/checks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/checks/not_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.264650 phidata-1.7.0/phidata/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/decorators/validate_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.264650 phidata-1.7.0/phidata/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.264650 phidata-1.7.0/phidata/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14274 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/resource/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/resource/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.264650 phidata-1.7.0/phidata/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.264650 phidata-1.7.0/phidata/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/exceptions/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/exceptions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/exceptions/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/infra/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/infra/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/infra/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/infra/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.268650 phidata-1.7.0/phidata/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.272650 phidata-1.7.0/phidata/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.276650 phidata-1.7.0/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/k8s/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/utils/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/k8s/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/llm/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/llm/duckdb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/product/data_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/resource/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/table/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/local/local_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/local/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/table/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/s3/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/s3/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/sql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/task/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.280650 phidata-1.7.0/phidata/task/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/aws/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/aws/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/download/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/download/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/download/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/download/url/to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/plot/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/plot/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/python_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/run/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/run/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/task_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/task/upload/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.284650 phidata-1.7.0/phidata/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/types/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/types/phidata_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.288650 phidata-1.7.0/phidata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/get_python_objects_from_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/workspace_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/utils/yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.288650 phidata-1.7.0/phidata/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/workflow/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.288650 phidata-1.7.0/phidata/workflow/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.288650 phidata-1.7.0/phidata/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-12 21:23:12.000000 phidata-1.7.0/phidata/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.244650 phidata-1.7.0/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-12 21:23:33.000000 phidata-1.7.0/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-06-12 21:23:33.000000 phidata-1.7.0/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:23:33.000000 phidata-1.7.0/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-12 21:23:33.000000 phidata-1.7.0/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 21:23:33.000000 phidata-1.7.0/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-12 21:23:12.000000 phidata-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:23:33.288650 phidata-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 21:23:12.000000 phidata-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:33.288650 phidata-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 21:23:12.000000 phidata-1.7.0/tests/test_placeholder.py
```

### Comparing `phidata-1.6.9/LICENSE` & `phidata-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/airflow/operators/empty.py` & `phidata-1.7.0/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/app/airflow/airflow_base.py` & `phidata-1.7.0/phidata/app/airflow/airflow_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,20 +341,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
```

### Comparing `phidata-1.6.9/phidata/app/airflow/airflow_flower.py` & `phidata-1.7.0/phidata/app/airflow/airflow_flower.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,20 +108,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
```

### Comparing `phidata-1.6.9/phidata/app/airflow/airflow_manager.py` & `phidata-1.7.0/phidata/app/airflow/airflow_webserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 from phidata.app.airflow.airflow_base import (
     AirflowBase,
     AirflowLogsVolumeType,
     ServiceType,
     DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
+    RestartPolicy,
 )
 
 
-class AirflowManager(AirflowBase):
+class AirflowWebserver(AirflowBase):
     def __init__(
         self,
-        name: str = "airflow-manager",
+        name: str = "airflow-ws",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/airflow",
         image_tag: str = "2.5.0",
-        entrypoint: Optional[Union[str, List]] = "/scripts/manager",
-        command: Optional[Union[str, List]] = None,
+        entrypoint: Optional[Union[str, List]] = None,
+        command: Optional[Union[str, List]] = "webserver",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Airflow Configuration,
         # The AIRFLOW_ENV defines the current airflow runtime and can be used by,
         # DAGs to separate dev/stg/prd code,
@@ -108,35 +109,35 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
         # Port number on the container,
         container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
         container_host_port: int = 8000,
         # Open the webserver port if open_webserver_port=True,
-        open_webserver_port: bool = False,
+        open_webserver_port: bool = True,
         # Webserver port number on the container,
         webserver_port: int = 8080,
         # Port name: Only used by the K8sContainer,
         webserver_port_name: str = "webserver",
         # Host port: Only used by the DockerContainer,
         webserver_host_port: int = 8080,
         # Open the worker_log_port if open_worker_log_port=True,
@@ -305,15 +306,15 @@
         # If ServiceType == ServiceType.LoadBalancer,
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
-        create_webserver_service: bool = False,
+        create_webserver_service: bool = True,
         # Configure the webserver service,
         ws_svc_name: Optional[str] = None,
         ws_svc_type: Optional[ServiceType] = None,
         # The port exposed by the webserver service.,
         ws_svc_port: int = 8080,
         # The node_port exposed by the service if ws_svc_type = ServiceType.NODE_PORT,
         ws_node_port: Optional[int] = None,
```

### Comparing `phidata-1.6.9/phidata/app/airflow/airflow_scheduler.py` & `phidata-1.7.0/phidata/app/airflow/airflow_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,20 +108,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
```

### Comparing `phidata-1.6.9/phidata/app/airflow/airflow_webserver.py` & `phidata-1.7.0/phidata/app/airflow/airflow_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,30 @@
 from phidata.app.airflow.airflow_base import (
     AirflowBase,
     AirflowLogsVolumeType,
     ServiceType,
     DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
-    RestartPolicy,
 )
 
 
-class AirflowWebserver(AirflowBase):
+class AirflowManager(AirflowBase):
     def __init__(
         self,
-        name: str = "airflow-ws",
+        name: str = "airflow-manager",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/airflow",
         image_tag: str = "2.5.0",
-        entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "webserver",
+        entrypoint: Optional[Union[str, List]] = "/scripts/manager",
+        command: Optional[Union[str, List]] = None,
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Airflow Configuration,
         # The AIRFLOW_ENV defines the current airflow runtime and can be used by,
         # DAGs to separate dev/stg/prd code,
@@ -109,35 +108,35 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
         # Port number on the container,
         container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
         container_host_port: int = 8000,
         # Open the webserver port if open_webserver_port=True,
-        open_webserver_port: bool = True,
+        open_webserver_port: bool = False,
         # Webserver port number on the container,
         webserver_port: int = 8080,
         # Port name: Only used by the K8sContainer,
         webserver_port_name: str = "webserver",
         # Host port: Only used by the DockerContainer,
         webserver_host_port: int = 8080,
         # Open the worker_log_port if open_worker_log_port=True,
@@ -306,15 +305,15 @@
         # If ServiceType == ServiceType.LoadBalancer,
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
-        create_webserver_service: bool = True,
+        create_webserver_service: bool = False,
         # Configure the webserver service,
         ws_svc_name: Optional[str] = None,
         ws_svc_type: Optional[ServiceType] = None,
         # The port exposed by the webserver service.,
         ws_svc_port: int = 8080,
         # The node_port exposed by the service if ws_svc_type = ServiceType.NODE_PORT,
         ws_node_port: Optional[int] = None,
```

### Comparing `phidata-1.6.9/phidata/app/airflow/airflow_worker.py` & `phidata-1.7.0/phidata/app/airflow/airflow_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,20 +110,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
```

### Comparing `phidata-1.6.9/phidata/app/alertmanager/alertmanager.py` & `phidata-1.7.0/phidata/app/alertmanager/alertmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/amundsen/frontend.py` & `phidata-1.7.0/phidata/app/amundsen/frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/amundsen/metadata.py` & `phidata-1.7.0/phidata/app/amundsen/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/amundsen/search.py` & `phidata-1.7.0/phidata/app/amundsen/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/assistant/assistant.py` & `phidata-1.7.0/phidata/app/assistant/assistant.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,20 +61,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/cadvisor/cadvisor.py` & `phidata-1.7.0/phidata/app/cadvisor/cadvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/databox/databox.py` & `phidata-1.7.0/phidata/app/databox/databox.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,20 +258,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Start airflow standalone,
         start_airflow_standalone: bool = False,
         # Open the airflow_standalone_container_port on the container,
```

### Comparing `phidata-1.6.9/phidata/app/db/base_db.py` & `phidata-1.7.0/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/app/django/django_app.py` & `phidata-1.7.0/phidata/app/django/django_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         # Add NGINX to serve static file
         enable_nginx: bool = False,
         nginx_image: Optional[Any] = None,
         nginx_image_name: str = "phidata/django-nginx",
         nginx_image_tag: str = "latest",
         # -*- AWS configuration
         aws_subnets: Optional[List[str]] = None,
-        aws_security_groups: Optional[List[str]] = None,
+        aws_security_groups: Optional[List[Any]] = None,
         # Other args,
         print_env_on_load: bool = False,
         skip_create: bool = False,
         skip_read: bool = False,
         skip_update: bool = False,
         recreate_on_update: bool = False,
         skip_delete: bool = False,
@@ -413,15 +413,15 @@
             TargetGroup,
             Listener,
             Subnet,
         )
         from phidata.types.context import ContainerPathContext
         from phidata.utils.common import get_default_volume_name
 
-        app_name = self.args.name
+        app_name = self.name
 
         if self.workspace_root_path is None:
             raise Exception("Invalid workspace_root_path")
         workspace_name = self.workspace_root_path.stem
 
         logger.debug(f"Building AwsResourceGroup: {app_name} for {workspace_name}")
```

### Comparing `phidata-1.6.9/phidata/app/elastic/elastic_app.py` & `phidata-1.7.0/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/app/elasticsearch/elasticsearch.py` & `phidata-1.7.0/phidata/app/elasticsearch/elasticsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,20 +54,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/fastapi/fastapi.py` & `phidata-1.7.0/phidata/app/server/api_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,28 @@
     ServiceType,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class FastApiServerArgs(ServerBaseArgs):
+class ApiServerArgs(ServerBaseArgs):
     pass
 
 
-class FastApiServer(ServerBase):
+class ApiServer(ServerBase):
     def __init__(
         self,
-        name: str = "fastapi-server",
+        name: str = "api-server",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/fastapi",
+        image_name: str = "phidata/server",
         image_tag: str = "latest",
         entrypoint: Optional[Union[str, List]] = None,
         command: Optional[Union[str, List]] = "api start",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
@@ -56,19 +56,19 @@
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 9090,
+        container_port: int = 80,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 9090,
+        container_host_port: int = 80,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
         # Path to mount the workspace volume inside the container,
         workspace_volume_container_path: str = "/usr/local/app",
@@ -162,15 +162,15 @@
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # K8s Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[ServiceType] = None,
         # The port exposed by the service.,
-        service_port: int = 9090,
+        service_port: int = 80,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
@@ -239,15 +239,15 @@
         ecs_launch_type: str = "FARGATE",
         ecs_task_cpu: str = "256",
         ecs_task_memory: str = "512",
         ecs_service_count: int = 1,
         assign_public_ip: bool = True,
         elb: Optional[Any] = None,
         aws_subnets: Optional[List[str]] = None,
-        aws_security_groups: Optional[List[str]] = None,
+        aws_security_groups: Optional[List[Any]] = None,
         # Other args,
         print_env_on_load: bool = False,
         skip_create: bool = False,
         skip_read: bool = False,
         skip_update: bool = False,
         recreate_on_update: bool = False,
         skip_delete: bool = False,
```

### Comparing `phidata-1.6.9/phidata/app/grafana/grafana.py` & `phidata-1.7.0/phidata/app/grafana/grafana.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,20 +56,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/group.py` & `phidata-1.7.0/phidata/app/group.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from typing import List, Optional
+from typing import List, Optional, Union
 
 from pydantic import BaseModel
 
+from phidata.app.base_app import BaseApp
 from phidata.app.phidata_app import PhidataApp
 
 
 class AppGroup(BaseModel):
     """
     The AppGroup is a collection of PhidataApps acting as a single unit.
     """
 
-    # Name
     name: Optional[str] = None
     enabled: bool = True
-    # Apps
-    apps: Optional[List[PhidataApp]] = None
+    apps: Optional[List[Union[BaseApp, PhidataApp]]] = None
 
     class Config:
         arbitrary_types_allowed = True
 
-    def get_apps(self) -> List[PhidataApp]:
+    def get_apps(self) -> List[Union[BaseApp, PhidataApp]]:
         if self.enabled and self.apps is not None:
             return self.apps
         return []
 
 
-def get_apps_from_app_groups(app_groups: List[AppGroup]) -> List[PhidataApp]:
+def get_apps_from_app_groups(
+    app_groups: List[AppGroup],
+) -> List[Union[BaseApp, PhidataApp]]:
     apps = []
     for app_group in app_groups:
         apps.extend(app_group.get_apps())
     return apps
```

### Comparing `phidata-1.6.9/phidata/app/jupyter/jupyter_hub.py` & `phidata-1.7.0/phidata/app/jupyter/jupyter_hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     app_port: int = 8000
     # Only used by the K8sContainer
     app_port_name: str = "app"
     # Only used by the DockerContainer
     app_host_port: int = 8000
 
     # Add env variables to container env
-    env: Optional[Dict[str, str]] = None
+    env: Optional[Dict[str, Any]] = None
     # Read env variables from a file in yaml format
     env_file: Optional[Path] = None
     # Configure the ConfigMap used for env variables that are not Secret
     config_map_name: Optional[str] = None
     # Configure the Secret used for env variables that are Secret
     secret_name: Optional[str] = None
     # Read secrets from a file in yaml format
```

### Comparing `phidata-1.6.9/phidata/app/jupyter/jupyter_lab.py` & `phidata-1.7.0/phidata/app/jupyter/jupyter_lab.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class JupyterLabArgs(PhidataAppArgs):
     name: str = "jupyter"
     version: str = "1"
     enabled: bool = True
 
     # -*- Image Configuration
     image_name: str = "phidata/jupyterlab"
-    image_tag: str = "3.4.8"
+    image_tag: str = "3.5.2"
     entrypoint: Optional[Union[str, List]] = None
     command: Union[str, List] = "jupyter lab"
 
     # -*- Jupyter Configuration
     # Absolute path to JUPYTER_CONFIG_FILE
     # Also used to set the JUPYTER_CONFIG_FILE env var
     # This value if provided is appended to the command using `--config`
@@ -208,15 +208,15 @@
         name: str = "jupyter",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/jupyterlab",
-        image_tag: str = "3.4.8",
+        image_tag: str = "3.5.2",
         entrypoint: Optional[Union[str, List]] = None,
         command: Union[str, List] = "jupyter lab",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Jupyter Configuration,
@@ -297,20 +297,20 @@
         # Overwrite the PYTHONPATH env var,
         # which is usually set to the workspace_root_container_path,
         python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
```

### Comparing `phidata-1.6.9/phidata/app/k8s/app.py` & `phidata-1.7.0/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/app/k8s/dir.py` & `phidata-1.7.0/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/app/k8s/url.py` & `phidata-1.7.0/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/app/mysql/mysql_db.py` & `phidata-1.7.0/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/app/neo4j/neo4j.py` & `phidata-1.7.0/phidata/app/neo4j/neo4j.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,20 +52,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/nodeexporter/nodeexporter.py` & `phidata-1.7.0/phidata/app/nodeexporter/nodeexporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/phidata_app.py` & `phidata-1.7.0/phidata/app/phidata_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from phidata.utils.enums import ExtendedEnum
 from phidata.utils.log import logger
 
 
 class WorkspaceVolumeType(ExtendedEnum):
     HostPath = "HostPath"
     EmptyDir = "EmptyDir"
-    # PersistentVolume = "PersistentVolume"
     AwsEbs = "AwsEbs"
-    # AwsEfs = "AwsEfs"
+    AwsEfs = "AwsEfs"
+    PersistentVolume = "PersistentVolume"
 
 
 class PhidataAppArgs(PhidataBaseArgs):
-    name: str
+    name: Optional[str]
 
     # -*- Path parameters
     # The following args are populated by the K8sWorker and DockerWorker classes.
     # The build_resource_groups() function passes these args from the
     # WorkspaceConfig -> K8sConfig -> K8sArgs -> PhidataApp
 
     # Path to the workspace root directory
@@ -51,34 +51,28 @@
     # Image can be provided as a DockerImage object or as image_name:image_tag
     image: Optional[Any] = None
     image_name: Optional[str] = None
     image_tag: Optional[str] = None
     entrypoint: Optional[Union[str, List]] = None
     command: Optional[Union[str, List]] = None
 
+    # -*- Debug Mode
+    debug_mode: bool = False
+
+    # -*- Python Configuration
     # Install python dependencies using a requirements.txt file
     install_requirements: bool = False
     # Path to the requirements.txt file relative to the workspace_root
     requirements_file: str = "requirements.txt"
-
-    # -*- Debug Mode
-    debug_mode: bool = False
-
-    # -*- Container Configuration
-    # Each PhidataApp has 1 main container and multiple sidecar containers
-    # The main container name
-    container_name: Optional[str] = None
-    # Overwrite the PYTHONPATH env var, default: False
+    # Set the container PYTHONPATH
     set_python_path: bool = False
-    # Set the python_path, default: workspace_volume_container_path,
+    # Manually provide the PYTHONPATH. If None, defaults to the workspace_root
     python_path: Optional[str] = None
-    # Add to the PYTHONPATH env var. If python_path is set, this is ignored
+    # Add to the PYTHONPATH env var. If python_path is provided, this value is ignored
     add_python_path: Optional[str] = None
-    # Add labels to the container
-    container_labels: Optional[Dict[str, Any]] = None
 
     # Container env passed to the PhidataApp
     # Add env variables to container env
     env: Optional[Dict[str, Any]] = None
     # Read env variables from a file in yaml format
     env_file: Optional[Path] = None
 
@@ -86,53 +80,46 @@
     # Add secret variables to container env
     secrets: Optional[Dict[str, Any]] = None
     # Read secret variables from a file in yaml format
     secrets_file: Optional[Path] = None
     # Read secret variables from AWS Secrets
     aws_secrets: Optional[Any] = None
 
-    # Container ports
+    # -*- Container Ports
     # Open a container port if open_container_port=True
     open_container_port: bool = False
     # Port number on the container
     container_port: int = 8000
-    # Port name: Only used by the K8sContainer
+    # Port name
     container_port_name: str = "http"
-    # Host port: Only used by the DockerContainer
+    # Host port to map to the container port
     container_host_port: int = 8000
 
-    # Container volumes
+    # -*- Container Volumes
     # Mount the workspace directory on the container
     mount_workspace: bool = False
     workspace_volume_name: Optional[str] = None
     workspace_volume_type: Optional[WorkspaceVolumeType] = None
-    # Path to mount the workspace volume
-    # This is the parent directory for the workspace on the container
-    # i.e. the ws is mounted as a subdir in this dir
-    # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata
+    # Path to mount the workspace volume inside the container
     workspace_volume_container_path: str = "/mnt/workspaces"
-    # How to mount the workspace volume
-    # Option 1: Mount the workspace from the host machine
+    # Mount the workspace from the host machine
     # If None, use the workspace_root_path
-    # Note: This is the default on DockerContainers. We assume that DockerContainers
-    # are running locally on the user's machine so the local workspace_root_path
-    # is mounted to the workspace_volume_container_path
     workspace_volume_host_path: Optional[str] = None
-    # Option 2: Load the workspace from git using a git-sync sidecar container
-    # This the default on K8sContainers.
+    # Load the workspace from git using a git-sync sidecar container
     create_git_sync_sidecar: bool = False
     # Required to create an initial copy of the workspace
     create_git_sync_init_container: bool = True
     git_sync_image_name: str = "k8s.gcr.io/git-sync"
     git_sync_image_tag: str = "v3.1.1"
     git_sync_repo: Optional[str] = None
     git_sync_branch: Optional[str] = None
     git_sync_wait: int = 1
 
-    # -*- Docker configuration
+    # -*- Docker Configuration
+    container_name: Optional[str] = None
     # Run container in the background and return a Container object.
     container_detach: bool = True
     # Enable auto-removal of the container on daemon side when the container’s process exits.
     container_auto_remove: bool = True
     # Remove the container when it has finished running. Default: True.
     container_remove: bool = True
     # Username or UID to run commands as inside the container.
@@ -177,71 +164,68 @@
     #       For example, {'2222/tcp': 3333} will expose port 2222 inside the container as port 3333 on the host.
     #   - None, to assign a random host port. For example, {'2222/tcp': None}.
     #   - A tuple of (address, port) if you want to specify the host interface.
     #       For example, {'1111/tcp': ('127.0.0.1', 1111)}.
     #   - A list of integers, if you want to bind multiple host ports to a single container port.
     #       For example, {'1111/tcp': [1234, 4567]}.
     container_ports_docker: Optional[Dict[str, Any]] = None
+    # Add labels to the container
+    container_labels: Optional[Dict[str, Any]] = None
 
-    # -*- K8s configuration
-    # K8s Deployment configuration
+    # -*- K8s Deployment Configuration
     replicas: int = 1
     pod_name: Optional[str] = None
     deploy_name: Optional[str] = None
     secret_name: Optional[str] = None
     configmap_name: Optional[str] = None
     # Type: ImagePullPolicy
     image_pull_policy: Optional[Any] = None
     pod_annotations: Optional[Dict[str, str]] = None
     pod_node_selector: Optional[Dict[str, str]] = None
     # Type: RestartPolicy
     deploy_restart_policy: Optional[Any] = None
     deploy_labels: Optional[Dict[str, Any]] = None
     termination_grace_period_seconds: Optional[int] = None
-    # How to spread the deployment across a topology
-    # Key to spread the pods across
+    # Key to spread the pods across a topology
     topology_spread_key: Optional[str] = None
     # The degree to which pods may be unevenly distributed
     topology_spread_max_skew: Optional[int] = None
     # How to deal with a pod if it doesn't satisfy the spread constraint.
     topology_spread_when_unsatisfiable: Optional[str] = None
 
-    # K8s Service Configuration
+    # -*- K8s Service Configuration
     create_service: bool = False
     service_name: Optional[str] = None
     # Type: ServiceType
     service_type: Optional[Any] = None
     # The port exposed by the service.
     service_port: int = 8000
     # The node_port exposed by the service if service_type = ServiceType.NODE_PORT
     service_node_port: Optional[int] = None
     # The target_port is the port to access on the pods targeted by the service.
     # It can be the port number or port name on the pod.
     service_target_port: Optional[Union[str, int]] = None
     # Extra ports exposed by the webserver service. Type: List[CreatePort]
     service_ports: Optional[List[Any]] = None
-    # Service labels
     service_labels: Optional[Dict[str, Any]] = None
-    # Service annotations
     service_annotations: Optional[Dict[str, str]] = None
     # If ServiceType == ServiceType.LoadBalancer
     service_health_check_node_port: Optional[int] = None
     service_internal_traffic_policy: Optional[str] = None
     service_load_balancer_class: Optional[str] = None
     service_load_balancer_ip: Optional[str] = None
     service_load_balancer_source_ranges: Optional[List[str]] = None
     service_allocate_load_balancer_node_ports: Optional[bool] = None
 
-    # K8s Ingress Configuration
+    # -*- K8s Ingress Configuration
     create_ingress: bool = False
     ingress_name: Optional[str] = None
-    # Ingress annotations
     ingress_annotations: Optional[Dict[str, str]] = None
 
-    # K8s RBAC Configuration
+    # -*- K8s RBAC Configuration
     use_rbac: bool = False
     # Create a Namespace with name ns_name & default values
     ns_name: Optional[str] = None
     # or Provide the full Namespace definition
     # Type: CreateNamespace
     namespace: Optional[Any] = None
     # Create a ServiceAccount with name sa_name & default values
@@ -286,15 +270,15 @@
     # Type: CreateCustomObject
     extra_custom_objects: Optional[List[Any]] = None
     # Type: CreateCustomResourceDefinition
     extra_crds: Optional[List[Any]] = None
 
     # -*- AWS configuration
     aws_subnets: Optional[List[str]] = None
-    aws_security_groups: Optional[List[str]] = None
+    aws_security_groups: Optional[List[Any]] = None
 
     # Other args
     print_env_on_load: bool = False
     # If True, skip resource creation if active resources with the same name exist.
     use_cache: bool = True
 
     # Extra kwargs used to ensure older versions of phidata don't throw syntax errors
@@ -317,16 +301,16 @@
     def __init__(self) -> None:
         super().__init__()
 
         # Cache env_data & secret_data
         self.env_data: Optional[Dict[str, Any]] = None
         self.secret_data: Optional[Dict[str, Any]] = None
 
-        # Args for the PhidataApp, provided by the subclass
-        self.args: PhidataAppArgs
+        # Args for the PhidataApp, set by the subclass
+        self.args: PhidataAppArgs = PhidataAppArgs()
 
         # Dict of DockerResourceGroups
         # Type: Optional[Dict[str, DockerResourceGroup]]
         self.docker_resource_groups: Optional[Dict[str, Any]] = None
 
         # Dict of KubernetesResourceGroups
         # Type: Optional[Dict[str, K8sResourceGroup]]
@@ -484,74 +468,99 @@
             return f"{self.args.image_name}:latest"
         else:
             return None
 
     def get_container_name(self) -> str:
         from phidata.utils.common import get_default_container_name
 
-        return self.args.container_name or get_default_container_name(self.args.name)
+        return self.args.container_name or get_default_container_name(self.name)
 
     def get_container_port(self) -> int:
         return self.args.container_port
 
     def get_container_host_port(self) -> int:
         return self.args.container_host_port
 
     def get_pod_name(self) -> str:
         from phidata.utils.common import get_default_pod_name
 
-        return self.args.pod_name or get_default_pod_name(self.args.name)
+        return self.args.pod_name or get_default_pod_name(self.name)
 
     def get_deploy_name(self) -> str:
         from phidata.utils.common import get_default_deploy_name
 
-        return self.args.deploy_name or get_default_deploy_name(self.args.name)
+        return self.args.deploy_name or get_default_deploy_name(self.name)
 
     def get_secret_name(self) -> str:
         from phidata.utils.common import get_default_secret_name
 
-        return self.args.secret_name or get_default_secret_name(self.args.name)
+        return self.args.secret_name or get_default_secret_name(self.name)
 
     def get_configmap_name(self) -> str:
         from phidata.utils.common import get_default_configmap_name
 
-        return self.args.configmap_name or get_default_configmap_name(self.args.name)
+        return self.args.configmap_name or get_default_configmap_name(self.name)
 
     def get_service_name(self) -> str:
         from phidata.utils.common import get_default_service_name
 
-        return self.args.service_name or get_default_service_name(self.args.name)
+        return self.args.service_name or get_default_service_name(self.name)
 
     def get_service_port(self) -> int:
         return self.args.service_port
 
     def get_sa_name(self) -> str:
         from phidata.utils.common import get_default_sa_name
 
-        return self.args.sa_name or get_default_sa_name(self.args.name)
+        return self.args.sa_name or get_default_sa_name(self.name)
 
     def get_cr_name(self) -> str:
         from phidata.utils.common import get_default_cr_name
 
-        return self.args.cr_name or get_default_cr_name(self.args.name)
+        return self.args.cr_name or get_default_cr_name(self.name)
 
     def get_crb_name(self) -> str:
         from phidata.utils.common import get_default_crb_name
 
-        return self.args.crb_name or get_default_crb_name(self.args.name)
+        return self.args.crb_name or get_default_crb_name(self.name)
 
     def get_env_data(self) -> Optional[Dict[str, str]]:
         if self.env_data is None:
             self.env_data = self.read_yaml_file(file_path=self.args.env_file)
         return self.env_data
 
     def get_secret_data(self) -> Optional[Dict[str, str]]:
         if self.secret_data is None:
+            # Read from secrets_file
             self.secret_data = self.read_yaml_file(file_path=self.args.secrets_file)
-        # Read from aws_secrets
+
+            # Read from aws_secrets
+            if self.args.aws_secrets is not None:
+                from phidata.aws.resource.secret.manager import SecretsManager
+
+                aws_secrets: Dict[str, Any] = {}
+                if isinstance(self.args.aws_secrets, SecretsManager):
+                    _secret_dict = self.args.aws_secrets.get_secrets_as_dict()
+                    if _secret_dict is not None and isinstance(_secret_dict, dict):
+                        aws_secrets.update(_secret_dict)
+                elif isinstance(self.args.aws_secrets, list):
+                    for _aws_secret in self.args.aws_secrets:
+                        if isinstance(_aws_secret, SecretsManager):
+                            _secret_dict = _aws_secret.get_secrets_as_dict()
+                            if _secret_dict is not None and isinstance(
+                                _secret_dict, dict
+                            ):
+                                aws_secrets.update(_secret_dict)
+
+                if len(aws_secrets) > 0:
+                    if self.secret_data is None:
+                        self.secret_data = aws_secrets
+                    else:
+                        self.secret_data.update(aws_secrets)
+        # logger.debug(f"{self.name} secrets: {self.secret_data}")
         return self.secret_data
 
     def set_container_env(self, container_env: Dict[str, Any]) -> None:
         # Update the container env using env_file
         env_data_from_file = self.get_env_data()
         if env_data_from_file is not None:
             container_env.update(env_data_from_file)
@@ -807,21 +816,21 @@
 
     def get_aws_resource_groups(
         self, aws_build_context: Any
     ) -> Optional[Dict[str, Any]]:
         if self.aws_resource_groups is None:
             self.init_aws_resource_groups(aws_build_context)
         # Comment out in production
-        if self.aws_resource_groups:
-            logger.debug("AwsResourceGroups:")
-            for rg_name, rg in self.aws_resource_groups.items():
-                try:
-                    logger.debug("{}\n{}".format(rg_name, rg.json(indent=2)))
-                except Exception:
-                    pass
+        # if self.aws_resource_groups:
+        #     logger.debug("qAwsResourceGroups:")
+        #     for rg_name, rg in self.aws_resource_groups.items():
+        #         try:
+        #             logger.debug("{}\n{}".format(rg_name, rg.json(indent=2)))
+        #         except Exception:
+        #             pass
         return self.aws_resource_groups
 
     ######################################################
     ## Helpers
     ######################################################
 
     def get_container_paths(self, add_ws_name_to_ws_root: bool = True) -> Optional[Any]:
```

### Comparing `phidata-1.6.9/phidata/app/postgres/postgres_db.py` & `phidata-1.7.0/phidata/app/postgres/postgres_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,20 +120,20 @@
         postgres_initdb_args_file: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/prometheus/prometheus.py` & `phidata-1.7.0/phidata/app/prometheus/prometheus.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,20 +58,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/redis/redis.py` & `phidata-1.7.0/phidata/app/redis/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,20 +106,20 @@
         logging_level: str = "debug",
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/redis/stack.py` & `phidata-1.7.0/phidata/app/redis/stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,20 +127,20 @@
         redisbloom_args: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open the container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/server/api_server.py` & `phidata-1.7.0/phidata/app/spark/spark_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.server.server_base import (
-    ServerBase,
-    ServerBaseArgs,
+from phidata.app.spark.spark_base import (
+    SparkBase,
+    SparkBaseArgs,
     ServiceType,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class ApiServerArgs(ServerBaseArgs):
-    pass
-
-
-class ApiServer(ServerBase):
+class SparkWorker(SparkBase):
     def __init__(
         self,
-        name: str = "api-server",
+        name: str = "spark-worker",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/server",
-        image_tag: str = "latest",
+        image_name: str = "phidata/spark",
+        image_tag: str = "3.3.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "api start",
+        command: Optional[Union[str, List]] = "worker",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
-        # -*- Debug Mode
-        debug_mode: bool = False,
+        # -*- Spark Configuration
+        cores: Optional[int] = None,
+        memory: Optional[str] = None,
+        driver_url: Optional[str] = None,
+        properties_file: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Overwrite the PYTHONPATH env var,
         # which is usually set to the workspace_root_container_path,
         python_path: Optional[str] = None,
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
@@ -56,26 +55,29 @@
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 80,
+        container_port: int = 8080,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 80,
+        container_host_port: int = 8080,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume inside the container,
-        workspace_volume_container_path: str = "/usr/local/app",
+        # Path to mount the workspace volume,
+        # This is the parent directory for the workspace on the container,
+        # i.e. the ws is mounted as a subdir in this dir,
+        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
+        workspace_volume_container_path: str = "/mnt/workspaces",
         # How to mount the workspace volume,
         # Option 1: Mount the workspace from the host machine,
         # If None, use the workspace_root_path,
         # Note: This is the default on DockerContainers. We assume that DockerContainers,
         # are running locally on the user's machine so the local workspace_root_path,
         # is mounted to the workspace_volume_container_path,
         workspace_volume_host_path: Optional[str] = None,
@@ -162,15 +164,15 @@
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # K8s Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[ServiceType] = None,
         # The port exposed by the service.,
-        service_port: int = 80,
+        service_port: int = 8000,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
@@ -230,52 +232,38 @@
         extra_volumes: Optional[List[Any]] = None,
         # Type: CreateStorageClass,
         extra_storage_classes: Optional[List[Any]] = None,
         # Type: CreateCustomObject,
         extra_custom_objects: Optional[List[Any]] = None,
         # Type: CreateCustomResourceDefinition,
         extra_crds: Optional[List[Any]] = None,
-        # -*- AWS configuration,
-        ecs_cluster: Optional[Any] = None,
-        ecs_launch_type: str = "FARGATE",
-        ecs_task_cpu: str = "256",
-        ecs_task_memory: str = "512",
-        ecs_service_count: int = 1,
-        assign_public_ip: bool = True,
-        elb: Optional[Any] = None,
-        aws_subnets: Optional[List[str]] = None,
-        aws_security_groups: Optional[List[str]] = None,
         # Other args,
-        print_env_on_load: bool = False,
-        skip_create: bool = False,
-        skip_read: bool = False,
-        skip_update: bool = False,
-        recreate_on_update: bool = False,
-        skip_delete: bool = False,
-        wait_for_creation: bool = True,
-        wait_for_update: bool = True,
-        wait_for_deletion: bool = True,
-        waiter_delay: int = 30,
-        waiter_max_attempts: int = 50,
+        print_env_on_load: bool = True,
         # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
         **kwargs,
     ):
+        if driver_url is None:
+            raise ValueError("driver_url is required for SparkWorker")
+
         super().__init__(
             name=name,
             version=version,
             enabled=enabled,
             image=image,
             image_name=image_name,
             image_tag=image_tag,
             entrypoint=entrypoint,
             command=command,
             install_requirements=install_requirements,
             requirements_file=requirements_file,
-            debug_mode=debug_mode,
+            cores=cores,
+            memory=memory,
+            driver_url=driver_url,
+            properties_file=properties_file,
             container_name=container_name,
             python_path=python_path,
             add_python_path=add_python_path,
             container_labels=container_labels,
             env=env,
             env_file=env_file,
             secrets=secrets,
@@ -357,30 +345,11 @@
             extra_containers=extra_containers,
             extra_init_containers=extra_init_containers,
             extra_ports=extra_ports,
             extra_volumes=extra_volumes,
             extra_storage_classes=extra_storage_classes,
             extra_custom_objects=extra_custom_objects,
             extra_crds=extra_crds,
-            ecs_cluster=ecs_cluster,
-            ecs_launch_type=ecs_launch_type,
-            ecs_task_cpu=ecs_task_cpu,
-            ecs_task_memory=ecs_task_memory,
-            ecs_service_count=ecs_service_count,
-            assign_public_ip=assign_public_ip,
-            elb=elb,
-            aws_subnets=aws_subnets,
-            aws_security_groups=aws_security_groups,
             print_env_on_load=print_env_on_load,
-            skip_create=skip_create,
-            skip_read=skip_read,
-            skip_update=skip_update,
-            recreate_on_update=recreate_on_update,
-            skip_delete=skip_delete,
-            wait_for_creation=wait_for_creation,
-            wait_for_update=wait_for_update,
-            wait_for_deletion=wait_for_deletion,
-            waiter_delay=waiter_delay,
-            waiter_max_attempts=waiter_max_attempts,
             use_cache=use_cache,
             **kwargs,
         )
```

### Comparing `phidata-1.6.9/phidata/app/server/server_base.py` & `phidata-1.7.0/phidata/app/server/server_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         ecs_launch_type: str = "FARGATE",
         ecs_task_cpu: str = "256",
         ecs_task_memory: str = "512",
         ecs_service_count: int = 1,
         assign_public_ip: bool = True,
         elb: Optional[Any] = None,
         aws_subnets: Optional[List[str]] = None,
-        aws_security_groups: Optional[List[str]] = None,
+        aws_security_groups: Optional[List[Any]] = None,
         # Other args,
         print_env_on_load: bool = False,
         skip_create: bool = False,
         skip_read: bool = False,
         skip_update: bool = False,
         recreate_on_update: bool = False,
         skip_delete: bool = False,
```

### Comparing `phidata-1.6.9/phidata/app/spark/spark_base.py` & `phidata-1.7.0/phidata/app/spark/spark_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,20 +58,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/spark/spark_driver.py` & `phidata-1.7.0/phidata/app/spark/spark_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,20 +41,20 @@
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
```

### Comparing `phidata-1.6.9/phidata/app/spark/spark_worker.py` & `phidata-1.7.0/phidata/app/superset/superset_worker_beat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,118 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.spark.spark_base import (
-    SparkBase,
-    SparkBaseArgs,
+from phidata.app.superset.superset_base import (
+    SupersetBase,
     ServiceType,
+    DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SparkWorker(SparkBase):
+class SupersetWorkerBeat(SupersetBase):
     def __init__(
         self,
-        name: str = "spark-worker",
+        name: str = "superset-worker-beat",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/spark",
-        image_tag: str = "3.3.1",
+        image_name: str = "phidata/superset",
+        image_tag: str = "2.0.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "worker",
+        command: Optional[Union[str, List]] = "beat",
         # Install python dependencies using a requirements.txt file,
+        # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
-        # -*- Spark Configuration
-        cores: Optional[int] = None,
-        memory: Optional[str] = None,
-        driver_url: Optional[str] = None,
-        properties_file: Optional[str] = None,
+        # -*- Superset Configuration,
+        # Configure Superset db,
+        wait_for_db: bool = False,
+        # Connect to database using a DbApp,
+        db_app: Optional[DbApp] = None,
+        # Provide database connection details manually,
+        # db_user can be provided here or as the,
+        # DATABASE_USER env var in the secrets_file,
+        db_user: Optional[str] = None,
+        # db_password can be provided here or as the,
+        # DATABASE_PASSWORD env var in the secrets_file,
+        db_password: Optional[str] = None,
+        # db_schema can be provided here or as the,
+        # DATABASE_DB env var in the secrets_file,
+        db_schema: Optional[str] = None,
+        # db_host can be provided here or as the,
+        # DATABASE_HOST env var in the secrets_file,
+        db_host: Optional[str] = None,
+        # db_port can be provided here or as the,
+        # DATABASE_PORT env var in the secrets_file,
+        db_port: Optional[int] = None,
+        # db_driver can be provided here or as the,
+        # DATABASE_DIALECT env var in the secrets_file,
+        db_dialect: Optional[str] = None,
+        # Configure superset redis,
+        wait_for_redis: bool = False,
+        # Connect to redis using a PhidataApp,
+        redis_app: Optional[DbApp] = None,
+        # redis_host can be provided here or as the,
+        # REDIS_HOST env var in the secrets_file,
+        redis_host: Optional[str] = None,
+        # redis_port can be provided here or as the,
+        # REDIS_PORT env var in the secrets_file,
+        redis_port: Optional[int] = None,
+        # redis_driver can be provided here or as the,
+        # REDIS_DRIVER env var in the secrets_file,
+        redis_driver: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
-        # Overwrite the PYTHONPATH env var,
-        # which is usually set to the workspace_root_container_path,
+        # Set the SUPERSET_CONFIG_PATH env var,
+        superset_config_path: Optional[str] = None,
+        # Set the FLASK_ENV env var,
+        flask_env: str = "production",
+        # Set the SUPERSET_ENV env var,
+        superset_env: str = "production",
+        # Set the PYTHONPATH env var,
+        # defaults to "/app/pythonpath:/app/docker/pythonpath_dev",
         python_path: Optional[str] = None,
-        # Add to the PYTHONPATH env var. If python_path is set, this is ignored
-        # Does not overwrite the PYTHONPATH env var - adds to it.
-        add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
-        open_container_port: bool = True,
+        open_container_port: bool = False,
         # Port number on the container,
-        container_port: int = 8080,
+        container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 8080,
+        container_host_port: int = 8000,
+        # Open the app port if open_app_port=True,
+        open_app_port: bool = False,
+        # App port number on the container,
+        # Set the SUPERSET_PORT env var,
+        app_port: int = 8088,
+        # Only used by the K8sContainer,
+        app_port_name: str = "app",
+        # Only used by the DockerContainer,
+        app_host_port: int = 8088,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
         # Path to mount the workspace volume,
         # This is the parent directory for the workspace on the container,
@@ -87,14 +132,23 @@
         # Required to create an initial copy of the workspace,
         create_git_sync_init_container: bool = True,
         git_sync_image_name: str = "k8s.gcr.io/git-sync",
         git_sync_image_tag: str = "v3.1.1",
         git_sync_repo: Optional[str] = None,
         git_sync_branch: Optional[str] = None,
         git_sync_wait: int = 1,
+        # Configure resources volume. Only on docker,
+        # Superset resources directory relative to the workspace_root,
+        # This directory contains all the files required by superset.,
+        # eg: docker-bootstrap.sh,
+        # This dir is mounted to the `/app/docker` directory on the container,
+        mount_resources: bool = False,
+        resources_dir: str = "workspace/superset",
+        resources_dir_container_path: str = "/app/docker",
+        resources_volume_name: Optional[str] = None,
         # -*- Docker configuration,
         # Run container in the background and return a Container object.,
         container_detach: bool = True,
         # Enable auto-removal of the container on daemon side when the container’s process exits.,
         container_auto_remove: bool = True,
         # Remove the container when it has finished running. Default: True.,
         container_remove: bool = True,
@@ -162,15 +216,15 @@
         topology_spread_max_skew: Optional[int] = None,
         # How to deal with a pod if it doesn't satisfy the spread constraint.,
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # K8s Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
-        service_type: Optional[ServiceType] = None,
+        service_type: Optional[Any] = None,
         # The port exposed by the service.,
         service_port: int = 8000,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
@@ -183,14 +237,39 @@
         # If ServiceType == ServiceType.LoadBalancer,
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
+        # App Service Configuration,
+        create_app_service: bool = False,
+        # Configure the app service,
+        app_svc_name: Optional[str] = None,
+        app_svc_type: Optional[ServiceType] = None,
+        # The port that will be exposed by the service.,
+        app_svc_port: int = 8088,
+        # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
+        app_node_port: Optional[int] = None,
+        # The app_target_port is the port to access on the pods targeted by the service.,
+        # It can be the port number or port name on the pod.,
+        app_target_port: Optional[Union[str, int]] = None,
+        # Extra ports exposed by the app service,
+        app_svc_ports: Optional[List[Any]] = None,
+        # Add labels to app service,
+        app_svc_labels: Optional[Dict[str, Any]] = None,
+        # Add annotations to app service,
+        app_svc_annotations: Optional[Dict[str, str]] = None,
+        # If ServiceType == LoadBalancer,
+        app_svc_health_check_node_port: Optional[int] = None,
+        app_svc_internal_taffic_policy: Optional[str] = None,
+        app_svc_load_balancer_class: Optional[str] = None,
+        app_svc_load_balancer_ip: Optional[str] = None,
+        app_svc_load_balancer_source_ranges: Optional[List[str]] = None,
+        app_svc_allocate_load_balancer_node_ports: Optional[bool] = None,
         # K8s RBAC Configuration,
         use_rbac: bool = False,
         # Create a Namespace with name ns_name & default values,
         ns_name: Optional[str] = None,
         # or Provide the full Namespace definition,
         # Type: CreateNamespace,
         namespace: Optional[Any] = None,
@@ -236,59 +315,77 @@
         extra_custom_objects: Optional[List[Any]] = None,
         # Type: CreateCustomResourceDefinition,
         extra_crds: Optional[List[Any]] = None,
         # Other args,
         print_env_on_load: bool = True,
         # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
+        # Set SUPERSET_LOAD_EXAMPLES = "yes",
+        load_examples: bool = False,
         **kwargs,
     ):
-        if driver_url is None:
-            raise ValueError("driver_url is required for SparkWorker")
-
         super().__init__(
             name=name,
             version=version,
             enabled=enabled,
             image=image,
             image_name=image_name,
             image_tag=image_tag,
             entrypoint=entrypoint,
             command=command,
             install_requirements=install_requirements,
             requirements_file=requirements_file,
-            cores=cores,
-            memory=memory,
-            driver_url=driver_url,
-            properties_file=properties_file,
+            wait_for_db=wait_for_db,
+            db_app=db_app,
+            db_user=db_user,
+            db_password=db_password,
+            db_schema=db_schema,
+            db_host=db_host,
+            db_port=db_port,
+            db_dialect=db_dialect,
+            wait_for_redis=wait_for_redis,
+            redis_app=redis_app,
+            redis_host=redis_host,
+            redis_port=redis_port,
+            redis_driver=redis_driver,
             container_name=container_name,
+            superset_config_path=superset_config_path,
+            flask_env=flask_env,
+            superset_env=superset_env,
             python_path=python_path,
-            add_python_path=add_python_path,
             container_labels=container_labels,
             env=env,
             env_file=env_file,
             secrets=secrets,
             secrets_file=secrets_file,
             aws_secrets=aws_secrets,
             open_container_port=open_container_port,
             container_port=container_port,
             container_port_name=container_port_name,
             container_host_port=container_host_port,
+            open_app_port=open_app_port,
+            app_port=app_port,
+            app_port_name=app_port_name,
+            app_host_port=app_host_port,
             mount_workspace=mount_workspace,
             workspace_volume_name=workspace_volume_name,
             workspace_volume_type=workspace_volume_type,
             workspace_volume_container_path=workspace_volume_container_path,
             workspace_volume_host_path=workspace_volume_host_path,
             create_git_sync_sidecar=create_git_sync_sidecar,
             create_git_sync_init_container=create_git_sync_init_container,
             git_sync_image_name=git_sync_image_name,
             git_sync_image_tag=git_sync_image_tag,
             git_sync_repo=git_sync_repo,
             git_sync_branch=git_sync_branch,
             git_sync_wait=git_sync_wait,
+            mount_resources=mount_resources,
+            resources_dir=resources_dir,
+            resources_dir_container_path=resources_dir_container_path,
+            resources_volume_name=resources_volume_name,
             container_detach=container_detach,
             container_auto_remove=container_auto_remove,
             container_remove=container_remove,
             container_user=container_user,
             container_stdin_open=container_stdin_open,
             container_tty=container_tty,
             container_healthcheck=container_healthcheck,
@@ -323,14 +420,29 @@
             service_annotations=service_annotations,
             service_health_check_node_port=service_health_check_node_port,
             service_internal_traffic_policy=service_internal_traffic_policy,
             service_load_balancer_class=service_load_balancer_class,
             service_load_balancer_ip=service_load_balancer_ip,
             service_load_balancer_source_ranges=service_load_balancer_source_ranges,
             service_allocate_load_balancer_node_ports=service_allocate_load_balancer_node_ports,
+            create_app_service=create_app_service,
+            app_svc_name=app_svc_name,
+            app_svc_type=app_svc_type,
+            app_svc_port=app_svc_port,
+            app_node_port=app_node_port,
+            app_target_port=app_target_port,
+            app_svc_ports=app_svc_ports,
+            app_svc_labels=app_svc_labels,
+            app_svc_annotations=app_svc_annotations,
+            app_svc_health_check_node_port=app_svc_health_check_node_port,
+            app_svc_internal_taffic_policy=app_svc_internal_taffic_policy,
+            app_svc_load_balancer_class=app_svc_load_balancer_class,
+            app_svc_load_balancer_ip=app_svc_load_balancer_ip,
+            app_svc_load_balancer_source_ranges=app_svc_load_balancer_source_ranges,
+            app_svc_allocate_load_balancer_node_ports=app_svc_allocate_load_balancer_node_ports,
             use_rbac=use_rbac,
             ns_name=ns_name,
             namespace=namespace,
             sa_name=sa_name,
             service_account=service_account,
             cr_name=cr_name,
             cluster_role=cluster_role,
@@ -347,9 +459,10 @@
             extra_ports=extra_ports,
             extra_volumes=extra_volumes,
             extra_storage_classes=extra_storage_classes,
             extra_custom_objects=extra_custom_objects,
             extra_crds=extra_crds,
             print_env_on_load=print_env_on_load,
             use_cache=use_cache,
+            load_examples=load_examples,
             **kwargs,
         )
```

### Comparing `phidata-1.6.9/phidata/app/streamlit/streamlit.py` & `phidata-1.7.0/phidata/app/superset/superset_init.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,86 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.server.server_base import (
-    ServerBase,
-    ServerBaseArgs,
+from phidata.app.superset.superset_base import (
+    SupersetBase,
     ServiceType,
+    DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class StreamlitAppArgs(ServerBaseArgs):
-    pass
-
-
-class StreamlitApp(ServerBase):
+class SupersetInit(SupersetBase):
     def __init__(
         self,
-        name: str = "streamlit-app",
+        name: str = "superset-init",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/streamlit",
-        image_tag: str = "latest",
-        entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "app start",
+        image_name: str = "phidata/superset",
+        image_tag: str = "2.0.1",
+        entrypoint: Optional[Union[str, List]] = "/scripts/init-superset.sh",
+        command: Optional[Union[str, List]] = None,
         # Install python dependencies using a requirements.txt file,
+        # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
-        # -*- Debug Mode
-        debug_mode: bool = False,
+        # -*- Superset Configuration,
+        # Configure Superset db,
+        wait_for_db: bool = False,
+        # Connect to database using a DbApp,
+        db_app: Optional[DbApp] = None,
+        # Provide database connection details manually,
+        # db_user can be provided here or as the,
+        # DATABASE_USER env var in the secrets_file,
+        db_user: Optional[str] = None,
+        # db_password can be provided here or as the,
+        # DATABASE_PASSWORD env var in the secrets_file,
+        db_password: Optional[str] = None,
+        # db_schema can be provided here or as the,
+        # DATABASE_DB env var in the secrets_file,
+        db_schema: Optional[str] = None,
+        # db_host can be provided here or as the,
+        # DATABASE_HOST env var in the secrets_file,
+        db_host: Optional[str] = None,
+        # db_port can be provided here or as the,
+        # DATABASE_PORT env var in the secrets_file,
+        db_port: Optional[int] = None,
+        # db_driver can be provided here or as the,
+        # DATABASE_DIALECT env var in the secrets_file,
+        db_dialect: Optional[str] = None,
+        # Configure superset redis,
+        wait_for_redis: bool = False,
+        # Connect to redis using a PhidataApp,
+        redis_app: Optional[DbApp] = None,
+        # redis_host can be provided here or as the,
+        # REDIS_HOST env var in the secrets_file,
+        redis_host: Optional[str] = None,
+        # redis_port can be provided here or as the,
+        # REDIS_PORT env var in the secrets_file,
+        redis_port: Optional[int] = None,
+        # redis_driver can be provided here or as the,
+        # REDIS_DRIVER env var in the secrets_file,
+        redis_driver: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
-        # Overwrite the PYTHONPATH env var,
-        # which is usually set to the workspace_root_container_path,
+        # Set the SUPERSET_CONFIG_PATH env var,
+        superset_config_path: Optional[str] = None,
+        # Set the FLASK_ENV env var,
+        flask_env: str = "production",
+        # Set the SUPERSET_ENV env var,
+        superset_env: str = "production",
+        # Set the PYTHONPATH env var,
+        # defaults to "/app/pythonpath:/app/docker/pythonpath_dev",
         python_path: Optional[str] = None,
-        # Add to the PYTHONPATH env var. If python_path is set, this is ignored
-        # Does not overwrite the PYTHONPATH env var - adds to it.
-        add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
         env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
@@ -54,28 +89,40 @@
         secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
-        open_container_port: bool = True,
+        open_container_port: bool = False,
         # Port number on the container,
-        container_port: int = 9095,
+        container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 9095,
+        container_host_port: int = 8000,
+        # Open the app port if open_app_port=True,
+        open_app_port: bool = False,
+        # App port number on the container,
+        # Set the SUPERSET_PORT env var,
+        app_port: int = 8088,
+        # Only used by the K8sContainer,
+        app_port_name: str = "app",
+        # Only used by the DockerContainer,
+        app_host_port: int = 8088,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume inside the container,
-        workspace_volume_container_path: str = "/usr/local/app",
+        # Path to mount the workspace volume,
+        # This is the parent directory for the workspace on the container,
+        # i.e. the ws is mounted as a subdir in this dir,
+        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
+        workspace_volume_container_path: str = "/mnt/workspaces",
         # How to mount the workspace volume,
         # Option 1: Mount the workspace from the host machine,
         # If None, use the workspace_root_path,
         # Note: This is the default on DockerContainers. We assume that DockerContainers,
         # are running locally on the user's machine so the local workspace_root_path,
         # is mounted to the workspace_volume_container_path,
         workspace_volume_host_path: Optional[str] = None,
@@ -85,14 +132,23 @@
         # Required to create an initial copy of the workspace,
         create_git_sync_init_container: bool = True,
         git_sync_image_name: str = "k8s.gcr.io/git-sync",
         git_sync_image_tag: str = "v3.1.1",
         git_sync_repo: Optional[str] = None,
         git_sync_branch: Optional[str] = None,
         git_sync_wait: int = 1,
+        # Configure resources volume. Only on docker,
+        # Superset resources directory relative to the workspace_root,
+        # This directory contains all the files required by superset.,
+        # eg: docker-bootstrap.sh,
+        # This dir is mounted to the `/app/docker` directory on the container,
+        mount_resources: bool = False,
+        resources_dir: str = "workspace/superset",
+        resources_dir_container_path: str = "/app/docker",
+        resources_volume_name: Optional[str] = None,
         # -*- Docker configuration,
         # Run container in the background and return a Container object.,
         container_detach: bool = True,
         # Enable auto-removal of the container on daemon side when the container’s process exits.,
         container_auto_remove: bool = True,
         # Remove the container when it has finished running. Default: True.,
         container_remove: bool = True,
@@ -160,17 +216,17 @@
         topology_spread_max_skew: Optional[int] = None,
         # How to deal with a pod if it doesn't satisfy the spread constraint.,
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # K8s Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
-        service_type: Optional[ServiceType] = None,
+        service_type: Optional[Any] = None,
         # The port exposed by the service.,
-        service_port: int = 9095,
+        service_port: int = 8000,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
@@ -181,14 +237,39 @@
         # If ServiceType == ServiceType.LoadBalancer,
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
+        # App Service Configuration,
+        create_app_service: bool = False,
+        # Configure the app service,
+        app_svc_name: Optional[str] = None,
+        app_svc_type: Optional[ServiceType] = None,
+        # The port that will be exposed by the service.,
+        app_svc_port: int = 8088,
+        # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
+        app_node_port: Optional[int] = None,
+        # The app_target_port is the port to access on the pods targeted by the service.,
+        # It can be the port number or port name on the pod.,
+        app_target_port: Optional[Union[str, int]] = None,
+        # Extra ports exposed by the app service,
+        app_svc_ports: Optional[List[Any]] = None,
+        # Add labels to app service,
+        app_svc_labels: Optional[Dict[str, Any]] = None,
+        # Add annotations to app service,
+        app_svc_annotations: Optional[Dict[str, str]] = None,
+        # If ServiceType == LoadBalancer,
+        app_svc_health_check_node_port: Optional[int] = None,
+        app_svc_internal_taffic_policy: Optional[str] = None,
+        app_svc_load_balancer_class: Optional[str] = None,
+        app_svc_load_balancer_ip: Optional[str] = None,
+        app_svc_load_balancer_source_ranges: Optional[List[str]] = None,
+        app_svc_allocate_load_balancer_node_ports: Optional[bool] = None,
         # K8s RBAC Configuration,
         use_rbac: bool = False,
         # Create a Namespace with name ns_name & default values,
         ns_name: Optional[str] = None,
         # or Provide the full Namespace definition,
         # Type: CreateNamespace,
         namespace: Optional[Any] = None,
@@ -230,77 +311,81 @@
         extra_volumes: Optional[List[Any]] = None,
         # Type: CreateStorageClass,
         extra_storage_classes: Optional[List[Any]] = None,
         # Type: CreateCustomObject,
         extra_custom_objects: Optional[List[Any]] = None,
         # Type: CreateCustomResourceDefinition,
         extra_crds: Optional[List[Any]] = None,
-        # -*- AWS configuration,
-        ecs_cluster: Optional[Any] = None,
-        ecs_launch_type: str = "FARGATE",
-        ecs_task_cpu: str = "256",
-        ecs_task_memory: str = "512",
-        ecs_service_count: int = 1,
-        assign_public_ip: bool = True,
-        elb: Optional[Any] = None,
-        aws_subnets: Optional[List[str]] = None,
-        aws_security_groups: Optional[List[str]] = None,
         # Other args,
-        print_env_on_load: bool = False,
-        skip_create: bool = False,
-        skip_read: bool = False,
-        skip_update: bool = False,
-        recreate_on_update: bool = False,
-        skip_delete: bool = False,
-        wait_for_creation: bool = True,
-        wait_for_update: bool = True,
-        wait_for_deletion: bool = True,
-        waiter_delay: int = 30,
-        waiter_max_attempts: int = 50,
+        print_env_on_load: bool = True,
         # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
+        # Set SUPERSET_LOAD_EXAMPLES = "yes",
+        load_examples: bool = False,
         **kwargs,
     ):
         super().__init__(
             name=name,
             version=version,
             enabled=enabled,
             image=image,
             image_name=image_name,
             image_tag=image_tag,
             entrypoint=entrypoint,
             command=command,
             install_requirements=install_requirements,
             requirements_file=requirements_file,
-            debug_mode=debug_mode,
+            wait_for_db=wait_for_db,
+            db_app=db_app,
+            db_user=db_user,
+            db_password=db_password,
+            db_schema=db_schema,
+            db_host=db_host,
+            db_port=db_port,
+            db_dialect=db_dialect,
+            wait_for_redis=wait_for_redis,
+            redis_app=redis_app,
+            redis_host=redis_host,
+            redis_port=redis_port,
+            redis_driver=redis_driver,
             container_name=container_name,
+            superset_config_path=superset_config_path,
+            flask_env=flask_env,
+            superset_env=superset_env,
             python_path=python_path,
-            add_python_path=add_python_path,
             container_labels=container_labels,
             env=env,
             env_file=env_file,
             secrets=secrets,
             secrets_file=secrets_file,
             aws_secrets=aws_secrets,
             open_container_port=open_container_port,
             container_port=container_port,
             container_port_name=container_port_name,
             container_host_port=container_host_port,
+            open_app_port=open_app_port,
+            app_port=app_port,
+            app_port_name=app_port_name,
+            app_host_port=app_host_port,
             mount_workspace=mount_workspace,
             workspace_volume_name=workspace_volume_name,
             workspace_volume_type=workspace_volume_type,
             workspace_volume_container_path=workspace_volume_container_path,
             workspace_volume_host_path=workspace_volume_host_path,
             create_git_sync_sidecar=create_git_sync_sidecar,
             create_git_sync_init_container=create_git_sync_init_container,
             git_sync_image_name=git_sync_image_name,
             git_sync_image_tag=git_sync_image_tag,
             git_sync_repo=git_sync_repo,
             git_sync_branch=git_sync_branch,
             git_sync_wait=git_sync_wait,
+            mount_resources=mount_resources,
+            resources_dir=resources_dir,
+            resources_dir_container_path=resources_dir_container_path,
+            resources_volume_name=resources_volume_name,
             container_detach=container_detach,
             container_auto_remove=container_auto_remove,
             container_remove=container_remove,
             container_user=container_user,
             container_stdin_open=container_stdin_open,
             container_tty=container_tty,
             container_healthcheck=container_healthcheck,
@@ -335,14 +420,29 @@
             service_annotations=service_annotations,
             service_health_check_node_port=service_health_check_node_port,
             service_internal_traffic_policy=service_internal_traffic_policy,
             service_load_balancer_class=service_load_balancer_class,
             service_load_balancer_ip=service_load_balancer_ip,
             service_load_balancer_source_ranges=service_load_balancer_source_ranges,
             service_allocate_load_balancer_node_ports=service_allocate_load_balancer_node_ports,
+            create_app_service=create_app_service,
+            app_svc_name=app_svc_name,
+            app_svc_type=app_svc_type,
+            app_svc_port=app_svc_port,
+            app_node_port=app_node_port,
+            app_target_port=app_target_port,
+            app_svc_ports=app_svc_ports,
+            app_svc_labels=app_svc_labels,
+            app_svc_annotations=app_svc_annotations,
+            app_svc_health_check_node_port=app_svc_health_check_node_port,
+            app_svc_internal_taffic_policy=app_svc_internal_taffic_policy,
+            app_svc_load_balancer_class=app_svc_load_balancer_class,
+            app_svc_load_balancer_ip=app_svc_load_balancer_ip,
+            app_svc_load_balancer_source_ranges=app_svc_load_balancer_source_ranges,
+            app_svc_allocate_load_balancer_node_ports=app_svc_allocate_load_balancer_node_ports,
             use_rbac=use_rbac,
             ns_name=ns_name,
             namespace=namespace,
             sa_name=sa_name,
             service_account=service_account,
             cr_name=cr_name,
             cluster_role=cluster_role,
@@ -357,30 +457,12 @@
             extra_containers=extra_containers,
             extra_init_containers=extra_init_containers,
             extra_ports=extra_ports,
             extra_volumes=extra_volumes,
             extra_storage_classes=extra_storage_classes,
             extra_custom_objects=extra_custom_objects,
             extra_crds=extra_crds,
-            ecs_cluster=ecs_cluster,
-            ecs_launch_type=ecs_launch_type,
-            ecs_task_cpu=ecs_task_cpu,
-            ecs_task_memory=ecs_task_memory,
-            ecs_service_count=ecs_service_count,
-            assign_public_ip=assign_public_ip,
-            elb=elb,
-            aws_subnets=aws_subnets,
-            aws_security_groups=aws_security_groups,
             print_env_on_load=print_env_on_load,
-            skip_create=skip_create,
-            skip_read=skip_read,
-            skip_update=skip_update,
-            recreate_on_update=recreate_on_update,
-            skip_delete=skip_delete,
-            wait_for_creation=wait_for_creation,
-            wait_for_update=wait_for_update,
-            wait_for_deletion=wait_for_deletion,
-            waiter_delay=waiter_delay,
-            waiter_max_attempts=waiter_max_attempts,
             use_cache=use_cache,
+            load_examples=load_examples,
             **kwargs,
         )
```

### Comparing `phidata-1.6.9/phidata/app/superset/superset_base.py` & `phidata-1.7.0/phidata/app/superset/superset_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,20 +192,20 @@
         # Set the PYTHONPATH env var,
         # defaults to "/app/pythonpath:/app/docker/pythonpath_dev",
         python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
```

### Comparing `phidata-1.6.9/phidata/app/superset/superset_init.py` & `phidata-1.7.0/phidata/app/superset/superset_webserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
     DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SupersetInit(SupersetBase):
+class SupersetWebserver(SupersetBase):
     def __init__(
         self,
-        name: str = "superset-init",
+        name: str = "superset-ws",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/superset",
         image_tag: str = "2.0.1",
-        entrypoint: Optional[Union[str, List]] = "/scripts/init-superset.sh",
-        command: Optional[Union[str, List]] = None,
+        entrypoint: Optional[Union[str, List]] = None,
+        command: Optional[Union[str, List]] = "webserver",
         # Install python dependencies using a requirements.txt file,
         # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Superset Configuration,
         # Configure Superset db,
@@ -77,35 +77,35 @@
         # Set the PYTHONPATH env var,
         # defaults to "/app/pythonpath:/app/docker/pythonpath_dev",
         python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
         # Port number on the container,
         container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
         container_host_port: int = 8000,
         # Open the app port if open_app_port=True,
-        open_app_port: bool = False,
+        open_app_port: bool = True,
         # App port number on the container,
         # Set the SUPERSET_PORT env var,
         app_port: int = 8088,
         # Only used by the K8sContainer,
         app_port_name: str = "app",
         # Only used by the DockerContainer,
         app_host_port: int = 8088,
@@ -238,15 +238,15 @@
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
         # App Service Configuration,
-        create_app_service: bool = False,
+        create_app_service: bool = True,
         # Configure the app service,
         app_svc_name: Optional[str] = None,
         app_svc_type: Optional[ServiceType] = None,
         # The port that will be exposed by the service.,
         app_svc_port: int = 8088,
         # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
         app_node_port: Optional[int] = None,
```

### Comparing `phidata-1.6.9/phidata/app/superset/superset_webserver.py` & `phidata-1.7.0/phidata/app/superset/superset_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,27 @@
     DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SupersetWebserver(SupersetBase):
+class SupersetWorker(SupersetBase):
     def __init__(
         self,
-        name: str = "superset-ws",
+        name: str = "superset-worker",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/superset",
         image_tag: str = "2.0.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "webserver",
+        command: Optional[Union[str, List]] = "worker",
         # Install python dependencies using a requirements.txt file,
         # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Superset Configuration,
         # Configure Superset db,
@@ -77,35 +77,35 @@
         # Set the PYTHONPATH env var,
         # defaults to "/app/pythonpath:/app/docker/pythonpath_dev",
         python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = False,
         # Port number on the container,
         container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
         container_host_port: int = 8000,
         # Open the app port if open_app_port=True,
-        open_app_port: bool = True,
+        open_app_port: bool = False,
         # App port number on the container,
         # Set the SUPERSET_PORT env var,
         app_port: int = 8088,
         # Only used by the K8sContainer,
         app_port_name: str = "app",
         # Only used by the DockerContainer,
         app_host_port: int = 8088,
@@ -238,15 +238,15 @@
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
         # App Service Configuration,
-        create_app_service: bool = True,
+        create_app_service: bool = False,
         # Configure the app service,
         app_svc_name: Optional[str] = None,
         app_svc_type: Optional[ServiceType] = None,
         # The port that will be exposed by the service.,
         app_svc_port: int = 8088,
         # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
         app_node_port: Optional[int] = None,
```

### Comparing `phidata-1.6.9/phidata/app/superset/superset_worker.py` & `phidata-1.7.0/phidata/app/fastapi/fastapi_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,276 +1,196 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.superset.superset_base import (
-    SupersetBase,
-    ServiceType,
-    DbApp,
-    WorkspaceVolumeType,
+from phidata.app.aws_app import AwsApp, AwsAppArgs
+from phidata.app.base_app import WorkspaceVolumeType
+from phidata.app.docker_app import DockerApp, DockerAppArgs
+from phidata.app.k8s_app import (
+    K8sApp,
+    K8sAppArgs,
     ImagePullPolicy,
     RestartPolicy,
+    ServiceType,
 )
+from phidata.utils.log import logger
+
 
+class FastApiServerArgs(AwsAppArgs, DockerAppArgs, K8sAppArgs):
+    pass
 
-class SupersetWorker(SupersetBase):
+
+class FastApiServer(AwsApp, DockerApp, K8sApp):
     def __init__(
         self,
-        name: str = "superset-worker",
+        name: str = "fastapi",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/superset",
-        image_tag: str = "2.0.1",
-        entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "worker",
+        image_name: str = "phidata/fastapi",
+        image_tag: str = "0.96",
+        entrypoint: Optional[Union[str, List[str]]] = None,
+        command: Union[
+            str, List[str]
+        ] = "uvicorn main:app --reload --host 0.0.0.0 --port 9090",
+        # -*- Debug Mode
+        debug_mode: bool = False,
+        # -*- Python Configuration,
         # Install python dependencies using a requirements.txt file,
-        # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
-        # -*- Superset Configuration,
-        # Configure Superset db,
-        wait_for_db: bool = False,
-        # Connect to database using a DbApp,
-        db_app: Optional[DbApp] = None,
-        # Provide database connection details manually,
-        # db_user can be provided here or as the,
-        # DATABASE_USER env var in the secrets_file,
-        db_user: Optional[str] = None,
-        # db_password can be provided here or as the,
-        # DATABASE_PASSWORD env var in the secrets_file,
-        db_password: Optional[str] = None,
-        # db_schema can be provided here or as the,
-        # DATABASE_DB env var in the secrets_file,
-        db_schema: Optional[str] = None,
-        # db_host can be provided here or as the,
-        # DATABASE_HOST env var in the secrets_file,
-        db_host: Optional[str] = None,
-        # db_port can be provided here or as the,
-        # DATABASE_PORT env var in the secrets_file,
-        db_port: Optional[int] = None,
-        # db_driver can be provided here or as the,
-        # DATABASE_DIALECT env var in the secrets_file,
-        db_dialect: Optional[str] = None,
-        # Configure superset redis,
-        wait_for_redis: bool = False,
-        # Connect to redis using a PhidataApp,
-        redis_app: Optional[DbApp] = None,
-        # redis_host can be provided here or as the,
-        # REDIS_HOST env var in the secrets_file,
-        redis_host: Optional[str] = None,
-        # redis_port can be provided here or as the,
-        # REDIS_PORT env var in the secrets_file,
-        redis_port: Optional[int] = None,
-        # redis_driver can be provided here or as the,
-        # REDIS_DRIVER env var in the secrets_file,
-        redis_driver: Optional[str] = None,
-        # -*- Container Configuration,
-        container_name: Optional[str] = None,
-        # Set the SUPERSET_CONFIG_PATH env var,
-        superset_config_path: Optional[str] = None,
-        # Set the FLASK_ENV env var,
-        flask_env: str = "production",
-        # Set the SUPERSET_ENV env var,
-        superset_env: str = "production",
         # Set the PYTHONPATH env var,
-        # defaults to "/app/pythonpath:/app/docker/pythonpath_dev",
+        set_python_path: bool = False,
+        # Manually provide the PYTHONPATH,
         python_path: Optional[str] = None,
-        # Add labels to the container,
-        container_labels: Optional[Dict[str, Any]] = None,
-        # Container env passed to the PhidataApp,
-        # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        # Add paths to the PYTHONPATH env var,
+        # If python_path is provided, this value is ignored,
+        add_python_paths: Optional[List[str]] = None,
+        # -*- Container Environment,
+        # Add env variables to container,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
-        # Container secrets,
-        # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        # Add secret variables to container,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
-        # Container ports,
+        # -*- Container Ports,
         # Open a container port if open_container_port=True,
-        open_container_port: bool = False,
+        open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 8000,
-        # Port name: Only used by the K8sContainer,
+        container_port: int = 9090,
+        # Port name (only used by the K8sContainer),
         container_port_name: str = "http",
-        # Host port: Only used by the DockerContainer,
-        container_host_port: int = 8000,
-        # Open the app port if open_app_port=True,
-        open_app_port: bool = False,
-        # App port number on the container,
-        # Set the SUPERSET_PORT env var,
-        app_port: int = 8088,
-        # Only used by the K8sContainer,
-        app_port_name: str = "app",
-        # Only used by the DockerContainer,
-        app_host_port: int = 8088,
-        # Container volumes,
+        # Host port to map to the container port,
+        container_host_port: int = 9090,
+        # -*- Workspace Volume,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume,
-        # This is the parent directory for the workspace on the container,
-        # i.e. the ws is mounted as a subdir in this dir,
-        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
-        workspace_volume_container_path: str = "/mnt/workspaces",
-        # How to mount the workspace volume,
-        # Option 1: Mount the workspace from the host machine,
-        # If None, use the workspace_root_path,
-        # Note: This is the default on DockerContainers. We assume that DockerContainers,
-        # are running locally on the user's machine so the local workspace_root_path,
-        # is mounted to the workspace_volume_container_path,
-        workspace_volume_host_path: Optional[str] = None,
-        # Option 2: Load the workspace from git using a git-sync sidecar container,
-        # This the default on K8sContainers.,
-        create_git_sync_sidecar: bool = False,
-        # Required to create an initial copy of the workspace,
-        create_git_sync_init_container: bool = True,
-        git_sync_image_name: str = "k8s.gcr.io/git-sync",
-        git_sync_image_tag: str = "v3.1.1",
-        git_sync_repo: Optional[str] = None,
-        git_sync_branch: Optional[str] = None,
-        git_sync_wait: int = 1,
-        # Configure resources volume. Only on docker,
-        # Superset resources directory relative to the workspace_root,
-        # This directory contains all the files required by superset.,
-        # eg: docker-bootstrap.sh,
-        # This dir is mounted to the `/app/docker` directory on the container,
-        mount_resources: bool = False,
-        resources_dir: str = "workspace/superset",
-        resources_dir_container_path: str = "/app/docker",
-        resources_volume_name: Optional[str] = None,
-        # -*- Docker configuration,
+        # Path to mount the workspace volume inside the container,
+        workspace_dir_container_path: str = "/usr/local/app",
+        # Add the workspace name to the container path,
+        add_workspace_name_to_container_path: bool = False,
+        # -*- If workspace_volume_type=WorkspaceVolumeType.HostPath,
+        # Mount workspace_dir to workspace_dir_container_path,
+        # If None, use the workspace_root,
+        workspace_dir: Optional[str] = None,
+        # -*- Container Configuration,
+        container_name: Optional[str] = None,
         # Run container in the background and return a Container object.,
         container_detach: bool = True,
         # Enable auto-removal of the container on daemon side when the container’s process exits.,
         container_auto_remove: bool = True,
         # Remove the container when it has finished running. Default: True.,
         container_remove: bool = True,
         # Username or UID to run commands as inside the container.,
         container_user: Optional[Union[str, int]] = None,
         # Keep STDIN open even if not attached.,
         container_stdin_open: bool = True,
+        # Return logs from STDOUT when container_detach=False.,
+        container_stdout: Optional[bool] = True,
+        # Return logs from STDERR when container_detach=False.,
+        container_stderr: Optional[bool] = True,
         container_tty: bool = True,
         # Specify a test to perform to check that the container is healthy.,
         container_healthcheck: Optional[Dict[str, Any]] = None,
         # Optional hostname for the container.,
         container_hostname: Optional[str] = None,
         # Platform in the format os[/arch[/variant]].,
         container_platform: Optional[str] = None,
         # Path to the working directory.,
         container_working_dir: Optional[str] = None,
+        # Add labels to the container,
+        container_labels: Optional[Dict[str, str]] = None,
         # Restart the container when it exits. Configured as a dictionary with keys:,
         # Name: One of on-failure, or always.,
         # MaximumRetryCount: Number of times to restart the container on failure.,
         # For example: {"Name": "on-failure", "MaximumRetryCount": 5},
-        container_restart_policy_docker: Optional[Dict[str, Any]] = None,
+        container_restart_policy: Optional[Dict[str, Any]] = None,
         # Add volumes to DockerContainer,
         # container_volumes is a dictionary which adds the volumes to mount,
         # inside the container. The key is either the host path or a volume name,,
         # and the value is a dictionary with 2 keys:,
         #   bind - The path to mount the volume inside the container,
         #   mode - Either rw to mount the volume read/write, or ro to mount it read-only.,
         # For example:,
         # {,
         #   '/home/user1/': {'bind': '/mnt/vol2', 'mode': 'rw'},,
         #   '/var/www': {'bind': '/mnt/vol1', 'mode': 'ro'},
         # },
-        container_volumes_docker: Optional[Dict[str, dict]] = None,
+        container_volumes: Optional[Dict[str, dict]] = None,
         # Add ports to DockerContainer,
         # The keys of the dictionary are the ports to bind inside the container,,
         # either as an integer or a string in the form port/protocol, where the protocol is either tcp, udp.,
         # The values of the dictionary are the corresponding ports to open on the host, which can be either:,
         #   - The port number, as an integer.,
         #       For example, {'2222/tcp': 3333} will expose port 2222 inside the container as port 3333 on the host.,
         #   - None, to assign a random host port. For example, {'2222/tcp': None}.,
         #   - A tuple of (address, port) if you want to specify the host interface.,
         #       For example, {'1111/tcp': ('127.0.0.1', 1111)}.,
         #   - A list of integers, if you want to bind multiple host ports to a single container port.,
         #       For example, {'1111/tcp': [1234, 4567]}.,
-        container_ports_docker: Optional[Dict[str, Any]] = None,
-        # -*- K8s configuration,
-        # K8s Deployment configuration,
-        replicas: int = 1,
+        container_ports: Optional[Dict[str, Any]] = None,
+        # -*- Pod Configuration,
         pod_name: Optional[str] = None,
-        deploy_name: Optional[str] = None,
+        pod_annotations: Optional[Dict[str, str]] = None,
+        pod_node_selector: Optional[Dict[str, str]] = None,
+        # -*- Secret Configuration,
         secret_name: Optional[str] = None,
+        # -*- Configmap Configuration,
         configmap_name: Optional[str] = None,
+        # -*- Deployment Configuration,
+        replicas: int = 1,
+        deploy_name: Optional[str] = None,
         # Type: ImagePullPolicy,
-        image_pull_policy: Optional[ImagePullPolicy] = None,
-        pod_annotations: Optional[Dict[str, str]] = None,
-        pod_node_selector: Optional[Dict[str, str]] = None,
+        image_pull_policy: Optional[Any] = None,
         # Type: RestartPolicy,
-        deploy_restart_policy: Optional[RestartPolicy] = None,
+        deploy_restart_policy: Optional[Any] = None,
         deploy_labels: Optional[Dict[str, Any]] = None,
         termination_grace_period_seconds: Optional[int] = None,
-        # How to spread the deployment across a topology,
-        # Key to spread the pods across,
+        # Key to spread the pods across a topology,
         topology_spread_key: Optional[str] = None,
         # The degree to which pods may be unevenly distributed,
         topology_spread_max_skew: Optional[int] = None,
         # How to deal with a pod if it doesn't satisfy the spread constraint.,
         topology_spread_when_unsatisfiable: Optional[str] = None,
-        # K8s Service Configuration,
+        # -*- Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[Any] = None,
         # The port exposed by the service.,
-        service_port: int = 8000,
+        service_port: int = 9090,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
-        # Service labels,
         service_labels: Optional[Dict[str, Any]] = None,
-        # Service annotations,
         service_annotations: Optional[Dict[str, str]] = None,
         # If ServiceType == ServiceType.LoadBalancer,
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
-        # App Service Configuration,
-        create_app_service: bool = False,
-        # Configure the app service,
-        app_svc_name: Optional[str] = None,
-        app_svc_type: Optional[ServiceType] = None,
-        # The port that will be exposed by the service.,
-        app_svc_port: int = 8088,
-        # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
-        app_node_port: Optional[int] = None,
-        # The app_target_port is the port to access on the pods targeted by the service.,
-        # It can be the port number or port name on the pod.,
-        app_target_port: Optional[Union[str, int]] = None,
-        # Extra ports exposed by the app service,
-        app_svc_ports: Optional[List[Any]] = None,
-        # Add labels to app service,
-        app_svc_labels: Optional[Dict[str, Any]] = None,
-        # Add annotations to app service,
-        app_svc_annotations: Optional[Dict[str, str]] = None,
-        # If ServiceType == LoadBalancer,
-        app_svc_health_check_node_port: Optional[int] = None,
-        app_svc_internal_taffic_policy: Optional[str] = None,
-        app_svc_load_balancer_class: Optional[str] = None,
-        app_svc_load_balancer_ip: Optional[str] = None,
-        app_svc_load_balancer_source_ranges: Optional[List[str]] = None,
-        app_svc_allocate_load_balancer_node_ports: Optional[bool] = None,
-        # K8s RBAC Configuration,
+        # -*- Ingress Configuration,
+        create_ingress: bool = False,
+        ingress_name: Optional[str] = None,
+        ingress_annotations: Optional[Dict[str, str]] = None,
+        # -*- RBAC Configuration,
         use_rbac: bool = False,
         # Create a Namespace with name ns_name & default values,
         ns_name: Optional[str] = None,
         # or Provide the full Namespace definition,
         # Type: CreateNamespace,
         namespace: Optional[Any] = None,
         # Create a ServiceAccount with name sa_name & default values,
@@ -284,185 +204,207 @@
         # Type: CreateClusterRole,
         cluster_role: Optional[Any] = None,
         # Create a ClusterRoleBinding with name crb_name & default values,
         crb_name: Optional[str] = None,
         # or Provide the full ClusterRoleBinding definition,
         # Type: CreateClusterRoleBinding,
         cluster_role_binding: Optional[Any] = None,
-        # Add additional Kubernetes resources to the App,
-        # Type: CreateSecret,
-        extra_secrets: Optional[List[Any]] = None,
-        # Type: CreateConfigMap,
-        extra_configmaps: Optional[List[Any]] = None,
-        # Type: CreateService,
-        extra_services: Optional[List[Any]] = None,
-        # Type: CreateDeployment,
-        extra_deployments: Optional[List[Any]] = None,
-        # Type: CreatePersistentVolume,
-        extra_pvs: Optional[List[Any]] = None,
-        # Type: CreatePVC,
-        extra_pvcs: Optional[List[Any]] = None,
-        # Type: CreateContainer,
-        extra_containers: Optional[List[Any]] = None,
-        # Type: CreateContainer,
-        extra_init_containers: Optional[List[Any]] = None,
-        # Type: CreatePort,
-        extra_ports: Optional[List[Any]] = None,
-        # Type: CreateVolume,
-        extra_volumes: Optional[List[Any]] = None,
-        # Type: CreateStorageClass,
-        extra_storage_classes: Optional[List[Any]] = None,
-        # Type: CreateCustomObject,
-        extra_custom_objects: Optional[List[Any]] = None,
-        # Type: CreateCustomResourceDefinition,
-        extra_crds: Optional[List[Any]] = None,
-        # Other args,
-        print_env_on_load: bool = True,
-        # If True, skip resource creation if active resources with the same name exist.,
+        # -*- AWS Configuration,
+        aws_subnets: Optional[List[str]] = None,
+        aws_security_groups: Optional[List[Any]] = None,
+        # -*- ECS Configuration,
+        ecs_cluster: Optional[Any] = None,
+        ecs_launch_type: str = "FARGATE",
+        ecs_task_cpu: str = "1024",
+        ecs_task_memory: str = "2048",
+        ecs_service_count: int = 1,
+        assign_public_ip: bool = True,
+        ecs_enable_exec: bool = True,
+        # -*- LoadBalancer Configuration,
+        load_balancer: Optional[Any] = None,
+        listener: Optional[Any] = None,
+        # Create a load balancer if load_balancer is None,
+        create_load_balancer: bool = False,
+        # HTTP or HTTPS,
+        load_balancer_protocol: str = "HTTP",
+        load_balancer_security_groups: Optional[List[Any]] = None,
+        # Default 80 for HTTP and 443 for HTTPS,
+        load_balancer_port: Optional[int] = None,
+        load_balancer_certificate: Optional[Any] = None,
+        load_balancer_certificate_arn: Optional[str] = None,
+        # -*- TargetGroup Configuration,
+        target_group: Optional[Any] = None,
+        # HTTP or HTTPS,
+        target_group_protocol: str = "HTTP",
+        # Default 80 for HTTP and 443 for HTTPS,
+        target_group_port: Optional[int] = None,
+        target_group_type: str = "ip",
+        health_check_protocol: Optional[str] = None,
+        health_check_port: Optional[str] = None,
+        health_check_enabled: Optional[bool] = None,
+        health_check_path: Optional[str] = None,
+        health_check_interval_seconds: Optional[int] = None,
+        health_check_timeout_seconds: Optional[int] = None,
+        healthy_threshold_count: Optional[int] = None,
+        unhealthy_threshold_count: Optional[int] = None,
+        #  -*- Resource Control,
+        skip_create: bool = False,
+        skip_read: bool = False,
+        skip_update: bool = False,
+        recreate_on_update: bool = False,
+        skip_delete: bool = False,
+        wait_for_creation: bool = True,
+        wait_for_update: bool = True,
+        wait_for_deletion: bool = True,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 50,
+        #  -*- Save Resources to output directory,
+        # If True, save the resources to files,
+        save_output: bool = False,
+        # The resource directory for the output files,
+        resource_dir: Optional[str] = None,
+        # Skip creation if resource with the same name is active,
         use_cache: bool = True,
-        # Set SUPERSET_LOAD_EXAMPLES = "yes",
-        load_examples: bool = False,
-        **kwargs,
+        #  -*- Other args,
+        print_env_on_load: bool = False,
+        # Extra kwargs used to capture additional args,
+        **extra_kwargs,
     ):
-        super().__init__(
-            name=name,
-            version=version,
-            enabled=enabled,
-            image=image,
-            image_name=image_name,
-            image_tag=image_tag,
-            entrypoint=entrypoint,
-            command=command,
-            install_requirements=install_requirements,
-            requirements_file=requirements_file,
-            wait_for_db=wait_for_db,
-            db_app=db_app,
-            db_user=db_user,
-            db_password=db_password,
-            db_schema=db_schema,
-            db_host=db_host,
-            db_port=db_port,
-            db_dialect=db_dialect,
-            wait_for_redis=wait_for_redis,
-            redis_app=redis_app,
-            redis_host=redis_host,
-            redis_port=redis_port,
-            redis_driver=redis_driver,
-            container_name=container_name,
-            superset_config_path=superset_config_path,
-            flask_env=flask_env,
-            superset_env=superset_env,
-            python_path=python_path,
-            container_labels=container_labels,
-            env=env,
-            env_file=env_file,
-            secrets=secrets,
-            secrets_file=secrets_file,
-            aws_secrets=aws_secrets,
-            open_container_port=open_container_port,
-            container_port=container_port,
-            container_port_name=container_port_name,
-            container_host_port=container_host_port,
-            open_app_port=open_app_port,
-            app_port=app_port,
-            app_port_name=app_port_name,
-            app_host_port=app_host_port,
-            mount_workspace=mount_workspace,
-            workspace_volume_name=workspace_volume_name,
-            workspace_volume_type=workspace_volume_type,
-            workspace_volume_container_path=workspace_volume_container_path,
-            workspace_volume_host_path=workspace_volume_host_path,
-            create_git_sync_sidecar=create_git_sync_sidecar,
-            create_git_sync_init_container=create_git_sync_init_container,
-            git_sync_image_name=git_sync_image_name,
-            git_sync_image_tag=git_sync_image_tag,
-            git_sync_repo=git_sync_repo,
-            git_sync_branch=git_sync_branch,
-            git_sync_wait=git_sync_wait,
-            mount_resources=mount_resources,
-            resources_dir=resources_dir,
-            resources_dir_container_path=resources_dir_container_path,
-            resources_volume_name=resources_volume_name,
-            container_detach=container_detach,
-            container_auto_remove=container_auto_remove,
-            container_remove=container_remove,
-            container_user=container_user,
-            container_stdin_open=container_stdin_open,
-            container_tty=container_tty,
-            container_healthcheck=container_healthcheck,
-            container_hostname=container_hostname,
-            container_platform=container_platform,
-            container_working_dir=container_working_dir,
-            container_restart_policy_docker=container_restart_policy_docker,
-            container_volumes_docker=container_volumes_docker,
-            container_ports_docker=container_ports_docker,
-            replicas=replicas,
-            pod_name=pod_name,
-            deploy_name=deploy_name,
-            secret_name=secret_name,
-            configmap_name=configmap_name,
-            image_pull_policy=image_pull_policy,
-            pod_annotations=pod_annotations,
-            pod_node_selector=pod_node_selector,
-            deploy_restart_policy=deploy_restart_policy,
-            deploy_labels=deploy_labels,
-            termination_grace_period_seconds=termination_grace_period_seconds,
-            topology_spread_key=topology_spread_key,
-            topology_spread_max_skew=topology_spread_max_skew,
-            topology_spread_when_unsatisfiable=topology_spread_when_unsatisfiable,
-            create_service=create_service,
-            service_name=service_name,
-            service_type=service_type,
-            service_port=service_port,
-            service_node_port=service_node_port,
-            service_target_port=service_target_port,
-            service_ports=service_ports,
-            service_labels=service_labels,
-            service_annotations=service_annotations,
-            service_health_check_node_port=service_health_check_node_port,
-            service_internal_traffic_policy=service_internal_traffic_policy,
-            service_load_balancer_class=service_load_balancer_class,
-            service_load_balancer_ip=service_load_balancer_ip,
-            service_load_balancer_source_ranges=service_load_balancer_source_ranges,
-            service_allocate_load_balancer_node_ports=service_allocate_load_balancer_node_ports,
-            create_app_service=create_app_service,
-            app_svc_name=app_svc_name,
-            app_svc_type=app_svc_type,
-            app_svc_port=app_svc_port,
-            app_node_port=app_node_port,
-            app_target_port=app_target_port,
-            app_svc_ports=app_svc_ports,
-            app_svc_labels=app_svc_labels,
-            app_svc_annotations=app_svc_annotations,
-            app_svc_health_check_node_port=app_svc_health_check_node_port,
-            app_svc_internal_taffic_policy=app_svc_internal_taffic_policy,
-            app_svc_load_balancer_class=app_svc_load_balancer_class,
-            app_svc_load_balancer_ip=app_svc_load_balancer_ip,
-            app_svc_load_balancer_source_ranges=app_svc_load_balancer_source_ranges,
-            app_svc_allocate_load_balancer_node_ports=app_svc_allocate_load_balancer_node_ports,
-            use_rbac=use_rbac,
-            ns_name=ns_name,
-            namespace=namespace,
-            sa_name=sa_name,
-            service_account=service_account,
-            cr_name=cr_name,
-            cluster_role=cluster_role,
-            crb_name=crb_name,
-            cluster_role_binding=cluster_role_binding,
-            extra_secrets=extra_secrets,
-            extra_configmaps=extra_configmaps,
-            extra_services=extra_services,
-            extra_deployments=extra_deployments,
-            extra_pvs=extra_pvs,
-            extra_pvcs=extra_pvcs,
-            extra_containers=extra_containers,
-            extra_init_containers=extra_init_containers,
-            extra_ports=extra_ports,
-            extra_volumes=extra_volumes,
-            extra_storage_classes=extra_storage_classes,
-            extra_custom_objects=extra_custom_objects,
-            extra_crds=extra_crds,
-            print_env_on_load=print_env_on_load,
-            use_cache=use_cache,
-            load_examples=load_examples,
-            **kwargs,
-        )
+        super().__init__()
+
+        try:
+            self.args: FastApiServerArgs = FastApiServerArgs(
+                name=name,
+                version=version,
+                enabled=enabled,
+                image=image,
+                image_name=image_name,
+                image_tag=image_tag,
+                entrypoint=entrypoint,
+                command=command,
+                debug_mode=debug_mode,
+                install_requirements=install_requirements,
+                requirements_file=requirements_file,
+                set_python_path=set_python_path,
+                python_path=python_path,
+                add_python_paths=add_python_paths,
+                env=env,
+                env_file=env_file,
+                secrets=secrets,
+                secrets_file=secrets_file,
+                aws_secrets=aws_secrets,
+                open_container_port=open_container_port,
+                container_port=container_port,
+                container_port_name=container_port_name,
+                container_host_port=container_host_port,
+                mount_workspace=mount_workspace,
+                workspace_volume_name=workspace_volume_name,
+                workspace_volume_type=workspace_volume_type,
+                workspace_dir_container_path=workspace_dir_container_path,
+                add_workspace_name_to_container_path=add_workspace_name_to_container_path,
+                workspace_dir=workspace_dir,
+                container_name=container_name,
+                container_detach=container_detach,
+                container_auto_remove=container_auto_remove,
+                container_remove=container_remove,
+                container_user=container_user,
+                container_stdin_open=container_stdin_open,
+                container_stdout=container_stdout,
+                container_stderr=container_stderr,
+                container_tty=container_tty,
+                container_healthcheck=container_healthcheck,
+                container_hostname=container_hostname,
+                container_platform=container_platform,
+                container_working_dir=container_working_dir,
+                container_labels=container_labels,
+                container_restart_policy=container_restart_policy,
+                container_volumes=container_volumes,
+                container_ports=container_ports,
+                pod_name=pod_name,
+                pod_annotations=pod_annotations,
+                pod_node_selector=pod_node_selector,
+                secret_name=secret_name,
+                configmap_name=configmap_name,
+                replicas=replicas,
+                deploy_name=deploy_name,
+                image_pull_policy=image_pull_policy,
+                deploy_restart_policy=deploy_restart_policy,
+                deploy_labels=deploy_labels,
+                termination_grace_period_seconds=termination_grace_period_seconds,
+                topology_spread_key=topology_spread_key,
+                topology_spread_max_skew=topology_spread_max_skew,
+                topology_spread_when_unsatisfiable=topology_spread_when_unsatisfiable,
+                create_service=create_service,
+                service_name=service_name,
+                service_type=service_type,
+                service_port=service_port,
+                service_node_port=service_node_port,
+                service_target_port=service_target_port,
+                service_ports=service_ports,
+                service_labels=service_labels,
+                service_annotations=service_annotations,
+                service_health_check_node_port=service_health_check_node_port,
+                service_internal_traffic_policy=service_internal_traffic_policy,
+                service_load_balancer_class=service_load_balancer_class,
+                service_load_balancer_ip=service_load_balancer_ip,
+                service_load_balancer_source_ranges=service_load_balancer_source_ranges,
+                service_allocate_load_balancer_node_ports=service_allocate_load_balancer_node_ports,
+                create_ingress=create_ingress,
+                ingress_name=ingress_name,
+                ingress_annotations=ingress_annotations,
+                use_rbac=use_rbac,
+                ns_name=ns_name,
+                namespace=namespace,
+                sa_name=sa_name,
+                service_account=service_account,
+                cr_name=cr_name,
+                cluster_role=cluster_role,
+                crb_name=crb_name,
+                cluster_role_binding=cluster_role_binding,
+                aws_subnets=aws_subnets,
+                aws_security_groups=aws_security_groups,
+                ecs_cluster=ecs_cluster,
+                ecs_launch_type=ecs_launch_type,
+                ecs_task_cpu=ecs_task_cpu,
+                ecs_task_memory=ecs_task_memory,
+                ecs_service_count=ecs_service_count,
+                assign_public_ip=assign_public_ip,
+                ecs_enable_exec=ecs_enable_exec,
+                load_balancer=load_balancer,
+                listener=listener,
+                create_load_balancer=create_load_balancer,
+                load_balancer_protocol=load_balancer_protocol,
+                load_balancer_security_groups=load_balancer_security_groups,
+                load_balancer_port=load_balancer_port,
+                load_balancer_certificate=load_balancer_certificate,
+                load_balancer_certificate_arn=load_balancer_certificate_arn,
+                target_group=target_group,
+                target_group_protocol=target_group_protocol,
+                target_group_port=target_group_port,
+                target_group_type=target_group_type,
+                health_check_protocol=health_check_protocol,
+                health_check_port=health_check_port,
+                health_check_enabled=health_check_enabled,
+                health_check_path=health_check_path,
+                health_check_interval_seconds=health_check_interval_seconds,
+                health_check_timeout_seconds=health_check_timeout_seconds,
+                healthy_threshold_count=healthy_threshold_count,
+                unhealthy_threshold_count=unhealthy_threshold_count,
+                skip_create=skip_create,
+                skip_read=skip_read,
+                skip_update=skip_update,
+                recreate_on_update=recreate_on_update,
+                skip_delete=skip_delete,
+                wait_for_creation=wait_for_creation,
+                wait_for_update=wait_for_update,
+                wait_for_deletion=wait_for_deletion,
+                waiter_delay=waiter_delay,
+                waiter_max_attempts=waiter_max_attempts,
+                save_output=save_output,
+                resource_dir=resource_dir,
+                use_cache=use_cache,
+                print_env_on_load=print_env_on_load,
+                **extra_kwargs,
+            )
+        except Exception as e:
+            logger.error(f"Args for {self.name} are not valid: {e}")
+            raise
```

### Comparing `phidata-1.6.9/phidata/app/superset/superset_worker_beat.py` & `phidata-1.7.0/phidata/app/streamlit/streamlit_app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,276 +1,194 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.superset.superset_base import (
-    SupersetBase,
-    ServiceType,
-    DbApp,
-    WorkspaceVolumeType,
+from phidata.app.aws_app import AwsApp, AwsAppArgs
+from phidata.app.base_app import WorkspaceVolumeType
+from phidata.app.docker_app import DockerApp, DockerAppArgs
+from phidata.app.k8s_app import (
+    K8sApp,
+    K8sAppArgs,
     ImagePullPolicy,
     RestartPolicy,
+    ServiceType,
 )
+from phidata.utils.log import logger
+
 
+class StreamlitAppArgs(AwsAppArgs, DockerAppArgs, K8sAppArgs):
+    pass
 
-class SupersetWorkerBeat(SupersetBase):
+
+class StreamlitApp(AwsApp, DockerApp, K8sApp):
     def __init__(
         self,
-        name: str = "superset-worker-beat",
+        name: str = "streamlit",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/superset",
-        image_tag: str = "2.0.1",
+        image_name: str = "phidata/streamlit",
+        image_tag: str = "1.23",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "beat",
+        command: Optional[Union[str, List]] = "streamlit hello",
+        # -*- Debug Mode
+        debug_mode: bool = False,
+        # -*- Python Configuration,
         # Install python dependencies using a requirements.txt file,
-        # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
-        # -*- Superset Configuration,
-        # Configure Superset db,
-        wait_for_db: bool = False,
-        # Connect to database using a DbApp,
-        db_app: Optional[DbApp] = None,
-        # Provide database connection details manually,
-        # db_user can be provided here or as the,
-        # DATABASE_USER env var in the secrets_file,
-        db_user: Optional[str] = None,
-        # db_password can be provided here or as the,
-        # DATABASE_PASSWORD env var in the secrets_file,
-        db_password: Optional[str] = None,
-        # db_schema can be provided here or as the,
-        # DATABASE_DB env var in the secrets_file,
-        db_schema: Optional[str] = None,
-        # db_host can be provided here or as the,
-        # DATABASE_HOST env var in the secrets_file,
-        db_host: Optional[str] = None,
-        # db_port can be provided here or as the,
-        # DATABASE_PORT env var in the secrets_file,
-        db_port: Optional[int] = None,
-        # db_driver can be provided here or as the,
-        # DATABASE_DIALECT env var in the secrets_file,
-        db_dialect: Optional[str] = None,
-        # Configure superset redis,
-        wait_for_redis: bool = False,
-        # Connect to redis using a PhidataApp,
-        redis_app: Optional[DbApp] = None,
-        # redis_host can be provided here or as the,
-        # REDIS_HOST env var in the secrets_file,
-        redis_host: Optional[str] = None,
-        # redis_port can be provided here or as the,
-        # REDIS_PORT env var in the secrets_file,
-        redis_port: Optional[int] = None,
-        # redis_driver can be provided here or as the,
-        # REDIS_DRIVER env var in the secrets_file,
-        redis_driver: Optional[str] = None,
-        # -*- Container Configuration,
-        container_name: Optional[str] = None,
-        # Set the SUPERSET_CONFIG_PATH env var,
-        superset_config_path: Optional[str] = None,
-        # Set the FLASK_ENV env var,
-        flask_env: str = "production",
-        # Set the SUPERSET_ENV env var,
-        superset_env: str = "production",
         # Set the PYTHONPATH env var,
-        # defaults to "/app/pythonpath:/app/docker/pythonpath_dev",
+        set_python_path: bool = False,
+        # Manually provide the PYTHONPATH,
         python_path: Optional[str] = None,
-        # Add labels to the container,
-        container_labels: Optional[Dict[str, Any]] = None,
-        # Container env passed to the PhidataApp,
-        # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        # Add paths to the PYTHONPATH env var,
+        # If python_path is provided, this value is ignored,
+        add_python_paths: Optional[List[str]] = None,
+        # -*- Container Environment,
+        # Add env variables to container,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
-        # Container secrets,
-        # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        # Add secret variables to container,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
-        # Container ports,
+        # -*- Container Ports,
         # Open a container port if open_container_port=True,
-        open_container_port: bool = False,
+        open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 8000,
-        # Port name: Only used by the K8sContainer,
+        container_port: int = 9095,
+        # Port name (only used by the K8sContainer),
         container_port_name: str = "http",
-        # Host port: Only used by the DockerContainer,
-        container_host_port: int = 8000,
-        # Open the app port if open_app_port=True,
-        open_app_port: bool = False,
-        # App port number on the container,
-        # Set the SUPERSET_PORT env var,
-        app_port: int = 8088,
-        # Only used by the K8sContainer,
-        app_port_name: str = "app",
-        # Only used by the DockerContainer,
-        app_host_port: int = 8088,
-        # Container volumes,
+        # Host port to map to the container port,
+        container_host_port: int = 9095,
+        # -*- Workspace Volume,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume,
-        # This is the parent directory for the workspace on the container,
-        # i.e. the ws is mounted as a subdir in this dir,
-        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
-        workspace_volume_container_path: str = "/mnt/workspaces",
-        # How to mount the workspace volume,
-        # Option 1: Mount the workspace from the host machine,
-        # If None, use the workspace_root_path,
-        # Note: This is the default on DockerContainers. We assume that DockerContainers,
-        # are running locally on the user's machine so the local workspace_root_path,
-        # is mounted to the workspace_volume_container_path,
-        workspace_volume_host_path: Optional[str] = None,
-        # Option 2: Load the workspace from git using a git-sync sidecar container,
-        # This the default on K8sContainers.,
-        create_git_sync_sidecar: bool = False,
-        # Required to create an initial copy of the workspace,
-        create_git_sync_init_container: bool = True,
-        git_sync_image_name: str = "k8s.gcr.io/git-sync",
-        git_sync_image_tag: str = "v3.1.1",
-        git_sync_repo: Optional[str] = None,
-        git_sync_branch: Optional[str] = None,
-        git_sync_wait: int = 1,
-        # Configure resources volume. Only on docker,
-        # Superset resources directory relative to the workspace_root,
-        # This directory contains all the files required by superset.,
-        # eg: docker-bootstrap.sh,
-        # This dir is mounted to the `/app/docker` directory on the container,
-        mount_resources: bool = False,
-        resources_dir: str = "workspace/superset",
-        resources_dir_container_path: str = "/app/docker",
-        resources_volume_name: Optional[str] = None,
-        # -*- Docker configuration,
+        # Path to mount the workspace volume inside the container,
+        workspace_dir_container_path: str = "/usr/local/app",
+        # Add the workspace name to the container path,
+        add_workspace_name_to_container_path: bool = False,
+        # -*- If workspace_volume_type=WorkspaceVolumeType.HostPath,
+        # Mount workspace_dir to workspace_dir_container_path,
+        # If None, use the workspace_root,
+        workspace_dir: Optional[str] = None,
+        # -*- Container Configuration,
+        container_name: Optional[str] = None,
         # Run container in the background and return a Container object.,
         container_detach: bool = True,
         # Enable auto-removal of the container on daemon side when the container’s process exits.,
         container_auto_remove: bool = True,
         # Remove the container when it has finished running. Default: True.,
         container_remove: bool = True,
         # Username or UID to run commands as inside the container.,
         container_user: Optional[Union[str, int]] = None,
         # Keep STDIN open even if not attached.,
         container_stdin_open: bool = True,
+        # Return logs from STDOUT when container_detach=False.,
+        container_stdout: Optional[bool] = True,
+        # Return logs from STDERR when container_detach=False.,
+        container_stderr: Optional[bool] = True,
         container_tty: bool = True,
         # Specify a test to perform to check that the container is healthy.,
         container_healthcheck: Optional[Dict[str, Any]] = None,
         # Optional hostname for the container.,
         container_hostname: Optional[str] = None,
         # Platform in the format os[/arch[/variant]].,
         container_platform: Optional[str] = None,
         # Path to the working directory.,
         container_working_dir: Optional[str] = None,
+        # Add labels to the container,
+        container_labels: Optional[Dict[str, str]] = None,
         # Restart the container when it exits. Configured as a dictionary with keys:,
         # Name: One of on-failure, or always.,
         # MaximumRetryCount: Number of times to restart the container on failure.,
         # For example: {"Name": "on-failure", "MaximumRetryCount": 5},
-        container_restart_policy_docker: Optional[Dict[str, Any]] = None,
+        container_restart_policy: Optional[Dict[str, Any]] = None,
         # Add volumes to DockerContainer,
         # container_volumes is a dictionary which adds the volumes to mount,
         # inside the container. The key is either the host path or a volume name,,
         # and the value is a dictionary with 2 keys:,
         #   bind - The path to mount the volume inside the container,
         #   mode - Either rw to mount the volume read/write, or ro to mount it read-only.,
         # For example:,
         # {,
         #   '/home/user1/': {'bind': '/mnt/vol2', 'mode': 'rw'},,
         #   '/var/www': {'bind': '/mnt/vol1', 'mode': 'ro'},
         # },
-        container_volumes_docker: Optional[Dict[str, dict]] = None,
+        container_volumes: Optional[Dict[str, dict]] = None,
         # Add ports to DockerContainer,
         # The keys of the dictionary are the ports to bind inside the container,,
         # either as an integer or a string in the form port/protocol, where the protocol is either tcp, udp.,
         # The values of the dictionary are the corresponding ports to open on the host, which can be either:,
         #   - The port number, as an integer.,
         #       For example, {'2222/tcp': 3333} will expose port 2222 inside the container as port 3333 on the host.,
         #   - None, to assign a random host port. For example, {'2222/tcp': None}.,
         #   - A tuple of (address, port) if you want to specify the host interface.,
         #       For example, {'1111/tcp': ('127.0.0.1', 1111)}.,
         #   - A list of integers, if you want to bind multiple host ports to a single container port.,
         #       For example, {'1111/tcp': [1234, 4567]}.,
-        container_ports_docker: Optional[Dict[str, Any]] = None,
-        # -*- K8s configuration,
-        # K8s Deployment configuration,
-        replicas: int = 1,
+        container_ports: Optional[Dict[str, Any]] = None,
+        # -*- Pod Configuration,
         pod_name: Optional[str] = None,
-        deploy_name: Optional[str] = None,
+        pod_annotations: Optional[Dict[str, str]] = None,
+        pod_node_selector: Optional[Dict[str, str]] = None,
+        # -*- Secret Configuration,
         secret_name: Optional[str] = None,
+        # -*- Configmap Configuration,
         configmap_name: Optional[str] = None,
+        # -*- Deployment Configuration,
+        replicas: int = 1,
+        deploy_name: Optional[str] = None,
         # Type: ImagePullPolicy,
-        image_pull_policy: Optional[ImagePullPolicy] = None,
-        pod_annotations: Optional[Dict[str, str]] = None,
-        pod_node_selector: Optional[Dict[str, str]] = None,
+        image_pull_policy: Optional[Any] = None,
         # Type: RestartPolicy,
-        deploy_restart_policy: Optional[RestartPolicy] = None,
+        deploy_restart_policy: Optional[Any] = None,
         deploy_labels: Optional[Dict[str, Any]] = None,
         termination_grace_period_seconds: Optional[int] = None,
-        # How to spread the deployment across a topology,
-        # Key to spread the pods across,
+        # Key to spread the pods across a topology,
         topology_spread_key: Optional[str] = None,
         # The degree to which pods may be unevenly distributed,
         topology_spread_max_skew: Optional[int] = None,
         # How to deal with a pod if it doesn't satisfy the spread constraint.,
         topology_spread_when_unsatisfiable: Optional[str] = None,
-        # K8s Service Configuration,
+        # -*- Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[Any] = None,
         # The port exposed by the service.,
-        service_port: int = 8000,
+        service_port: int = 9095,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
-        # Service labels,
         service_labels: Optional[Dict[str, Any]] = None,
-        # Service annotations,
         service_annotations: Optional[Dict[str, str]] = None,
         # If ServiceType == ServiceType.LoadBalancer,
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
-        # App Service Configuration,
-        create_app_service: bool = False,
-        # Configure the app service,
-        app_svc_name: Optional[str] = None,
-        app_svc_type: Optional[ServiceType] = None,
-        # The port that will be exposed by the service.,
-        app_svc_port: int = 8088,
-        # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
-        app_node_port: Optional[int] = None,
-        # The app_target_port is the port to access on the pods targeted by the service.,
-        # It can be the port number or port name on the pod.,
-        app_target_port: Optional[Union[str, int]] = None,
-        # Extra ports exposed by the app service,
-        app_svc_ports: Optional[List[Any]] = None,
-        # Add labels to app service,
-        app_svc_labels: Optional[Dict[str, Any]] = None,
-        # Add annotations to app service,
-        app_svc_annotations: Optional[Dict[str, str]] = None,
-        # If ServiceType == LoadBalancer,
-        app_svc_health_check_node_port: Optional[int] = None,
-        app_svc_internal_taffic_policy: Optional[str] = None,
-        app_svc_load_balancer_class: Optional[str] = None,
-        app_svc_load_balancer_ip: Optional[str] = None,
-        app_svc_load_balancer_source_ranges: Optional[List[str]] = None,
-        app_svc_allocate_load_balancer_node_ports: Optional[bool] = None,
-        # K8s RBAC Configuration,
+        # -*- Ingress Configuration,
+        create_ingress: bool = False,
+        ingress_name: Optional[str] = None,
+        ingress_annotations: Optional[Dict[str, str]] = None,
+        # -*- RBAC Configuration,
         use_rbac: bool = False,
         # Create a Namespace with name ns_name & default values,
         ns_name: Optional[str] = None,
         # or Provide the full Namespace definition,
         # Type: CreateNamespace,
         namespace: Optional[Any] = None,
         # Create a ServiceAccount with name sa_name & default values,
@@ -284,185 +202,207 @@
         # Type: CreateClusterRole,
         cluster_role: Optional[Any] = None,
         # Create a ClusterRoleBinding with name crb_name & default values,
         crb_name: Optional[str] = None,
         # or Provide the full ClusterRoleBinding definition,
         # Type: CreateClusterRoleBinding,
         cluster_role_binding: Optional[Any] = None,
-        # Add additional Kubernetes resources to the App,
-        # Type: CreateSecret,
-        extra_secrets: Optional[List[Any]] = None,
-        # Type: CreateConfigMap,
-        extra_configmaps: Optional[List[Any]] = None,
-        # Type: CreateService,
-        extra_services: Optional[List[Any]] = None,
-        # Type: CreateDeployment,
-        extra_deployments: Optional[List[Any]] = None,
-        # Type: CreatePersistentVolume,
-        extra_pvs: Optional[List[Any]] = None,
-        # Type: CreatePVC,
-        extra_pvcs: Optional[List[Any]] = None,
-        # Type: CreateContainer,
-        extra_containers: Optional[List[Any]] = None,
-        # Type: CreateContainer,
-        extra_init_containers: Optional[List[Any]] = None,
-        # Type: CreatePort,
-        extra_ports: Optional[List[Any]] = None,
-        # Type: CreateVolume,
-        extra_volumes: Optional[List[Any]] = None,
-        # Type: CreateStorageClass,
-        extra_storage_classes: Optional[List[Any]] = None,
-        # Type: CreateCustomObject,
-        extra_custom_objects: Optional[List[Any]] = None,
-        # Type: CreateCustomResourceDefinition,
-        extra_crds: Optional[List[Any]] = None,
-        # Other args,
-        print_env_on_load: bool = True,
-        # If True, skip resource creation if active resources with the same name exist.,
+        # -*- AWS Configuration,
+        aws_subnets: Optional[List[str]] = None,
+        aws_security_groups: Optional[List[Any]] = None,
+        # -*- ECS Configuration,
+        ecs_cluster: Optional[Any] = None,
+        ecs_launch_type: str = "FARGATE",
+        ecs_task_cpu: str = "1024",
+        ecs_task_memory: str = "2048",
+        ecs_service_count: int = 1,
+        assign_public_ip: bool = True,
+        ecs_enable_exec: bool = True,
+        # -*- LoadBalancer Configuration,
+        load_balancer: Optional[Any] = None,
+        listener: Optional[Any] = None,
+        # Create a load balancer if load_balancer is None,
+        create_load_balancer: bool = False,
+        # HTTP or HTTPS,
+        load_balancer_protocol: str = "HTTP",
+        load_balancer_security_groups: Optional[List[Any]] = None,
+        # Default 80 for HTTP and 443 for HTTPS,
+        load_balancer_port: Optional[int] = None,
+        load_balancer_certificate: Optional[Any] = None,
+        load_balancer_certificate_arn: Optional[str] = None,
+        # -*- TargetGroup Configuration,
+        target_group: Optional[Any] = None,
+        # HTTP or HTTPS,
+        target_group_protocol: str = "HTTP",
+        # Default 80 for HTTP and 443 for HTTPS,
+        target_group_port: Optional[int] = None,
+        target_group_type: str = "ip",
+        health_check_protocol: Optional[str] = None,
+        health_check_port: Optional[str] = None,
+        health_check_enabled: Optional[bool] = None,
+        health_check_path: Optional[str] = None,
+        health_check_interval_seconds: Optional[int] = None,
+        health_check_timeout_seconds: Optional[int] = None,
+        healthy_threshold_count: Optional[int] = None,
+        unhealthy_threshold_count: Optional[int] = None,
+        #  -*- Resource Control,
+        skip_create: bool = False,
+        skip_read: bool = False,
+        skip_update: bool = False,
+        recreate_on_update: bool = False,
+        skip_delete: bool = False,
+        wait_for_creation: bool = True,
+        wait_for_update: bool = True,
+        wait_for_deletion: bool = True,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 50,
+        #  -*- Save Resources to output directory,
+        # If True, save the resources to files,
+        save_output: bool = False,
+        # The resource directory for the output files,
+        resource_dir: Optional[str] = None,
+        # Skip creation if resource with the same name is active,
         use_cache: bool = True,
-        # Set SUPERSET_LOAD_EXAMPLES = "yes",
-        load_examples: bool = False,
-        **kwargs,
+        #  -*- Other args,
+        print_env_on_load: bool = False,
+        # Extra kwargs used to capture additional args,
+        **extra_kwargs,
     ):
-        super().__init__(
-            name=name,
-            version=version,
-            enabled=enabled,
-            image=image,
-            image_name=image_name,
-            image_tag=image_tag,
-            entrypoint=entrypoint,
-            command=command,
-            install_requirements=install_requirements,
-            requirements_file=requirements_file,
-            wait_for_db=wait_for_db,
-            db_app=db_app,
-            db_user=db_user,
-            db_password=db_password,
-            db_schema=db_schema,
-            db_host=db_host,
-            db_port=db_port,
-            db_dialect=db_dialect,
-            wait_for_redis=wait_for_redis,
-            redis_app=redis_app,
-            redis_host=redis_host,
-            redis_port=redis_port,
-            redis_driver=redis_driver,
-            container_name=container_name,
-            superset_config_path=superset_config_path,
-            flask_env=flask_env,
-            superset_env=superset_env,
-            python_path=python_path,
-            container_labels=container_labels,
-            env=env,
-            env_file=env_file,
-            secrets=secrets,
-            secrets_file=secrets_file,
-            aws_secrets=aws_secrets,
-            open_container_port=open_container_port,
-            container_port=container_port,
-            container_port_name=container_port_name,
-            container_host_port=container_host_port,
-            open_app_port=open_app_port,
-            app_port=app_port,
-            app_port_name=app_port_name,
-            app_host_port=app_host_port,
-            mount_workspace=mount_workspace,
-            workspace_volume_name=workspace_volume_name,
-            workspace_volume_type=workspace_volume_type,
-            workspace_volume_container_path=workspace_volume_container_path,
-            workspace_volume_host_path=workspace_volume_host_path,
-            create_git_sync_sidecar=create_git_sync_sidecar,
-            create_git_sync_init_container=create_git_sync_init_container,
-            git_sync_image_name=git_sync_image_name,
-            git_sync_image_tag=git_sync_image_tag,
-            git_sync_repo=git_sync_repo,
-            git_sync_branch=git_sync_branch,
-            git_sync_wait=git_sync_wait,
-            mount_resources=mount_resources,
-            resources_dir=resources_dir,
-            resources_dir_container_path=resources_dir_container_path,
-            resources_volume_name=resources_volume_name,
-            container_detach=container_detach,
-            container_auto_remove=container_auto_remove,
-            container_remove=container_remove,
-            container_user=container_user,
-            container_stdin_open=container_stdin_open,
-            container_tty=container_tty,
-            container_healthcheck=container_healthcheck,
-            container_hostname=container_hostname,
-            container_platform=container_platform,
-            container_working_dir=container_working_dir,
-            container_restart_policy_docker=container_restart_policy_docker,
-            container_volumes_docker=container_volumes_docker,
-            container_ports_docker=container_ports_docker,
-            replicas=replicas,
-            pod_name=pod_name,
-            deploy_name=deploy_name,
-            secret_name=secret_name,
-            configmap_name=configmap_name,
-            image_pull_policy=image_pull_policy,
-            pod_annotations=pod_annotations,
-            pod_node_selector=pod_node_selector,
-            deploy_restart_policy=deploy_restart_policy,
-            deploy_labels=deploy_labels,
-            termination_grace_period_seconds=termination_grace_period_seconds,
-            topology_spread_key=topology_spread_key,
-            topology_spread_max_skew=topology_spread_max_skew,
-            topology_spread_when_unsatisfiable=topology_spread_when_unsatisfiable,
-            create_service=create_service,
-            service_name=service_name,
-            service_type=service_type,
-            service_port=service_port,
-            service_node_port=service_node_port,
-            service_target_port=service_target_port,
-            service_ports=service_ports,
-            service_labels=service_labels,
-            service_annotations=service_annotations,
-            service_health_check_node_port=service_health_check_node_port,
-            service_internal_traffic_policy=service_internal_traffic_policy,
-            service_load_balancer_class=service_load_balancer_class,
-            service_load_balancer_ip=service_load_balancer_ip,
-            service_load_balancer_source_ranges=service_load_balancer_source_ranges,
-            service_allocate_load_balancer_node_ports=service_allocate_load_balancer_node_ports,
-            create_app_service=create_app_service,
-            app_svc_name=app_svc_name,
-            app_svc_type=app_svc_type,
-            app_svc_port=app_svc_port,
-            app_node_port=app_node_port,
-            app_target_port=app_target_port,
-            app_svc_ports=app_svc_ports,
-            app_svc_labels=app_svc_labels,
-            app_svc_annotations=app_svc_annotations,
-            app_svc_health_check_node_port=app_svc_health_check_node_port,
-            app_svc_internal_taffic_policy=app_svc_internal_taffic_policy,
-            app_svc_load_balancer_class=app_svc_load_balancer_class,
-            app_svc_load_balancer_ip=app_svc_load_balancer_ip,
-            app_svc_load_balancer_source_ranges=app_svc_load_balancer_source_ranges,
-            app_svc_allocate_load_balancer_node_ports=app_svc_allocate_load_balancer_node_ports,
-            use_rbac=use_rbac,
-            ns_name=ns_name,
-            namespace=namespace,
-            sa_name=sa_name,
-            service_account=service_account,
-            cr_name=cr_name,
-            cluster_role=cluster_role,
-            crb_name=crb_name,
-            cluster_role_binding=cluster_role_binding,
-            extra_secrets=extra_secrets,
-            extra_configmaps=extra_configmaps,
-            extra_services=extra_services,
-            extra_deployments=extra_deployments,
-            extra_pvs=extra_pvs,
-            extra_pvcs=extra_pvcs,
-            extra_containers=extra_containers,
-            extra_init_containers=extra_init_containers,
-            extra_ports=extra_ports,
-            extra_volumes=extra_volumes,
-            extra_storage_classes=extra_storage_classes,
-            extra_custom_objects=extra_custom_objects,
-            extra_crds=extra_crds,
-            print_env_on_load=print_env_on_load,
-            use_cache=use_cache,
-            load_examples=load_examples,
-            **kwargs,
-        )
+        super().__init__()
+
+        try:
+            self.args: StreamlitAppArgs = StreamlitAppArgs(
+                name=name,
+                version=version,
+                enabled=enabled,
+                image=image,
+                image_name=image_name,
+                image_tag=image_tag,
+                entrypoint=entrypoint,
+                command=command,
+                debug_mode=debug_mode,
+                install_requirements=install_requirements,
+                requirements_file=requirements_file,
+                set_python_path=set_python_path,
+                python_path=python_path,
+                add_python_paths=add_python_paths,
+                env=env,
+                env_file=env_file,
+                secrets=secrets,
+                secrets_file=secrets_file,
+                aws_secrets=aws_secrets,
+                open_container_port=open_container_port,
+                container_port=container_port,
+                container_port_name=container_port_name,
+                container_host_port=container_host_port,
+                mount_workspace=mount_workspace,
+                workspace_volume_name=workspace_volume_name,
+                workspace_volume_type=workspace_volume_type,
+                workspace_dir_container_path=workspace_dir_container_path,
+                add_workspace_name_to_container_path=add_workspace_name_to_container_path,
+                workspace_dir=workspace_dir,
+                container_name=container_name,
+                container_detach=container_detach,
+                container_auto_remove=container_auto_remove,
+                container_remove=container_remove,
+                container_user=container_user,
+                container_stdin_open=container_stdin_open,
+                container_stdout=container_stdout,
+                container_stderr=container_stderr,
+                container_tty=container_tty,
+                container_healthcheck=container_healthcheck,
+                container_hostname=container_hostname,
+                container_platform=container_platform,
+                container_working_dir=container_working_dir,
+                container_labels=container_labels,
+                container_restart_policy=container_restart_policy,
+                container_volumes=container_volumes,
+                container_ports=container_ports,
+                pod_name=pod_name,
+                pod_annotations=pod_annotations,
+                pod_node_selector=pod_node_selector,
+                secret_name=secret_name,
+                configmap_name=configmap_name,
+                replicas=replicas,
+                deploy_name=deploy_name,
+                image_pull_policy=image_pull_policy,
+                deploy_restart_policy=deploy_restart_policy,
+                deploy_labels=deploy_labels,
+                termination_grace_period_seconds=termination_grace_period_seconds,
+                topology_spread_key=topology_spread_key,
+                topology_spread_max_skew=topology_spread_max_skew,
+                topology_spread_when_unsatisfiable=topology_spread_when_unsatisfiable,
+                create_service=create_service,
+                service_name=service_name,
+                service_type=service_type,
+                service_port=service_port,
+                service_node_port=service_node_port,
+                service_target_port=service_target_port,
+                service_ports=service_ports,
+                service_labels=service_labels,
+                service_annotations=service_annotations,
+                service_health_check_node_port=service_health_check_node_port,
+                service_internal_traffic_policy=service_internal_traffic_policy,
+                service_load_balancer_class=service_load_balancer_class,
+                service_load_balancer_ip=service_load_balancer_ip,
+                service_load_balancer_source_ranges=service_load_balancer_source_ranges,
+                service_allocate_load_balancer_node_ports=service_allocate_load_balancer_node_ports,
+                create_ingress=create_ingress,
+                ingress_name=ingress_name,
+                ingress_annotations=ingress_annotations,
+                use_rbac=use_rbac,
+                ns_name=ns_name,
+                namespace=namespace,
+                sa_name=sa_name,
+                service_account=service_account,
+                cr_name=cr_name,
+                cluster_role=cluster_role,
+                crb_name=crb_name,
+                cluster_role_binding=cluster_role_binding,
+                aws_subnets=aws_subnets,
+                aws_security_groups=aws_security_groups,
+                ecs_cluster=ecs_cluster,
+                ecs_launch_type=ecs_launch_type,
+                ecs_task_cpu=ecs_task_cpu,
+                ecs_task_memory=ecs_task_memory,
+                ecs_service_count=ecs_service_count,
+                assign_public_ip=assign_public_ip,
+                ecs_enable_exec=ecs_enable_exec,
+                load_balancer=load_balancer,
+                listener=listener,
+                create_load_balancer=create_load_balancer,
+                load_balancer_protocol=load_balancer_protocol,
+                load_balancer_security_groups=load_balancer_security_groups,
+                load_balancer_port=load_balancer_port,
+                load_balancer_certificate=load_balancer_certificate,
+                load_balancer_certificate_arn=load_balancer_certificate_arn,
+                target_group=target_group,
+                target_group_protocol=target_group_protocol,
+                target_group_port=target_group_port,
+                target_group_type=target_group_type,
+                health_check_protocol=health_check_protocol,
+                health_check_port=health_check_port,
+                health_check_enabled=health_check_enabled,
+                health_check_path=health_check_path,
+                health_check_interval_seconds=health_check_interval_seconds,
+                health_check_timeout_seconds=health_check_timeout_seconds,
+                healthy_threshold_count=healthy_threshold_count,
+                unhealthy_threshold_count=unhealthy_threshold_count,
+                skip_create=skip_create,
+                skip_read=skip_read,
+                skip_update=skip_update,
+                recreate_on_update=recreate_on_update,
+                skip_delete=skip_delete,
+                wait_for_creation=wait_for_creation,
+                wait_for_update=wait_for_update,
+                wait_for_deletion=wait_for_deletion,
+                waiter_delay=waiter_delay,
+                waiter_max_attempts=waiter_max_attempts,
+                save_output=save_output,
+                resource_dir=resource_dir,
+                use_cache=use_cache,
+                print_env_on_load=print_env_on_load,
+                **extra_kwargs,
+            )
+        except Exception as e:
+            logger.error(f"Args for {self.name} are not valid: {e}")
+            raise
```

### Comparing `phidata-1.6.9/phidata/app/traefik/crds.py` & `phidata-1.7.0/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/app/traefik/ingress_route.py` & `phidata-1.7.0/phidata/app/traefik/ingress_route.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     # Configure the service
     service_name: Optional[str] = None
     service_type: ServiceType = ServiceType.LOAD_BALANCER
     service_annotations: Optional[Dict[str, str]] = None
     external_traffic_policy: Optional[Literal["Cluster", "Local"]] = None
 
     # Add env variables to container env
-    env: Optional[Dict[str, str]] = None
+    env: Optional[Dict[str, Any]] = None
     # Read env variables from a file in yaml format
     env_file: Optional[Path] = None
     # Configure the ConfigMap used for env variables that are not Secret
     config_map_name: Optional[str] = None
     # Configure the Secret used for env variables that are Secret
     secret_name: Optional[str] = None
     # Read secrets from a file in yaml format
```

### Comparing `phidata-1.6.9/phidata/app/traefik/router.py` & `phidata-1.7.0/phidata/app/traefik/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,23 +178,23 @@
 
     # K8s configuration
     # NOTE: Only available for Kubernetes
     image_pull_policy: ImagePullPolicy = ImagePullPolicy.IF_NOT_PRESENT
 
     # Container env
     # Add env variables to container env
-    env: Optional[Dict[str, str]] = None
+    env: Optional[Dict[str, Any]] = None
     # Read env variables from a file in yaml format
     env_file: Optional[Path] = None
     # Configure the ConfigMap name used for env variables that are not Secret
     config_map_name: Optional[str] = None
 
     # Container secrets
     # Add secret variables to container env
-    secrets: Optional[Dict[str, str]] = None
+    secrets: Optional[Dict[str, Any]] = None
     # Read secret variables from a file in yaml format
     secrets_file: Optional[Path] = None
     # Read secret variables from AWS Secrets Manager
     aws_secret: Optional[Any] = None
     # Configure the Secret name used for env variables that are Secret
     secret_name: Optional[str] = None
```

### Comparing `phidata-1.6.9/phidata/asset/aws/aws_asset.py` & `phidata-1.7.0/phidata/asset/aws/aws_asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     aws_api_client: Optional[AwsApiClient] = None
 
 
 class AwsAsset(DataAsset):
     def __init__(self) -> None:
         super().__init__()
-        self.args: Optional[AwsAssetArgs] = None
+        self.args: AwsAssetArgs = AwsAssetArgs()
 
     @property
     def aws_region(self) -> Optional[str]:
         # aws_asset not yet initialized
         if self.args is None:
             return None
```

### Comparing `phidata-1.6.9/phidata/asset/data_asset.py` & `phidata-1.7.0/phidata/asset/data_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def __init__(self) -> None:
         super().__init__()
         self.fs: Optional[Any] = None
         self.resource_created: bool = False
         self.resource_updated: bool = False
         self.resource_deleted: bool = False
-        self.args: Optional[DataAssetArgs] = None
+        self.args: DataAssetArgs = DataAssetArgs()
 
     @property
     def phidata_runtime(self) -> Optional[PhidataRuntimeType]:
         # data_asset not yet initialized
         if self.args is None:
             return PhidataRuntimeType.local
```

### Comparing `phidata-1.6.9/phidata/asset/local/file.py` & `phidata-1.7.0/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/asset/local/local_asset.py` & `phidata-1.7.0/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/api_client.py` & `phidata-1.7.0/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/athena/query.py` & `phidata-1.7.0/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/config.py` & `phidata-1.7.0/phidata/aws/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Optional, List, Union
 
+from phidata.app.base_app import BaseApp
 from phidata.app.phidata_app import PhidataApp
 from phidata.app.group import AppGroup, get_apps_from_app_groups
-from phidata.infra.config import InfraConfig
 from phidata.aws.args import AwsArgs
 from phidata.aws.manager import AwsManager
 from phidata.aws.resource.group import AwsResourceGroup
+from phidata.infra.config import InfraConfig
 from phidata.utils.log import logger
 
 
 class AwsConfig(InfraConfig):
     def __init__(
         self,
         env: Optional[str] = "prd",
         version: Optional[str] = None,
         enabled: bool = True,
-        apps: Optional[List[PhidataApp]] = None,
+        apps: Optional[List[Union[BaseApp, PhidataApp]]] = None,
         app_groups: Optional[List[AppGroup]] = None,
         # AwsResourceGroups to deploy
         resources: Optional[Union[AwsResourceGroup, List[AwsResourceGroup]]] = None,
         # Resources dir where aws manifests are stored
         resources_dir: str = "aws",
         # Aws params for this Config
         # Override the aws params from WorkspaceConfig if provided
```

### Comparing `phidata-1.6.9/phidata/aws/create/iam/eks_admin_role.py` & `phidata-1.7.0/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/create/iam/role.py` & `phidata-1.7.0/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/enums/manager_status.py` & `phidata-1.7.0/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/manager.py` & `phidata-1.7.0/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/acm/certificate.py` & `phidata-1.7.0/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/athena/query.py` & `phidata-1.7.0/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/base.py` & `phidata-1.7.0/phidata/aws/resource/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional
+from typing import Any, Optional, Dict
 
 from phidata.constants import AWS_REGION_ENV_VAR, AWS_PROFILE_ENV_VAR
 from phidata.infra.resource import InfraResource
 from phidata.aws.api_client import AwsApiClient
 from phidata.utils.cli_console import print_info
 from phidata.utils.log import logger
 
@@ -115,20 +115,25 @@
             print_info(
                 f"{self.get_resource_type()}: {self.get_resource_name()} already active."
             )
         # Step 4: Create the resource
         else:
             self.resource_available = self._create(client)
 
-        # Step 5: Run post create steps
+        # Step 5: Save resource to file
+        if self.save_output:
+            self.save_resource_file()
+
+        # Step 6: Run post create steps
         if self.resource_available:
             logger.debug(
                 f"Running post-create steps for {self.get_resource_type()}: {self.get_resource_name()}."
             )
             return self.post_create(client)
+
         return self.resource_available
 
     def post_create(self, aws_client: AwsApiClient) -> bool:
         # return True because this function is not used for most resources
         return True
 
     def _read(self, aws_client: AwsApiClient) -> Any:
@@ -141,15 +146,15 @@
         Args:
             aws_client: The AwsApiClient for the current Cluster
         """
         # Step 1: Check if resource is valid
         if not self.is_valid():
             return None
 
-        # Step 2: Use cached value is availabe
+        # Step 2: Use cached value is available
         if self.use_cache and self.active_resource is not None:
             return self.active_resource
 
         # Step 3: Skip resource creation if skip_read = True
         if self.skip_read:
             print_info(f"Skipping read: {self.get_resource_name()}")
             return True
@@ -183,20 +188,25 @@
             self.resource_updated = self._update(client)
         else:
             print_info(
                 f"{self.get_resource_type()}: {self.get_resource_name()} does not exist."
             )
             return True
 
-        # Step 4: Run post update steps
+        # Step 5: Save resource to file
+        if self.save_output:
+            self.save_resource_file()
+
+        # Step 5: Run post update steps
         if self.resource_updated:
             logger.debug(
                 f"Running post-update steps for {self.get_resource_type()}: {self.get_resource_name()}."
             )
             return self.post_update(client)
+
         return self.resource_updated
 
     def post_update(self, aws_client: AwsApiClient) -> bool:
         # return True because this function is not used for most resources
         return True
 
     def _delete(self, aws_client: AwsApiClient) -> Any:
@@ -224,20 +234,25 @@
             self.resource_deleted = self._delete(client)
         else:
             print_info(
                 f"{self.get_resource_type()}: {self.get_resource_name()} does not exist."
             )
             return True
 
-        # Step 4: Run post delete steps
+        # Step 4: Delete resource file
+        if self.save_output:
+            self.delete_resource_file()
+
+        # Step 5: Run post delete steps
         if self.resource_deleted:
             logger.debug(
                 f"Running post-delete steps for {self.get_resource_type()}: {self.get_resource_name()}."
             )
             return self.post_delete(client)
+
         return self.resource_deleted
 
     def post_delete(self, aws_client: AwsApiClient) -> bool:
         # return True because this function is not used for most resources
         return True
 
     def is_active(self, aws_client: AwsApiClient) -> bool:
```

### Comparing `phidata-1.6.9/phidata/aws/resource/cloudformation/stack.py` & `phidata-1.7.0/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/ec2/subnet.py` & `phidata-1.7.0/phidata/aws/resource/ec2/subnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from phidata.aws.resource.base import AwsResource
 from phidata.utils.cli_console import print_error
 from phidata.utils.log import logger
 
 
 class Subnet(AwsResource):
     """
-    # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#subnet
+    Reference:
+        - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#subnet
     """
 
     resource_type = "Subnet"
     service_name = "ec2"
 
     # Subnet id
     id: str
@@ -53,7 +54,24 @@
             logger.debug(f"VPC ID for {self.id}: {vpc_id}")
             return vpc_id
         except ClientError as ce:
             logger.debug(f"ClientError: {ce}")
         except Exception as e:
             print_error(f"Error reading {self.get_resource_type()}: {e}")
         return None
+
+
+def get_vpc_id_from_subnet_ids(
+    subnet_ids: Optional[list[str]], aws_client: Optional[AwsApiClient] = None
+) -> Optional[str]:
+    if subnet_ids is None:
+        return None
+
+    # Get VPC ID from subnets
+    vpc_ids = set()
+    for subnet in subnet_ids:
+        _vpc = Subnet(id=subnet).get_vpc_id(aws_client)
+        vpc_ids.add(_vpc)
+    if len(vpc_ids) > 1:
+        raise ValueError("Subnets must be in the same VPC")
+    vpc_id = vpc_ids.pop() if len(vpc_ids) == 1 else None
+    return vpc_id
```

### Comparing `phidata-1.6.9/phidata/aws/resource/ec2/volume.py` & `phidata-1.7.0/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/ecs/cluster.py` & `phidata-1.7.0/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/ecs/container.py` & `phidata-1.7.0/phidata/aws/resource/ecs/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from typing import Optional, Any, Dict, List
+from typing import Optional, Any, Dict, List, Union
 
 from phidata.aws.resource.base import AwsResource
+from phidata.aws.resource.secret.manager import SecretsManager
+from phidata.aws.resource.secret.reader import read_secrets
 from phidata.utils.log import logger
 
 
 class EcsContainer(AwsResource):
     """
-    # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html
+    Reference: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html
     """
 
     resource_type = "EcsContainer"
     service_name = "ecs"
 
     # The name of a container.
     # If you're linking multiple containers together in a task definition, the name of one container can be entered in
@@ -38,16 +40,18 @@
     essential: Optional[bool] = None
     # The entry point that's passed to the container.
     entry_point: Optional[List[str]] = None
     # The command that's passed to the container.
     command: Optional[List[str]] = None
     # The environment variables to pass to a container.
     environment: Optional[List[Dict[str, Any]]] = None
-    # The entry point that's passed to the container.
+    # A list of files containing the environment variables to pass to a container.
     environment_files: Optional[List[Dict[str, Any]]] = None
+    # Read environment variables from AWS Secrets.
+    env_from_secrets: Optional[Union[SecretsManager, List[SecretsManager]]] = None
     # The mount points for data volumes in your container.
     mount_points: Optional[List[Dict[str, Any]]] = None
     # Data volumes to mount from another container.
     volumes_from: Optional[List[Dict[str, Any]]] = None
     # Linux-specific modifications that are applied to the container, such as Linux kernel capabilities.
     linux_parameters: Optional[Dict[str, Any]] = None
     # The secrets to pass to the container.
@@ -82,14 +86,20 @@
     health_check: Optional[Dict[str, Any]] = None
     system_controls: Optional[List[Dict[str, Any]]] = None
     resource_requirements: Optional[List[Dict[str, Any]]] = None
     firelens_configuration: Optional[Dict[str, Any]] = None
 
     def get_container_definition(self) -> Dict[str, Any]:
         container_definition: Dict[str, Any] = {}
+
+        # Build container environment
+        container_environment: List[Dict[str, Any]] = self.build_container_environment()
+        if container_environment is not None:
+            container_definition["environment"] = container_environment
+
         if self.name is not None:
             container_definition["name"] = self.name
         if self.image is not None:
             container_definition["image"] = self.image
         if self.repository_credentials is not None:
             container_definition["repositoryCredentials"] = self.repository_credentials
         if self.cpu is not None:
@@ -104,16 +114,14 @@
             container_definition["portMappings"] = self.port_mappings
         if self.essential is not None:
             container_definition["essential"] = self.essential
         if self.entry_point is not None:
             container_definition["entryPoint"] = self.entry_point
         if self.command is not None:
             container_definition["command"] = self.command
-        if self.environment is not None:
-            container_definition["environment"] = self.environment
         if self.environment_files is not None:
             container_definition["environmentFiles"] = self.environment_files
         if self.mount_points is not None:
             container_definition["mountPoints"] = self.mount_points
         if self.volumes_from is not None:
             container_definition["volumesFrom"] = self.volumes_from
         if self.linux_parameters is not None:
@@ -165,14 +173,48 @@
         if self.resource_requirements is not None:
             container_definition["resourceRequirements"] = self.resource_requirements
         if self.firelens_configuration is not None:
             container_definition["firelensConfiguration"] = self.firelens_configuration
 
         return container_definition
 
+    def build_container_environment(self) -> List[Dict[str, Any]]:
+        logger.debug("Building container environment")
+        container_environment: List[Dict[str, Any]] = []
+        if self.environment is not None:
+            from phidata.resource.reference import Reference
+
+            for env in self.environment:
+                env_value = env.get("value", None)
+                if isinstance(env_value, Reference):
+                    env_name = env.get("name", None)
+                    logger.debug(f"{env_name} is a Reference")
+                    try:
+                        env_val = env_value.get_reference()
+                        try:
+                            env_val_str = str(env_val)
+                            container_environment.append(
+                                {"name": env_name, "value": env_val_str}
+                            )
+                        except Exception as e:
+                            logger.error(
+                                f"Error while converting {env_val} to str: {e}"
+                            )
+                    except Exception as e:
+                        logger.error(f"Error while getting {env_name}: {e}")
+                else:
+                    container_environment.append(env)
+        if self.env_from_secrets is not None:
+            secrets: Dict[str, Any] = read_secrets(self.env_from_secrets)
+            for secret_name, secret_value in secrets.items():
+                container_environment.append(
+                    {"name": secret_name, "value": secret_value}
+                )
+        return container_environment
+
     def container_definition_up_to_date(
         self, container_definition: Dict[str, Any]
     ) -> bool:
         """This is not working"""
 
         from phidata.utils.compare import compare_dicts
```

### Comparing `phidata-1.6.9/phidata/aws/resource/ecs/service.py` & `phidata-1.7.0/phidata/aws/resource/elasticache/cluster.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,363 +1,338 @@
-from typing import Optional, Any, Dict, List, Literal, Union
+from pathlib import Path
+from typing import Optional, Any, Dict, List
+from typing_extensions import Literal
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
-from phidata.aws.resource.ecs.cluster import EcsCluster
-from phidata.aws.resource.ecs.task_definition import EcsTaskDefinition
-from phidata.aws.resource.elb.target_group import TargetGroup
-from phidata.utils.cli_console import print_info, print_error
+from phidata.aws.resource.ec2.security_group import SecurityGroup
+from phidata.aws.resource.elasticache.subnet_group import CacheSubnetGroup
+from phidata.utils.cli_console import print_info, print_error, print_warning
 from phidata.utils.log import logger
 
 
-class EcsService(AwsResource):
+class CacheCluster(AwsResource):
     """
-    # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html
+    Reference:
+    - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html
     """
 
-    resource_type = "EcsService"
-    service_name = "ecs"
+    resource_type = "CacheCluster"
+    service_name = "elasticache"
 
-    # Name for the service.
+    # Name of the cluster.
     name: str
-    # Name for the service.
-    # Use name if not provided.
-    ecs_service_name: Optional[str] = None
-
-    # EcsCluster for the service.
-    # Can be
-    # - string: The short name or full Amazon Resource Name (ARN) of the cluster
-    # - EcsCluster
-    # If you do not specify a cluster, the default cluster is assumed.
-    cluster: Optional[Union[EcsCluster, str]] = None
-
-    # EcsTaskDefinition for the service.
-    # Can be
-    # - string: The family and revision (family:revision ) or full ARN of the task definition.
-    # - EcsTaskDefinition
-    # If a revision isn't specified, the latest ACTIVE revision is used.
-    task_definition: Optional[Union[EcsTaskDefinition, str]] = None
-
-    # A load balancer object representing the load balancers to use with your service.
-    load_balancers: Optional[List[Dict[str, Any]]] = None
-
-    # We can generate the load_balancers dict using
-    # the target_group, target_container_name and target_container_port
-    # Target group to attach to a service.
-    target_group: Optional[TargetGroup] = None
-    # Target container name for the service.
-    target_container_name: Optional[str] = None
-    target_container_port: Optional[int] = None
-
-    # The details of the service discovery registries to assign to this service.
-    service_registries: Optional[List[Dict[str, Any]]] = None
-    # The number of instantiations of the specified task definition to place and keep running on your cluster.
-    # This is required if schedulingStrategy is REPLICA or isn't specified.
-    # If schedulingStrategy is DAEMON then this isn't required.
-    desired_count: Optional[int] = None
-    # An identifier that you provide to ensure the idempotency of the request. It must be unique and is case-sensitive.
-    client_token: Optional[str] = None
-    # The infrastructure that you run your service on.
-    launch_type: Optional[Union[str, Literal["EC2", "FARGATE", "EXTERNAL"]]] = None
-    # The capacity provider strategy to use for the service.
-    capacity_provider_strategy: Optional[List[Dict[str, Any]]] = None
-    platform_version: Optional[str] = None
-    role: Optional[str] = None
-    deployment_configuration: Optional[Dict[str, Any]] = None
-    placement_constraints: Optional[List[Dict[str, Any]]] = None
-    placement_strategy: Optional[List[Dict[str, Any]]] = None
-    network_configuration: Optional[Dict[str, Any]] = None
-    health_check_grace_period_seconds: Optional[int] = None
-    scheduling_strategy: Optional[Literal["REPLICA", "DAEMON"]] = None
-    deployment_controller: Optional[Dict[str, Any]] = None
-    tags: Optional[List[Dict[str, Any]]] = None
-    enable_ecsmanaged_tags: Optional[bool] = None
-    propagate_tags: Optional[Literal["TASK_DEFINITION", "SERVICE", "NONE"]] = None
-    enable_execute_command: Optional[bool] = None
-
-    force_delete: Optional[bool] = None
-    # Force a new deployment of the service on update.
-    # By default, deployments aren't forced.
-    # You can use this option to start a new deployment with no service
-    # definition changes. For example, you can update a service's
-    # tasks to use a newer Docker image with the same
-    # image/tag combination (my_image:latest ) or
-    # to roll Fargate tasks onto a newer platform version.
-    force_new_deployment: Optional[bool] = None
-
-    def get_ecs_service_name(self):
-        return self.ecs_service_name or self.name
-
-    def get_ecs_cluster_name(self):
-        if self.cluster is not None:
-            if isinstance(self.cluster, EcsCluster):
-                return self.cluster.get_ecs_cluster_name()
-            else:
-                return self.cluster
-
-    def get_ecs_task_definition(self):
-        if self.task_definition is not None:
-            if isinstance(self.task_definition, EcsTaskDefinition):
-                return self.task_definition.get_task_family()
-            else:
-                return self.task_definition
+    # The node group (shard) identifier. This parameter is stored as a lowercase string.
+    # If None, use the name as the cache_cluster_id
+    # Constraints:
+    #   A name must contain from 1 to 50 alphanumeric characters or hyphens.
+    #   The first character must be a letter.
+    #   A name cannot end with a hyphen or contain two consecutive hyphens.
+    cache_cluster_id: Optional[str] = None
+    # The name of the cache engine to be used for this cluster.
+    engine: Literal["memcached", "redis"]
+
+    # Compute and memory capacity of the nodes in the node group (shard).
+    cache_node_type: str
+    # The initial number of cache nodes that the cluster has.
+    # For clusters running Redis, this value must be 1.
+    # For clusters running Memcached, this value must be between 1 and 40.
+    num_cache_nodes: int
+
+    # The ID of the replication group to which this cluster should belong.
+    # If this parameter is specified, the cluster is added to the specified replication group as a read replica;
+    # otherwise, the cluster is a standalone primary that is not part of any replication group.
+    replication_group_id: Optional[str] = None
+    # Specifies whether the nodes in this Memcached cluster are created in a single Availability Zone or
+    # created across multiple Availability Zones in the cluster's region.
+    # This parameter is only supported for Memcached clusters.
+    az_mode: Optional[Literal["single-az", "cross-az"]] = None
+    # The EC2 Availability Zone in which the cluster is created.
+    # All nodes belonging to this cluster are placed in the preferred Availability Zone. If you want to create your
+    # nodes across multiple Availability Zones, use PreferredAvailabilityZones .
+    # Default: System chosen Availability Zone.
+    preferred_availability_zone: Optional[str] = None
+    # A list of the Availability Zones in which cache nodes are created. The order of the zones is not important.
+    # This option is only supported on Memcached.
+    preferred_availability_zones: Optional[List[str]] = None
+    # The version number of the cache engine to be used for this cluster.
+    engine_version: Optional[str] = None
+    cache_parameter_group_name: Optional[str] = None
+
+    # The name of the subnet group to be used for the cluster.
+    cache_subnet_group_name: Optional[str] = None
+    # If cache_subnet_group_name is None,
+    # Read the cache_subnet_group_name from cache_subnet_group
+    cache_subnet_group: Optional[CacheSubnetGroup] = None
+
+    # A list of security group names to associate with this cluster.
+    # Use this parameter only when you are creating a cluster outside of an Amazon Virtual Private Cloud (Amazon VPC).
+    cache_security_group_names: Optional[List[str]] = None
+    # One or more VPC security groups associated with the cluster.
+    # Use this parameter only when you are creating a cluster in an Amazon Virtual Private Cloud (Amazon VPC).
+    security_group_ids: Optional[List[str]] = None
+    # If security_group_ids is None
+    # Read the security_group_id from security_groups
+    security_groups: Optional[List[SecurityGroup]] = None
+
+    tags: Optional[List[Dict[str, str]]] = None
+    snapshot_arns: Optional[List[str]] = None
+    snapshot_name: Optional[str] = None
+    preferred_maintenance_window: Optional[str] = None
+    # The version number of the cache engine to be used for this cluster.
+    port: Optional[int] = None
+    notification_topic_arn: Optional[str] = None
+    auto_minor_version_upgrade: Optional[bool] = None
+    snapshot_retention_limit: Optional[int] = None
+    snapshot_window: Optional[str] = None
+    # The password used to access a password protected server.
+    # Password constraints:
+    # - Must be only printable ASCII characters.
+    # - Must be at least 16 characters and no more than 128 characters in length.
+    # - The only permitted printable special characters are !, &, #, $, ^, <, >, and -.
+    # Other printable special characters cannot be used in the AUTH token.
+    # - For more information, see AUTH password at http://redis.io/commands/AUTH.
+    # Provide AUTH_TOKEN here or as AUTH_TOKEN in secrets_file
+    auth_token: Optional[str] = None
+    outpost_mode: Optional[Literal["single-outpost", "cross-outpost"]] = None
+    preferred_outpost_arn: Optional[str] = None
+    preferred_outpost_arns: Optional[List[str]] = None
+    log_delivery_configurations: Optional[List[Dict[str, Any]]] = None
+    transit_encryption_enabled: Optional[bool] = None
+    network_type: Optional[Literal["ipv4", "ipv6", "dual_stack"]] = None
+    ip_discovery: Optional[Literal["ipv4", "ipv6"]] = None
+
+    # The user-supplied name of a final cluster snapshot
+    final_snapshot_identifier: Optional[str] = None
+
+    # Read secrets from a file in yaml format
+    secrets_file: Optional[Path] = None
+
+    def get_cache_cluster_id(self):
+        return self.cache_cluster_id or self.name
+
+    def get_auth_token(self) -> Optional[str]:
+        auth_token = self.auth_token
+        if auth_token is None and self.secrets_file is not None:
+            # read from secrets_file
+            secret_data = self.get_secret_data()
+            if secret_data is not None:
+                auth_token = secret_data.get("AUTH_TOKEN", auth_token)
+        return auth_token
 
     def _create(self, aws_client: AwsApiClient) -> bool:
-        """Create EcsService"""
+        """Creates the CacheCluster
+
+        Args:
+            aws_client: The AwsApiClient for the current cluster
+        """
         print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
 
         # create a dict of args which are not null, otherwise aws type validation fails
         not_null_args: Dict[str, Any] = {}
 
-        cluster_name = self.get_ecs_cluster_name()
-        if cluster_name is not None:
-            not_null_args["cluster"] = cluster_name
-        if self.service_registries is not None:
-            not_null_args["serviceRegistries"] = self.service_registries
-        if self.desired_count is not None:
-            not_null_args["desiredCount"] = self.desired_count
-        if self.client_token is not None:
-            not_null_args["clientToken"] = self.client_token
-        if self.launch_type is not None:
-            not_null_args["launchType"] = self.launch_type
-        if self.capacity_provider_strategy is not None:
-            not_null_args["capacityProviderStrategy"] = self.capacity_provider_strategy
-        if self.platform_version is not None:
-            not_null_args["platformVersion"] = self.platform_version
-        if self.role is not None:
-            not_null_args["role"] = self.role
-        if self.deployment_configuration is not None:
-            not_null_args["deploymentConfiguration"] = self.deployment_configuration
-        if self.placement_constraints is not None:
-            not_null_args["placementConstraints"] = self.placement_constraints
-        if self.placement_strategy is not None:
-            not_null_args["placementStrategy"] = self.placement_strategy
-        if self.network_configuration is not None:
-            not_null_args["networkConfiguration"] = self.network_configuration
-        if self.health_check_grace_period_seconds is not None:
+        # Get the CacheSubnetGroupName
+        cache_subnet_group_name = self.cache_subnet_group_name
+        if cache_subnet_group_name is None and self.cache_subnet_group is not None:
+            cache_subnet_group_name = self.cache_subnet_group.name
+            logger.debug(f"Using CacheSubnetGroup: {cache_subnet_group_name}")
+        if cache_subnet_group_name is not None:
+            not_null_args["CacheSubnetGroupName"] = cache_subnet_group_name
+
+        security_group_ids = self.security_group_ids
+        if security_group_ids is None and self.security_groups is not None:
+            sg_ids = []
+            for sg in self.security_groups:
+                sg_id = sg.get_security_group_id(aws_client)
+                if sg_id is not None:
+                    sg_ids.append(sg_id)
+            if len(sg_ids) > 0:
+                security_group_ids = sg_ids
+                logger.debug(f"Using SecurityGroups: {security_group_ids}")
+        if security_group_ids is not None:
+            not_null_args["SecurityGroupIds"] = security_group_ids
+
+        if self.replication_group_id is not None:
+            not_null_args["ReplicationGroupId"] = self.replication_group_id
+        if self.az_mode is not None:
+            not_null_args["AZMode"] = self.az_mode
+        if self.preferred_availability_zone is not None:
+            not_null_args[
+                "PreferredAvailabilityZone"
+            ] = self.preferred_availability_zone
+        if self.preferred_availability_zones is not None:
             not_null_args[
-                "healthCheckGracePeriodSeconds"
-            ] = self.health_check_grace_period_seconds
-        if self.scheduling_strategy is not None:
-            not_null_args["schedulingStrategy"] = self.scheduling_strategy
-        if self.deployment_controller is not None:
-            not_null_args["deploymentController"] = self.deployment_controller
+                "PreferredAvailabilityZones"
+            ] = self.preferred_availability_zones
+        if self.num_cache_nodes is not None:
+            not_null_args["NumCacheNodes"] = self.num_cache_nodes
+        if self.cache_node_type is not None:
+            not_null_args["CacheNodeType"] = self.cache_node_type
+        if self.engine is not None:
+            not_null_args["Engine"] = self.engine
+        if self.engine_version is not None:
+            not_null_args["EngineVersion"] = self.engine_version
+        if self.cache_parameter_group_name is not None:
+            not_null_args["CacheParameterGroupName"] = self.cache_parameter_group_name
+        if self.cache_security_group_names is not None:
+            not_null_args["CacheSecurityGroupNames"] = self.cache_security_group_names
         if self.tags is not None:
-            not_null_args["tags"] = self.tags
-        if self.enable_ecsmanaged_tags is not None:
-            not_null_args["enableECSManagedTags"] = self.enable_ecsmanaged_tags
-        if self.propagate_tags is not None:
-            not_null_args["propagateTags"] = self.propagate_tags
-        if self.enable_execute_command is not None:
-            not_null_args["enableExecuteCommand"] = self.enable_execute_command
-
-        if self.load_balancers is not None:
-            not_null_args["loadBalancers"] = self.load_balancers
-        elif self.target_group is not None and self.target_container_name is not None:
-            not_null_args["loadBalancers"] = [
-                {
-                    "targetGroupArn": self.target_group.get_arn(aws_client),
-                    "containerName": self.target_container_name,
-                    "containerPort": self.target_container_port,
-                }
-            ]
+            not_null_args["Tags"] = self.tags
+        if self.snapshot_arns is not None:
+            not_null_args["SnapshotArns"] = self.snapshot_arns
+        if self.snapshot_name is not None:
+            not_null_args["SnapshotName"] = self.snapshot_name
+        if self.preferred_maintenance_window is not None:
+            not_null_args[
+                "PreferredMaintenanceWindow"
+            ] = self.preferred_maintenance_window
+        if self.port is not None:
+            not_null_args["Port"] = self.port
+        if self.notification_topic_arn is not None:
+            not_null_args["NotificationTopicArn"] = self.notification_topic_arn
+        if self.auto_minor_version_upgrade is not None:
+            not_null_args["AutoMinorVersionUpgrade"] = self.auto_minor_version_upgrade
+        if self.snapshot_retention_limit is not None:
+            not_null_args["SnapshotRetentionLimit"] = self.snapshot_retention_limit
+        if self.snapshot_window is not None:
+            not_null_args["SnapshotWindow"] = self.snapshot_window
+        if self.auth_token is not None:
+            not_null_args["AuthToken"] = self.get_auth_token()
+        if self.outpost_mode is not None:
+            not_null_args["OutpostMode"] = self.outpost_mode
+        if self.preferred_outpost_arn is not None:
+            not_null_args["PreferredOutpostArn"] = self.preferred_outpost_arn
+        if self.preferred_outpost_arns is not None:
+            not_null_args["PreferredOutpostArns"] = self.preferred_outpost_arns
+        if self.log_delivery_configurations is not None:
+            not_null_args[
+                "LogDeliveryConfigurations"
+            ] = self.log_delivery_configurations
+        if self.transit_encryption_enabled is not None:
+            not_null_args["TransitEncryptionEnabled"] = self.transit_encryption_enabled
+        if self.network_type is not None:
+            not_null_args["NetworkType"] = self.network_type
+        if self.ip_discovery is not None:
+            not_null_args["IpDiscovery"] = self.ip_discovery
 
-        # Register EcsService
+        # Create CacheCluster
         service_client = self.get_service_client(aws_client)
         try:
-            create_response = service_client.create_service(
-                serviceName=self.get_ecs_service_name(),
-                taskDefinition=self.get_ecs_task_definition(),
+            create_response = service_client.create_cache_cluster(
+                CacheClusterId=self.get_cache_cluster_id(),
                 **not_null_args,
             )
-            logger.debug(f"EcsService: {create_response}")
-            resource_dict = create_response.get("service", {})
+            logger.debug(f"CacheCluster: {create_response}")
+            resource_dict = create_response.get("CacheCluster", {})
 
             # Validate resource creation
             if resource_dict is not None:
-                print_info(f"EcsService created: {self.get_resource_name()}")
+                print_info(f"CacheCluster created: {self.get_cache_cluster_id()}")
                 self.active_resource = create_response
                 return True
         except Exception as e:
             print_error(f"{self.get_resource_type()} could not be created.")
             print_error(e)
         return False
 
     def post_create(self, aws_client: AwsApiClient) -> bool:
-        # Wait for EcsService to be created
+        # Wait for CacheCluster to be created
         if self.wait_for_creation:
             try:
-                cluster_name = self.get_ecs_cluster_name()
-                if cluster_name is not None:
-                    print_info(f"Waiting for {self.get_resource_type()} to be stable.")
-                    waiter = self.get_service_client(aws_client).get_waiter(
-                        "services_stable"
-                    )
-                    waiter.wait(
-                        cluster=cluster_name,
-                        services=[self.get_ecs_service_name()],
-                        WaiterConfig={
-                            "Delay": self.waiter_delay,
-                            "MaxAttempts": self.waiter_max_attempts,
-                        },
-                    )
-                else:
-                    logger.warning("Skipping waiter, no Service found")
+                print_info(f"Waiting for {self.get_resource_type()} to be active.")
+                waiter = self.get_service_client(aws_client).get_waiter(
+                    "cache_cluster_available"
+                )
+                waiter.wait(
+                    CacheClusterId=self.get_cache_cluster_id(),
+                    WaiterConfig={
+                        "Delay": self.waiter_delay,
+                        "MaxAttempts": self.waiter_max_attempts,
+                    },
+                )
             except Exception as e:
                 print_error("Waiter failed.")
                 print_error(e)
         return True
 
     def _read(self, aws_client: AwsApiClient) -> Optional[Any]:
-        """Read EcsService"""
-        from botocore.exceptions import ClientError
+        """Returns the CacheCluster
 
+        Args:
+            aws_client: The AwsApiClient for the current cluster
+        """
         logger.debug(f"Reading {self.get_resource_type()}: {self.get_resource_name()}")
 
-        # create a dict of args which are not null, otherwise aws type validation fails
-        not_null_args: Dict[str, Any] = {}
-
-        cluster_name = self.get_ecs_cluster_name()
-        if cluster_name is not None:
-            not_null_args["cluster"] = cluster_name
+        from botocore.exceptions import ClientError
 
         service_client = self.get_service_client(aws_client)
         try:
-            service_name = self.get_ecs_service_name()
-            describe_response = service_client.describe_services(
-                services=[service_name], **not_null_args
+            cache_cluster_id = self.get_cache_cluster_id()
+            describe_response = service_client.describe_cache_clusters(
+                CacheClusterId=cache_cluster_id
             )
-            logger.debug(f"EcsService: {describe_response}")
-            resource_list = describe_response.get("services", None)
+            logger.debug(f"CacheCluster: {describe_response}")
+            resource_list = describe_response.get("CacheClusters", None)
 
             if resource_list is not None and isinstance(resource_list, list):
                 for resource in resource_list:
-                    _service_name = resource.get("serviceName", None)
-                    if _service_name == service_name:
-                        _service_status = resource.get("status", None)
-                        if _service_status == "ACTIVE":
-                            self.active_resource = resource
-                            break
+                    _cluster_identifier = resource.get("CacheClusterId", None)
+                    if _cluster_identifier == cache_cluster_id:
+                        self.active_resource = resource
+                        break
         except ClientError as ce:
             logger.debug(f"ClientError: {ce}")
         except Exception as e:
             print_error(f"Error reading {self.get_resource_type()}.")
             print_error(e)
         return self.active_resource
 
     def _delete(self, aws_client: AwsApiClient) -> bool:
-        """Delete EcsService"""
+        """Deletes the CacheCluster
+
+        Args:
+            aws_client: The AwsApiClient for the current cluster
+        """
         print_info(f"Deleting {self.get_resource_type()}: {self.get_resource_name()}")
 
         # create a dict of args which are not null, otherwise aws type validation fails
         not_null_args: Dict[str, Any] = {}
-
-        cluster_name = self.get_ecs_cluster_name()
-        if cluster_name is not None:
-            not_null_args["cluster"] = cluster_name
-        if self.force_delete is not None:
-            not_null_args["force"] = self.force_delete
+        if self.final_snapshot_identifier:
+            not_null_args["FinalSnapshotIdentifier"] = self.final_snapshot_identifier
 
         service_client = self.get_service_client(aws_client)
         self.active_resource = None
         try:
-            delete_response = service_client.delete_service(
-                service=self.get_ecs_service_name(),
+            delete_response = service_client.delete_cache_cluster(
+                CacheClusterId=self.get_cache_cluster_id(),
                 **not_null_args,
             )
-            logger.debug(f"EcsService: {delete_response}")
+            logger.debug(f"CacheCluster: {delete_response}")
             print_info(
                 f"{self.get_resource_type()}: {self.get_resource_name()} deleted"
             )
             return True
         except Exception as e:
             print_error(f"{self.get_resource_type()} could not be deleted.")
             print_error("Please try again or delete resources manually.")
             print_error(e)
         return False
 
     def post_delete(self, aws_client: AwsApiClient) -> bool:
-        # Wait for EcsService to be deleted
+        # Wait for CacheCluster to be deleted
         if self.wait_for_deletion:
             try:
-                cluster_name = self.get_ecs_cluster_name()
-                if cluster_name is not None:
-                    print_info(f"Waiting for {self.get_resource_type()} to be deleted.")
-                    waiter = self.get_service_client(aws_client).get_waiter(
-                        "services_inactive"
-                    )
-                    waiter.wait(
-                        cluster=cluster_name,
-                        services=[self.get_ecs_service_name()],
-                        WaiterConfig={
-                            "Delay": self.waiter_delay,
-                            "MaxAttempts": self.waiter_max_attempts,
-                        },
-                    )
-                else:
-                    logger.warning("Skipping waiter, no Service found")
+                print_info(f"Waiting for {self.get_resource_type()} to be deleted.")
+                waiter = self.get_service_client(aws_client).get_waiter(
+                    "cache_cluster_deleted"
+                )
+                waiter.wait(
+                    CacheClusterId=self.get_cache_cluster_id(),
+                    WaiterConfig={
+                        "Delay": self.waiter_delay,
+                        "MaxAttempts": self.waiter_max_attempts,
+                    },
+                )
             except Exception as e:
                 print_error("Waiter failed.")
                 print_error(e)
         return True
-
-    def _update(self, aws_client: AwsApiClient) -> bool:
-        """Update EcsService"""
-        print_info(f"Updating {self.get_resource_type()}: {self.get_resource_name()}")
-
-        # create a dict of args which are not null, otherwise aws type validation fails
-        not_null_args: Dict[str, Any] = {}
-
-        cluster_name = self.get_ecs_cluster_name()
-        if cluster_name is not None:
-            not_null_args["cluster"] = cluster_name
-        if self.desired_count is not None:
-            not_null_args["desiredCount"] = self.desired_count
-        if self.capacity_provider_strategy is not None:
-            not_null_args["capacityProviderStrategy"] = self.capacity_provider_strategy
-        if self.deployment_configuration is not None:
-            not_null_args["deploymentConfiguration"] = self.deployment_configuration
-        if self.network_configuration is not None:
-            not_null_args["networkConfiguration"] = self.network_configuration
-        if self.placement_constraints is not None:
-            not_null_args["placementConstraints"] = self.placement_constraints
-        if self.placement_strategy is not None:
-            not_null_args["placementStrategy"] = self.placement_strategy
-        if self.platform_version is not None:
-            not_null_args["platformVersion"] = self.platform_version
-        if self.force_new_deployment is not None:
-            not_null_args["forceNewDeployment"] = self.force_new_deployment
-        if self.health_check_grace_period_seconds is not None:
-            not_null_args[
-                "healthCheckGracePeriodSeconds"
-            ] = self.health_check_grace_period_seconds
-        if self.enable_execute_command is not None:
-            not_null_args["enableExecuteCommand"] = self.enable_execute_command
-        if self.enable_ecsmanaged_tags is not None:
-            not_null_args["enableECSManagedTags"] = self.enable_ecsmanaged_tags
-        if self.load_balancers is not None:
-            not_null_args["loadBalancers"] = self.load_balancers
-        if self.propagate_tags is not None:
-            not_null_args["propagateTags"] = self.propagate_tags
-        if self.service_registries is not None:
-            not_null_args["serviceRegistries"] = self.service_registries
-
-        # Update EcsService
-        service_client = self.get_service_client(aws_client)
-        try:
-            update_response = service_client.update_service(
-                service=self.get_ecs_service_name(),
-                taskDefinition=self.get_ecs_task_definition(),
-                **not_null_args,
-            )
-            logger.debug(f"EcsService: {update_response}")
-            resource_dict = update_response.get("service", {})
-
-            # Validate resource creation
-            if resource_dict is not None:
-                print_info(f"EcsService updated: {self.get_resource_name()}")
-                self.active_resource = update_response
-                return True
-        except Exception as e:
-            print_error(f"{self.get_resource_type()} could not be updated.")
-            print_error(e)
-        return False
```

### Comparing `phidata-1.6.9/phidata/aws/resource/ecs/task_definition.py` & `phidata-1.7.0/phidata/aws/resource/ecs/task_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from textwrap import dedent
-from typing import Optional, Any, Dict, List, Literal
+from typing import Optional, Any, Dict, List
+from typing_extensions import Literal
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
 from phidata.aws.resource.ecs.container import EcsContainer
 from phidata.aws.resource.ecs.volume import EcsVolume
 from phidata.aws.resource.iam.role import IamRole
 from phidata.aws.resource.iam.policy import IamPolicy
 from phidata.utils.cli_console import print_info, print_error
 from phidata.utils.log import logger
 
 
 class EcsTaskDefinition(AwsResource):
     """
-    # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html
+    Reference: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs/client/register_task_definition.html
     """
 
-    resource_type = "EcsTaskDefinition"
+    resource_type = "TaskDefinition"
     service_name = "ecs"
 
     # Name of the task definition.
     # Used as task definition family.
     name: str
     # The family for a task definition.
     # Use name as family if not provided
@@ -50,28 +51,34 @@
     # The short name or full Amazon Resource Name (ARN) of the IAM role that containers in this task can assume.
     task_role_arn: Optional[str] = None
     # If task_role_arn is None, a default role is created if create_task_role is True
     create_task_role: bool = True
     # Name for the default role when task_role_arn is None, use "name-task-role" if not provided
     task_role_name: Optional[str] = None
     # Provide a list of policy ARNs to attach to the role
-    add_task_role_policy_arns: Optional[List[str]] = None
+    add_policy_arns_to_task_role: Optional[List[str]] = None
+    # Provide a list of IamPolicy to attach to the task role
+    add_policies_to_task_role: Optional[List[IamPolicy]] = None
     # Add ecs_exec_policy to task role
     add_ecs_exec_policy: bool = False
 
     # The Amazon Resource Name (ARN) of the task execution role that grants the Amazon ECS container agent permission
     # to make Amazon Web Services API calls on your behalf. The task execution IAM role is required depending on the
     # requirements of your task.
     execution_role_arn: Optional[str] = None
     # If execution_role_arn is None, a default role is created if create_execution_role is True
     create_execution_role: bool = True
     # Name for the default role when execution_role_arn is None, use "name-execution-role" if not provided
     execution_role_name: Optional[str] = None
     # Provide a list of policy ARNs to attach to the role
-    add_execution_role_policy_arns: Optional[List[str]] = None
+    add_policy_arns_to_execution_role: Optional[List[str]] = None
+    # Provide a list of IamPolicy to attach to the execution role
+    add_policies_to_execution_role: Optional[List[IamPolicy]] = None
+    # Add policy to read secrets to execution role
+    add_ecs_secret_policy: bool = False
 
     def get_task_family(self):
         return self.family or self.name
 
     def _create(self, aws_client: AwsApiClient) -> bool:
         """Create EcsTaskDefinition"""
         print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
@@ -244,18 +251,18 @@
         return self._create(aws_client)
 
     def get_task_role(self) -> IamRole:
         policy_arns = [
             "arn:aws:iam::aws:policy/service-role/AmazonECSTaskExecutionRolePolicy",
             "arn:aws:iam::aws:policy/CloudWatchFullAccess",
         ]
-        if self.add_task_role_policy_arns is not None and isinstance(
-            self.add_task_role_policy_arns, list
+        if self.add_policy_arns_to_task_role is not None and isinstance(
+            self.add_policy_arns_to_task_role, list
         ):
-            policy_arns.extend(self.add_task_role_policy_arns)
+            policy_arns.extend(self.add_policy_arns_to_task_role)
 
         ecs_exec_policy = IamPolicy(
             name=f"{self.name}-ecs-exec-policy",
             policy_document=dedent(
                 """\
             {
                "Version": "2012-10-17",
@@ -271,14 +278,19 @@
                   "Resource": "*"
                   }
                ]
             }
             """
             ),
         )
+        policies = []
+        if self.add_ecs_exec_policy:
+            policies.append(ecs_exec_policy)
+        if self.add_policies_to_task_role:
+            policies.extend(self.add_policies_to_task_role)
 
         return IamRole(
             name=self.task_role_name or f"{self.name}-task-role",
             assume_role_policy_document=dedent(
                 """\
             {
               "Version": "2012-10-17",
@@ -290,27 +302,54 @@
                   },
                   "Action": "sts:AssumeRole"
                 }
               ]
             }
             """
             ),
-            policies=[ecs_exec_policy] if self.add_ecs_exec_policy else [],
+            policies=policies,
             policy_arns=policy_arns,
         )
 
     def get_execution_role(self) -> IamRole:
         policy_arns = [
             "arn:aws:iam::aws:policy/service-role/AmazonECSTaskExecutionRolePolicy",
             "arn:aws:iam::aws:policy/CloudWatchFullAccess",
         ]
-        if self.add_execution_role_policy_arns is not None and isinstance(
-            self.add_execution_role_policy_arns, list
+        if self.add_policy_arns_to_execution_role is not None and isinstance(
+            self.add_policy_arns_to_execution_role, list
         ):
-            policy_arns.extend(self.add_execution_role_policy_arns)
+            policy_arns.extend(self.add_policy_arns_to_execution_role)
+
+        ecs_secret_policy = IamPolicy(
+            name=f"{self.name}-ecs-secret-policy",
+            policy_document=dedent(
+                """\
+            {
+               "Version": "2012-10-17",
+               "Statement": [
+                   {
+                   "Effect": "Allow",
+                   "Action": [
+                        "secretsmanager:GetSecretValue",
+                        "secretsmanager:DescribeSecret",
+                        "secretsmanager:ListSecretVersionIds"
+                   ],
+                  "Resource": "*"
+                  }
+               ]
+            }
+            """
+            ),
+        )
+        policies = []
+        if self.add_ecs_secret_policy:
+            policies.append(ecs_secret_policy)
+        if self.add_policies_to_execution_role:
+            policies.extend(self.add_policies_to_execution_role)
 
         return IamRole(
             name=self.execution_role_name or f"{self.name}-execution-role",
             assume_role_policy_document=dedent(
                 """\
             {
               "Version": "2012-10-17",
@@ -322,14 +361,15 @@
                   },
                   "Action": "sts:AssumeRole"
                 }
               ]
             }
             """
             ),
+            policies=policies,
             policy_arns=policy_arns,
         )
 
     def task_definition_up_to_date(self, task_definition: Dict[str, Any]) -> bool:
         """Return True if task_definition from the cluster matches the current state"""
 
         # Validate container definitions
```

### Comparing `phidata-1.6.9/phidata/aws/resource/ecs/volume.py` & `phidata-1.7.0/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/eks/addon.py` & `phidata-1.7.0/phidata/aws/resource/eks/addon.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Optional, Any, Dict, Literal
+from typing import Optional, Any, Dict
+from typing_extensions import Literal
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
 from phidata.utils.cli_console import print_info, print_error
 from phidata.utils.log import logger
```

### Comparing `phidata-1.6.9/phidata/aws/resource/eks/cluster.py` & `phidata-1.7.0/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/eks/fargate_profile.py` & `phidata-1.7.0/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/eks/kubeconfig.py` & `phidata-1.7.0/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/eks/node_group.py` & `phidata-1.7.0/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/elasticache/cluster.py` & `phidata-1.7.0/phidata/aws/resource/emr/cluster.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,323 +1,267 @@
-from pathlib import Path
-from typing import Optional, Any, Dict, List, Literal
+from typing import Optional, Any, Dict, List
+from typing_extensions import Literal
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
-from phidata.aws.resource.elasticache.subnet_group import CacheSubnetGroup
 from phidata.utils.cli_console import print_info, print_error, print_warning
 from phidata.utils.log import logger
 
 
-class CacheCluster(AwsResource):
+class EmrCluster(AwsResource):
     """
-    # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html
+    # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html
     """
 
-    resource_type = "CacheCluster"
-    service_name = "elasticache"
+    resource_type = "EmrCluster"
+    service_name = "emr"
 
     # Name of the cluster.
     name: str
-    # The node group (shard) identifier. This parameter is stored as a lowercase string.
-    # If None, use the name as the cache_cluster_id
-    # Constraints:
-    #   A name must contain from 1 to 50 alphanumeric characters or hyphens.
-    #   The first character must be a letter.
-    #   A name cannot end with a hyphen or contain two consecutive hyphens.
-    cache_cluster_id: Optional[str] = None
-    # The name of the cache engine to be used for this cluster.
-    engine: Literal["memcached", "redis"]
-
-    # Compute and memory capacity of the nodes in the node group (shard).
-    cache_node_type: str
-    # The initial number of cache nodes that the cluster has.
-    # For clusters running Redis, this value must be 1.
-    # For clusters running Memcached, this value must be between 1 and 40.
-    num_cache_nodes: int
-
-    # The ID of the replication group to which this cluster should belong.
-    # If this parameter is specified, the cluster is added to the specified replication group as a read replica;
-    # otherwise, the cluster is a standalone primary that is not part of any replication group.
-    replication_group_id: Optional[str] = None
-    # Specifies whether the nodes in this Memcached cluster are created in a single Availability Zone or
-    # created across multiple Availability Zones in the cluster's region.
-    # This parameter is only supported for Memcached clusters.
-    az_mode: Optional[Literal["single-az", "cross-az"]] = None
-    # The EC2 Availability Zone in which the cluster is created.
-    # All nodes belonging to this cluster are placed in the preferred Availability Zone. If you want to create your
-    # nodes across multiple Availability Zones, use PreferredAvailabilityZones .
-    # Default: System chosen Availability Zone.
-    preferred_availability_zone: Optional[str] = None
-    # A list of the Availability Zones in which cache nodes are created. The order of the zones is not important.
-    # This option is only supported on Memcached.
-    preferred_availability_zones: Optional[List[str]] = None
-    # The version number of the cache engine to be used for this cluster.
-    engine_version: Optional[str] = None
-    cache_parameter_group_name: Optional[str] = None
-    cache_subnet_group_name: Optional[str] = None
-    # If cache_subnet_group_name is None,
-    # Read the cache_subnet_group_name from cache_subnet_group
-    cache_subnet_group: Optional[CacheSubnetGroup] = None
-    cache_security_group_names: Optional[List[str]] = None
-    security_group_ids: Optional[List[str]] = None
+    # The location in Amazon S3 to write the log files of the job flow.
+    # If a value is not provided, logs are not created.
+    log_uri: Optional[str] = None
+    # The KMS key used for encrypting log files. If a value is not provided, the logs remain encrypted by AES-256.
+    # This attribute is only available with Amazon EMR version 5.30.0 and later, excluding Amazon EMR 6.0.0.
+    log_encryption_kms_key_id: Optional[str] = None
+    # A JSON string for selecting additional features.
+    additional_info: Optional[str] = None
+    # The Amazon EMR release label, which determines the version of open-source application packages installed on the
+    # cluster. Release labels are in the form emr-x.x.x,
+    # where x.x.x is an Amazon EMR release version such as emr-5.14.0 .
+    release_label: Optional[str] = None
+    # A specification of the number and type of Amazon EC2 instances.
+    instances: Optional[Dict[str, Any]] = None
+    # A list of steps to run.
+    steps: Optional[List[Dict[str, Any]]] = None
+    # A list of bootstrap actions to run before Hadoop starts on the cluster nodes.
+    bootstrap_actions: Optional[List[Dict[str, Any]]] = None
+    # For Amazon EMR releases 3.x and 2.x. For Amazon EMR releases 4.x and later, use Applications.
+    # A list of strings that indicates third-party software to use.
+    supported_products: Optional[List[str]]
+    new_supported_products: Optional[List[Dict[str, Any]]] = None
+    # Applies to Amazon EMR releases 4.0 and later.
+    # A case-insensitive list of applications for Amazon EMR to install and configure when launching the cluster.
+    applications: Optional[List[Dict[str, Any]]] = None
+    # For Amazon EMR releases 4.0 and later. The list of configurations supplied for the EMR cluster you are creating.
+    configurations: Optional[List[Dict[str, Any]]] = None
+    # Also called instance profile and EC2 role. An IAM role for an EMR cluster.
+    # The EC2 instances of the cluster assume this role. The default role is EMR_EC2_DefaultRole.
+    # In order to use the default role, you must have already created it using the CLI or console.
+    job_flow_role: Optional[str] = None
+    # he IAM role that Amazon EMR assumes in order to access Amazon Web Services resources on your behalf.
+    service_role: Optional[str] = None
+    # A list of tags to associate with a cluster and propagate to Amazon EC2 instances.
     tags: Optional[List[Dict[str, str]]] = None
-    snapshot_arns: Optional[List[str]] = None
-    snapshot_name: Optional[str] = None
-    preferred_maintenance_window: Optional[str] = None
-    # The version number of the cache engine to be used for this cluster.
-    port: Optional[int] = None
-    notification_topic_arn: Optional[str] = None
-    auto_minor_version_upgrade: Optional[bool] = None
-    snapshot_retention_limit: Optional[int] = None
-    snapshot_window: Optional[str] = None
-    # The password used to access a password protected server.
-    # Password constraints:
-    # - Must be only printable ASCII characters.
-    # - Must be at least 16 characters and no more than 128 characters in length.
-    # - The only permitted printable special characters are !, &, #, $, ^, <, >, and -.
-    # Other printable special characters cannot be used in the AUTH token.
-    # - For more information, see AUTH password at http://redis.io/commands/AUTH.
-    # Provide AUTH_TOKEN here or as AUTH_TOKEN in secrets_file
-    auth_token: Optional[str] = None
-    outpost_mode: Optional[Literal["single-outpost", "cross-outpost"]] = None
-    preferred_outpost_arn: Optional[str] = None
-    preferred_outpost_arns: Optional[List[str]] = None
-    log_delivery_configurations: Optional[List[Dict[str, Any]]] = None
-    transit_encryption_enabled: Optional[bool] = None
-    network_type: Optional[Literal["ipv4", "ipv6", "dual_stack"]] = None
-    ip_discovery: Optional[Literal["ipv4", "ipv6"]] = None
-
-    # The user-supplied name of a final cluster snapshot
-    final_snapshot_identifier: Optional[str] = None
-
-    # Read secrets from a file in yaml format
-    secrets_file: Optional[Path] = None
-
-    # Cache secret_data
-    cached_secret_data: Optional[Dict[str, Any]] = None
-
-    def get_cache_cluster_id(self):
-        return self.cache_cluster_id or self.name
-
-    def get_secret_data(self) -> Optional[Dict[str, str]]:
-        if self.cached_secret_data is not None:
-            return self.cached_secret_data
-
-        if self.secrets_file is not None:
-            self.cached_secret_data = self.read_yaml_file(self.secrets_file)
-        return self.cached_secret_data
-
-    def get_auth_token(self) -> Optional[str]:
-        auth_token = self.auth_token
-        if auth_token is None and self.secrets_file is not None:
-            # read from secrets_file
-            secret_data = self.get_secret_data()
-            if secret_data is not None:
-                auth_token = secret_data.get("AUTH_TOKEN", auth_token)
-        return auth_token
+    # The name of a security configuration to apply to the cluster.
+    security_configuration: Optional[str] = None
+    # An IAM role for automatic scaling policies. The default role is EMR_AutoScaling_DefaultRole.
+    # The IAM role provides permissions that the automatic scaling feature requires to launch and terminate EC2
+    # instances in an instance group.
+    auto_scaling_role: Optional[str] = None
+    scale_down_behavior: Optional[
+        Literal["TERMINATE_AT_INSTANCE_HOUR", "TERMINATE_AT_TASK_COMPLETION"]
+    ] = None
+    custom_ami_id: Optional[str] = None
+    # The size, in GiB, of the Amazon EBS root device volume of the Linux AMI that is used for each EC2 instance.
+    ebs_root_volume_size: Optional[int] = None
+    repo_upgrade_on_boot: Optional[Literal["SECURITY", "NONE"]] = None
+    # Attributes for Kerberos configuration when Kerberos authentication is enabled using a security configuration.
+    kerberos_attributes: Optional[Dict[str, str]] = None
+    # Specifies the number of steps that can be executed concurrently.
+    # The default value is 1 . The maximum value is 256 .
+    step_concurrency_level: Optional[int] = None
+    # The specified managed scaling policy for an Amazon EMR cluster.
+    managed_scaling_policy: Optional[Dict[str, Any]] = None
+    placement_group_configs: Optional[List[Dict[str, Any]]] = None
+    # The auto-termination policy defines the amount of idle time in seconds after which a cluster terminates.
+    auto_termination_policy: Optional[Dict[str, int]] = None
+
+    # provided by api on create
+    # A unique identifier for the job flow.
+    job_flow_id: Optional[str] = None
+    # The Amazon Resource Name (ARN) of the cluster.
+    cluster_arn: Optional[str] = None
+    # ClusterSummary returned on read
+    cluster_summary: Optional[Dict] = None
 
     def _create(self, aws_client: AwsApiClient) -> bool:
-        """Creates the CacheCluster
+        """Creates the EmrCluster
 
         Args:
             aws_client: The AwsApiClient for the current cluster
         """
-        print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
-
-        # Get the CacheSubnetGroupName
-        cache_subnet_group_name = self.cache_subnet_group_name
-        if cache_subnet_group_name is None and self.cache_subnet_group is not None:
-            cache_subnet_group_name = self.cache_subnet_group.name
-            logger.debug(f"Using CacheSubnetGroup: {cache_subnet_group_name}")
-
-        # create a dict of args which are not null, otherwise aws type validation fails
-        not_null_args: Dict[str, Any] = {}
-        if self.replication_group_id is not None:
-            not_null_args["ReplicationGroupId"] = self.replication_group_id
-        if self.az_mode is not None:
-            not_null_args["AZMode"] = self.az_mode
-        if self.preferred_availability_zone is not None:
-            not_null_args[
-                "PreferredAvailabilityZone"
-            ] = self.preferred_availability_zone
-        if self.preferred_availability_zones is not None:
-            not_null_args[
-                "PreferredAvailabilityZones"
-            ] = self.preferred_availability_zones
-        if self.num_cache_nodes is not None:
-            not_null_args["NumCacheNodes"] = self.num_cache_nodes
-        if self.cache_node_type is not None:
-            not_null_args["CacheNodeType"] = self.cache_node_type
-        if self.engine is not None:
-            not_null_args["Engine"] = self.engine
-        if self.engine_version is not None:
-            not_null_args["EngineVersion"] = self.engine_version
-        if self.cache_parameter_group_name is not None:
-            not_null_args["CacheParameterGroupName"] = self.cache_parameter_group_name
-        if cache_subnet_group_name is not None:
-            not_null_args["CacheSubnetGroupName"] = cache_subnet_group_name
-        if self.cache_security_group_names is not None:
-            not_null_args["CacheSecurityGroupNames"] = self.cache_security_group_names
-        if self.security_group_ids is not None:
-            not_null_args["SecurityGroupIds"] = self.security_group_ids
-        if self.tags is not None:
-            not_null_args["Tags"] = self.tags
-        if self.snapshot_arns is not None:
-            not_null_args["SnapshotArns"] = self.snapshot_arns
-        if self.snapshot_name is not None:
-            not_null_args["SnapshotName"] = self.snapshot_name
-        if self.preferred_maintenance_window is not None:
-            not_null_args[
-                "PreferredMaintenanceWindow"
-            ] = self.preferred_maintenance_window
-        if self.port is not None:
-            not_null_args["Port"] = self.port
-        if self.notification_topic_arn is not None:
-            not_null_args["NotificationTopicArn"] = self.notification_topic_arn
-        if self.auto_minor_version_upgrade is not None:
-            not_null_args["AutoMinorVersionUpgrade"] = self.auto_minor_version_upgrade
-        if self.snapshot_retention_limit is not None:
-            not_null_args["SnapshotRetentionLimit"] = self.snapshot_retention_limit
-        if self.snapshot_window is not None:
-            not_null_args["SnapshotWindow"] = self.snapshot_window
-        if self.auth_token is not None:
-            not_null_args["AuthToken"] = self.get_auth_token()
-        if self.outpost_mode is not None:
-            not_null_args["OutpostMode"] = self.outpost_mode
-        if self.preferred_outpost_arn is not None:
-            not_null_args["PreferredOutpostArn"] = self.preferred_outpost_arn
-        if self.preferred_outpost_arns is not None:
-            not_null_args["PreferredOutpostArns"] = self.preferred_outpost_arns
-        if self.log_delivery_configurations is not None:
-            not_null_args[
-                "LogDeliveryConfigurations"
-            ] = self.log_delivery_configurations
-        if self.transit_encryption_enabled is not None:
-            not_null_args["TransitEncryptionEnabled"] = self.transit_encryption_enabled
-        if self.network_type is not None:
-            not_null_args["NetworkType"] = self.network_type
-        if self.ip_discovery is not None:
-            not_null_args["IpDiscovery"] = self.ip_discovery
 
-        # Create CacheCluster
-        service_client = self.get_service_client(aws_client)
+        print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
         try:
-            create_response = service_client.create_cache_cluster(
-                CacheClusterId=self.get_cache_cluster_id(),
+            # create a dict of args which are not null, otherwise aws type validation fails
+            not_null_args: Dict[str, Any] = {}
+
+            if self.log_uri:
+                not_null_args["LogUri"] = self.log_uri
+            if self.log_encryption_kms_key_id:
+                not_null_args["LogEncryptionKmsKeyId"] = self.log_encryption_kms_key_id
+            if self.additional_info:
+                not_null_args["AdditionalInfo"] = self.additional_info
+            if self.release_label:
+                not_null_args["ReleaseLabel"] = self.release_label
+            if self.instances:
+                not_null_args["Instances"] = self.instances
+            if self.steps:
+                not_null_args["Steps"] = self.steps
+            if self.bootstrap_actions:
+                not_null_args["BootstrapActions"] = self.bootstrap_actions
+            if self.supported_products:
+                not_null_args["SupportedProducts"] = self.supported_products
+            if self.new_supported_products:
+                not_null_args["NewSupportedProducts"] = self.new_supported_products
+            if self.applications:
+                not_null_args["Applications"] = self.applications
+            if self.configurations:
+                not_null_args["Configurations"] = self.configurations
+            if self.job_flow_role:
+                not_null_args["JobFlowRole"] = self.job_flow_role
+            if self.service_role:
+                not_null_args["ServiceRole"] = self.service_role
+            if self.tags:
+                not_null_args["Tags"] = self.tags
+            if self.security_configuration:
+                not_null_args["SecurityConfiguration"] = self.security_configuration
+            if self.auto_scaling_role:
+                not_null_args["AutoScalingRole"] = self.auto_scaling_role
+            if self.scale_down_behavior:
+                not_null_args["ScaleDownBehavior"] = self.scale_down_behavior
+            if self.custom_ami_id:
+                not_null_args["CustomAmiId"] = self.custom_ami_id
+            if self.ebs_root_volume_size:
+                not_null_args["EbsRootVolumeSize"] = self.ebs_root_volume_size
+            if self.repo_upgrade_on_boot:
+                not_null_args["RepoUpgradeOnBoot"] = self.repo_upgrade_on_boot
+            if self.kerberos_attributes:
+                not_null_args["KerberosAttributes"] = self.kerberos_attributes
+            if self.step_concurrency_level:
+                not_null_args["StepConcurrencyLevel"] = self.step_concurrency_level
+            if self.managed_scaling_policy:
+                not_null_args["ManagedScalingPolicy"] = self.managed_scaling_policy
+            if self.placement_group_configs:
+                not_null_args["PlacementGroupConfigs"] = self.placement_group_configs
+            if self.auto_termination_policy:
+                not_null_args["AutoTerminationPolicy"] = self.auto_termination_policy
+
+            # Get the service_client
+            service_client = self.get_service_client(aws_client)
+
+            # Create EmrCluster
+            create_response = service_client.run_job_flow(
+                Name=self.name,
                 **not_null_args,
             )
-            logger.debug(f"CacheCluster: {create_response}")
-            resource_dict = create_response.get("CacheCluster", {})
+            logger.debug(f"create_response type: {type(create_response)}")
+            logger.debug(f"create_response: {create_response}")
 
-            # Validate resource creation
-            if resource_dict is not None:
-                print_info(f"CacheCluster created: {self.get_cache_cluster_id()}")
-                self.active_resource = create_response
+            self.job_flow_id = create_response.get("JobFlowId", None)
+            self.cluster_arn = create_response.get("ClusterArn", None)
+            self.active_resource = create_response
+            if self.active_resource is not None:
+                print_info(
+                    f"{self.get_resource_type()}: {self.get_resource_name()} created"
+                )
+                logger.debug(f"JobFlowId: {self.job_flow_id}")
+                logger.debug(f"ClusterArn: {self.cluster_arn}")
                 return True
         except Exception as e:
             print_error(f"{self.get_resource_type()} could not be created.")
             print_error(e)
         return False
 
     def post_create(self, aws_client: AwsApiClient) -> bool:
-        # Wait for CacheCluster to be created
+        ## Wait for Cluster to be created
         if self.wait_for_creation:
             try:
-                print_info(f"Waiting for {self.get_resource_type()} to be active.")
-                waiter = self.get_service_client(aws_client).get_waiter(
-                    "cache_cluster_available"
-                )
-                waiter.wait(
-                    CacheClusterId=self.get_cache_cluster_id(),
-                    WaiterConfig={
-                        "Delay": self.waiter_delay,
-                        "MaxAttempts": self.waiter_max_attempts,
-                    },
-                )
+                print_info("Waiting for EmrCluster to be active.")
+                if self.job_flow_id is not None:
+                    waiter = self.get_service_client(aws_client).get_waiter(
+                        "cluster_running"
+                    )
+                    waiter.wait(
+                        ClusterId=self.job_flow_id,
+                        WaiterConfig={
+                            "Delay": self.waiter_delay,
+                            "MaxAttempts": self.waiter_max_attempts,
+                        },
+                    )
+                else:
+                    print_warning("Skipping waiter, No ClusterId found")
             except Exception as e:
                 print_error("Waiter failed.")
                 print_error(e)
         return True
 
     def _read(self, aws_client: AwsApiClient) -> Optional[Any]:
-        """Returns the CacheCluster
+        """Returns the EmrCluster
 
         Args:
             aws_client: The AwsApiClient for the current cluster
         """
-        logger.debug(f"Reading {self.get_resource_type()}: {self.get_resource_name()}")
-
         from botocore.exceptions import ClientError
 
-        service_client = self.get_service_client(aws_client)
+        logger.debug(f"Reading {self.get_resource_type()}: {self.get_resource_name()}")
         try:
-            cache_cluster_id = self.get_cache_cluster_id()
-            describe_response = service_client.describe_cache_clusters(
-                CacheClusterId=cache_cluster_id
-            )
-            logger.debug(f"CacheCluster: {describe_response}")
-            resource_list = describe_response.get("CacheClusters", None)
-
-            if resource_list is not None and isinstance(resource_list, list):
-                for resource in resource_list:
-                    _cluster_identifier = resource.get("CacheClusterId", None)
-                    if _cluster_identifier == cache_cluster_id:
-                        self.active_resource = resource
+            service_client = self.get_service_client(aws_client)
+            list_response = service_client.list_clusters()
+            # logger.debug(f"list_response type: {type(list_response)}")
+            # logger.debug(f"list_response: {list_response}")
+
+            cluster_summary_list = list_response.get("Clusters", None)
+            if cluster_summary_list is not None and isinstance(
+                cluster_summary_list, list
+            ):
+                for _cluster_summary in cluster_summary_list:
+                    cluster_name = _cluster_summary.get("Name", None)
+                    if cluster_name == self.name:
+                        self.active_resource = _cluster_summary
                         break
+
+            if self.active_resource is None:
+                logger.debug(f"No {self.get_resource_type()} found")
+                return None
+
+            # logger.debug(f"EmrCluster: {self.active_resource}")
+            self.job_flow_id = self.active_resource.get("Id", None)
+            self.cluster_arn = self.active_resource.get("ClusterArn", None)
         except ClientError as ce:
             logger.debug(f"ClientError: {ce}")
         except Exception as e:
             print_error(f"Error reading {self.get_resource_type()}.")
             print_error(e)
         return self.active_resource
 
     def _delete(self, aws_client: AwsApiClient) -> bool:
-        """Deletes the CacheCluster
+        """Deletes the EmrCluster
 
         Args:
             aws_client: The AwsApiClient for the current cluster
         """
+
         print_info(f"Deleting {self.get_resource_type()}: {self.get_resource_name()}")
+        try:
+            # populate self.job_flow_id
+            self._read(aws_client)
 
-        # create a dict of args which are not null, otherwise aws type validation fails
-        not_null_args: Dict[str, Any] = {}
-        if self.final_snapshot_identifier:
-            not_null_args["FinalSnapshotIdentifier"] = self.final_snapshot_identifier
+            service_client = self.get_service_client(aws_client)
+            self.active_resource = None
 
-        service_client = self.get_service_client(aws_client)
-        self.active_resource = None
-        try:
-            delete_response = service_client.delete_cache_cluster(
-                CacheClusterId=self.get_cache_cluster_id(),
-                **not_null_args,
-            )
-            logger.debug(f"CacheCluster: {delete_response}")
-            print_info(
-                f"{self.get_resource_type()}: {self.get_resource_name()} deleted"
-            )
+            if self.job_flow_id:
+                delete_response = service_client.terminate_job_flows(
+                    JobFlowIds=[self.job_flow_id]
+                )
+                print_info(
+                    f"{self.get_resource_type()}: {self.get_resource_name()} deleted"
+                )
+            else:
+                print_error("Could not find cluster id")
             return True
         except Exception as e:
             print_error(f"{self.get_resource_type()} could not be deleted.")
             print_error("Please try again or delete resources manually.")
             print_error(e)
         return False
-
-    def post_delete(self, aws_client: AwsApiClient) -> bool:
-        # Wait for CacheCluster to be deleted
-        if self.wait_for_deletion:
-            try:
-                print_info(f"Waiting for {self.get_resource_type()} to be deleted.")
-                waiter = self.get_service_client(aws_client).get_waiter(
-                    "cache_cluster_deleted"
-                )
-                waiter.wait(
-                    CacheClusterId=self.get_cache_cluster_id(),
-                    WaiterConfig={
-                        "Delay": self.waiter_delay,
-                        "MaxAttempts": self.waiter_max_attempts,
-                    },
-                )
-            except Exception as e:
-                print_error("Waiter failed.")
-                print_error(e)
-        return True
```

### Comparing `phidata-1.6.9/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-1.7.0/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/elb/listener.py` & `phidata-1.7.0/phidata/aws/resource/elb/listener.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, Any, Dict, List
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
+from phidata.aws.resource.acm.certificate import AcmCertificate
 from phidata.aws.resource.elb.load_balancer import LoadBalancer
 from phidata.aws.resource.elb.target_group import TargetGroup
 from phidata.utils.cli_console import print_info, print_error, print_warning
 from phidata.utils.log import logger
 
 
 class Listener(AwsResource):
@@ -21,14 +22,15 @@
     load_balancer: Optional[LoadBalancer] = None
     target_group: Optional[TargetGroup] = None
     load_balancer_arn: Optional[str] = None
     protocol: Optional[str] = None
     port: Optional[int] = None
     ssl_policy: Optional[str] = None
     certificates: Optional[List[Dict[str, Any]]]
+    acm_certificates: Optional[List[AcmCertificate]] = None
     default_actions: Optional[List[Dict]]
     alpn_policy: Optional[List[str]]
     tags: Optional[List[Dict[str, str]]]
 
     def _create(self, aws_client: AwsApiClient) -> bool:
         """Creates the Listener
 
@@ -36,26 +38,30 @@
             aws_client: The AwsApiClient for the current Listener
         """
         print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
 
         load_balancer_arn = self.get_load_balancer_arn(aws_client)
         if load_balancer_arn is None:
             logger.error(f"Load balancer ARN not available")
-            return True
+            return False
+
+        listener_port = self.get_listener_port()
+        listener_protocol = self.get_listener_protocol()
+        listener_certificates = self.get_listener_certificates(aws_client)
 
         # create a dict of args which are not null, otherwise aws type validation fails
         not_null_args: Dict[str, Any] = {}
-        if self.protocol is not None:
-            not_null_args["Protocol"] = self.protocol
-        if self.port is not None:
-            not_null_args["Port"] = self.port
+        if listener_port is not None:
+            not_null_args["Port"] = listener_port
+        if listener_protocol is not None:
+            not_null_args["Protocol"] = listener_protocol
+        if listener_certificates is not None:
+            not_null_args["Certificates"] = listener_certificates
         if self.ssl_policy is not None:
             not_null_args["SslPolicy"] = self.ssl_policy
-        if self.certificates is not None:
-            not_null_args["Certificates"] = self.certificates
         if self.alpn_policy is not None:
             not_null_args["AlpnPolicy"] = self.alpn_policy
         if self.tags is not None:
             not_null_args["Tags"] = self.tags
 
         if self.default_actions is not None:
             not_null_args["DefaultActions"] = self.default_actions
@@ -161,29 +167,47 @@
         print_info(f"Updating {self.get_resource_type()}: {self.get_resource_name()}")
 
         listener_arn = self.get_arn
         if listener_arn is None:
             print_error(f"Listener {self.get_resource_name()} not found.")
             return True
 
+        listener_port = self.get_listener_port()
+        listener_protocol = self.get_listener_protocol()
+        listener_certificates = self.get_listener_certificates(aws_client)
+
         # create a dict of args which are not null, otherwise aws type validation fails
         not_null_args: Dict[str, Any] = {}
-        if self.protocol is not None:
-            not_null_args["Protocol"] = self.protocol
-        if self.port is not None:
-            not_null_args["Port"] = self.port
+        if listener_port is not None:
+            not_null_args["Port"] = listener_port
+        if listener_protocol is not None:
+            not_null_args["Protocol"] = listener_protocol
+        if listener_certificates is not None:
+            not_null_args["Certificates"] = listener_certificates
         if self.ssl_policy is not None:
             not_null_args["SslPolicy"] = self.ssl_policy
-        if self.certificates is not None:
-            not_null_args["Certificates"] = self.certificates
-        if self.default_actions is not None:
-            not_null_args["DefaultActions"] = self.default_actions
         if self.alpn_policy is not None:
             not_null_args["AlpnPolicy"] = self.alpn_policy
 
+        if self.default_actions is not None:
+            not_null_args["DefaultActions"] = self.default_actions
+        elif self.target_group is not None:
+            target_group_arn = self.target_group.get_arn(aws_client)
+            if target_group_arn is None:
+                logger.error(f"Target group ARN not available")
+                return False
+            not_null_args["DefaultActions"] = [
+                {"Type": "forward", "TargetGroupArn": target_group_arn}
+            ]
+        else:
+            print_warning(
+                f"Neither target group nor default actions provided for {self.get_resource_name()}"
+            )
+            return True
+
         service_client = self.get_service_client(aws_client)
         try:
             create_response = service_client.modify_listener(
                 ListenerArn=listener_arn,
                 **not_null_args,
             )
             logger.debug(f"Update Response: {create_response}")
@@ -209,7 +233,41 @@
 
     def get_load_balancer_arn(self, aws_client: AwsApiClient):
         load_balancer_arn = self.load_balancer_arn
         if load_balancer_arn is None and self.load_balancer:
             load_balancer_arn = self.load_balancer.get_arn(aws_client)
 
         return load_balancer_arn
+
+    def get_listener_port(self):
+        listener_port = self.port
+        if listener_port is None and self.load_balancer:
+            lb_protocol = self.load_balancer.protocol
+            listener_port = 443 if lb_protocol == "HTTPS" else 80
+
+        return listener_port
+
+    def get_listener_protocol(self):
+        listener_protocol = self.protocol
+        if listener_protocol is None and self.load_balancer:
+            listener_protocol = self.load_balancer.protocol
+
+        return listener_protocol
+
+    def get_listener_certificates(self, aws_client: AwsApiClient):
+        listener_protocol = self.protocol
+        if listener_protocol is None and self.load_balancer:
+            listener_protocol = self.load_balancer.protocol
+
+        certificates = self.certificates
+        if (
+            certificates is None
+            and self.acm_certificates is not None
+            and len(self.acm_certificates) > 0
+        ):
+            certificates = []
+            for cert in self.acm_certificates:
+                certificates.append(
+                    {"CertificateArn": cert.get_certificate_arn(aws_client)}
+                )
+
+        return certificates
```

### Comparing `phidata-1.6.9/phidata/aws/resource/elb/load_balancer.py` & `phidata-1.7.0/phidata/aws/resource/elb/load_balancer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from typing import Optional, Any, Dict, List
+from typing import Optional, Any, Dict, List, Union
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
+from phidata.aws.resource.ec2.subnet import Subnet
+from phidata.aws.resource.ec2.security_group import SecurityGroup
 from phidata.utils.cli_console import print_info, print_error, print_warning
 from phidata.utils.log import logger
 
 
 class LoadBalancer(AwsResource):
     """
     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html
     """
 
     resource_type = "LoadBalancer"
     service_name = "elbv2"
 
     # Name of the Load Balancer.
     name: str
-    subnets: Optional[List[str]] = None
+    subnets: Optional[List[Union[str, Subnet]]] = None
     subnet_mappings: Optional[List[Dict[str, str]]] = None
-    security_groups: Optional[List[str]] = None
+    security_groups: Optional[List[Union[str, SecurityGroup]]] = None
     scheme: Optional[str] = None
     tags: Optional[List[Dict[str, str]]] = None
     type: Optional[str] = None
     ip_address_type: Optional[str] = None
     customer_owned_ipv_4_pool: Optional[str] = None
 
     # Protocol for load_balancer: HTTP or HTTPS
@@ -34,20 +36,36 @@
         Args:
             aws_client: The AwsApiClient for the current Load Balancer
         """
         print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
 
         # create a dict of args which are not null, otherwise aws type validation fails
         not_null_args: Dict[str, Any] = {}
+
         if self.subnets is not None:
-            not_null_args["Subnets"] = self.subnets
+            subnet_ids = []
+            for subnet in self.subnets:
+                if isinstance(subnet, Subnet):
+                    subnet_ids.append(subnet.id)
+                elif isinstance(subnet, str):
+                    subnet_ids.append(subnet)
+            not_null_args["Subnets"] = subnet_ids
+
         if self.subnet_mappings is not None:
             not_null_args["SubnetMappings"] = self.subnet_mappings
+
         if self.security_groups is not None:
-            not_null_args["SecurityGroups"] = self.security_groups
+            security_group_ids = []
+            for sg in self.security_groups:
+                if isinstance(sg, SecurityGroup):
+                    security_group_ids.append(sg.get_security_group_id(aws_client))
+                else:
+                    security_group_ids.append(sg)
+            not_null_args["SecurityGroups"] = security_group_ids
+
         if self.scheme is not None:
             not_null_args["Scheme"] = self.scheme
         if self.tags is not None:
             not_null_args["tags"] = self.tags
         if self.type is not None:
             not_null_args["Type"] = self.type
         if self.ip_address_type is not None:
```

### Comparing `phidata-1.6.9/phidata/aws/resource/elb/target_group.py` & `phidata-1.7.0/phidata/aws/resource/elb/target_group.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Optional, Any, Dict, List
+from typing import Optional, Any, Dict, List, Union
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
+from phidata.aws.resource.ec2.subnet import Subnet
 from phidata.utils.cli_console import print_info, print_error, print_warning
 from phidata.utils.log import logger
 
 
 class TargetGroup(AwsResource):
     """
     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/client/create_target_group.html
@@ -16,14 +17,15 @@
 
     # Name of the Target Group
     name: str
     protocol: Optional[str] = None
     protocol_version: Optional[str] = None
     port: Optional[int] = None
     vpc_id: Optional[str] = None
+    subnets: Optional[List[Union[str, Subnet]]] = None
     health_check_protocol: Optional[str] = None
     health_check_port: Optional[str] = None
     health_check_enabled: Optional[bool] = None
     health_check_path: Optional[str] = None
     health_check_interval_seconds: Optional[int] = None
     health_check_timeout_seconds: Optional[int] = None
     healthy_threshold_count: Optional[int] = None
@@ -39,22 +41,36 @@
         Args:
             aws_client: The AwsApiClient for the current Target Group
         """
         print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
 
         # create a dict of args which are not null, otherwise aws type validation fails
         not_null_args: Dict[str, Any] = {}
+
+        # Get vpc_id
+        vpc_id = self.vpc_id
+        if vpc_id is None and self.subnets is not None:
+            from phidata.aws.resource.ec2.subnet import get_vpc_id_from_subnet_ids
+
+            subnet_ids = []
+            for subnet in self.subnets:
+                if isinstance(subnet, Subnet):
+                    subnet_ids.append(subnet.id)
+                elif isinstance(subnet, str):
+                    subnet_ids.append(subnet)
+            vpc_id = get_vpc_id_from_subnet_ids(subnet_ids, aws_client)
+        if vpc_id is not None:
+            not_null_args["VpcId"] = vpc_id
+
         if self.protocol is not None:
             not_null_args["Protocol"] = self.protocol
         if self.protocol_version is not None:
             not_null_args["ProtocolVersion"] = self.protocol_version
         if self.port is not None:
             not_null_args["Port"] = self.port
-        if self.vpc_id is not None:
-            not_null_args["VpcId"] = self.vpc_id
         if self.health_check_protocol is not None:
             not_null_args["HealthCheckProtocol"] = self.health_check_protocol
         if self.health_check_port is not None:
             not_null_args["HealthCheckPort"] = self.health_check_port
         if self.health_check_enabled is not None:
             not_null_args["HealthCheckEnabled"] = self.health_check_enabled
         if self.health_check_path is not None:
@@ -83,15 +99,15 @@
         # Create TargetGroup
         service_client = self.get_service_client(aws_client)
         try:
             create_response = service_client.create_target_group(
                 Name=self.name,
                 **not_null_args,
             )
-            logger.debug(f"Create Response: {create_response}")
+            logger.debug(f"Response: {create_response}")
             resource_dict = create_response.get("TargetGroups", {})
 
             # Validate resource creation
             if resource_dict is not None:
                 print_info(f"TargetGroup created: {self.get_resource_name()}")
                 self.active_resource = create_response
                 return True
@@ -102,26 +118,27 @@
 
     def _read(self, aws_client: AwsApiClient) -> Optional[Any]:
         """Returns the TargetGroup
 
         Args:
             aws_client: The AwsApiClient for the current TargetGroup
         """
-        logger.debug(f"Reading {self.get_resource_type()}: {self.get_resource_name()}")
-
         from botocore.exceptions import ClientError
 
+        logger.debug(f"Reading {self.get_resource_type()}: {self.get_resource_name()}")
         service_client = self.get_service_client(aws_client)
         try:
             describe_response = service_client.describe_target_groups(Names=[self.name])
             logger.debug(f"Describe Response: {describe_response}")
             resource_list = describe_response.get("TargetGroups", None)
 
             if resource_list is not None and isinstance(resource_list, list):
-                self.active_resource = resource_list[0]
+                for resource in resource_list:
+                    if resource.get("TargetGroupName") == self.name:
+                        self.active_resource = resource
         except ClientError as ce:
             logger.debug(f"ClientError: {ce}")
         except Exception as e:
             print_error(f"Error reading {self.get_resource_type()}.")
             print_error(e)
         return self.active_resource
```

### Comparing `phidata-1.6.9/phidata/aws/resource/glue/crawler.py` & `phidata-1.7.0/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/group.py` & `phidata-1.7.0/phidata/aws/resource/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 from phidata.aws.resource.acm.certificate import AcmCertificate
 from phidata.aws.resource.cloudformation.stack import CloudFormationStack
 from phidata.aws.resource.ec2.volume import EbsVolume
+from phidata.aws.resource.ec2.security_group import (
+    SecurityGroup,
+    InboundRule,
+    OutboundRule,
+)
 from phidata.aws.resource.ec2.subnet import Subnet
 from phidata.aws.resource.ecs.cluster import EcsCluster
 from phidata.aws.resource.ecs.container import EcsContainer
 from phidata.aws.resource.ecs.task_definition import EcsTaskDefinition
 from phidata.aws.resource.ecs.volume import EcsVolume
 from phidata.aws.resource.ecs.service import EcsService
 from phidata.aws.resource.eks.cluster import EksCluster
@@ -18,15 +23,15 @@
 from phidata.aws.resource.elb.load_balancer import LoadBalancer
 from phidata.aws.resource.elb.target_group import TargetGroup
 from phidata.aws.resource.elb.listener import Listener
 from phidata.aws.resource.iam.role import IamRole
 from phidata.aws.resource.iam.policy import IamPolicy
 from phidata.aws.resource.glue.crawler import GlueCrawler
 from phidata.aws.resource.s3.bucket import S3Bucket
-# from phidata.aws.resource.secret.manager import SecretsManager
+from phidata.aws.resource.secret.manager import SecretsManager
 from phidata.aws.resource.emr.cluster import EmrCluster
 from phidata.aws.resource.rds.db_cluster import DbCluster
 from phidata.aws.resource.rds.db_instance import DbInstance
 from phidata.aws.resource.rds.db_subnet_group import DbSubnetGroup
 from phidata.aws.resource.elasticache.cluster import CacheCluster
 from phidata.aws.resource.elasticache.subnet_group import CacheSubnetGroup
 
@@ -38,25 +43,26 @@
     enabled: bool = True
     weight: int = 100
 
     subnets: Optional[List[Subnet]] = None
     iam_roles: Optional[List[IamRole]] = None
     iam_policies: Optional[List[IamPolicy]] = None
     acm_certificates: Optional[List[AcmCertificate]] = None
-    # secrets: Optional[List[SecretsManager]] = None
+    secrets: Optional[List[SecretsManager]] = None
     s3_buckets: Optional[List[S3Bucket]] = None
     cache_clusters: Optional[List[CacheCluster]] = None
     cache_subnet_groups: Optional[List[CacheSubnetGroup]] = None
     db_clusters: Optional[List[DbCluster]] = None
     db_subnet_groups: Optional[List[DbSubnetGroup]] = None
     db_instances: Optional[List[DbInstance]] = None
     ecs_clusters: Optional[List[EcsCluster]] = None
     ecs_task_definitions: Optional[List[EcsTaskDefinition]] = None
     ecs_services: Optional[List[EcsService]] = None
     volumes: Optional[List[EbsVolume]] = None
+    security_groups: Optional[List[SecurityGroup]] = None
     cloudformation_stacks: Optional[List[CloudFormationStack]] = None
     eks_cluster: Optional[EksCluster] = None
     eks_kubeconfig: Optional[EksKubeconfig] = None
     eks_fargate_profiles: Optional[List[EksFargateProfile]] = None
     eks_nodegroups: Optional[List[EksNodeGroup]] = None
     crawlers: Optional[List[GlueCrawler]] = None
     emr: Optional[List[EmrCluster]] = None
```

### Comparing `phidata-1.6.9/phidata/aws/resource/iam/group.py` & `phidata-1.7.0/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/iam/policy.py` & `phidata-1.7.0/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/iam/role.py` & `phidata-1.7.0/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/rds/db_cluster.py` & `phidata-1.7.0/phidata/aws/resource/rds/db_cluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
-from typing import Optional, Any, Dict, List, Literal, Union
+from typing import Optional, Any, Dict, List, Union
+from typing_extensions import Literal
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
 from phidata.aws.resource.cloudformation.stack import CloudFormationStack
+from phidata.aws.resource.ec2.security_group import SecurityGroup
 from phidata.aws.resource.rds.db_instance import DbInstance
 from phidata.aws.resource.rds.db_subnet_group import DbSubnetGroup
 from phidata.utils.cli_console import print_info, print_error, print_warning
 from phidata.utils.log import logger
 
 
 class DbCluster(AwsResource):
@@ -81,20 +83,22 @@
     db_cluster_identifier: Optional[str] = None
     # The name of the DB cluster parameter group to associate with this DB cluster.
     # If you do not specify a value, then the default DB cluster parameter group for the specified
     # DB engine and version is used.
     # Constraints: If supplied, must match the name of an existing DB cluster parameter group.
     db_cluster_parameter_group_name: Optional[str] = None
 
-    ## Networking
     # A list of EC2 VPC security groups to associate with this DB cluster.
     vpc_security_group_ids: Optional[List[str]] = None
     # If vpc_security_group_ids is None,
     # Read the security_group_id from vpc_stack
     vpc_stack: Optional[CloudFormationStack] = None
+    # If vpc_security_group_ids is None and vpc_stack is None
+    # Read the security_group_id from db_security_groups
+    db_security_groups: Optional[List[SecurityGroup]] = None
 
     # A DB subnet group to associate with this DB cluster.
     # This setting is required to create a Multi-AZ DB cluster.
     # Constraints: Must match the name of an existing DBSubnetGroup. Must not be default.
     db_subnet_group_name: Optional[str] = None
     # If db_subnet_group_name is None,
     # Read the db_subnet_group_name from db_subnet_group
@@ -230,28 +234,31 @@
     # If skip_final_snapshot = None, a DB cluster snapshot is created before the DB cluster is deleted.
     #
     # You must specify a FinalDBSnapshotIdentifier parameter
     # if skip_final_snapshot = None.
     skip_final_snapshot: Optional[bool] = True
     final_db_snapshot_identifier: Optional[str] = None
 
+    # Parameters for update function
+    new_db_cluster_identifier: Optional[str] = None
+    apply_immediately: Optional[bool] = None
+    cloudwatch_logs_exports: Optional[List[str]] = None
+    allow_major_version_upgrade: Optional[bool] = None
+    db_instance_parameter_group_name: Optional[str] = None
+    manage_master_user_password: Optional[bool] = None
+    rotate_master_user_password: Optional[bool] = None
+    master_iser_secter_kms_key_id: Optional[str] = None
+    allow_engine_mode_change: Optional[bool] = None
+
     # Cache secret_data
     cached_secret_data: Optional[Dict[str, Any]] = None
 
     def get_db_cluster_identifier(self):
         return self.db_cluster_identifier or self.name
 
-    def get_secret_data(self) -> Optional[Dict[str, str]]:
-        if self.cached_secret_data is not None:
-            return self.cached_secret_data
-
-        if self.secrets_file is not None:
-            self.cached_secret_data = self.read_yaml_file(self.secrets_file)
-        return self.cached_secret_data
-
     def get_master_username(self) -> Optional[str]:
         master_username = self.master_username
         if master_username is None and self.secrets_file is not None:
             # read from secrets_file
             secret_data = self.get_secret_data()
             if secret_data is not None:
                 master_username = secret_data.get("MASTER_USERNAME", master_username)
@@ -287,51 +294,60 @@
         """Creates the DbCluster
 
         Args:
             aws_client: The AwsApiClient for the current cluster
         """
         print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
 
+        # create a dict of args which are not null, otherwise aws type validation fails
+        not_null_args: Dict[str, Any] = {}
+
         # Step 1: Get the VpcSecurityGroupIds
         vpc_security_group_ids = self.vpc_security_group_ids
         if vpc_security_group_ids is None and self.vpc_stack is not None:
             vpc_stack_sg = self.vpc_stack.get_security_group(aws_client=aws_client)
             if vpc_stack_sg is not None:
                 logger.debug(f"Using SecurityGroup: {vpc_stack_sg}")
                 vpc_security_group_ids = [vpc_stack_sg]
+        if vpc_security_group_ids is None and self.db_security_groups is not None:
+            sg_ids = []
+            for sg in self.db_security_groups:
+                sg_id = sg.get_security_group_id(aws_client)
+                if sg_id is not None:
+                    sg_ids.append(sg_id)
+            if len(sg_ids) > 0:
+                vpc_security_group_ids = sg_ids
+                logger.debug(f"Using SecurityGroups: {vpc_security_group_ids}")
+        if vpc_security_group_ids is not None:
+            not_null_args["VpcSecurityGroupIds"] = vpc_security_group_ids
 
         # Step 2: Get the DbSubnetGroupName
         db_subnet_group_name = self.db_subnet_group_name
         if db_subnet_group_name is None and self.db_subnet_group is not None:
             db_subnet_group_name = self.db_subnet_group.name
             logger.debug(f"Using DbSubnetGroup: {db_subnet_group_name}")
+        if db_subnet_group_name is not None:
+            not_null_args["DBSubnetGroupName"] = db_subnet_group_name
+
+        database_name = self.get_database_name()
+        if database_name:
+            not_null_args["DatabaseName"] = database_name
 
-        # create a dict of args which are not null, otherwise aws type validation fails
-        not_null_args: Dict[str, Any] = {}
         if self.availability_zones:
             not_null_args["AvailabilityZones"] = self.availability_zones
         if self.backup_retention_period:
             not_null_args["BackupRetentionPeriod"] = self.backup_retention_period
         if self.character_set_name:
             not_null_args["CharacterSetName"] = self.character_set_name
 
-        database_name = self.get_database_name()
-        if database_name:
-            not_null_args["DatabaseName"] = database_name
-
         if self.db_cluster_parameter_group_name:
             not_null_args[
                 "DBClusterParameterGroupName"
             ] = self.db_cluster_parameter_group_name
 
-        if vpc_security_group_ids is not None:
-            not_null_args["VpcSecurityGroupIds"] = vpc_security_group_ids
-        if db_subnet_group_name is not None:
-            not_null_args["DBSubnetGroupName"] = db_subnet_group_name
-
         if self.engine_version:
             not_null_args["EngineVersion"] = self.engine_version
         if self.port:
             not_null_args["Port"] = self.port
 
         master_username = self.get_master_username()
         if master_username:
@@ -423,28 +439,28 @@
         if self.network_type:
             not_null_args["NetworkType"] = self.network_type
         if self.db_system_id:
             not_null_args["DBSystemId"] = self.db_system_id
         if self.source_region:
             not_null_args["SourceRegion"] = self.source_region
 
-        # Step 3: Create DbCluster
+        # Step 3: Create DBCluster
         service_client = self.get_service_client(aws_client)
         try:
             create_response = service_client.create_db_cluster(
                 DBClusterIdentifier=self.get_db_cluster_identifier(),
                 Engine=self.engine,
                 **not_null_args,
             )
             logger.debug(f"DbCluster: {create_response}")
             database_dict = create_response.get("DBCluster", {})
 
             # Validate database creation
             if database_dict is not None:
-                print_info(f"DbCluster created: {self.get_db_cluster_identifier()}")
+                print_info(f"DBCluster created: {self.get_db_cluster_identifier()}")
                 self.active_resource = create_response
                 return True
         except Exception as e:
             print_error(f"{self.get_resource_type()} could not be created.")
             print_error(e)
         return False
 
@@ -452,15 +468,15 @@
         db_instances_created = []
         if self.db_instances is not None:
             for db_instance in self.db_instances:
                 db_instance.db_cluster_identifier = self.get_db_cluster_identifier()
                 if db_instance._create(aws_client):  # type: ignore
                     db_instances_created.append(db_instance)
 
-        # Wait for DbCluster to be created
+        # Wait for DBCluster to be created
         if self.wait_for_creation:
             try:
                 print_info(f"Waiting for {self.get_resource_type()} to be active.")
                 waiter = self.get_service_client(aws_client).get_waiter(
                     "db_cluster_available"
                 )
                 waiter.wait(
@@ -569,7 +585,158 @@
                         "MaxAttempts": self.waiter_max_attempts,
                     },
                 )
             except Exception as e:
                 print_error("Waiter failed.")
                 print_error(e)
         return True
+
+    def _update(self, aws_client: AwsApiClient) -> bool:
+        """Updates the DbCluster"""
+
+        print_info(f"Updating {self.get_resource_type()}: {self.get_resource_name()}")
+
+        # create a dict of args which are not null, otherwise aws type validation fails
+        not_null_args: Dict[str, Any] = {}
+
+        # Step 1: Get the VpcSecurityGroupIds
+        vpc_security_group_ids = self.vpc_security_group_ids
+        if vpc_security_group_ids is None and self.vpc_stack is not None:
+            vpc_stack_sg = self.vpc_stack.get_security_group(aws_client=aws_client)
+            if vpc_stack_sg is not None:
+                logger.debug(f"Using SecurityGroup: {vpc_stack_sg}")
+                vpc_security_group_ids = [vpc_stack_sg]
+        if vpc_security_group_ids is None and self.db_security_groups is not None:
+            sg_ids = []
+            for sg in self.db_security_groups:
+                sg_id = sg.get_security_group_id(aws_client)
+                if sg_id is not None:
+                    sg_ids.append(sg_id)
+            if len(sg_ids) > 0:
+                vpc_security_group_ids = sg_ids
+                logger.debug(f"Using SecurityGroups: {vpc_security_group_ids}")
+        if vpc_security_group_ids is not None:
+            not_null_args["VpcSecurityGroupIds"] = vpc_security_group_ids
+
+        if self.new_db_cluster_identifier:
+            not_null_args["NewDBClusterIdentifier"] = self.new_db_cluster_identifier
+        if self.apply_immediately:
+            not_null_args["ApplyImmediately"] = self.apply_immediately
+        if self.backup_retention_period:
+            not_null_args["BackupRetentionPeriod"] = self.backup_retention_period
+        if self.db_cluster_parameter_group_name:
+            not_null_args[
+                "DBClusterParameterGroupName"
+            ] = self.db_cluster_parameter_group_name
+        if self.port:
+            not_null_args["Port"] = self.port
+
+        master_user_password = self.get_master_user_password()
+        if master_user_password:
+            not_null_args["MasterUserPassword"] = master_user_password
+
+        if self.option_group_name:
+            not_null_args["OptionGroupName"] = self.option_group_name
+        if self.preferred_backup_window:
+            not_null_args["PreferredBackupWindow"] = self.preferred_backup_window
+        if self.preferred_maintenance_window:
+            not_null_args[
+                "PreferredMaintenanceWindow"
+            ] = self.preferred_maintenance_window
+        if self.enable_iam_database_authentication:
+            not_null_args[
+                "EnableIAMDbClusterAuthentication"
+            ] = self.enable_iam_database_authentication
+        if self.backtrack_window:
+            not_null_args["BacktrackWindow"] = self.backtrack_window
+        if self.cloudwatch_logs_exports:
+            not_null_args[
+                "CloudwatchLogsExportConfiguration"
+            ] = self.cloudwatch_logs_exports
+        if self.engine_version:
+            not_null_args["EngineVersion"] = self.engine_version
+        if self.allow_major_version_upgrade:
+            not_null_args["AllowMajorVersionUpgrade"] = self.allow_major_version_upgrade
+        if self.db_instance_parameter_group_name:
+            not_null_args[
+                "DBInstanceParameterGroupName"
+            ] = self.db_instance_parameter_group_name
+        if self.domain:
+            not_null_args["Domain"] = self.domain
+        if self.domain_iam_role_name:
+            not_null_args["DomainIAMRoleName"] = self.domain_iam_role_name
+        if self.scaling_configuration:
+            not_null_args["ScalingConfiguration"] = self.scaling_configuration
+        if self.deletion_protection:
+            not_null_args["DeletionProtection"] = self.deletion_protection
+        if self.enable_http_endpoint:
+            not_null_args["EnableHttpEndpoint"] = self.enable_http_endpoint
+        if self.copy_tags_to_snapshot:
+            not_null_args["CopyTagsToSnapshot"] = self.copy_tags_to_snapshot
+        if self.enable_global_write_forwarding:
+            not_null_args[
+                "EnableGlobalWriteForwarding"
+            ] = self.enable_global_write_forwarding
+        if self.db_instance_class:
+            not_null_args["DBClusterInstanceClass"] = self.db_instance_class
+        if self.allocated_storage:
+            not_null_args["AllocatedStorage"] = self.allocated_storage
+        if self.storage_type:
+            not_null_args["StorageType"] = self.storage_type
+        if self.iops:
+            not_null_args["Iops"] = self.iops
+        if self.auto_minor_version_upgrade:
+            not_null_args["AutoMinorVersionUpgrade"] = self.auto_minor_version_upgrade
+        if self.monitoring_interval:
+            not_null_args["MonitoringInterval"] = self.monitoring_interval
+        if self.monitoring_role_arn:
+            not_null_args["MonitoringRoleArn"] = self.monitoring_role_arn
+        if self.enable_performance_insights:
+            not_null_args[
+                "EnablePerformanceInsights"
+            ] = self.enable_performance_insights
+        if self.performance_insights_kms_key_id:
+            not_null_args[
+                "PerformanceInsightsKMSKeyId"
+            ] = self.performance_insights_kms_key_id
+        if self.performance_insights_retention_period:
+            not_null_args[
+                "PerformanceInsightsRetentionPeriod"
+            ] = self.performance_insights_retention_period
+        if self.serverless_v2_scaling_configuration:
+            not_null_args[
+                "ServerlessV2ScalingConfiguration"
+            ] = self.serverless_v2_scaling_configuration
+        if self.network_type:
+            not_null_args["NetworkType"] = self.network_type
+        if self.manage_master_user_password:
+            not_null_args["ManageMasterUserPassword"] = self.manage_master_user_password
+        if self.rotate_master_user_password:
+            not_null_args["RotateMasterUserPassword"] = self.rotate_master_user_password
+        if self.master_iser_secter_kms_key_id:
+            not_null_args[
+                "MasterUserSecretKmsKeyId"
+            ] = self.master_iser_secter_kms_key_id
+        if self.engine_mode:
+            not_null_args["EngineMode"] = self.engine_mode
+        if self.allow_engine_mode_change:
+            not_null_args["AllowEngineModeChange"] = self.allow_engine_mode_change
+
+        # Step 2: Update DBCluster
+        service_client = self.get_service_client(aws_client)
+        try:
+            update_response = service_client.modify_db_cluster(
+                DBClusterIdentifier=self.get_db_cluster_identifier(),
+                **not_null_args,
+            )
+            logger.debug(f"DBCluster: {update_response}")
+            resource_dict = update_response.get("DBCluster", {})
+
+            # Validate resource update
+            if resource_dict is not None:
+                print_info(f"DBCluster updated: {self.get_resource_name()}")
+                self.active_resource = update_response
+                return True
+        except Exception as e:
+            print_error(f"{self.get_resource_type()} could not be updated.")
+            print_error(e)
+        return False
```

### Comparing `phidata-1.6.9/phidata/aws/resource/rds/db_instance.py` & `phidata-1.7.0/phidata/table/s3/s3_table.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,486 +1,583 @@
-from pathlib import Path
-from typing import Optional, Any, Dict, List, Literal, Union
+from typing import Optional, Any, List, Dict
+from typing_extensions import Literal
 
-from phidata.aws.api_client import AwsApiClient
-from phidata.aws.resource.base import AwsResource
-from phidata.aws.resource.cloudformation.stack import CloudFormationStack
-from phidata.aws.resource.rds.db_subnet_group import DbSubnetGroup
-from phidata.utils.cli_console import print_info, print_error, print_warning
+from phidata.asset.aws.aws_asset import AwsAsset, AwsAssetArgs
+from phidata.checks.check import Check
+from phidata.aws.resource.s3.bucket import S3Bucket
+from phidata.utils.enums import ExtendedEnum
 from phidata.utils.log import logger
 
 
-class DbInstance(AwsResource):
-    """
-    # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html
+class S3TableFormat(ExtendedEnum):
+    CSV = "csv"
+    IPC = "ipc"
+    ARROW = "arrow"
+    FEATHER = "feather"
+    ORC = "orc"
+    PARQUET = "parquet"
 
-    The DBInstance can be an RDS DB instance, or it can be a DB instance in an Aurora DB cluster.
-    """
 
-    resource_type = "DbInstance"
-    service_name = "rds"
-
-    # Name of the db instance.
+class S3TableArgs(AwsAssetArgs):
+    # Table Name
     name: str
-    # The name of the database engine to be used for this instance.
-    engine: Union[
-        str,
-        Literal[
-            "aurora",
-            "aurora-mysql",
-            "aurora-postgresql",
-            "custom-oracle-ee",
-            "custom-sqlserver-ee",
-            "custom-sqlserver-se",
-            "custom-sqlserver-web",
-            "mariadb",
-            "mysql",
-            "oracle-ee",
-            "oracle-ee-cdb",
-            "oracle-se2",
-            "oracle-se2-cdb",
-            "postgres",
-            "sqlserver-ee",
-            "sqlserver-se",
-            "sqlserver-ex",
-            "sqlserver-web",
-        ],
-    ]
-    # Compute and memory capacity of the DB instance, for example db.m5.large.
-    db_instance_class: Optional[str] = None
-
-    # This is the name of the database to create when the DB instance is created.
-    # Note: The meaning of this parameter differs according to the database engine you use.
-    # Provide DB_NAME here or as DB_NAME in secrets_file
-    db_name: Optional[str] = None
-    # The DB instance identifier. This parameter is stored as a lowercase string.
-    # If None, use the name as the db_instance_identifier
-    # Constraints:
-    # - Must contain from 1 to 63 letters, numbers, or hyphens.
-    # - First character must be a letter.
-    # - Can't end with a hyphen or contain two consecutive hyphens.
-    db_instance_identifier: Optional[str] = None
-    # The amount of storage in gibibytes (GiB) to allocate for the DB instance.
-    allocated_storage: Optional[int] = None
-
-    # The name for the master user.
-    # Provide MASTER_USERNAME here or as MASTER_USERNAME in secrets_file
-    master_username: Optional[str] = None
-    # The password for the master user.
-    # The password can include any printable ASCII character except "/", """, or "@".
-    # Provide MASTER_USER_PASSWORD here or as MASTER_USER_PASSWORD in secrets_file
-    master_user_password: Optional[str] = None
-    # Read secrets from a file in yaml format
-    secrets_file: Optional[Path] = None
-
-    # A list of DB security groups to associate with this DB instance.
-    # This setting applies to the legacy EC2-Classic platform, which no longer creates new DB instances.
-    # Use the VpcSecurityGroupIds setting instead.
-    db_security_groups: Optional[List[str]] = None
-    # A list of Amazon EC2 VPC security groups to associate with this DB instance.
-    vpc_security_group_ids: Optional[List[str]] = None
-    # If vpc_security_group_ids is None,
-    # Read the security_group_id from vpc_stack
-    vpc_stack: Optional[CloudFormationStack] = None
-
-    # The Availability Zone (AZ) where the database will be created.
-    availability_zone: Optional[str] = None
-    # A DB subnet group to associate with this DB instance.
-    db_subnet_group_name: Optional[str] = None
-    # If db_subnet_group_name is None,
-    # Read the db_subnet_group_name from db_subnet_group
-    db_subnet_group: Optional[DbSubnetGroup] = None
-
-    # The time range each week during which system maintenance can occur, in Universal Coordinated Time (UTC).
-    preferred_maintenance_window: Optional[str] = None
-    # The name of the DB parameter group to associate with this DB instance.
-    db_parameter_group_name: Optional[str] = None
-    backup_retention_period: Optional[int] = None
-    preferred_backup_window: Optional[str] = None
-    # The port number on which the database accepts connections.
-    port: Optional[int] = None
-    # A value that indicates whether the DB instance is a Multi-AZ deployment.
-    # You can't set the AvailabilityZone parameter if the DB instance is a Multi-AZ deployment.
-    multi_az: Optional[bool] = None
-    # The version number of the database engine to use.
-    engine_version: Optional[str] = None
-    auto_minor_version_upgrade: Optional[bool] = None
-    license_model: Optional[str] = None
-    iops: Optional[int] = None
-    option_group_name: Optional[str] = None
-    character_set_name: Optional[str] = None
-    nchar_character_set_name: Optional[str] = None
-    # A value that indicates whether the DB instance is publicly accessible.
-    # When the DB instance is publicly accessible, its Domain Name System (DNS) endpoint resolves to the private IP
-    # from within the DB instance's virtual private cloud (VPC). It resolves to the public IP address from outside
-    # the DB instance's VPC. Access to the DB instance is ultimately controlled by the security group it uses.
-    # That public access is not permitted if the security group assigned to the DB instance doesn't permit it.
-    #
-    # When the DB instance isn't publicly accessible, it is an internal DB instance with a DNS name that resolves
-    # to a private IP address.
-    publicly_accessible: Optional[bool] = None
-    tags: Optional[List[Dict[str, str]]] = None
-    # The identifier of the DB cluster that the instance will belong to.
-    db_cluster_identifier: Optional[str] = None
-    # Specifies the storage type to be associated with the DB instance.
-    # Valid values: gp2 | gp3 | io1 | standard
-    # If you specify io1 or gp3 , you must also include a value for the Iops parameter.
-    # Default: io1 if the Iops parameter is specified, otherwise gp2
-    storage_type: Optional[str] = None
-    tde_credential_arn: Optional[str] = None
-    tde_credential_password: Optional[str] = None
-    storage_encrypted: Optional[bool] = None
-    kms_key_id: Optional[str] = None
-    domain: Optional[str] = None
-    copy_tags_to_snapshot: Optional[bool] = None
-    monitoring_interval: Optional[int] = None
-    monitoring_role_arn: Optional[str] = None
-    domain_iamrole_name: Optional[str] = None
-    promotion_tier: Optional[int] = None
-    timezone: Optional[str] = None
-    enable_iamdatabase_authentication: Optional[bool] = None
-    enable_performance_insights: Optional[bool] = None
-    performance_insights_kmskey_id: Optional[str] = None
-    performance_insights_retention_period: Optional[int] = None
-    enable_cloudwatch_logs_exports: Optional[List[str]] = None
-    processor_features: Optional[List[Dict[str, str]]] = None
-    # A value that indicates whether the DB instance has deletion protection enabled. The database can't be deleted
-    # when deletion protection is enabled. By default, deletion protection isn't enabled.
-    deletion_protection: Optional[bool] = None
-    # The upper limit in gibibytes (GiB) to which Amazon RDS can automatically scale the storage of the DB instance.
-    max_allocated_storage: Optional[int] = None
-    enable_customer_owned_ip: Optional[bool] = None
-    custom_iam_instance_profile: Optional[str] = None
-    backup_target: Optional[str] = None
-    network_type: Optional[str] = None
-    storage_throughput: Optional[int] = None
-
-    # Skip the creation of a final DB cluster snapshot before the DB cluster is deleted.
-    # If skip_final_snapshot = True, no DB cluster snapshot is created.
-    # If skip_final_snapshot = None, a DB cluster snapshot is created before the DB cluster is deleted.
-    #
-    # You must specify a FinalDBSnapshotIdentifier parameter
-    # if skip_final_snapshot = None.
-    skip_final_snapshot: Optional[bool] = True
-    final_db_snapshot_identifier: Optional[str] = None
-
-    # Cache secret_data
-    cached_secret_data: Optional[Dict[str, Any]] = None
-
-    def get_db_instance_identifier(self):
-        return self.db_instance_identifier or self.name
-
-    def get_secret_data(self) -> Optional[Dict[str, str]]:
-        if self.cached_secret_data is not None:
-            return self.cached_secret_data
-
-        if self.secrets_file is not None:
-            self.cached_secret_data = self.read_yaml_file(self.secrets_file)
-        return self.cached_secret_data
-
-    def get_master_username(self) -> Optional[str]:
-        master_username = self.master_username
-        if master_username is None and self.secrets_file is not None:
-            # read from secrets_file
-            secret_data = self.get_secret_data()
-            if secret_data is not None:
-                master_username = secret_data.get("MASTER_USERNAME", master_username)
-        return master_username
-
-    def get_master_user_password(self) -> Optional[str]:
-        master_user_password = self.master_user_password
-        if master_user_password is None and self.secrets_file is not None:
-            # read from secrets_file
-            secret_data = self.get_secret_data()
-            if secret_data is not None:
-                master_user_password = secret_data.get(
-                    "MASTER_USER_PASSWORD", master_user_password
+    # Table Format
+    table_format: S3TableFormat
+    # Database for the table
+    database: str = "default"
+
+    # -*- Table Path
+    # S3 Bucket
+    bucket: Optional[S3Bucket] = None
+    # S3 Bucket Name must be provided if bucket is not provided
+    bucket_name: Optional[str] = None
+    # Path to table directory in bucket. Without the s3:// prefix
+    path: Optional[str] = None
+    # To level directory for all tables
+    top_level_dir: Optional[str] = None
+    # A template string used to generate basenames of written data files.
+    # The token ‘{i}’ will be replaced with an automatically incremented integer.
+    # If not specified, it defaults to “part-{i}.” + format.default_extname
+    basename_template: Optional[str] = None
+
+    # List of partition columns
+    partitions: Optional[List[str]] = None
+
+    # Maximum number of partitions any batch may be written into.
+    max_partitions: Optional[int] = None
+    # If greater than 0 then this will limit the maximum number of files that can be left open.
+    # If an attempt is made to open too many files then the least recently used file will be closed.
+    # If this setting is set too low you may end up fragmenting your data into many small files.
+    max_open_files: Optional[int] = None
+    # Maximum number of rows per file. If greater than 0 then this will limit how many rows are placed in any single
+    # file. Otherwise there will be no limit and one file will be created in each output directory unless files need
+    # to be closed to respect max_open_files
+    max_rows_per_file: Optional[int] = None
+    # Minimum number of rows per group. When the value is greater than 0, the dataset writer will batch incoming data
+    # and only write the row groups to the disk when sufficient rows have accumulated.
+    min_rows_per_group: Optional[int] = None
+    # Maximum number of rows per group. If the value is greater than 0, then the dataset writer may split up large
+    # incoming batches into multiple row groups. If this value is set, then min_rows_per_group should also be set.
+    # Otherwise it could end up with very small row groups.
+    max_rows_per_group: Optional[int] = None
+    # Controls how the dataset will handle data that already exists in the destination.
+    # The default behavior (‘error’) is to raise an error if any data exists in the destination.
+    # ‘overwrite_or_ignore’ will ignore any existing data and will overwrite files with the same name
+    # as an output file. Other existing files will be ignored. This behavior, in combination with a unique
+    # basename_template for each write, will allow for an append workflow.
+    # ‘delete_matching’ is useful when you are writing a partitioned dataset.
+    # The first time each partition directory is encountered the entire directory will be deleted.
+    # This allows you to overwrite old partitions completely.
+    write_mode: Literal[
+        "delete_matching", "overwrite_or_ignore", "error"
+    ] = "delete_matching"
+
+
+class S3Table(AwsAsset):
+    """Base Class for S3 tables"""
+
+    def __init__(
+        self,
+        # Table Name: required
+        name: str,
+        # Table Format: required
+        table_format: S3TableFormat,
+        # Database for the table
+        database: str = "default",
+        # DataModel for this table
+        data_model: Optional[Any] = None,
+        # Checks to run before reading from disk
+        read_checks: Optional[List[Check]] = None,
+        # Checks to run before writing to disk
+        write_checks: Optional[List[Check]] = None,
+        # -*- Table Path
+        # S3 Bucket
+        bucket: Optional[S3Bucket] = None,
+        # S3 Bucket Name
+        bucket_name: Optional[str] = None,
+        # Path to table directory in bucket. Without the s3:// prefix
+        path: Optional[str] = None,
+        # To level directory for all tables
+        top_level_dir: Optional[str] = "tables",
+        # A template string used to generate basenames of written data files.
+        # The token ‘{i}’ will be replaced with an automatically incremented integer.
+        # If not specified, it defaults to “part-{i}.” + format.default_extname
+        basename_template: Optional[str] = None,
+        # List of partition columns
+        partitions: Optional[List[str]] = None,
+        # Maximum number of partitions any batch may be written into.
+        max_partitions: Optional[int] = None,
+        # If greater than 0 then this will limit the maximum number of files that can be left open.
+        # If an attempt is made to open too many files then the least recently used file will be closed.
+        # If this setting is set too low you may end up fragmenting your data into many small files.
+        max_open_files: Optional[int] = None,
+        # Maximum number of rows per file. If greater than 0 then this will limit how many rows are placed in any single
+        # file. Otherwise there will be no limit and one file will be created in each output directory unless files need
+        # to be closed to respect max_open_files
+        max_rows_per_file: Optional[int] = None,
+        # Minimum number of rows per group. When the value is greater than 0, the dataset writer will batch incoming data
+        # and only write the row groups to the disk when sufficient rows have accumulated.
+        min_rows_per_group: Optional[int] = None,
+        # Maximum number of rows per group. If the value is greater than 0, then the dataset writer may split up large
+        # incoming batches into multiple row groups. If this value is set, then min_rows_per_group should also be set.
+        # Otherwise it could end up with very small row groups.
+        max_rows_per_group: Optional[int] = None,
+        # Controls how the dataset will handle data that already exists in the destination.
+        # The default behavior (‘error’) is to raise an error if any data exists in the destination.
+        # ‘overwrite_or_ignore’ will ignore any existing data and will overwrite files with the same name
+        # as an output file. Other existing files will be ignored. This behavior, in combination with a unique
+        # basename_template for each write, will allow for an append workflow.
+        # ‘delete_matching’ is useful when you are writing a partitioned dataset.
+        # The first time each partition directory is encountered the entire directory will be deleted.
+        # This allows you to overwrite old partitions completely.
+        write_mode: Literal[
+            "delete_matching", "overwrite_or_ignore", "error"
+        ] = "delete_matching",
+        version: Optional[str] = None,
+        enabled: bool = True,
+        **kwargs,
+    ) -> None:
+        super().__init__()
+        try:
+            self.args: S3TableArgs = S3TableArgs(
+                name=name,
+                table_format=table_format,
+                database=database,
+                data_model=data_model,
+                read_checks=read_checks,
+                write_checks=write_checks,
+                bucket=bucket,
+                bucket_name=bucket_name,
+                path=path,
+                top_level_dir=top_level_dir,
+                basename_template=basename_template,
+                partitions=partitions,
+                max_partitions=max_partitions,
+                max_open_files=max_open_files,
+                max_rows_per_file=max_rows_per_file,
+                min_rows_per_group=min_rows_per_group,
+                max_rows_per_group=max_rows_per_group,
+                write_mode=write_mode,
+                version=version,
+                enabled=enabled,
+                **kwargs,
+            )
+        except Exception as e:
+            logger.error(f"Args for {self.name} are not valid")
+            raise
+
+    @property
+    def table_format(self) -> Optional[S3TableFormat]:
+        return self.args.table_format if self.args else None
+
+    @table_format.setter
+    def table_format(self, table_format: S3TableFormat) -> None:
+        if self.args and table_format:
+            self.args.table_format = table_format
+
+    @property
+    def database(self) -> Optional[str]:
+        return self.args.database if self.args else None
+
+    @database.setter
+    def database(self, database: str) -> None:
+        if self.args and database:
+            self.args.database = database
+
+    @property
+    def bucket(self) -> Optional[S3Bucket]:
+        return self.args.bucket if self.args else None
+
+    @bucket.setter
+    def bucket(self, bucket: S3Bucket) -> None:
+        if self.args and bucket:
+            self.args.bucket = bucket
+
+    @property
+    def bucket_name(self) -> Optional[str]:
+        return self.args.bucket_name if self.args else None
+
+    @bucket_name.setter
+    def bucket_name(self, bucket_name: str) -> None:
+        if self.args and bucket_name:
+            self.args.bucket_name = bucket_name
+
+    @property
+    def path(self) -> Optional[str]:
+        return self.args.path if self.args else None
+
+    @path.setter
+    def path(self, path: str) -> None:
+        if self.args and path:
+            self.args.path = path
+
+    @property
+    def top_level_dir(self) -> Optional[str]:
+        return self.args.top_level_dir if self.args else None
+
+    @top_level_dir.setter
+    def top_level_dir(self, top_level_dir: str) -> None:
+        if self.args and top_level_dir:
+            self.args.top_level_dir = top_level_dir
+
+    @property
+    def basename_template(self) -> Optional[str]:
+        return self.args.basename_template if self.args else None
+
+    @basename_template.setter
+    def basename_template(self, basename_template: str) -> None:
+        if self.args and basename_template:
+            self.args.basename_template = basename_template
+
+    @property
+    def partitions(self) -> Optional[List[str]]:
+        return self.args.partitions if self.args else None
+
+    @partitions.setter
+    def partitions(self, partitions: List[str]) -> None:
+        if self.args and partitions:
+            self.args.partitions = partitions
+
+    @property
+    def max_partitions(self) -> Optional[int]:
+        return self.args.max_partitions if self.args else None
+
+    @max_partitions.setter
+    def max_partitions(self, max_partitions: int) -> None:
+        if self.args and max_partitions:
+            self.args.max_partitions = max_partitions
+
+    @property
+    def max_open_files(self) -> Optional[int]:
+        return self.args.max_open_files if self.args else None
+
+    @max_open_files.setter
+    def max_open_files(self, max_open_files: int) -> None:
+        if self.args and max_open_files:
+            self.args.max_open_files = max_open_files
+
+    @property
+    def max_rows_per_file(self) -> Optional[int]:
+        return self.args.max_rows_per_file if self.args else None
+
+    @max_rows_per_file.setter
+    def max_rows_per_file(self, max_rows_per_file: int) -> None:
+        if self.args and max_rows_per_file:
+            self.args.max_rows_per_file = max_rows_per_file
+
+    @property
+    def min_rows_per_group(self) -> Optional[int]:
+        return self.args.min_rows_per_group if self.args else None
+
+    @min_rows_per_group.setter
+    def min_rows_per_group(self, min_rows_per_group: int) -> None:
+        if self.args and min_rows_per_group:
+            self.args.min_rows_per_group = min_rows_per_group
+
+    @property
+    def max_rows_per_group(self) -> Optional[int]:
+        return self.args.max_rows_per_group if self.args else None
+
+    @max_rows_per_group.setter
+    def max_rows_per_group(self, max_rows_per_group: int) -> None:
+        if self.args and max_rows_per_group:
+            self.args.max_rows_per_group = max_rows_per_group
+
+    @property
+    def write_mode(
+        self,
+    ) -> Optional[Literal["delete_matching", "overwrite_or_ignore", "error"]]:
+        return self.args.write_mode if self.args else None
+
+    @write_mode.setter
+    def write_mode(
+        self, write_mode: Literal["delete_matching", "overwrite_or_ignore", "error"]
+    ) -> None:
+        if self.args and write_mode:
+            self.args.write_mode = write_mode
+
+    @property
+    def table_location(self) -> str:
+        if self.path is not None:
+            return self.path
+        else:
+            if self.bucket_name is not None:
+                return "{}/{}{}/{}".format(
+                    self.bucket_name,
+                    f"{self.top_level_dir}/" if self.top_level_dir else "",
+                    self.database,
+                    self.name,
+                )
+            if self.bucket is not None:
+                return "{}/{}{}/{}".format(
+                    self.bucket.name,
+                    f"{self.top_level_dir}/" if self.top_level_dir else "",
+                    self.database,
+                    self.name,
                 )
-        return master_user_password
+        return ""
 
-    def get_db_name(self) -> Optional[str]:
-        db_name = self.db_name
-        if db_name is None and self.secrets_file is not None:
-            # read from secrets_file
-            secret_data = self.get_secret_data()
-            if secret_data is not None:
-                db_name = secret_data.get("DB_NAME", db_name)
-                if db_name is None:
-                    db_name = secret_data.get("DATABASE_NAME", db_name)
-        return db_name
-
-    def get_database_name(self) -> Optional[str]:
-        # Alias for get_db_name because db_instances use `db_name` and db_clusters use `database_name`
-        return self.get_db_name()
+    ######################################################
+    ## Validate data asset
+    ######################################################
 
-    def _create(self, aws_client: AwsApiClient) -> bool:
-        """Creates the DbInstance
+    def is_valid(self) -> bool:
+        return True
 
-        Args:
-            aws_client: The AwsApiClient for the current cluster
+    ######################################################
+    ## Build data asset
+    ######################################################
+
+    def build(self) -> bool:
+        logger.debug(f"@build not defined for {self.name}")
+        return False
+
+    ######################################################
+    ## Write DataAsset
+    ######################################################
+
+    def write_table(self, table: Any, **write_options) -> bool:
         """
-        print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
+        Write pyarrow.Table to disk.
 
-        # Step 1: Get the VpcSecurityGroupIds
-        vpc_security_group_ids = self.vpc_security_group_ids
-        if vpc_security_group_ids is None and self.vpc_stack is not None:
-            vpc_stack_sg = self.vpc_stack.get_security_group(aws_client=aws_client)
-            if vpc_stack_sg is not None:
-                logger.debug(f"Using SecurityGroup: {vpc_stack_sg}")
-                vpc_security_group_ids = [vpc_stack_sg]
-
-        # Step 2: Get the DbSubnetGroupName
-        db_subnet_group_name = self.db_subnet_group_name
-        if db_subnet_group_name is None and self.db_subnet_group is not None:
-            db_subnet_group_name = self.db_subnet_group.name
-            logger.debug(f"Using DbSubnetGroup: {db_subnet_group_name}")
-
-        # create a dict of args which are not null, otherwise aws type validation fails
-        not_null_args: Dict[str, Any] = {}
-        db_name = self.get_db_name()
-        if db_name:
-            not_null_args["DBName"] = db_name
-
-        if self.allocated_storage:
-            not_null_args["AllocatedStorage"] = self.allocated_storage
-        if self.db_instance_class:
-            not_null_args["DBInstanceClass"] = self.db_instance_class
-
-        master_username = self.get_master_username()
-        if master_username:
-            not_null_args["MasterUsername"] = master_username
-        master_user_password = self.get_master_user_password()
-        if master_user_password:
-            not_null_args["MasterUserPassword"] = master_user_password
-
-        if self.db_security_groups is not None:
-            not_null_args["DBSecurityGroups"] = self.db_security_groups
-        if vpc_security_group_ids is not None:
-            not_null_args["VpcSecurityGroupIds"] = vpc_security_group_ids
-        if self.availability_zone is not None:
-            not_null_args["AvailabilityZone"] = self.availability_zone
-        if db_subnet_group_name is not None:
-            not_null_args["DBSubnetGroupName"] = db_subnet_group_name
-
-        if self.preferred_maintenance_window:
-            not_null_args[
-                "PreferredMaintenanceWindow"
-            ] = self.preferred_maintenance_window
-        if self.db_parameter_group_name:
-            not_null_args["DBParameterGroupName"] = self.db_parameter_group_name
-        if self.backup_retention_period:
-            not_null_args["BackupRetentionPeriod"] = self.backup_retention_period
-        if self.preferred_backup_window:
-            not_null_args["PreferredBackupWindow"] = self.preferred_backup_window
-        if self.port:
-            not_null_args["Port"] = self.port
-        if self.multi_az:
-            not_null_args["MultiAZ"] = self.multi_az
-        if self.engine_version:
-            not_null_args["EngineVersion"] = self.engine_version
-        if self.auto_minor_version_upgrade:
-            not_null_args["AutoMinorVersionUpgrade"] = self.auto_minor_version_upgrade
-        if self.license_model:
-            not_null_args["LicenseModel"] = self.license_model
-        if self.iops:
-            not_null_args["Iops"] = self.iops
-        if self.option_group_name:
-            not_null_args["OptionGroupName"] = self.option_group_name
-        if self.character_set_name:
-            not_null_args["CharacterSetName"] = self.character_set_name
-        if self.nchar_character_set_name:
-            not_null_args["NcharCharacterSetName"] = self.nchar_character_set_name
-        if self.publicly_accessible:
-            not_null_args["PubliclyAccessible"] = self.publicly_accessible
-        if self.tags:
-            not_null_args["Tags"] = self.tags
-        if self.db_cluster_identifier:
-            not_null_args["DBClusterIdentifier"] = self.db_cluster_identifier
-        if self.storage_type:
-            not_null_args["StorageType"] = self.storage_type
-        if self.tde_credential_arn:
-            not_null_args["TdeCredentialArn"] = self.tde_credential_arn
-        if self.tde_credential_password:
-            not_null_args["TdeCredentialPassword"] = self.tde_credential_password
-        if self.storage_encrypted:
-            not_null_args["StorageEncrypted"] = self.storage_encrypted
-        if self.kms_key_id:
-            not_null_args["KmsKeyId"] = self.kms_key_id
-        if self.domain:
-            not_null_args["Domain"] = self.domain
-        if self.copy_tags_to_snapshot:
-            not_null_args["CopyTagsToSnapshot"] = self.copy_tags_to_snapshot
-        if self.monitoring_interval:
-            not_null_args["MonitoringInterval"] = self.monitoring_interval
-        if self.monitoring_role_arn:
-            not_null_args["MonitoringRoleArn"] = self.monitoring_role_arn
-        if self.domain_iamrole_name:
-            not_null_args["DomainIAMRoleName"] = self.domain_iamrole_name
-        if self.promotion_tier:
-            not_null_args["PromotionTier"] = self.promotion_tier
-        if self.timezone:
-            not_null_args["Timezone"] = self.timezone
-        if self.enable_iamdatabase_authentication:
-            not_null_args[
-                "EnableIAMDatabaseAuthentication"
-            ] = self.enable_iamdatabase_authentication
-        if self.enable_performance_insights:
-            not_null_args[
-                "EnablePerformanceInsights"
-            ] = self.enable_performance_insights
-        if self.performance_insights_kmskey_id:
-            not_null_args[
-                "PerformanceInsightsKMSKeyId"
-            ] = self.performance_insights_kmskey_id
-        if self.performance_insights_retention_period:
-            not_null_args[
-                "PerformanceInsightsRetentionPeriod"
-            ] = self.performance_insights_retention_period
-        if self.enable_cloudwatch_logs_exports:
-            not_null_args[
-                "EnableCloudwatchLogsExports"
-            ] = self.enable_cloudwatch_logs_exports
-        if self.processor_features:
-            not_null_args["ProcessorFeatures"] = self.processor_features
-        if self.deletion_protection:
-            not_null_args["DeletionProtection"] = self.deletion_protection
-        if self.max_allocated_storage:
-            not_null_args["MaxAllocatedStorage"] = self.max_allocated_storage
-        if self.enable_customer_owned_ip:
-            not_null_args["EnableCustomerOwnedIp"] = self.enable_customer_owned_ip
-        if self.custom_iam_instance_profile:
-            not_null_args["CustomIamInstanceProfile"] = self.custom_iam_instance_profile
-        if self.backup_target:
-            not_null_args["BackupTarget"] = self.backup_target
-        if self.network_type:
-            not_null_args["NetworkType"] = self.network_type
-        if self.storage_throughput:
-            not_null_args["StorageThroughput"] = self.storage_throughput
+        https://arrow.apache.org/docs/python/generated/pyarrow.Table.html#pyarrow.Table
+        """
+        # Validate pyarrow is installed
+        try:
+            import pyarrow as pa
+            import pyarrow.dataset as ds
+        except ImportError as ie:
+            raise Exception(
+                f"PyArrow not installed. Please install with `pip install pyarrow`"
+            ) from ie
+
+        # Validate table
+        if table is None or not isinstance(table, pa.Table):
+            logger.error("Table invalid")
+            return False
+
+        # Check table_location is available
+        table_location = self.table_location
+        if table_location is None:
+            logger.error("Table location invalid")
+            return False
+
+        # Check S3FileSystem is available
+        fs = self._get_fs()
+        if fs is None:
+            logger.error("Could not create S3FileSystem")
+            return False
 
-        # Step 3: Create DbInstance
-        service_client = self.get_service_client(aws_client)
+        logger.debug("Format: {}".format(self.args.table_format.value))
         try:
-            create_response = service_client.create_db_instance(
-                DBInstanceIdentifier=self.get_db_instance_identifier(),
-                Engine=self.engine,
+            # Run write checks
+            if self.write_checks is not None:
+                for check in self.write_checks:
+                    if not check.check_table(table):
+                        return False
+
+            # Create a dict of args which are not null
+            not_null_args: Dict[str, Any] = {}
+            if self.args.basename_template is not None:
+                not_null_args["basename_template"] = self.args.basename_template
+            if self.args.partitions is not None:
+                not_null_args["partitioning"] = self.args.partitions
+                not_null_args["partitioning_flavor"] = "hive"
+                # cast partition keys to string
+                # ref: https://bneijt.nl/blog/write-polars-dataframe-as-parquet-dataset/
+                table = table.cast(
+                    pa.schema(
+                        [
+                            f.with_type(pa.string())
+                            if f.name in self.args.partitions
+                            else f
+                            for f in table.schema
+                        ]
+                    )
+                )
+            if self.args.max_partitions is not None:
+                not_null_args["max_partitions"] = self.args.max_partitions
+            if self.args.max_open_files is not None:
+                not_null_args["max_open_files"] = self.args.max_open_files
+            if self.args.max_rows_per_file is not None:
+                not_null_args["max_rows_per_file"] = self.args.max_rows_per_file
+            if self.args.min_rows_per_group is not None:
+                not_null_args["min_rows_per_group"] = self.args.min_rows_per_group
+            if self.args.max_rows_per_group is not None:
+                not_null_args["max_rows_per_group"] = self.args.max_rows_per_group
+
+            # Build file_options: FileFormat specific write options
+            # created using the FileFormat.make_write_options() function.
+            if write_options:
+                file_options = ds.FileFormat.make_write_options(**write_options)
+                not_null_args["file_options"] = file_options
+
+            # Write table to disk
+            ds.write_dataset(
+                table,
+                table_location,
+                format=self.args.table_format.value,
+                filesystem=fs,
+                existing_data_behavior=self.args.write_mode,
                 **not_null_args,
             )
-            logger.debug(f"DbInstance: {create_response}")
-            resource_dict = create_response.get("DBInstance", {})
+            logger.info(f"Table {self.name} written to {table_location}")
 
-            # Validate resource creation
-            if resource_dict is not None:
-                print_info(f"DbInstance created: {self.get_db_instance_identifier()}")
-                self.active_resource = create_response
-                return True
-        except Exception as e:
-            print_error(f"{self.get_resource_type()} could not be created.")
-            print_error(e)
+            return True
+        except Exception:
+            logger.error("Could not write table: {}".format(self.name))
+            raise
+
+    def write_polars_df(
+        self,
+        df: Optional[Any] = None,
+        options: Optional[Dict[str, Any]] = None,
+        **kwargs,
+    ) -> bool:
+        """
+        Write Polars DataFrame to disk.
+        """
+        # Validate polars is installed
+        try:
+            import polars as pl  # type: ignore
+        except ImportError as ie:
+            logger.error(f"Polars not installed: {ie}")
+            return False
+
+        # Validate df
+        if df is None or not isinstance(df, pl.DataFrame):
+            logger.error("DataFrame invalid")
+            return False
+
+        # Create arrow table and write to disk
+        return self.write_table(df.to_arrow(), options=options)
+
+    def write_pandas_df(self, df: Optional[Any] = None, **kwargs) -> bool:
+        logger.debug(f"@write_pandas_df not defined for {self.name}")
         return False
 
-    def post_create(self, aws_client: AwsApiClient) -> bool:
-        # Wait for DbInstance to be created
-        if self.wait_for_creation:
-            try:
-                print_info(f"Waiting for {self.get_resource_type()} to be active.")
-                waiter = self.get_service_client(aws_client).get_waiter(
-                    "db_instance_available"
-                )
-                waiter.wait(
-                    DBInstanceIdentifier=self.get_db_instance_identifier(),
-                    WaiterConfig={
-                        "Delay": self.waiter_delay,
-                        "MaxAttempts": self.waiter_max_attempts,
-                    },
-                )
-            except Exception as e:
-                print_error("Waiter failed.")
-                print_error(e)
+    ######################################################
+    ## Create DataAsset
+    ######################################################
+
+    def _create(self) -> bool:
+        logger.error(f"@_create not defined for {self.name}")
+        return False
+
+    def post_create(self) -> bool:
         return True
 
-    def _read(self, aws_client: AwsApiClient) -> Optional[Any]:
-        """Returns the DbInstance
+    ######################################################
+    ## Read DataAsset
+    ######################################################
 
-        Args:
-            aws_client: The AwsApiClient for the current cluster
+    def read_table(self, **read_options) -> Optional[Any]:
         """
-        logger.debug(f"Reading {self.get_resource_type()}: {self.get_resource_name()}")
+        Read pyarrow.Table from disk.
 
-        from botocore.exceptions import ClientError
+        https://arrow.apache.org/docs/python/generated/pyarrow.Table.html#pyarrow.Table
+        """
+        # Validate pyarrow is installed
+        try:
+            import pyarrow as pa
+            import pyarrow.dataset as ds
+        except ImportError as ie:
+            raise Exception(
+                f"PyArrow not installed. Please install with `pip install pyarrow`"
+            ) from ie
+
+        # Check table_location is available
+        table_location = self.table_location
+        if table_location is None:
+            logger.error("Table location invalid")
+            return False
+
+        # Check S3FileSystem is available
+        fs = self._get_fs()
+        if fs is None:
+            logger.error("Could not create S3FileSystem")
+            return False
 
-        service_client = self.get_service_client(aws_client)
+        logger.debug("Format: {}".format(self.args.table_format.value))
         try:
-            db_instance_identifier = self.get_db_instance_identifier()
-            describe_response = service_client.describe_db_instances(
-                DBInstanceIdentifier=db_instance_identifier
+            # Create a dict of args which are not null
+            not_null_args: Dict[str, Any] = {}
+            if self.args.partitions is not None:
+                not_null_args["partitioning"] = "hive"
+
+            # Read dataset from s3
+            # https://arrow.apache.org/docs/python/generated/pyarrow.dataset.dataset.html#pyarrow.dataset.dataset
+            # https://arrow.apache.org/docs/python/generated/pyarrow.dataset.Dataset.html#pyarrow.dataset.Dataset
+            dataset: ds.Dataset = ds.dataset(
+                table_location,
+                format=self.args.table_format.value,
+                filesystem=fs,
+                **not_null_args,
             )
-            logger.debug(f"DbInstance: {describe_response}")
-            resources_list = describe_response.get("DBInstances", None)
-
-            if resources_list is not None and isinstance(resources_list, list):
-                for _db_cluster in resources_list:
-                    _cluster_identifier = _db_cluster.get("DBInstanceIdentifier", None)
-                    if _cluster_identifier == db_instance_identifier:
-                        self.active_resource = _db_cluster
-                        break
-        except ClientError as ce:
-            logger.debug(f"ClientError: {ce}")
-        except Exception as e:
-            print_error(f"Error reading {self.get_resource_type()}.")
-            print_error(e)
-        return self.active_resource
 
-    def _delete(self, aws_client: AwsApiClient) -> bool:
-        """Deletes the DbInstance
+            # Convert dataset to table
+            # https://arrow.apache.org/docs/python/generated/pyarrow.dataset.Dataset.html#pyarrow.dataset.Dataset.to_table
+            table: pa.Table = dataset.to_table(**read_options)
+
+            # Run read checks
+            if self.read_checks is not None:
+                for check in self.read_checks:
+                    if not check.check_table(table):
+                        return None
+
+            return table
+        except Exception:
+            logger.error("Could not read table: {}".format(self.name))
+            raise
+
+    def read_polars_df(
+        self, options: Optional[Dict[str, Any]] = None, **kwargs
+    ) -> Optional[Any]:
+        """
+        Read Polars DataFrame from disk.
 
-        Args:
-            aws_client: The AwsApiClient for the current cluster
+        options: Dict[str, Any]
+            Additional options to pass to the reader.
+            More info:
+                https://arrow.apache.org/docs/python/generated/pyarrow.dataset.Scanner.html#pyarrow.dataset.Scanner.from_dataset
+                https://arrow.apache.org/docs/python/generated/pyarrow.dataset.dataset.html#pyarrow.dataset.dataset.to_table
         """
-        print_info(f"Deleting {self.get_resource_type()}: {self.get_resource_name()}")
+        # Validate polars is installed
+        try:
+            import polars as pl
+        except ImportError as ie:
+            logger.error(f"Polars not installed: {ie}")
+            return None
+
+        # Convert table to polars DataFrame
+        # https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.from_arrow.html
+        return pl.from_arrow(self.read_table(options=options))
 
-        service_client = self.get_service_client(aws_client)
-        self.active_resource = None
+    def read_pandas_df(self, **kwargs) -> Optional[Any]:
+        logger.debug(f"@read_pandas_df not defined for {self.name}")
+        return False
 
-        # create a dict of args which are not null, otherwise aws type validation fails
-        not_null_args: Dict[str, Any] = {}
-        if self.final_db_snapshot_identifier:
-            not_null_args[
-                "FinalDBSnapshotIdentifier"
-            ] = self.final_db_snapshot_identifier
+    def _read(self) -> Any:
+        logger.error(f"@_read not defined for {self.name}")
+        return False
 
-        try:
-            db_instance_identifier = self.get_db_instance_identifier()
-            delete_response = service_client.delete_db_instance(
-                DBInstanceIdentifier=db_instance_identifier,
-                SkipFinalSnapshot=self.skip_final_snapshot,
-                **not_null_args,
-            )
-            logger.debug(f"Delete Response: {delete_response}")
-            print_info(
-                f"{self.get_resource_type()}: {self.get_resource_name()} deleted"
-            )
-            return True
-        except Exception as e:
-            print_error(f"{self.get_resource_type()} could not be deleted.")
-            print_error("Please try again or delete resources manually.")
-            print_error(e)
+    ######################################################
+    ## Update DataAsset
+    ######################################################
+
+    def _update(self) -> Any:
+        logger.error(f"@_update not defined for {self.name}")
         return False
 
-    def post_delete(self, aws_client: AwsApiClient) -> bool:
-        # Wait for DbInstance to be deleted
-        if self.wait_for_deletion:
-            try:
-                print_info(f"Waiting for {self.get_resource_type()} to be deleted.")
-                waiter = self.get_service_client(aws_client).get_waiter(
-                    "db_instance_deleted"
-                )
-                waiter.wait(
-                    DBInstanceIdentifier=self.get_db_instance_identifier(),
-                    WaiterConfig={
-                        "Delay": self.waiter_delay,
-                        "MaxAttempts": self.waiter_max_attempts,
-                    },
-                )
-            except Exception as e:
-                print_error("Waiter failed.")
-                print_error(e)
+    def post_update(self) -> bool:
+        return True
+
+    ######################################################
+    ## Delete DataAsset
+    ######################################################
+
+    def _delete(self) -> Any:
+        logger.error(f"@_delete not defined for {self.name}")
+        return False
+
+    def post_delete(self) -> bool:
         return True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `phidata-1.6.9/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-1.7.0/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files 24% similar despite different names*

```diff
@@ -149,7 +149,44 @@
             )
             return True
         except Exception as e:
             print_error(f"{self.get_resource_type()} could not be deleted.")
             print_error("Please try again or delete resources manually.")
             print_error(e)
         return False
+
+    def _update(self, aws_client: AwsApiClient) -> bool:
+        subnet_ids = self.subnet_ids
+        if subnet_ids is None and self.vpc_stack is not None:
+            subnet_ids = []
+            logger.debug("Getting public subnet_ids from vpc stack")
+            public_subnet_ids = self.vpc_stack.get_private_subnets(
+                aws_client=aws_client
+            )
+            if public_subnet_ids is not None:
+                subnet_ids.extend(public_subnet_ids)
+            logger.debug("Getting private subnet_ids from vpc stack")
+            private_subnet_ids = self.vpc_stack.get_private_subnets(
+                aws_client=aws_client
+            )
+            if private_subnet_ids is not None:
+                subnet_ids.extend(private_subnet_ids)
+
+        service_client = self.get_service_client(aws_client)
+        try:
+            update_response = service_client.modify_db_subnet_group(
+                DBSubnetGroupName=self.name,
+                DBSubnetGroupDescription=self.description or f"Created for {self.name}",
+                SubnetIds=self.subnet_ids,
+            )
+            logger.debug(f"Response: {update_response}")
+            resource_dict = update_response.get("DBSubnetGroup", {})
+
+            # Validate resource update
+            if resource_dict is not None:
+                print_info(f"DBSubnetGroup updated: {self.get_resource_name()}")
+                self.active_resource = resource_dict
+                return True
+        except Exception as e:
+            print_error(f"{self.get_resource_type()} could not be updated.")
+            print_error(e)
+        return False
```

### Comparing `phidata-1.6.9/phidata/aws/resource/s3/bucket.py` & `phidata-1.7.0/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/resource/secret/manager.py` & `phidata-1.7.0/phidata/aws/resource/secret/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+import json
 from pathlib import Path
-from typing import Optional, Any, Dict, List, Union
+from typing import Optional, Any, Dict, List
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
 from phidata.utils.cli_console import print_info, print_error
 from phidata.utils.log import logger
 
 
 class SecretsManager(AwsResource):
     """
-    # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html
+    Reference: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html
     """
 
-    resource_type = "SecretsManager"
+    resource_type = "Secret"
     service_name = "secretsmanager"
 
-    # The name of the new secret.
+    # The name of the secret.
     name: str
     client_request_token: Optional[str] = None
     # The description of the secret.
     description: Optional[str] = None
     kms_key_id: Optional[str] = None
     # The binary data to encrypt and store in the new version of the secret.
     # We recommend that you store your binary data in a file and then pass the contents of the file as a parameter.
@@ -38,55 +39,62 @@
     # Read secret key/value pairs from yaml files
     secret_files: Optional[List[Path]] = None
     # Read secret key/value pairs from yaml files in a directory
     secrets_dir: Optional[Path] = None
     # Force delete the secret without recovery
     force_delete: Optional[bool] = True
 
-    # provided by api on create
+    # Provided by api on create
     secret_arn: Optional[str] = None
-    secret_resource_name: Optional[str] = None
+    secret_name: Optional[str] = None
     secret_value: Optional[dict] = None
 
-    def _create(self, aws_client: AwsApiClient) -> bool:
-        """Creates the SecretsManager
-
-        Args:
-            aws_client: The AwsApiClient for the current secret
-        """
-        print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
+    cached_secret: Optional[Dict[str, Any]] = None
 
-        # Step 1: Read secrets from files
+    def read_secrets_from_files(self) -> Dict[str, Any]:
+        """Reads secrets from files"""
         secret_dict: Dict[str, Any] = {}
         if self.secret_files:
             for f in self.secret_files:
                 _s = self.read_yaml_file(f)
-                if _s:
+                if _s is not None:
                     secret_dict.update(_s)
         if self.secrets_dir:
             for f in self.secrets_dir.glob("*.yaml"):
                 _s = self.read_yaml_file(f)
-                if _s:
+                if _s is not None:
                     secret_dict.update(_s)
             for f in self.secrets_dir.glob("*.yml"):
                 _s = self.read_yaml_file(f)
-                if _s:
+                if _s is not None:
                     secret_dict.update(_s)
+        return secret_dict
+
+    def _create(self, aws_client: AwsApiClient) -> bool:
+        """Creates the SecretsManager
 
-        secret_string = self.secret_string
-        if secret_dict:
-            import json
+        Args:
+            aws_client: The AwsApiClient for the current secret
+        """
+        print_info(f"Creating {self.get_resource_type()}: {self.get_resource_name()}")
 
-            if secret_string:
-                secret_dict.update(json.loads(secret_string))
+        # Step 1: Read secrets from files
+        secret_dict: Dict[str, Any] = self.read_secrets_from_files()
 
-            secret_string = json.dumps(secret_dict)
-            logger.debug(f"secret_string: {secret_string}")
+        # Step 2: Add secret_string if provided
+        if self.secret_string is not None:
+            secret_dict.update(json.loads(self.secret_string))
+
+        # Step 3: Build secret_string
+        secret_string: Optional[str] = (
+            json.dumps(secret_dict) if len(secret_dict) > 0 else None
+        )
+        # logger.debug(f"secret_string: {secret_string}")
 
-        # Step 2: Build SecretsManager configuration
+        # Step 4: Build SecretsManager configuration
         # create a dict of args which are not null, otherwise aws type validation fails
         not_null_args: Dict[str, Any] = {}
         if self.client_request_token:
             not_null_args["ClientRequestToken"] = self.client_request_token
         if self.description:
             not_null_args["Description"] = self.description
         if self.kms_key_id:
@@ -111,21 +119,21 @@
                 Name=self.name,
                 **not_null_args,
             )
             logger.debug(f"SecretsManager: {created_resource}")
 
             # Validate SecretsManager creation
             self.secret_arn = created_resource.get("ARN", None)
-            self.secret_resource_name = created_resource.get("Name", None)
+            self.secret_name = created_resource.get("Name", None)
             logger.debug(f"secret_arn: {self.secret_arn}")
-            logger.debug(f"secret_resource_name: {self.secret_resource_name}")
+            logger.debug(f"secret_name: {self.secret_name}")
             if self.secret_arn is not None:
                 print_info(f"SecretsManager created: {self.name}")
+                self.cached_secret = secret_dict
                 self.active_resource = created_resource
-                self.save_resource_file()
                 return True
         except Exception as e:
             print_error(f"{self.get_resource_type()} could not be created.")
             print_error(e)
         return False
 
     def _read(self, aws_client: AwsApiClient) -> Optional[Any]:
@@ -140,23 +148,22 @@
 
         service_client = self.get_service_client(aws_client)
         try:
             describe_response = service_client.describe_secret(SecretId=self.name)
             logger.debug(f"SecretsManager: {describe_response}")
 
             self.secret_arn = describe_response.get("ARN", None)
-            self.secret_resource_name = describe_response.get("Name", None)
+            self.secret_name = describe_response.get("Name", None)
             secret_deleted_date = describe_response.get("DeletedDate", None)
             logger.debug(f"secret_arn: {self.secret_arn}")
-            logger.debug(f"secret_resource_name: {self.secret_resource_name}")
-            logger.debug(f"secret_deleted_date: {secret_deleted_date}")
+            logger.debug(f"secret_name: {self.secret_name}")
+            # logger.debug(f"secret_deleted_date: {secret_deleted_date}")
             if self.secret_arn is not None:
-                print_info(f"SecretsManager available: {self.name}")
+                # print_info(f"SecretsManager available: {self.name}")
                 self.active_resource = describe_response
-                self.save_resource_file()
         except ClientError as ce:
             logger.debug(f"ClientError: {ce}")
         except Exception as e:
             print_error(f"Error reading {self.get_resource_type()}.")
             print_error(e)
         return self.active_resource
 
@@ -175,55 +182,99 @@
             delete_response = service_client.delete_secret(
                 SecretId=self.name, ForceDeleteWithoutRecovery=self.force_delete
             )
             logger.debug(f"SecretsManager: {delete_response}")
             print_info(
                 f"{self.get_resource_type()}: {self.get_resource_name()} deleted"
             )
-            self.save_resource_file()
             return True
         except Exception as e:
             print_error(f"{self.get_resource_type()} could not be deleted.")
             print_error("Please try again or delete resources manually.")
             print_error(e)
         return False
 
-    def get_secret_dict(self, aws_client: Optional[AwsApiClient] = None) -> Any:
+    def _update(self, aws_client: AwsApiClient) -> bool:
+        """Update SecretsManager"""
+        print_info(f"Updating {self.get_resource_type()}: {self.get_resource_name()}")
+
+        # Step 1: Read secrets from files
+        secret_dict: Dict[str, Any] = self.read_secrets_from_files()
+
+        # Step 2: Add secret_string is provided
+        if self.secret_string is not None:
+            secret_dict.update(json.loads(self.secret_string))
+
+        # Step 3: Read secrets from AWS SecretsManager
+        aws_secrets = self.get_secrets_as_dict()
+        logger.debug(f"aws_secrets: {aws_secrets}")
+        if aws_secrets is not None:
+            secret_dict.update(aws_secrets)
+
+        # Step 3: Update AWS SecretsManager
+        service_client = self.get_service_client(aws_client)
+        self.active_resource = None
+        self.secret_value = None
+        try:
+            create_response = service_client.update_secret(
+                SecretId=self.name,
+                SecretString=json.dumps(secret_dict),
+            )
+            logger.debug(f"SecretsManager: {create_response}")
+            print_info(
+                f"{self.get_resource_type()}: {self.get_resource_name()} Updated"
+            )
+            return True
+        except Exception as e:
+            print_error(f"{self.get_resource_type()} could not be Updated.")
+            print_error(e)
+        return False
+
+    def get_secrets_as_dict(
+        self, aws_client: Optional[AwsApiClient] = None
+    ) -> Optional[Dict[str, Any]]:
         """Get secret value
 
         Args:
             aws_client: The AwsApiClient for the current secret
         """
-        logger.debug(f"Getting {self.get_resource_type()}: {self.get_resource_name()}")
-
         from botocore.exceptions import ClientError
 
+        if self.cached_secret is not None:
+            return self.cached_secret
+
+        logger.debug(f"Getting {self.get_resource_type()}: {self.get_resource_name()}")
         client: AwsApiClient = aws_client or self.get_aws_client()
         service_client = self.get_service_client(client)
         try:
             secret_value = service_client.get_secret_value(SecretId=self.name)
-            logger.debug(f"SecretsManager: {secret_value}")
+            # logger.debug(f"SecretsManager: {secret_value}")
 
             if secret_value is None:
-                logger.warning(f"SecretsManager is None: {self.name}")
+                logger.warning(f"Secret Empty: {self.name}")
                 return None
 
             self.secret_value = secret_value
             self.secret_arn = secret_value.get("ARN", None)
-            self.secret_resource_name = secret_value.get("Name", None)
-            self.save_resource_file()
+            self.secret_name = secret_value.get("Name", None)
 
             secret_string = secret_value.get("SecretString", None)
             if secret_string is not None:
-                import json
-
-                return json.loads(secret_string)
+                self.cached_secret = json.loads(secret_string)
+                return self.cached_secret
 
             secret_binary = secret_value.get("SecretBinary", None)
             if secret_binary is not None:
-                return secret_binary
+                self.cached_secret = json.loads(secret_binary.decode("utf-8"))
+                return self.cached_secret
         except ClientError as ce:
             logger.debug(f"ClientError: {ce}")
         except Exception as e:
             print_error(f"Error reading {self.get_resource_type()}.")
             print_error(e)
         return None
+
+    def get_secret_value(self, secret_name: str) -> Optional[Any]:
+        secret_dict = self.get_secrets_as_dict()
+        if secret_dict is not None:
+            return secret_dict.get(secret_name, None)
+        return None
```

### Comparing `phidata-1.6.9/phidata/aws/resource/types.py` & `phidata-1.7.0/phidata/aws/resource/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 from typing import Dict, List, Type, Union
 
 from phidata.aws.resource.base import AwsResource
 from phidata.aws.resource.acm.certificate import AcmCertificate
 from phidata.aws.resource.cloudformation.stack import CloudFormationStack
 from phidata.aws.resource.ec2.volume import EbsVolume
 from phidata.aws.resource.ec2.subnet import Subnet
+from phidata.aws.resource.ec2.security_group import SecurityGroup
 from phidata.aws.resource.ecs.cluster import EcsCluster
 from phidata.aws.resource.ecs.task_definition import EcsTaskDefinition
 from phidata.aws.resource.eks.cluster import EksCluster
 from phidata.aws.resource.ecs.service import EcsService
 from phidata.aws.resource.eks.fargate_profile import EksFargateProfile
 from phidata.aws.resource.eks.node_group import EksNodeGroup
 from phidata.aws.resource.eks.kubeconfig import EksKubeconfig
 from phidata.aws.resource.elb.load_balancer import LoadBalancer
 from phidata.aws.resource.elb.target_group import TargetGroup
 from phidata.aws.resource.elb.listener import Listener
 from phidata.aws.resource.iam.role import IamRole
 from phidata.aws.resource.iam.policy import IamPolicy
 from phidata.aws.resource.glue.crawler import GlueCrawler
 from phidata.aws.resource.s3.bucket import S3Bucket
+from phidata.aws.resource.secret.manager import SecretsManager
 from phidata.aws.resource.emr.cluster import EmrCluster
 from phidata.aws.resource.rds.db_cluster import DbCluster
 from phidata.aws.resource.rds.db_instance import DbInstance
 from phidata.aws.resource.rds.db_subnet_group import DbSubnetGroup
 from phidata.aws.resource.elasticache.cluster import CacheCluster
 from phidata.aws.resource.elasticache.subnet_group import CacheSubnetGroup
 
@@ -36,15 +38,17 @@
     EksFargateProfile,
     EksNodeGroup,
     EksKubeconfig,
     IamRole,
     IamPolicy,
     GlueCrawler,
     S3Bucket,
+    SecretsManager,
     Subnet,
+    SecurityGroup,
     DbSubnetGroup,
     DbCluster,
     DbInstance,
     CacheSubnetGroup,
     CacheCluster,
     EmrCluster,
     EcsCluster,
@@ -55,17 +59,19 @@
     Listener,
 ]
 
 # Use this as an ordered list to iterate over all Aws Resource Classes
 # This list is the order in which resources should be installed as well.
 AwsResourceTypeList: List[Type[AwsResource]] = [
     Subnet,
+    SecurityGroup,
     IamRole,
     IamPolicy,
     S3Bucket,
+    SecretsManager,
     EbsVolume,
     AcmCertificate,
     CloudFormationStack,
     GlueCrawler,
     DbSubnetGroup,
     DbCluster,
     DbInstance,
```

### Comparing `phidata-1.6.9/phidata/aws/resource/utils.py` & `phidata-1.7.0/phidata/aws/resource/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,20 @@
                         # logger.debug(f"type_filter: {type_filter.lower()}")
                         # logger.debug(f"class: {rt.lower()}")
                         if type_filter.lower() != rt.lower():
                             logger.debug(f"  -*- skipping {rt}:{rn}")
                             continue
                     aws_resources.append(_r)  # type: ignore
 
+                    # Add the resource dependencies to the aws_resources list
+                    if _r.depends_on is not None:
+                        for dep in _r.depends_on:
+                            if isinstance(dep, AwsResource):
+                                aws_resources.append(dep)
+
         # If its a single resource, verify that the resource is a subclass of
         # AwsResource and add it to the aws_resources list
         elif isinstance(resource_data, AwsResource):
             rn = resource_data.get_resource_name()
             rt = resource_data.get_resource_type()
             # skip disabled resources
             if not resource_data.enabled:
```

### Comparing `phidata-1.6.9/phidata/aws/s3/csv_dataset.py` & `phidata-1.7.0/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/s3/dataset.py` & `phidata-1.7.0/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/s3/dataset_base.py` & `phidata-1.7.0/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/s3/object.py` & `phidata-1.7.0/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/aws/worker.py` & `phidata-1.7.0/phidata/aws/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import OrderedDict
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
 from phidata.aws.args import AwsArgs
+from phidata.app.base_app import BaseApp
 from phidata.app.phidata_app import PhidataApp
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
 from phidata.aws.resource.group import AwsResourceGroup
 from phidata.aws.resource.utils import (
     filter_and_flatten_aws_resource_groups,
 )
@@ -46,15 +47,15 @@
         """
         Build the AwsResourceGroups for the requested apps
         """
         logger.debug("-*- Initializing AwsResourceGroups")
 
         aws_resource_groups: Optional[Dict[str, AwsResourceGroup]] = None
 
-        aws_apps: Optional[List[PhidataApp]] = self.aws_args.apps
+        aws_apps: Optional[List[Union[BaseApp, PhidataApp]]] = self.aws_args.apps
         aws_rgs: Optional[List[AwsResourceGroup]] = self.aws_args.resources
 
         num_apps = len(aws_apps) if aws_apps is not None else 0
         num_rgs = len(aws_rgs) if aws_rgs is not None else 0
         num_rgs_to_build = num_apps + num_rgs
         num_rgs_built = 0
```

### Comparing `phidata-1.6.9/phidata/base.py` & `phidata-1.7.0/phidata/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-from typing import Optional
+from typing import Optional, Dict, Any
 
 from pydantic import BaseModel
 
 
 class PhidataBaseArgs(BaseModel):
     name: Optional[str] = None
     version: Optional[str] = None
     enabled: bool = True
 
+    #  -*- Resource Control
     skip_create: bool = False
     skip_read: bool = False
     skip_update: bool = False
     recreate_on_update: bool = False
     skip_delete: bool = False
-
     wait_for_creation: bool = True
     wait_for_update: bool = True
     wait_for_deletion: bool = True
     waiter_delay: int = 30
     waiter_max_attempts: int = 50
 
+    #  -*- Save Resources to output directory
+    # If True, save the resources to files
+    save_output: bool = False
+    # The resource directory for the output files
+    resource_dir: Optional[str] = None
+
+    # Skip creation if resource with the same name is active
+    use_cache: bool = True
+
     class Config:
         arbitrary_types_allowed = True
 
 
 class PhidataBase:
     """Phidata Base Class"""
 
     def __init__(self) -> None:
-        self.args: Optional[PhidataBaseArgs] = None
+        self.args: PhidataBaseArgs = PhidataBaseArgs()
 
     @property
     def name(self) -> str:
-        return (
-            self.args.name
-            if (self.args and self.args.name)
-            else self.__class__.__name__
-        )
+        return self.args.name or self.__class__.__name__
 
     @property
     def version(self) -> Optional[str]:
-        return self.args.version if self.args else None
+        return self.args.version
 
     @property
     def enabled(self) -> bool:
-        return self.args.enabled if self.args else False
+        return self.args.enabled
```

### Comparing `phidata-1.6.9/phidata/checks/check.py` & `phidata-1.7.0/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/checks/not_empty.py` & `phidata-1.7.0/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/constants.py` & `phidata-1.7.0/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/decorators/timer.py` & `phidata-1.7.0/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/decorators/validate_env.py` & `phidata-1.7.0/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/api_client.py` & `phidata-1.7.0/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/args.py` & `phidata-1.7.0/phidata/k8s/args.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,53 @@
-from typing import List, Optional
+from pathlib import Path
+from typing import List, Optional, Dict, Any, Union
 
 from pydantic import validator
 
+from phidata.app.base_app import BaseApp
 from phidata.app.phidata_app import PhidataApp
 from phidata.app.databox import default_databox_name
 from phidata.infra.args import InfraArgs
-from phidata.docker.resource.image import DockerImage
-from phidata.docker.resource.container import DockerContainer
-from phidata.docker.resource.volume import DockerVolume
-from phidata.docker.resource.group import DockerResourceGroup
-
-
-class DockerArgs(InfraArgs):
-    network: str = "bridge"
-    # configure the DockerClient
-    # URL to the Docker server. For example, unix:///var/run/docker.sock or tcp://127.0.0.1:1234.
-    # when None, phidata use DockerClient.from_env()
-    base_url: Optional[str] = None
-    apps: Optional[List[PhidataApp]] = None
-    # default resources
-    images: Optional[List[DockerImage]] = None
-    containers: Optional[List[DockerContainer]] = None
-    volumes: Optional[List[DockerVolume]] = None
-    # additional resource groups
-    resources: Optional[List[DockerResourceGroup]] = None
+from phidata.k8s.resource.group import K8sResourceGroup
+from phidata.k8s.create.group import CreateK8sResourceGroup
+
+
+class K8sArgs(InfraArgs):
+    # K8s namespace to use
+    namespace: str = "default"
+    # K8s context to use
+    context: Optional[str] = None
+    # K8s service account to use
+    service_account_name: Optional[str] = None
+    # Common K8s labels to add to all resources
+    common_labels: Optional[Dict[str, str]] = None
+    # PhidataApp to deploy
+    apps: Optional[List[Union[BaseApp, PhidataApp]]] = None
+    # K8sResourceGroup to deploy
+    resources: Optional[List[K8sResourceGroup]] = None
+    # CreateK8sResourceGroup to deploy
+    create_resources: Optional[List[CreateK8sResourceGroup]] = None
+    # Resources dir where k8s manifests are stored
+    resources_dir: str = "k8s"
+    # databox name for `phi dx ...` commands
     databox_name: str = default_databox_name
+    kubeconfig_path: Optional[Path] = None
+
+    # Get K8s context and kubeconfig from an EksCluster resource
+    eks_cluster: Optional[Any] = None
 
     @validator("apps")
     def apps_are_valid(cls, apps):
         if apps is not None:
             for _app in apps:
-                if not isinstance(_app, PhidataApp):
-                    raise TypeError("App not of type PhidataApp: {}".format(_app))
-        return apps
-
-    def default_resources_available(self) -> bool:
-        return (
-            self.images is not None
-            or self.containers is not None
-            or self.volumes is not None
-        )
+                if not (isinstance(_app, PhidataApp) or isinstance(_app, BaseApp)):
+                    raise TypeError(f"App not of type PhidataApp or BaseApp: {_app}")
+            return apps
+
+    @validator("eks_cluster")
+    def eks_cluster_is_valid(cls, eks_cluster):
+        if eks_cluster is not None:
+            from phidata.aws.resource.eks.cluster import EksCluster
+
+            if not isinstance(eks_cluster, EksCluster):
+                raise TypeError("eks_cluster not of type EksCluster")
+            return eks_cluster
```

### Comparing `phidata-1.6.9/phidata/docker/config.py` & `phidata-1.7.0/phidata/docker/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import List, Optional
+from typing import List, Optional, Union
 
+from phidata.app.base_app import BaseApp
 from phidata.app.phidata_app import PhidataApp
 from phidata.app.group import AppGroup, get_apps_from_app_groups
 from phidata.app.databox import default_databox_name
 from phidata.infra.config import InfraConfig
 from phidata.docker.args import DockerArgs
 from phidata.docker.manager import DockerManager
 from phidata.docker.resource.image import DockerImage
@@ -18,15 +19,15 @@
         self,
         name: Optional[str] = None,
         env: Optional[str] = "dev",
         version: Optional[str] = None,
         enabled: bool = True,
         network: str = "bridge",
         base_url: Optional[str] = None,
-        apps: Optional[List[PhidataApp]] = None,
+        apps: Optional[List[Union[BaseApp, PhidataApp]]] = None,
         app_groups: Optional[List[AppGroup]] = None,
         images: Optional[List[DockerImage]] = None,
         containers: Optional[List[DockerContainer]] = None,
         volumes: Optional[List[DockerVolume]] = None,
         resources: Optional[List[DockerResourceGroup]] = None,
         databox: str = default_databox_name,
     ):
@@ -58,15 +59,15 @@
         return self.args.network if self.args else None
 
     @property
     def base_url(self) -> Optional[str]:
         return self.args.base_url if self.args else None
 
     @property
-    def apps(self) -> Optional[List[PhidataApp]]:
+    def apps(self) -> Optional[List[Union[BaseApp, PhidataApp]]]:
         return self.args.apps if self.args else None
 
     @property
     def images(self) -> Optional[List[DockerImage]]:
         return self.args.images if self.args else None
 
     @property
@@ -85,15 +86,15 @@
     def databox_name(self) -> Optional[str]:
         return self.args.databox_name if self.args else None
 
     def apps_are_valid(self) -> bool:
         if self.apps is None:
             return False
         for _app in self.apps:
-            if not isinstance(_app, PhidataApp):
+            if not (isinstance(_app, PhidataApp) or isinstance(_app, BaseApp)):
                 raise TypeError("Invalid App: {}".format(_app))
         return True
 
     def resources_are_valid(self) -> bool:
         if self.resources is None:
             return False
         for _resource in self.resources:
@@ -112,15 +113,15 @@
             or self.resources_are_valid()
             or self.default_resources_are_valid()
         )
 
     def get_docker_manager(self) -> DockerManager:
         return DockerManager(docker_args=self.args)
 
-    def get_app_by_name(self, app_name: str) -> Optional[PhidataApp]:
+    def get_app_by_name(self, app_name: str) -> Optional[Union[BaseApp, PhidataApp]]:
         if self.apps is None:
             return None
 
         for _app in self.apps:
             try:
                 if app_name == _app.name:
                     return _app
```

### Comparing `phidata-1.6.9/phidata/docker/enums.py` & `phidata-1.7.0/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/manager.py` & `phidata-1.7.0/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/resource/base.py` & `phidata-1.7.0/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/resource/container.py` & `phidata-1.7.0/phidata/docker/resource/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,53 +107,58 @@
 
     # Data provided by the resource running on the docker client
     status: Optional[str] = None
 
     def run_container(self, docker_client: DockerApiClient) -> Optional[Any]:
         from docker import DockerClient
         from docker.errors import NotFound, ImageNotFound, APIError
+        from rich.progress import Progress
 
-        print_info("Running container: {}".format(self.name))
+        print_info("Starting container: {}".format(self.name))
         # logger.debug()(
         #     "Args: {}".format(
         #         self.json(indent=2, exclude_unset=True, exclude_none=True)
         #     )
         # )
         try:
+            # Delete container if exists
+            delete_success = self._delete(docker_client)
             _api_client: DockerClient = docker_client.api_client
-            container = _api_client.containers.run(
-                name=self.name,
-                image=self.image,
-                command=self.command,
-                auto_remove=self.auto_remove,
-                detach=self.detach,
-                entrypoint=self.entrypoint,
-                environment=self.environment,
-                group_add=self.group_add,
-                healthcheck=self.healthcheck,
-                hostname=self.hostname,
-                labels=self.labels,
-                mounts=self.mounts,
-                network=self.network,
-                network_disabled=self.network_disabled,
-                network_mode=self.network_mode,
-                platform=self.platform,
-                ports=self.ports,
-                remove=self.remove,
-                restart_policy=self.restart_policy,
-                stdin_open=self.stdin_open,
-                stdout=self.stdout,
-                stderr=self.stderr,
-                tty=self.tty,
-                user=self.user,
-                volumes=self.volumes,
-                working_dir=self.working_dir,
-                devices=self.devices,
-            )
-            return container
+            with Progress(transient=True) as progress:
+                task = progress.add_task("Downloading Image", total=None)
+                container_object = _api_client.containers.run(
+                    name=self.name,
+                    image=self.image,
+                    command=self.command,
+                    auto_remove=self.auto_remove,
+                    detach=self.detach,
+                    entrypoint=self.entrypoint,
+                    environment=self.environment,
+                    group_add=self.group_add,
+                    healthcheck=self.healthcheck,
+                    hostname=self.hostname,
+                    labels=self.labels,
+                    mounts=self.mounts,
+                    network=self.network,
+                    network_disabled=self.network_disabled,
+                    network_mode=self.network_mode,
+                    platform=self.platform,
+                    ports=self.ports,
+                    remove=self.remove,
+                    restart_policy=self.restart_policy,
+                    stdin_open=self.stdin_open,
+                    stdout=self.stdout,
+                    stderr=self.stderr,
+                    tty=self.tty,
+                    user=self.user,
+                    volumes=self.volumes,
+                    working_dir=self.working_dir,
+                    devices=self.devices,
+                )
+                return container_object
         except AttributeError as attr_error:
             logger.error("AttributeError")
             raise DockerResourceCreationFailedException(attr_error)
         except ImageNotFound as img_error:
             logger.error("ImageNotFound")
             raise DockerResourceCreationFailedException(
                 f"Image {self.image} not found. Explanation: {img_error.explanation}"
@@ -229,29 +234,28 @@
             if _status == "exited":
                 logger.debug(f"Starting container {container_name}")
                 container_object.remove()
                 container_object = self.run_container(docker_client)
                 wait_for_container_to_start = True
 
             if wait_for_container_to_start:
-                logger.debug("Waiting for 30 seconds for the container to start")
-                sleep(30)
+                logger.debug("Waiting 5 seconds for the container to start")
+                sleep(5)
                 _status = container_object.status
                 while _status != "created":
                     logger.debug(
                         "--> status: {}, trying again in 5 seconds".format(_status)
                     )
                     sleep(5)
                     _status = container_object.status
                 logger.debug("--> status: {}".format(_status))
 
             if _status == "running" or "created":
                 logger.debug("Container Created")
                 self.active_resource = container_object
-                self.active_resource_class = Container
                 return True
 
         logger.debug("Container not found :(")
         return False
 
     def _read(self, docker_client: DockerApiClient) -> Optional[Any]:
         """Returns a Container object if the container is active on the docker_client"""
@@ -266,15 +270,14 @@
                 all=True, filters={"name": container_name}
             )
             if container_list is not None:
                 for container in container_list:
                     if container.name == container_name:
                         logger.debug(f"Container {container_name} exists")
                         self.active_resource = container
-                        self.active_resource_class = Container
                         return container
         except Exception:
             logger.debug(f"Container {container_name} not found")
 
         return None
 
     def _delete(self, docker_client: DockerApiClient) -> bool:
@@ -321,14 +324,28 @@
                 logger.debug("Waiting for NotFound Exception...")
                 sleep(1)
         except NotFound as e:
             logger.debug("Got NotFound Exception, container is deleted")
 
         return True
 
+    def is_active_on_cluster(self, docker_client: DockerApiClient) -> bool:
+        """Returns True if the container is running on the docker cluster"""
+        from docker.models.containers import Container
+
+        container_object: Optional[Container] = self.read(docker_client=docker_client)
+        if container_object is not None:
+            # Check if container is stopped/paused
+            status: str = container_object.status
+            if status in ["exited", "paused"]:
+                logger.debug(f"Container status: {status}")
+                return False
+            return True
+        return False
+
     def create(self, docker_client: DockerApiClient) -> bool:
         # if self.force then always create container
         if not self.force:
             if self.use_cache and self.is_active_on_cluster(docker_client):
                 print_info(
                     f"{self.get_resource_type()} {self.get_resource_name()} already active."
                 )
```

### Comparing `phidata-1.6.9/phidata/docker/resource/group.py` & `phidata-1.7.0/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/resource/image.py` & `phidata-1.7.0/phidata/docker/resource/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Any, Dict, List
 
 from phidata.docker.api_client import DockerApiClient
 from phidata.docker.resource.base import DockerResource
-from phidata.utils.cli_console import print_info, print_error
+from phidata.utils.cli_console import print_info, print_error, console
 from phidata.utils.log import logger
 
 
 class DockerImage(DockerResource):
     resource_type: str = "Image"
 
     # Docker image name, usually as repo/image
@@ -69,14 +69,17 @@
     # will be set in the container being built.
     use_config_proxy: Optional[bool] = None
 
     # so that images arent deleted when phi ws down is run
     skip_delete: bool = True
     image_build_id: Optional[str] = None
 
+    # Set use_cache to False so image is always built
+    use_cache: bool = False
+
     def get_resource_name(self) -> Optional[str]:
         return self.get_name_tag()
 
     def get_name_tag(self) -> str:
         # Deprecated
         image_name_tag = self.name
         if self.tag:
@@ -87,14 +90,17 @@
         if self.tag:
             return f"{self.name}:{self.tag}"
         return f"{self.name}:latest"
 
     def build_image(self, docker_client: DockerApiClient) -> Optional[Any]:
         from docker import DockerClient
         from docker.errors import BuildError, APIError
+        from rich import box
+        from rich.live import Live
+        from rich.table import Table
 
         print_info(f"Building image: {self.get_name_tag()}")
         nocache = self.skip_docker_cache or self.force
         pull = self.pull or self.force
         if self.path is not None:
             print_info(f"\t  path: {self.path}")
         if self.dockerfile is not None:
@@ -127,75 +133,117 @@
                 extra_hosts=self.extra_hosts,
                 platform=self.platform,
                 isolation=self.isolation,
                 use_config_proxy=self.use_config_proxy,
                 decode=True,
             )
 
-            for build_log in build_stream:
-                if build_log != last_build_log:
-                    last_build_log = build_log
-
-                build_status: str = build_log.get("status")
-                if build_status is not None:
-                    _status = build_status.lower()
-                    if _status in (
-                        "waiting",
-                        "downloading",
-                        "extracting",
-                        "verifying checksum",
-                        "pulling fs layer",
-                    ):
+            with Live(transient=True, console=console) as live_log:
+                progress: List[str] = []
+                for build_log in build_stream:
+                    if build_log != last_build_log:
+                        last_build_log = build_log
+
+                    build_status: str = build_log.get("status")
+                    if build_status is not None:
+                        _status = build_status.lower()
+                        if _status in (
+                            "waiting",
+                            "downloading",
+                            "extracting",
+                            "verifying checksum",
+                            "pulling fs layer",
+                        ):
+                            continue
+                        if build_status != last_status:
+                            logger.debug(build_status)
+                            last_status = build_status
+                    stream = build_log.get("stream", None)
+                    if stream is None or stream == "\n":
                         continue
-                    if build_status != last_status:
-                        logger.debug(build_status)
-                        last_status = build_status
-
-                stream = build_log.get("stream", None)
-                if stream is None or stream == "\n":
-                    continue
-                stream = stream.strip()
-                if "Step" in stream and self.print_build_log:
-                    print_info(stream)
-                else:
-                    logger.debug(stream)
-                if "ERROR" in stream or "error" in stream:
-                    logger.debug(build_log)
-                    print_error(f"Image build failed: {self.get_name_tag()}")
-                    print_error(stream)
-                    return None
-                if build_log.get("aux", None) is not None:
-                    logger.debug("build_log['aux'] :{}".format(build_log["aux"]))
-                    self.image_build_id = build_log.get("aux", {}).get("ID")
+                    stream = stream.strip()
+
+                    if "Step" in stream and self.print_build_log:
+                        progress = []
+                        print_info(stream)
+                    else:
+                        progress.append(stream)
+                        if len(progress) > 10:
+                            progress.pop(0)
+
+                    if "ERROR" in stream or "error" in stream:
+                        print(stream)
+                        live_log.stop()
+                        print_error(f"Image build failed: {self.get_name_tag()}")
+                        return None
+                    if build_log.get("aux", None) is not None:
+                        logger.debug("build_log['aux'] :{}".format(build_log["aux"]))
+                        self.image_build_id = build_log.get("aux", {}).get("ID")
+
+                    # Render table
+                    table = Table(show_edge=False, show_header=False, show_lines=False)
+                    for line in progress:
+                        table.add_row(line, style="dim")
+                    live_log.update(table)
+
             if self.push_image:
                 print_info(f"Pushing {self.get_name_tag()}")
-                push_progress = None
-                prev_push_progress = None
-                for push_output in _api_client.images.push(
-                    repository=self.name,
-                    tag=self.tag,
-                    stream=True,
-                    decode=True,
-                ):
-                    if push_output.get("error", None) is not None:
-                        print_error(push_output["error"])
-                        print_error(f"Push failed for {self.get_name_tag()}")
-                        print_error(
-                            "If you are using a private registry, make sure you are logged in"
-                        )
-                    if self.print_push_output and push_output.get("status", None) in (
-                        "Pushing",
-                        "Pushed",
+                with Live(transient=True, console=console) as live_log:
+                    push_status = {}
+                    last_push_progress = None
+                    for push_output in _api_client.images.push(
+                        repository=self.name,
+                        tag=self.tag,
+                        stream=True,
+                        decode=True,
                     ):
-                        push_progress = push_output.get("progress", None)
-                        if push_progress != prev_push_progress:
-                            print_info(push_progress)
-                            prev_push_progress = push_progress
-                    if push_output.get("aux", {}).get("Size", 0) > 0:
-                        print_info(f"Push complete: {push_output.get('aux', {})}")
+                        # logger.info(push_output)
+                        _id = push_output.get("id", None)
+                        _status = push_output.get("status", None)
+                        _progress = push_output.get("progress", None)
+                        if _id is not None and _status is not None:
+                            push_status[_id] = {
+                                "status": _status,
+                                "progress": _progress,
+                            }
+
+                        if push_output.get("error", None) is not None:
+                            print_error(push_output["error"])
+                            print_error(f"Push failed for {self.get_name_tag()}")
+                            print_error(
+                                "If you are using a private registry, make sure you are logged in"
+                            )
+
+                        if self.print_push_output and push_output.get(
+                            "status", None
+                        ) in (
+                            "Pushing",
+                            "Pushed",
+                        ):
+                            current_progress = push_output.get("progress", None)
+                            if current_progress != last_push_progress:
+                                print_info(current_progress)
+                                last_push_progress = current_progress
+                        if push_output.get("aux", {}).get("Size", 0) > 0:
+                            print_info(f"Push complete: {push_output.get('aux', {})}")
+
+                        # Render table
+                        table = Table(box=box.ASCII2)
+                        table.add_column("Layer", justify="center")
+                        table.add_column("Status", justify="center")
+                        table.add_column("Progress", justify="center")
+                        for layer, layer_status in push_status.items():
+                            table.add_row(
+                                layer,
+                                layer_status["status"],
+                                layer_status["progress"],
+                                style="dim",
+                            )
+                        live_log.update(table)
+
             return self._read(docker_client)
         except TypeError as type_error:
             print_error(type_error)
         except BuildError as build_error:
             print_error(build_error)
         except APIError as api_err:
             print_error(api_err)
@@ -215,16 +263,14 @@
         try:
             image_object = self.build_image(docker_client)
             if image_object is not None and isinstance(image_object, Image):
                 logger.debug("Image built: {}".format(image_object))
                 self.active_resource = image_object
                 self.active_resource_class = Image
                 return True
-            else:
-                logger.error("Image {} could not be built".format(self.tag))
         except Exception as e:
             logger.exception(e)
             logger.error("Error while creating image: {}".format(e))
             raise
 
         return False
```

### Comparing `phidata-1.6.9/phidata/docker/resource/network.py` & `phidata-1.7.0/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/resource/types.py` & `phidata-1.7.0/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/resource/utils.py` & `phidata-1.7.0/phidata/docker/resource/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,20 @@
                         # logger.debug(f"type_filter: {type_filter.lower()}")
                         # logger.debug(f"class: {rt.lower()}")
                         if type_filter.lower() not in rt.lower():
                             logger.debug(f"  -*- skipping {rt}:{rn}")
                             continue
                     docker_resources.append(_r)  # type: ignore
 
+                    # Add the resource dependencies to the aws_resources list
+                    if _r.depends_on is not None:
+                        for dep in _r.depends_on:
+                            if isinstance(dep, DockerResource):
+                                docker_resources.append(dep)
+
         # If its a single resource, verify that the resource is a subclass of
         # DockerResource and add it to the docker_resources list
         elif isinstance(resource_data, DockerResource):
             rn = resource_data.get_resource_name()
             rt = resource_data.get_resource_type()
             # skip disabled resources
             if not resource_data.enabled:
```

### Comparing `phidata-1.6.9/phidata/docker/resource/volume.py` & `phidata-1.7.0/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/utils/container.py` & `phidata-1.7.0/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/docker/worker.py` & `phidata-1.7.0/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/infra/args.py` & `phidata-1.7.0/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/infra/config.py` & `phidata-1.7.0/phidata/infra/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class InfraConfig(PhidataBase):
     """Base Class for all phidata infra configs"""
 
     def __init__(self) -> None:
         super().__init__()
-        self.args: Optional[InfraArgs] = None
+        self.args: InfraArgs = InfraArgs()
 
     @property
     def env(self) -> Optional[str]:
         return self.args.env if self.args else None
 
     @env.setter
     def env(self, env: str) -> None:
```

### Comparing `phidata-1.6.9/phidata/infra/resource.py` & `phidata-1.7.0/phidata/infra/resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, Optional, Type, Union, Dict
+from typing import Any, Optional, Type, Union, Dict, List
 
 from pydantic import BaseModel, validator
 
 from phidata.utils.log import logger
 
 
 class InfraResource(BaseModel):
@@ -48,18 +48,37 @@
     # If True, waits for the resource to be deleted
     wait_for_deletion: bool = True
     # The amount of time in seconds to wait between attempts.
     waiter_delay: int = 30
     # The maximum number of attempts to be made.
     waiter_max_attempts: int = 50
 
+    # Active resource object
     active_resource: Optional[Any] = None
+    # Deprecated: the class of the active resource
     active_resource_class: Optional[Type] = None
 
+    # If True, save the resource to a file
+    save_output: bool = False
     resource_file: Optional[Union[str, Path]] = None
+    # Add a resource directory to the resource file path
+    resource_dir: Optional[str] = None
+
+    # Other resources this resource depends on
+    # Dependencies are always created if this resource is created
+    depends_on: Optional[List[Any]] = None
+
+    # Add secret variables to resource where applicable
+    secret_data: Optional[Dict[str, Any]] = None
+    # Read secrets from a file in yaml format
+    secrets_file: Optional[Path] = None
+    # Add env variables to resource where applicable
+    env_data: Optional[Dict[str, Any]] = None
+    # Read env from a file in yaml format
+    env_file: Optional[Path] = None
 
     def get_resource_name(self) -> Optional[str]:
         return self.name
 
     def get_resource_type(self) -> Optional[str]:
         return self.resource_type
 
@@ -199,29 +218,93 @@
             data_from_file = yaml.safe_load(file_path.read_text())
             if data_from_file is not None and isinstance(data_from_file, dict):
                 return data_from_file
             else:
                 logger.error(f"Invalid file: {file_path}")
         return None
 
-    def save_resource_file(self) -> bool:
-        if self.resource_file is not None:
-            resource_file_path: Optional[Path] = None
-            if isinstance(self.resource_file, str):
-                resource_file_path = Path(self.resource_file)
-            elif isinstance(self.resource_file, Path):
-                resource_file_path = self.resource_file
-
-            if resource_file_path is None or not isinstance(resource_file_path, Path):
-                logger.error(f"Invalid resource_file: {resource_file_path}")
+    def get_resource_file_path(self) -> Optional[Path]:
+        if self.resource_file is None:
+            workspace_config_dir = self.get_workspace_config_dir()
+            if workspace_config_dir is not None:
+                if self.name is not None and self.resource_type is not None:
+                    file_name = f"{self.name}.json"
+                    resource_dir = self.resource_dir or self.resource_type
+                    return workspace_config_dir.joinpath(
+                        "output", resource_dir, file_name
+                    )
+        if isinstance(self.resource_file, str):
+            return Path(self.resource_file)
+        elif isinstance(self.resource_file, Path):
+            return self.resource_file
+        return None
 
+    def save_resource_file(self) -> bool:
+        resource_file_path: Optional[Path] = self.get_resource_file_path()
+        if resource_file_path is not None:
             try:
+                from phidata.utils.json_io import write_json_file
+
                 if not resource_file_path.exists():
                     resource_file_path.parent.mkdir(parents=True, exist_ok=True)
                     resource_file_path.touch(exist_ok=True)
-                resource_file_path.write_text(self.json(indent=2))
-                logger.debug(f"Resource stored at: {str(resource_file_path)}")
+                write_json_file(resource_file_path, self.active_resource)
+                logger.info(f"Resource saved to: {str(resource_file_path)}")
                 return True
             except Exception as e:
-                logger.error("Could not write resource to file")
-                logger.error(e)
+                logger.error(f"Could not write resource to file {e}")
         return False
+
+    def read_resource_from_file(self) -> Optional[Dict[str, Any]]:
+        resource_file_path: Optional[Path] = self.get_resource_file_path()
+        if resource_file_path is not None:
+            try:
+                from phidata.utils.json_io import read_json_file
+
+                if resource_file_path.exists() and resource_file_path.is_file():
+                    data_from_file = read_json_file(resource_file_path)
+                    if data_from_file is not None and isinstance(data_from_file, dict):
+                        return data_from_file
+                    else:
+                        logger.warning(
+                            f"Could not read {self.name} from {resource_file_path}"
+                        )
+            except Exception as e:
+                logger.error(f"Could not read resource from file {e}")
+        return None
+
+    def delete_resource_file(self) -> bool:
+        resource_file_path: Optional[Path] = self.get_resource_file_path()
+        if resource_file_path is not None:
+            try:
+                if resource_file_path.exists() and resource_file_path.is_file():
+                    resource_file_path.unlink()
+                    logger.debug(f"Resource file deleted: {str(resource_file_path)}")
+                    return True
+            except Exception as e:
+                logger.error(f"Could not delete resource file {e}")
+        return False
+
+    def attribute(self, name: str) -> Optional[Any]:
+        resource_attributes = self.read_resource_from_file()
+        if resource_attributes is not None:
+            if name in resource_attributes:
+                return resource_attributes[name]
+            else:
+                logger.warning(f"Resource attribute not found: {name}")
+        return None
+
+    def get_secret_data(self) -> Optional[Dict[str, str]]:
+        if self.secret_data is not None:
+            return self.secret_data
+
+        if self.secrets_file is not None:
+            self.secret_data = self.read_yaml_file(self.secrets_file)
+        return self.secret_data
+
+    def get_env_data(self) -> Optional[Dict[str, str]]:
+        if self.env_data is not None:
+            return self.env_data
+
+        if self.env_file is not None:
+            self.env_data = self.read_yaml_file(self.env_file)
+        return self.env_data
```

### Comparing `phidata-1.6.9/phidata/k8s/api_client.py` & `phidata-1.7.0/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/config.py` & `phidata-1.7.0/phidata/k8s/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
-from typing import List, Optional, Dict, Any
+from typing import List, Optional, Dict, Any, Union
 
+from phidata.app.base_app import BaseApp
 from phidata.app.phidata_app import PhidataApp
 from phidata.app.group import AppGroup, get_apps_from_app_groups
 from phidata.app.databox import default_databox_name
 from phidata.infra.config import InfraConfig
 from phidata.k8s.args import K8sArgs
 from phidata.k8s.manager import K8sManager
 from phidata.k8s.resource.group import K8sResourceGroup
@@ -23,15 +24,15 @@
         # K8s context to use
         context: Optional[str] = None,
         # K8s service account to use
         service_account_name: Optional[str] = None,
         # Common K8s labels to add to all resources
         common_labels: Optional[Dict[str, str]] = None,
         # PhidataApp to deploy
-        apps: Optional[List[PhidataApp]] = None,
+        apps: Optional[List[Union[BaseApp, PhidataApp]]] = None,
         # AppGroups to deploy
         app_groups: Optional[List[AppGroup]] = None,
         # K8sResourceGroup to deploy
         resources: Optional[List[K8sResourceGroup]] = None,
         # CreateK8sResourceGroup to deploy
         create_resources: Optional[List[CreateK8sResourceGroup]] = None,
         # Resources dir where k8s manifests are stored
@@ -122,15 +123,15 @@
 
     @common_labels.setter
     def common_labels(self, common_labels: Dict[str, str]) -> None:
         if self.args is not None and common_labels is not None:
             self.args.common_labels = common_labels
 
     @property
-    def apps(self) -> Optional[List[PhidataApp]]:
+    def apps(self) -> Optional[List[Union[BaseApp, PhidataApp]]]:
         if self.args and self.args.apps:
             return self.args.apps
         return None
 
     @property
     def resources(self) -> Optional[List[K8sResourceGroup]]:
         if self.args and self.args.resources:
@@ -167,15 +168,15 @@
             return self.args.eks_cluster
         return None
 
     def apps_are_valid(self) -> bool:
         if self.apps is None:
             return True
         for _app in self.apps:
-            if not isinstance(_app, PhidataApp):
+            if not (isinstance(_app, PhidataApp) or isinstance(_app, BaseApp)):
                 raise TypeError("Invalid App: {}".format(_app))
         return True
 
     def resources_are_valid(self) -> bool:
         if self.resources is None:
             return True
         for _resource in self.resources:
@@ -197,15 +198,15 @@
             and self.resources_are_valid()
             and self.create_resources_are_valid()
         )
 
     def get_k8s_manager(self) -> Optional[K8sManager]:
         return K8sManager(k8s_args=self.args)
 
-    def get_app_by_name(self, app_name: str) -> Optional[PhidataApp]:
+    def get_app_by_name(self, app_name: str) -> Optional[Union[BaseApp, PhidataApp]]:
         if self.apps is None:
             return None
 
         for _app in self.apps:
             try:
                 if app_name == _app.name:
                     return _app
```

### Comparing `phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.7.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.7.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/apps/v1/deployment.py` & `phidata-1.7.0/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/common/port.py` & `phidata-1.7.0/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/core/v1/config_map.py` & `phidata-1.7.0/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/core/v1/container.py` & `phidata-1.7.0/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/core/v1/namespace.py` & `phidata-1.7.0/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-1.7.0/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-1.7.0/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/core/v1/secret.py` & `phidata-1.7.0/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/core/v1/service.py` & `phidata-1.7.0/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/core/v1/service_account.py` & `phidata-1.7.0/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/core/v1/volume.py` & `phidata-1.7.0/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-1.7.0/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/group.py` & `phidata-1.7.0/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/kubeconfig.py` & `phidata-1.7.0/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-1.7.0/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.7.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.7.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-1.7.0/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/enums/api_version.py` & `phidata-1.7.0/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/enums/kind.py` & `phidata-1.7.0/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/enums/manager_status.py` & `phidata-1.7.0/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/enums/pv.py` & `phidata-1.7.0/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/manager.py` & `phidata-1.7.0/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.7.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.7.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-1.7.0/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-1.7.0/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/base.py` & `phidata-1.7.0/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/config_map.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/container.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/namespace.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/pod.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/secret.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/service.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/service_account.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/toleration.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/volume.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-1.7.0/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/group.py` & `phidata-1.7.0/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/kubeconfig.py` & `phidata-1.7.0/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-1.7.0/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-1.7.0/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-1.7.0/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.7.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.7.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-1.7.0/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/types.py` & `phidata-1.7.0/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/resource/utils.py` & `phidata-1.7.0/phidata/k8s/resource/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,20 @@
                         logger.debug(f"type_filter: {type_filter.lower()}")
                         # logger.debug(f"class: {rt.lower()}")
                         if type_filter.lower() != rt.lower():
                             logger.debug(f"  -*- skipping {rt}:{rn}")
                             continue
                     k8s_resources.append(_r)  # type: ignore
 
+                    # Add the resource dependencies to the aws_resources list
+                    if _r.depends_on is not None:
+                        for dep in _r.depends_on:
+                            if isinstance(dep, K8sResource):
+                                k8s_resources.append(dep)
+
         # If its a single resource, verify that the resource is a subclass of
         # K8sResource and add it to the k8s_resources list
         elif isinstance(resource_data, K8sResource):
             rn = resource_data.get_resource_name()
             rt = resource_data.get_resource_type()
             # skip disabled resources
             if not resource_data.enabled:
```

### Comparing `phidata-1.6.9/phidata/k8s/utils/pod.py` & `phidata-1.7.0/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/k8s/worker.py` & `phidata-1.7.0/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/llm/duckdb/agent.py` & `phidata-1.7.0/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/llm/duckdb/chain.py` & `phidata-1.7.0/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/llm/duckdb/connection.py` & `phidata-1.7.0/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/llm/duckdb/loader.py` & `phidata-1.7.0/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/llm/duckdb/query.py` & `phidata-1.7.0/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/llm/duckdb/tool.py` & `phidata-1.7.0/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/product/data_product.py` & `phidata-1.7.0/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/table/local/csv.py` & `phidata-1.7.0/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/table/local/local_table.py` & `phidata-1.7.0/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/table/local/parquet.py` & `phidata-1.7.0/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/table/s3/csv.py` & `phidata-1.7.0/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/table/s3/parquet.py` & `phidata-1.7.0/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/table/s3/s3_table.py` & `phidata-1.7.0/phidata/app/aws_app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,583 +1,502 @@
 from typing import Optional, Any, List, Dict
-from typing_extensions import Literal
+from collections import OrderedDict
 
-from phidata.asset.aws.aws_asset import AwsAsset, AwsAssetArgs
-from phidata.checks.check import Check
-from phidata.aws.resource.s3.bucket import S3Bucket
-from phidata.utils.enums import ExtendedEnum
+from phidata.app.base_app import BaseApp, BaseAppArgs
+from phidata.types.context import ContainerPathContext
 from phidata.utils.log import logger
 
 
-class S3TableFormat(ExtendedEnum):
-    CSV = "csv"
-    IPC = "ipc"
-    ARROW = "arrow"
-    FEATHER = "feather"
-    ORC = "orc"
-    PARQUET = "parquet"
-
-
-class S3TableArgs(AwsAssetArgs):
-    # Table Name
-    name: str
-    # Table Format
-    table_format: S3TableFormat
-    # Database for the table
-    database: str = "default"
-
-    # -*- Table Path
-    # S3 Bucket
-    bucket: Optional[S3Bucket] = None
-    # S3 Bucket Name must be provided if bucket is not provided
-    bucket_name: Optional[str] = None
-    # Path to table directory in bucket. Without the s3:// prefix
-    path: Optional[str] = None
-    # To level directory for all tables
-    top_level_dir: Optional[str] = None
-    # A template string used to generate basenames of written data files.
-    # The token ‘{i}’ will be replaced with an automatically incremented integer.
-    # If not specified, it defaults to “part-{i}.” + format.default_extname
-    basename_template: Optional[str] = None
-
-    # List of partition columns
-    partitions: Optional[List[str]] = None
-
-    # Maximum number of partitions any batch may be written into.
-    max_partitions: Optional[int] = None
-    # If greater than 0 then this will limit the maximum number of files that can be left open.
-    # If an attempt is made to open too many files then the least recently used file will be closed.
-    # If this setting is set too low you may end up fragmenting your data into many small files.
-    max_open_files: Optional[int] = None
-    # Maximum number of rows per file. If greater than 0 then this will limit how many rows are placed in any single
-    # file. Otherwise there will be no limit and one file will be created in each output directory unless files need
-    # to be closed to respect max_open_files
-    max_rows_per_file: Optional[int] = None
-    # Minimum number of rows per group. When the value is greater than 0, the dataset writer will batch incoming data
-    # and only write the row groups to the disk when sufficient rows have accumulated.
-    min_rows_per_group: Optional[int] = None
-    # Maximum number of rows per group. If the value is greater than 0, then the dataset writer may split up large
-    # incoming batches into multiple row groups. If this value is set, then min_rows_per_group should also be set.
-    # Otherwise it could end up with very small row groups.
-    max_rows_per_group: Optional[int] = None
-    # Controls how the dataset will handle data that already exists in the destination.
-    # The default behavior (‘error’) is to raise an error if any data exists in the destination.
-    # ‘overwrite_or_ignore’ will ignore any existing data and will overwrite files with the same name
-    # as an output file. Other existing files will be ignored. This behavior, in combination with a unique
-    # basename_template for each write, will allow for an append workflow.
-    # ‘delete_matching’ is useful when you are writing a partitioned dataset.
-    # The first time each partition directory is encountered the entire directory will be deleted.
-    # This allows you to overwrite old partitions completely.
-    write_mode: Literal[
-        "delete_matching", "overwrite_or_ignore", "error"
-    ] = "delete_matching"
-
-
-class S3Table(AwsAsset):
-    """Base Class for S3 tables"""
-
-    def __init__(
-        self,
-        # Table Name: required
-        name: str,
-        # Table Format: required
-        table_format: S3TableFormat,
-        # Database for the table
-        database: str = "default",
-        # DataModel for this table
-        data_model: Optional[Any] = None,
-        # Checks to run before reading from disk
-        read_checks: Optional[List[Check]] = None,
-        # Checks to run before writing to disk
-        write_checks: Optional[List[Check]] = None,
-        # -*- Table Path
-        # S3 Bucket
-        bucket: Optional[S3Bucket] = None,
-        # S3 Bucket Name
-        bucket_name: Optional[str] = None,
-        # Path to table directory in bucket. Without the s3:// prefix
-        path: Optional[str] = None,
-        # To level directory for all tables
-        top_level_dir: Optional[str] = "tables",
-        # A template string used to generate basenames of written data files.
-        # The token ‘{i}’ will be replaced with an automatically incremented integer.
-        # If not specified, it defaults to “part-{i}.” + format.default_extname
-        basename_template: Optional[str] = None,
-        # List of partition columns
-        partitions: Optional[List[str]] = None,
-        # Maximum number of partitions any batch may be written into.
-        max_partitions: Optional[int] = None,
-        # If greater than 0 then this will limit the maximum number of files that can be left open.
-        # If an attempt is made to open too many files then the least recently used file will be closed.
-        # If this setting is set too low you may end up fragmenting your data into many small files.
-        max_open_files: Optional[int] = None,
-        # Maximum number of rows per file. If greater than 0 then this will limit how many rows are placed in any single
-        # file. Otherwise there will be no limit and one file will be created in each output directory unless files need
-        # to be closed to respect max_open_files
-        max_rows_per_file: Optional[int] = None,
-        # Minimum number of rows per group. When the value is greater than 0, the dataset writer will batch incoming data
-        # and only write the row groups to the disk when sufficient rows have accumulated.
-        min_rows_per_group: Optional[int] = None,
-        # Maximum number of rows per group. If the value is greater than 0, then the dataset writer may split up large
-        # incoming batches into multiple row groups. If this value is set, then min_rows_per_group should also be set.
-        # Otherwise it could end up with very small row groups.
-        max_rows_per_group: Optional[int] = None,
-        # Controls how the dataset will handle data that already exists in the destination.
-        # The default behavior (‘error’) is to raise an error if any data exists in the destination.
-        # ‘overwrite_or_ignore’ will ignore any existing data and will overwrite files with the same name
-        # as an output file. Other existing files will be ignored. This behavior, in combination with a unique
-        # basename_template for each write, will allow for an append workflow.
-        # ‘delete_matching’ is useful when you are writing a partitioned dataset.
-        # The first time each partition directory is encountered the entire directory will be deleted.
-        # This allows you to overwrite old partitions completely.
-        write_mode: Literal[
-            "delete_matching", "overwrite_or_ignore", "error"
-        ] = "delete_matching",
-        version: Optional[str] = None,
-        enabled: bool = True,
-        **kwargs,
-    ) -> None:
+class AwsAppArgs(BaseAppArgs):
+    # -*- AWS Configuration
+    # List of subnets: str or Subnet
+    aws_subnets: Optional[List[Any]] = None
+    # List of security groups: str or SecurityGroup
+    aws_security_groups: Optional[List[Any]] = None
+
+    # -*- ECS Configuration
+    ecs_cluster: Optional[Any] = None
+    ecs_launch_type: str = "FARGATE"
+    ecs_task_cpu: str = "1024"
+    ecs_task_memory: str = "2048"
+    ecs_service_count: int = 1
+    assign_public_ip: Optional[bool] = None
+    ecs_enable_exec: bool = True
+
+    # -*- LoadBalancer Configuration
+    load_balancer: Optional[Any] = None
+    listener: Optional[Any] = None
+    # Create a load balancer if load_balancer is None
+    create_load_balancer: bool = False
+    # HTTP or HTTPS
+    load_balancer_protocol: str = "HTTP"
+    load_balancer_security_groups: Optional[List[Any]] = None
+    # Default 80 for HTTP and 443 for HTTPS
+    load_balancer_port: Optional[int] = None
+    load_balancer_certificate: Optional[Any] = None
+    load_balancer_certificate_arn: Optional[str] = None
+
+    # -*- TargetGroup Configuration
+    target_group: Optional[Any] = None
+    # HTTP or HTTPS
+    target_group_protocol: str = "HTTP"
+    # Default 80 for HTTP and 443 for HTTPS
+    target_group_port: Optional[int] = None
+    target_group_type: str = "ip"
+    health_check_protocol: Optional[str] = None
+    health_check_port: Optional[str] = None
+    health_check_enabled: Optional[bool] = None
+    health_check_path: Optional[str] = None
+    health_check_interval_seconds: Optional[int] = None
+    health_check_timeout_seconds: Optional[int] = None
+    healthy_threshold_count: Optional[int] = None
+    unhealthy_threshold_count: Optional[int] = None
+
+
+class AwsApp(BaseApp):
+    def __init__(self) -> None:
         super().__init__()
-        try:
-            self.args: S3TableArgs = S3TableArgs(
-                name=name,
-                table_format=table_format,
-                database=database,
-                data_model=data_model,
-                read_checks=read_checks,
-                write_checks=write_checks,
-                bucket=bucket,
-                bucket_name=bucket_name,
-                path=path,
-                top_level_dir=top_level_dir,
-                basename_template=basename_template,
-                partitions=partitions,
-                max_partitions=max_partitions,
-                max_open_files=max_open_files,
-                max_rows_per_file=max_rows_per_file,
-                min_rows_per_group=min_rows_per_group,
-                max_rows_per_group=max_rows_per_group,
-                write_mode=write_mode,
-                version=version,
-                enabled=enabled,
-                **kwargs,
-            )
-        except Exception as e:
-            logger.error(f"Args for {self.name} are not valid")
-            raise
 
-    @property
-    def table_format(self) -> Optional[S3TableFormat]:
-        return self.args.table_format if self.args else None
+        # Args for the AwsAppArgs, updated by the subclass
+        self.args: AwsAppArgs = AwsAppArgs()
 
-    @table_format.setter
-    def table_format(self, table_format: S3TableFormat) -> None:
-        if self.args and table_format:
-            self.args.table_format = table_format
+        # Dict of AwsResourceGroups
+        # Type: Optional[Dict[str, AwsResourceGroup]]
+        self.aws_resource_groups: Optional[Dict[str, Any]] = None
 
     @property
-    def database(self) -> Optional[str]:
-        return self.args.database if self.args else None
+    def aws_subnets(self) -> Optional[List[Any]]:
+        return self.args.aws_subnets
 
-    @database.setter
-    def database(self, database: str) -> None:
-        if self.args and database:
-            self.args.database = database
+    @aws_subnets.setter
+    def aws_subnets(self, aws_subnets: List[Any]) -> None:
+        if self.args is not None and aws_subnets is not None:
+            self.args.aws_subnets = aws_subnets
 
     @property
-    def bucket(self) -> Optional[S3Bucket]:
-        return self.args.bucket if self.args else None
+    def aws_security_groups(self) -> Optional[List[Any]]:
+        return self.args.aws_security_groups
 
-    @bucket.setter
-    def bucket(self, bucket: S3Bucket) -> None:
-        if self.args and bucket:
-            self.args.bucket = bucket
+    @aws_security_groups.setter
+    def aws_security_groups(self, aws_security_groups: List[Any]) -> None:
+        if self.args is not None and aws_security_groups is not None:
+            self.args.aws_security_groups = aws_security_groups
 
     @property
-    def bucket_name(self) -> Optional[str]:
-        return self.args.bucket_name if self.args else None
+    def ecs_cluster(self) -> Optional[Any]:
+        return self.args.ecs_cluster
 
-    @bucket_name.setter
-    def bucket_name(self, bucket_name: str) -> None:
-        if self.args and bucket_name:
-            self.args.bucket_name = bucket_name
+    @ecs_cluster.setter
+    def ecs_cluster(self, ecs_cluster: Any) -> None:
+        if self.args is not None and ecs_cluster is not None:
+            self.args.ecs_cluster = ecs_cluster
 
     @property
-    def path(self) -> Optional[str]:
-        return self.args.path if self.args else None
+    def ecs_launch_type(self) -> Optional[str]:
+        return self.args.ecs_launch_type
 
-    @path.setter
-    def path(self, path: str) -> None:
-        if self.args and path:
-            self.args.path = path
+    @ecs_launch_type.setter
+    def ecs_launch_type(self, ecs_launch_type: str) -> None:
+        if self.args is not None and ecs_launch_type is not None:
+            self.args.ecs_launch_type = ecs_launch_type
 
     @property
-    def top_level_dir(self) -> Optional[str]:
-        return self.args.top_level_dir if self.args else None
+    def ecs_task_cpu(self) -> Optional[str]:
+        return self.args.ecs_task_cpu
 
-    @top_level_dir.setter
-    def top_level_dir(self, top_level_dir: str) -> None:
-        if self.args and top_level_dir:
-            self.args.top_level_dir = top_level_dir
+    @ecs_task_cpu.setter
+    def ecs_task_cpu(self, ecs_task_cpu: str) -> None:
+        if self.args is not None and ecs_task_cpu is not None:
+            self.args.ecs_task_cpu = ecs_task_cpu
 
     @property
-    def basename_template(self) -> Optional[str]:
-        return self.args.basename_template if self.args else None
+    def ecs_task_memory(self) -> Optional[str]:
+        return self.args.ecs_task_memory
 
-    @basename_template.setter
-    def basename_template(self, basename_template: str) -> None:
-        if self.args and basename_template:
-            self.args.basename_template = basename_template
+    @ecs_task_memory.setter
+    def ecs_task_memory(self, ecs_task_memory: str) -> None:
+        if self.args is not None and ecs_task_memory is not None:
+            self.args.ecs_task_memory = ecs_task_memory
 
     @property
-    def partitions(self) -> Optional[List[str]]:
-        return self.args.partitions if self.args else None
+    def ecs_service_count(self) -> Optional[int]:
+        return self.args.ecs_service_count
 
-    @partitions.setter
-    def partitions(self, partitions: List[str]) -> None:
-        if self.args and partitions:
-            self.args.partitions = partitions
+    @ecs_service_count.setter
+    def ecs_service_count(self, ecs_service_count: int) -> None:
+        if self.args is not None and ecs_service_count is not None:
+            self.args.ecs_service_count = ecs_service_count
 
     @property
-    def max_partitions(self) -> Optional[int]:
-        return self.args.max_partitions if self.args else None
+    def assign_public_ip(self) -> Optional[bool]:
+        return self.args.assign_public_ip
 
-    @max_partitions.setter
-    def max_partitions(self, max_partitions: int) -> None:
-        if self.args and max_partitions:
-            self.args.max_partitions = max_partitions
+    @assign_public_ip.setter
+    def assign_public_ip(self, assign_public_ip: bool) -> None:
+        if self.args is not None and assign_public_ip is not None:
+            self.args.assign_public_ip = assign_public_ip
 
     @property
-    def max_open_files(self) -> Optional[int]:
-        return self.args.max_open_files if self.args else None
+    def ecs_enable_exec(self) -> Optional[bool]:
+        return self.args.ecs_enable_exec
 
-    @max_open_files.setter
-    def max_open_files(self, max_open_files: int) -> None:
-        if self.args and max_open_files:
-            self.args.max_open_files = max_open_files
+    @ecs_enable_exec.setter
+    def ecs_enable_exec(self, ecs_enable_exec: bool) -> None:
+        if self.args is not None and ecs_enable_exec is not None:
+            self.args.ecs_enable_exec = ecs_enable_exec
 
     @property
-    def max_rows_per_file(self) -> Optional[int]:
-        return self.args.max_rows_per_file if self.args else None
+    def create_load_balancer(self) -> Optional[bool]:
+        return self.args.create_load_balancer
 
-    @max_rows_per_file.setter
-    def max_rows_per_file(self, max_rows_per_file: int) -> None:
-        if self.args and max_rows_per_file:
-            self.args.max_rows_per_file = max_rows_per_file
+    @create_load_balancer.setter
+    def create_load_balancer(self, create_load_balancer: bool) -> None:
+        if self.args is not None and create_load_balancer is not None:
+            self.args.create_load_balancer = create_load_balancer
 
     @property
-    def min_rows_per_group(self) -> Optional[int]:
-        return self.args.min_rows_per_group if self.args else None
+    def load_balancer(self) -> Optional[Any]:
+        return self.args.load_balancer
 
-    @min_rows_per_group.setter
-    def min_rows_per_group(self, min_rows_per_group: int) -> None:
-        if self.args and min_rows_per_group:
-            self.args.min_rows_per_group = min_rows_per_group
+    @load_balancer.setter
+    def load_balancer(self, load_balancer: Any) -> None:
+        if self.args is not None and load_balancer is not None:
+            self.args.load_balancer = load_balancer
 
     @property
-    def max_rows_per_group(self) -> Optional[int]:
-        return self.args.max_rows_per_group if self.args else None
+    def load_balancer_protocol(self) -> Optional[str]:
+        return self.args.load_balancer_protocol
 
-    @max_rows_per_group.setter
-    def max_rows_per_group(self, max_rows_per_group: int) -> None:
-        if self.args and max_rows_per_group:
-            self.args.max_rows_per_group = max_rows_per_group
+    @load_balancer_protocol.setter
+    def load_balancer_protocol(self, load_balancer_protocol: str) -> None:
+        if self.args is not None and load_balancer_protocol is not None:
+            self.args.load_balancer_protocol = load_balancer_protocol
 
     @property
-    def write_mode(
-        self,
-    ) -> Optional[Literal["delete_matching", "overwrite_or_ignore", "error"]]:
-        return self.args.write_mode if self.args else None
+    def load_balancer_port(self) -> Optional[int]:
+        return self.args.load_balancer_port
 
-    @write_mode.setter
-    def write_mode(
-        self, write_mode: Literal["delete_matching", "overwrite_or_ignore", "error"]
-    ) -> None:
-        if self.args and write_mode:
-            self.args.write_mode = write_mode
+    @load_balancer_port.setter
+    def load_balancer_port(self, load_balancer_port: int) -> None:
+        if self.args is not None and load_balancer_port is not None:
+            self.args.load_balancer_port = load_balancer_port
 
     @property
-    def table_location(self) -> str:
-        if self.path is not None:
-            return self.path
-        else:
-            if self.bucket_name is not None:
-                return "{}/{}{}/{}".format(
-                    self.bucket_name,
-                    f"{self.top_level_dir}/" if self.top_level_dir else "",
-                    self.database,
-                    self.name,
-                )
-            if self.bucket is not None:
-                return "{}/{}{}/{}".format(
-                    self.bucket.name,
-                    f"{self.top_level_dir}/" if self.top_level_dir else "",
-                    self.database,
-                    self.name,
-                )
-        return ""
+    def load_balancer_certificate_arn(self) -> Optional[str]:
+        return self.args.load_balancer_certificate_arn
+
+    @load_balancer_certificate_arn.setter
+    def load_balancer_certificate_arn(self, load_balancer_certificate_arn: str) -> None:
+        if self.args is not None and load_balancer_certificate_arn is not None:
+            self.args.load_balancer_certificate_arn = load_balancer_certificate_arn
+
+    def get_container_env_ecs(
+        self, container_paths: ContainerPathContext
+    ) -> Dict[str, str]:
+        from phidata.constants import (
+            PYTHONPATH_ENV_VAR,
+            PHIDATA_RUNTIME_ENV_VAR,
+            SCRIPTS_DIR_ENV_VAR,
+            STORAGE_DIR_ENV_VAR,
+            META_DIR_ENV_VAR,
+            PRODUCTS_DIR_ENV_VAR,
+            NOTEBOOKS_DIR_ENV_VAR,
+            WORKFLOWS_DIR_ENV_VAR,
+            WORKSPACE_ROOT_ENV_VAR,
+            WORKSPACE_CONFIG_DIR_ENV_VAR,
+        )
+
+        # Container Environment
+        container_env: Dict[str, str] = self.container_env or {}
+        container_env.update(
+            {
+                PHIDATA_RUNTIME_ENV_VAR: "ecs",
+                SCRIPTS_DIR_ENV_VAR: container_paths.scripts_dir or "",
+                STORAGE_DIR_ENV_VAR: container_paths.storage_dir or "",
+                META_DIR_ENV_VAR: container_paths.meta_dir or "",
+                PRODUCTS_DIR_ENV_VAR: container_paths.products_dir or "",
+                NOTEBOOKS_DIR_ENV_VAR: container_paths.notebooks_dir or "",
+                WORKFLOWS_DIR_ENV_VAR: container_paths.workflows_dir or "",
+                WORKSPACE_ROOT_ENV_VAR: container_paths.workspace_root or "",
+                WORKSPACE_CONFIG_DIR_ENV_VAR: container_paths.workspace_config_dir
+                or "",
+                "INSTALL_REQUIREMENTS": str(self.args.install_requirements),
+                "REQUIREMENTS_FILE_PATH": container_paths.requirements_file or "",
+                "MOUNT_WORKSPACE": str(self.args.mount_workspace),
+                "WORKSPACE_DIR_CONTAINER_PATH": str(
+                    self.args.workspace_dir_container_path
+                ),
+                "PRINT_ENV_ON_LOAD": str(self.args.print_env_on_load),
+            }
+        )
 
-    ######################################################
-    ## Validate data asset
-    ######################################################
-
-    def is_valid(self) -> bool:
-        return True
-
-    ######################################################
-    ## Build data asset
-    ######################################################
-
-    def build(self) -> bool:
-        logger.debug(f"@build not defined for {self.name}")
-        return False
-
-    ######################################################
-    ## Write DataAsset
-    ######################################################
-
-    def write_table(self, table: Any, **write_options) -> bool:
-        """
-        Write pyarrow.Table to disk.
-
-        https://arrow.apache.org/docs/python/generated/pyarrow.Table.html#pyarrow.Table
-        """
-        # Validate pyarrow is installed
-        try:
-            import pyarrow as pa
-            import pyarrow.dataset as ds
-        except ImportError as ie:
-            raise Exception(
-                f"PyArrow not installed. Please install with `pip install pyarrow`"
-            ) from ie
-
-        # Validate table
-        if table is None or not isinstance(table, pa.Table):
-            logger.error("Table invalid")
-            return False
-
-        # Check table_location is available
-        table_location = self.table_location
-        if table_location is None:
-            logger.error("Table location invalid")
-            return False
-
-        # Check S3FileSystem is available
-        fs = self._get_fs()
-        if fs is None:
-            logger.error("Could not create S3FileSystem")
-            return False
-
-        logger.debug("Format: {}".format(self.args.table_format.value))
-        try:
-            # Run write checks
-            if self.write_checks is not None:
-                for check in self.write_checks:
-                    if not check.check_table(table):
-                        return False
-
-            # Create a dict of args which are not null
-            not_null_args: Dict[str, Any] = {}
-            if self.args.basename_template is not None:
-                not_null_args["basename_template"] = self.args.basename_template
-            if self.args.partitions is not None:
-                not_null_args["partitioning"] = self.args.partitions
-                not_null_args["partitioning_flavor"] = "hive"
-                # cast partition keys to string
-                # ref: https://bneijt.nl/blog/write-polars-dataframe-as-parquet-dataset/
-                table = table.cast(
-                    pa.schema(
-                        [
-                            f.with_type(pa.string())
-                            if f.name in self.args.partitions
-                            else f
-                            for f in table.schema
-                        ]
+        if self.args.set_python_path:
+            python_path = self.args.python_path
+            if python_path is None:
+                python_path = container_paths.workspace_root
+                if self.args.add_python_paths is not None:
+                    python_path = "{}:{}".format(
+                        python_path, ":".join(self.args.add_python_paths)
                     )
-                )
-            if self.args.max_partitions is not None:
-                not_null_args["max_partitions"] = self.args.max_partitions
-            if self.args.max_open_files is not None:
-                not_null_args["max_open_files"] = self.args.max_open_files
-            if self.args.max_rows_per_file is not None:
-                not_null_args["max_rows_per_file"] = self.args.max_rows_per_file
-            if self.args.min_rows_per_group is not None:
-                not_null_args["min_rows_per_group"] = self.args.min_rows_per_group
-            if self.args.max_rows_per_group is not None:
-                not_null_args["max_rows_per_group"] = self.args.max_rows_per_group
-
-            # Build file_options: FileFormat specific write options
-            # created using the FileFormat.make_write_options() function.
-            if write_options:
-                file_options = ds.FileFormat.make_write_options(**write_options)
-                not_null_args["file_options"] = file_options
-
-            # Write table to disk
-            ds.write_dataset(
-                table,
-                table_location,
-                format=self.args.table_format.value,
-                filesystem=fs,
-                existing_data_behavior=self.args.write_mode,
-                **not_null_args,
+            if python_path is not None:
+                container_env[PYTHONPATH_ENV_VAR] = python_path
+
+        # Set aws env vars
+        self.set_aws_env_vars(env_dict=container_env)
+
+        # Update the container env using env_file
+        env_data_from_file = self.get_env_data()
+        if env_data_from_file is not None:
+            container_env.update(
+                {k: str(v) for k, v in env_data_from_file.items() if v is not None}
             )
-            logger.info(f"Table {self.name} written to {table_location}")
 
-            return True
-        except Exception:
-            logger.error("Could not write table: {}".format(self.name))
-            raise
-
-    def write_polars_df(
-        self,
-        df: Optional[Any] = None,
-        options: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ) -> bool:
-        """
-        Write Polars DataFrame to disk.
-        """
-        # Validate polars is installed
-        try:
-            import polars as pl  # type: ignore
-        except ImportError as ie:
-            logger.error(f"Polars not installed: {ie}")
-            return False
-
-        # Validate df
-        if df is None or not isinstance(df, pl.DataFrame):
-            logger.error("DataFrame invalid")
-            return False
-
-        # Create arrow table and write to disk
-        return self.write_table(df.to_arrow(), options=options)
-
-    def write_pandas_df(self, df: Optional[Any] = None, **kwargs) -> bool:
-        logger.debug(f"@write_pandas_df not defined for {self.name}")
-        return False
-
-    ######################################################
-    ## Create DataAsset
-    ######################################################
-
-    def _create(self) -> bool:
-        logger.error(f"@_create not defined for {self.name}")
-        return False
-
-    def post_create(self) -> bool:
-        return True
-
-    ######################################################
-    ## Read DataAsset
-    ######################################################
-
-    def read_table(self, **read_options) -> Optional[Any]:
-        """
-        Read pyarrow.Table from disk.
-
-        https://arrow.apache.org/docs/python/generated/pyarrow.Table.html#pyarrow.Table
-        """
-        # Validate pyarrow is installed
-        try:
-            import pyarrow as pa
-            import pyarrow.dataset as ds
-        except ImportError as ie:
-            raise Exception(
-                f"PyArrow not installed. Please install with `pip install pyarrow`"
-            ) from ie
-
-        # Check table_location is available
-        table_location = self.table_location
-        if table_location is None:
-            logger.error("Table location invalid")
-            return False
-
-        # Check S3FileSystem is available
-        fs = self._get_fs()
-        if fs is None:
-            logger.error("Could not create S3FileSystem")
-            return False
-
-        logger.debug("Format: {}".format(self.args.table_format.value))
-        try:
-            # Create a dict of args which are not null
-            not_null_args: Dict[str, Any] = {}
-            if self.args.partitions is not None:
-                not_null_args["partitioning"] = "hive"
-
-            # Read dataset from s3
-            # https://arrow.apache.org/docs/python/generated/pyarrow.dataset.dataset.html#pyarrow.dataset.dataset
-            # https://arrow.apache.org/docs/python/generated/pyarrow.dataset.Dataset.html#pyarrow.dataset.Dataset
-            dataset: ds.Dataset = ds.dataset(
-                table_location,
-                format=self.args.table_format.value,
-                filesystem=fs,
-                **not_null_args,
+        # Update the container env using secrets_file
+        secret_data_from_file = self.get_secret_data()
+        if secret_data_from_file is not None:
+            container_env.update(
+                {k: str(v) for k, v in secret_data_from_file.items() if v is not None}
             )
 
-            # Convert dataset to table
-            # https://arrow.apache.org/docs/python/generated/pyarrow.dataset.Dataset.html#pyarrow.dataset.Dataset.to_table
-            table: pa.Table = dataset.to_table(**read_options)
-
-            # Run read checks
-            if self.read_checks is not None:
-                for check in self.read_checks:
-                    if not check.check_table(table):
-                        return None
-
-            return table
-        except Exception:
-            logger.error("Could not read table: {}".format(self.name))
-            raise
+        # Update the container env with user provided env
+        # this overwrites any existing variables with the same key
+        if self.args.env is not None and isinstance(self.args.env, dict):
+            container_env.update(
+                {k: v for k, v in self.args.env.items() if v is not None}
+            )
+
+        # logger.debug("Container Environment: {}".format(container_env))
+        return container_env
 
-    def read_polars_df(
-        self, options: Optional[Dict[str, Any]] = None, **kwargs
+    def get_container_command_aws(self) -> Optional[List[str]]:
+        if isinstance(self.args.command, str):
+            return self.args.command.split(" ")
+        return self.args.command
+
+    def get_aws_rg(
+        self, aws_build_context: Any, defer_api_calls: bool = False
     ) -> Optional[Any]:
-        """
-        Read Polars DataFrame from disk.
+        from phidata.aws.resource.group import (
+            AwsResourceGroup,
+            EcsCluster,
+            EcsContainer,
+            EcsTaskDefinition,
+            EcsService,
+            LoadBalancer,
+            TargetGroup,
+            Listener,
+            AcmCertificate,
+        )
+
+        # -*- Build Container Paths
+        container_paths: Optional[ContainerPathContext] = self.get_container_paths()
+        if container_paths is None:
+            raise Exception("Could not build Container Paths")
+        logger.debug(f"ContainerPaths: {container_paths.json(indent=2)}")
+
+        app_name = self.name
+        workspace_name = container_paths.workspace_name
+        logger.debug(f"Building AwsResourceGroup: {app_name} for {workspace_name}")
+
+        # -*- Build Container Environment
+        container_env: Dict[str, str] = self.get_container_env_ecs(
+            container_paths=container_paths
+        )
+
+        # -*- Create ECS cluster
+        ecs_cluster = self.args.ecs_cluster
+        if ecs_cluster is None:
+            ecs_cluster = EcsCluster(
+                name=f"{app_name}-cluster",
+                ecs_cluster_name=app_name,
+                capacity_providers=[self.args.ecs_launch_type],
+                save_output=self.args.save_output,
+                resource_dir=self.args.resource_dir or app_name,
+                skip_create=self.args.skip_create,
+                skip_delete=self.args.skip_delete,
+                wait_for_creation=self.args.wait_for_creation,
+                wait_for_deletion=self.args.wait_for_deletion,
+            )
 
-        options: Dict[str, Any]
-            Additional options to pass to the reader.
-            More info:
-                https://arrow.apache.org/docs/python/generated/pyarrow.dataset.Scanner.html#pyarrow.dataset.Scanner.from_dataset
-                https://arrow.apache.org/docs/python/generated/pyarrow.dataset.dataset.html#pyarrow.dataset.dataset.to_table
-        """
-        # Validate polars is installed
-        try:
-            import polars as pl
-        except ImportError as ie:
-            logger.error(f"Polars not installed: {ie}")
-            return None
-
-        # Convert table to polars DataFrame
-        # https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.from_arrow.html
-        return pl.from_arrow(self.read_table(options=options))
-
-    def read_pandas_df(self, **kwargs) -> Optional[Any]:
-        logger.debug(f"@read_pandas_df not defined for {self.name}")
-        return False
-
-    def _read(self) -> Any:
-        logger.error(f"@_read not defined for {self.name}")
-        return False
-
-    ######################################################
-    ## Update DataAsset
-    ######################################################
-
-    def _update(self) -> Any:
-        logger.error(f"@_update not defined for {self.name}")
-        return False
-
-    def post_update(self) -> bool:
-        return True
-
-    ######################################################
-    ## Delete DataAsset
-    ######################################################
-
-    def _delete(self) -> Any:
-        logger.error(f"@_delete not defined for {self.name}")
-        return False
+        # -*- Create Load Balancer
+        load_balancer = self.args.load_balancer
+        if load_balancer is None and self.args.create_load_balancer:
+            if self.args.load_balancer_protocol not in ["HTTP", "HTTPS"]:
+                raise Exception(
+                    "Load Balancer Protocol must be one of: HTTP, HTTPS. "
+                    f"Got: {self.args.load_balancer_protocol}"
+                )
+            load_balancer_sgs = (
+                self.args.load_balancer_security_groups or self.args.aws_security_groups
+            )
+            load_balancer = LoadBalancer(
+                name=f"{app_name}-lb",
+                subnets=self.args.aws_subnets,
+                security_groups=load_balancer_sgs,
+                protocol=self.args.load_balancer_protocol,
+                save_output=self.args.save_output,
+                resource_dir=self.args.resource_dir or app_name,
+                skip_create=self.args.skip_create,
+                skip_delete=self.args.skip_delete,
+                wait_for_creation=self.args.wait_for_creation,
+                wait_for_deletion=self.args.wait_for_deletion,
+            )
 
-    def post_delete(self) -> bool:
-        return True
+        # -*- Create Target Group
+        target_group = self.args.target_group
+        if target_group is None and self.args.create_load_balancer:
+            if self.args.target_group_protocol not in ["HTTP", "HTTPS"]:
+                raise Exception(
+                    "Target Group Protocol must be one of: HTTP, HTTPS. "
+                    f"Got: {self.args.target_group_protocol}"
+                )
+            target_group = TargetGroup(
+                name=f"{app_name}-tg",
+                port=self.container_port,
+                protocol=self.args.target_group_protocol,
+                subnets=self.args.aws_subnets,
+                target_type=self.args.target_group_type,
+                health_check_protocol=self.args.health_check_protocol,
+                health_check_port=self.args.health_check_port,
+                health_check_enabled=self.args.health_check_enabled,
+                health_check_path=self.args.health_check_path,
+                health_check_interval_seconds=self.args.health_check_interval_seconds,
+                health_check_timeout_seconds=self.args.health_check_timeout_seconds,
+                healthy_threshold_count=self.args.healthy_threshold_count,
+                unhealthy_threshold_count=self.args.unhealthy_threshold_count,
+                save_output=self.args.save_output,
+                resource_dir=self.args.resource_dir or app_name,
+                skip_create=self.args.skip_create,
+                skip_delete=self.args.skip_delete,
+                wait_for_creation=self.args.wait_for_creation,
+                wait_for_deletion=self.args.wait_for_deletion,
+            )
+
+        # -*- Create Listener
+        listener = self.args.listener
+        if listener is None and self.args.create_load_balancer:
+            listener = Listener(
+                name=f"{app_name}-listener",
+                load_balancer=load_balancer,
+                target_group=target_group,
+                save_output=self.args.save_output,
+                resource_dir=self.args.resource_dir or app_name,
+                skip_create=self.args.skip_create,
+                skip_delete=self.args.skip_delete,
+                wait_for_creation=self.args.wait_for_creation,
+                wait_for_deletion=self.args.wait_for_deletion,
+            )
+            if self.args.load_balancer_certificate_arn is not None:
+                listener.certificates = [
+                    {"CertificateArn": self.args.load_balancer_certificate_arn}
+                ]
+            if self.args.load_balancer_certificate is not None:
+                listener.acm_certificates = [self.args.load_balancer_certificate]
+
+        # -*- Build Container Command
+        container_cmd: Optional[List[str]] = self.get_container_command_aws()
+        if container_cmd:
+            logger.debug("Command: {}".format(" ".join(container_cmd)))
+
+        # -*- Create ECS Container
+        ecs_container = EcsContainer(
+            name=app_name,
+            image=self.get_image_str(),
+            port_mappings=[{"containerPort": self.container_port}],
+            command=container_cmd,
+            environment=[{"name": k, "value": v} for k, v in container_env.items()],
+            log_configuration={
+                "logDriver": "awslogs",
+                "options": {
+                    "awslogs-group": app_name,
+                    "awslogs-region": self.aws_region,
+                    "awslogs-create-group": "true",
+                    "awslogs-stream-prefix": app_name,
+                },
+            },
+            env_from_secrets=self.args.aws_secrets,
+            save_output=self.args.save_output,
+            resource_dir=self.args.resource_dir or app_name,
+            skip_create=self.args.skip_create,
+            skip_delete=self.args.skip_delete,
+            wait_for_creation=self.args.wait_for_creation,
+            wait_for_deletion=self.args.wait_for_deletion,
+        )
+
+        # -*- Create ECS Task Definition
+        ecs_task_definition = EcsTaskDefinition(
+            name=f"{app_name}-td",
+            family=app_name,
+            network_mode="awsvpc",
+            cpu=self.args.ecs_task_cpu,
+            memory=self.args.ecs_task_memory,
+            containers=[ecs_container],
+            requires_compatibilities=[self.args.ecs_launch_type],
+            add_ecs_exec_policy=True,
+            add_ecs_secret_policy=True,
+            save_output=self.args.save_output,
+            resource_dir=self.args.resource_dir or app_name,
+            skip_create=self.args.skip_create,
+            skip_delete=self.args.skip_delete,
+            wait_for_creation=self.args.wait_for_creation,
+            wait_for_deletion=self.args.wait_for_deletion,
+        )
+
+        # -*- Create ECS Service
+        ecs_service = EcsService(
+            name=f"{app_name}-service",
+            desired_count=self.args.ecs_service_count,
+            launch_type=self.args.ecs_launch_type,
+            cluster=ecs_cluster,
+            task_definition=ecs_task_definition,
+            target_group=target_group,
+            target_container_name=ecs_container.name,
+            target_container_port=self.container_port,
+            subnets=self.args.aws_subnets,
+            security_groups=self.args.aws_security_groups,
+            assign_public_ip=self.args.assign_public_ip,
+            # Force delete the service.
+            force_delete=True,
+            # Force a new deployment of the service on update.
+            force_new_deployment=True,
+            save_output=self.args.save_output,
+            resource_dir=self.args.resource_dir or app_name,
+            skip_create=self.args.skip_create,
+            skip_delete=self.args.skip_delete,
+            wait_for_creation=self.args.wait_for_creation,
+            wait_for_deletion=self.args.wait_for_deletion,
+        )
+
+        # -*- Create AwsResourceGroup
+        return AwsResourceGroup(
+            name=app_name,
+            enabled=self.enabled,
+            ecs_clusters=[ecs_cluster],
+            ecs_task_definitions=[ecs_task_definition],
+            ecs_services=[ecs_service],
+            load_balancers=[load_balancer],
+            target_groups=[target_group],
+            listeners=[listener],
+        )
+
+    def build_aws_resource_groups(
+        self, aws_build_context: Any, defer_api_calls: bool = False
+    ) -> None:
+        aws_rg = self.get_aws_rg(aws_build_context)
+        if aws_rg is not None:
+            if self.aws_resource_groups is None:
+                self.aws_resource_groups = OrderedDict()
+            self.aws_resource_groups[aws_rg.name] = aws_rg
+
+    def get_aws_resource_groups(
+        self, aws_build_context: Any, defer_api_calls: bool = False
+    ) -> Optional[Dict[str, Any]]:
+        if self.aws_resource_groups is None:
+            self.build_aws_resource_groups(aws_build_context)
+        # # Comment out in production
+        # if self.aws_resource_groups:
+        #     logger.debug("K8sResourceGroups:")
+        #     for rg_name, rg in self.aws_resource_groups.items():
+        #         logger.debug(
+        #             "{}:{}\n{}".format(rg_name, type(rg), rg)
+        #         )
+        return self.aws_resource_groups
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `phidata-1.6.9/phidata/table/sql/postgres.py` & `phidata-1.7.0/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/table/sql/sql_table.py` & `phidata-1.7.0/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/aws/athena/run_query.py` & `phidata-1.7.0/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/aws/emr/create_cluster.py` & `phidata-1.7.0/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/aws/emr/delete_cluster.py` & `phidata-1.7.0/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/aws/glue/start_crawler.py` & `phidata-1.7.0/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/decorator.py` & `phidata-1.7.0/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/download/s3/to_file.py` & `phidata-1.7.0/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/download/url/to_file.py` & `phidata-1.7.0/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/download/url/to_s3.py` & `phidata-1.7.0/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/download/url/to_sql.py` & `phidata-1.7.0/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/plot/sql/query.py` & `phidata-1.7.0/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/python_task.py` & `phidata-1.7.0/phidata/task/python_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,30 +39,28 @@
         dag_id: Optional[str] = None,
         entrypoint_args: Optional[Tuple[Any, ...]] = None,
         entrypoint_kwargs: Optional[Dict] = None,
         version: Optional[str] = None,
         enabled: bool = True,
     ) -> None:
         super().__init__()
-        self.args: Optional[PythonTaskArgs] = None
-        if name is not None and entrypoint is not None:
-            try:
-                self.args = PythonTaskArgs(
-                    name=name,
-                    entrypoint=entrypoint,
-                    task_id=task_id,
-                    dag_id=dag_id,
-                    entrypoint_args=entrypoint_args,
-                    entrypoint_kwargs=entrypoint_kwargs,
-                    version=version,
-                    enabled=enabled,
-                )
-            except Exception as e:
-                logger.error(f"Args for {self.__class__.__name__} are not valid")
-                raise
+        try:
+            self.args: PythonTaskArgs = PythonTaskArgs(
+                name=name,
+                entrypoint=entrypoint,
+                task_id=task_id,
+                dag_id=dag_id,
+                entrypoint_args=entrypoint_args,
+                entrypoint_kwargs=entrypoint_kwargs,
+                version=version,
+                enabled=enabled,
+            )
+        except Exception as e:
+            logger.error(f"Args for {self.name} are not valid {e}")
+            raise
 
     @property
     def entrypoint(self) -> Optional[Callable[..., bool]]:
         return self.args.entrypoint if self.args else None
 
     ######################################################
     ## Run PythonTask
```

### Comparing `phidata-1.6.9/phidata/task/run/sql/query.py` & `phidata-1.7.0/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/task.py` & `phidata-1.7.0/phidata/task/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         version: Optional[str] = None,
         enabled: bool = True,
         run_context: Optional[RunContext] = None,
         path_context: Optional[PathContext] = None,
         airflow_context: Optional[AirflowContext] = None,
     ) -> None:
         super().__init__()
-        self.args: Optional[TaskArgs] = None
+        self.args: TaskArgs = TaskArgs()
         if name is not None and task_id is not None:
             self.args = TaskArgs(
                 name=name,
                 task_id=task_id,
                 dag_id=dag_id,
                 version=version,
                 enabled=enabled,
```

### Comparing `phidata-1.6.9/phidata/task/task_relatives.py` & `phidata-1.7.0/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/upload/file/to_s3.py` & `phidata-1.7.0/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/task/upload/file/to_sql.py` & `phidata-1.7.0/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/types/airflow.py` & `phidata-1.7.0/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/types/context.py` & `phidata-1.7.0/phidata/types/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 
 class PathContext(BaseModel):
     # Env specific path variables - their values are different on
     # local, docker or cloud environments.
     # These are updated by `phi wf run` for local runs
     # And are provided as Environment variables on containers
-
     scripts_dir: Optional[Path] = None
     storage_dir: Optional[Path] = None
     meta_dir: Optional[Path] = None
     products_dir: Optional[Path] = None
     notebooks_dir: Optional[Path] = None
     workspace_config_dir: Optional[Path] = None
     workflow_file: Optional[Path] = None
```

### Comparing `phidata-1.6.9/phidata/types/phidata_runtime.py` & `phidata-1.7.0/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/cli_console.py` & `phidata-1.7.0/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/common.py` & `phidata-1.7.0/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/compare.py` & `phidata-1.7.0/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/context.py` & `phidata-1.7.0/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/dttm.py` & `phidata-1.7.0/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/enums.py` & `phidata-1.7.0/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/env_file.py` & `phidata-1.7.0/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/env_var.py` & `phidata-1.7.0/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/filesystem.py` & `phidata-1.7.0/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/log.py` & `phidata-1.7.0/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/print_table.py` & `phidata-1.7.0/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/utils/workspace_path.py` & `phidata-1.7.0/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/workflow/decorator.py` & `phidata-1.7.0/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/workflow/workflow.py` & `phidata-1.7.0/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/workflow/workflow_relatives.py` & `phidata-1.7.0/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.9/phidata/workspace/settings.py` & `phidata-1.7.0/phidata/workspace/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 
     # Workspace name: used for naming cloud resources
     ws_name: str
     # Workspace git repo url: used to git-sync DAGs and Charts
     ws_repo: Optional[str] = None
     # Path to the workspace root
     ws_root: Path
+    # default env for phi ws commands
+    default_env: Optional[str] = None
+    # default config for phi ws commands
+    default_config: Optional[str] = None
     #
     # -*- Dev settings
     #
     dev_env: str = "dev"
     # Dev git repo branch: used to git-sync DAGs and Charts
     dev_branch: str = "main"
     # Key for naming dev resources
@@ -130,14 +134,28 @@
     # Private subnets. 1 in each AZ.
     private_subnets: List[str] = []
     # Subnet IDs. 1 in each AZ.
     # Derived from public and private subnets if not provided.
     subnet_ids: Optional[List[str]] = None
     # Security Groups
     security_groups: Optional[List[str]] = None
+    aws_profile: Optional[str] = None
+    aws_config_file: Optional[str] = None
+    aws_shared_credentials_file: Optional[str] = None
+    # -*- Cli settings
+    # Set to True if `phi` should continue creating
+    # resources after a resource creation has failed
+    continue_on_create_failure: Optional[bool] = None
+    # Set to True if `phi` should continue deleting
+    # resources after a resource deleting has failed
+    # Defaults to True because we normally want to continue deleting
+    continue_on_delete_failure: Optional[bool] = None
+    # Set to True if `phi` should continue patching
+    # resources after a resource patch has failed
+    continue_on_patch_failure: Optional[bool] = None
     #
     # -*- Image Settings
     #
     # Repository for images
     image_repo: str = "phidata"
     # Suffix added to the image name
     image_suffix: Optional[str] = None
```

### Comparing `phidata-1.6.9/phidata.egg-info/SOURCES.txt` & `phidata-1.7.0/phidata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 phidata.egg-info/requires.txt
 phidata.egg-info/top_level.txt
 phidata/airflow/__init__.py
 phidata/airflow/airflow_installed.py
 phidata/airflow/operators/__init__.py
 phidata/airflow/operators/empty.py
 phidata/app/__init__.py
+phidata/app/aws_app.py
+phidata/app/base_app.py
+phidata/app/docker_app.py
 phidata/app/group.py
+phidata/app/k8s_app.py
 phidata/app/phidata_app.py
 phidata/app/airflow/__init__.py
 phidata/app/airflow/airflow_base.py
 phidata/app/airflow/airflow_flower.py
 phidata/app/airflow/airflow_manager.py
 phidata/app/airflow/airflow_scheduler.py
 phidata/app/airflow/airflow_webserver.py
@@ -41,18 +45,19 @@
 phidata/app/django/__init__.py
 phidata/app/django/django_app.py
 phidata/app/elastic/__init__.py
 phidata/app/elastic/elastic_app.py
 phidata/app/elasticsearch/__init__.py
 phidata/app/elasticsearch/elasticsearch.py
 phidata/app/fastapi/__init__.py
-phidata/app/fastapi/fastapi.py
+phidata/app/fastapi/fastapi_server.py
 phidata/app/grafana/__init__.py
 phidata/app/grafana/grafana.py
 phidata/app/jupyter/__init__.py
+phidata/app/jupyter/jupyter.py
 phidata/app/jupyter/jupyter_hub.py
 phidata/app/jupyter/jupyter_lab.py
 phidata/app/k8s/__init__.py
 phidata/app/k8s/app.py
 phidata/app/k8s/dir.py
 phidata/app/k8s/url.py
 phidata/app/mysql/__init__.py
@@ -72,15 +77,15 @@
 phidata/app/server/api_server.py
 phidata/app/server/server_base.py
 phidata/app/spark/__init__.py
 phidata/app/spark/spark_base.py
 phidata/app/spark/spark_driver.py
 phidata/app/spark/spark_worker.py
 phidata/app/streamlit/__init__.py
-phidata/app/streamlit/streamlit.py
+phidata/app/streamlit/streamlit_app.py
 phidata/app/superset/__init__.py
 phidata/app/superset/superset_base.py
 phidata/app/superset/superset_init.py
 phidata/app/superset/superset_webserver.py
 phidata/app/superset/superset_worker.py
 phidata/app/superset/superset_worker_beat.py
 phidata/app/traefik/__init__.py
@@ -94,14 +99,15 @@
 phidata/asset/local/__init__.py
 phidata/asset/local/file.py
 phidata/asset/local/local_asset.py
 phidata/aws/__init__.py
 phidata/aws/api_client.py
 phidata/aws/args.py
 phidata/aws/config.py
+phidata/aws/driver.py
 phidata/aws/exceptions.py
 phidata/aws/manager.py
 phidata/aws/worker.py
 phidata/aws/athena/__init__.py
 phidata/aws/athena/query.py
 phidata/aws/create/__init__.py
 phidata/aws/create/iam/__init__.py
@@ -117,14 +123,15 @@
 phidata/aws/resource/acm/__init__.py
 phidata/aws/resource/acm/certificate.py
 phidata/aws/resource/athena/__init__.py
 phidata/aws/resource/athena/query.py
 phidata/aws/resource/cloudformation/__init__.py
 phidata/aws/resource/cloudformation/stack.py
 phidata/aws/resource/ec2/__init__.py
+phidata/aws/resource/ec2/security_group.py
 phidata/aws/resource/ec2/subnet.py
 phidata/aws/resource/ec2/volume.py
 phidata/aws/resource/ecs/__init__.py
 phidata/aws/resource/ecs/cluster.py
 phidata/aws/resource/ecs/container.py
 phidata/aws/resource/ecs/service.py
 phidata/aws/resource/ecs/task_definition.py
@@ -154,14 +161,15 @@
 phidata/aws/resource/rds/db_cluster.py
 phidata/aws/resource/rds/db_instance.py
 phidata/aws/resource/rds/db_subnet_group.py
 phidata/aws/resource/s3/__init__.py
 phidata/aws/resource/s3/bucket.py
 phidata/aws/resource/secret/__init__.py
 phidata/aws/resource/secret/manager.py
+phidata/aws/resource/secret/reader.py
 phidata/aws/s3/__init__.py
 phidata/aws/s3/csv_dataset.py
 phidata/aws/s3/dataset.py
 phidata/aws/s3/dataset_base.py
 phidata/aws/s3/object.py
 phidata/checks/__init__.py
 phidata/checks/check.py
@@ -311,14 +319,16 @@
 phidata/llm/duckdb/chain.py
 phidata/llm/duckdb/connection.py
 phidata/llm/duckdb/loader.py
 phidata/llm/duckdb/query.py
 phidata/llm/duckdb/tool.py
 phidata/product/__init__.py
 phidata/product/data_product.py
+phidata/resource/__init__.py
+phidata/resource/reference.py
 phidata/table/__init__.py
 phidata/table/local/__init__.py
 phidata/table/local/csv.py
 phidata/table/local/local_table.py
 phidata/table/local/parquet.py
 phidata/table/s3/__init__.py
 phidata/table/s3/csv.py
@@ -369,18 +379,21 @@
 phidata/utils/compare.py
 phidata/utils/context.py
 phidata/utils/dttm.py
 phidata/utils/enums.py
 phidata/utils/env_file.py
 phidata/utils/env_var.py
 phidata/utils/filesystem.py
+phidata/utils/get_python_objects_from_module.py
+phidata/utils/json_io.py
+phidata/utils/k8s.py
 phidata/utils/log.py
-phidata/utils/prep_infra_config.py
 phidata/utils/print_table.py
 phidata/utils/workspace_path.py
+phidata/utils/yaml_io.py
 phidata/workflow/__init__.py
 phidata/workflow/decorator.py
 phidata/workflow/workflow.py
 phidata/workflow/workflow_relatives.py
 phidata/workflow/dev/__init__.py
 phidata/workspace/__init__.py
 phidata/workspace/config.py
```

### Comparing `phidata-1.6.9/pyproject.toml` & `phidata-1.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "phidata"
-version = "1.6.9"
-description = "Building blocks for Data Engineering"
+version = "1.7.0"
+description = "Phidata is a toolkit for building applications using OSS"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
-  "boto3",
-  "phiterm==1.6.9",
+  "boto3>=1.26.76,<1.26.77",
+  "botocore>=1.29.76,<1.29.77",
+  "phiterm==1.7.0",
   "pyarrow",
   "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
@@ -23,16 +24,16 @@
     "types-PyYAML",
 ]
 aws = [
     "boto3",
 ]
 
 [project.urls]
-homepage = "https://www.phidata.com"
-documentation = "https://www.docs.phidata.com"
+homepage = "https://phidata.com"
+documentation = "https://docs.phidata.com"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.mypy]
 plugins = [
```

