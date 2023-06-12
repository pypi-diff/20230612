# Comparing `tmp/autofit-2023.7.7.1.tar.gz` & `tmp/autofit-2023.7.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofit-2023.7.7.1.tar", last modified: Wed Jun  7 09:42:59 2023, max compression
+gzip compressed data, was "autofit-2023.7.7.2.tar", last modified: Wed Jun  7 09:58:30 2023, max compression
```

## Comparing `autofit-2023.7.7.1.tar` & `autofit-2023.7.7.2.tar`

### file list

```diff
@@ -1,388 +1,388 @@
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.841664 autofit-2023.7.7.1/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:58.992246 autofit-2023.7.7.1/.github/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.048964 autofit-2023.7.7.1/.github/workflows/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2821 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/.github/workflows/main.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/CITATIONS.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18817 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2454 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/CONTRIBUTING.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1091 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      379 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/MANIFEST.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9143 2023-06-07 09:42:59.841664 autofit-2023.7.7.1/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8348 2023-05-10 13:41:29.000000 autofit-2023.7.7.1/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.059876 autofit-2023.7.7.1/autofit/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5232 2023-06-07 09:38:14.000000 autofit-2023.7.7.1/autofit/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.067824 autofit-2023.7.7.1/autofit/aggregator/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      106 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/aggregator/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8944 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/aggregator/aggregator.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9866 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/aggregator/predicate.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4275 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/aggregator/search_output.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       27 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/conf.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.077823 autofit-2023.7.7.1/autofit/config/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/config/.gitignore
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2023-05-09 16:10:42.000000 autofit-2023.7.7.1/autofit/config/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2870 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/config/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      306 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/logging.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.089820 autofit-2023.7.7.1/autofit/config/non_linear/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/non_linear/GridSearch.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      439 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/non_linear/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5905 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/non_linear/mcmc.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6765 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/non_linear/nest.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8407 2023-03-27 14:43:03.000000 autofit-2023.7.7.1/autofit/config/non_linear/optimize.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1252 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/notation.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.112582 autofit-2023.7.7.1/autofit/config/priors/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      511 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/Exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/Gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      796 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/GaussianKurtosis.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/MultiLevelGaussians.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1706 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/model.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      123 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/prior.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/profiles.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1187 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/template.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.119581 autofit-2023.7.7.1/autofit/config/visualize/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      301 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/visualize/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/visualize/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1849 2023-03-27 14:43:03.000000 autofit-2023.7.7.1/autofit/config/visualize/plots_search.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.124017 autofit-2023.7.7.1/autofit/database/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.130954 autofit-2023.7.7.1/autofit/database/aggregator/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/database/aggregator/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15442 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/aggregator/aggregator.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6939 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/aggregator/scrape.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.141104 autofit-2023.7.7.1/autofit/database/migration/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       82 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/database/migration/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6131 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/migration/migration.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2485 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/migration/session_wrapper.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      450 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/migration/steps.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.152914 autofit-2023.7.7.1/autofit/database/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       85 2021-02-10 16:12:06.000000 autofit-2023.7.7.1/autofit/database/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8445 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/model/fit.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3125 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/model/instance.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6319 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/model/model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2853 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/model/prior.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.159919 autofit-2023.7.7.1/autofit/database/query/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      468 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6449 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/query/condition.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4888 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/junction.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.174281 autofit-2023.7.7.1/autofit/database/query/query/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      129 2021-07-01 15:18:16.000000 autofit-2023.7.7.1/autofit/database/query/query/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1643 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/query/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3012 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/query/query/attribute.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1199 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/query/info.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8878 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/query/named.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1086 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/sqlalchemy_.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.182851 autofit-2023.7.7.1/autofit/example/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      126 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/example/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6895 2023-06-05 10:53:40.000000 autofit-2023.7.7.1/autofit/example/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5889 2023-05-10 13:41:29.000000 autofit-2023.7.7.1/autofit/example/model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1746 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/example/util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1647 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/exc.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      845 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/fixtures.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.189851 autofit-2023.7.7.1/autofit/graphical/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.201945 autofit-2023.7.7.1/autofit/graphical/declarative/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        1 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/declarative/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8648 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3186 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/collection.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.215895 autofit-2023.7.7.1/autofit/graphical/declarative/factor/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2554 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4025 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6630 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/hierarchical.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1920 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/prior.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8192 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/graph.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4964 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/result.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.233904 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      213 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17242 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/ep_mean_field.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2068 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/factor_optimiser.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9719 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/history.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17494 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/optimiser.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4417 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/stochastic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1621 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/visualise.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.249913 autofit-2023.7.7.1/autofit/graphical/factor_graphs/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      274 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14727 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16298 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/factor.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16109 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/graph.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4870 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/jacobians.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6392 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/transform.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.259665 autofit-2023.7.7.1/autofit/graphical/laplace/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      155 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/laplace/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10747 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/laplace/line_search.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12004 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/laplace/newton.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6087 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/laplace/optimiser.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18909 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/mean_field.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16822 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/utils.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6343 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/interpolator.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.277189 autofit-2023.7.7.1/autofit/mapper/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      124 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4849 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/identifier.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.281189 autofit-2023.7.7.1/autofit/mapper/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4507 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/mock/mock_model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13695 2023-06-03 08:34:09.000000 autofit-2023.7.7.1/autofit/mapper/model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2656 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/model_mapper.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5691 2023-06-03 08:34:09.000000 autofit-2023.7.7.1/autofit/mapper/model_object.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23069 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/operator.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.304591 autofit-2023.7.7.1/autofit/mapper/prior/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      154 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/prior/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7904 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/abstract.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.315604 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       40 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6412 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/arithmetic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2661 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/assertion.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7211 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/compound.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2066 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/mapper/prior/deferred.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3214 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3124 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/log_gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4258 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/log_uniform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4523 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/tuple_prior.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3275 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/uniform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2654 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/prior/width_modifier.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.335469 autofit-2023.7.7.1/autofit/mapper/prior_model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    63100 2023-06-03 08:34:09.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      666 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/annotation.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/attribute_pair.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8290 2023-05-10 13:42:01.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/collection.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13987 2023-05-10 13:42:01.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/prior_model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2787 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/recursion.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17043 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/variable.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19865 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/variable_operator.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.357353 autofit-2023.7.7.1/autofit/messages/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14433 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4679 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/beta.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9477 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/composed_transform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2568 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/fixed.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/gamma.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7813 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/messages/interface.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8896 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/normal.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11028 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/transform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/messages/utils.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1775 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mock.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.370727 autofit-2023.7.7.1/autofit/non_linear/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/non_linear/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36116 2023-06-05 20:26:47.000000 autofit-2023.7.7.1/autofit/non_linear/abstract_search.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.388446 autofit-2023.7.7.1/autofit/non_linear/analysis/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      120 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5735 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12394 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/combined.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3827 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/free_parameter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4103 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/indexed.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1901 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/model_analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4550 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/multiprocessing.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.396357 autofit-2023.7.7.1/autofit/non_linear/grid/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/non_linear/grid/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.407213 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13550 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1750 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/job.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7283 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2556 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/result_builder.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15909 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/sensitivity.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1728 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/simple_grid.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11223 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/initializer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.415889 autofit-2023.7.7.1/autofit/non_linear/mcmc/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1650 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/abstract_mcmc.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5401 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/auto_correlations.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.426889 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9990 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/emcee.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1105 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4770 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/samples.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.438889 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1140 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4765 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11570 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/zeus.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.452533 autofit-2023.7.7.1/autofit/non_linear/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      761 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mock/mock_analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1319 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mock/mock_result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3584 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mock/mock_samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5717 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mock/mock_search.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.457532 autofit-2023.7.7.1/autofit/non_linear/nest/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/non_linear/nest/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4048 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/abstract_nest.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.475536 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      144 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15669 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6070 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/dynamic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3701 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4272 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6353 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/static.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.487098 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1756 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3042 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11292 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/ultranest.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.492109 autofit-2023.7.7.1/autofit/non_linear/optimize/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1055 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/abstract_optimize.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.500107 autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7760 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/drawer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      102 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/plotter.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.509088 autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6894 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/lbfgs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2799 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/samples.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.526148 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9683 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3455 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/globe.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3460 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/local.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1892 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2894 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/samples.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.533670 autofit-2023.7.7.1/autofit/non_linear/parallel/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      167 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/parallel/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5220 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/parallel/process.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9687 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/parallel/sneaky.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.548604 autofit-2023.7.7.1/autofit/non_linear/paths/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       74 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/paths/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12102 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/paths/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5834 2023-05-10 13:42:01.000000 autofit-2023.7.7.1/autofit/non_linear/paths/database.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11042 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/paths/directory.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1582 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/paths/null.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3621 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/paths/sub_directory_paths.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8898 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/result.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.566829 autofit-2023.7.7.1/autofit/non_linear/samples/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/samples/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9194 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/mcmc.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6968 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/nest.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17430 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/pdf.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8118 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/sample.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21413 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1028 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/stored.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2726 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/settings.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2356 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/timer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.573608 autofit-2023.7.7.1/autofit/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      436 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3998 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/plot/output.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4330 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/plot/samples_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.582545 autofit-2023.7.7.1/autofit/text/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       50 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/text/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6261 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/text/formatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2873 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/text/samples_text.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4039 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/text/text_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.593388 autofit-2023.7.7.1/autofit/tools/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/tools/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      766 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/tools/add_notebook_quotes.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      438 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/tools/namer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6651 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/tools/update_identifiers.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3670 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/tools/util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.840108 autofit-2023.7.7.1/autofit.egg-info/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11169 2023-06-07 09:42:58.000000 autofit-2023.7.7.1/autofit.egg-info/SOURCES.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       40 2023-06-05 10:53:40.000000 autofit-2023.7.7.1/build_requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.603329 autofit-2023.7.7.1/docs/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/docs/Makefile
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.607250 autofit-2023.7.7.1/docs/_templates/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/_templates/custom-class-template.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/_templates/custom_module_template.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.625162 autofit-2023.7.7.1/docs/api/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      967 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/analysis.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      944 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/database.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1281 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/model.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      846 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/plot.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1201 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/priors.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1145 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/samples.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2659 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/searches.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      649 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3755 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/docs/conf.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.636170 autofit-2023.7.7.1/docs/cookbooks/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8234 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_1_basics.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11816 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_2_collections.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11221 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_3_multiple_datasets.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10571 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_4_multi_level.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11943 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_5_model_linking.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.647167 autofit-2023.7.7.1/docs/features/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6471 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/features/database.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8209 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/features/graphical.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.688758 autofit-2023.7.7.1/docs/features/images/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    53610 2021-01-26 21:44:53.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_1__low_snr.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38449 2021-01-26 21:44:53.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_2__low_snr.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37485 2021-01-26 21:44:53.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_3__low_snr.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33505 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44404 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature_fit_feature.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43221 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature_fit_no_feature.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46794 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25965 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_left.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38024 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_left_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    47517 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_right_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33623 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_split.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23811 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/sensitivity_data_high.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28902 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/sensitivity_data_high_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34204 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/sensitivity_data_low.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40377 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/sensitivity_data_low_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9083 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/features/search_chaining.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5844 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/features/search_grid_search.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12076 2023-06-05 10:53:40.000000 autofit-2023.7.7.1/docs/features/sensitivity_mapping.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.705765 autofit-2023.7.7.1/docs/general/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10257 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/adding_a_model_component.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/citations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1017 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/configs.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2021-01-28 19:37:07.000000 autofit-2023.7.7.1/docs/general/credits.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1097 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/roadmap.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      494 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/docs/general/software.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2300 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/workspace.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.715423 autofit-2023.7.7.1/docs/howtofit/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2033 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/howtofit/chapter_1_introduction.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1614 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/howtofit/chapter_database.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2198 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/howtofit/chapter_graphical_models.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5493 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/howtofit/howtofit.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.723051 autofit-2023.7.7.1/docs/images/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69268 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/images/cornerplot.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/docs/images/toy_model_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    57271 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/docs/images/toy_model_fit_x2.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9989 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/index.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.736045 autofit-2023.7.7.1/docs/installation/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1409 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/installation/conda.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1543 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/installation/overview.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1156 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/installation/pip.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1439 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/installation/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1446 2021-01-26 22:07:31.000000 autofit-2023.7.7.1/docs/installation/troubleshooting.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/docs/make.bat
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.748639 autofit-2023.7.7.1/docs/overview/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.763170 autofit-2023.7.7.1/docs/overview/image/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1010915 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/image/cluster_example.jpg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  2030601 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/image/lens_model.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  3051390 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/image/lens_model_cluster.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13863 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/model_complex.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10198 2023-05-09 16:10:42.000000 autofit-2023.7.7.1/docs/overview/model_fit.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12585 2023-03-27 14:43:03.000000 autofit-2023.7.7.1/docs/overview/multi_datasets.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6800 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/non_linear_search.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11895 2023-06-05 10:53:40.000000 autofit-2023.7.7.1/docs/overview/result.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      344 2023-05-10 13:41:29.000000 autofit-2023.7.7.1/docs/requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.771730 autofit-2023.7.7.1/docs/science_examples/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13077 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/science_examples/astronomy.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      139 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/eden.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.790293 autofit-2023.7.7.1/files/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1339 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/files/citation.tex
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13632 2023-02-21 14:10:09.000000 autofit-2023.7.7.1/files/citations.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1171 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/files/citations.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       31 2021-06-17 13:08:20.000000 autofit-2023.7.7.1/files/eden.ini
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27322 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/files/gaussian_example.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      544 2021-02-11 23:21:00.000000 autofit-2023.7.7.1/files/release.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1226 2021-06-17 13:08:20.000000 autofit-2023.7.7.1/files/to_do_list
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/files/toy_model_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       74 2023-06-01 08:52:02.000000 autofit-2023.7.7.1/optional_requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.798829 autofit-2023.7.7.1/paper/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2020-11-16 19:40:52.000000 autofit-2023.7.7.1/paper/README.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12475 2023-02-21 14:10:09.000000 autofit-2023.7.7.1/paper/paper.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2021-12-09 20:28:25.000000 autofit-2023.7.7.1/paper/paper.json
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11881 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/paper/paper.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      175 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/readthedocs.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      240 2023-05-10 13:41:29.000000 autofit-2023.7.7.1/requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.818429 autofit-2023.7.7.1/scripts/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-02-24 17:53:38.000000 autofit-2023.7.7.1/scripts/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      454 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/scripts/add_notebook_quotes.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      268 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/scripts/aggregate.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/scripts/example_map.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      833 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/scripts/update_identifiers.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      910 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/scripts/update_identifiers_from_file.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       63 2023-06-07 09:42:59.843660 autofit-2023.7.7.1/setup.cfg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1917 2023-06-07 09:42:35.000000 autofit-2023.7.7.1/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2081 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/to_do_list
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:30.032927 autofit-2023.7.7.2/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.407571 autofit-2023.7.7.2/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.456549 autofit-2023.7.7.2/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2821 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18817 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2454 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1091 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      379 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9143 2023-06-07 09:58:30.032927 autofit-2023.7.7.2/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8348 2023-05-10 13:41:29.000000 autofit-2023.7.7.2/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.464593 autofit-2023.7.7.2/autofit/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5232 2023-06-07 09:57:30.000000 autofit-2023.7.7.2/autofit/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.471590 autofit-2023.7.7.2/autofit/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      106 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/autofit/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8944 2023-05-15 17:36:10.000000 autofit-2023.7.7.2/autofit/aggregator/aggregator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9866 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/aggregator/predicate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4275 2023-05-15 17:36:10.000000 autofit-2023.7.7.2/autofit/aggregator/search_output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       27 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.479589 autofit-2023.7.7.2/autofit/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/autofit/config/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2023-05-09 16:10:42.000000 autofit-2023.7.7.2/autofit/config/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2870 2023-05-15 17:36:10.000000 autofit-2023.7.7.2/autofit/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      306 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/logging.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.489564 autofit-2023.7.7.2/autofit/config/non_linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/non_linear/GridSearch.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      439 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/non_linear/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5905 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/non_linear/mcmc.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6765 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/non_linear/nest.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8407 2023-03-27 14:43:03.000000 autofit-2023.7.7.2/autofit/config/non_linear/optimize.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1252 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/notation.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.507496 autofit-2023.7.7.2/autofit/config/priors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      511 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/priors/Exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/priors/Gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      796 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/priors/GaussianKurtosis.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/priors/MultiLevelGaussians.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1706 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/priors/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/priors/model.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      123 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/priors/prior.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/priors/profiles.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1187 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/priors/template.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.513538 autofit-2023.7.7.2/autofit/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      301 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/visualize/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/config/visualize/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1849 2023-03-27 14:43:03.000000 autofit-2023.7.7.2/autofit/config/visualize/plots_search.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.516526 autofit-2023.7.7.2/autofit/database/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.522527 autofit-2023.7.7.2/autofit/database/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/database/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15442 2023-05-15 17:36:10.000000 autofit-2023.7.7.2/autofit/database/aggregator/aggregator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6939 2023-05-15 17:36:10.000000 autofit-2023.7.7.2/autofit/database/aggregator/scrape.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.529531 autofit-2023.7.7.2/autofit/database/migration/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       82 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/database/migration/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6131 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/migration/migration.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2485 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/migration/session_wrapper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      450 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/migration/steps.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.539185 autofit-2023.7.7.2/autofit/database/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       85 2021-02-10 16:12:06.000000 autofit-2023.7.7.2/autofit/database/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8445 2023-05-15 17:36:10.000000 autofit-2023.7.7.2/autofit/database/model/fit.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3125 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/model/instance.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6319 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/model/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2853 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/model/prior.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.545227 autofit-2023.7.7.2/autofit/database/query/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      468 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/query/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6449 2023-05-15 17:36:10.000000 autofit-2023.7.7.2/autofit/database/query/condition.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4888 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/query/junction.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.556013 autofit-2023.7.7.2/autofit/database/query/query/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      129 2021-07-01 15:18:16.000000 autofit-2023.7.7.2/autofit/database/query/query/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1643 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/query/query/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3012 2023-05-15 17:36:10.000000 autofit-2023.7.7.2/autofit/database/query/query/attribute.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1199 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/query/query/info.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8878 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/query/query/named.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1086 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/database/sqlalchemy_.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.563270 autofit-2023.7.7.2/autofit/example/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      126 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/example/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6895 2023-06-05 10:53:40.000000 autofit-2023.7.7.2/autofit/example/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5889 2023-05-10 13:41:29.000000 autofit-2023.7.7.2/autofit/example/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1746 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/example/util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1647 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/exc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      845 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.568206 autofit-2023.7.7.2/autofit/graphical/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/graphical/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.577263 autofit-2023.7.7.2/autofit/graphical/declarative/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        1 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/graphical/declarative/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8648 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/declarative/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3186 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/declarative/collection.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.587200 autofit-2023.7.7.2/autofit/graphical/declarative/factor/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/graphical/declarative/factor/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2554 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/declarative/factor/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4025 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/declarative/factor/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6630 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/declarative/factor/hierarchical.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1920 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/graphical/declarative/factor/prior.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8192 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/declarative/graph.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4964 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/declarative/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.601233 autofit-2023.7.7.2/autofit/graphical/expectation_propagation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      213 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/graphical/expectation_propagation/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17242 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/expectation_propagation/ep_mean_field.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2068 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/expectation_propagation/factor_optimiser.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9719 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/expectation_propagation/history.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17494 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/expectation_propagation/optimiser.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4417 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/expectation_propagation/stochastic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1621 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/graphical/expectation_propagation/visualise.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.612048 autofit-2023.7.7.2/autofit/graphical/factor_graphs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      274 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/graphical/factor_graphs/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14727 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/factor_graphs/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16298 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/factor_graphs/factor.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16109 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/factor_graphs/graph.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4870 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/factor_graphs/jacobians.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6392 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/factor_graphs/transform.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.619928 autofit-2023.7.7.2/autofit/graphical/laplace/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      155 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/graphical/laplace/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10747 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/laplace/line_search.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12004 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/laplace/newton.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6087 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/laplace/optimiser.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18909 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/mean_field.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16822 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/graphical/utils.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6343 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/interpolator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.632974 autofit-2023.7.7.2/autofit/mapper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      124 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/mapper/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4849 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/mapper/identifier.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.636905 autofit-2023.7.7.2/autofit/mapper/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/mapper/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4507 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/mock/mock_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13695 2023-06-03 08:34:09.000000 autofit-2023.7.7.2/autofit/mapper/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2656 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/mapper/model_mapper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5691 2023-06-03 08:34:09.000000 autofit-2023.7.7.2/autofit/mapper/model_object.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23069 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/operator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.653252 autofit-2023.7.7.2/autofit/mapper/prior/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      154 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/mapper/prior/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7904 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/prior/abstract.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.662167 autofit-2023.7.7.2/autofit/mapper/prior/arithmetic/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       40 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/mapper/prior/arithmetic/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6412 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/prior/arithmetic/arithmetic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2661 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/prior/arithmetic/assertion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7211 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/prior/arithmetic/compound.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2066 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/autofit/mapper/prior/deferred.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3214 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/prior/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3124 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/prior/log_gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4258 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/prior/log_uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4523 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/prior/tuple_prior.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3275 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/prior/uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2654 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/mapper/prior/width_modifier.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.678081 autofit-2023.7.7.2/autofit/mapper/prior_model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/autofit/mapper/prior_model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    63100 2023-06-03 08:34:09.000000 autofit-2023.7.7.2/autofit/mapper/prior_model/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      666 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/mapper/prior_model/annotation.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/autofit/mapper/prior_model/attribute_pair.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8290 2023-05-10 13:42:01.000000 autofit-2023.7.7.2/autofit/mapper/prior_model/collection.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13987 2023-05-10 13:42:01.000000 autofit-2023.7.7.2/autofit/mapper/prior_model/prior_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2787 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/autofit/mapper/prior_model/recursion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/autofit/mapper/prior_model/util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17043 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/variable.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19865 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mapper/variable_operator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.694285 autofit-2023.7.7.2/autofit/messages/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/messages/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14433 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/messages/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4679 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/messages/beta.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9477 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/messages/composed_transform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2568 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/messages/fixed.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/messages/gamma.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7813 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/messages/interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8896 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/messages/normal.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11028 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/messages/transform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/messages/utils.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1775 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.705534 autofit-2023.7.7.2/autofit/non_linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/autofit/non_linear/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36116 2023-06-05 20:26:47.000000 autofit-2023.7.7.2/autofit/non_linear/abstract_search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.718530 autofit-2023.7.7.2/autofit/non_linear/analysis/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      120 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/analysis/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5735 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/analysis/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12394 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/analysis/combined.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3827 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/analysis/free_parameter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4103 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/analysis/indexed.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1901 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/analysis/model_analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4550 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/analysis/multiprocessing.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.725576 autofit-2023.7.7.2/autofit/non_linear/grid/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/autofit/non_linear/grid/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.734584 autofit-2023.7.7.2/autofit/non_linear/grid/grid_search/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13550 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/grid/grid_search/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1750 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/grid/grid_search/job.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7283 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/grid/grid_search/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2556 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/grid/grid_search/result_builder.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15909 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/grid/sensitivity.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1728 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/grid/simple_grid.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11223 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/initializer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.741577 autofit-2023.7.7.2/autofit/non_linear/mcmc/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1650 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/abstract_mcmc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5401 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/auto_correlations.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.750576 autofit-2023.7.7.2/autofit/non_linear/mcmc/emcee/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/emcee/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9990 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/emcee/emcee.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1105 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/emcee/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4770 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/emcee/samples.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.759622 autofit-2023.7.7.2/autofit/non_linear/mcmc/zeus/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/zeus/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1140 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/zeus/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4765 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/zeus/samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11570 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mcmc/zeus/zeus.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.770579 autofit-2023.7.7.2/autofit/non_linear/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      761 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mock/mock_analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1319 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mock/mock_result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3584 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mock/mock_samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5717 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/mock/mock_search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.774653 autofit-2023.7.7.2/autofit/non_linear/nest/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/autofit/non_linear/nest/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4048 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/nest/abstract_nest.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.787718 autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      144 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15669 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6070 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/dynamic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3701 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4272 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6353 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/static.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.795686 autofit-2023.7.7.2/autofit/non_linear/nest/ultranest/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/nest/ultranest/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1756 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/nest/ultranest/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3042 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/nest/ultranest/samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11292 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/nest/ultranest/ultranest.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.799688 autofit-2023.7.7.2/autofit/non_linear/optimize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1055 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/abstract_optimize.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.806688 autofit-2023.7.7.2/autofit/non_linear/optimize/drawer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/drawer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7760 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/drawer/drawer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      102 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/drawer/plotter.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.813214 autofit-2023.7.7.2/autofit/non_linear/optimize/lbfgs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/lbfgs/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6894 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/lbfgs/lbfgs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2799 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/lbfgs/samples.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.826138 autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9683 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3455 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/globe.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3460 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/local.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1892 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2894 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/samples.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.831821 autofit-2023.7.7.2/autofit/non_linear/parallel/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      167 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/parallel/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5220 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/parallel/process.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9687 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/parallel/sneaky.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.843823 autofit-2023.7.7.2/autofit/non_linear/paths/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       74 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/paths/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12102 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/paths/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5834 2023-05-10 13:42:01.000000 autofit-2023.7.7.2/autofit/non_linear/paths/database.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11042 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/paths/directory.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1582 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/paths/null.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3621 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/paths/sub_directory_paths.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8898 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.857651 autofit-2023.7.7.2/autofit/non_linear/samples/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/non_linear/samples/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9194 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/samples/mcmc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6968 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/samples/nest.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17430 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/samples/pdf.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8118 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/samples/sample.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21413 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/samples/samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1028 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/samples/stored.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2726 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2356 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/non_linear/timer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.862686 autofit-2023.7.7.2/autofit/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      436 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3998 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/plot/output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4330 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/plot/samples_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.869653 autofit-2023.7.7.2/autofit/text/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       50 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/autofit/text/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6261 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/text/formatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2873 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/text/samples_text.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4039 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/text/text_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.877653 autofit-2023.7.7.2/autofit/tools/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/autofit/tools/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      766 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/tools/add_notebook_quotes.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      438 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/autofit/tools/namer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6651 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/tools/update_identifiers.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3670 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/autofit/tools/util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:30.031892 autofit-2023.7.7.2/autofit.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11169 2023-06-07 09:58:29.000000 autofit-2023.7.7.2/autofit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       40 2023-06-05 10:53:40.000000 autofit-2023.7.7.2/build_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.884694 autofit-2023.7.7.2/docs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/docs/Makefile
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.887562 autofit-2023.7.7.2/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.900549 autofit-2023.7.7.2/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      967 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/api/analysis.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      944 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/api/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1281 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/api/model.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      846 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1201 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/api/priors.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1145 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/api/samples.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2659 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/api/searches.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      649 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/api/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3755 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.908542 autofit-2023.7.7.2/docs/cookbooks/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8234 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/cookbooks/cookbook_1_basics.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11816 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/cookbooks/cookbook_2_collections.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11221 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/cookbooks/cookbook_3_multiple_datasets.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10571 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/cookbooks/cookbook_4_multi_level.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11943 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/cookbooks/cookbook_5_model_linking.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.917655 autofit-2023.7.7.2/docs/features/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6471 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/features/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8209 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/features/graphical.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.946824 autofit-2023.7.7.2/docs/features/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    53610 2021-01-26 21:44:53.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x1_1__low_snr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38449 2021-01-26 21:44:53.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x1_2__low_snr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37485 2021-01-26 21:44:53.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x1_3__low_snr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33505 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x1_with_feature.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44404 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x1_with_feature_fit_feature.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43221 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x1_with_feature_fit_no_feature.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46794 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x2_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25965 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x2_left.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38024 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x2_left_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    47517 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x2_right_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33623 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/gaussian_x2_split.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23811 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/sensitivity_data_high.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28902 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/sensitivity_data_high_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34204 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/sensitivity_data_low.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40377 2021-01-26 18:42:54.000000 autofit-2023.7.7.2/docs/features/images/sensitivity_data_low_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9083 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/features/search_chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5844 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/features/search_grid_search.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12076 2023-06-05 10:53:40.000000 autofit-2023.7.7.2/docs/features/sensitivity_mapping.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.958714 autofit-2023.7.7.2/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10257 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/general/adding_a_model_component.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1017 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2021-01-28 19:37:07.000000 autofit-2023.7.7.2/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1097 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/general/roadmap.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      494 2020-11-16 19:40:51.000000 autofit-2023.7.7.2/docs/general/software.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2300 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/general/workspace.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.965620 autofit-2023.7.7.2/docs/howtofit/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2033 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/howtofit/chapter_1_introduction.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1614 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/howtofit/chapter_database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2198 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/howtofit/chapter_graphical_models.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5493 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/howtofit/howtofit.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.971624 autofit-2023.7.7.2/docs/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69268 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/images/cornerplot.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/docs/images/toy_model_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    57271 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/docs/images/toy_model_fit_x2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9989 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.980586 autofit-2023.7.7.2/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1409 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1543 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1156 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1439 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1446 2021-01-26 22:07:31.000000 autofit-2023.7.7.2/docs/installation/troubleshooting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/docs/make.bat
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.988629 autofit-2023.7.7.2/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:29.998627 autofit-2023.7.7.2/docs/overview/image/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1010915 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/overview/image/cluster_example.jpg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  2030601 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/overview/image/lens_model.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  3051390 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/overview/image/lens_model_cluster.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13863 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/overview/model_complex.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10198 2023-05-09 16:10:42.000000 autofit-2023.7.7.2/docs/overview/model_fit.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12585 2023-03-27 14:43:03.000000 autofit-2023.7.7.2/docs/overview/multi_datasets.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6800 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/overview/non_linear_search.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11895 2023-06-05 10:53:40.000000 autofit-2023.7.7.2/docs/overview/result.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      344 2023-05-10 13:41:29.000000 autofit-2023.7.7.2/docs/requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:30.004756 autofit-2023.7.7.2/docs/science_examples/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13077 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/docs/science_examples/astronomy.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      139 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/eden.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:30.017090 autofit-2023.7.7.2/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1339 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/files/citation.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13632 2023-02-21 14:10:09.000000 autofit-2023.7.7.2/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1171 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       31 2021-06-17 13:08:20.000000 autofit-2023.7.7.2/files/eden.ini
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27322 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/files/gaussian_example.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      544 2021-02-11 23:21:00.000000 autofit-2023.7.7.2/files/release.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1226 2021-06-17 13:08:20.000000 autofit-2023.7.7.2/files/to_do_list
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2020-11-10 18:15:59.000000 autofit-2023.7.7.2/files/toy_model_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       74 2023-06-01 08:52:02.000000 autofit-2023.7.7.2/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:30.022647 autofit-2023.7.7.2/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2020-11-16 19:40:52.000000 autofit-2023.7.7.2/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12475 2023-02-21 14:10:09.000000 autofit-2023.7.7.2/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2021-12-09 20:28:25.000000 autofit-2023.7.7.2/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11881 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      175 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/readthedocs.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      240 2023-05-10 13:41:29.000000 autofit-2023.7.7.2/requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:30.031102 autofit-2023.7.7.2/scripts/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-02-24 17:53:38.000000 autofit-2023.7.7.2/scripts/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      454 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/scripts/add_notebook_quotes.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      268 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/scripts/aggregate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/scripts/example_map.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      833 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/scripts/update_identifiers.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      910 2023-06-05 20:26:39.000000 autofit-2023.7.7.2/scripts/update_identifiers_from_file.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       63 2023-06-07 09:58:30.034767 autofit-2023.7.7.2/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1917 2023-06-07 09:57:48.000000 autofit-2023.7.7.2/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2081 2023-02-21 14:09:59.000000 autofit-2023.7.7.2/to_do_list
```

### Comparing `autofit-2023.7.7.1/.github/workflows/main.yml` & `autofit-2023.7.7.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/CITATIONS.rst` & `autofit-2023.7.7.2/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/CODE_OF_CONDUCT.md` & `autofit-2023.7.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/CONTRIBUTING.md` & `autofit-2023.7.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/LICENSE` & `autofit-2023.7.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/PKG-INFO` & `autofit-2023.7.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofit
-Version: 2023.7.7.1
+Version: 2023.7.7.2
 Summary: Classy Probabilistic Programming
 Home-page: https://github.com/rhayes777/PyAutoFit
 Author: James Nightingale and Richard Hayes
 Author-email: richard@rghsoftware.co.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autofit-2023.7.7.1/README.rst` & `autofit-2023.7.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/__init__.py` & `autofit-2023.7.7.2/autofit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,8 +106,8 @@
 @register(abc.ABCMeta)
 def save_abc(pickler, obj):
     pickle._Pickler.save_type(pickler, obj)
 
 
 conf.instance.register(__file__)
 
-__version__ = "2023.7.7.1"
+__version__ = "2023.7.7.2"
```

### Comparing `autofit-2023.7.7.1/autofit/aggregator/aggregator.py` & `autofit-2023.7.7.2/autofit/aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/aggregator/predicate.py` & `autofit-2023.7.7.2/autofit/aggregator/predicate.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/aggregator/search_output.py` & `autofit-2023.7.7.2/autofit/aggregator/search_output.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/README.rst` & `autofit-2023.7.7.2/autofit/config/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/general.yaml` & `autofit-2023.7.7.2/autofit/config/general.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/non_linear/mcmc.yaml` & `autofit-2023.7.7.2/autofit/config/non_linear/mcmc.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/non_linear/nest.yaml` & `autofit-2023.7.7.2/autofit/config/non_linear/nest.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/non_linear/optimize.yaml` & `autofit-2023.7.7.2/autofit/config/non_linear/optimize.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/notation.yaml` & `autofit-2023.7.7.2/autofit/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/priors/Gaussian.yaml` & `autofit-2023.7.7.2/autofit/config/priors/Gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/priors/GaussianKurtosis.yaml` & `autofit-2023.7.7.2/autofit/config/priors/GaussianKurtosis.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/priors/README.rst` & `autofit-2023.7.7.2/autofit/config/priors/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/priors/model.yaml` & `autofit-2023.7.7.2/autofit/config/priors/model.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/priors/profiles.yaml` & `autofit-2023.7.7.2/autofit/config/priors/profiles.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/priors/template.yaml` & `autofit-2023.7.7.2/autofit/config/priors/template.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/config/visualize/plots_search.yaml` & `autofit-2023.7.7.2/autofit/config/visualize/plots_search.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/__init__.py` & `autofit-2023.7.7.2/autofit/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/aggregator/aggregator.py` & `autofit-2023.7.7.2/autofit/database/aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/aggregator/scrape.py` & `autofit-2023.7.7.2/autofit/database/aggregator/scrape.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/migration/migration.py` & `autofit-2023.7.7.2/autofit/database/migration/migration.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/migration/session_wrapper.py` & `autofit-2023.7.7.2/autofit/database/migration/session_wrapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/model/fit.py` & `autofit-2023.7.7.2/autofit/database/model/fit.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/model/instance.py` & `autofit-2023.7.7.2/autofit/database/model/instance.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/model/model.py` & `autofit-2023.7.7.2/autofit/database/model/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/model/prior.py` & `autofit-2023.7.7.2/autofit/database/model/prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/query/condition.py` & `autofit-2023.7.7.2/autofit/database/query/condition.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/query/junction.py` & `autofit-2023.7.7.2/autofit/database/query/junction.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/query/query/abstract.py` & `autofit-2023.7.7.2/autofit/database/query/query/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/query/query/attribute.py` & `autofit-2023.7.7.2/autofit/database/query/query/attribute.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/query/query/info.py` & `autofit-2023.7.7.2/autofit/database/query/query/info.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/query/query/named.py` & `autofit-2023.7.7.2/autofit/database/query/query/named.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/database/sqlalchemy_.py` & `autofit-2023.7.7.2/autofit/database/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/example/analysis.py` & `autofit-2023.7.7.2/autofit/example/analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/example/model.py` & `autofit-2023.7.7.2/autofit/example/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/example/util.py` & `autofit-2023.7.7.2/autofit/example/util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/exc.py` & `autofit-2023.7.7.2/autofit/exc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/fixtures.py` & `autofit-2023.7.7.2/autofit/fixtures.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/__init__.py` & `autofit-2023.7.7.2/autofit/graphical/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/declarative/abstract.py` & `autofit-2023.7.7.2/autofit/graphical/declarative/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/declarative/collection.py` & `autofit-2023.7.7.2/autofit/graphical/declarative/collection.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/declarative/factor/abstract.py` & `autofit-2023.7.7.2/autofit/graphical/declarative/factor/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/declarative/factor/analysis.py` & `autofit-2023.7.7.2/autofit/graphical/declarative/factor/analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/declarative/factor/hierarchical.py` & `autofit-2023.7.7.2/autofit/graphical/declarative/factor/hierarchical.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/declarative/factor/prior.py` & `autofit-2023.7.7.2/autofit/graphical/declarative/factor/prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/declarative/graph.py` & `autofit-2023.7.7.2/autofit/graphical/declarative/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/declarative/result.py` & `autofit-2023.7.7.2/autofit/graphical/declarative/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/ep_mean_field.py` & `autofit-2023.7.7.2/autofit/graphical/expectation_propagation/ep_mean_field.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/factor_optimiser.py` & `autofit-2023.7.7.2/autofit/graphical/expectation_propagation/factor_optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/history.py` & `autofit-2023.7.7.2/autofit/graphical/expectation_propagation/history.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/optimiser.py` & `autofit-2023.7.7.2/autofit/graphical/expectation_propagation/optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/stochastic.py` & `autofit-2023.7.7.2/autofit/graphical/expectation_propagation/stochastic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/visualise.py` & `autofit-2023.7.7.2/autofit/graphical/expectation_propagation/visualise.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/factor_graphs/abstract.py` & `autofit-2023.7.7.2/autofit/graphical/factor_graphs/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/factor_graphs/factor.py` & `autofit-2023.7.7.2/autofit/graphical/factor_graphs/factor.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/factor_graphs/graph.py` & `autofit-2023.7.7.2/autofit/graphical/factor_graphs/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/factor_graphs/jacobians.py` & `autofit-2023.7.7.2/autofit/graphical/factor_graphs/jacobians.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/factor_graphs/transform.py` & `autofit-2023.7.7.2/autofit/graphical/factor_graphs/transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/laplace/line_search.py` & `autofit-2023.7.7.2/autofit/graphical/laplace/line_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/laplace/newton.py` & `autofit-2023.7.7.2/autofit/graphical/laplace/newton.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/laplace/optimiser.py` & `autofit-2023.7.7.2/autofit/graphical/laplace/optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/mean_field.py` & `autofit-2023.7.7.2/autofit/graphical/mean_field.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/graphical/utils.py` & `autofit-2023.7.7.2/autofit/graphical/utils.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/interpolator.py` & `autofit-2023.7.7.2/autofit/interpolator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/identifier.py` & `autofit-2023.7.7.2/autofit/mapper/identifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/mock/mock_model.py` & `autofit-2023.7.7.2/autofit/mapper/mock/mock_model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/model.py` & `autofit-2023.7.7.2/autofit/mapper/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/model_mapper.py` & `autofit-2023.7.7.2/autofit/mapper/model_mapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/model_object.py` & `autofit-2023.7.7.2/autofit/mapper/model_object.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/operator.py` & `autofit-2023.7.7.2/autofit/mapper/operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/abstract.py` & `autofit-2023.7.7.2/autofit/mapper/prior/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/arithmetic.py` & `autofit-2023.7.7.2/autofit/mapper/prior/arithmetic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/assertion.py` & `autofit-2023.7.7.2/autofit/mapper/prior/arithmetic/assertion.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/compound.py` & `autofit-2023.7.7.2/autofit/mapper/prior/arithmetic/compound.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/deferred.py` & `autofit-2023.7.7.2/autofit/mapper/prior/deferred.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/gaussian.py` & `autofit-2023.7.7.2/autofit/mapper/prior/gaussian.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/log_gaussian.py` & `autofit-2023.7.7.2/autofit/mapper/prior/log_gaussian.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/log_uniform.py` & `autofit-2023.7.7.2/autofit/mapper/prior/log_uniform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/tuple_prior.py` & `autofit-2023.7.7.2/autofit/mapper/prior/tuple_prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/uniform.py` & `autofit-2023.7.7.2/autofit/mapper/prior/uniform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior/width_modifier.py` & `autofit-2023.7.7.2/autofit/mapper/prior/width_modifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior_model/abstract.py` & `autofit-2023.7.7.2/autofit/mapper/prior_model/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior_model/annotation.py` & `autofit-2023.7.7.2/autofit/mapper/prior_model/annotation.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior_model/attribute_pair.py` & `autofit-2023.7.7.2/autofit/mapper/prior_model/attribute_pair.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior_model/collection.py` & `autofit-2023.7.7.2/autofit/mapper/prior_model/collection.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior_model/prior_model.py` & `autofit-2023.7.7.2/autofit/mapper/prior_model/prior_model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/prior_model/recursion.py` & `autofit-2023.7.7.2/autofit/mapper/prior_model/recursion.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/variable.py` & `autofit-2023.7.7.2/autofit/mapper/variable.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mapper/variable_operator.py` & `autofit-2023.7.7.2/autofit/mapper/variable_operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/messages/abstract.py` & `autofit-2023.7.7.2/autofit/messages/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/messages/beta.py` & `autofit-2023.7.7.2/autofit/messages/beta.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/messages/composed_transform.py` & `autofit-2023.7.7.2/autofit/messages/composed_transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/messages/fixed.py` & `autofit-2023.7.7.2/autofit/messages/fixed.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/messages/gamma.py` & `autofit-2023.7.7.2/autofit/messages/gamma.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/messages/interface.py` & `autofit-2023.7.7.2/autofit/messages/interface.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/messages/normal.py` & `autofit-2023.7.7.2/autofit/messages/normal.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/messages/transform.py` & `autofit-2023.7.7.2/autofit/messages/transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/messages/utils.py` & `autofit-2023.7.7.2/autofit/messages/utils.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/mock.py` & `autofit-2023.7.7.2/autofit/mock.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/abstract_search.py` & `autofit-2023.7.7.2/autofit/non_linear/abstract_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/analysis/analysis.py` & `autofit-2023.7.7.2/autofit/non_linear/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/analysis/combined.py` & `autofit-2023.7.7.2/autofit/non_linear/analysis/combined.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/analysis/free_parameter.py` & `autofit-2023.7.7.2/autofit/non_linear/analysis/free_parameter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/analysis/indexed.py` & `autofit-2023.7.7.2/autofit/non_linear/analysis/indexed.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/analysis/model_analysis.py` & `autofit-2023.7.7.2/autofit/non_linear/analysis/model_analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/analysis/multiprocessing.py` & `autofit-2023.7.7.2/autofit/non_linear/analysis/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/__init__.py` & `autofit-2023.7.7.2/autofit/non_linear/grid/grid_search/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/job.py` & `autofit-2023.7.7.2/autofit/non_linear/grid/grid_search/job.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/result.py` & `autofit-2023.7.7.2/autofit/non_linear/grid/grid_search/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/result_builder.py` & `autofit-2023.7.7.2/autofit/non_linear/grid/grid_search/result_builder.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/grid/sensitivity.py` & `autofit-2023.7.7.2/autofit/non_linear/grid/sensitivity.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/grid/simple_grid.py` & `autofit-2023.7.7.2/autofit/non_linear/grid/simple_grid.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/initializer.py` & `autofit-2023.7.7.2/autofit/non_linear/initializer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mcmc/abstract_mcmc.py` & `autofit-2023.7.7.2/autofit/non_linear/mcmc/abstract_mcmc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mcmc/auto_correlations.py` & `autofit-2023.7.7.2/autofit/non_linear/mcmc/auto_correlations.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/emcee.py` & `autofit-2023.7.7.2/autofit/non_linear/mcmc/emcee/emcee.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/plotter.py` & `autofit-2023.7.7.2/autofit/non_linear/mcmc/emcee/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/samples.py` & `autofit-2023.7.7.2/autofit/non_linear/mcmc/emcee/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/plotter.py` & `autofit-2023.7.7.2/autofit/non_linear/mcmc/zeus/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/samples.py` & `autofit-2023.7.7.2/autofit/non_linear/mcmc/zeus/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/zeus.py` & `autofit-2023.7.7.2/autofit/non_linear/mcmc/zeus/zeus.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mock/mock_analysis.py` & `autofit-2023.7.7.2/autofit/non_linear/mock/mock_analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mock/mock_result.py` & `autofit-2023.7.7.2/autofit/non_linear/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mock/mock_samples.py` & `autofit-2023.7.7.2/autofit/non_linear/mock/mock_samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/mock/mock_search.py` & `autofit-2023.7.7.2/autofit/non_linear/mock/mock_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/nest/abstract_nest.py` & `autofit-2023.7.7.2/autofit/non_linear/nest/abstract_nest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/abstract.py` & `autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/dynamic.py` & `autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/dynamic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/plotter.py` & `autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/samples.py` & `autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/static.py` & `autofit-2023.7.7.2/autofit/non_linear/nest/dynesty/static.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/plotter.py` & `autofit-2023.7.7.2/autofit/non_linear/nest/ultranest/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/samples.py` & `autofit-2023.7.7.2/autofit/non_linear/nest/ultranest/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/ultranest.py` & `autofit-2023.7.7.2/autofit/non_linear/nest/ultranest/ultranest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/optimize/abstract_optimize.py` & `autofit-2023.7.7.2/autofit/non_linear/optimize/abstract_optimize.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/drawer.py` & `autofit-2023.7.7.2/autofit/non_linear/optimize/drawer/drawer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/lbfgs.py` & `autofit-2023.7.7.2/autofit/non_linear/optimize/lbfgs/lbfgs.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/samples.py` & `autofit-2023.7.7.2/autofit/non_linear/optimize/lbfgs/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/abstract.py` & `autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/globe.py` & `autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/globe.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/local.py` & `autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/local.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/plotter.py` & `autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/samples.py` & `autofit-2023.7.7.2/autofit/non_linear/optimize/pyswarms/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/parallel/process.py` & `autofit-2023.7.7.2/autofit/non_linear/parallel/process.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/parallel/sneaky.py` & `autofit-2023.7.7.2/autofit/non_linear/parallel/sneaky.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/paths/abstract.py` & `autofit-2023.7.7.2/autofit/non_linear/paths/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/paths/database.py` & `autofit-2023.7.7.2/autofit/non_linear/paths/database.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/paths/directory.py` & `autofit-2023.7.7.2/autofit/non_linear/paths/directory.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/paths/null.py` & `autofit-2023.7.7.2/autofit/non_linear/paths/null.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/paths/sub_directory_paths.py` & `autofit-2023.7.7.2/autofit/non_linear/paths/sub_directory_paths.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/result.py` & `autofit-2023.7.7.2/autofit/non_linear/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/samples/mcmc.py` & `autofit-2023.7.7.2/autofit/non_linear/samples/mcmc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/samples/nest.py` & `autofit-2023.7.7.2/autofit/non_linear/samples/nest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/samples/pdf.py` & `autofit-2023.7.7.2/autofit/non_linear/samples/pdf.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/samples/sample.py` & `autofit-2023.7.7.2/autofit/non_linear/samples/sample.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/samples/samples.py` & `autofit-2023.7.7.2/autofit/non_linear/samples/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/samples/stored.py` & `autofit-2023.7.7.2/autofit/non_linear/samples/stored.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/settings.py` & `autofit-2023.7.7.2/autofit/non_linear/settings.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/non_linear/timer.py` & `autofit-2023.7.7.2/autofit/non_linear/timer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/plot/output.py` & `autofit-2023.7.7.2/autofit/plot/output.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/plot/samples_plotters.py` & `autofit-2023.7.7.2/autofit/plot/samples_plotters.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/text/formatter.py` & `autofit-2023.7.7.2/autofit/text/formatter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/text/samples_text.py` & `autofit-2023.7.7.2/autofit/text/samples_text.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/text/text_util.py` & `autofit-2023.7.7.2/autofit/text/text_util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/tools/add_notebook_quotes.py` & `autofit-2023.7.7.2/autofit/tools/add_notebook_quotes.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/tools/update_identifiers.py` & `autofit-2023.7.7.2/autofit/tools/update_identifiers.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit/tools/util.py` & `autofit-2023.7.7.2/autofit/tools/util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/autofit.egg-info/SOURCES.txt` & `autofit-2023.7.7.2/autofit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/Makefile` & `autofit-2023.7.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/_templates/custom-class-template.rst` & `autofit-2023.7.7.2/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/_templates/custom_module_template.rst` & `autofit-2023.7.7.2/docs/_templates/custom_module_template.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/api/analysis.rst` & `autofit-2023.7.7.2/docs/api/analysis.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/api/database.rst` & `autofit-2023.7.7.2/docs/api/database.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/api/model.rst` & `autofit-2023.7.7.2/docs/api/model.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/api/plot.rst` & `autofit-2023.7.7.2/docs/api/plot.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/api/priors.rst` & `autofit-2023.7.7.2/docs/api/priors.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/api/samples.rst` & `autofit-2023.7.7.2/docs/api/samples.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/api/searches.rst` & `autofit-2023.7.7.2/docs/api/searches.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/api/source.rst` & `autofit-2023.7.7.2/docs/api/source.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/conf.py` & `autofit-2023.7.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/cookbooks/cookbook_1_basics.rst` & `autofit-2023.7.7.2/docs/cookbooks/cookbook_1_basics.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/cookbooks/cookbook_2_collections.rst` & `autofit-2023.7.7.2/docs/cookbooks/cookbook_2_collections.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/cookbooks/cookbook_3_multiple_datasets.rst` & `autofit-2023.7.7.2/docs/cookbooks/cookbook_3_multiple_datasets.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/cookbooks/cookbook_4_multi_level.rst` & `autofit-2023.7.7.2/docs/cookbooks/cookbook_4_multi_level.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/cookbooks/cookbook_5_model_linking.rst` & `autofit-2023.7.7.2/docs/cookbooks/cookbook_5_model_linking.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/database.rst` & `autofit-2023.7.7.2/docs/features/database.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/graphical.rst` & `autofit-2023.7.7.2/docs/features/graphical.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x1_1__low_snr.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x1_1__low_snr.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x1_2__low_snr.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x1_2__low_snr.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x1_3__low_snr.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x1_3__low_snr.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x1_with_feature.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature_fit_feature.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x1_with_feature_fit_feature.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature_fit_no_feature.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x1_with_feature_fit_no_feature.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x2_fit.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x2_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x2_left.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x2_left.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x2_left_fit.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x2_left_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x2_right_fit.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x2_right_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/gaussian_x2_split.png` & `autofit-2023.7.7.2/docs/features/images/gaussian_x2_split.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/sensitivity_data_high.png` & `autofit-2023.7.7.2/docs/features/images/sensitivity_data_high.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/sensitivity_data_high_fit.png` & `autofit-2023.7.7.2/docs/features/images/sensitivity_data_high_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/sensitivity_data_low.png` & `autofit-2023.7.7.2/docs/features/images/sensitivity_data_low.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/images/sensitivity_data_low_fit.png` & `autofit-2023.7.7.2/docs/features/images/sensitivity_data_low_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/search_chaining.rst` & `autofit-2023.7.7.2/docs/features/search_chaining.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/search_grid_search.rst` & `autofit-2023.7.7.2/docs/features/search_grid_search.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/features/sensitivity_mapping.rst` & `autofit-2023.7.7.2/docs/features/sensitivity_mapping.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/general/adding_a_model_component.rst` & `autofit-2023.7.7.2/docs/general/adding_a_model_component.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/general/citations.rst` & `autofit-2023.7.7.2/docs/general/citations.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/general/configs.rst` & `autofit-2023.7.7.2/docs/general/configs.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/general/roadmap.rst` & `autofit-2023.7.7.2/docs/general/roadmap.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/general/workspace.rst` & `autofit-2023.7.7.2/docs/general/workspace.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/howtofit/chapter_1_introduction.rst` & `autofit-2023.7.7.2/docs/howtofit/chapter_1_introduction.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/howtofit/chapter_database.rst` & `autofit-2023.7.7.2/docs/howtofit/chapter_database.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/howtofit/chapter_graphical_models.rst` & `autofit-2023.7.7.2/docs/howtofit/chapter_graphical_models.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/howtofit/howtofit.rst` & `autofit-2023.7.7.2/docs/howtofit/howtofit.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/images/cornerplot.png` & `autofit-2023.7.7.2/docs/images/cornerplot.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/images/toy_model_fit.png` & `autofit-2023.7.7.2/docs/images/toy_model_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/images/toy_model_fit_x2.png` & `autofit-2023.7.7.2/docs/images/toy_model_fit_x2.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/index.rst` & `autofit-2023.7.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/installation/conda.rst` & `autofit-2023.7.7.2/docs/installation/conda.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/installation/overview.rst` & `autofit-2023.7.7.2/docs/installation/overview.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/installation/pip.rst` & `autofit-2023.7.7.2/docs/installation/pip.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/installation/source.rst` & `autofit-2023.7.7.2/docs/installation/source.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/installation/troubleshooting.rst` & `autofit-2023.7.7.2/docs/installation/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/make.bat` & `autofit-2023.7.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/overview/image/cluster_example.jpg` & `autofit-2023.7.7.2/docs/overview/image/cluster_example.jpg`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/overview/image/lens_model.png` & `autofit-2023.7.7.2/docs/overview/image/lens_model.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/overview/image/lens_model_cluster.png` & `autofit-2023.7.7.2/docs/overview/image/lens_model_cluster.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/overview/model_complex.rst` & `autofit-2023.7.7.2/docs/overview/model_complex.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/overview/model_fit.rst` & `autofit-2023.7.7.2/docs/overview/model_fit.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/overview/multi_datasets.rst` & `autofit-2023.7.7.2/docs/overview/multi_datasets.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/overview/non_linear_search.rst` & `autofit-2023.7.7.2/docs/overview/non_linear_search.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/overview/result.rst` & `autofit-2023.7.7.2/docs/overview/result.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/docs/science_examples/astronomy.rst` & `autofit-2023.7.7.2/docs/science_examples/astronomy.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/files/citation.tex` & `autofit-2023.7.7.2/files/citation.tex`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/files/citations.bib` & `autofit-2023.7.7.2/files/citations.bib`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/files/citations.md` & `autofit-2023.7.7.2/files/citations.md`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/files/gaussian_example.png` & `autofit-2023.7.7.2/files/gaussian_example.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/files/release.sh` & `autofit-2023.7.7.2/files/release.sh`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/files/to_do_list` & `autofit-2023.7.7.2/files/to_do_list`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/files/toy_model_fit.png` & `autofit-2023.7.7.2/files/toy_model_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/paper/paper.bib` & `autofit-2023.7.7.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/paper/paper.json` & `autofit-2023.7.7.2/paper/paper.json`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/paper/paper.md` & `autofit-2023.7.7.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/scripts/update_identifiers.py` & `autofit-2023.7.7.2/scripts/update_identifiers.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/scripts/update_identifiers_from_file.py` & `autofit-2023.7.7.2/scripts/update_identifiers_from_file.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.7.7.1/setup.py` & `autofit-2023.7.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "2023.7.7.1")
+version = environ.get("VERSION", "2023.7.7.2")
 requirements.extend([
     f'autoconf=={version}'
 ])
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
```

### Comparing `autofit-2023.7.7.1/to_do_list` & `autofit-2023.7.7.2/to_do_list`

 * *Files identical despite different names*

