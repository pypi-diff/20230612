# Comparing `tmp/yapapi-0.9.2.tar.gz` & `tmp/yapapi-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapapi-0.9.2.tar", last modified: Tue Jun  7 10:36:57 2022, max compression
+gzip compressed data, was "yapapi-0.9.3.tar", last modified: Tue Oct 11 05:55:48 2022, max compression
```

## Comparing `yapapi-0.9.2.tar` & `yapapi-0.9.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     7652 2022-06-07 10:36:46.472757 yapapi-0.9.2/LICENSE
--rw-r--r--   0        0        0     5863 2022-06-07 10:36:46.472757 yapapi-0.9.2/README.md
--rw-r--r--   0        0        0     4433 2022-06-07 10:36:46.552758 yapapi-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1482 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/__init__.py
--rw-r--r--   0        0        0     9177 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/agreements_pool.py
--rw-r--r--   0        0        0      532 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/contrib/__init__.py
--rw-r--r--   0        0        0        0 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/contrib/service/__init__.py
--rw-r--r--   0        0        0     8992 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/contrib/service/http_proxy.py
--rw-r--r--   0        0        0       44 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/contrib/strategy/__init__.py
--rw-r--r--   0        0        0     3157 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/contrib/strategy/provider_filter.py
--rw-r--r--   0        0        0    13615 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/ctx.py
--rw-r--r--   0        0        0    39962 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/engine.py
--rw-r--r--   0        0        0     1077 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/event_dispatcher.py
--rw-r--r--   0        0        0    15694 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/events.py
--rw-r--r--   0        0        0    15036 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/executor/__init__.py
--rw-r--r--   0        0        0     7718 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/executor/_smartq.py
--rw-r--r--   0        0        0      837 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/executor/ctx.py
--rw-r--r--   0        0        0      874 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/executor/events.py
--rw-r--r--   0        0        0     1038 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/executor/strategy.py
--rw-r--r--   0        0        0     4946 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/executor/task.py
--rw-r--r--   0        0        0    23319 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/golem.py
--rw-r--r--   0        0        0    24778 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/log.py
--rw-r--r--   0        0        0    11030 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/network.py
--rw-r--r--   0        0        0      405 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/package/__init__.py
--rw-r--r--   0        0        0     1419 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/package/vm.py
--rw-r--r--   0        0        0     1386 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/payload/__init__.py
--rw-r--r--   0        0        0     1149 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/payload/package.py
--rw-r--r--   0        0        0     6184 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/payload/vm.py
--rw-r--r--   0        0        0     2400 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/props/__init__.py
--rw-r--r--   0        0        0    10669 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/props/base.py
--rw-r--r--   0        0        0     4388 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/props/builder.py
--rw-r--r--   0        0        0     2793 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/props/com.py
--rw-r--r--   0        0        0     1886 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/props/inf.py
--rw-r--r--   0        0        0        0 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/py.typed
--rw-r--r--   0        0        0      410 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/rest/__init__.py
--rw-r--r--   0        0        0    13418 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/rest/activity.py
--rw-r--r--   0        0        0     2955 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/rest/common.py
--rw-r--r--   0        0        0     6693 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/rest/configuration.py
--rw-r--r--   0        0        0    10918 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/rest/market.py
--rw-r--r--   0        0        0     1125 2022-06-07 10:36:46.556758 yapapi-0.9.2/yapapi/rest/net.py
--rw-r--r--   0        0        0     9454 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/rest/payment.py
--rw-r--r--   0        0        0      216 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/rest/resource.py
--rw-r--r--   0        0        0     8490 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/script/__init__.py
--rw-r--r--   0        0        0     1703 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/script/capture.py
--rw-r--r--   0        0        0     9966 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/script/command.py
--rw-r--r--   0        0        0      170 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/services/__init__.py
--rw-r--r--   0        0        0     8221 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/services/cluster.py
--rw-r--r--   0        0        0    17456 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/services/service.py
--rw-r--r--   0        0        0    15902 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/services/service_runner.py
--rw-r--r--   0        0        0     3029 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/services/service_state.py
--rw-r--r--   0        0        0     3961 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/storage/__init__.py
--rw-r--r--   0        0        0    15947 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/storage/gftp.py
--rw-r--r--   0        0        0     5436 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/storage/webdav.py
--rw-r--r--   0        0        0      500 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/strategy/__init__.py
--rw-r--r--   0        0        0     8185 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/strategy/base.py
--rw-r--r--   0        0        0     2455 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/strategy/decrease_score_unconfirmed.py
--rw-r--r--   0        0        0     2602 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/strategy/dummy.py
--rw-r--r--   0        0        0     3342 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/strategy/least_expensive.py
--rw-r--r--   0        0        0     1583 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/strategy/wrapping_strategy.py
--rw-r--r--   0        0        0     5548 2022-06-07 10:36:46.560758 yapapi-0.9.2/yapapi/utils.py
--rw-r--r--   0        0        0     7760 2022-06-07 10:36:58.029633 yapapi-0.9.2/setup.py
--rw-r--r--   0        0        0     8030 2022-06-07 10:36:58.030184 yapapi-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     7652 2022-10-11 05:55:35.177903 yapapi-0.9.3/LICENSE
+-rw-r--r--   0        0        0     5863 2022-10-11 05:55:35.177903 yapapi-0.9.3/README.md
+-rw-r--r--   0        0        0     4570 2022-10-11 05:55:35.257902 yapapi-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1482 2022-10-11 05:55:35.261902 yapapi-0.9.3/yapapi/__init__.py
+-rw-r--r--   0        0        0     9411 2022-10-11 05:55:35.261902 yapapi-0.9.3/yapapi/agreements_pool.py
+-rw-r--r--   0        0        0      532 2022-10-11 05:55:35.261902 yapapi-0.9.3/yapapi/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-11 05:55:35.261902 yapapi-0.9.3/yapapi/contrib/service/__init__.py
+-rw-r--r--   0        0        0     8992 2022-10-11 05:55:35.261902 yapapi-0.9.3/yapapi/contrib/service/http_proxy.py
+-rw-r--r--   0        0        0       44 2022-10-11 05:55:35.261902 yapapi-0.9.3/yapapi/contrib/strategy/__init__.py
+-rw-r--r--   0        0        0     3157 2022-10-11 05:55:35.261902 yapapi-0.9.3/yapapi/contrib/strategy/provider_filter.py
+-rw-r--r--   0        0        0    13615 2022-10-11 05:55:35.261902 yapapi-0.9.3/yapapi/ctx.py
+-rw-r--r--   0        0        0    39962 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/engine.py
+-rw-r--r--   0        0        0     1077 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/event_dispatcher.py
+-rw-r--r--   0        0        0    15694 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/events.py
+-rw-r--r--   0        0        0    15036 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/executor/__init__.py
+-rw-r--r--   0        0        0     7718 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/executor/_smartq.py
+-rw-r--r--   0        0        0      837 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/executor/ctx.py
+-rw-r--r--   0        0        0      874 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/executor/events.py
+-rw-r--r--   0        0        0     1038 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/executor/strategy.py
+-rw-r--r--   0        0        0     4946 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/executor/task.py
+-rw-r--r--   0        0        0    23319 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/golem.py
+-rw-r--r--   0        0        0    24778 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/log.py
+-rw-r--r--   0        0        0    11030 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/network.py
+-rw-r--r--   0        0        0      405 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/package/__init__.py
+-rw-r--r--   0        0        0     1419 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/package/vm.py
+-rw-r--r--   0        0        0     1386 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/payload/__init__.py
+-rw-r--r--   0        0        0     1149 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/payload/package.py
+-rw-r--r--   0        0        0     6184 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/payload/vm.py
+-rw-r--r--   0        0        0     2400 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/props/__init__.py
+-rw-r--r--   0        0        0    10669 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/props/base.py
+-rw-r--r--   0        0        0     4388 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/props/builder.py
+-rw-r--r--   0        0        0     2793 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/props/com.py
+-rw-r--r--   0        0        0     1886 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/props/inf.py
+-rw-r--r--   0        0        0        0 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/py.typed
+-rw-r--r--   0        0        0      410 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/rest/__init__.py
+-rw-r--r--   0        0        0    13418 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/rest/activity.py
+-rw-r--r--   0        0        0     2955 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/rest/common.py
+-rw-r--r--   0        0        0     6693 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/rest/configuration.py
+-rw-r--r--   0        0        0    10918 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/rest/market.py
+-rw-r--r--   0        0        0     1125 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/rest/net.py
+-rw-r--r--   0        0        0     9454 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/rest/payment.py
+-rw-r--r--   0        0        0      216 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/rest/resource.py
+-rw-r--r--   0        0        0     8490 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/script/__init__.py
+-rw-r--r--   0        0        0     1703 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/script/capture.py
+-rw-r--r--   0        0        0     9966 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/script/command.py
+-rw-r--r--   0        0        0      170 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/services/__init__.py
+-rw-r--r--   0        0        0     8221 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/services/cluster.py
+-rw-r--r--   0        0        0    17456 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/services/service.py
+-rw-r--r--   0        0        0    15902 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/services/service_runner.py
+-rw-r--r--   0        0        0     3029 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/services/service_state.py
+-rw-r--r--   0        0        0     3961 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/storage/__init__.py
+-rw-r--r--   0        0        0    15947 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/storage/gftp.py
+-rw-r--r--   0        0        0     5436 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/storage/webdav.py
+-rw-r--r--   0        0        0      500 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/strategy/__init__.py
+-rw-r--r--   0        0        0     8185 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/strategy/base.py
+-rw-r--r--   0        0        0     2455 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/strategy/decrease_score_unconfirmed.py
+-rw-r--r--   0        0        0     2602 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/strategy/dummy.py
+-rw-r--r--   0        0        0     3342 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/strategy/least_expensive.py
+-rw-r--r--   0        0        0     1583 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/strategy/wrapping_strategy.py
+-rw-r--r--   0        0        0     5548 2022-10-11 05:55:35.265902 yapapi-0.9.3/yapapi/utils.py
+-rw-r--r--   0        0        0     7760 2022-10-11 05:55:48.305899 yapapi-0.9.3/setup.py
+-rw-r--r--   0        0        0     8030 2022-10-11 05:55:48.306646 yapapi-0.9.3/PKG-INFO
```

### Comparing `yapapi-0.9.2/LICENSE` & `yapapi-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/README.md` & `yapapi-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/pyproject.toml` & `yapapi-0.9.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yapapi"
-version = "0.9.2"
+version = "0.9.3"
 description = "High-level Python API for the New Golem"
 authors = ["Przemysław K. Rekucki <przemyslaw.rekucki@golem.network>", "GolemFactory <contact@golem.network>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -40,15 +40,15 @@
 # Adding `goth` to dependencies causes > 40 additional packages to be installed. Given
 # that dependency resolution in `poetry` is rather slow, we'd like to avoid installing
 # `goth` for example in a CI pipeline that only runs linters/unit tests, not integration
 # tests. Therefore we specify `goth` as an "extra" dependency, with `optional = "true"`.
 # It will be then installable with `poetry install -E integration-tests`.
 # Note that putting `goth` in `poetry.dev-dependencies` instead of `poetry.dependencies`
 # would not work: see https://github.com/python-poetry/poetry/issues/129.
-goth = { version = "^0.11", optional = true, python = "^3.8.0" }
+goth = { version = "^0.13", optional = true, python = "^3.8.0" }
 # goth = { git = "https://github.com/golemfactory/goth.git", branch = "master", optional = true, python = "^3.8.0", develop = true }
 Deprecated = "^1.2.12"
 python-statemachine = "^0.8.0"
 
 # goth tests
 pexpect = {version = "^4.8.0", optional = true}
 
@@ -102,15 +102,15 @@
 ya-client-activity = "0.1.0"
 ya-client-payment = "0.1.0"
 ya-market = "0.1.0"
 
 [tool.poe.tasks]
 test = "pytest --cov=yapapi --ignore tests/goth_tests"
 goth-assets = "python -m goth create-assets tests/goth_tests/assets"
-goth-tests = "pytest -svx tests/goth_tests --ssh-verify-connection --reruns 3 --only-rerun AssertionError --only-rerun TimeoutError --only-rerun goth.runner.exceptions.TemporalAssertionError --only-rerun urllib.error.URLError --only-rerun goth.runner.exceptions.CommandError"
+goth-tests = "pytest -svx tests/goth_tests --config-override docker-compose.build-environment.release-tag=pre-rel-v0.12.0-rc2 --config-path tests/goth_tests/assets/goth-config.yml --ssh-verify-connection --reruns 3 --only-rerun AssertionError --only-rerun TimeoutError --only-rerun goth.runner.exceptions.TemporalAssertionError --only-rerun urllib.error.URLError --only-rerun goth.runner.exceptions.CommandError"
 typecheck = "mypy --check-untyped-defs --no-implicit-optional ."
 codestyle = "black --check --diff ."
 _liccheck_export = "poetry export -f requirements.txt -o .requirements.txt"
 _liccheck_verify = "liccheck -r .requirements.txt"
 liccheck = ["_liccheck_export", "_liccheck_verify"]
 check = ["test", "typecheck", "codestyle", "liccheck"]
 clean = "rm -rf .coverage .requirements.txt dist md handbook build"
```

### Comparing `yapapi-0.9.2/yapapi/__init__.py` & `yapapi-0.9.3/yapapi/__init__.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/agreements_pool.py` & `yapapi-0.9.3/yapapi/agreements_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,18 +202,25 @@
             if not await buffered_agreement.agreement.terminate(reason):
                 logger.debug(
                     "Couldn't terminate agreement. id: %s, provider: %s",
                     buffered_agreement.agreement.id,
                     provider,
                 )
 
-        del self._agreements[agreement_id]
-        self.emitter(
-            events.AgreementTerminated, agreement=buffered_agreement.agreement, reason=reason
-        )
+        try:
+            del self._agreements[agreement_id]
+            self.emitter(
+                events.AgreementTerminated, agreement=buffered_agreement.agreement, reason=reason
+            )
+        except KeyError:
+            logger.debug(
+                "Terminated agreement no longer in the pool. id: %s, provider: %s",
+                agreement_id,
+                provider,
+            )
 
     async def terminate_all(self, reason: dict) -> None:
         """Terminate all agreements."""
 
         async with self._lock:
             for agreement_id in frozenset(self._agreements):
                 await self._terminate_agreement(agreement_id, reason)
```

### Comparing `yapapi-0.9.2/yapapi/contrib/__init__.py` & `yapapi-0.9.3/yapapi/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/contrib/service/http_proxy.py` & `yapapi-0.9.3/yapapi/contrib/service/http_proxy.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/contrib/strategy/provider_filter.py` & `yapapi-0.9.3/yapapi/contrib/strategy/provider_filter.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/ctx.py` & `yapapi-0.9.3/yapapi/ctx.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/engine.py` & `yapapi-0.9.3/yapapi/engine.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/event_dispatcher.py` & `yapapi-0.9.3/yapapi/event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/events.py` & `yapapi-0.9.3/yapapi/events.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/executor/__init__.py` & `yapapi-0.9.3/yapapi/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/executor/_smartq.py` & `yapapi-0.9.3/yapapi/executor/_smartq.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/executor/ctx.py` & `yapapi-0.9.3/yapapi/executor/ctx.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/executor/events.py` & `yapapi-0.9.3/yapapi/executor/events.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/executor/strategy.py` & `yapapi-0.9.3/yapapi/executor/strategy.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/executor/task.py` & `yapapi-0.9.3/yapapi/executor/task.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/golem.py` & `yapapi-0.9.3/yapapi/golem.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/log.py` & `yapapi-0.9.3/yapapi/log.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/network.py` & `yapapi-0.9.3/yapapi/network.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/package/vm.py` & `yapapi-0.9.3/yapapi/package/vm.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/payload/__init__.py` & `yapapi-0.9.3/yapapi/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/payload/package.py` & `yapapi-0.9.3/yapapi/payload/package.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/payload/vm.py` & `yapapi-0.9.3/yapapi/payload/vm.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/props/__init__.py` & `yapapi-0.9.3/yapapi/props/__init__.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/props/base.py` & `yapapi-0.9.3/yapapi/props/base.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/props/builder.py` & `yapapi-0.9.3/yapapi/props/builder.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/props/com.py` & `yapapi-0.9.3/yapapi/props/com.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/props/inf.py` & `yapapi-0.9.3/yapapi/props/inf.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/rest/activity.py` & `yapapi-0.9.3/yapapi/rest/activity.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/rest/common.py` & `yapapi-0.9.3/yapapi/rest/common.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/rest/configuration.py` & `yapapi-0.9.3/yapapi/rest/configuration.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/rest/market.py` & `yapapi-0.9.3/yapapi/rest/market.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/rest/net.py` & `yapapi-0.9.3/yapapi/rest/net.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/rest/payment.py` & `yapapi-0.9.3/yapapi/rest/payment.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/script/__init__.py` & `yapapi-0.9.3/yapapi/script/__init__.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/script/capture.py` & `yapapi-0.9.3/yapapi/script/capture.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/script/command.py` & `yapapi-0.9.3/yapapi/script/command.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/services/cluster.py` & `yapapi-0.9.3/yapapi/services/cluster.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/services/service.py` & `yapapi-0.9.3/yapapi/services/service.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/services/service_runner.py` & `yapapi-0.9.3/yapapi/services/service_runner.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/services/service_state.py` & `yapapi-0.9.3/yapapi/services/service_state.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/storage/__init__.py` & `yapapi-0.9.3/yapapi/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/storage/gftp.py` & `yapapi-0.9.3/yapapi/storage/gftp.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/storage/webdav.py` & `yapapi-0.9.3/yapapi/storage/webdav.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/strategy/base.py` & `yapapi-0.9.3/yapapi/strategy/base.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/strategy/decrease_score_unconfirmed.py` & `yapapi-0.9.3/yapapi/strategy/decrease_score_unconfirmed.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/strategy/dummy.py` & `yapapi-0.9.3/yapapi/strategy/dummy.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/strategy/least_expensive.py` & `yapapi-0.9.3/yapapi/strategy/least_expensive.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/strategy/wrapping_strategy.py` & `yapapi-0.9.3/yapapi/strategy/wrapping_strategy.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/yapapi/utils.py` & `yapapi-0.9.3/yapapi/utils.py`

 * *Files identical despite different names*

### Comparing `yapapi-0.9.2/setup.py` & `yapapi-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.8,<0.9'],
  'docs': ['sphinx>=4.0.1,<5.0.0',
           'sphinx-autodoc-typehints>=1.12.0,<2.0.0',
           'sphinx-rtd-theme>=1.0.0,<2.0.0'],
  'integration-tests': ['pexpect>=4.8.0,<5.0.0'],
- 'integration-tests:python_version >= "3.8.0" and python_version < "4.0.0"': ['goth>=0.11,<0.12']}
+ 'integration-tests:python_version >= "3.8.0" and python_version < "4.0.0"': ['goth>=0.13,<0.14']}
 
 setup_kwargs = {
     'name': 'yapapi',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'High-level Python API for the New Golem',
     'long_description': '# Golem Python API\n\n[![Tests - Status](https://img.shields.io/github/workflow/status/golemfactory/yapapi/Continuous%20integration/master?label=tests)](https://github.com/golemfactory/yapapi/actions?query=workflow%3A%22Continuous+integration%22+branch%3Amaster)\n[![Docs status](https://readthedocs.org/projects/yapapi/badge/?version=latest)](https://yapapi.readthedocs.io/en/latest/)\n![PyPI - Status](https://img.shields.io/pypi/status/yapapi)\n[![PyPI version](https://badge.fury.io/py/yapapi.svg)](https://badge.fury.io/py/yapapi)\n[![GitHub license](https://img.shields.io/github/license/golemfactory/yapapi)](https://github.com/golemfactory/yapapi/blob/master/LICENSE)\n[![GitHub issues](https://img.shields.io/github/issues/golemfactory/yapapi)](https://github.com/golemfactory/yapapi/issues)\n\n## What\'s Golem and yapapi?\n\n**[Golem](https://golem.network)** is a global, open-source, decentralized supercomputer that anyone can access.\nIt connects individual machines to form a vast network which combines their resources and allows requestors to utilize its unique potential - which may be its combined computing power, storage, the geographical distribution or its censorship resistance.\n\n**Yapapi** is the Python high-level API that allows developers to connect to their Golem nodes and manage their distributed, computational loads through Golem Network.\n\n## Golem application development\n\nFor a detailed introduction to using Golem and yapapi to run your tasks on Golem and a guide to Golem Network application development in general, [please consult our handbook](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development).\n\n\n### Installation\n\n`yapapi` is available as a [PyPI package](https://pypi.org/project/yapapi/).\n\nYou can install it through `pip`:\n```\npip install yapapi\n```\n\nOr if your project uses [`poetry`](https://python-poetry.org/) you can add it to your dependencies like this:\n```\npoetry add yapapi\n```\n\n### API Reference\n\nFor a comprehensive API reference, please refer to [our official readthedocs page](https://yapapi.readthedocs.io/).\n\n## Local setup for yapapi developers\n\n### Poetry\n`yapapi` uses [`poetry`](https://python-poetry.org/) to manage its dependencies and provide a runner for common tasks.\n\nIf you don\'t have `poetry` available on your system then follow its [installation instructions](https://python-poetry.org/docs/#installation) before proceeding.\nVerify your installation by running:\n```\npoetry --version\n```\n\n### Project dependencies\nTo install the project\'s dependencies run:\n```\npoetry install\n```\nBy default, `poetry` looks for the required Python version on your `PATH` and creates a virtual environment for the project if there\'s none active (or already configured by Poetry).\n\nAll of the project\'s dependencies will be installed to that virtual environment.\n\n### Running `goth` integration tests\n\n#### Prerequisites\n\nIf you\'d like to run the `yapapi` integration test suite locally then you\'ll need to install an additional set of dependencies separately.\n\nFirst, install [the dependencies required to run goth](https://github.com/golemfactory/goth#requirements).\n\nNext, [configure goth\'s GitHub API token](https://github.com/golemfactory/goth#getting-a-github-api-token).\n\nNow, you can install goth and its additional python requirements:\n\n```\npoetry install -E integration-tests\n```\n\nFinally, generate goth\'s default assets:\n\n```\npoetry run poe goth-assets\n```\n\n#### Running the tests\n\nOnce you have the environment set up, to run all the integration tests, use:\n\n```\npoetry run poe goth-tests\n```\n\n## See also\n\n* [Golem](https://golem.network), a global, open-source, decentralized supercomputer that anyone can access.\n* Learn what you need to know to set-up your Golem requestor node:\n    * [Requestor development: a quick primer](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development)\n    * [Run first task on Golem](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development/run-first-task-on-golem)\n* Have a look at the most important concepts behind any Golem application: [Golem application fundamentals](https://handbook.golem.network/requestor-tutorials/golem-application-fundamentals)\n* Learn about preparing your own Docker-like images for the [VM runtime](https://handbook.golem.network/requestor-tutorials/vm-runtime)\n* Write your own app with yapapi:\n    * [Task Model development](https://handbook.golem.network/requestor-tutorials/task-processing-development)\n    * [Service Model development](https://handbook.golem.network/requestor-tutorials/service-development)\n\n## Environment variables\n\nIt\'s possible to set various elements of `yagna` configuration through environment variables.\n`yapapi` currently supports the following environment variables:\n- `YAGNA_ACTIVITY_URL`, URL to `yagna` activity API, e.g. `http://localhost:7500/activity-api/v1`\n- `YAGNA_API_URL`, base URL to `yagna` REST API, e.g. `http://localhost:7500`\n- `YAGNA_APPKEY`, `yagna` app key to be used, e.g. `a70facb9501d4528a77f25574ab0f12b`\n- `YAGNA_MARKET_URL`, URL to `yagna` market API, e.g. `http://localhost:7500/market-api/v1`\n- `YAGNA_PAYMENT_NETWORK`, Ethereum network name for `yagna` to use, e.g. `rinkeby`\n- `YAGNA_PAYMENT_DRIVER`, payment driver name for `yagna` to use, e.g. `erc20`\n- `YAGNA_PAYMENT_URL`, URL to `yagna` payment API, e.g. `http://localhost:7500/payment-api/v1`\n- `YAGNA_SUBNET`, name of the `yagna` sub network to be used, e.g. `devnet-beta`\n- `YAPAPI_USE_GFTP_CLOSE`, if set to a _truthy_ value (e.g. "1", "Y", "True", "on") then `yapapi`\n  will ask `gftp` to close files when there\'s no need to publish them any longer. This may greatly\n  reduce the number of files kept open while `yapapi` is running but requires `yagna`\n  0.7.3 or newer, with older versions it will cause errors.\n',
     'author': 'Przemysław K. Rekucki',
     'author_email': 'przemyslaw.rekucki@golem.network',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/golemfactory/yapapi',
```

### Comparing `yapapi-0.9.2/PKG-INFO` & `yapapi-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapapi
-Version: 0.9.2
+Version: 0.9.3
 Summary: High-level Python API for the New Golem
 Home-page: https://github.com/golemfactory/yapapi
 License: LGPL-3.0-or-later
 Author: Przemysław K. Rekucki
 Author-email: przemyslaw.rekucki@golem.network
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,15 @@
 Requires-Dist: Deprecated (>=1.2.12,<2.0.0)
 Requires-Dist: aiohttp (>=3.6,<4.0)
 Requires-Dist: aiohttp-sse-client (>=0.1.7,<0.2.0)
 Requires-Dist: async_exit_stack (>=1.0.1,<2.0.0)
 Requires-Dist: attrs (>=19.3)
 Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: dataclasses (>=0.8,<0.9); python_version >= "3.6" and python_version < "3.7"
-Requires-Dist: goth (>=0.11,<0.12); (python_version >= "3.8.0" and python_version < "4.0.0") and (extra == "integration-tests")
+Requires-Dist: goth (>=0.13,<0.14); (python_version >= "3.8.0" and python_version < "4.0.0") and (extra == "integration-tests")
 Requires-Dist: jsonrpc-base (>=1.0.3,<2.0.0)
 Requires-Dist: more-itertools (>=8.6.0,<9.0.0)
 Requires-Dist: pexpect (>=4.8.0,<5.0.0); extra == "integration-tests"
 Requires-Dist: python-statemachine (>=0.8.0,<0.9.0)
 Requires-Dist: semantic-version (>=2.8,<3.0)
 Requires-Dist: sphinx (>=4.0.1,<5.0.0); extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints (>=1.12.0,<2.0.0); extra == "docs"
```

