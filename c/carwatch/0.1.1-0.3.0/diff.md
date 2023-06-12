# Comparing `tmp/carwatch-0.1.1.tar.gz` & `tmp/carwatch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carwatch-0.1.1.tar", max compression
+gzip compressed data, was "carwatch-0.3.0.tar", max compression
```

## Comparing `carwatch-0.1.1.tar` & `carwatch-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
--rw-r--r--   0        0        0     1100 2023-04-05 12:21:23.085450 carwatch-0.1.1/LICENSE
--rw-r--r--   0        0        0     8293 2023-04-05 12:21:23.085450 carwatch-0.1.1/README.md
--rw-r--r--   0        0        0      233 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/examples/__init__.py
--rw-r--r--   0        0        0      689 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/examples/generate_labels.py
--rw-r--r--   0        0        0      467 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/examples/generate_qr_code.py
--rw-r--r--   0        0        0      181 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/labels/__init__.py
--rw-r--r--   0        0        0      336 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/labels/barcode_template.tex
--rw-r--r--   0        0        0    15114 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/labels/label_generator.py
--rw-r--r--   0        0        0     5594 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/labels/print_layout.py
--rw-r--r--   0        0        0      157 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/qr_codes/__init__.py
--rw-r--r--   0        0        0     5820 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/qr_codes/study_qr_generator.py
--rw-r--r--   0        0        0      619 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/utils/__init__.py
--rw-r--r--   0        0        0     4677 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/utils/click_helper.py
--rw-r--r--   0        0        0     6012 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/utils/study.py
--rw-r--r--   0        0        0     5060 2023-04-05 12:21:23.085450 carwatch-0.1.1/carwatch/utils/utils.py
--rw-r--r--   0        0        0     1898 2023-04-05 12:21:23.089451 carwatch-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9203 1970-01-01 00:00:00.000000 carwatch-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-06-12 08:02:09.937279 carwatch-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8836 2023-06-12 08:02:09.937279 carwatch-0.3.0/README.md
+-rw-r--r--   0        0        0      219 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/__init__.py
+-rw-r--r--   0        0        0     2188 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/example_data.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/examples/__init__.py
+-rw-r--r--   0        0        0      730 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/examples/generate_labels.py
+-rw-r--r--   0        0        0      467 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/examples/generate_qr_code.py
+-rw-r--r--   0        0        0      141 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/labels/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/labels/barcode_template.tex
+-rw-r--r--   0        0        0    14726 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/labels/label_generator.py
+-rw-r--r--   0        0        0     5594 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/labels/print_layout.py
+-rw-r--r--   0        0        0      200 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/logs/__init__.py
+-rw-r--r--   0        0        0    33100 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/logs/_participant_logs.py
+-rw-r--r--   0        0        0     9709 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/logs/_study_logs.py
+-rw-r--r--   0        0        0     1447 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/logs/_utils.py
+-rw-r--r--   0        0        0      157 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/qr_codes/__init__.py
+-rw-r--r--   0        0        0     5801 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/qr_codes/study_qr_generator.py
+-rw-r--r--   0        0        0       77 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/scripts/__init__.py
+-rw-r--r--   0        0        0    13722 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/scripts/prepare_study.py
+-rw-r--r--   0        0        0      616 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/utils/__init__.py
+-rw-r--r--   0        0        0    10124 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/utils/_datatype_validation_helper.py
+-rw-r--r--   0        0        0      335 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/utils/_types.py
+-rw-r--r--   0        0        0     6154 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/utils/click_helper.py
+-rw-r--r--   0        0        0      445 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/utils/exceptions.py
+-rw-r--r--   0        0        0     6319 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/utils/study.py
+-rw-r--r--   0        0        0     5064 2023-06-12 08:02:09.937279 carwatch-0.3.0/carwatch/utils/utils.py
+-rw-r--r--   0        0        0     2556 2023-06-12 08:02:09.949279 carwatch-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10119 1970-01-01 00:00:00.000000 carwatch-0.3.0/PKG-INFO
```

### Comparing `carwatch-0.1.1/LICENSE` & `carwatch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `carwatch-0.1.1/README.md` & `carwatch-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # CARWatch
 
 [![PyPI](https://img.shields.io/pypi/v/carwatch)](https://pypi.org/project/carwatch/)
 ![GitHub](https://img.shields.io/github/license/mad-lab-fau/carwatch)
+[![codecov](https://codecov.io/github/mad-lab-fau/carwatch/branch/main/graph/badge.svg?token=WS66IJ41FU)](https://codecov.io/github/mad-lab-fau/carwatch)
 [![Test and Lint](https://github.com/mad-lab-fau/carwatch/actions/workflows/test-and-lint.yml/badge.svg)](https://github.com/mad-lab-fau/carwatch/actions/workflows/test-and-lint.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/carwatch)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/mad-lab-fau/carwatch)
 
 **Get the Android app on the Play Store:**  
 [![Google Play](https://img.shields.io/badge/Google%20Play-CARWatch-3DDC84?logo=google-play&logoColor=white)](https://play.google.com/store/apps/details?id=de.fau.cs.mad.carwatch)
@@ -14,17 +15,21 @@
 Its primary focus especially, but not limited to, during the **cortisol awakening response (CAR)** in real-world, unsupervised environments.
 It consists of an [Android application](https://github.com/mad-lab-fau/carwatch-app) that schedules sampling times and tracks
 them by scanning a barcode on the respective sampling tube as well as a Python package that provides tools to 
 **configure studies** and **prepare the study materials** and to **process the log data** recorded by the app.
 
 
 ## Features
-In order to use CARWatch, you need to prepare the study materials and configure the app. 
 
-All these features are provided by `carwatch` which offers a  user-friendly command-line interface 
+In order to use CARWatch, you need to prepare the study materials and configure the app. The whole workflow is
+illustrated in the following figure:
+
+<img src="./docs/img/carwarch_overview.png" width="600" alt="CARWatch Workflow">
+
+All these features are provided by `carwatch` which offers a user-friendly command-line interface (CLI)
 for the following tasks: 
 1. **Setting up a CAR study.**   
 This includes: 
    * Customizing study properties to your needs
    * Setting up your desired sampling schedule
    * Generating a QR-Code for the [CARWatch app](https://github.com/mad-lab-fau/carwatch-app) to automatically set up 
    the study in the app
@@ -39,14 +44,16 @@
 This includes:
    * Extracting the sampling timestamps from the log data
    * Extracting the self-reported awakening times (if available)
    * Merging the time information with the cortisol measures
 
 
 
+
+
 ## Installation
 
 `carwatch` requires Python >=3.8. First, install a compatible version of Python 
 (e.g. using [miniconda](https://docs.conda.io/en/latest/miniconda.html)). Then, open a terminal (or Anaconda prompt)
 and install the `carwatch` package via pip:
 
 ```bash
@@ -117,15 +124,16 @@
 custom printing label layout can be specified using the `CustomLayout` class. By default, the 
 [_AveryZweckform J4791_](https://www.avery-zweckform.com/vorlage-j4791) layout is used.   
 To start the PDF generation, call the `generate` method of the `LabelGenerator` class. The output PDF will be exported 
 to the directory specified by `output_dir` (per default: the current working directory).
 
 ```python
 from carwatch.utils import Study
-from carwatch.labels import CustomLayout, LabelGenerator
+from carwatch.labels.print_layout import CustomLayout
+from carwatch.labels.label_generator import LabelGenerator
 
 study = Study(
     study_name="ExampleStudy",
     num_days=3,
     num_subjects=15,
     num_samples=5,
     subject_prefix="VP_",
@@ -174,34 +182,34 @@
 #### Postprocessing Example
 
 To be added
 
 ### Command Line Interface
 
 For the preparation steps, `carwatch` also provides a CLI for more convenient usage.
-To use it, open a terminal session in the `carwatch` directory, and activate the corresponding python environment by
-typing:
+Make sure you installed the `carwatch` package with `pip install carwatch`.
 
+After that, you can simply run the TUI (terminal user interface) by running
 ```
-poetry shell
+prepare_study tui
 ```
+in a terminal session.
 
-Then, start the CLI by typing:
+This will implicitly run the `scripts/prepare_study.py` script, which will guide you through the preparation steps.
+You will then be prompted to enter all the required information step-by-step. The desired output files will 
+be automatically generated for you.
 
+The regular command line interface (CLI) can be used by running
 ```
-python generate_labels.py
+prepare_study run
 ```
 
-You will then be prompted to enter all the required information step-by-step. The desired output files will 
-be automatically generated for you.
-
 For more information about the prompted commands please run:
-
 ```
-python generate_labels.py --help
+prepare_study run --help
 ```
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 ## Contributing
```

### Comparing `carwatch-0.1.1/carwatch/examples/generate_labels.py` & `carwatch-0.3.0/carwatch/examples/generate_labels.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Example of how to generate labels for a study."""
 
-from carwatch.labels import CustomLayout, LabelGenerator
+from carwatch.labels import LabelGenerator
+from carwatch.labels.print_layout import CustomLayout
 from carwatch.utils import Study
 
 if __name__ == "__main__":
     study = Study(
         study_name="ExampleStudy",
         num_days=3,
         num_subjects=15,
@@ -18,8 +19,8 @@
         left_margin=3,
         right_margin=3,
         top_margin=2,
         bottom_margin=2,
         inter_col=0.2,
         inter_row=0.5,
     )
-    generator.generate(output_dir=".", debug=True, layout=layout)
+    generator.generate(output_dir=".", debug=False, layout=layout)
```

### Comparing `carwatch-0.1.1/carwatch/labels/label_generator.py` & `carwatch-0.3.0/carwatch/labels/label_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,52 +21,51 @@
     labels in A4 format. Note that for smaller labels, text overflows might occur.
 
     """
 
     EAN8 = barcode.get_barcode_class("ean8")
     MAX_NAME_LEN = 12
 
-    def __init__(self, study: Study, has_barcode: bool = False, add_name: bool = False, sample_prefix: str = "S"):
+    def __init__(self, study: Study, has_barcode: bool = False, add_name: bool = False):
         """Generate printable PDF files with labels for all biomarker samples taken within a study.
 
         If the parameter ``add_name`` is ``True`` then the text next to the barcode will have the following layout:
         ```
         <study_name>_<subject_id>
-        T<day>_<sample_prefix><sample_id or A for evening sample>
+        D<day>_<study.sample_prefix><sample_id or E for evening sample>
         ```
         For example:
         ```
         ExampleStudy_01
-        T1_S4
+        D1_S4
         ```
 
         If ``add_name`` is set to ``False`` then only the second line is printed:
         ```
-        T<day>_<sample_prefix><sample_id or A for evening sample>
+        D<day>_<study.sample_prefix><sample_id or E for evening sample>
         ```
         For example:
         ```
-        T0_SA
+        D0_SE
         ```
 
         Parameters
         ----------
         study: :obj:`~carwatch.labels.Study`
             Study object for which labels will be created
         has_barcode: bool, optional
             Whether a barcode of type `EAN-8` will be printed on each label
         add_name: bool, optional
             Whether the name of the study will be printed on each label
-        sample_prefix: str, optional
-            Abbreviation of the type of sample taken, default is ``'S'`` for 'Saliva'
 
         Examples
         --------
         Create a Study and print labels for a custom layout
-        >>> from carwatch.labels import LabelGenerator, CustomLayout
+        >>> from carwatch.labels import LabelGenerator
+        >>> from carwatch.labels.print_layout import CustomLayout
         >>> from carwatch.utils import Study
         >>> Study(
         >>>     study_name="ExampleStudy", num_days=3, num_subjects=4, num_samples=5, has_evening_sample=True
         >>> )
         >>> generator = LabelGenerator(study=study, add_name=True, has_barcode=True)
         >>> layout = CustomLayout(
         >>>     num_cols=4, num_rows=10, left_margin=10, right_margin=10,
@@ -74,15 +73,15 @@
         >>> )
         >>> generator.generate(output_dir="./output_labels", layout=layout)
 
         """
         self.study = study
         self.has_barcode = has_barcode
         self.add_name = add_name
-        self.sample_prefix = sanitize_str_for_tex(sample_prefix)
+        self.sample_prefix = sanitize_str_for_tex(self.study.sample_prefix)
         self.output_dir = None
         self.output_name = f"barcodes_{self.study.study_name}"
         self.layout = None
         self.barcode_paths = None
         self.barcodes = None
         self.barcode_ids = None
 
@@ -179,15 +178,15 @@
         barcode_paths = np.array(
             [
                 barcode_object.save(img_path.joinpath(f"barcode_{barcode_id}"), options=options)
                 for barcode_id, barcode_object in zip(self.barcode_ids, self.barcodes)
             ]
         )
         for path in barcode_paths:
-            with open(path, "rb") as file:
+            with Path(path).open(mode="rb") as file:
                 cairosvg.svg2pdf(file_obj=file, write_to=path.replace("svg", "pdf"))
         return barcode_paths
 
     def _create_output_dir(self):
         """Create output directory for intermediate files or clears it (if already exists).
 
         The directory name will be ``{output_dir}/img``.
@@ -248,97 +247,90 @@
             8-digit number of the respective barcode with the format `cpppddss`
             with c: check digit, p: participant id, d: study day, s: biomarker sample
 
         """
         study_name = sanitize_str_for_tex(self.study.study_name)
         day = int(barcode_id // 100) % 100
         sample = barcode_id % 100
-        if self.study.start_sample_from_zero:
-            sample_name = barcode_id % 100
-        else:
-            sample_name = (barcode_id + 1) % 100
+        sample_name = barcode_id % 100 if self.study.start_sample_from_zero else (barcode_id + 1) % 100
         subject_index = int(barcode_id // 1e4)
         subject_name = self.study.subject_names[subject_index - 1]
         subject_name = sanitize_str_for_tex(subject_name)
         # label is realized with latex table
-        label_head = r"\genericlabel" + "\n" + r"\begin{tabular}"
-        label_foot = r"\end{tabular}" + "\n\n"
+        label_head = "\\genericlabel\n\\begin{tabular}"
+        label_foot = "\\end{tabular}\n\n"
         table_content = ""
         if self.has_barcode:
             # create table with 2 columns
-            table_properties = r"{m{0.45\linewidth} m{0.4\linewidth}}" + "\n"
+            table_properties = "{m{0.45\\linewidth} m{0.4\\linewidth}}\n"
             # add barcode to first column
             table_content += (
-                rf"\includegraphics[height={self.layout.get_label_height() - 4}mm,width="
-                + rf"\linewidth,keepaspectratio]{{img/barcode_{subject_index:03d}{day:02d}{sample:02d}.pdf}} &"
+                f"\\includegraphics[height={self.layout.get_label_height() - 4}mm,"
+                f"width=\\linewidth,keepaspectratio]{{img/barcode_{subject_index:03d}{day:02d}{sample:02d}.pdf}} &"
             )
+
             font_size = r"\tiny"  # decrease font size to make it fit next to barcode
         else:
             # create table with only one column
             table_properties = r"{c}"
             font_size = ""  # use default font size
             # center text in label
-            label_head = r"\genericlabel" + "\n" + r"\begin{center}" + "\n" + r"\begin{tabular}"
-            label_foot = r"\end{tabular}" + "\n" + r"\end{center}" + "\n\n"
-        if self.study.has_evening_sample:
-            # if last sample of the day is evening sample, it is marked with "A"
-            if all([sample == self.study.num_samples - 1]):
-                sample_name = "A"
+            label_head = "\\genericlabel\n\\begin{center}\n\\begin{tabular}"
+            label_foot = "\\end{tabular}\n\\end{center}\n\n"
+        if self.study.has_evening_sample and all([sample == self.study.num_samples]):
+            # if last sample of the day is evening sample, it is marked with "E"
+            sample_name = "E"
         if self.add_name:
             delimiter = r"\_"
             if len(study_name) + len(subject_name) > LabelGenerator.MAX_NAME_LEN:
                 # insert linebreak between study name and subject id to prevent overflow
                 delimiter = r"\newline "
             # add study name, subject id, day, and sample to second column
             if self.has_barcode:
                 # insert infos as one row in the second column
                 table_content += (
-                    rf"{font_size}{{{study_name}{delimiter}{subject_name}"
-                    + rf"\newline T{day}\_{self.sample_prefix}{sample_name}}}"
-                    + "\n"
+                    f"{font_size}{{{study_name}{delimiter}{subject_name}"
+                    f"\\newline D{day}\\_{self.sample_prefix}{sample_name}}}\n"
                 )
-            else:
+            elif len(study_name) + len(subject_name) > LabelGenerator.MAX_NAME_LEN:
                 # insert infos centered in two rows
-                if len(study_name) + len(subject_name) > LabelGenerator.MAX_NAME_LEN:
-                    table_content += (
-                        rf"{font_size}{{{study_name}}}\\{{{subject_name}\_T{day}\_{self.sample_prefix}{sample_name}}}"
-                        + "\n"
-                    )
-                else:
-                    table_content += (
-                        rf"{font_size}{{{study_name}\_{subject_name}}}\\{{T{day}\_{self.sample_prefix}{sample_name}}}"
-                        + "\n"
-                    )
+                table_content += (
+                    f"{font_size}{{{study_name}}}\\\\{{{subject_name}\\_D{day}\\_{self.sample_prefix}{sample_name}}}\n"
+                )
+            else:
+                table_content += (
+                    f"{font_size}{{{study_name}\\_{subject_name}}}\\\\{{D{day}\\_{self.sample_prefix}{sample_name}}}\n"
+                )
         else:
             # add day and sample to second column
-            table_content += rf"\centering{font_size}{{T{day}\_{self.sample_prefix}{sample_name}}}" + "\n"
+            table_content += f"\\centering{font_size}{{D{day}\\_{self.sample_prefix}{sample_name}}}\n"
         label_tex = label_head + table_properties + table_content + label_foot
         return label_tex
 
     def _generate_tex_label_properties(self, debug: bool) -> str:
         """Define arrangement of labels based on specified :obj:`~carwatch.labels.PrintLayout`."""
         tex_properties = ""
-        tex_properties += rf"\LabelCols={self.layout.num_cols}" + "\n"  # number of columns of labels per page
-        tex_properties += rf"\LabelRows={self.layout.num_rows}" + "\n"  # number of rows of labels per page
-        tex_properties += rf"\LeftPageMargin={self.layout.left_margin}mm" + "\n"  # margin to the left
-        tex_properties += rf"\RightPageMargin={self.layout.right_margin}mm" + "\n"  # margin to the right
-        tex_properties += rf"\TopPageMargin={self.layout.top_margin}mm" + "\n"  # margin to the top
-        tex_properties += rf"\BottomPageMargin={self.layout.bottom_margin}mm" + "\n"  # margin to the bottom
-        tex_properties += rf"\InterLabelColumn={self.layout.inter_col}mm" + "\n"  # gap between columns of labels
-        tex_properties += rf"\InterLabelRow={self.layout.inter_row}mm" + "\n"  # gap between rows of labels
-        tex_properties += r"\LeftLabelBorder=1mm" + "\n"  # minimum gap between text and label border on the left
-        tex_properties += r"\RightLabelBorder=1mm" + "\n"  # minimum gap between text and label border on the right
-        tex_properties += r"\TopLabelBorder=2mm" + "\n"  # minimum gap between text and label border on the top
-        tex_properties += r"\BottomLabelBorder=2mm" + "\n"  # minimum gap between text and label border on the bottom
+        tex_properties += f"\\LabelCols={self.layout.num_cols}\n"  # number of columns of labels per page
+        tex_properties += f"\\LabelRows={self.layout.num_rows}\n"  # number of rows of labels per page
+        tex_properties += f"\\LeftPageMargin={self.layout.left_margin}mm\n"  # margin to the left
+        tex_properties += f"\\RightPageMargin={self.layout.right_margin}mm\n"  # margin to the right
+        tex_properties += f"\\TopPageMargin={self.layout.top_margin}mm\n"  # margin to the top
+        tex_properties += f"\\BottomPageMargin={self.layout.bottom_margin}mm\n"  # margin to the bottom
+        tex_properties += f"\\InterLabelColumn={self.layout.inter_col}mm\n"  # gap between columns of labels
+        tex_properties += f"\\InterLabelRow={self.layout.inter_row}mm\n"  # gap between rows of labels
+        tex_properties += "\\LeftLabelBorder=1mm\n"  # minimum gap between text and label border on the left
+        tex_properties += "\\RightLabelBorder=1mm\n"  # minimum gap between text and label border on the right
+        tex_properties += "\\TopLabelBorder=2mm\n"  # minimum gap between text and label border on the top
+        tex_properties += "\\BottomLabelBorder=2mm\n"  # minimum gap between text and label border on the bottom
         if debug:
-            tex_properties += r"\LabelGridtrue" + "\n"  # draw label borders
+            tex_properties += "\\LabelGridtrue\n"  # draw label borders
         return tex_properties
 
     def _generate_tex_body(self):
         """Iterate over all barcodes and generate corresponding LaTeX code."""
-        tex_head = r"\begin{labels}" + "\n"
+        tex_head = "\\begin{labels}\n"
         tex_foot = r"\end{labels}"
         tex_body = ""
         for sample in self.barcode_ids:
             # add tex code for every label to body
             tex_body += self._generate_label_tex(int(sample))
         return tex_head + tex_body + tex_foot
```

### Comparing `carwatch-0.1.1/carwatch/labels/print_layout.py` & `carwatch-0.3.0/carwatch/labels/print_layout.py`

 * *Files identical despite different names*

### Comparing `carwatch-0.1.1/carwatch/qr_codes/study_qr_generator.py` & `carwatch-0.3.0/carwatch/qr_codes/study_qr_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module for generating QR codes to configure a study for the CARWatch app."""
 import sys
 from pathlib import Path
-from typing import Sequence, Union
+from typing import Optional, Sequence, Union
 
 import qrcode
 from qrcode.image.pil import PilImage
 
 from carwatch.utils.study import Study
 from carwatch.utils.utils import assert_is_dir, sanitize_str_for_qr
 
@@ -47,36 +47,37 @@
         self.saliva_distances = self._sanitize_distances(saliva_distances)
         self.contact = contact_email
         self.check_duplicates = check_duplicates
         self.enable_manual_scan = enable_manual_scan
         self.output_dir = None
         self.output_name = f"qr_code_{self.study.study_name}"
 
-    def generate(self, output_dir: str = ".", output_name: Union[str, None] = None):
+    def generate(self, output_dir: str = ".", output_name: Optional[str] = None):  # pragma: no cover
         """Generate a `*.png` file with QR code according to the properties of the created ``QrCodeGenerator``.
 
         Parameters
         ----------
         output_dir: str
             Path to the directory where the generated QR-Code will be stored
         output_name: str, optional
-            Filename of the generated QR-Code
+            Filename of the generated QR-Code.
 
         """
         output_dir = Path(output_dir)
+        output_name = Path(output_name)
         try:
             assert_is_dir(output_dir)
         except ValueError as e:
             print(e)
             sys.exit(1)
         self.output_dir = output_dir
         if output_name:
-            if output_name.endswith(".png"):
+            if output_name.suffix == ".png":
                 # store without file ending
-                output_name = output_name.rsplit(".", 1)[0]
+                output_name = output_name.stem
             self.output_name = output_name
         qr_img = self._generate_qr_code()
         self._save_qr_img(qr_img)
 
     def _generate_qr_code(self) -> PilImage:
         """Generate a QR-Code with the study information.
 
@@ -97,51 +98,48 @@
         subject_names = []
         for name in self.study.subject_names:
             sanitized_name = sanitize_str_for_qr(name, forbidden)
             subject_names.append(sanitized_name)
 
         app_id = "CARWATCH"
         name_string = ",".join(str(dist) for dist in subject_names)
+        start_sample = 0 if self.study.start_sample_from_zero else 1
+        start_sample = f"{self.study.sample_prefix}{start_sample}"
         distance_string = ",".join(str(dist) for dist in self.saliva_distances)
 
         # create encoding
         data = (
             f"{app_id};"
             f"N:{study_name};"
             f"D:{self.study.num_days};"
             f"S:{name_string};"
+            f"SS:{start_sample};"
             f"T:{distance_string};"
             f"E:{int(self.study.has_evening_sample)};"
             f"M:{self.contact};"
             f"FD:{int(self.check_duplicates)};"
             f"FM:{int(self.enable_manual_scan)}"
         )
-
         # create qr code
         img = qrcode.make(data)
         return img
 
     def _save_qr_img(self, qr_img):
         img_location = self.output_dir.joinpath(f"{self.output_name}.png")
         qr_img.save(img_location)
 
     def _sanitize_distances(self, saliva_distances: Union[int, Sequence[int]]) -> Sequence[int]:
-        # required number of saliva distances
-        num_morning_samples = self.study.num_samples
-        if self.study.has_evening_sample:
-            # evening sample counts into total number of distances
-            num_morning_samples = num_morning_samples - 1
         if isinstance(saliva_distances, int):
-            return [saliva_distances] * (num_morning_samples - 1)
+            return [saliva_distances] * (self.study.num_samples - 1)
         if isinstance(saliva_distances, list):
             # all elements are ints
             if all(isinstance(dist, int) for dist in saliva_distances):
                 # length is correct
-                if len(saliva_distances) == num_morning_samples - 1:
+                if len(saliva_distances) == self.study.num_samples - 1:
                     return saliva_distances
                 raise ValueError(
                     f"Incorrect number of saliva distances provided! "
-                    f"Needs to be {num_morning_samples - 1}, as "
-                    f"{num_morning_samples} morning samples will be taken."
+                    f"Needs to be {self.study.num_samples - 1}, as "
+                    f"{self.study.num_samples} samples will be taken throughout the day."
                 )
             raise ValueError("Invalid data detected in saliva distances! All values need to be integers!")
         raise ValueError("Saliva distances data type is invalid! Needs to be int or list of ints.")
```

### Comparing `carwatch-0.1.1/carwatch/utils/__init__.py` & `carwatch-0.3.0/carwatch/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This module contains all the utility functions and classes used in the carwatch package."""
+"""Module containing all the utility functions and classes used in the carwatch package."""
 from carwatch.utils.click_helper import Condition, validate_mail_input, validate_saliva_distances, validate_subject_path
 from carwatch.utils.study import Study
 from carwatch.utils.utils import assert_file_ending, assert_is_dir, sanitize_str_for_tex, tex_to_pdf, write_to_file
 
 __all__ = [
     "assert_is_dir",
     "assert_file_ending",
```

### Comparing `carwatch-0.1.1/carwatch/utils/click_helper.py` & `carwatch-0.3.0/carwatch/utils/click_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,14 +32,25 @@
             self.is_positive = True
         else:
             self.condition = kwargs.pop("neg_condition")
             self.is_positive = False
         super().__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
+        """Handle parse result.
+
+        Parameters
+        ----------
+        ctx : :class:`click.Context`
+            the context object
+        opts : dict
+            the options that have been parsed so far
+        args : list
+            the arguments that have been parsed so far
+        """
         is_condition = ctx.params[self.condition]
 
         if not is_condition:
             if self.is_positive:
                 self.prompt = None
             else:
                 self.required = True
@@ -72,51 +83,113 @@
 
         """
         self.option = kwargs.pop("chosen_number")
         self.option_map = kwargs.pop("option_map")
         super().__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
+        """Handle parse result.
+
+        Parameters
+        ----------
+        ctx : :class:`click.Context`
+            the context object
+        opts : dict
+            the options that have been parsed so far
+        args : list
+            the arguments that have been parsed so far
+
+        """
         chosen_number = ctx.params[self.option]
         is_positive = self.option_map[chosen_number]
         if is_positive:
             self.required = True
         else:
             self.prompt = None
         return super().handle_parse_result(ctx, opts, args)
 
 
-def validate_subject_path(ctx, param, value):  # pylint:disable=unused-argument # noqa: C901
+def validate_subject_path(ctx, param, value) -> str:  # noqa: ARG001
+    """Validate subject path.
+
+    Parameters
+    ----------
+    ctx : :class:`click.Context`
+        the context object
+    param : :class:`click.Parameter`
+        the parameter object
+    value : str
+        the value of the parameter
+
+    Returns
+    -------
+    str
+        the validated value of the parameter
+
+    """
     if value:
         try:
             assert_file_ending(Path(value), [".csv", ".txt"])
         except ValueError as e:
-            raise click.BadParameter(str(e))
+            raise click.BadParameter(str(e)) from e
     return value
 
 
-def validate_mail_input(ctx, param, value):  # pylint:disable=unused-argument # noqa: C901
+def validate_mail_input(ctx, param, value):  # noqa: ARG001
+    """Validate mail input.
+
+    Parameters
+    ----------
+    ctx : :class:`click.Context`
+        the context object
+    param : :class:`click.Parameter`
+        the parameter object
+    value : str
+        the value of the parameter
+
+    Returns
+    -------
+    str
+        the validated value of the parameter
+
+    """
     if value:
         email_regex = r"[^@]+@[^@]+\.[^@]+"  # pattern <...>@<...>.<...>
         if not re.fullmatch(email_regex, value):
             raise click.BadParameter(f"{value} is not an email address!")
     return value
 
 
-def validate_saliva_distances(ctx, param, value):  # pylint:disable=unused-argument # noqa: C901
+def validate_saliva_distances(ctx, param, value):  # noqa: ARG001
+    """Validate saliva distances.
+
+    Parameters
+    ----------
+    ctx : :class:`click.Context`
+        the context object
+    param : :class:`click.Parameter`
+        the parameter object
+    value : str
+        the value of the parameter
+
+    Returns
+    -------
+    str
+        the validated value of the parameter
+
+    """
     if value:
         value = value.replace(" ", "")  # trim spaces
         if "," in value:
             distances = value.split(",")
             for dist in distances:
                 if not dist.isdigit():
                     raise click.BadParameter("Saliva distances need to be comma-separated integers!")
-        else:
-            if not value.isdigit():
-                raise click.BadParameter("Saliva distance needs to be an integer!")
+        elif not value.isdigit():
+            raise click.BadParameter("Saliva distance needs to be an integer!")
     return value
 
 
 def get_file_name(suffix: str) -> str:
     """Get file name from click context.
 
     Parameters
```

### Comparing `carwatch-0.1.1/carwatch/utils/study.py` & `carwatch-0.3.0/carwatch/utils/study.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,37 +19,40 @@
         num_days: int,
         num_samples: int,
         num_subjects: Optional[int] = None,
         subject_path: Optional[Union[str, Path]] = None,
         subject_column: Optional[str] = "subject",
         subject_prefix: Optional[str] = None,
         has_evening_sample: bool = False,
+        sample_prefix: Optional[str] = "S",
         start_sample_from_zero: bool = False,
     ):
         """Class that represents a study.
 
         Parameters
         ----------
         study_name: str
             Study name that will be printed on the labels
         num_days: int
             Number of days the study will be conducted
         num_samples: int
-            *Total* number of biomarker samples per day (including a potential evening sample!)
+            Number of biomarker samples per day (*excluding* a potential evening sample!)
         num_subjects: int, optional
             Number of subjects in the study
         subject_path: str or :class:`~pathlib.Path`, optional
             Path to a tabular list of all subjects
         subject_column: str, optional
             Only used when ``subject_path`` is set, specifies the column name containing the subject ids,
             default value is ``"subject"``.
         subject_prefix: str, optional
             Add prefix to participant number (e.g., "VP_")
         has_evening_sample: bool, optional
-            Whether a biomarker sample in the evening is also collected, default is ``False``
+            Whether an *additional* biomarker sample in the evening is collected, default is ``False``
+        sample_prefix: str, optional
+            Abbreviation of the type of sample taken, default is ``'S'`` for 'Saliva'
         start_sample_from_zero: bool, optional
             Whether the ID of the first biomarker sample is 0, default is ``False``
             When set to ``False``, ID starts from 1
 
         """
         self.study_name = study_name
         self.num_days = num_days
@@ -68,14 +71,15 @@
         if self.num_subjects > Study.MAX_NUM_SUBJECTS:
             raise ValueError(f"Sorry, studies with more than {Study.MAX_NUM_SUBJECTS} participants are not supported!")
         # if subject_prefix:
         #     subject_prefix = subject_prefix
         self.subject_prefix = subject_prefix
         self.has_evening_sample = has_evening_sample
         self.start_sample_from_zero = start_sample_from_zero
+        self.sample_prefix = sample_prefix
 
     @staticmethod
     def _determine_subject_ids(subject_path: Union[str, Path], subject_column: str) -> Optional[Sequence[str]]:
         """Extract the IDs of the study participants.
 
         The IDs uf the study participants are extracted depending on the content of the subject data file.
         It is assumed that the subject data contains comma-separated tabular data with a header row.
@@ -96,19 +100,19 @@
         """
         subject_path = Path(subject_path)
         try:
             if assert_file_ending(subject_path, [".csv", ".txt"]):
                 subject_data = pd.read_csv(subject_path)
                 subject_ids = subject_data[subject_column]
                 return subject_ids.to_list()
-            return None
-        # _assert_file_ending throws value error if file has wrong ending/doesn't exist
+            # _assert_file_ending throws value error if file has wrong ending/doesn't exist
         except ValueError as e:
             print(e)
             sys.exit(1)
+        return None
 
     def get_subject_name(self, subject_index: int) -> str:
         """Return the name of a subject.
 
         Parameters
         ----------
         subject_index : int
@@ -121,15 +125,15 @@
 
         """
         if self.subject_path:
             # no prefix or padding used
             return self.subject_ids[subject_index]
         # use padding and prefix if specified
         subject_name_padding = len(str(self.num_subjects))  # length of zero-padding depending on subject count
-        subject_name = f"{subject_index:0{subject_name_padding}d}"
+        subject_name = f"{subject_index+1:0{subject_name_padding}d}"
         if self.subject_prefix:
             subject_name = f"{self.subject_prefix}{subject_name}"
         return subject_name
 
     @property
     def subject_indices(self):
         """Return a list of subject indices.
@@ -172,8 +176,10 @@
 
         Returns
         -------
         list
             list of sample indices
 
         """
+        if self.has_evening_sample:
+            return list(range(0, self.num_samples + 1))
         return list(range(0, self.num_samples))
```

### Comparing `carwatch-0.1.1/carwatch/utils/utils.py` & `carwatch-0.3.0/carwatch/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         path to file that will be written
     content : str
         string that will be inserted to file
 
     """
     # ensure pathlib
     file_name = Path(file)
-    with open(file_name, "w+", encoding="utf-8") as fp:
+    with file_name.open(mode="w+", encoding="utf-8") as fp:
         fp.write(content)
 
 
 def tex_to_pdf(output_dir: Path, tex_file: Union[str, Path]):
     """Run shell command to compile a tex file to a pdf document.
 
     Parameters
```

### Comparing `carwatch-0.1.1/pyproject.toml` & `carwatch-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "carwatch"
-version = "0.1.1"
+version = "0.3.0"
 description = "A Python package for the CARWatch framework to improve cortisol awakening response sampling."
 authors = [
     "Annika Muecke <annika.muecke@fau.de>",
     "Robert Richer <robert.richer@fau.de>",
     "Arne Küderle <arne.kuederle@fau.de>",
     "Luca Abel <luca.abel@fau.de>"
 ]
@@ -17,29 +17,39 @@
 python = ">=3.8, <3.11"
 jupyterlab = "^3.4.5"
 python-barcode = "^0.14.0"
 CairoSVG = "^2.5.2"
 click = "^8.1.3"
 pandas = "^1.5.0"
 qrcode = "^7.3.1"
+matplotlib = { version = "^3.5.0", optional = true }
+seaborn = { version = "^0.11.2", optional = true }
+ipywidgets = {version = "^8", optional = true}
+ipympl = {version = "^0.9", optional = true}
+fau_colors = {version = "^1.6.0", optional=true}
+trogon = "^0.4.0"
+
+[tool.poetry.extras]
+plotting = ["matplotlib", "seaborn", "ipywidgets", "ipympl", "fau_colors"]
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 poethepoet = "^0.16.0"
 pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-prospector = "^1.7.7"
+pytest-cov = "^4.0.0"
+ruff = "^0.0.261"
 ipykernel = "^6.15.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
+target-version = ['py38']
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
     | \.mypy_cache
@@ -50,24 +60,24 @@
     | build
     | dist
     | \.virtual_documents
   )/
 )
 '''
 
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-line_length = 120
-skip_gitignore = true
-
 
 [tool.poe.tasks]
 _format_black = "black ."
-_format_isort = "isort ."
-format = { sequence = ["_format_black", "_format_isort"], help = "Format all files." }
-lint = { cmd = "prospector", help = "Lint all files with Prospector." }
+_format_ruff = "ruff . --fix-only"
+format = { sequence = ["_format_black", "_format_ruff"], help = "Format all files." }
+lint = { cmd = "ruff carwatch --fix", help = "Lint all files with ruff." }
+_lint_ci = "ruff carwatch --format=github"
 _check_black = "black . --check"
-_check_isort = "isort . --check"
-check = { sequence = ["_check_black", "_check_isort", "lint"], help = "Check all potential format and linting issues." }
-test = { cmd = "pytest --cov=carwatch --cov-report=term-missing --cov-report=xml", help = "Run Pytest with coverage." }
+ci_check = { sequence = ["_check_black", "_lint_ci"], help = "Check all potential format and linting issues." }
+test = { cmd = "pytest --cov=carwatch -cov-report=term-missing --cov-report=xml", help = "Run Pytest with coverage." }
 update_version = { script = "_tasks:task_update_version()" }
+register_ipykernel = { cmd = "python -m ipykernel install --user --name carwatch --display-name carwatch", help = "Add a new jupyter kernel for the project." }
+remove_ipykernel = { cmd = "jupyter kernelspec uninstall carwatch", help = "Remove the project specific jupyter kernel."}
+
+
+[tool.poetry.scripts]
+prepare_study = 'carwatch.scripts.prepare_study:run'
```

### Comparing `carwatch-0.1.1/PKG-INFO` & `carwatch-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: carwatch
-Version: 0.1.1
+Version: 0.3.0
 Summary: A Python package for the CARWatch framework to improve cortisol awakening response sampling.
 Home-page: https://github.com/mad-lab-fau/carwatch
 License: MIT
 Author: Annika Muecke
 Author-email: annika.muecke@fau.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: plotting
 Requires-Dist: CairoSVG (>=2.5.2,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: fau_colors (>=1.6.0,<2.0.0) ; extra == "plotting"
+Requires-Dist: ipympl (>=0.9,<0.10) ; extra == "plotting"
+Requires-Dist: ipywidgets (>=8,<9) ; extra == "plotting"
 Requires-Dist: jupyterlab (>=3.4.5,<4.0.0)
+Requires-Dist: matplotlib (>=3.5.0,<4.0.0) ; extra == "plotting"
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: python-barcode (>=0.14.0,<0.15.0)
 Requires-Dist: qrcode (>=7.3.1,<8.0.0)
+Requires-Dist: seaborn (>=0.11.2,<0.12.0) ; extra == "plotting"
+Requires-Dist: trogon (>=0.4.0,<0.5.0)
 Project-URL: Repository, https://github.com/mad-lab-fau/carwatch
 Description-Content-Type: text/markdown
 
 # CARWatch
 
 [![PyPI](https://img.shields.io/pypi/v/carwatch)](https://pypi.org/project/carwatch/)
 ![GitHub](https://img.shields.io/github/license/mad-lab-fau/carwatch)
+[![codecov](https://codecov.io/github/mad-lab-fau/carwatch/branch/main/graph/badge.svg?token=WS66IJ41FU)](https://codecov.io/github/mad-lab-fau/carwatch)
 [![Test and Lint](https://github.com/mad-lab-fau/carwatch/actions/workflows/test-and-lint.yml/badge.svg)](https://github.com/mad-lab-fau/carwatch/actions/workflows/test-and-lint.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/carwatch)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/mad-lab-fau/carwatch)
 
 **Get the Android app on the Play Store:**  
 [![Google Play](https://img.shields.io/badge/Google%20Play-CARWatch-3DDC84?logo=google-play&logoColor=white)](https://play.google.com/store/apps/details?id=de.fau.cs.mad.carwatch)
@@ -37,17 +45,21 @@
 Its primary focus especially, but not limited to, during the **cortisol awakening response (CAR)** in real-world, unsupervised environments.
 It consists of an [Android application](https://github.com/mad-lab-fau/carwatch-app) that schedules sampling times and tracks
 them by scanning a barcode on the respective sampling tube as well as a Python package that provides tools to 
 **configure studies** and **prepare the study materials** and to **process the log data** recorded by the app.
 
 
 ## Features
-In order to use CARWatch, you need to prepare the study materials and configure the app. 
 
-All these features are provided by `carwatch` which offers a  user-friendly command-line interface 
+In order to use CARWatch, you need to prepare the study materials and configure the app. The whole workflow is
+illustrated in the following figure:
+
+<img src="./docs/img/carwarch_overview.png" width="600" alt="CARWatch Workflow">
+
+All these features are provided by `carwatch` which offers a user-friendly command-line interface (CLI)
 for the following tasks: 
 1. **Setting up a CAR study.**   
 This includes: 
    * Customizing study properties to your needs
    * Setting up your desired sampling schedule
    * Generating a QR-Code for the [CARWatch app](https://github.com/mad-lab-fau/carwatch-app) to automatically set up 
    the study in the app
@@ -62,14 +74,16 @@
 This includes:
    * Extracting the sampling timestamps from the log data
    * Extracting the self-reported awakening times (if available)
    * Merging the time information with the cortisol measures
 
 
 
+
+
 ## Installation
 
 `carwatch` requires Python >=3.8. First, install a compatible version of Python 
 (e.g. using [miniconda](https://docs.conda.io/en/latest/miniconda.html)). Then, open a terminal (or Anaconda prompt)
 and install the `carwatch` package via pip:
 
 ```bash
@@ -140,15 +154,16 @@
 custom printing label layout can be specified using the `CustomLayout` class. By default, the 
 [_AveryZweckform J4791_](https://www.avery-zweckform.com/vorlage-j4791) layout is used.   
 To start the PDF generation, call the `generate` method of the `LabelGenerator` class. The output PDF will be exported 
 to the directory specified by `output_dir` (per default: the current working directory).
 
 ```python
 from carwatch.utils import Study
-from carwatch.labels import CustomLayout, LabelGenerator
+from carwatch.labels.print_layout import CustomLayout
+from carwatch.labels.label_generator import LabelGenerator
 
 study = Study(
     study_name="ExampleStudy",
     num_days=3,
     num_subjects=15,
     num_samples=5,
     subject_prefix="VP_",
@@ -197,34 +212,34 @@
 #### Postprocessing Example
 
 To be added
 
 ### Command Line Interface
 
 For the preparation steps, `carwatch` also provides a CLI for more convenient usage.
-To use it, open a terminal session in the `carwatch` directory, and activate the corresponding python environment by
-typing:
+Make sure you installed the `carwatch` package with `pip install carwatch`.
 
+After that, you can simply run the TUI (terminal user interface) by running
 ```
-poetry shell
+prepare_study tui
 ```
+in a terminal session.
 
-Then, start the CLI by typing:
+This will implicitly run the `scripts/prepare_study.py` script, which will guide you through the preparation steps.
+You will then be prompted to enter all the required information step-by-step. The desired output files will 
+be automatically generated for you.
 
+The regular command line interface (CLI) can be used by running
 ```
-python generate_labels.py
+prepare_study run
 ```
 
-You will then be prompted to enter all the required information step-by-step. The desired output files will 
-be automatically generated for you.
-
 For more information about the prompted commands please run:
-
 ```
-python generate_labels.py --help
+prepare_study run --help
 ```
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 ## Contributing
```

