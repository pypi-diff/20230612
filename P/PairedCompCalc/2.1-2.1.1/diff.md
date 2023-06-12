# Comparing `tmp/PairedCompCalc-2.1.tar.gz` & `tmp/PairedCompCalc-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PairedCompCalc-2.1.tar", last modified: Fri Sep  9 12:20:04 2022, max compression
+gzip compressed data, was "PairedCompCalc-2.1.1.tar", last modified: Mon Jun 12 13:09:50 2023, max compression
```

## Comparing `PairedCompCalc-2.1.tar` & `PairedCompCalc-2.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2022-09-09 12:20:04.058766 PairedCompCalc-2.1/
--rw-r--r--   0 arne       (503) staff       (20)     1083 2018-08-05 14:59:07.000000 PairedCompCalc-2.1/LICENSE.txt
--rw-r--r--   0 arne       (503) staff       (20)     7721 2022-09-09 12:20:04.059112 PairedCompCalc-2.1/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)     7029 2022-09-01 12:14:18.000000 PairedCompCalc-2.1/README.md
--rw-r--r--   0 arne       (503) staff       (20)      103 2021-09-24 09:50:47.000000 PairedCompCalc-2.1/pyproject.toml
--rw-r--r--   0 arne       (503) staff       (20)      935 2022-09-09 12:20:04.060298 PairedCompCalc-2.1/setup.cfg
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2022-09-09 12:20:04.030010 PairedCompCalc-2.1/src/
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2022-09-09 12:20:04.053118 PairedCompCalc-2.1/src/PairedCompCalc/
--rw-r--r--   0 arne       (503) staff       (20)     7299 2022-09-09 08:50:18.000000 PairedCompCalc-2.1/src/PairedCompCalc/__init__.py
--rw-r--r--   0 arne       (503) staff       (20)    21300 2019-08-07 06:38:31.000000 PairedCompCalc-2.1/src/PairedCompCalc/gauss_gamma.py
--rw-r--r--   0 arne       (503) staff       (20)     4714 2019-08-07 06:38:40.000000 PairedCompCalc-2.1/src/PairedCompCalc/gauss_gamma_null.py
--rw-r--r--   0 arne       (503) staff       (20)    36025 2022-09-09 08:04:48.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_data.py
--rw-r--r--   0 arne       (503) staff       (20)    55503 2022-09-07 07:22:35.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_display.py
--rw-r--r--   0 arne       (503) staff       (20)    25591 2022-09-06 09:04:19.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_display_format.py
--rw-r--r--   0 arne       (503) staff       (20)    15054 2022-09-08 13:45:45.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_file.py
--rw-r--r--   0 arne       (503) staff       (20)    16281 2022-09-07 08:02:14.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_file_res.py
--rw-r--r--   0 arne       (503) staff       (20)     1191 2018-08-15 09:19:30.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_logging.py
--rw-r--r--   0 arne       (503) staff       (20)     2807 2022-09-06 08:24:59.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_lr_test.py
--rw-r--r--   0 arne       (503) staff       (20)    43214 2022-09-04 08:52:29.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_model.py
--rw-r--r--   0 arne       (503) staff       (20)    23837 2022-09-09 08:50:18.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_planning.py
--rw-r--r--   0 arne       (503) staff       (20)    27553 2022-07-01 13:51:33.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_simulation.py
--rw-r--r--   0 arne       (503) staff       (20)    12939 2022-06-20 10:55:31.000000 PairedCompCalc-2.1/src/PairedCompCalc/pc_subject.py
--rw-r--r--   0 arne       (503) staff       (20)     8823 2022-09-09 08:22:14.000000 PairedCompCalc-2.1/src/PairedCompCalc/run_pc.py
--rw-r--r--   0 arne       (503) staff       (20)     9211 2022-09-09 09:28:08.000000 PairedCompCalc-2.1/src/PairedCompCalc/run_plan.py
--rw-r--r--   0 arne       (503) staff       (20)     8746 2022-09-09 08:22:14.000000 PairedCompCalc-2.1/src/PairedCompCalc/run_sim.py
--rw-r--r--   0 arne       (503) staff       (20)     3689 2021-09-24 08:41:42.000000 PairedCompCalc-2.1/src/PairedCompCalc/safe_logistic.py
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2022-09-09 12:20:04.057890 PairedCompCalc-2.1/src/PairedCompCalc.egg-info/
--rw-r--r--   0 arne       (503) staff       (20)     7721 2022-09-09 12:20:04.000000 PairedCompCalc-2.1/src/PairedCompCalc.egg-info/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)      852 2022-09-09 12:20:04.000000 PairedCompCalc-2.1/src/PairedCompCalc.egg-info/SOURCES.txt
--rw-r--r--   0 arne       (503) staff       (20)        1 2022-09-09 12:20:04.000000 PairedCompCalc-2.1/src/PairedCompCalc.egg-info/dependency_links.txt
--rw-r--r--   0 arne       (503) staff       (20)       72 2022-09-09 12:20:04.000000 PairedCompCalc-2.1/src/PairedCompCalc.egg-info/requires.txt
--rw-r--r--   0 arne       (503) staff       (20)       15 2022-09-09 12:20:04.000000 PairedCompCalc-2.1/src/PairedCompCalc.egg-info/top_level.txt
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-06-12 13:09:50.973306 PairedCompCalc-2.1.1/
+-rw-r--r--   0 arne       (503) staff       (20)     1083 2018-08-05 14:59:07.000000 PairedCompCalc-2.1.1/LICENSE.txt
+-rw-r--r--   0 arne       (503) staff       (20)     7723 2023-06-12 13:09:50.973358 PairedCompCalc-2.1.1/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)     7029 2022-09-01 12:14:18.000000 PairedCompCalc-2.1.1/README.md
+-rw-r--r--   0 arne       (503) staff       (20)      103 2021-09-24 09:50:47.000000 PairedCompCalc-2.1.1/pyproject.toml
+-rw-r--r--   0 arne       (503) staff       (20)      945 2023-06-12 13:09:50.973590 PairedCompCalc-2.1.1/setup.cfg
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-06-12 13:09:50.966476 PairedCompCalc-2.1.1/src/
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-06-12 13:09:50.972392 PairedCompCalc-2.1.1/src/PairedCompCalc/
+-rw-r--r--   0 arne       (503) staff       (20)     7493 2023-06-12 07:18:11.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/__init__.py
+-rw-r--r--   0 arne       (503) staff       (20)    21300 2019-08-07 06:38:31.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/gauss_gamma.py
+-rw-r--r--   0 arne       (503) staff       (20)     4714 2019-08-07 06:38:40.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/gauss_gamma_null.py
+-rw-r--r--   0 arne       (503) staff       (20)    36025 2022-09-09 08:04:48.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_data.py
+-rw-r--r--   0 arne       (503) staff       (20)    55501 2023-06-12 09:29:08.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_display.py
+-rw-r--r--   0 arne       (503) staff       (20)    26103 2023-06-12 08:47:03.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_display_format.py
+-rw-r--r--   0 arne       (503) staff       (20)    15054 2022-09-08 13:45:45.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_file.py
+-rw-r--r--   0 arne       (503) staff       (20)    16281 2022-09-07 08:02:14.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_file_res.py
+-rw-r--r--   0 arne       (503) staff       (20)     9480 2023-06-12 08:19:42.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_latent.py
+-rw-r--r--   0 arne       (503) staff       (20)     1191 2018-08-15 09:19:30.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_logging.py
+-rw-r--r--   0 arne       (503) staff       (20)    39134 2023-06-12 09:38:47.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_model.py
+-rw-r--r--   0 arne       (503) staff       (20)    23837 2022-09-09 08:50:18.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_planning.py
+-rw-r--r--   0 arne       (503) staff       (20)    27553 2022-07-01 13:51:33.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_simulation.py
+-rw-r--r--   0 arne       (503) staff       (20)    12939 2022-06-20 10:55:31.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/pc_subject.py
+-rw-r--r--   0 arne       (503) staff       (20)     9218 2023-06-12 09:06:26.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/run_pc.py
+-rw-r--r--   0 arne       (503) staff       (20)     9211 2022-09-09 09:28:08.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/run_plan.py
+-rw-r--r--   0 arne       (503) staff       (20)     8746 2022-09-09 08:22:14.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/run_sim.py
+-rw-r--r--   0 arne       (503) staff       (20)     3689 2021-09-24 08:41:42.000000 PairedCompCalc-2.1.1/src/PairedCompCalc/safe_logistic.py
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-06-12 13:09:50.973201 PairedCompCalc-2.1.1/src/PairedCompCalc.egg-info/
+-rw-r--r--   0 arne       (503) staff       (20)     7723 2023-06-12 13:09:50.000000 PairedCompCalc-2.1.1/src/PairedCompCalc.egg-info/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)      851 2023-06-12 13:09:50.000000 PairedCompCalc-2.1.1/src/PairedCompCalc.egg-info/SOURCES.txt
+-rw-r--r--   0 arne       (503) staff       (20)        1 2023-06-12 13:09:50.000000 PairedCompCalc-2.1.1/src/PairedCompCalc.egg-info/dependency_links.txt
+-rw-r--r--   0 arne       (503) staff       (20)       81 2023-06-12 13:09:50.000000 PairedCompCalc-2.1.1/src/PairedCompCalc.egg-info/requires.txt
+-rw-r--r--   0 arne       (503) staff       (20)       15 2023-06-12 13:09:50.000000 PairedCompCalc-2.1.1/src/PairedCompCalc.egg-info/top_level.txt
```

### Comparing `PairedCompCalc-2.1/LICENSE.txt` & `PairedCompCalc-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/PKG-INFO` & `PairedCompCalc-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PairedCompCalc
-Version: 2.1
+Version: 2.1.1
 Summary: Statistical Analysis of Paired-Comparison Data
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: paired-comparison,Bayesian,psycho-physics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PairedCompCalc-2.1/README.md` & `PairedCompCalc-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/setup.cfg` & `PairedCompCalc-2.1.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
 install_requires = 
-	numpy >=1.17
+	numpy >=1.22
 	scipy >=1.7
-	matplotlib
-	samppy >=1.2
-	pandas >=1.4
+	matplotlib >=3.6.2
+	samppy >=1.3
+	pandas >=2.0.1
 	openpyxl >=3.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/__init__.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,19 @@
 
 R. A. Bradley and M. E. Terry (1952).
 Rank analysis of incomplete block designs. I. The method of paired comparisons.
 *Biometrika* 39, 324–345, doi: 10.2307/2334029.
 
 
 *** Version history:
+** Version 2.1.1:
+2023-06-14, new module pc_latent with numerically safer versions of
+            Bradley, Thurstone, for distributions of latent variables.
+            (copied from EmaCalc)
+
 ** Version 2.1:
 2022-09-01, likelihood ratio test deprecated, as suggested by JASA paper reviewer.
 2022-07-04, using Pandas for data input and result tables
 
 ** Version 2.0.1:
 2022-03-09, minor fix pc_model, pc_data, pc_file_xlsx for clearer logging/error displays
 
@@ -155,9 +160,9 @@
 2018-05-21, allow choice among three types of predictive distributions
 2018-08-05, using prior gauss_gamma module for population distribution, tested pc_power
 2018-08-14, simplified internal structure of PairedCompDataSet
 2018-08-15, First public version 0.8.3
 """
 
 __name__ = 'PairedCompCalc'
-__version__ = '2.1'
+__version__ = '2.1.1'
 __all__ = ['__version__', 'run_pc', 'run_plan', 'run_sim']
```

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/gauss_gamma.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/gauss_gamma.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/gauss_gamma_null.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/gauss_gamma_null.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_data.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_data.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_display.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_display.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,20 +40,20 @@
     The display elements are accessible as, e.g.,
     pc_ds.groups['NormalHearing']['population_mean']['Intelligibility'].range.percentile_plot.ax
         = the Axes object where percentiles are plotted for this group, pooled across all test conditions
     pc_ds.groups['NormalHearing'].attr_corr is a table of credible correlations between attributes,
         in the results for the selected group, if any are credible
 
 Figures and tables are automatically assigned descriptive names,
-and stored in sub-directories with names constructed from
+and stored in subdirectories with names constructed from
 string labels of Groups and Attributes and test conditions,
 as defined in the PairedCompFrame object of the input PairedCompResultSet instance.
 
 If there is more than one Group,
-    one sub-directory is created for each group, and one extra for all groups pooled,
+    one subdirectory is created for each group, and one extra for all groups pooled,
     and one sub-sub-directory for each requested population / subject predictive result,
     and one sub-sub-sub-directory for each attribute, with results within the group.
     If there is more than one attribute,
     the group sub-directory may also include tables with correlations between attributes.
 
 Thus, after saving, the display files are stored in a directory structure as, e.g.,
 result_path / group / 'population_individual' / attribute / ....
```

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_display_format.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_display_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """This module includes functions to format output displays of
 PairedCompResultSet model results,
 in either graphic or textual form.
 
 *** Version History:
+* Version 2.1.1:
+2023-06-12, interaction_sep, condition_sep -> FMT
+            (old hard-coded interaction_sep='*' not allowed in file names)
+
 * Version 2.1:
 2022-09-04, allow mpl_style and mpl_params argument for plot parameters
 2022-09-01, attribute table as pandas.DataFrame; function tab_lr_test deleted!
 2022-07-05, set figure save format in FigureRef.save method, to allow several save calls
 2022-07-04, make tables as subclass of pandas.DataFrame to allow more save formats
 
 * Version 2.0:
@@ -47,14 +51,16 @@
        'markers': 'oxs*_',  # corresponding markers, cyclic use
        'show_intervals': True,  # include median response thresholds in plots
        'probability': 'Probability',  # heading in tables
        'attribute': 'Attribute',  # heading in tables
        'group': 'Group',  # heading in tables
        'correlation': 'Correlation',  # heading in tables
        'scale_unit': '',  # scale unit for attribute plot axis
+       'interaction_sep': '\u00D7',  # mult.sign. separating condition labels in result file names
+       'condition_sep': '_',    # separating attribute and its test condition(s) in file names
        }
 # = module-global dict with default settings for display details
 # that may be changed by user
 
 
 def set_format_param(mpl_style=None, mpl_params=None, **kwargs):
     """Set / modify format parameters.
@@ -280,16 +286,16 @@
         y1 = y_max
     ax.set_ylim(y0, y1)
     ax.set_ylabel(y_label)
     ax.set_xlabel(x_label)
     if len(case_list) > 1:
         ax.legend(loc='best')
     if len(file_label) > 0:
-        file_label += '_'
-    f_name = file_label + '*'.join(df.index.names)
+        file_label += FMT['condition_sep']
+    f_name = file_label + FMT['interaction_sep'].join(df.index.names)
     # fig.set_tight_layout(tight=True)
     return FigureRef(ax, name=f_name)
 
 
 def fig_indiv_boxplot(q,
                       y_label,
                       object_tuple,
@@ -370,15 +376,17 @@
     if len(y_unit) > 0:
         ax.set_ylabel(y_label + ' (' + y_unit + ')')
     else:
         ax.set_ylabel(y_label)
     ax.set_xlabel(x_label)
     if np.any([len(cl) > 0 for cl in case_labels]):
         ax.legend(loc='best')
-    f_name = y_label + '-box' + '_' + x_label + ('_' + case_head if len(case_head) > 0 else '')
+    f_name = (y_label + '-box'
+              + FMT['condition_sep'] + x_label
+              + (FMT['interaction_sep'] + case_head if len(case_head) > 0 else ''))
     return FigureRef(ax, name=f_name)
 
 
 def _plot_response_intervals(ax, c_lim):
     """plot horizontal lines to indicate response-category intervals
     :param ax: axis object
     :param c_lim: 1D array with scalar interval limits
@@ -457,31 +465,31 @@
     # --------------------------------------------------------------------
     df = pd.DataFrame({f'{p_i:.1f}%': q_i
                        for (p_i, q_i) in zip(perc,
                                              q_perc.T)},  # .reshape((n_perc, -1)))},
                       index=pd.MultiIndex.from_product([*case_labels.values()],
                                                        names=[*case_labels.keys()]))
     if len(file_label) > 0:
-        file_label += '_'
-    f_name = file_label + '*'.join(case_labels.keys())
+        file_label += FMT['condition_sep']  #_'
+    f_name = file_label + FMT['interaction_sep'].join(case_labels.keys())
     return TableRef(df, name=f_name)
 
 
 def tab_credible_diff(diff,
                       diff_labels,
                       diff_head,
                       cred_head,
                       case_labels=(),
                       case_head=(),
                       y_label='',
                       file_label='',
                       # high_low=('Higher', 'Lower'),
                       and_label='and',  # label in And column
                       and_head=('', '')
-                      ):  # **************** copied from EmaCalc
+                      ):
     """Create table with credible differences among results
     :param diff: list of tuples ((i,j), p) OR ((i,j,c), p),
         defining jointly credible differences, indicating that
         prob{ quality of diff_labels[i] > quality of diff_labels[j]}, OR
         prob{ quality of diff_labels[i] > quality of diff_labels[j] | case_labels[c] }
         AND all previous pairs } == p
     :param diff_labels: list of tuples with labels of compared random-vector elements
@@ -526,18 +534,18 @@
                   for d in diff]
         col |= {('', c_head_k): [c_val[k] for c_val in diff_c]
                 for (k, c_head_k) in enumerate(case_head)}
     col |= {('', cred_head): [d[1] for d in diff]}
     df = pd.DataFrame(col)
     df = df.reindex(columns=pd.MultiIndex.from_tuples(df.columns))
     if len(file_label) > 0:
-        file_label += '_'
-    f_name = file_label + '*'.join(diff_head) + '-diff'
+        file_label += FMT['condition_sep']
+    f_name = file_label + FMT['interaction_sep'].join(diff_head) + '-diff'
     if len(case_head) > 0:
-        f_name += '_' + '*'.join(case_head)
+        f_name += FMT['condition_sep'] + FMT['interaction_sep'].join(case_head)
     return DiffTableRef(df, name=f_name)
 
 
 def tab_credible_corr(c, a_labels,
                       file_label='Correlation',
                       and_head='',
                       and_label='and'):
```

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_file.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_file.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_file_res.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_file_res.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_logging.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_logging.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_model.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,23 +41,24 @@
     thus representing a single mixture distribution for all individuals in a group.
 
 PopulationModel: a GaussianRV prior and posterior model for population parameters.
 
 PopulationPredictiveModel: Parametric predictive model for
     the marginal distribution of parameters in the population.
 
-Bradley:   Bradley-Terry-Luce model: logistic probability distribution for decision variables
-Thurstone: Thurstone Case V model: Gaussian probability distribution for decision variables
-
 *** Reference:
 Leijon et al (2019) Bayesian Analysis of Paired-comparison Sound Quality Ratings.
     J Acoust Soc Amer, 146(5), 3174-3183. doi: 10.1121/1.5131024
     Appendices describe the probabilistic model in detail.
 
 *** Version History:
+** Version 2.1.1:
+2023-06-12, Bradley, Thurstone moved to separate module pc_latent.py,
+            and modified for better numerical behavior in extreme cases.
+
 ** Version 2.1:
 2022-07-01, modified to use pc_data.PairedCompDataSet with pd.DataFrame storage
 
 ** Version 2.0.1:
 2022-03-12, subject entropy calculation from PairedCompGroupModel -> PairedCompIndModel.adapt()
 2022-03-10, PairedCompIndModel -> separate module pc_subject
 2022-03-10, simplified logger.info output during iterative learning
@@ -92,26 +93,26 @@
 
 # perhaps integrate out population mean and prec and use Student-t distribution directly,
 # with ML type II point estimation of hyperparameters (beta, a, b) ???
 # or perhaps fixed beta = N, and free (a, b) only ???
 # *** but present VI approximation seems already quite OK
 
 import numpy as np
-from scipy.special import expit, ndtr
 # import pandas as pd
 
 # from collections import OrderedDict  # , Counter
 import logging
 import copy
 
 from PairedCompCalc import gauss_gamma, gauss_gamma_null
 from PairedCompCalc.pc_subject import PairedCompIndModel
 from PairedCompCalc.pc_subject import cat_limits_transform, d_cat_limits_transform
 from PairedCompCalc.pc_file import PAIR_COLUMN, DIFF_COLUMN
 # = globally fixed column names in input DataFrame objects
+from PairedCompCalc.pc_latent import Bradley, Thurstone
 
 PopulationModel = gauss_gamma.GaussianRV
 PopulationNullModel = gauss_gamma_null.GaussianNullRV
 # *** used only for likelihood ratio test, deprecated in version >=2.1
 
 # an alternative model might be gauss_wishart.GaussianRV
 # with correlated quality parameters
@@ -131,130 +132,20 @@
 # = prior scale for log response-interval width parameters
 #   used to restrict ratio between interval widths
 # typical width ratio = cw_big / cw_small = exp(2 * PRIOR_CAT_WIDTH_SCALE)
 
 # 2018-07-11, gives OK empirical coverage of cred.interval for population mean
 # initial sampler epsilon = 0.1 seems generally OK, several tests
 
-# ------------------------------------------------------------------------
-
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # test
 
 
 # ------------------------------------------------------------------
-class Bradley:
-    """Distribution of decision variable in the Bradley-Terry-Luce model.
-    """
-    unit_label = 'BTL unit'
-    # for axis label in quality plots
-
-    @staticmethod
-    def log_cdf_diff(a, b):
-        """log prob( a < Z <= b)
-        where Z is a standard logistic random variable
-        :param a: = array with LOWER interval limits
-        :param b: = arrays with UPPER interval limits
-            a.shape == b.shape
-            all( a < b )
-        :return: log_p = array with log probabilities, element-wise
-            log_p.shape == a.shape == b.shape
-        """
-        return np.log(expit(b) - expit(a))
-
-    @staticmethod
-    def d_log_cdf_diff(a, b):
-        """Element-wise partial derivatives of log_cdf_diff(a, b)
-        :param a: = array with LOWER interval limits
-        :param b: = arrays with UPPER interval limits
-            a.shape == b.shape
-            all( a < b )
-        :return: tuple (dll_da, dll_db) of arrays, where
-            dll_da[...] = d log_cdf_diff(a[...], b[...]) / d a[...]
-            dll_db[...] = d log_cdf_diff(a[...], b[...]) / d b[...]
-            dll_da.shape == dll_db.shape == a.shape == b.shape
-        Arne Leijon, 2017-12-08, tested by finite-diff comparison
-        """
-        return (1. / np.expm1(a - b) + expit(-a),
-                1. / np.expm1(b - a) + expit(-b))
-
-    def __repr__(self):
-        return '<class Bradley>'
-
-
-class Thurstone:
-    """Distribution of decision variable in the Thurstone Case V model.
-    NOTE: Thurstone.scale is now included in all calculations.
-    This is different from corresponding MatLab code.
-    """
-    unit_label = 'd-prime unit'
-
-    sqrt_2pi = np.sqrt(2. * np.pi)
-    scale = np.sqrt(2.)
-
-    @staticmethod
-    def cdf_diff(a, b):
-        """prob( a < Z <= b)
-        where Z is a Gaussian standard random variable with variance = 2.
-        :param a: = array with LOWER interval limits
-        :param b: = arrays with UPPER interval limits
-            a.shape == b.shape
-            all( a < b )
-        :return: log_p = array with log probabilities, element-wise
-            log_p.shape == a.shape == b.shape
-        2018-04-24, include Thurstone.scale factor
-        """
-        a_s = a / Thurstone.scale
-        b_s = b / Thurstone.scale
-        cdf_diff = ndtr(b_s) - ndtr(a_s)
-        ch_sign = a_s >= 0.  # and (b > a) always
-        cdf_diff[ch_sign] = ndtr(-a_s[ch_sign]) - ndtr(-b_s[ch_sign])
-        # better precision of difference in case of large positive a, b
-        return cdf_diff
-
-    @staticmethod
-    def log_cdf_diff(a, b):
-        """log cdf_diff(a, b)
-        :param a: = array with LOWER interval limits
-        :param b: = arrays with UPPER interval limits
-            a.shape == b.shape
-            all( a < b )
-        :return: log_p = array with log probabilities, element-wise
-            log_p.shape == a.shape == b.shape
-        """
-        return np.log(Thurstone.cdf_diff(a, b))
-
-    @staticmethod
-    def d_log_cdf_diff(a, b):
-        """Element-wise partial derivatives of log_cdf_diff(a, b)
-        :param a: = array with LOWER interval limits
-        :param b: = arrays with UPPER interval limits
-            a.shape == b.shape
-            all( a < b )
-        :return: tuple (dll_da, dll_db), where
-            dll_da[...] = d log_cdf_diff[a[...], b[...]) / d a[...]
-            dll_db[...] = d log_cdf_diff[a[...], b[...]) / d b[...]
-            dll_da.shape == dll_db.shape == a.shape == b.shape
-        Arne Leijon, 2017-12-08, tested by finite-diff comparison
-        2018-04-24, include Thurstone.scale factor
-        """
-        def norm_pdf(x):
-            """Gaussian density function = derivative of ndtr(x / scale)
-            """
-            return np.exp(- (x / Thurstone.scale)**2 / 2) / Thurstone.sqrt_2pi / Thurstone.scale
-        # ----------------------------------------------------
-        cdf_diff = Thurstone.cdf_diff(a, b)
-        return - norm_pdf(a) / cdf_diff, norm_pdf(b) / cdf_diff
-
-    def __repr__(self):
-        return '<class Thurstone>'
-
-
-# ------------------------------------------------------------------
 class PairedCompResultSet:
     """Defines probabilistic models for all selected data
     from a paired-comparison experiment.
     """
     def __init__(self, pcf, models, rv_class):
         """Create a PairedCompResultSet from pre-learned attributes.
         :param pcf: single PairedCompFrame instance,
@@ -591,14 +482,15 @@
 
 def _make_population_prior(pcf, null_quality=False):
     """Create a single prior model to be used in all learned models,
     using global scale constants.
 
     :param pcf: single PairedCompFrame object defining experimental layout
     :param null_quality: (optional) boolean => model with all quality params == 0.
+        *** needed only for frequentist hypothesis test, deprecated ***
     :return: single PopulationModel instance (or PopulationNullModel)
 
     Arne Leijon, 2018-07-08, modified for gauss-gamma population model
     2018-11-27, can also generate NULL model for population-model comparison
     """
     nq = pcf.n_quality_params
     # = n quality params
@@ -869,23 +761,23 @@
         # dll_dx[..., self.n_q:] = np.einsum('...m, ...mi -> ...i',
         #                                    dll_db, db_dx)
         dll_dx[..., self.n_q:] = np.sum(dll_db[..., :, None] * db_dx, axis=-2)
         return dll_dx
 
 
 # --------------------------------------------------------------- TEST:
-if __name__ == '__main__':
-
-    a = np.array([2.])
-    # b = np.array([np.inf])
-    b = np.array([3.])
-
-    print('Thurstone log_cdf_diff = ', Thurstone.log_cdf_diff(a, b))
-    (da, db) = Thurstone.d_log_cdf_diff(a, b)
-    print('dll_da =', da)
-    print('dll_db =', db)
-    eps = 1e-6
-    print('approx dll_da: ', (Thurstone.log_cdf_diff(a+eps/2, b) -
-                              Thurstone.log_cdf_diff(a-eps/2, b)) / eps)
-    print('approx dll_db: ', (Thurstone.log_cdf_diff(a, b+eps/2) -
-                              Thurstone.log_cdf_diff(a, b-eps/2)) / eps)
-    # -------------------------------------- OK
+# if __name__ == '__main__':
+#
+#     a = np.array([2.])
+#     # b = np.array([np.inf])
+#     b = np.array([3.])
+#
+#     print('Thurstone log_cdf_diff = ', Thurstone.log_cdf_diff(a, b))
+#     (da, db) = Thurstone.d_log_cdf_diff(a, b)
+#     print('dll_da =', da)
+#     print('dll_db =', db)
+#     eps = 1e-6
+#     print('approx dll_da: ', (Thurstone.log_cdf_diff(a+eps/2, b) -
+#                               Thurstone.log_cdf_diff(a-eps/2, b)) / eps)
+#     print('approx dll_db: ', (Thurstone.log_cdf_diff(a, b+eps/2) -
+#                               Thurstone.log_cdf_diff(a, b-eps/2)) / eps)
+#     # -------------------------------------- OK
```

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_planning.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_planning.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_simulation.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_simulation.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/pc_subject.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/pc_subject.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/run_pc.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/run_pc.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,40 +20,49 @@
 
 * Version 2.0:
 2021-09-13, new function pc_display.display; user interface to select display variants
 """
 from pathlib import Path
 import pickle
 import logging
+import datetime as dt
 
 from PairedCompCalc import pc_logging, __version__
 from PairedCompCalc.pc_data import PairedCompFrame, PairedCompDataSet
 from PairedCompCalc.pc_model import PairedCompResultSet
 from PairedCompCalc.pc_display import PairedCompDisplaySet
 
 # -----------------------------------
-# from PairedCompCalc.pc_model import Bradley
+# from PairedCompCalc.pc_latent import Bradley
 # model_class = Bradley
-from PairedCompCalc.pc_model import Thurstone
+from PairedCompCalc.pc_latent import Thurstone
 model_class = Thurstone
 # = selected class of probabilistic choice model for the analysis
 
 # ---------------------- location of input and output data:
+timestamp_result = True  # New result folder for each run, to prevent over-writing
+# timestamp_result = False  # Repeated runs will over-write existing results
+
 work_path = Path.home() / 'Documents' / 'PairedComp_sim'  # data generated by run_sim.py
 # work_path = Path.home() / 'Documents' / 'My_PairedComp_project'  # or whatever...
 
 data_path = work_path / 'data_sim'
 # = directory to be searched for read-only input data files
 
 result_path = work_path / 'result'
 # = top directory for all result files,
 # with subdirectories created as needed.
 # NOTE: Existing result files in this directory are OVER-WRITTEN WITHOUT WARNING,
 # but different analysis runs may add new result files to the same existing directory.
 
+if timestamp_result:
+    t = dt.datetime.now()
+    result_path = result_path.with_name(result_path.name +
+                                        f'-{t.year}-{t.month:02}-{t.day:02}-{t.hour:02}{t.minute:02}')
+
 assert result_path != data_path, 'Result directory must be different from input data directory'
 
 model_result_file = 'pc_result.pkl'
 # = name of file with saved PairedCompResultSet instance, if used
 
 display_file = 'pc_displays.pkl'
 # = name of file with saved PairedCompDisplaySet instance, if used
```

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/run_plan.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/run_plan.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/run_sim.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/run_sim.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc/safe_logistic.py` & `PairedCompCalc-2.1.1/src/PairedCompCalc/safe_logistic.py`

 * *Files identical despite different names*

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc.egg-info/PKG-INFO` & `PairedCompCalc-2.1.1/src/PairedCompCalc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PairedCompCalc
-Version: 2.1
+Version: 2.1.1
 Summary: Statistical Analysis of Paired-Comparison Data
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: paired-comparison,Bayesian,psycho-physics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PairedCompCalc-2.1/src/PairedCompCalc.egg-info/SOURCES.txt` & `PairedCompCalc-2.1.1/src/PairedCompCalc.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 src/PairedCompCalc/gauss_gamma.py
 src/PairedCompCalc/gauss_gamma_null.py
 src/PairedCompCalc/pc_data.py
 src/PairedCompCalc/pc_display.py
 src/PairedCompCalc/pc_display_format.py
 src/PairedCompCalc/pc_file.py
 src/PairedCompCalc/pc_file_res.py
+src/PairedCompCalc/pc_latent.py
 src/PairedCompCalc/pc_logging.py
-src/PairedCompCalc/pc_lr_test.py
 src/PairedCompCalc/pc_model.py
 src/PairedCompCalc/pc_planning.py
 src/PairedCompCalc/pc_simulation.py
 src/PairedCompCalc/pc_subject.py
 src/PairedCompCalc/run_pc.py
 src/PairedCompCalc/run_plan.py
 src/PairedCompCalc/run_sim.py
```

