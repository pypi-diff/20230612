# Comparing `tmp/bliss_deblender-0.1.1.tar.gz` & `tmp/bliss_deblender-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bliss_deblender-0.1.1.tar", max compression
+gzip compressed data, was "bliss_deblender-0.2.0.tar", max compression
```

## Comparing `bliss_deblender-0.1.1.tar` & `bliss_deblender-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
--rw-r--r--   0        0        0     1102 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     3823 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/README.md
--rw-r--r--   0        0        0        0 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/__init__.py
--rw-r--r--   0        0        0    27445 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/catalog.py
--rw-r--r--   0        0        0        0 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/datasets/__init__.py
--rw-r--r--   0        0        0     1716 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/datasets/background.py
--rw-r--r--   0        0        0     9082 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/datasets/galsim_galaxies.py
--rw-r--r--   0        0        0     4861 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/datasets/sdss.py
--rw-r--r--   0        0        0     6741 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/datasets/sdss_blended_galaxies.py
--rw-r--r--   0        0        0     4394 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/datasets/simulated.py
--rw-r--r--   0        0        0    11900 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/encoder.py
--rw-r--r--   0        0        0     1730 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/generate.py
--rw-r--r--   0        0        0    11064 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/inference.py
--rw-r--r--   0        0        0        0 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/__init__.py
--rw-r--r--   0        0        0     9696 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/binary.py
--rw-r--r--   0        0        0    24093 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/decoder.py
--rw-r--r--   0        0        0    26191 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/detection_encoder.py
--rw-r--r--   0        0        0     3794 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/encoder_layers.py
--rw-r--r--   0        0        0    15806 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/galaxy_encoder.py
--rw-r--r--   0        0        0     9965 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/galaxy_net.py
--rw-r--r--   0        0        0    18106 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/galsim_decoder.py
--rw-r--r--   0        0        0    14897 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/galsim_encoder.py
--rw-r--r--   0        0        0    14177 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/lens_encoder.py
--rw-r--r--   0        0        0     9833 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/lensing_binary_encoder.py
--rw-r--r--   0        0        0    13984 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/prior.py
--rw-r--r--   0        0        0     5044 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/psf_decoder.py
--rw-r--r--   0        0        0        0 2022-12-10 21:38:15.044870 bliss_deblender-0.1.1/bliss/models/vae/__init__.py
--rw-r--r--   0        0        0     5488 2022-12-10 21:38:15.048870 bliss_deblender-0.1.1/bliss/models/vae/galaxy_flow.py
--rw-r--r--   0        0        0     2199 2022-12-10 21:38:15.048870 bliss_deblender-0.1.1/bliss/models/vae/galaxy_vae.py
--rw-r--r--   0        0        0     1060 2022-12-10 21:38:15.048870 bliss_deblender-0.1.1/bliss/models/vae/prior.py
--rw-r--r--   0        0        0     7646 2022-12-10 21:38:15.048870 bliss_deblender-0.1.1/bliss/plotting.py
--rw-r--r--   0        0        0    19369 2022-12-10 21:38:15.048870 bliss_deblender-0.1.1/bliss/reporting.py
--rwxr-xr-x   0        0        0     5160 2022-12-10 21:38:15.048870 bliss_deblender-0.1.1/bliss/train.py
--rw-r--r--   0        0        0     1893 2022-12-10 21:41:22.752336 bliss_deblender-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 bliss_deblender-0.1.1/setup.py
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 bliss_deblender-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-23 14:00:53.255529 bliss_deblender-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     3815 2023-06-02 15:18:56.594384 bliss_deblender-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 14:00:53.255529 bliss_deblender-0.2.0/bliss/__init__.py
+-rw-r--r--   0        0        0    15704 2023-06-12 20:09:58.928512 bliss_deblender-0.2.0/bliss/api.py
+-rw-r--r--   0        0        0    15923 2023-06-05 14:45:24.369403 bliss_deblender-0.2.0/bliss/catalog.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:09:58.388337 bliss_deblender-0.2.0/bliss/conf/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-02 16:12:28.618668 bliss_deblender-0.2.0/bliss/conf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      608 2023-06-02 16:13:56.845685 bliss_deblender-0.2.0/bliss/conf/__pycache__/igs.cpython-310.pyc
+-rw-r--r--   0        0        0     5089 2023-06-06 20:45:09.947707 bliss_deblender-0.2.0/bliss/conf/base_config.yaml
+-rw-r--r--   0        0        0      377 2023-06-02 16:13:22.930063 bliss_deblender-0.2.0/bliss/conf/igs.py
+-rw-r--r--   0        0        0    11953 2023-06-12 19:30:00.443780 bliss_deblender-0.2.0/bliss/encoder.py
+-rw-r--r--   0        0        0     3855 2023-06-02 15:18:56.598384 bliss_deblender-0.2.0/bliss/generate.py
+-rw-r--r--   0        0        0     8343 2023-05-23 14:00:53.259529 bliss_deblender-0.2.0/bliss/metrics.py
+-rw-r--r--   0        0        0     6499 2023-05-23 14:00:53.259529 bliss_deblender-0.2.0/bliss/plotting.py
+-rw-r--r--   0        0        0     6737 2023-06-12 14:19:07.851845 bliss_deblender-0.2.0/bliss/predict.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/simulator/__init__.py
+-rw-r--r--   0        0        0      157 2023-05-23 19:50:39.942679 bliss_deblender-0.2.0/bliss/simulator/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2968 2023-06-02 16:10:03.460281 bliss_deblender-0.2.0/bliss/simulator/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     7086 2023-06-02 16:15:19.560760 bliss_deblender-0.2.0/bliss/simulator/__pycache__/decoder.cpython-310.pyc
+-rw-r--r--   0        0        0     8499 2023-06-02 16:08:20.485420 bliss_deblender-0.2.0/bliss/simulator/__pycache__/prior.cpython-310.pyc
+-rw-r--r--   0        0        0     8128 2023-06-02 16:15:19.556760 bliss_deblender-0.2.0/bliss/simulator/__pycache__/simulated_dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     2698 2023-06-02 15:18:56.598384 bliss_deblender-0.2.0/bliss/simulator/background.py
+-rw-r--r--   0        0        0     8978 2023-06-02 15:18:56.598384 bliss_deblender-0.2.0/bliss/simulator/decoder.py
+-rw-r--r--   0        0        0    11764 2023-06-02 15:18:56.598384 bliss_deblender-0.2.0/bliss/simulator/prior.py
+-rw-r--r--   0        0        0     8472 2023-06-02 15:18:56.602384 bliss_deblender-0.2.0/bliss/simulator/simulated_dataset.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/surveys/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-23 19:50:39.950679 bliss_deblender-0.2.0/bliss/surveys/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4185 2023-05-25 16:12:09.290263 bliss_deblender-0.2.0/bliss/surveys/__pycache__/decals.cpython-310.pyc
+-rw-r--r--   0        0        0     6648 2023-06-07 14:59:25.957594 bliss_deblender-0.2.0/bliss/surveys/__pycache__/sdss.cpython-310.pyc
+-rw-r--r--   0        0        0     2176 2023-06-08 19:15:21.049829 bliss_deblender-0.2.0/bliss/surveys/__pycache__/sdss_download.cpython-310.pyc
+-rw-r--r--   0        0        0     4644 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/surveys/decals.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/surveys/hst.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/surveys/lsst.py
+-rw-r--r--   0        0        0     7730 2023-06-07 14:59:23.705618 bliss_deblender-0.2.0/bliss/surveys/sdss.py
+-rw-r--r--   0        0        0     2482 2023-06-08 19:14:31.130458 bliss_deblender-0.2.0/bliss/surveys/sdss_download.py
+-rwxr-xr-x   0        0        0     5278 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/train.py
+-rw-r--r--   0        0        0     1820 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/unconstrained_dists.py
+-rw-r--r--   0        0        0     2263 2023-06-12 19:51:19.733301 bliss_deblender-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 bliss_deblender-0.2.0/PKG-INFO
```

### Comparing `bliss_deblender-0.1.1/LICENSE.md` & `bliss_deblender-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bliss_deblender-0.1.1/README.md` & `bliss_deblender-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 BLISS uses state-of-the-art variational inference techniques including
   - __Amortized inference__, in which a neural network maps telescope images to an approximate Bayesian posterior on parameters of interest.
   - __Variational auto-encoders__ (VAEs) to fit a flexible model for galaxy morphology and deblend galaxies.
   - __Wake-sleep algorithm__ to jointly fit the approximate posterior and model parameters such as the PSF and the galaxy VAE.
 
 # Installation
 
-BLISS is pip installable with the following command: 
+BLISS is pip installable with the following command:
 
 ```bash
 pip install bliss-deblender
-``` 
+```
 
 and the required dependencies are listed in the ``[tool.poetry.dependencies]`` block of the ``pyproject.toml`` file.
 
 # Installation (Developers)
 
 1. To use and install `bliss` you first need to install [poetry](https://python-poetry.org/docs/).
 
@@ -45,15 +45,15 @@
 ```bash
 git-lfs install
 ```
 
 4. Now download the bliss repo and fetch some pre-trained models and test data from git-lfs:
 
 ```bash
-git clone https://github.com/prob-ml/bliss.git
+git clone git@github.com:prob-ml/bliss.git
 ```
 
 5. To create a poetry environment with the `bliss` dependencies satisified, run
 
 ```bash
 cd bliss
 poetry install
@@ -66,15 +66,15 @@
 pytest
 pytest --gpu
 ```
 
 7. Finally, if you are planning to contribute code to this repository, consider installing our pre-commit hooks so that your code commits will be checked locally for compliance with our coding conventions:
 
 ```bash
-pre-commit --install
+pre-commit install
 ```
 
 # Latest updates
 ## Galaxies
    - BLISS now includes a galaxy model based on a VAE that was trained on Galsim galaxies.
    - BLISS now includes an algorithm for detecting, measuring, and deblending galaxies.
```

### Comparing `bliss_deblender-0.1.1/bliss/plotting.py` & `bliss_deblender-0.2.0/bliss/surveys/sdss.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,259 +1,214 @@
-"""Common functions to plot results."""
-from abc import abstractmethod
+import os
+import warnings
 from pathlib import Path
-from typing import Optional, Tuple
 
-import matplotlib as mpl
 import numpy as np
-import seaborn as sns
 import torch
-from matplotlib import pyplot as plt
-from matplotlib.figure import Figure
-from matplotlib.pyplot import Axes
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-
-CB_color_cycle = [
-    "#377eb8",
-    "#ff7f00",
-    "#4daf4a",
-    "#f781bf",
-    "#a65628",
-    "#984ea3",
-    "#999999",
-    "#e41a1c",
-    "#dede00",
-]
-
-
-def _to_numpy(d: dict):
-    for k, v in d.items():
-        if isinstance(v, torch.Tensor):
-            d[k] = v.numpy()
-        elif isinstance(v, (float, int, np.ndarray)):
-            d[k] = v
-        elif isinstance(v, dict):
-            v = _to_numpy(v)
-            d[k] = v
-        else:
-            msg = f"Data returned can only be dict, tensor, array, or float but got {type(v)}"
-            raise TypeError(msg)
-    return d
-
-
-def set_rc_params(
-    figsize=(10, 10),
-    fontsize=18,
-    title_size="large",
-    label_size="medium",
-    legend_fontsize="medium",
-    tick_label_size="small",
-    major_tick_size=7,
-    minor_tick_size=4,
-    major_tick_width=0.8,
-    minor_tick_width=0.6,
-    lines_marker_size=8,
-):
-    # named size options: 'xx-small', 'x-small', 'small', 'medium', 'large', 'x-large', 'xx-large'.
-    rc_params = {
-        # font.
-        "font.family": "serif",
-        "font.sans-serif": "Helvetica",
-        "text.usetex": True,
-        "text.latex.preamble": r"\usepackage{amsmath}",
-        "mathtext.fontset": "cm",
-        "font.size": fontsize,
-        # figure
-        "figure.figsize": figsize,
-        # axes
-        "axes.labelsize": label_size,
-        "axes.titlesize": title_size,
-        # ticks
-        "xtick.labelsize": tick_label_size,
-        "ytick.labelsize": tick_label_size,
-        "xtick.major.size": major_tick_size,
-        "ytick.major.size": major_tick_size,
-        "xtick.major.width": major_tick_width,
-        "ytick.major.width": major_tick_width,
-        "ytick.minor.size": minor_tick_size,
-        "xtick.minor.size": minor_tick_size,
-        "xtick.minor.width": minor_tick_width,
-        "ytick.minor.width": minor_tick_width,
-        # markers
-        "lines.markersize": lines_marker_size,
-        # legend
-        "legend.fontsize": legend_fontsize,
-        # colors
-        "axes.prop_cycle": mpl.cycler(color=CB_color_cycle),
-        # images
-        "image.cmap": "gray",
-        "figure.autolayout": True,
+from astropy.io import fits
+from astropy.wcs import WCS, FITSFixedWarning
+from einops import rearrange
+from scipy.interpolate import RegularGridInterpolator
+from torch import Tensor
+from torch.utils.data import Dataset
+
+from bliss.catalog import FullCatalog
+
+
+def convert_mag_to_flux(mag: Tensor, nelec_per_nmgy=987.31) -> Tensor:
+    # default corresponds to average value of columns for run 94, camcol 1, field 12
+    return 10 ** ((22.5 - mag) / 2.5) * nelec_per_nmgy
+
+
+def convert_flux_to_mag(flux: Tensor, nelec_per_nmgy=987.31) -> Tensor:
+    # default corresponds to average value of columns for run 94, camcol 1, field 12
+    return 22.5 - 2.5 * torch.log10(flux / nelec_per_nmgy)
+
+
+def column_to_tensor(table, colname):
+    dtypes = {
+        np.dtype(">i2"): int,
+        np.dtype(">i4"): int,
+        np.dtype(">i8"): int,
+        np.dtype("bool"): bool,
+        np.dtype(">f4"): np.float32,
+        np.dtype(">f8"): np.float32,
+        np.dtype("float32"): np.float32,
+        np.dtype("float64"): np.dtype("float64"),
     }
-    mpl.rcParams.update(rc_params)
-    sns.set_context(rc=rc_params)
+    x = np.array(table[colname])
+    dtype = dtypes[x.dtype]
+    x = x.astype(dtype)
+    return torch.from_numpy(x)
 
 
-class BlissFigure:
+class SloanDigitalSkySurvey(Dataset):
     def __init__(
         self,
-        figdir: str,
-        cachedir: str,
-        overwrite: bool = False,
-        img_format: str = "png",
-    ) -> None:
-
-        self.figdir = Path(figdir)
-        self.cachefile = Path(cachedir) / (self.cache_name + ".pt")
-        self.overwrite = overwrite
-        self.img_format = img_format
-
-    @property
-    def rc_kwargs(self) -> dict:
-        return {}
-
-    @property
-    @abstractmethod
-    def cache_name(self) -> str:
-        """Unique identifier for set of figures including cache."""
-        return "cache_name"
-
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        """Unique identifier for set of figures including cache."""
-        return "bliss_fig"
-
-    @abstractmethod
-    def compute_data(self, *args, **kwargs) -> dict:
-        """Should only return tensors that can be casted to numpy."""
-        return {}
-
-    @abstractmethod
-    def create_figure(self, data) -> Figure:
-        """Return matplotlib figure instances to save based on data."""
-        return {}
-
-    def get_data(self, *args, **kwargs) -> dict:
-        """Return summary of data for producing plot, must be cachable w/ torch.save()."""
-        if self.cachefile.exists() and not self.overwrite:
-            return torch.load(self.cachefile)
-
-        data = self.compute_data(*args, **kwargs)
-        torch.save(data, self.cachefile)
-        return data
-
-    def __call__(self, *args, **kwargs):
-        """Create figures and save to output directory with names from `self.fignames`."""
-        set_rc_params(**self.rc_kwargs)
-        data = self.get_data(*args, **kwargs)
-        data_np = _to_numpy(data)
-        fig: Figure = self.create_figure(data_np)  # data for figures is all numpy arrays or floats.
-        figfile = self.figdir / f"{self.name}.{self.img_format}"
-        fig.savefig(figfile, format=self.img_format)  # pylint: disable=no-member
-        plt.close(fig)
-
-
-def plot_image(
-    fig: Figure,
-    ax: Axes,
-    image: np.ndarray,
-    vrange: Optional[tuple] = None,
-    colorbar: bool = True,
-    cmap="gray",
-) -> None:
-    h, w = image.shape
-    assert h == w
-    vmin = image.min().item() if vrange is None else vrange[0]
-    vmax = image.max().item() if vrange is None else vrange[1]
-
-    if colorbar:
-        divider = make_axes_locatable(ax)
-        cax = divider.append_axes("right", size="5%", pad=0.05)
-    im = ax.matshow(image, vmin=vmin, vmax=vmax, cmap=cmap)
-    if colorbar:
-        fig.colorbar(im, cax=cax, orientation="vertical")
-
-
-def plot_locs(
-    ax: Axes,
-    bp: int,
-    slen: int,
-    plocs: np.ndarray,
-    galaxy_probs: np.ndarray,
-    m: str = "x",
-    s: float = 20,
-    lw: float = 1,
-    alpha: float = 1,
-    annotate=False,
-    cmap: str = "bwr",
-) -> None:
-    n_samples, xy = plocs.shape
-    assert galaxy_probs.shape == (n_samples,) and xy == 2
-
-    x = plocs[:, 1] - 0.5 + bp
-    y = plocs[:, 0] - 0.5 + bp
-    for i, (xi, yi) in enumerate(zip(x, y)):
-        prob = galaxy_probs[i]
-        cmp = mpl.colormaps[cmap]
-        color = cmp(prob)
-        if bp < xi < slen - bp and bp < yi < slen - bp:
-            ax.scatter(xi, yi, color=color, marker=m, s=s, lw=lw, alpha=alpha)
-            if annotate:
-                ax.annotate(f"{galaxy_probs[i]:.2f}", (xi, yi), color=color, fontsize=8)
-
-
-def add_loc_legend(ax: mpl.axes.Axes, labels: list, cmap1="cool", cmap2="bwr", s=20):
-    cmp1 = mpl.colormaps[cmap1]
-    cmp2 = mpl.colormaps[cmap2]
-    colors = (cmp1(1.0), cmp1(0.0), cmp2(1.0), cmp2(0.0))
-    markers = ("+", "+", "x", "x")
-    sizes = (s * 2, s * 2, s + 5, s + 5)
-    for label, c, m, size in zip(labels, colors, markers, sizes):
-        ax.scatter([], [], color=c, marker=m, label=label, s=size)
-    ax.legend(
-        bbox_to_anchor=(0.0, 1.2, 1.0, 0.102),
-        loc="lower left",
-        ncol=2,
-        mode="expand",
-        borderaxespad=0.0,
-    )
-
-
-def scatter_bin_plot(
-    ax: plt.Axes,
-    x: np.ndarray,
-    y: np.ndarray,
-    xlims: Tuple[int, int],
-    delta: float,
-    capsize=5.0,
-    qs=(0.25, 0.75),
-    color="m",
-):
-    # plot median and 25/75 quantiles on each bin decided by delta and xlims.
-    xbins = np.arange(xlims[0], xlims[1], delta)
-
-    xs = np.zeros(len(xbins))
-    ys = np.zeros(len(xbins))
-    errs = np.zeros((len(xbins), 2))
-
-    for i, bx in enumerate(xbins):
-        keep_x = (x > bx) & (x < bx + delta)
-        y_bin: np.ndarray = y[keep_x]
-
-        xs[i] = bx + delta / 2
-
-        if y_bin.shape[0] == 0:
-            ys[i] = np.nan
-            errs[i] = (np.nan, np.nan)
-            continue
-
-        ys[i] = np.median(y_bin)
-        errs[i, :] = ys[i] - np.quantile(y_bin, qs[0]), np.quantile(y_bin, qs[1]) - ys[i]
-
-    errs = errs.T.reshape(2, -1)
-    ax.errorbar(xs, ys, yerr=errs, marker="o", c=color, linestyle="-", capsize=capsize)
-
-
-def make_scatter_contours(ax, x, y):
-    sns.scatterplot(x=x, y=y, s=10, color="0.15", ax=ax)
-    sns.histplot(x=x, y=y, pthresh=0.1, cmap="mako", ax=ax, cbar=True)
-    sns.kdeplot(x=x, y=y, levels=10, color="w", linewidths=1, ax=ax)
+        sdss_dir="data/sdss",
+        run=3900,
+        camcol=6,
+        fields=(269,),
+        bands=(0, 1, 2, 3, 4),
+    ):
+        super().__init__()
+
+        self.sdss_path = Path(sdss_dir)
+        self.rcfgcs = []
+        self.bands = bands
+        pf_file = f"photoField-{run:06d}-{camcol:d}.fits"
+        camcol_path = self.sdss_path.joinpath(str(run), str(camcol))
+        pf_path = camcol_path.joinpath(pf_file)
+        msg = (
+            f"{pf_path} does not exist. "
+            + "Make sure data files are available for specified fields."
+        )
+        assert os.path.exists(pf_path), msg
+        self.pf_fits = fits.getdata(pf_path)
+
+        fieldnums = self.pf_fits["FIELD"]
+        fieldgains = self.pf_fits["GAIN"]
+
+        # get desired field
+        for i, field in enumerate(fieldnums):
+            gain = fieldgains[i]
+            if (not fields) or field in fields:
+                self.rcfgcs.append((run, camcol, field, gain))
+        self.items = [None for _ in range(len(self.rcfgcs))]
+
+    def __len__(self):
+        return len(self.rcfgcs)
+
+    def __getitem__(self, idx):
+        if not self.items[idx]:
+            self.items[idx] = self.get_from_disk(idx)
+        return self.items[idx]
+
+    def get_from_disk(self, idx):
+        if self.rcfgcs[idx] is None:
+            return None
+        run, camcol, field, gain = self.rcfgcs[idx]
+
+        camcol_dir = self.sdss_path.joinpath(str(run), str(camcol))
+        field_dir = camcol_dir.joinpath(str(field))
+        frame_list = []
+
+        for b, bl in enumerate("ugriz"):
+            if b in self.bands:
+                frame = self.read_frame_for_band(bl, field_dir, run, camcol, field, gain[b])
+                frame_list.append(frame)
+
+        ret = {}
+        for k in frame_list[0]:
+            data_per_band = [frame[k] for frame in frame_list]
+            if isinstance(data_per_band[0], np.ndarray):
+                ret[k] = np.stack(data_per_band)
+            else:
+                ret[k] = data_per_band
+        ret.update({"field": field})
+        return ret
+
+    def read_frame_for_band(self, bl, field_dir, run, camcol, field, gain):
+        frame_name = f"frame-{bl}-{run:06d}-{camcol:d}-{field:04d}.fits"
+        frame_path = str(field_dir.joinpath(frame_name))
+        frame = fits.open(frame_path)
+        calibration = frame[1].data  # pylint: disable=maybe-no-member
+        nelec_per_nmgy = gain / calibration
+
+        sky_small = frame[2].data["ALLSKY"][0]  # pylint: disable=maybe-no-member
+        sky_x = frame[2].data["XINTERP"][0]  # pylint: disable=maybe-no-member
+        sky_y = frame[2].data["YINTERP"][0]  # pylint: disable=maybe-no-member
+
+        small_rows = np.mgrid[0 : sky_small.shape[0]]
+        small_cols = np.mgrid[0 : sky_small.shape[1]]
+        small_rcs = (small_rows, small_cols)
+        sky_interp = RegularGridInterpolator(small_rcs, sky_small, method="nearest")
+
+        sky_y = sky_y.clip(0, sky_small.shape[0] - 1)
+        sky_x = sky_x.clip(0, sky_small.shape[1] - 1)
+        large_points = rearrange(np.meshgrid(sky_y, sky_x), "n x y -> y x n")
+        large_sky = sky_interp(large_points)
+        large_sky_nelec = large_sky * gain
+
+        pixels_ss_nmgy = frame[0].data  # pylint: disable=maybe-no-member
+        pixels_ss_nelec = pixels_ss_nmgy * nelec_per_nmgy
+        pixels_nelec = pixels_ss_nelec + large_sky_nelec
+
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=FITSFixedWarning)
+            wcs = WCS(frame[0])
+
+        frame.close()
+        return {
+            "image": pixels_nelec,
+            "background": large_sky_nelec,
+            "gain": np.array(gain),
+            "nelec_per_nmgy_list": nelec_per_nmgy,
+            "calibration": calibration,
+            "wcs": wcs,
+        }
+
+
+class PhotoFullCatalog(FullCatalog):
+    """Class for the SDSS PHOTO Catalog.
+
+    Some resources:
+    - https://www.sdss.org/dr12/algorithms/classify/
+    - https://www.sdss.org/dr12/algorithms/resolve/
+    """
+
+    @classmethod
+    def from_file(cls, sdss_path, run, camcol, field, band):
+        sdss_path = Path(sdss_path)
+        camcol_dir = sdss_path / str(run) / str(camcol) / str(field)
+        po_path = camcol_dir / f"photoObj-{run:06d}-{camcol:d}-{field:04d}.fits"
+        po_fits = fits.getdata(po_path)
+        objc_type = column_to_tensor(po_fits, "objc_type")
+        thing_id = column_to_tensor(po_fits, "thing_id")
+        ras = column_to_tensor(po_fits, "ra")
+        decs = column_to_tensor(po_fits, "dec")
+        galaxy_bools = (objc_type == 3) & (thing_id != -1)
+        star_bools = (objc_type == 6) & (thing_id != -1)
+        star_fluxes = column_to_tensor(po_fits, "psfflux") * star_bools.reshape(-1, 1)
+        star_mags = column_to_tensor(po_fits, "psfmag") * star_bools.reshape(-1, 1)
+        galaxy_fluxes = column_to_tensor(po_fits, "cmodelflux") * galaxy_bools.reshape(-1, 1)
+        galaxy_mags = column_to_tensor(po_fits, "cmodelmag") * galaxy_bools.reshape(-1, 1)
+        fluxes = star_fluxes + galaxy_fluxes
+        mags = star_mags + galaxy_mags
+        keep = galaxy_bools | star_bools
+        galaxy_bools = galaxy_bools[keep]
+        star_bools = star_bools[keep]
+        ras = ras[keep]
+        decs = decs[keep]
+        fluxes = fluxes[keep][:, band]
+        mags = mags[keep][:, band]
+
+        sdss = SloanDigitalSkySurvey(sdss_path, run, camcol, fields=(field,), bands=(band,))
+        wcs: WCS = sdss[0]["wcs"][0]
+
+        # get pixel coordinates
+        pts = []
+        prs = []
+        for ra, dec in zip(ras, decs):
+            pt, pr = wcs.wcs_world2pix(ra, dec, 0)
+            pts.append(float(pt))
+            prs.append(float(pr))
+        pts = torch.tensor(pts) + 0.5  # For consistency with BLISS
+        prs = torch.tensor(prs) + 0.5
+        plocs = torch.stack((prs, pts), dim=-1)
+        nobj = plocs.shape[0]
+
+        d = {
+            "plocs": plocs.reshape(1, nobj, 2),
+            "n_sources": torch.tensor((nobj,)),
+            "galaxy_bools": galaxy_bools.reshape(1, nobj, 1).float(),
+            "star_bools": star_bools.reshape(1, nobj, 1).float(),
+            "fluxes": fluxes.reshape(1, nobj, 1),
+            "mags": mags.reshape(1, nobj, 1),
+            "ra": ras.reshape(1, nobj, 1),
+            "dec": decs.reshape(1, nobj, 1),
+        }
+
+        height = sdss[0]["image"].shape[1]
+        width = sdss[0]["image"].shape[2]
+
+        return cls(height, width, d)
```

### Comparing `bliss_deblender-0.1.1/bliss/train.py` & `bliss_deblender-0.2.0/bliss/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,79 @@
 import datetime as dt
 import json
 from pathlib import Path
 from time import time_ns
-from typing import Any, Dict, Optional
+from typing import Any, Dict
 
 import pytorch_lightning as pl
 import torch
 from hydra.utils import instantiate
 from omegaconf import DictConfig, OmegaConf
 from pytorch_lightning.callbacks import ModelCheckpoint
+from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 from pytorch_lightning.loggers import TensorBoardLogger
 from pytorch_lightning.profiler import AdvancedProfiler
 from pytorch_lightning.utilities import rank_zero_only
 
 
-def train(cfg: DictConfig):
-
+def train(cfg: DictConfig):  # pylint: disable=too-many-branches, too-many-statements
     # setup paths and seed
     paths = OmegaConf.to_container(cfg.paths, resolve=True)
     assert isinstance(paths, dict)
     for key in paths.keys():
         path = Path(paths[key])
         if not path.exists():
             if key == "output":
                 path.mkdir(parents=True)
             else:
                 err = "path for {} ({}) does not exist".format(str(key), path.as_posix())
                 raise FileNotFoundError(err)
     pl.seed_everything(cfg.training.seed)
 
     # setup dataset.
-    dataset = instantiate(cfg.training.dataset)
+    if cfg.training.use_cached_simulator:
+        dataset = instantiate(cfg.cached_simulator)
+    else:
+        dataset = instantiate(cfg.simulator)
 
     # setup model
-    model = instantiate(cfg.training.model, optimizer_params=cfg.training.optimizer_params)
+    encoder = instantiate(cfg.encoder)
+
+    # load pretrained weights
+    if "pretrained_weights" in cfg.training and cfg.training.pretrained_weights is not None:
+        enc_state_dict = torch.load(cfg.training.pretrained_weights)
+        encoder.load_state_dict(enc_state_dict)
 
     # setup trainer
     logger = setup_logger(cfg, paths)
-    checkpoint_callback = setup_callbacks(cfg)
+    checkpoint_callback = setup_checkpoint_callback(cfg)
+    early_stopping = setup_early_stopping(cfg)
     profiler = setup_profiler(cfg)
 
-    callbacks = [] if checkpoint_callback is None else [checkpoint_callback]
+    callbacks = []
+    if checkpoint_callback:
+        callbacks.append(checkpoint_callback)
+    if early_stopping:
+        callbacks.append(early_stopping)
 
     trainer = instantiate(
         cfg.training.trainer, logger=logger, profiler=profiler, callbacks=callbacks
     )
 
     if logger:
-        log_hyperparameters(config=cfg, model=model, trainer=trainer)
+        log_hyperparameters(config=cfg, trainer=trainer)
 
     # train!
     tic = time_ns()
-    trainer.fit(model, datamodule=dataset)
+    trainer.fit(encoder, datamodule=dataset)
     toc = time_ns()
     train_time_sec = (toc - tic) * 1e-9
     # test!
     if cfg.training.testing.file is not None:
-        trainer.test(model, datamodule=dataset)
+        trainer.test(encoder, datamodule=dataset)
 
     # Load best weights from checkpoint
     if cfg.training.weight_save_path is not None and (checkpoint_callback is not None):
         model_checkpoint = torch.load(checkpoint_callback.best_model_path, map_location="cpu")
         model_state_dict = model_checkpoint["state_dict"]
         Path(cfg.training.weight_save_path).parent.mkdir(parents=True, exist_ok=True)
         torch.save(model_state_dict, cfg.training.weight_save_path)
@@ -82,68 +95,58 @@
 
 
 def setup_logger(cfg, paths):
     logger = False
     if cfg.training.trainer.logger:
         logger = TensorBoardLogger(
             save_dir=paths["output"],
-            name=cfg.training.experiment,
+            name=cfg.training.name,
             version=cfg.training.version,
             default_hp_metric=False,
         )
     return logger
 
 
-def setup_callbacks(cfg) -> Optional[ModelCheckpoint]:
+def setup_checkpoint_callback(cfg):
+    checkpoint_callback = None
     if cfg.training.trainer.enable_checkpointing:
         checkpoint_callback = ModelCheckpoint(
             filename="epoch={epoch}-val_loss={val/loss:.3f}",
             save_top_k=cfg.training.save_top_k,
             verbose=True,
             monitor="val/loss",
             mode="min",
             save_on_train_epoch_end=False,
             auto_insert_metric_name=False,
         )
-    else:
-        checkpoint_callback = None
     return checkpoint_callback
 
 
+def setup_early_stopping(cfg):
+    early_stopping = None
+    if cfg.training.enable_early_stopping:
+        early_stopping = EarlyStopping(
+            monitor="val/loss", mode="min", patience=cfg.training.patience
+        )
+    return early_stopping
+
+
 def setup_profiler(cfg):
     profiler = None
     if cfg.training.trainer.profiler:
         profiler = AdvancedProfiler(filename="profile.txt")
     return profiler
 
 
 # https://github.com/ashleve/lightning-hydra-template/blob/main/src/utils/utils.py
 @rank_zero_only
-def log_hyperparameters(config, model, trainer) -> None:
-    """Log config and num of model parameters to all Lightning loggers."""
-
-    hparams = {}
-
-    # choose which parts of hydra config will be saved to loggers
-    hparams["mode"] = config["mode"]
-    hparams["training"] = config["training"]
-    hparams["optimizer"] = config["training"]["optimizer_params"]
-
-    # save number of model parameters
-    hparams["model/params_total"] = sum(p.numel() for p in model.parameters())
-    hparams["model/params_trainable"] = sum(
-        p.numel() for p in model.parameters() if p.requires_grad
-    )
-    hparams["model/params_not_trainable"] = sum(
-        p.numel() for p in model.parameters() if not p.requires_grad
-    )
-
+def log_hyperparameters(config, trainer) -> None:
+    """Log config to all Lightning loggers."""
     # send hparams to all loggers
-    trainer.logger.log_hyperparams(hparams)
-
+    trainer.logger.log_hyperparams(config)
     # trick to disable logging any more hyperparameters for all loggers
     trainer.logger.log_hyperparams = empty
 
 
 def empty(*args, **kwargs):
     pass
```

### Comparing `bliss_deblender-0.1.1/pyproject.toml` & `bliss_deblender-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,68 +14,81 @@
 documentation = "https://prob-ml.github.io/bliss/"
 keywords = ["cosmology", "blending", "weak lensing", "bayesian", "ml", "pytorch"]
 license = "MIT"
 name = "bliss-deblender"
 packages = [{include = "bliss"}]
 readme = "README.md"
 repository = "https://github.com/prob-ml/bliss"
-version = "0.1.1"
+version = "0.2.0"
+
+[tool.poetry.scripts]
+bliss = "main:main"
 
 [tool.poetry.dependencies]
 astropy = ">=4.2.1"
 einops = ">=0.3.0"
 galsim = ">=2.2.4"
 hydra-core = ">=1.0.4"
 matplotlib = ">=3.3.3"
 nflows = ">=0.14"
 numpy = ">=1.18.5"
-python = "^3.8"
-pytorch-lightning = ">=1.5.1"
+python = "^3.10"
+pytorch-lightning = ">=1.9"
 scikit-learn = ">=0.24.2"
 scipy = ">=1.4.1"
 seaborn = ">=0.11.2"
 torch = ">=1.9"
 torchmetrics = ">=0.5.1"
+yolov5 = "^7.0.9"
+bokeh = "^3.1.1"
+requests = "^2.31.0"
+types-requests = "^2.31.0.1"
 
 [tool.poetry.dev-dependencies]
 Cython = ">=0.29.21"
 Sphinx = ">=4.0.2"
 black = ">=22.3.0"
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
 flake8-docstrings = ">=1.6.0"
 git-lfs = ">=1.6"
+ipykernel = "^6.21.0"
 isort = ">=5.9.3"
 jupyter = ">=1.0.0"
 jupyter_contrib_nbextensions = ">=0.5.1"
 nbstripout = ">=0.5.0"
 plotly = ">=4.14.3"
 pre-commit = ">=2.9.2"
+pre-commit-hooks = "^4.4.0"
 pylint = ">=2.6.0"
 pytest = ">=6.1.2"
 pytest-cov = ">=2.10"
 pytest-mypy = ">=0.9.1"
 sphinx-rtd-theme = ">=0.5.2"
+torch-tb-profiler = "^0.4.1"
 tqdm = ">=4.62.3"
 wemake-python-styleguide = ">=0.16.1"
+nbsphinx = "^0.9.2"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.black]
 line-length = 100
-target-version = ['py38']
+target-version = ['py310']
 
 # pyproject.toml
 [tool.pytest.ini_options]
 addopts = "-ra"
 filterwarnings = [
   "ignore:.*does not have many workers which may be a bottleneck.*:UserWarning",
   "ignore:GPU available but not used.*:UserWarning",
   "ignore:numpy.ndarray size changed:RuntimeWarning",
   "ignore:.*when logging on epoch level in distributed setting.*",
+  "ignore:.*pkg_resources.declare_namespace.*:DeprecationWarning",
+  "ignore:.*distutils Version classes are deprecated.*:DeprecationWarning",
 ]
 minversion = "6.0"
 testpaths = [
   "tests",
 ]
```

### Comparing `bliss_deblender-0.1.1/PKG-INFO` & `bliss_deblender-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: bliss-deblender
-Version: 0.1.1
+Version: 0.2.0
 Summary: Bayesian Light Source Separator
 Home-page: https://github.com/prob-ml/bliss
 License: MIT
 Keywords: cosmology,blending,weak lensing,bayesian,ml,pytorch
 Author: Ismael Mendoza
 Author-email: imendoza@umich.edu
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astropy (>=4.2.1)
+Requires-Dist: bokeh (>=3.1.1,<4.0.0)
 Requires-Dist: einops (>=0.3.0)
 Requires-Dist: galsim (>=2.2.4)
 Requires-Dist: hydra-core (>=1.0.4)
 Requires-Dist: matplotlib (>=3.3.3)
 Requires-Dist: nflows (>=0.14)
 Requires-Dist: numpy (>=1.18.5)
-Requires-Dist: pytorch-lightning (>=1.5.1)
+Requires-Dist: pytorch-lightning (>=1.9)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scikit-learn (>=0.24.2)
 Requires-Dist: scipy (>=1.4.1)
 Requires-Dist: seaborn (>=0.11.2)
 Requires-Dist: torch (>=1.9)
 Requires-Dist: torchmetrics (>=0.5.1)
+Requires-Dist: types-requests (>=2.31.0.1,<3.0.0.0)
+Requires-Dist: yolov5 (>=7.0.9,<8.0.0)
 Project-URL: Documentation, https://prob-ml.github.io/bliss/
 Project-URL: Repository, https://github.com/prob-ml/bliss
 Description-Content-Type: text/markdown
 
 ![](http://portal.nersc.gov/project/dasrepo/celeste/sample_sky.jpg)
 
 
@@ -51,19 +53,19 @@
 BLISS uses state-of-the-art variational inference techniques including
   - __Amortized inference__, in which a neural network maps telescope images to an approximate Bayesian posterior on parameters of interest.
   - __Variational auto-encoders__ (VAEs) to fit a flexible model for galaxy morphology and deblend galaxies.
   - __Wake-sleep algorithm__ to jointly fit the approximate posterior and model parameters such as the PSF and the galaxy VAE.
 
 # Installation
 
-BLISS is pip installable with the following command: 
+BLISS is pip installable with the following command:
 
 ```bash
 pip install bliss-deblender
-``` 
+```
 
 and the required dependencies are listed in the ``[tool.poetry.dependencies]`` block of the ``pyproject.toml`` file.
 
 # Installation (Developers)
 
 1. To use and install `bliss` you first need to install [poetry](https://python-poetry.org/docs/).
 
@@ -78,15 +80,15 @@
 ```bash
 git-lfs install
 ```
 
 4. Now download the bliss repo and fetch some pre-trained models and test data from git-lfs:
 
 ```bash
-git clone https://github.com/prob-ml/bliss.git
+git clone git@github.com:prob-ml/bliss.git
 ```
 
 5. To create a poetry environment with the `bliss` dependencies satisified, run
 
 ```bash
 cd bliss
 poetry install
@@ -99,15 +101,15 @@
 pytest
 pytest --gpu
 ```
 
 7. Finally, if you are planning to contribute code to this repository, consider installing our pre-commit hooks so that your code commits will be checked locally for compliance with our coding conventions:
 
 ```bash
-pre-commit --install
+pre-commit install
 ```
 
 # Latest updates
 ## Galaxies
    - BLISS now includes a galaxy model based on a VAE that was trained on Galsim galaxies.
    - BLISS now includes an algorithm for detecting, measuring, and deblending galaxies.
```

