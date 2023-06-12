# Comparing `tmp/lnschema_lamin1-0.18a1.tar.gz` & `tmp/lnschema_lamin1-0.19a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_lamin1-0.18a1.tar", last modified: Thu Jun  1 12:09:46 2023, max compression
+gzip compressed data, was "lnschema_lamin1-0.19a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lnschema_lamin1-0.18a1.tar` & `lnschema_lamin1-0.19a1.tar`

### file list

```diff
@@ -1,33 +1,19 @@
--rw-r--r--   0        0        0     3403 2023-05-29 08:07:10.544417 lnschema_lamin1-0.18a1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.18a1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.18a1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.18a1/.gitignore
--rw-r--r--   0        0        0     1795 2023-04-24 17:49:33.167540 lnschema_lamin1-0.18a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      154 2023-05-25 15:48:48.190697 lnschema_lamin1-0.18a1/README.md
--rw-r--r--   0        0        0     1221 2023-06-01 12:09:29.000748 lnschema_lamin1-0.18a1/docs/changelog.md
--rw-r--r--   0        0        0     5478 2023-05-29 08:15:51.257095 lnschema_lamin1-0.18a1/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0     2190 2023-04-24 17:39:09.199540 lnschema_lamin1-0.18a1/docs/guide/02-orms.ipynb
--rw-r--r--   0        0        0     3402 2023-05-27 08:19:25.110706 lnschema_lamin1-0.18a1/docs/guide/10-migrate.ipynb
--rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.18a1/docs/guide/index.md
--rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.18a1/docs/index.md
--rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.18a1/docs/reference.md
--rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.18a1/lamin-project.yaml
--rw-r--r--   0        0        0      684 2023-06-01 12:09:19.607061 lnschema_lamin1-0.18a1/lnschema_lamin1/__init__.py
--rw-r--r--   0        0        0     5854 2023-06-01 10:57:40.910668 lnschema_lamin1-0.18a1/lnschema_lamin1/_core.py
--rw-r--r--   0        0        0     2902 2023-05-25 21:05:50.420200 lnschema_lamin1-0.18a1/lnschema_lamin1/_link.py
--rw-r--r--   0        0        0      259 2023-05-25 15:48:48.191950 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/__init__.py
--rw-r--r--   0        0        0      346 2023-05-25 15:48:48.192035 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/_type.py
--rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/_versions.py
--rw-r--r--   0        0        0     1021 2023-06-01 10:57:40.910866 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/id.py
--rw-r--r--   0        0        0      156 2023-05-25 15:48:48.192133 lnschema_lamin1-0.18a1/lnschema_lamin1/dev/type.py
--rw-r--r--   0        0        0      426 2023-05-25 15:48:48.192250 lnschema_lamin1-0.18a1/lnschema_lamin1/link.py
--rw-r--r--   0        0        0     1063 2023-04-24 17:49:33.169471 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
--rw-r--r--   0        0        0     4097 2023-05-25 15:48:48.192371 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py
--rw-r--r--   0        0        0     2251 2023-05-25 15:48:48.192464 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py
--rw-r--r--   0        0        0     5149 2023-05-30 05:26:00.254109 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17a.py
--rw-r--r--   0        0        0     8494 2023-05-30 05:26:00.253105 lnschema_lamin1-0.18a1/lnschema_lamin1/migrations/versions/2023-05-30-be880ab5ad00-v0_17b.py
--rw-r--r--   0        0        0      776 2023-04-24 16:11:06.697345 lnschema_lamin1-0.18a1/noxfile.py
--rw-r--r--   0        0        0      722 2023-06-01 12:04:08.676295 lnschema_lamin1-0.18a1/pyproject.toml
--rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.18a1/tests/test_migrations.py
--rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.18a1/tests/test_notebooks.py
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 lnschema_lamin1-0.18a1/PKG-INFO
+-rw-r--r--   0        0        0     1987 2023-06-12 12:45:51.522922 lnschema_lamin1-0.19a1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.19a1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.19a1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.19a1/.gitignore
+-rw-r--r--   0        0        0     1795 2023-06-12 18:05:45.140101 lnschema_lamin1-0.19a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      113 2023-06-12 12:45:51.523274 lnschema_lamin1-0.19a1/README.md
+-rw-r--r--   0        0        0     1681 2023-06-12 18:08:42.044060 lnschema_lamin1-0.19a1/docs/changelog.md
+-rw-r--r--   0        0        0     5251 2023-06-12 12:45:51.541874 lnschema_lamin1-0.19a1/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.19a1/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.19a1/docs/index.md
+-rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.19a1/docs/reference.md
+-rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.19a1/lamin-project.yaml
+-rw-r--r--   0        0        0      512 2023-06-12 18:08:23.348934 lnschema_lamin1-0.19a1/lnschema_lamin1/__init__.py
+-rw-r--r--   0        0        0     9114 2023-06-12 18:06:30.025984 lnschema_lamin1-0.19a1/lnschema_lamin1/migrations/0001_initial.py
+-rw-r--r--   0        0        0     5891 2023-06-12 17:01:32.725441 lnschema_lamin1-0.19a1/lnschema_lamin1/models.py
+-rw-r--r--   0        0        0      509 2023-06-12 12:45:51.561539 lnschema_lamin1-0.19a1/noxfile.py
+-rw-r--r--   0        0        0      721 2023-06-12 17:01:32.725731 lnschema_lamin1-0.19a1/pyproject.toml
+-rw-r--r--   0        0        0      401 2023-06-12 12:45:51.562581 lnschema_lamin1-0.19a1/tests/test_notebooks.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 lnschema_lamin1-0.19a1/PKG-INFO
```

### Comparing `lnschema_lamin1-0.18a1/.github/workflows/build.yml` & `lnschema_lamin1-0.19a1/.github/workflows/build.yml`

 * *Files 21% similar despite different names*

```diff
@@ -25,77 +25,38 @@
       - name: Checkout lndocs
         uses: actions/checkout@v3
         with:
           repository: laminlabs/lndocs
           ssh-key: ${{ secrets.READ_LNDOCS }}
           path: lndocs
           ref: main
-      - name: Setup Python
-        uses: actions/setup-python@v4
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
-          cache-dependency-path: ".github/workflows/build.yml" # See dependencies below
-      - name: Cache nox
-        uses: actions/cache@v3
-        with:
-          path: .nox
-          key: nox-${{ runner.os }}
-      - name: Cache pre-commit
-        uses: actions/cache@v3
+          cache-dependency-path: "pyproject.toml"
+      - uses: actions/cache@v3
         with:
           path: ~/.cache/pre-commit
           key: pre-commit-${{ runner.os }}-${{ hashFiles('.pre-commit-config.yaml') }}
-      - name: Cache postgres
-        id: cache-postgres
-        uses: actions/cache@v3
-        with:
-          path: ~/postgres.tar
-          key: cache-postgres-0
-      - name: Cache postgres miss
-        if: steps.cache-postgres.outputs.cache-hit != 'true'
-        run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
-      - name: Cache postgres use
-        if: steps.cache-postgres.outputs.cache-hit == 'true'
-        run: docker image load --input ~/postgres.tar
-      - name: Install Python dependencies
+      - name: install Python deps
         run: |
           python -m pip install -U pip
-          pip install lamindb>=0.41a5
-      - name: Install apt-get dependencies
-        run: |
-          sudo apt-get -y install graphviz
-          sudo apt-get install sqlite3-tools=3.37.2-2
-          sudo apt-get install libpq-dev
-      - name: Lint
-        run: |
-          nox -s lint
-      - name: Configure AWS
-        uses: aws-actions/configure-aws-credentials@v1
+          pip install -U laminci
+      - uses: aws-actions/configure-aws-credentials@v2
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
-      - name: Build
-        run: |
-          nox -s build --python ${{ matrix.python-version }}
-        env:
-          GITHUB_EVENT_NAME: ${{ github.event_name }}
-      - name: Codecov
-        if: matrix.python-version == '3.9'
-        uses: codecov/codecov-action@v2
-        with:
-          token: ${{ secrets.CODECOV_TOKEN }}
-      - name: Read lamin-project.yaml
-        if: matrix.python-version == '3.9'
-        id: lamin-project
-        uses: CumulusDS/get-yaml-paths-action@v0.1.0
-        with:
-          file: lamin-project.yaml
-          project_slug: project_slug
+      - name: install graphviz
+        run: sudo apt-get -y install graphviz
+      # - run: nox -s lint
+      - run: nox -s install
+      - run: nox -s test
+      - run: nox -s docs
       - name: Deploy docs
         if: matrix.python-version == '3.9'
         id: netlify
         uses: nwtgck/actions-netlify@v1.2
         with:
           publish-dir: "_build/html"
           production-deploy: ${{ github.event_name == 'push' }}
```

### Comparing `lnschema_lamin1-0.18a1/.github/workflows/latest-changes.yml` & `lnschema_lamin1-0.19a1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.18a1/.gitignore` & `lnschema_lamin1-0.19a1/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.18a1/.pre-commit-config.yaml` & `lnschema_lamin1-0.19a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.18a1/docs/changelog.md` & `lnschema_lamin1-0.19a1/docs/changelog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Prettify | [13](https://github.com/laminlabs/lnschema-lamin1/pull/13) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.19a1
+🚚 Finish first proper draft of migration | [12](https://github.com/laminlabs/lnschema-lamin1/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-06-11 |
+🚧 Partial migration to Django | [11](https://github.com/laminlabs/lnschema-lamin1/pull/11) | [falexwolf](https://github.com/falexwolf) | 2023-06-09 |
 ➖ Remove lnbase-biolab | [10](https://github.com/laminlabs/lnschema-lamin1/pull/10) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.18a1
 🏗️ Remove SQL-level schema modules | [9](https://github.com/laminlabs/lnschema-lamin1/pull/9) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.17.0
 🎨 Add `Well` table, File.cell_lines | [8](https://github.com/laminlabs/lnschema-lamin1/pull/8) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-23 | 0.16.3
 💚 Removed treatment relationships | [4](https://github.com/laminlabs/lnschema-lamin1/pull/4) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 | 0.16.2
 ✨ Added `Treatment` table | [3](https://github.com/laminlabs/lnschema-lamin1/pull/3) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 |
 🚚 Link `CellType` to `File` | [2](https://github.com/laminlabs/lnschema-lamin1/pull/2) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.16.1
 🎉 Move content from `lnschema-wetlab` here | [1](https://github.com/laminlabs/lnschema-lamin1/pull/1) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.15.1
```

### Comparing `lnschema_lamin1-0.18a1/docs/guide/01-get-started.ipynb` & `lnschema_lamin1-0.19a1/docs/guide/01-get-started.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9925170068027211%*

 * *Differences: {"'cells'": "{8: {'source': ['### Company-wide production instance: Postgres + Cloud bucket']}, 9: "*

 * *            '{\'source\': {insert: [(4, \'ln.setup.init(storage="s3://ln-lamin1-pg-std", '*

 * *            'schema="lamin1,bionty", '*

 * *            'db="postgresql://batman:robin@35.222.187.204:5432/lamin1")\\n\')], delete: [4]}}, 10: '*

 * *            '{\'source\': {insert: [(4, \'ln.setup.load("testuser1/lamin1")  # CLI: lamin load '*

 * *            "testuser1/lamin1\\n')], delete: [4]}}, 12: {'source': ['### Test insta […]*

```diff
@@ -85,55 +85,42 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "43b3d4dd-051c-4982-929f-445c6cec2d3e",
             "metadata": {},
             "source": [
-                "### Company-wide production instance: Postgres + GCP bucket"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "a45f84b1",
-            "metadata": {},
-            "source": [
-                "```{note}\n",
-                "\n",
-                "All of the following calls can also be done using the CLI, e.g., `lamin init --storage ...`\n",
-                "\n",
-                "```"
+                "### Company-wide production instance: Postgres + Cloud bucket"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "bf2b0199-d119-42ac-ac27-6e99deb8b8ca",
             "metadata": {},
             "source": [
                 "To set up a test instance with Google Cloud storage and postgres by an admin (here `testuser1`):\n",
                 "\n",
                 "```{code}\n",
                 "\n",
-                "ln.setup.init(storage=\"gs://ln-lamin1-pg-std\", schema=\"lamin1,bionty\", db=\"postgresql://batman:robin@35.222.187.204:5432/lamin1\")\n",
+                "ln.setup.init(storage=\"s3://ln-lamin1-pg-std\", schema=\"lamin1,bionty\", db=\"postgresql://batman:robin@35.222.187.204:5432/lamin1\")\n",
                 "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "188096d8",
             "metadata": {},
             "source": [
                 "Other users can simply run:\n",
                 "\n",
                 "```{code}\n",
                 "\n",
-                "ln.setup.load(\"testuser1/lamin1\")\n",
+                "ln.setup.load(\"testuser1/lamin1\")  # CLI: lamin load testuser1/lamin1\n",
                 "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "4a4c43b1-55d8-465c-9eaa-4aeed603d265",
@@ -149,15 +136,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "5b22cceb-0456-4f68-bd47-1fa909b1f2f2",
             "metadata": {},
             "source": [
-                "### Mini-instance: SQLite + GCP bucket"
+                "### Test instances: SQLite on cloud bucket"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "49d4a2e1-7ee2-48ce-b4ac-6855920bb19b",
             "metadata": {},
```

### Comparing `lnschema_lamin1-0.18a1/pyproject.toml` & `lnschema_lamin1-0.19a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     "lnschema_bionty",  # do not pin lamindb, lamindb pins lnschema_lamin1!
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lnschema-lamin1"
 
 [project.optional-dependencies]
-test = [
-    "lamindb[bionty]==0.41.2",
+dev = [
+    "lamindb[bionty]==0.42a9",
     "pre-commit",
     "nox",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject_test>=0.4.1",
 ]
```

### Comparing `lnschema_lamin1-0.18a1/PKG-INFO` & `lnschema_lamin1-0.19a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lnschema_lamin1
-Version: 0.18a1
-Summary: Lamin's `lamin1` lab schema (`tvhn`).
+Version: 0.19a1
+Summary: Lamin's `lamin1` exemplary lab schema.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_bionty
-Requires-Dist: lamindb[bionty]==0.41.2 ; extra == "test"
-Requires-Dist: pre-commit ; extra == "test"
-Requires-Dist: nox ; extra == "test"
-Requires-Dist: pytest>=6.0 ; extra == "test"
-Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: nbproject_test>=0.4.1 ; extra == "test"
+Requires-Dist: lamindb[bionty]==0.42a9 ; extra == "dev"
+Requires-Dist: pre-commit ; extra == "dev"
+Requires-Dist: nox ; extra == "dev"
+Requires-Dist: pytest>=6.0 ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: nbproject_test>=0.4.1 ; extra == "dev"
 Project-URL: Home, https://github.com/laminlabs/lnschema-lamin1
-Provides-Extra: test
+Provides-Extra: dev
 
-# lnschema-lamin1: Customized schema of Lamin (`tvhn`)
+# `lnschema_lamin1`: Examplary lab schema
 
-Latest developer docs: [netlify](https://lnschema-lamin1-tvhn.netlify.app/docs/lnschema-lamin1/).
+Latest dev docs: [netlify](https://lnschema-lamin1-tvhn.netlify.app).
```

