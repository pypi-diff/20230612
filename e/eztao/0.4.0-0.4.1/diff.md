# Comparing `tmp/eztao-0.4.0.tar.gz` & `tmp/eztao-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztao-0.4.0.tar", max compression
+gzip compressed data, was "eztao-0.4.1.tar", max compression
```

## Comparing `eztao-0.4.0.tar` & `eztao-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2021-07-20 01:08:06.506228 eztao-0.4.0/LICENSE
--rw-r--r--   0        0        0     3351 2021-07-20 01:08:06.506228 eztao-0.4.0/README.md
--rw-r--r--   0        0        0      895 2021-07-20 01:08:06.530230 eztao-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      325 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/__init__.py
--rw-r--r--   0        0        0    15796 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/carma/CARMATerm.py
--rw-r--r--   0        0        0      108 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/carma/__init__.py
--rw-r--r--   0        0        0     4005 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/carma/model_utils.py
--rw-r--r--   0        0        0       99 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/ts/__init__.py
--rw-r--r--   0        0        0    21496 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/ts/carma_fit.py
--rw-r--r--   0        0        0     3130 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/ts/carma_mcmc.py
--rw-r--r--   0        0        0     8990 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/ts/carma_sim.py
--rw-r--r--   0        0        0     3640 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/ts/utils.py
--rw-r--r--   0        0        0      190 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/viz/__init__.py
--rw-r--r--   0        0        0    40312 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/viz/eztao.rc
--rw-r--r--   0        0        0    11048 2021-07-20 01:08:06.530230 eztao-0.4.0/src/eztao/viz/mpl_viz.py
--rw-r--r--   0        0        0     4332 2021-07-20 01:08:26.217205 eztao-0.4.0/setup.py
--rw-r--r--   0        0        0     4182 2021-07-20 01:08:26.217782 eztao-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-12 17:41:51.246025 eztao-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4407 2023-06-12 17:41:51.246025 eztao-0.4.1/README.md
+-rw-r--r--   0        0        0      894 2023-06-12 17:41:51.266025 eztao-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/__init__.py
+-rw-r--r--   0        0        0    15789 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/carma/CARMATerm.py
+-rw-r--r--   0        0        0      108 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/carma/__init__.py
+-rw-r--r--   0        0        0     3999 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/carma/model_utils.py
+-rw-r--r--   0        0        0       99 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/ts/__init__.py
+-rw-r--r--   0        0        0    21645 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/ts/carma_fit.py
+-rw-r--r--   0        0        0     3130 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/ts/carma_mcmc.py
+-rw-r--r--   0        0        0     8990 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/ts/carma_sim.py
+-rw-r--r--   0        0        0     3682 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/ts/utils.py
+-rw-r--r--   0        0        0      190 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/viz/__init__.py
+-rw-r--r--   0        0        0    40312 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/viz/eztao.rc
+-rw-r--r--   0        0        0    11048 2023-06-12 17:41:51.266025 eztao-0.4.1/src/eztao/viz/mpl_viz.py
+-rw-r--r--   0        0        0     5413 1970-01-01 00:00:00.000000 eztao-0.4.1/setup.py
+-rw-r--r--   0        0        0     5339 1970-01-01 00:00:00.000000 eztao-0.4.1/PKG-INFO
```

### Comparing `eztao-0.4.0/LICENSE` & `eztao-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eztao-0.4.0/README.md` & `eztao-0.4.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -4,207 +4,273 @@
 00000030: 6f72 6b66 6c6f 7773 2f74 6573 7473 2f62  orkflows/tests/b
 00000040: 6164 6765 2e73 7667 290a 5b21 5b42 696e  adge.svg).[![Bin
 00000050: 6465 725d 2868 7474 7073 3a2f 2f6d 7962  der](https://myb
 00000060: 696e 6465 722e 6f72 672f 6261 6467 655f  inder.org/badge_
 00000070: 6c6f 676f 2e73 7667 295d 2868 7474 7073  logo.svg)](https
 00000080: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
 00000090: 7632 2f67 682f 7977 7836 3439 3939 3933  v2/gh/ywx6499993
-000000a0: 3131 2f45 7a54 616f 2f76 302e 342e 303f  11/EzTao/v0.4.0?
+000000a0: 3131 2f45 7a54 616f 2f76 302e 342e 313f  11/EzTao/v0.4.1?
 000000b0: 6669 6c65 7061 7468 3d64 6f63 732f 6e6f  filepath=docs/no
 000000c0: 7465 626f 6f6b 7329 0a5b 215b 446f 6375  tebooks).[![Docu
 000000d0: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
 000000e0: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
 000000f0: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
 00000100: 7473 2f65 7a74 616f 2f62 6164 6765 2f3f  ts/eztao/badge/?
 00000110: 7665 7273 696f 6e3d 6c61 7465 7374 295d  version=latest)]
 00000120: 2868 7474 7073 3a2f 2f65 7a74 616f 2e72  (https://eztao.r
 00000130: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000140: 2f6c 6174 6573 742f 290a 2320 457a 5461  /latest/).# EzTa
-00000150: 6f20 28e6 9893 e981 9329 0a2a 2a45 7a54  o (......).**EzT
-00000160: 616f 2a2a 2069 7320 6120 746f 6f6c 6b69  ao** is a toolki
-00000170: 7420 666f 7220 636f 6e64 7563 7469 6e67  t for conducting
-00000180: 2041 474e 2074 696d 652d 7365 7269 6573   AGN time-series
-00000190: 2f76 6172 6961 6269 6c69 7479 2061 6e61  /variability ana
-000001a0: 6c79 7369 732c 206d 6169 6e6c 7920 7574  lysis, mainly ut
-000001b0: 696c 697a 696e 6720 7468 6520 636f 6e74  ilizing the cont
-000001c0: 696e 756f 7573 2d74 696d 6520 6175 746f  inuous-time auto
-000001d0: 2d72 6567 7265 7373 6976 6520 6d6f 7669  -regressive movi
-000001e0: 6e67 2061 7665 7261 6765 206d 6f64 656c  ng average model
-000001f0: 2028 4341 524d 4129 0a0a 2323 2049 6e73   (CARMA)..## Ins
-00000200: 7461 6c6c 6174 696f 6e0a 6060 600a 7069  tallation.```.pi
-00000210: 7020 696e 7374 616c 6c20 657a 7461 6f0a  p install eztao.
-00000220: 6060 600a 6f72 2028 6672 6f6d 206d 6173  ```.or (from mas
-00000230: 7465 7229 0a60 6060 0a70 6970 2069 6e73  ter).```.pip ins
-00000240: 7461 6c6c 2067 6974 2b68 7474 7073 3a2f  tall git+https:/
-00000250: 2f67 6974 6875 622e 636f 6d2f 7977 7836  /github.com/ywx6
-00000260: 3439 3939 3933 3131 2f45 7a54 616f 2e67  49999311/EzTao.g
-00000270: 6974 0a60 6060 0a23 2323 2044 6570 656e  it.```.### Depen
-00000280: 6465 6e63 6965 730a 3e60 6060 0a3e 7079  dencies.>```.>py
-00000290: 7468 6f6e 203d 2022 5e33 2e37 220a 3e63  thon = "^3.7".>c
-000002a0: 656c 6572 6974 6520 3d20 223e 3d20 302e  elerite = ">= 0.
-000002b0: 332e 3022 0a3e 6d61 7470 6c6f 746c 6962  3.0".>matplotlib
-000002c0: 203d 2022 5e33 2e33 2e30 220a 3e73 6369   = "^3.3.0".>sci
-000002d0: 7079 203d 2022 3e20 312e 352e 3022 0a3e  py = "> 1.5.0".>
-000002e0: 6e75 6d62 6120 3d20 223e 3d20 302e 3531  numba = ">= 0.51
-000002f0: 2e30 220a 3e65 6d63 6565 203d 2022 3e3d  .0".>emcee = ">=
-00000300: 332e 302e 3022 0a3e 6060 600a 0a23 2323  3.0.0".>```..###
-00000310: 2051 7569 636b 2045 7861 6d70 6c65 730a   Quick Examples.
-00000320: 4c65 7427 7320 6669 7273 7420 7369 6d75  Let's first simu
-00000330: 6c61 7465 2061 2044 5257 2f43 4152 4d41  late a DRW/CARMA
-00000340: 2831 2c30 2920 7072 6f63 6573 7320 7769  (1,0) process wi
-00000350: 7468 2061 2076 6172 6961 6e63 6520 6f66  th a variance of
-00000360: 2030 2e33 5e32 2061 6e64 2061 2072 656c   0.3^2 and a rel
-00000370: 6178 6174 696f 6e20 7469 6d65 7363 616c  axation timescal
-00000380: 6520 6f66 2031 3030 2064 6179 732e 2054  e of 100 days. T
-00000390: 6869 7320 7469 6d65 2073 6572 6965 7320  his time series 
-000003a0: 7769 6c6c 2068 6176 6520 6120 746f 7461  will have a tota
-000003b0: 6c20 6f66 2032 3030 2064 6174 6120 706f  l of 200 data po
-000003c0: 696e 7473 2061 6e64 2073 7061 6e20 3130  ints and span 10
-000003d0: 2079 6561 7273 2e0a 6060 6070 7974 686f   years..```pytho
-000003e0: 6e0a 696d 706f 7274 206e 756d 7079 2061  n.import numpy a
-000003f0: 7320 6e70 0a69 6d70 6f72 7420 6d61 7470  s np.import matp
-00000400: 6c6f 746c 6962 2e70 7970 6c6f 7420 6173  lotlib.pyplot as
-00000410: 2070 6c74 0a66 726f 6d20 657a 7461 6f2e   plt.from eztao.
-00000420: 6361 726d 6120 696d 706f 7274 2044 5257  carma import DRW
-00000430: 5f74 6572 6d0a 6672 6f6d 2065 7a74 616f  _term.from eztao
-00000440: 2e74 7320 696d 706f 7274 2067 7053 696d  .ts import gpSim
-00000450: 5261 6e64 0a0a 2320 6465 6669 6e65 2061  Rand..# define a
-00000460: 2044 5257 206b 6572 6e65 6c20 2620 616e   DRW kernel & an
-00000470: 6420 7369 6d75 6c61 7465 2061 2070 726f  d simulate a pro
-00000480: 6365 7373 0a61 6d70 203d 2030 2e32 0a74  cess.amp = 0.2.t
-00000490: 6175 203d 2031 3030 0a44 5257 5f6b 6572  au = 100.DRW_ker
-000004a0: 6e65 6c20 3d20 4452 575f 7465 726d 286e  nel = DRW_term(n
-000004b0: 702e 6c6f 6728 616d 7029 2c20 6e70 2e6c  p.log(amp), np.l
-000004c0: 6f67 2874 6175 2929 0a74 2c20 792c 2079  og(tau)).t, y, y
-000004d0: 6572 7220 3d20 6770 5369 6d52 616e 6428  err = gpSimRand(
-000004e0: 4452 575f 6b65 726e 656c 2c20 3130 2c20  DRW_kernel, 10, 
-000004f0: 3336 352a 3130 2c20 3230 3029 0a0a 2320  365*10, 200)..# 
-00000500: 6e6f 772c 2070 6c6f 7420 6974 0a66 6967  now, plot it.fig
-00000510: 2c20 6178 203d 2070 6c74 2e73 7562 706c  , ax = plt.subpl
-00000520: 6f74 7328 312c 312c 2064 7069 3d31 3530  ots(1,1, dpi=150
-00000530: 2c20 6669 6773 697a 653d 2838 2c33 2929  , figsize=(8,3))
-00000540: 0a61 782e 6572 726f 7262 6172 2874 2c20  .ax.errorbar(t, 
-00000550: 792c 2079 6572 722c 2066 6d74 3d27 2e27  y, yerr, fmt='.'
-00000560: 290a 2e2e 2e0a 6060 600a 215b 6472 775f  ).....```.![drw_
-00000570: 7369 6d5d 2869 6e63 6c75 6465 2f64 7277  sim](include/drw
-00000580: 5f73 696d 2e70 6e67 290a 0a57 6520 6361  _sim.png)..We ca
-00000590: 6e20 6669 7420 7468 6520 7369 6d75 6c61  n fit the simula
-000005a0: 7465 6420 7469 6d65 2073 6572 6965 7320  ted time series 
-000005b0: 746f 2074 6865 2044 5257 206d 6f64 656c  to the DRW model
-000005c0: 2061 6e64 2073 6565 2068 6f77 2077 656c   and see how wel
-000005d0: 6c20 7765 2063 616e 2072 6563 6f76 6572  l we can recover
-000005e0: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
-000005f0: 6574 6572 732e 0a60 6060 7079 7468 6f6e  eters..```python
-00000600: 0a66 726f 6d20 657a 7461 6f2e 7473 2069  .from eztao.ts i
-00000610: 6d70 6f72 7420 6472 775f 6669 740a 0a62  mport drw_fit..b
-00000620: 6573 745f 6669 7420 3d20 6472 775f 6669  est_fit = drw_fi
-00000630: 7428 742c 2079 2c20 7965 7272 290a 7072  t(t, y, yerr).pr
-00000640: 696e 7428 6627 4265 7374 2d66 6974 2044  int(f'Best-fit D
-00000650: 5257 2070 6172 616d 6574 6572 733a 207b  RW parameters: {
-00000660: 6265 7374 5f66 6974 7d27 290a 6060 600a  best_fit}').```.
-00000670: 6060 6073 6865 6c6c 0a42 6573 742d 6669  ```shell.Best-fi
-00000680: 7420 4452 5720 7061 7261 6d65 7465 7273  t DRW parameters
-00000690: 3a20 5b30 2e31 3733 3536 3938 3320 3838  : [0.17356983 88
-000006a0: 2e33 3632 3632 3436 375d 0a60 6060 0a0a  .36262467].```..
-000006b0: 486f 7720 646f 6573 2074 6865 2070 6f77  How does the pow
-000006c0: 6572 2073 7065 6374 7275 6d20 6465 6e73  er spectrum dens
-000006d0: 6974 7920 2850 5344 2920 636f 6d70 6172  ity (PSD) compar
-000006e0: 653f 0a60 6060 7079 7468 6f6e 0a66 726f  e?.```python.fro
-000006f0: 6d20 657a 7461 6f2e 6361 726d 6120 696d  m eztao.carma im
-00000700: 706f 7274 2067 705f 7073 640a 0a23 2067  port gp_psd..# g
-00000710: 6574 2070 7364 2066 756e 6374 696f 6e73  et psd functions
-00000720: 0a74 7275 655f 7073 6420 3d20 6770 5f70  .true_psd = gp_p
-00000730: 7364 2844 5257 5f6b 6572 6e65 6c29 0a62  sd(DRW_kernel).b
-00000740: 6573 745f 7073 6420 3d20 6770 5f70 7364  est_psd = gp_psd
-00000750: 2844 5257 5f74 6572 6d28 2a6e 702e 6c6f  (DRW_term(*np.lo
-00000760: 6728 6265 7374 5f66 6974 2929 290a 0a23  g(best_fit)))..#
-00000770: 2070 6c6f 740a 6669 672c 2061 7820 3d20   plot.fig, ax = 
-00000780: 706c 742e 7375 6270 6c6f 7473 2831 2c31  plt.subplots(1,1
-00000790: 2c20 6470 693d 3135 302c 2066 6967 7369  , dpi=150, figsi
-000007a0: 7a65 3d28 362c 3329 290a 6672 6571 203d  ze=(6,3)).freq =
-000007b0: 206e 702e 6c6f 6773 7061 6365 282d 352c   np.logspace(-5,
-000007c0: 2032 290a 6178 2e70 6c6f 7428 6672 6571   2).ax.plot(freq
-000007d0: 2c20 7472 7565 5f70 7364 2866 7265 7129  , true_psd(freq)
-000007e0: 2c20 6c61 6265 6c3d 2749 6e70 7574 2050  , label='Input P
-000007f0: 5344 2729 0a61 782e 706c 6f74 2866 7265  SD').ax.plot(fre
-00000800: 712c 2062 6573 745f 7073 6428 6672 6571  q, best_psd(freq
-00000810: 292c 206c 6162 656c 3d27 4265 7374 2d66  ), label='Best-f
-00000820: 6974 2050 5344 2729 0a2e 2e2e 0a60 6060  it PSD').....```
-00000830: 0a21 5b64 7277 5f70 7364 5d28 696e 636c  .![drw_psd](incl
-00000840: 7564 652f 6472 775f 7073 642e 706e 6729  ude/drw_psd.png)
-00000850: 0a0a 5f5f 4e6f 7465 3a5f 5f20 486f 7720  ..__Note:__ How 
-00000860: 7765 6c6c 2074 6865 2069 6e70 7574 2061  well the input a
-00000870: 6e64 2062 6573 742d 6669 7420 5053 4420  nd best-fit PSD 
-00000880: 6d61 7463 6820 6973 2075 7020 746f 2068  match is up to h
-00000890: 6f77 2067 6f6f 6420 7468 6520 6265 7374  ow good the best
-000008a0: 2d66 6974 2070 6172 616d 6574 6572 7320  -fit parameters 
-000008b0: 6172 652c 2077 6869 6368 2069 7320 6869  are, which is hi
-000008c0: 6768 6c79 2069 6e66 6c75 656e 6365 6420  ghly influenced 
-000008d0: 6279 2074 6865 2071 7561 6c69 7479 206f  by the quality o
-000008e0: 6620 7468 6520 696e 7075 7420 7469 6d65  f the input time
-000008f0: 2073 6572 6965 732e 200a 0a46 6f72 206d   series. ..For m
-00000900: 6f72 6520 6578 616d 706c 6573 2c20 706c  ore examples, pl
-00000910: 6561 7365 2063 6865 636b 206f 7574 2074  ease check out t
-00000920: 6865 205b 6f6e 6c69 6e65 2064 6f63 756d  he [online docum
-00000930: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-00000940: 2f2f 657a 7461 6f2e 7265 6164 7468 6564  //eztao.readthed
-00000950: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000960: 2f29 206f 7220 7275 6e20 7468 6520 7475  /) or run the tu
-00000970: 746f 7269 616c 206e 6f74 6562 6f6f 6b73  torial notebooks
-00000980: 2061 7420 2d3e 0a5b 215b 4269 6e64 6572   at ->.[![Binder
-00000990: 5d28 6874 7470 733a 2f2f 6d79 6269 6e64  ](https://mybind
-000009a0: 6572 2e6f 7267 2f62 6164 6765 5f6c 6f67  er.org/badge_log
-000009b0: 6f2e 7376 6729 5d28 6874 7470 733a 2f2f  o.svg)](https://
-000009c0: 6d79 6269 6e64 6572 2e6f 7267 2f76 322f  mybinder.org/v2/
-000009d0: 6768 2f79 7778 3634 3939 3939 3331 312f  gh/ywx649999311/
-000009e0: 457a 5461 6f2f 7630 2e33 2e30 3f66 696c  EzTao/v0.3.0?fil
-000009f0: 6570 6174 683d 646f 6373 2f6e 6f74 6562  epath=docs/noteb
-00000a00: 6f6f 6b73 292e 0a0a 2323 2320 4465 7665  ooks)...### Deve
-00000a10: 6c6f 706d 656e 740a 6070 6f65 7472 7960  lopment.`poetry`
-00000a20: 2069 7320 7573 6564 2074 6f20 736f 6c76   is used to solv
-00000a30: 6520 6465 7065 6e64 656e 6369 6573 2061  e dependencies a
-00000a40: 6e64 2074 6f20 6275 696c 642f 7075 626c  nd to build/publ
-00000a50: 6973 6820 7468 6973 2070 6163 6b61 6765  ish this package
-00000a60: 2e20 4265 6c6f 7720 7368 6f77 7320 686f  . Below shows ho
-00000a70: 7720 7365 7475 7020 7468 6520 656e 7669  w setup the envi
-00000a80: 726f 6e6d 656e 7420 666f 7220 6465 7665  ronment for deve
-00000a90: 6c6f 706d 656e 7420 2861 7373 756d 696e  lopment (assumin
-00000aa0: 6720 796f 7520 616c 7265 6164 7920 6861  g you already ha
-00000ab0: 7665 2060 706f 6574 7279 6020 696e 7374  ve `poetry` inst
-00000ac0: 616c 6c65 6420 6f6e 2079 6f75 7220 6d61  alled on your ma
-00000ad0: 6368 696e 6529 2e20 0a0a 312e 2043 6c6f  chine). ..1. Clo
-00000ae0: 6e65 2074 6869 7320 7265 706f 7369 746f  ne this reposito
-00000af0: 7279 2c20 616e 6420 656e 7465 7220 7468  ry, and enter th
-00000b00: 6520 7265 706f 7369 746f 7279 2066 6f6c  e repository fol
-00000b10: 6465 722e 0a32 2e20 4372 6561 7465 2061  der..2. Create a
-00000b20: 2070 7974 686f 6e20 7669 7274 7561 6c20   python virtual 
-00000b30: 656e 7669 726f 6e6d 656e 7420 616e 6420  environment and 
-00000b40: 6163 7469 7661 7465 2069 7420 2874 6865  activate it (the
-00000b50: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
-00000b60: 6d65 6e74 206e 616d 6520 6d75 7374 2062  ment name must b
-00000b70: 6520 272e 7665 6e76 2729 2e20 0a20 2020  e '.venv'). .   
-00000b80: 2060 6060 0a20 2020 2070 7974 686f 6e20   ```.    python 
-00000b90: 2d6d 2076 656e 7620 2e76 656e 760a 2020  -m venv .venv.  
-00000ba0: 2020 736f 7572 6365 202e 7665 6e76 2f62    source .venv/b
-00000bb0: 696e 2f61 6374 6976 6174 650a 2020 2020  in/activate.    
-00000bc0: 6060 600a 332e 2049 6e73 7461 6c6c 2064  ```.3. Install d
-00000bd0: 6570 656e 6465 6e63 6965 7320 616e 6420  ependencies and 
-00000be0: 2a2a 457a 5461 6f2a 2a20 696e 2065 6469  **EzTao** in edi
-00000bf0: 7461 626c 6520 6d6f 6465 2e0a 2020 2060  table mode..   `
-00000c00: 6060 0a20 2020 706f 6574 7279 2069 6e73  ``.   poetry ins
-00000c10: 7461 6c6c 0a20 2020 6060 600a 0a4e 6f77  tall.   ```..Now
-00000c20: 2079 6f75 2073 686f 756c 6420 6265 2072   you should be r
-00000c30: 6561 6479 2074 6f20 7374 6172 7420 6164  eady to start ad
-00000c40: 6469 6e67 206e 6577 2066 6561 7475 7265  ding new feature
-00000c50: 732e 2042 6520 7375 7265 2074 6f20 6368  s. Be sure to ch
-00000c60: 6563 6b6f 7574 2074 6865 206e 6f72 6d61  eckout the norma
-00000c70: 6c20 7072 6163 7469 6365 2072 6567 6172  l practice regar
-00000c80: 6469 6e67 2068 6f77 2074 6f20 7573 6520  ding how to use 
-00000c90: 6070 6f65 7472 7960 206f 6e20 6974 7320  `poetry` on its 
-00000ca0: 7765 6273 6974 652e 2057 6865 6e20 796f  website. When yo
-00000cb0: 7520 6172 6520 7265 6164 7920 746f 2070  u are ready to p
-00000cc0: 7573 682c 2061 6c73 6f20 6d61 6b65 2073  ush, also make s
-00000cd0: 7572 6520 7468 6520 706f 6574 7279 2e6c  ure the poetry.l
-00000ce0: 6f63 6b20 6669 6c65 2069 7320 6368 6563  ock file is chec
-00000cf0: 6b65 642d 696e 2069 6620 616e 7920 6465  ked-in if any de
-00000d00: 7065 6e64 656e 6379 2068 6173 2063 6861  pendency has cha
-00000d10: 6e67 6564 2e20 0a                        nged. .
+00000140: 2f6c 6174 6573 742f 290a 3c61 2068 7265  /latest/).<a hre
+00000150: 663d 2268 7474 7073 3a2f 2f61 7363 6c2e  f="https://ascl.
+00000160: 6e65 742f 3232 3031 2e30 3031 223e 3c69  net/2201.001"><i
+00000170: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000180: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000190: 6164 6765 2f61 7363 6c2d 3232 3031 2e30  adge/ascl-2201.0
+000001a0: 3031 2d62 6c75 652e 7376 673f 636f 6c6f  01-blue.svg?colo
+000001b0: 7242 3d32 3632 3235 3522 2061 6c74 3d22  rB=262255" alt="
+000001c0: 6173 636c 3a32 3230 312e 3030 3122 202f  ascl:2201.001" /
+000001d0: 3e3c 2f61 3e0a 2320 457a 5461 6f20 28e6  ></a>.# EzTao (.
+000001e0: 9893 e981 9329 0a2a 2a45 7a54 616f 2a2a  .....).**EzTao**
+000001f0: 2069 7320 6120 746f 6f6c 6b69 7420 666f   is a toolkit fo
+00000200: 7220 636f 6e64 7563 7469 6e67 2041 474e  r conducting AGN
+00000210: 2074 696d 652d 7365 7269 6573 2f76 6172   time-series/var
+00000220: 6961 6269 6c69 7479 2061 6e61 6c79 7369  iability analysi
+00000230: 732c 206d 6169 6e6c 7920 7574 696c 697a  s, mainly utiliz
+00000240: 696e 6720 7468 6520 636f 6e74 696e 756f  ing the continuo
+00000250: 7573 2d74 696d 6520 6175 746f 2d72 6567  us-time auto-reg
+00000260: 7265 7373 6976 6520 6d6f 7669 6e67 2061  ressive moving a
+00000270: 7665 7261 6765 206d 6f64 656c 2028 4341  verage model (CA
+00000280: 524d 4129 0a0a 2323 2049 6e73 7461 6c6c  RMA)..## Install
+00000290: 6174 696f 6e0a 3c21 2d2d 2d20 6060 600a  ation.<!--- ```.
+000002a0: 7069 7020 696e 7374 616c 6c20 657a 7461  pip install ezta
+000002b0: 6f0a 6060 600a 6f72 2028 6672 6f6d 206d  o.```.or (from m
+000002c0: 6173 7465 7229 2d2d 2d3e 0a60 6060 0a70  aster)--->.```.p
+000002d0: 6970 2069 6e73 7461 6c6c 2067 6974 2b68  ip install git+h
+000002e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000002f0: 6d2f 7977 7836 3439 3939 3933 3131 2f45  m/ywx649999311/E
+00000300: 7a54 616f 2e67 6974 0a60 6060 0a23 2323  zTao.git.```.###
+00000310: 2044 6570 656e 6465 6e63 6965 730a 3e60   Dependencies.>`
+00000320: 6060 0a3e 7079 7468 6f6e 203d 2022 5e33  ``.>python = "^3
+00000330: 2e37 220a 3e63 656c 6572 6974 6520 3d20  .7".>celerite = 
+00000340: 223e 3d20 302e 332e 3022 0a3e 6d61 7470  ">= 0.3.0".>matp
+00000350: 6c6f 746c 6962 203d 2022 5e33 2e33 2e30  lotlib = "^3.3.0
+00000360: 220a 3e73 6369 7079 203d 2022 3e20 312e  ".>scipy = "> 1.
+00000370: 352e 3022 0a3e 6e75 6d62 6120 3d20 223e  5.0".>numba = ">
+00000380: 3d20 302e 3531 2e30 220a 3e65 6d63 6565  = 0.51.0".>emcee
+00000390: 203d 2022 3e3d 332e 302e 3022 0a3e 6060   = ">=3.0.0".>``
+000003a0: 600a 0a23 2320 5175 6963 6b20 4578 616d  `..## Quick Exam
+000003b0: 706c 6573 0a4c 6574 2773 2066 6972 7374  ples.Let's first
+000003c0: 2073 696d 756c 6174 6520 6120 4452 572f   simulate a DRW/
+000003d0: 4341 524d 4128 312c 3029 2070 726f 6365  CARMA(1,0) proce
+000003e0: 7373 2077 6974 6820 6120 7661 7269 616e  ss with a varian
+000003f0: 6365 206f 6620 302e 335e 3220 616e 6420  ce of 0.3^2 and 
+00000400: 6120 7265 6c61 7861 7469 6f6e 2074 696d  a relaxation tim
+00000410: 6573 6361 6c65 206f 6620 3130 3020 6461  escale of 100 da
+00000420: 7973 2e20 5468 6973 2074 696d 6520 7365  ys. This time se
+00000430: 7269 6573 2077 696c 6c20 6861 7665 2061  ries will have a
+00000440: 2074 6f74 616c 206f 6620 3230 3020 6461   total of 200 da
+00000450: 7461 2070 6f69 6e74 7320 616e 6420 7370  ta points and sp
+00000460: 616e 2031 3020 7965 6172 732e 0a60 6060  an 10 years..```
+00000470: 7079 7468 6f6e 0a69 6d70 6f72 7420 6e75  python.import nu
+00000480: 6d70 7920 6173 206e 700a 696d 706f 7274  mpy as np.import
+00000490: 206d 6174 706c 6f74 6c69 622e 7079 706c   matplotlib.pypl
+000004a0: 6f74 2061 7320 706c 740a 6672 6f6d 2065  ot as plt.from e
+000004b0: 7a74 616f 2e63 6172 6d61 2069 6d70 6f72  ztao.carma impor
+000004c0: 7420 4452 575f 7465 726d 0a66 726f 6d20  t DRW_term.from 
+000004d0: 657a 7461 6f2e 7473 2069 6d70 6f72 7420  eztao.ts import 
+000004e0: 6770 5369 6d52 616e 640a 0a23 2064 6566  gpSimRand..# def
+000004f0: 696e 6520 6120 4452 5720 6b65 726e 656c  ine a DRW kernel
+00000500: 2026 2061 6e64 2073 696d 756c 6174 6520   & and simulate 
+00000510: 6120 7072 6f63 6573 730a 616d 7020 3d20  a process.amp = 
+00000520: 302e 320a 7461 7520 3d20 3130 300a 4452  0.2.tau = 100.DR
+00000530: 575f 6b65 726e 656c 203d 2044 5257 5f74  W_kernel = DRW_t
+00000540: 6572 6d28 6e70 2e6c 6f67 2861 6d70 292c  erm(np.log(amp),
+00000550: 206e 702e 6c6f 6728 7461 7529 290a 742c   np.log(tau)).t,
+00000560: 2079 2c20 7965 7272 203d 2067 7053 696d   y, yerr = gpSim
+00000570: 5261 6e64 2844 5257 5f6b 6572 6e65 6c2c  Rand(DRW_kernel,
+00000580: 2031 302c 2033 3635 2a31 302c 2032 3030   10, 365*10, 200
+00000590: 290a 0a23 206e 6f77 2c20 706c 6f74 2069  )..# now, plot i
+000005a0: 740a 6669 672c 2061 7820 3d20 706c 742e  t.fig, ax = plt.
+000005b0: 7375 6270 6c6f 7473 2831 2c31 2c20 6470  subplots(1,1, dp
+000005c0: 693d 3135 302c 2066 6967 7369 7a65 3d28  i=150, figsize=(
+000005d0: 382c 3329 290a 6178 2e65 7272 6f72 6261  8,3)).ax.errorba
+000005e0: 7228 742c 2079 2c20 7965 7272 2c20 666d  r(t, y, yerr, fm
+000005f0: 743d 272e 2729 0a2e 2e2e 0a60 6060 0a21  t='.').....```.!
+00000600: 5b64 7277 5f73 696d 5d28 696e 636c 7564  [drw_sim](includ
+00000610: 652f 6472 775f 7369 6d2e 706e 6729 0a0a  e/drw_sim.png)..
+00000620: 5765 2063 616e 2066 6974 2074 6865 2073  We can fit the s
+00000630: 696d 756c 6174 6564 2074 696d 6520 7365  imulated time se
+00000640: 7269 6573 2074 6f20 7468 6520 4452 5720  ries to the DRW 
+00000650: 6d6f 6465 6c20 616e 6420 7365 6520 686f  model and see ho
+00000660: 7720 7765 6c6c 2077 6520 6361 6e20 7265  w well we can re
+00000670: 636f 7665 7220 7468 6520 696e 7075 7420  cover the input 
+00000680: 7061 7261 6d65 7465 7273 2e0a 6060 6070  parameters..```p
+00000690: 7974 686f 6e0a 6672 6f6d 2065 7a74 616f  ython.from eztao
+000006a0: 2e74 7320 696d 706f 7274 2064 7277 5f66  .ts import drw_f
+000006b0: 6974 0a0a 6265 7374 5f66 6974 203d 2064  it..best_fit = d
+000006c0: 7277 5f66 6974 2874 2c20 792c 2079 6572  rw_fit(t, y, yer
+000006d0: 7229 0a70 7269 6e74 2866 2742 6573 742d  r).print(f'Best-
+000006e0: 6669 7420 4452 5720 7061 7261 6d65 7465  fit DRW paramete
+000006f0: 7273 3a20 7b62 6573 745f 6669 747d 2729  rs: {best_fit}')
+00000700: 0a60 6060 0a60 6060 7368 656c 6c0a 4265  .```.```shell.Be
+00000710: 7374 2d66 6974 2044 5257 2070 6172 616d  st-fit DRW param
+00000720: 6574 6572 733a 205b 302e 3137 3335 3639  eters: [0.173569
+00000730: 3833 2038 382e 3336 3236 3234 3637 5d0a  83 88.36262467].
+00000740: 6060 600a 0a48 6f77 2064 6f65 7320 7468  ```..How does th
+00000750: 6520 706f 7765 7220 7370 6563 7472 756d  e power spectrum
+00000760: 2064 656e 7369 7479 2028 5053 4429 2063   density (PSD) c
+00000770: 6f6d 7061 7265 3f0a 6060 6070 7974 686f  ompare?.```pytho
+00000780: 6e0a 6672 6f6d 2065 7a74 616f 2e63 6172  n.from eztao.car
+00000790: 6d61 2069 6d70 6f72 7420 6770 5f70 7364  ma import gp_psd
+000007a0: 0a0a 2320 6765 7420 7073 6420 6675 6e63  ..# get psd func
+000007b0: 7469 6f6e 730a 7472 7565 5f70 7364 203d  tions.true_psd =
+000007c0: 2067 705f 7073 6428 4452 575f 6b65 726e   gp_psd(DRW_kern
+000007d0: 656c 290a 6265 7374 5f70 7364 203d 2067  el).best_psd = g
+000007e0: 705f 7073 6428 4452 575f 7465 726d 282a  p_psd(DRW_term(*
+000007f0: 6e70 2e6c 6f67 2862 6573 745f 6669 7429  np.log(best_fit)
+00000800: 2929 0a0a 2320 706c 6f74 0a66 6967 2c20  ))..# plot.fig, 
+00000810: 6178 203d 2070 6c74 2e73 7562 706c 6f74  ax = plt.subplot
+00000820: 7328 312c 312c 2064 7069 3d31 3530 2c20  s(1,1, dpi=150, 
+00000830: 6669 6773 697a 653d 2836 2c33 2929 0a66  figsize=(6,3)).f
+00000840: 7265 7120 3d20 6e70 2e6c 6f67 7370 6163  req = np.logspac
+00000850: 6528 2d35 2c20 3229 0a61 782e 706c 6f74  e(-5, 2).ax.plot
+00000860: 2866 7265 712c 2074 7275 655f 7073 6428  (freq, true_psd(
+00000870: 6672 6571 292c 206c 6162 656c 3d27 496e  freq), label='In
+00000880: 7075 7420 5053 4427 290a 6178 2e70 6c6f  put PSD').ax.plo
+00000890: 7428 6672 6571 2c20 6265 7374 5f70 7364  t(freq, best_psd
+000008a0: 2866 7265 7129 2c20 6c61 6265 6c3d 2742  (freq), label='B
+000008b0: 6573 742d 6669 7420 5053 4427 290a 2e2e  est-fit PSD')...
+000008c0: 2e0a 6060 600a 215b 6472 775f 7073 645d  ..```.![drw_psd]
+000008d0: 2869 6e63 6c75 6465 2f64 7277 5f70 7364  (include/drw_psd
+000008e0: 2e70 6e67 290a 0a5f 5f4e 6f74 653a 5f5f  .png)..__Note:__
+000008f0: 2048 6f77 2077 656c 6c20 7468 6520 696e   How well the in
+00000900: 7075 7420 616e 6420 6265 7374 2d66 6974  put and best-fit
+00000910: 2050 5344 206d 6174 6368 2069 7320 7570   PSD match is up
+00000920: 2074 6f20 686f 7720 676f 6f64 2074 6865   to how good the
+00000930: 2062 6573 742d 6669 7420 7061 7261 6d65   best-fit parame
+00000940: 7465 7273 2061 7265 2c20 7768 6963 6820  ters are, which 
+00000950: 6973 2068 6967 686c 7920 696e 666c 7565  is highly influe
+00000960: 6e63 6564 2062 7920 7468 6520 7175 616c  nced by the qual
+00000970: 6974 7920 6f66 2074 6865 2069 6e70 7574  ity of the input
+00000980: 2074 696d 6520 7365 7269 6573 2e20 0a0a   time series. ..
+00000990: 466f 7220 6d6f 7265 2065 7861 6d70 6c65  For more example
+000009a0: 732c 2070 6c65 6173 6520 6368 6563 6b20  s, please check 
+000009b0: 6f75 7420 7468 6520 5b6f 6e6c 696e 6520  out the [online 
+000009c0: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
+000009d0: 7474 7073 3a2f 2f65 7a74 616f 2e72 6561  ttps://eztao.rea
+000009e0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000009f0: 6174 6573 742f 2920 6f72 2072 756e 2074  atest/) or run t
+00000a00: 6865 2074 7574 6f72 6961 6c20 6e6f 7465  he tutorial note
+00000a10: 626f 6f6b 7320 6174 202d 3e0a 5b21 5b42  books at ->.[![B
+00000a20: 696e 6465 725d 2868 7474 7073 3a2f 2f6d  inder](https://m
+00000a30: 7962 696e 6465 722e 6f72 672f 6261 6467  ybinder.org/badg
+00000a40: 655f 6c6f 676f 2e73 7667 295d 2868 7474  e_logo.svg)](htt
+00000a50: 7073 3a2f 2f6d 7962 696e 6465 722e 6f72  ps://mybinder.or
+00000a60: 672f 7632 2f67 682f 7977 7836 3439 3939  g/v2/gh/ywx64999
+00000a70: 3933 3131 2f45 7a54 616f 2f76 302e 342e  9311/EzTao/v0.4.
+00000a80: 303f 6669 6c65 7061 7468 3d64 6f63 732f  0?filepath=docs/
+00000a90: 6e6f 7465 626f 6f6b 7329 2e0a 0a23 2320  notebooks)...## 
+00000aa0: 4465 7665 6c6f 706d 656e 740a 6070 6f65  Development.`poe
+00000ab0: 7472 7960 2069 7320 7573 6564 2074 6f20  try` is used to 
+00000ac0: 736f 6c76 6520 6465 7065 6e64 656e 6369  solve dependenci
+00000ad0: 6573 2061 6e64 2074 6f20 6275 696c 642f  es and to build/
+00000ae0: 7075 626c 6973 6820 7468 6973 2070 6163  publish this pac
+00000af0: 6b61 6765 2e20 4265 6c6f 7720 7368 6f77  kage. Below show
+00000b00: 7320 686f 7720 7365 7475 7020 7468 6520  s how setup the 
+00000b10: 656e 7669 726f 6e6d 656e 7420 666f 7220  environment for 
+00000b20: 6465 7665 6c6f 706d 656e 7420 2861 7373  development (ass
+00000b30: 756d 696e 6720 796f 7520 616c 7265 6164  uming you alread
+00000b40: 7920 6861 7665 2060 706f 6574 7279 6020  y have `poetry` 
+00000b50: 696e 7374 616c 6c65 6420 6f6e 2079 6f75  installed on you
+00000b60: 7220 6d61 6368 696e 6529 2e20 5f2a 2a57  r machine). _**W
+00000b70: 6172 6e69 6e67 3a2a 2a5f 2060 706f 6574  arning:**_ `poet
+00000b80: 7279 6020 6973 2068 6176 696e 6720 6973  ry` is having is
+00000b90: 7375 6520 696e 7374 616c 6c69 6e67 2060  sue installing `
+00000ba0: 6c6c 766d 6c69 7465 203d 2030 2e33 342e  llvmlite = 0.34.
+00000bb0: 3060 2028 7573 6564 2066 6f72 2060 657a  0` (used for `ez
+00000bc0: 7461 6f20 3d20 5e30 2e34 2e30 6029 2075  tao = ^0.4.0`) u
+00000bd0: 6e64 6572 2050 7974 686f 6e20 332e 392e  nder Python 3.9.
+00000be0: 2054 6865 2069 7373 7565 2064 6973 6170   The issue disap
+00000bf0: 7065 6172 7320 666f 7220 5079 7468 6f6e  pears for Python
+00000c00: 2033 2e38 2e0a 0a31 2e20 436c 6f6e 6520   3.8...1. Clone 
+00000c10: 7468 6973 2072 6570 6f73 6974 6f72 792c  this repository,
+00000c20: 2061 6e64 2065 6e74 6572 2074 6865 2072   and enter the r
+00000c30: 6570 6f73 6974 6f72 7920 666f 6c64 6572  epository folder
+00000c40: 2e0a 322e 2043 7265 6174 6520 6120 7079  ..2. Create a py
+00000c50: 7468 6f6e 2076 6972 7475 616c 2065 6e76  thon virtual env
+00000c60: 6972 6f6e 6d65 6e74 2061 6e64 2061 6374  ironment and act
+00000c70: 6976 6174 6520 6974 2028 7468 6520 7669  ivate it (the vi
+00000c80: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
+00000c90: 7420 6e61 6d65 206d 7573 7420 6265 2027  t name must be '
+00000ca0: 2e76 656e 7627 292e 200a 2020 2020 6060  .venv'). .    ``
+00000cb0: 600a 2020 2020 7079 7468 6f6e 202d 6d20  `.    python -m 
+00000cc0: 7665 6e76 202e 7665 6e76 0a20 2020 2073  venv .venv.    s
+00000cd0: 6f75 7263 6520 2e76 656e 762f 6269 6e2f  ource .venv/bin/
+00000ce0: 6163 7469 7661 7465 0a20 2020 2060 6060  activate.    ```
+00000cf0: 0a33 2e20 496e 7374 616c 6c20 6465 7065  .3. Install depe
+00000d00: 6e64 656e 6369 6573 2061 6e64 202a 2a45  ndencies and **E
+00000d10: 7a54 616f 2a2a 2069 6e20 6564 6974 6162  zTao** in editab
+00000d20: 6c65 206d 6f64 652e 0a20 2020 6060 600a  le mode..   ```.
+00000d30: 2020 2070 6f65 7472 7920 696e 7374 616c     poetry instal
+00000d40: 6c0a 2020 2060 6060 0a0a 4e6f 7720 796f  l.   ```..Now yo
+00000d50: 7520 7368 6f75 6c64 2062 6520 7265 6164  u should be read
+00000d60: 7920 746f 2073 7461 7274 2061 6464 696e  y to start addin
+00000d70: 6720 6e65 7720 6665 6174 7572 6573 2e20  g new features. 
+00000d80: 4265 2073 7572 6520 746f 2063 6865 636b  Be sure to check
+00000d90: 6f75 7420 7468 6520 6e6f 726d 616c 2070  out the normal p
+00000da0: 7261 6374 6963 6520 7265 6761 7264 696e  ractice regardin
+00000db0: 6720 686f 7720 746f 2075 7365 2060 706f  g how to use `po
+00000dc0: 6574 7279 6020 6f6e 2069 7473 2077 6562  etry` on its web
+00000dd0: 7369 7465 2e20 5768 656e 2079 6f75 2061  site. When you a
+00000de0: 7265 2072 6561 6479 2074 6f20 7075 7368  re ready to push
+00000df0: 2c20 616c 736f 206d 616b 6520 7375 7265  , also make sure
+00000e00: 2074 6865 2070 6f65 7472 792e 6c6f 636b   the poetry.lock
+00000e10: 2066 696c 6520 6973 2063 6865 636b 6564   file is checked
+00000e20: 2d69 6e20 6966 2061 6e79 2064 6570 656e  -in if any depen
+00000e30: 6465 6e63 7920 6861 7320 6368 616e 6765  dency has change
+00000e40: 642e 200a 0a23 2320 4369 7461 7469 6f6e  d. ..## Citation
+00000e50: 0a57 6520 6172 6520 776f 726b 696e 6720  .We are working 
+00000e60: 6f6e 2061 2070 6170 6572 2074 6f20 6465  on a paper to de
+00000e70: 7363 7269 6265 2074 6865 2066 756c 6c20  scribe the full 
+00000e80: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
+00000e90: 6620 2a2a 457a 5461 6f2a 2a2e 2049 6e20  f **EzTao**. In 
+00000ea0: 7468 6520 6d65 616e 7469 6d65 2c20 6966  the meantime, if
+00000eb0: 2079 6f75 2066 696e 6420 2a2a 457a 5461   you find **EzTa
+00000ec0: 6f2a 2a20 7573 6566 756c 2066 6f72 2079  o** useful for y
+00000ed0: 6f75 7220 7265 7365 6172 6368 2c20 706c  our research, pl
+00000ee0: 6561 7365 2063 6f6e 7369 6465 7220 6163  ease consider ac
+00000ef0: 6b6e 6f77 6c65 6467 696e 6720 2a2a 457a  knowledging **Ez
+00000f00: 5461 6f2a 2a20 7573 696e 6720 7468 6520  Tao** using the 
+00000f10: 666f 6c6c 6f77 696e 673a 0a0a 6060 600a  following:..```.
+00000f20: 404d 4953 437b 5975 3230 3232 2c0a 2020  @MISC{Yu2022,.  
+00000f30: 2020 2020 2061 7574 686f 7220 3d20 7b7b       author = {{
+00000f40: 5975 7d2c 2057 6569 7869 616e 6720 616e  Yu}, Weixiang an
+00000f50: 6420 7b52 6963 6861 7264 737d 2c20 476f  d {Richards}, Go
+00000f60: 7264 6f6e 2054 2e7d 2c0a 2020 2020 2020  rdon T.},.      
+00000f70: 2020 7469 746c 6520 3d20 227b 457a 5461    title = "{EzTa
+00000f80: 6f3a 2045 6173 6965 7220 4341 524d 4120  o: Easier CARMA 
+00000f90: 4d6f 6465 6c69 6e67 7d22 2c0a 2020 2020  Modeling}",.    
+00000fa0: 206b 6579 776f 7264 7320 3d20 7b53 6f66   keywords = {Sof
+00000fb0: 7477 6172 657d 2c0a 2068 6f77 7075 626c  tware},. howpubl
+00000fc0: 6973 6865 6420 3d20 7b41 7374 726f 7068  ished = {Astroph
+00000fd0: 7973 6963 7320 536f 7572 6365 2043 6f64  ysics Source Cod
+00000fe0: 6520 4c69 6272 6172 792c 2072 6563 6f72  e Library, recor
+00000ff0: 6420 6173 636c 3a32 3230 312e 3030 317d  d ascl:2201.001}
+00001000: 2c0a 2020 2020 2020 2020 2079 6561 7220  ,.         year 
+00001010: 3d20 3230 3232 2c0a 2020 2020 2020 2020  = 2022,.        
+00001020: 6d6f 6e74 6820 3d20 6a61 6e2c 0a20 2020  month = jan,.   
+00001030: 2020 2020 2020 2065 6964 203d 207b 6173         eid = {as
+00001040: 636c 3a32 3230 312e 3030 317d 2c0a 2020  cl:2201.001},.  
+00001050: 2020 2020 2020 7061 6765 7320 3d20 7b61        pages = {a
+00001060: 7363 6c3a 3232 3031 2e30 3031 7d2c 0a61  scl:2201.001},.a
+00001070: 7263 6869 7665 5072 6566 6978 203d 207b  rchivePrefix = {
+00001080: 6173 636c 7d2c 0a20 2020 2020 2020 6570  ascl},.       ep
+00001090: 7269 6e74 203d 207b 3232 3031 2e30 3031  rint = {2201.001
+000010a0: 7d2c 0a20 2020 2020 2020 6164 7375 726c  },.       adsurl
+000010b0: 203d 207b 6874 7470 733a 2f2f 7569 2e61   = {https://ui.a
+000010c0: 6473 6162 732e 6861 7276 6172 642e 6564  dsabs.harvard.ed
+000010d0: 752f 6162 732f 3230 3232 6173 636c 2e73  u/abs/2022ascl.s
+000010e0: 6f66 7430 3130 3031 597d 2c0a 2020 2020  oft01001Y},.    
+000010f0: 2020 6164 736e 6f74 6520 3d20 7b50 726f    adsnote = {Pro
+00001100: 7669 6465 6420 6279 2074 6865 2053 414f  vided by the SAO
+00001110: 2f4e 4153 4120 4173 7472 6f70 6879 7369  /NASA Astrophysi
+00001120: 6373 2044 6174 6120 5379 7374 656d 7d0a  cs Data System}.
+00001130: 7d0a 6060 600a 0a                        }.```..
```

### Comparing `eztao-0.4.0/pyproject.toml` & `eztao-0.4.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "eztao"
-version = "0.4.0"
+version = "0.4.1"
 description = "A toolkit for Active Galactic Nuclei (AGN) time-series analysis."
 authors = ["Weixiang Yu <wy73@drexel.edu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ywx649999311/EzTao"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 celerite = ">= 0.3.0"
 matplotlib = "^3.3.0"
-scipy = "> 1.5.0"
+scipy = ">= 1.5"
 numba = ">= 0.51.0"
 importlib-metadata = ">= 2.0.0"
 emcee = ">=3.0.0"
 
 [tool.poetry.dev-dependencies]
 toml = "^0.10.1"
 pytest = "^6.0.1"
 pytest-cov = "^2.10.1"
-joblib = "^0.17.0"
+joblib = ">=1.2.0"
 pandas = "^1.1.4"
 Sphinx = "^3.4.1"
 sphinx-rtd-theme = "^0.5.0"
 nbsphinx = ">=0.8.6"
 sphinx-copybutton = "^0.3.1"
 black = "^21.7b0"
```

### Comparing `eztao-0.4.0/src/eztao/carma/CARMATerm.py` & `eztao-0.4.1/src/eztao/carma/CARMATerm.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     The input fcoeffs follow the notation (index) in Jones et al. (1981) with the last
     element being an additional multiplying factor (the coeff of the highest-order term
     in the final expanded polynomial).
 
     :meta private:
     """
     size = fcoeffs.shape[0] - 1
-    odd = np.bool(size & 0x1)
+    odd = bool(size & 0x1)
     nPair = size // 2
     poly = fcoeffs[-1:]  # The coeff of highest order term in the product
 
     if odd:
         poly = polymul(poly, np.array([1.0, fcoeffs[-2]]))
 
     for p in np.arange(nPair):
@@ -80,15 +80,15 @@
     """Generate factored polynomial from roots
 
     The notation (index) for the factored polynomial follows that in
     Jones et al. (1981). Note: No multiplying is returned.
     """
     coeffs = []
     size = len(roots)
-    odd = np.bool(size & 0x1)
+    odd = bool(size & 0x1)
     rootsComp = roots[roots.imag != 0]
     rootsReal = roots[roots.imag == 0]
     nCompPair = len(rootsComp) // 2
     nRealPair = len(rootsReal) // 2
 
     for i in range(nCompPair):
         root1 = rootsComp[i]
@@ -231,15 +231,15 @@
 
     def get_carma_parameter(self):
         """Get DRW parameters in CARMA notation (alpha_*/beta_*).
 
         Returns:
             [alpha_1, beta_0].
         """
-        return [-1 / np.exp(self.get_parameter("log_tau")), self.get_perturb_amp()]
+        return [1 / np.exp(self.get_parameter("log_tau")), self.get_perturb_amp()]
 
     @property
     def p(self):
         return 1
 
     @property
     def q(self):
```

### Comparing `eztao-0.4.0/src/eztao/carma/model_utils.py` & `eztao-0.4.1/src/eztao/carma/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     """
     arparams = np.insert(arparams, 0, 1)
     maparams = np.array(maparams)
     arparams_rv = arparams[::-1]
 
     def psd(f):
         # init terms
-        num_terms = np.complex(0)
-        denom_terms = np.complex(0)
+        num_terms = complex(0)
+        denom_terms = complex(0)
 
         for i, param in enumerate(maparams):
             num_terms += param * np.power(2 * np.pi * f * (1j), i)
 
         for k, param in enumerate(arparams_rv):
             denom_terms += param * np.power(2 * np.pi * f * (1j), k)
```

### Comparing `eztao-0.4.0/src/eztao/ts/carma_fit.py` & `eztao-0.4.1/src/eztao/ts/carma_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A collection of functions to fit/analyze time series using CARMA models.
 """
 
 import numpy as np
 from math import ceil
 from scipy.optimize import minimize
-from scipy.stats import median_absolute_deviation as mad
+from scipy.stats import median_abs_deviation as mad
 import celerite
 from celerite import GP
 from eztao.carma.CARMATerm import DRW_term, DHO_term, CARMA_term
 from functools import partial
 
 # change numpy warn setting
 old_settings = np.seterr(all="warn")
@@ -548,16 +548,20 @@
             opt_options=scipy_opt_options,
             debug=debug,
         )
     else:
         opt = optimizer_func
 
     # get best-fit solution & adjust MA params (multiply by y_std)
+    # if not fit found, return all nan
     best_fit_return = opt(y, gp, init, neg_lp, n_opt)
-    best_fit_return[2:] = best_fit_return[2:] * y_std
+    try:
+        best_fit_return[2:] = best_fit_return[2:] * y_std
+    except:
+        pass
 
     return best_fit_return
 
 
 def carma_fit(
     t,
     y,
@@ -655,11 +659,15 @@
             opt_options=scipy_opt_options,
             debug=debug,
         )
     else:
         opt = optimizer_func
 
     # get best-fit solution & adjust MA params (multiply by y_std)
+    # if not fit found, return all nan
     best_fit_return = opt(y, gp, init, neg_lp, n_opt)
-    best_fit_return[p:] = best_fit_return[p:] * y_std
+    try:
+        best_fit_return[p:] = best_fit_return[p:] * y_std
+    except:
+        pass
 
     return best_fit_return
```

### Comparing `eztao-0.4.0/src/eztao/ts/carma_mcmc.py` & `eztao-0.4.1/src/eztao/ts/carma_mcmc.py`

 * *Files identical despite different names*

### Comparing `eztao-0.4.0/src/eztao/ts/carma_sim.py` & `eztao-0.4.1/src/eztao/ts/carma_sim.py`

 * *Files identical despite different names*

### Comparing `eztao-0.4.0/src/eztao/ts/utils.py` & `eztao-0.4.1/src/eztao/ts/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 A collection of utility functions to assist analysis/simulation of time series data.
 """
 
 import numpy as np
 from numba import njit
 from functools import partial
+from scipy.stats import median_abs_deviation as mad
 
 __all__ = ["downsample_byN", "add_season", "downsample_byTime", "median_clip"]
 
 
 def downsample_byN(t, nObs):
     """
     Randomly choose N data points from a given time series.
@@ -70,15 +71,14 @@
     t = t + lc_start
 
     mask = (np.mod(t, 365.25) > season_start) & (np.mod(t, 365.25) < season_end)
 
     return mask
 
 
-@njit
 def median_clip(y, num_sigma=3):
     """Clip time series using a three point median filter.
 
     The sigma (standard deviation) for the time series is computed from the median  absolute deviation (MAD) as to reduce the effects from extreme outliers, where
     sigma \sim 1.4826*MAD. If more than 10% of the data points are removed, the upper
     bound will be lifted gradually until that fraction drops bellow 10%.
 
@@ -88,30 +88,30 @@
             away from the three point median will be removed. Defaults to 3.
 
     Returns:
         A 1d array booleans indicating which data points to keep.
     """
     y = np.atleast_1d(y)
     lc_len = y.shape[0]
-    sigma = 0.6745 * np.median(np.abs(y - np.median(y)))
     med = y.copy()
     med[1:-2] = [np.median(y[i - 1 : i + 2]) for i in range(1, lc_len - 2)]
 
     # need to deal with edges of median filter
     med[0] = np.median(np.array([y[-1], y[0], y[1]]))
     med[-1] = np.median(np.array([y[-2], y[-1], y[0]]))
 
-    # compute residual
+    # compute residual & sigma
     res = np.abs(y - med)
+    sigma = mad(res, scale='normal')
 
     # set clipping thresh hold
     raise_bar = True
     thresh = num_sigma * sigma
 
     # if remove too much, raise bar until only remove 10%
     while raise_bar:
         ratio = np.sum(res > thresh) / lc_len
         if ratio < 0.1:
             break
         else:
-            thresh += 0.1
+            thresh += 0.1 * sigma
     return res < thresh
```

### Comparing `eztao-0.4.0/src/eztao/viz/eztao.rc` & `eztao-0.4.1/src/eztao/viz/eztao.rc`

 * *Files identical despite different names*

### Comparing `eztao-0.4.0/src/eztao/viz/mpl_viz.py` & `eztao-0.4.1/src/eztao/viz/mpl_viz.py`

 * *Files identical despite different names*

### Comparing `eztao-0.4.0/PKG-INFO` & `eztao-0.4.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 657a 7461  : 2.1.Name: ezta
-00000020: 6f0a 5665 7273 696f 6e3a 2030 2e34 2e30  o.Version: 0.4.0
+00000020: 6f0a 5665 7273 696f 6e3a 2030 2e34 2e31  o.Version: 0.4.1
 00000030: 0a53 756d 6d61 7279 3a20 4120 746f 6f6c  .Summary: A tool
 00000040: 6b69 7420 666f 7220 4163 7469 7665 2047  kit for Active G
 00000050: 616c 6163 7469 6320 4e75 636c 6569 2028  alactic Nuclei (
 00000060: 4147 4e29 2074 696d 652d 7365 7269 6573  AGN) time-series
 00000070: 2061 6e61 6c79 7369 732e 0a48 6f6d 652d   analysis..Home-
 00000080: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 00000090: 7468 7562 2e63 6f6d 2f79 7778 3634 3939  thub.com/ywx6499
@@ -26,237 +26,309 @@
 00000190: 7468 6f6e 203a 3a20 332e 370a 436c 6173  thon :: 3.7.Clas
 000001a0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
 000001b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
 000001c0: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
 000001d0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
 000001e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 000001f0: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
-00000200: 5265 7175 6972 6573 2d44 6973 743a 2063  Requires-Dist: c
-00000210: 656c 6572 6974 6520 283e 3d30 2e33 2e30  elerite (>=0.3.0
-00000220: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000230: 2065 6d63 6565 2028 3e3d 332e 302e 3029   emcee (>=3.0.0)
-00000240: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000250: 696d 706f 7274 6c69 622d 6d65 7461 6461  importlib-metada
-00000260: 7461 2028 3e3d 322e 302e 3029 0a52 6571  ta (>=2.0.0).Req
-00000270: 7569 7265 732d 4469 7374 3a20 6d61 7470  uires-Dist: matp
-00000280: 6c6f 746c 6962 2028 3e3d 332e 332e 302c  lotlib (>=3.3.0,
-00000290: 3c34 2e30 2e30 290a 5265 7175 6972 6573  <4.0.0).Requires
-000002a0: 2d44 6973 743a 206e 756d 6261 2028 3e3d  -Dist: numba (>=
-000002b0: 302e 3531 2e30 290a 5265 7175 6972 6573  0.51.0).Requires
-000002c0: 2d44 6973 743a 2073 6369 7079 2028 3e31  -Dist: scipy (>1
-000002d0: 2e35 2e30 290a 5072 6f6a 6563 742d 5552  .5.0).Project-UR
-000002e0: 4c3a 2052 6570 6f73 6974 6f72 792c 2068  L: Repository, h
-000002f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000300: 6d2f 7977 7836 3439 3939 3933 3131 2f45  m/ywx649999311/E
-00000310: 7a54 616f 0a44 6573 6372 6970 7469 6f6e  zTao.Description
-00000320: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-00000330: 6578 742f 6d61 726b 646f 776e 0a0a 215b  ext/markdown..![
-00000340: 7465 7374 735d 2868 7474 7073 3a2f 2f67  tests](https://g
-00000350: 6974 6875 622e 636f 6d2f 7977 7836 3439  ithub.com/ywx649
-00000360: 3939 3933 3131 2f45 7a54 616f 2f77 6f72  999311/EzTao/wor
-00000370: 6b66 6c6f 7773 2f74 6573 7473 2f62 6164  kflows/tests/bad
-00000380: 6765 2e73 7667 290a 5b21 5b42 696e 6465  ge.svg).[![Binde
-00000390: 725d 2868 7474 7073 3a2f 2f6d 7962 696e  r](https://mybin
-000003a0: 6465 722e 6f72 672f 6261 6467 655f 6c6f  der.org/badge_lo
-000003b0: 676f 2e73 7667 295d 2868 7474 7073 3a2f  go.svg)](https:/
-000003c0: 2f6d 7962 696e 6465 722e 6f72 672f 7632  /mybinder.org/v2
-000003d0: 2f67 682f 7977 7836 3439 3939 3933 3131  /gh/ywx649999311
-000003e0: 2f45 7a54 616f 2f76 302e 342e 303f 6669  /EzTao/v0.4.0?fi
-000003f0: 6c65 7061 7468 3d64 6f63 732f 6e6f 7465  lepath=docs/note
-00000400: 626f 6f6b 7329 0a5b 215b 446f 6375 6d65  books).[![Docume
-00000410: 6e74 6174 696f 6e20 5374 6174 7573 5d28  ntation Status](
-00000420: 6874 7470 733a 2f2f 7265 6164 7468 6564  https://readthed
-00000430: 6f63 732e 6f72 672f 7072 6f6a 6563 7473  ocs.org/projects
-00000440: 2f65 7a74 616f 2f62 6164 6765 2f3f 7665  /eztao/badge/?ve
-00000450: 7273 696f 6e3d 6c61 7465 7374 295d 2868  rsion=latest)](h
-00000460: 7474 7073 3a2f 2f65 7a74 616f 2e72 6561  ttps://eztao.rea
-00000470: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000480: 6174 6573 742f 290a 2320 457a 5461 6f20  atest/).# EzTao 
-00000490: 28e6 9893 e981 9329 0a2a 2a45 7a54 616f  (......).**EzTao
-000004a0: 2a2a 2069 7320 6120 746f 6f6c 6b69 7420  ** is a toolkit 
-000004b0: 666f 7220 636f 6e64 7563 7469 6e67 2041  for conducting A
-000004c0: 474e 2074 696d 652d 7365 7269 6573 2f76  GN time-series/v
-000004d0: 6172 6961 6269 6c69 7479 2061 6e61 6c79  ariability analy
-000004e0: 7369 732c 206d 6169 6e6c 7920 7574 696c  sis, mainly util
-000004f0: 697a 696e 6720 7468 6520 636f 6e74 696e  izing the contin
-00000500: 756f 7573 2d74 696d 6520 6175 746f 2d72  uous-time auto-r
-00000510: 6567 7265 7373 6976 6520 6d6f 7669 6e67  egressive moving
-00000520: 2061 7665 7261 6765 206d 6f64 656c 2028   average model (
-00000530: 4341 524d 4129 0a0a 2323 2049 6e73 7461  CARMA)..## Insta
-00000540: 6c6c 6174 696f 6e0a 6060 600a 7069 7020  llation.```.pip 
-00000550: 696e 7374 616c 6c20 657a 7461 6f0a 6060  install eztao.``
-00000560: 600a 6f72 2028 6672 6f6d 206d 6173 7465  `.or (from maste
-00000570: 7229 0a60 6060 0a70 6970 2069 6e73 7461  r).```.pip insta
-00000580: 6c6c 2067 6974 2b68 7474 7073 3a2f 2f67  ll git+https://g
-00000590: 6974 6875 622e 636f 6d2f 7977 7836 3439  ithub.com/ywx649
-000005a0: 3939 3933 3131 2f45 7a54 616f 2e67 6974  999311/EzTao.git
-000005b0: 0a60 6060 0a23 2323 2044 6570 656e 6465  .```.### Depende
-000005c0: 6e63 6965 730a 3e60 6060 0a3e 7079 7468  ncies.>```.>pyth
-000005d0: 6f6e 203d 2022 5e33 2e37 220a 3e63 656c  on = "^3.7".>cel
-000005e0: 6572 6974 6520 3d20 223e 3d20 302e 332e  erite = ">= 0.3.
-000005f0: 3022 0a3e 6d61 7470 6c6f 746c 6962 203d  0".>matplotlib =
-00000600: 2022 5e33 2e33 2e30 220a 3e73 6369 7079   "^3.3.0".>scipy
-00000610: 203d 2022 3e20 312e 352e 3022 0a3e 6e75   = "> 1.5.0".>nu
-00000620: 6d62 6120 3d20 223e 3d20 302e 3531 2e30  mba = ">= 0.51.0
-00000630: 220a 3e65 6d63 6565 203d 2022 3e3d 332e  ".>emcee = ">=3.
-00000640: 302e 3022 0a3e 6060 600a 0a23 2323 2051  0.0".>```..### Q
-00000650: 7569 636b 2045 7861 6d70 6c65 730a 4c65  uick Examples.Le
-00000660: 7427 7320 6669 7273 7420 7369 6d75 6c61  t's first simula
-00000670: 7465 2061 2044 5257 2f43 4152 4d41 2831  te a DRW/CARMA(1
-00000680: 2c30 2920 7072 6f63 6573 7320 7769 7468  ,0) process with
-00000690: 2061 2076 6172 6961 6e63 6520 6f66 2030   a variance of 0
-000006a0: 2e33 5e32 2061 6e64 2061 2072 656c 6178  .3^2 and a relax
-000006b0: 6174 696f 6e20 7469 6d65 7363 616c 6520  ation timescale 
-000006c0: 6f66 2031 3030 2064 6179 732e 2054 6869  of 100 days. Thi
-000006d0: 7320 7469 6d65 2073 6572 6965 7320 7769  s time series wi
-000006e0: 6c6c 2068 6176 6520 6120 746f 7461 6c20  ll have a total 
-000006f0: 6f66 2032 3030 2064 6174 6120 706f 696e  of 200 data poin
-00000700: 7473 2061 6e64 2073 7061 6e20 3130 2079  ts and span 10 y
-00000710: 6561 7273 2e0a 6060 6070 7974 686f 6e0a  ears..```python.
-00000720: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-00000730: 6e70 0a69 6d70 6f72 7420 6d61 7470 6c6f  np.import matplo
-00000740: 746c 6962 2e70 7970 6c6f 7420 6173 2070  tlib.pyplot as p
-00000750: 6c74 0a66 726f 6d20 657a 7461 6f2e 6361  lt.from eztao.ca
-00000760: 726d 6120 696d 706f 7274 2044 5257 5f74  rma import DRW_t
-00000770: 6572 6d0a 6672 6f6d 2065 7a74 616f 2e74  erm.from eztao.t
-00000780: 7320 696d 706f 7274 2067 7053 696d 5261  s import gpSimRa
-00000790: 6e64 0a0a 2320 6465 6669 6e65 2061 2044  nd..# define a D
-000007a0: 5257 206b 6572 6e65 6c20 2620 616e 6420  RW kernel & and 
-000007b0: 7369 6d75 6c61 7465 2061 2070 726f 6365  simulate a proce
-000007c0: 7373 0a61 6d70 203d 2030 2e32 0a74 6175  ss.amp = 0.2.tau
-000007d0: 203d 2031 3030 0a44 5257 5f6b 6572 6e65   = 100.DRW_kerne
-000007e0: 6c20 3d20 4452 575f 7465 726d 286e 702e  l = DRW_term(np.
-000007f0: 6c6f 6728 616d 7029 2c20 6e70 2e6c 6f67  log(amp), np.log
-00000800: 2874 6175 2929 0a74 2c20 792c 2079 6572  (tau)).t, y, yer
-00000810: 7220 3d20 6770 5369 6d52 616e 6428 4452  r = gpSimRand(DR
-00000820: 575f 6b65 726e 656c 2c20 3130 2c20 3336  W_kernel, 10, 36
-00000830: 352a 3130 2c20 3230 3029 0a0a 2320 6e6f  5*10, 200)..# no
-00000840: 772c 2070 6c6f 7420 6974 0a66 6967 2c20  w, plot it.fig, 
-00000850: 6178 203d 2070 6c74 2e73 7562 706c 6f74  ax = plt.subplot
-00000860: 7328 312c 312c 2064 7069 3d31 3530 2c20  s(1,1, dpi=150, 
-00000870: 6669 6773 697a 653d 2838 2c33 2929 0a61  figsize=(8,3)).a
-00000880: 782e 6572 726f 7262 6172 2874 2c20 792c  x.errorbar(t, y,
-00000890: 2079 6572 722c 2066 6d74 3d27 2e27 290a   yerr, fmt='.').
-000008a0: 2e2e 2e0a 6060 600a 215b 6472 775f 7369  ....```.![drw_si
-000008b0: 6d5d 2869 6e63 6c75 6465 2f64 7277 5f73  m](include/drw_s
-000008c0: 696d 2e70 6e67 290a 0a57 6520 6361 6e20  im.png)..We can 
-000008d0: 6669 7420 7468 6520 7369 6d75 6c61 7465  fit the simulate
-000008e0: 6420 7469 6d65 2073 6572 6965 7320 746f  d time series to
-000008f0: 2074 6865 2044 5257 206d 6f64 656c 2061   the DRW model a
-00000900: 6e64 2073 6565 2068 6f77 2077 656c 6c20  nd see how well 
-00000910: 7765 2063 616e 2072 6563 6f76 6572 2074  we can recover t
-00000920: 6865 2069 6e70 7574 2070 6172 616d 6574  he input paramet
-00000930: 6572 732e 0a60 6060 7079 7468 6f6e 0a66  ers..```python.f
-00000940: 726f 6d20 657a 7461 6f2e 7473 2069 6d70  rom eztao.ts imp
-00000950: 6f72 7420 6472 775f 6669 740a 0a62 6573  ort drw_fit..bes
-00000960: 745f 6669 7420 3d20 6472 775f 6669 7428  t_fit = drw_fit(
-00000970: 742c 2079 2c20 7965 7272 290a 7072 696e  t, y, yerr).prin
-00000980: 7428 6627 4265 7374 2d66 6974 2044 5257  t(f'Best-fit DRW
-00000990: 2070 6172 616d 6574 6572 733a 207b 6265   parameters: {be
-000009a0: 7374 5f66 6974 7d27 290a 6060 600a 6060  st_fit}').```.``
-000009b0: 6073 6865 6c6c 0a42 6573 742d 6669 7420  `shell.Best-fit 
-000009c0: 4452 5720 7061 7261 6d65 7465 7273 3a20  DRW parameters: 
-000009d0: 5b30 2e31 3733 3536 3938 3320 3838 2e33  [0.17356983 88.3
-000009e0: 3632 3632 3436 375d 0a60 6060 0a0a 486f  6262467].```..Ho
-000009f0: 7720 646f 6573 2074 6865 2070 6f77 6572  w does the power
-00000a00: 2073 7065 6374 7275 6d20 6465 6e73 6974   spectrum densit
-00000a10: 7920 2850 5344 2920 636f 6d70 6172 653f  y (PSD) compare?
-00000a20: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00000a30: 657a 7461 6f2e 6361 726d 6120 696d 706f  eztao.carma impo
-00000a40: 7274 2067 705f 7073 640a 0a23 2067 6574  rt gp_psd..# get
-00000a50: 2070 7364 2066 756e 6374 696f 6e73 0a74   psd functions.t
-00000a60: 7275 655f 7073 6420 3d20 6770 5f70 7364  rue_psd = gp_psd
-00000a70: 2844 5257 5f6b 6572 6e65 6c29 0a62 6573  (DRW_kernel).bes
-00000a80: 745f 7073 6420 3d20 6770 5f70 7364 2844  t_psd = gp_psd(D
-00000a90: 5257 5f74 6572 6d28 2a6e 702e 6c6f 6728  RW_term(*np.log(
-00000aa0: 6265 7374 5f66 6974 2929 290a 0a23 2070  best_fit)))..# p
-00000ab0: 6c6f 740a 6669 672c 2061 7820 3d20 706c  lot.fig, ax = pl
-00000ac0: 742e 7375 6270 6c6f 7473 2831 2c31 2c20  t.subplots(1,1, 
-00000ad0: 6470 693d 3135 302c 2066 6967 7369 7a65  dpi=150, figsize
-00000ae0: 3d28 362c 3329 290a 6672 6571 203d 206e  =(6,3)).freq = n
-00000af0: 702e 6c6f 6773 7061 6365 282d 352c 2032  p.logspace(-5, 2
-00000b00: 290a 6178 2e70 6c6f 7428 6672 6571 2c20  ).ax.plot(freq, 
-00000b10: 7472 7565 5f70 7364 2866 7265 7129 2c20  true_psd(freq), 
-00000b20: 6c61 6265 6c3d 2749 6e70 7574 2050 5344  label='Input PSD
-00000b30: 2729 0a61 782e 706c 6f74 2866 7265 712c  ').ax.plot(freq,
-00000b40: 2062 6573 745f 7073 6428 6672 6571 292c   best_psd(freq),
-00000b50: 206c 6162 656c 3d27 4265 7374 2d66 6974   label='Best-fit
-00000b60: 2050 5344 2729 0a2e 2e2e 0a60 6060 0a21   PSD').....```.!
-00000b70: 5b64 7277 5f70 7364 5d28 696e 636c 7564  [drw_psd](includ
-00000b80: 652f 6472 775f 7073 642e 706e 6729 0a0a  e/drw_psd.png)..
-00000b90: 5f5f 4e6f 7465 3a5f 5f20 486f 7720 7765  __Note:__ How we
-00000ba0: 6c6c 2074 6865 2069 6e70 7574 2061 6e64  ll the input and
-00000bb0: 2062 6573 742d 6669 7420 5053 4420 6d61   best-fit PSD ma
-00000bc0: 7463 6820 6973 2075 7020 746f 2068 6f77  tch is up to how
-00000bd0: 2067 6f6f 6420 7468 6520 6265 7374 2d66   good the best-f
-00000be0: 6974 2070 6172 616d 6574 6572 7320 6172  it parameters ar
-00000bf0: 652c 2077 6869 6368 2069 7320 6869 6768  e, which is high
-00000c00: 6c79 2069 6e66 6c75 656e 6365 6420 6279  ly influenced by
-00000c10: 2074 6865 2071 7561 6c69 7479 206f 6620   the quality of 
-00000c20: 7468 6520 696e 7075 7420 7469 6d65 2073  the input time s
-00000c30: 6572 6965 732e 200a 0a46 6f72 206d 6f72  eries. ..For mor
-00000c40: 6520 6578 616d 706c 6573 2c20 706c 6561  e examples, plea
-00000c50: 7365 2063 6865 636b 206f 7574 2074 6865  se check out the
-00000c60: 205b 6f6e 6c69 6e65 2064 6f63 756d 656e   [online documen
-00000c70: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-00000c80: 657a 7461 6f2e 7265 6164 7468 6564 6f63  eztao.readthedoc
-00000c90: 732e 696f 2f65 6e2f 6c61 7465 7374 2f29  s.io/en/latest/)
-00000ca0: 206f 7220 7275 6e20 7468 6520 7475 746f   or run the tuto
-00000cb0: 7269 616c 206e 6f74 6562 6f6f 6b73 2061  rial notebooks a
-00000cc0: 7420 2d3e 0a5b 215b 4269 6e64 6572 5d28  t ->.[![Binder](
-00000cd0: 6874 7470 733a 2f2f 6d79 6269 6e64 6572  https://mybinder
-00000ce0: 2e6f 7267 2f62 6164 6765 5f6c 6f67 6f2e  .org/badge_logo.
-00000cf0: 7376 6729 5d28 6874 7470 733a 2f2f 6d79  svg)](https://my
-00000d00: 6269 6e64 6572 2e6f 7267 2f76 322f 6768  binder.org/v2/gh
-00000d10: 2f79 7778 3634 3939 3939 3331 312f 457a  /ywx649999311/Ez
-00000d20: 5461 6f2f 7630 2e33 2e30 3f66 696c 6570  Tao/v0.3.0?filep
-00000d30: 6174 683d 646f 6373 2f6e 6f74 6562 6f6f  ath=docs/noteboo
-00000d40: 6b73 292e 0a0a 2323 2320 4465 7665 6c6f  ks)...### Develo
-00000d50: 706d 656e 740a 6070 6f65 7472 7960 2069  pment.`poetry` i
-00000d60: 7320 7573 6564 2074 6f20 736f 6c76 6520  s used to solve 
-00000d70: 6465 7065 6e64 656e 6369 6573 2061 6e64  dependencies and
-00000d80: 2074 6f20 6275 696c 642f 7075 626c 6973   to build/publis
-00000d90: 6820 7468 6973 2070 6163 6b61 6765 2e20  h this package. 
-00000da0: 4265 6c6f 7720 7368 6f77 7320 686f 7720  Below shows how 
-00000db0: 7365 7475 7020 7468 6520 656e 7669 726f  setup the enviro
-00000dc0: 6e6d 656e 7420 666f 7220 6465 7665 6c6f  nment for develo
-00000dd0: 706d 656e 7420 2861 7373 756d 696e 6720  pment (assuming 
-00000de0: 796f 7520 616c 7265 6164 7920 6861 7665  you already have
-00000df0: 2060 706f 6574 7279 6020 696e 7374 616c   `poetry` instal
-00000e00: 6c65 6420 6f6e 2079 6f75 7220 6d61 6368  led on your mach
-00000e10: 696e 6529 2e20 0a0a 312e 2043 6c6f 6e65  ine). ..1. Clone
-00000e20: 2074 6869 7320 7265 706f 7369 746f 7279   this repository
-00000e30: 2c20 616e 6420 656e 7465 7220 7468 6520  , and enter the 
-00000e40: 7265 706f 7369 746f 7279 2066 6f6c 6465  repository folde
-00000e50: 722e 0a32 2e20 4372 6561 7465 2061 2070  r..2. Create a p
-00000e60: 7974 686f 6e20 7669 7274 7561 6c20 656e  ython virtual en
-00000e70: 7669 726f 6e6d 656e 7420 616e 6420 6163  vironment and ac
-00000e80: 7469 7661 7465 2069 7420 2874 6865 2076  tivate it (the v
-00000e90: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
-00000ea0: 6e74 206e 616d 6520 6d75 7374 2062 6520  nt name must be 
-00000eb0: 272e 7665 6e76 2729 2e20 0a20 2020 2060  '.venv'). .    `
-00000ec0: 6060 0a20 2020 2070 7974 686f 6e20 2d6d  ``.    python -m
-00000ed0: 2076 656e 7620 2e76 656e 760a 2020 2020   venv .venv.    
-00000ee0: 736f 7572 6365 202e 7665 6e76 2f62 696e  source .venv/bin
-00000ef0: 2f61 6374 6976 6174 650a 2020 2020 6060  /activate.    ``
-00000f00: 600a 332e 2049 6e73 7461 6c6c 2064 6570  `.3. Install dep
-00000f10: 656e 6465 6e63 6965 7320 616e 6420 2a2a  endencies and **
-00000f20: 457a 5461 6f2a 2a20 696e 2065 6469 7461  EzTao** in edita
-00000f30: 626c 6520 6d6f 6465 2e0a 2020 2060 6060  ble mode..   ```
-00000f40: 0a20 2020 706f 6574 7279 2069 6e73 7461  .   poetry insta
-00000f50: 6c6c 0a20 2020 6060 600a 0a4e 6f77 2079  ll.   ```..Now y
-00000f60: 6f75 2073 686f 756c 6420 6265 2072 6561  ou should be rea
-00000f70: 6479 2074 6f20 7374 6172 7420 6164 6469  dy to start addi
-00000f80: 6e67 206e 6577 2066 6561 7475 7265 732e  ng new features.
-00000f90: 2042 6520 7375 7265 2074 6f20 6368 6563   Be sure to chec
-00000fa0: 6b6f 7574 2074 6865 206e 6f72 6d61 6c20  kout the normal 
-00000fb0: 7072 6163 7469 6365 2072 6567 6172 6469  practice regardi
-00000fc0: 6e67 2068 6f77 2074 6f20 7573 6520 6070  ng how to use `p
-00000fd0: 6f65 7472 7960 206f 6e20 6974 7320 7765  oetry` on its we
-00000fe0: 6273 6974 652e 2057 6865 6e20 796f 7520  bsite. When you 
-00000ff0: 6172 6520 7265 6164 7920 746f 2070 7573  are ready to pus
-00001000: 682c 2061 6c73 6f20 6d61 6b65 2073 7572  h, also make sur
-00001010: 6520 7468 6520 706f 6574 7279 2e6c 6f63  e the poetry.loc
-00001020: 6b20 6669 6c65 2069 7320 6368 6563 6b65  k file is checke
-00001030: 642d 696e 2069 6620 616e 7920 6465 7065  d-in if any depe
-00001040: 6e64 656e 6379 2068 6173 2063 6861 6e67  ndency has chang
-00001050: 6564 2e20 0a0a                           ed. ..
+00000200: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000210: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000220: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000230: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00000240: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000250: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000260: 2033 2e31 310a 5265 7175 6972 6573 2d44   3.11.Requires-D
+00000270: 6973 743a 2063 656c 6572 6974 6520 283e  ist: celerite (>
+00000280: 3d30 2e33 2e30 290a 5265 7175 6972 6573  =0.3.0).Requires
+00000290: 2d44 6973 743a 2065 6d63 6565 2028 3e3d  -Dist: emcee (>=
+000002a0: 332e 302e 3029 0a52 6571 7569 7265 732d  3.0.0).Requires-
+000002b0: 4469 7374 3a20 696d 706f 7274 6c69 622d  Dist: importlib-
+000002c0: 6d65 7461 6461 7461 2028 3e3d 322e 302e  metadata (>=2.0.
+000002d0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+000002e0: 3a20 6d61 7470 6c6f 746c 6962 2028 3e3d  : matplotlib (>=
+000002f0: 332e 332e 302c 3c34 2e30 2e30 290a 5265  3.3.0,<4.0.0).Re
+00000300: 7175 6972 6573 2d44 6973 743a 206e 756d  quires-Dist: num
+00000310: 6261 2028 3e3d 302e 3531 2e30 290a 5265  ba (>=0.51.0).Re
+00000320: 7175 6972 6573 2d44 6973 743a 2073 6369  quires-Dist: sci
+00000330: 7079 2028 3e3d 312e 3529 0a50 726f 6a65  py (>=1.5).Proje
+00000340: 6374 2d55 524c 3a20 5265 706f 7369 746f  ct-URL: Reposito
+00000350: 7279 2c20 6874 7470 733a 2f2f 6769 7468  ry, https://gith
+00000360: 7562 2e63 6f6d 2f79 7778 3634 3939 3939  ub.com/ywx649999
+00000370: 3331 312f 457a 5461 6f0a 4465 7363 7269  311/EzTao.Descri
+00000380: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+00000390: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+000003a0: 6e0a 0a21 5b74 6573 7473 5d28 6874 7470  n..![tests](http
+000003b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
+000003c0: 7778 3634 3939 3939 3331 312f 457a 5461  wx649999311/EzTa
+000003d0: 6f2f 776f 726b 666c 6f77 732f 7465 7374  o/workflows/test
+000003e0: 732f 6261 6467 652e 7376 6729 0a5b 215b  s/badge.svg).[![
+000003f0: 4269 6e64 6572 5d28 6874 7470 733a 2f2f  Binder](https://
+00000400: 6d79 6269 6e64 6572 2e6f 7267 2f62 6164  mybinder.org/bad
+00000410: 6765 5f6c 6f67 6f2e 7376 6729 5d28 6874  ge_logo.svg)](ht
+00000420: 7470 733a 2f2f 6d79 6269 6e64 6572 2e6f  tps://mybinder.o
+00000430: 7267 2f76 322f 6768 2f79 7778 3634 3939  rg/v2/gh/ywx6499
+00000440: 3939 3331 312f 457a 5461 6f2f 7630 2e34  99311/EzTao/v0.4
+00000450: 2e31 3f66 696c 6570 6174 683d 646f 6373  .1?filepath=docs
+00000460: 2f6e 6f74 6562 6f6f 6b73 290a 5b21 5b44  /notebooks).[![D
+00000470: 6f63 756d 656e 7461 7469 6f6e 2053 7461  ocumentation Sta
+00000480: 7475 735d 2868 7474 7073 3a2f 2f72 6561  tus](https://rea
+00000490: 6474 6865 646f 6373 2e6f 7267 2f70 726f  dthedocs.org/pro
+000004a0: 6a65 6374 732f 657a 7461 6f2f 6261 6467  jects/eztao/badg
+000004b0: 652f 3f76 6572 7369 6f6e 3d6c 6174 6573  e/?version=lates
+000004c0: 7429 5d28 6874 7470 733a 2f2f 657a 7461  t)](https://ezta
+000004d0: 6f2e 7265 6164 7468 6564 6f63 732e 696f  o.readthedocs.io
+000004e0: 2f65 6e2f 6c61 7465 7374 2f29 0a3c 6120  /en/latest/).<a 
+000004f0: 6872 6566 3d22 6874 7470 733a 2f2f 6173  href="https://as
+00000500: 636c 2e6e 6574 2f32 3230 312e 3030 3122  cl.net/2201.001"
+00000510: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000520: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000530: 6f2f 6261 6467 652f 6173 636c 2d32 3230  o/badge/ascl-220
+00000540: 312e 3030 312d 626c 7565 2e73 7667 3f63  1.001-blue.svg?c
+00000550: 6f6c 6f72 423d 3236 3232 3535 2220 616c  olorB=262255" al
+00000560: 743d 2261 7363 6c3a 3232 3031 2e30 3031  t="ascl:2201.001
+00000570: 2220 2f3e 3c2f 613e 0a23 2045 7a54 616f  " /></a>.# EzTao
+00000580: 2028 e698 93e9 8193 290a 2a2a 457a 5461   (......).**EzTa
+00000590: 6f2a 2a20 6973 2061 2074 6f6f 6c6b 6974  o** is a toolkit
+000005a0: 2066 6f72 2063 6f6e 6475 6374 696e 6720   for conducting 
+000005b0: 4147 4e20 7469 6d65 2d73 6572 6965 732f  AGN time-series/
+000005c0: 7661 7269 6162 696c 6974 7920 616e 616c  variability anal
+000005d0: 7973 6973 2c20 6d61 696e 6c79 2075 7469  ysis, mainly uti
+000005e0: 6c69 7a69 6e67 2074 6865 2063 6f6e 7469  lizing the conti
+000005f0: 6e75 6f75 732d 7469 6d65 2061 7574 6f2d  nuous-time auto-
+00000600: 7265 6772 6573 7369 7665 206d 6f76 696e  regressive movin
+00000610: 6720 6176 6572 6167 6520 6d6f 6465 6c20  g average model 
+00000620: 2843 4152 4d41 290a 0a23 2320 496e 7374  (CARMA)..## Inst
+00000630: 616c 6c61 7469 6f6e 0a3c 212d 2d2d 2060  allation.<!--- `
+00000640: 6060 0a70 6970 2069 6e73 7461 6c6c 2065  ``.pip install e
+00000650: 7a74 616f 0a60 6060 0a6f 7220 2866 726f  ztao.```.or (fro
+00000660: 6d20 6d61 7374 6572 292d 2d2d 3e0a 6060  m master)--->.``
+00000670: 600a 7069 7020 696e 7374 616c 6c20 6769  `.pip install gi
+00000680: 742b 6874 7470 733a 2f2f 6769 7468 7562  t+https://github
+00000690: 2e63 6f6d 2f79 7778 3634 3939 3939 3331  .com/ywx64999931
+000006a0: 312f 457a 5461 6f2e 6769 740a 6060 600a  1/EzTao.git.```.
+000006b0: 2323 2320 4465 7065 6e64 656e 6369 6573  ### Dependencies
+000006c0: 0a3e 6060 600a 3e70 7974 686f 6e20 3d20  .>```.>python = 
+000006d0: 225e 332e 3722 0a3e 6365 6c65 7269 7465  "^3.7".>celerite
+000006e0: 203d 2022 3e3d 2030 2e33 2e30 220a 3e6d   = ">= 0.3.0".>m
+000006f0: 6174 706c 6f74 6c69 6220 3d20 225e 332e  atplotlib = "^3.
+00000700: 332e 3022 0a3e 7363 6970 7920 3d20 223e  3.0".>scipy = ">
+00000710: 2031 2e35 2e30 220a 3e6e 756d 6261 203d   1.5.0".>numba =
+00000720: 2022 3e3d 2030 2e35 312e 3022 0a3e 656d   ">= 0.51.0".>em
+00000730: 6365 6520 3d20 223e 3d33 2e30 2e30 220a  cee = ">=3.0.0".
+00000740: 3e60 6060 0a0a 2323 2051 7569 636b 2045  >```..## Quick E
+00000750: 7861 6d70 6c65 730a 4c65 7427 7320 6669  xamples.Let's fi
+00000760: 7273 7420 7369 6d75 6c61 7465 2061 2044  rst simulate a D
+00000770: 5257 2f43 4152 4d41 2831 2c30 2920 7072  RW/CARMA(1,0) pr
+00000780: 6f63 6573 7320 7769 7468 2061 2076 6172  ocess with a var
+00000790: 6961 6e63 6520 6f66 2030 2e33 5e32 2061  iance of 0.3^2 a
+000007a0: 6e64 2061 2072 656c 6178 6174 696f 6e20  nd a relaxation 
+000007b0: 7469 6d65 7363 616c 6520 6f66 2031 3030  timescale of 100
+000007c0: 2064 6179 732e 2054 6869 7320 7469 6d65   days. This time
+000007d0: 2073 6572 6965 7320 7769 6c6c 2068 6176   series will hav
+000007e0: 6520 6120 746f 7461 6c20 6f66 2032 3030  e a total of 200
+000007f0: 2064 6174 6120 706f 696e 7473 2061 6e64   data points and
+00000800: 2073 7061 6e20 3130 2079 6561 7273 2e0a   span 10 years..
+00000810: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00000820: 206e 756d 7079 2061 7320 6e70 0a69 6d70   numpy as np.imp
+00000830: 6f72 7420 6d61 7470 6c6f 746c 6962 2e70  ort matplotlib.p
+00000840: 7970 6c6f 7420 6173 2070 6c74 0a66 726f  yplot as plt.fro
+00000850: 6d20 657a 7461 6f2e 6361 726d 6120 696d  m eztao.carma im
+00000860: 706f 7274 2044 5257 5f74 6572 6d0a 6672  port DRW_term.fr
+00000870: 6f6d 2065 7a74 616f 2e74 7320 696d 706f  om eztao.ts impo
+00000880: 7274 2067 7053 696d 5261 6e64 0a0a 2320  rt gpSimRand..# 
+00000890: 6465 6669 6e65 2061 2044 5257 206b 6572  define a DRW ker
+000008a0: 6e65 6c20 2620 616e 6420 7369 6d75 6c61  nel & and simula
+000008b0: 7465 2061 2070 726f 6365 7373 0a61 6d70  te a process.amp
+000008c0: 203d 2030 2e32 0a74 6175 203d 2031 3030   = 0.2.tau = 100
+000008d0: 0a44 5257 5f6b 6572 6e65 6c20 3d20 4452  .DRW_kernel = DR
+000008e0: 575f 7465 726d 286e 702e 6c6f 6728 616d  W_term(np.log(am
+000008f0: 7029 2c20 6e70 2e6c 6f67 2874 6175 2929  p), np.log(tau))
+00000900: 0a74 2c20 792c 2079 6572 7220 3d20 6770  .t, y, yerr = gp
+00000910: 5369 6d52 616e 6428 4452 575f 6b65 726e  SimRand(DRW_kern
+00000920: 656c 2c20 3130 2c20 3336 352a 3130 2c20  el, 10, 365*10, 
+00000930: 3230 3029 0a0a 2320 6e6f 772c 2070 6c6f  200)..# now, plo
+00000940: 7420 6974 0a66 6967 2c20 6178 203d 2070  t it.fig, ax = p
+00000950: 6c74 2e73 7562 706c 6f74 7328 312c 312c  lt.subplots(1,1,
+00000960: 2064 7069 3d31 3530 2c20 6669 6773 697a   dpi=150, figsiz
+00000970: 653d 2838 2c33 2929 0a61 782e 6572 726f  e=(8,3)).ax.erro
+00000980: 7262 6172 2874 2c20 792c 2079 6572 722c  rbar(t, y, yerr,
+00000990: 2066 6d74 3d27 2e27 290a 2e2e 2e0a 6060   fmt='.').....``
+000009a0: 600a 215b 6472 775f 7369 6d5d 2869 6e63  `.![drw_sim](inc
+000009b0: 6c75 6465 2f64 7277 5f73 696d 2e70 6e67  lude/drw_sim.png
+000009c0: 290a 0a57 6520 6361 6e20 6669 7420 7468  )..We can fit th
+000009d0: 6520 7369 6d75 6c61 7465 6420 7469 6d65  e simulated time
+000009e0: 2073 6572 6965 7320 746f 2074 6865 2044   series to the D
+000009f0: 5257 206d 6f64 656c 2061 6e64 2073 6565  RW model and see
+00000a00: 2068 6f77 2077 656c 6c20 7765 2063 616e   how well we can
+00000a10: 2072 6563 6f76 6572 2074 6865 2069 6e70   recover the inp
+00000a20: 7574 2070 6172 616d 6574 6572 732e 0a60  ut parameters..`
+00000a30: 6060 7079 7468 6f6e 0a66 726f 6d20 657a  ``python.from ez
+00000a40: 7461 6f2e 7473 2069 6d70 6f72 7420 6472  tao.ts import dr
+00000a50: 775f 6669 740a 0a62 6573 745f 6669 7420  w_fit..best_fit 
+00000a60: 3d20 6472 775f 6669 7428 742c 2079 2c20  = drw_fit(t, y, 
+00000a70: 7965 7272 290a 7072 696e 7428 6627 4265  yerr).print(f'Be
+00000a80: 7374 2d66 6974 2044 5257 2070 6172 616d  st-fit DRW param
+00000a90: 6574 6572 733a 207b 6265 7374 5f66 6974  eters: {best_fit
+00000aa0: 7d27 290a 6060 600a 6060 6073 6865 6c6c  }').```.```shell
+00000ab0: 0a42 6573 742d 6669 7420 4452 5720 7061  .Best-fit DRW pa
+00000ac0: 7261 6d65 7465 7273 3a20 5b30 2e31 3733  rameters: [0.173
+00000ad0: 3536 3938 3320 3838 2e33 3632 3632 3436  56983 88.3626246
+00000ae0: 375d 0a60 6060 0a0a 486f 7720 646f 6573  7].```..How does
+00000af0: 2074 6865 2070 6f77 6572 2073 7065 6374   the power spect
+00000b00: 7275 6d20 6465 6e73 6974 7920 2850 5344  rum density (PSD
+00000b10: 2920 636f 6d70 6172 653f 0a60 6060 7079  ) compare?.```py
+00000b20: 7468 6f6e 0a66 726f 6d20 657a 7461 6f2e  thon.from eztao.
+00000b30: 6361 726d 6120 696d 706f 7274 2067 705f  carma import gp_
+00000b40: 7073 640a 0a23 2067 6574 2070 7364 2066  psd..# get psd f
+00000b50: 756e 6374 696f 6e73 0a74 7275 655f 7073  unctions.true_ps
+00000b60: 6420 3d20 6770 5f70 7364 2844 5257 5f6b  d = gp_psd(DRW_k
+00000b70: 6572 6e65 6c29 0a62 6573 745f 7073 6420  ernel).best_psd 
+00000b80: 3d20 6770 5f70 7364 2844 5257 5f74 6572  = gp_psd(DRW_ter
+00000b90: 6d28 2a6e 702e 6c6f 6728 6265 7374 5f66  m(*np.log(best_f
+00000ba0: 6974 2929 290a 0a23 2070 6c6f 740a 6669  it)))..# plot.fi
+00000bb0: 672c 2061 7820 3d20 706c 742e 7375 6270  g, ax = plt.subp
+00000bc0: 6c6f 7473 2831 2c31 2c20 6470 693d 3135  lots(1,1, dpi=15
+00000bd0: 302c 2066 6967 7369 7a65 3d28 362c 3329  0, figsize=(6,3)
+00000be0: 290a 6672 6571 203d 206e 702e 6c6f 6773  ).freq = np.logs
+00000bf0: 7061 6365 282d 352c 2032 290a 6178 2e70  pace(-5, 2).ax.p
+00000c00: 6c6f 7428 6672 6571 2c20 7472 7565 5f70  lot(freq, true_p
+00000c10: 7364 2866 7265 7129 2c20 6c61 6265 6c3d  sd(freq), label=
+00000c20: 2749 6e70 7574 2050 5344 2729 0a61 782e  'Input PSD').ax.
+00000c30: 706c 6f74 2866 7265 712c 2062 6573 745f  plot(freq, best_
+00000c40: 7073 6428 6672 6571 292c 206c 6162 656c  psd(freq), label
+00000c50: 3d27 4265 7374 2d66 6974 2050 5344 2729  ='Best-fit PSD')
+00000c60: 0a2e 2e2e 0a60 6060 0a21 5b64 7277 5f70  .....```.![drw_p
+00000c70: 7364 5d28 696e 636c 7564 652f 6472 775f  sd](include/drw_
+00000c80: 7073 642e 706e 6729 0a0a 5f5f 4e6f 7465  psd.png)..__Note
+00000c90: 3a5f 5f20 486f 7720 7765 6c6c 2074 6865  :__ How well the
+00000ca0: 2069 6e70 7574 2061 6e64 2062 6573 742d   input and best-
+00000cb0: 6669 7420 5053 4420 6d61 7463 6820 6973  fit PSD match is
+00000cc0: 2075 7020 746f 2068 6f77 2067 6f6f 6420   up to how good 
+00000cd0: 7468 6520 6265 7374 2d66 6974 2070 6172  the best-fit par
+00000ce0: 616d 6574 6572 7320 6172 652c 2077 6869  ameters are, whi
+00000cf0: 6368 2069 7320 6869 6768 6c79 2069 6e66  ch is highly inf
+00000d00: 6c75 656e 6365 6420 6279 2074 6865 2071  luenced by the q
+00000d10: 7561 6c69 7479 206f 6620 7468 6520 696e  uality of the in
+00000d20: 7075 7420 7469 6d65 2073 6572 6965 732e  put time series.
+00000d30: 200a 0a46 6f72 206d 6f72 6520 6578 616d   ..For more exam
+00000d40: 706c 6573 2c20 706c 6561 7365 2063 6865  ples, please che
+00000d50: 636b 206f 7574 2074 6865 205b 6f6e 6c69  ck out the [onli
+00000d60: 6e65 2064 6f63 756d 656e 7461 7469 6f6e  ne documentation
+00000d70: 5d28 6874 7470 733a 2f2f 657a 7461 6f2e  ](https://eztao.
+00000d80: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00000d90: 6e2f 6c61 7465 7374 2f29 206f 7220 7275  n/latest/) or ru
+00000da0: 6e20 7468 6520 7475 746f 7269 616c 206e  n the tutorial n
+00000db0: 6f74 6562 6f6f 6b73 2061 7420 2d3e 0a5b  otebooks at ->.[
+00000dc0: 215b 4269 6e64 6572 5d28 6874 7470 733a  ![Binder](https:
+00000dd0: 2f2f 6d79 6269 6e64 6572 2e6f 7267 2f62  //mybinder.org/b
+00000de0: 6164 6765 5f6c 6f67 6f2e 7376 6729 5d28  adge_logo.svg)](
+00000df0: 6874 7470 733a 2f2f 6d79 6269 6e64 6572  https://mybinder
+00000e00: 2e6f 7267 2f76 322f 6768 2f79 7778 3634  .org/v2/gh/ywx64
+00000e10: 3939 3939 3331 312f 457a 5461 6f2f 7630  9999311/EzTao/v0
+00000e20: 2e34 2e30 3f66 696c 6570 6174 683d 646f  .4.0?filepath=do
+00000e30: 6373 2f6e 6f74 6562 6f6f 6b73 292e 0a0a  cs/notebooks)...
+00000e40: 2323 2044 6576 656c 6f70 6d65 6e74 0a60  ## Development.`
+00000e50: 706f 6574 7279 6020 6973 2075 7365 6420  poetry` is used 
+00000e60: 746f 2073 6f6c 7665 2064 6570 656e 6465  to solve depende
+00000e70: 6e63 6965 7320 616e 6420 746f 2062 7569  ncies and to bui
+00000e80: 6c64 2f70 7562 6c69 7368 2074 6869 7320  ld/publish this 
+00000e90: 7061 636b 6167 652e 2042 656c 6f77 2073  package. Below s
+00000ea0: 686f 7773 2068 6f77 2073 6574 7570 2074  hows how setup t
+00000eb0: 6865 2065 6e76 6972 6f6e 6d65 6e74 2066  he environment f
+00000ec0: 6f72 2064 6576 656c 6f70 6d65 6e74 2028  or development (
+00000ed0: 6173 7375 6d69 6e67 2079 6f75 2061 6c72  assuming you alr
+00000ee0: 6561 6479 2068 6176 6520 6070 6f65 7472  eady have `poetr
+00000ef0: 7960 2069 6e73 7461 6c6c 6564 206f 6e20  y` installed on 
+00000f00: 796f 7572 206d 6163 6869 6e65 292e 205f  your machine). _
+00000f10: 2a2a 5761 726e 696e 673a 2a2a 5f20 6070  **Warning:**_ `p
+00000f20: 6f65 7472 7960 2069 7320 6861 7669 6e67  oetry` is having
+00000f30: 2069 7373 7565 2069 6e73 7461 6c6c 696e   issue installin
+00000f40: 6720 606c 6c76 6d6c 6974 6520 3d20 302e  g `llvmlite = 0.
+00000f50: 3334 2e30 6020 2875 7365 6420 666f 7220  34.0` (used for 
+00000f60: 6065 7a74 616f 203d 205e 302e 342e 3060  `eztao = ^0.4.0`
+00000f70: 2920 756e 6465 7220 5079 7468 6f6e 2033  ) under Python 3
+00000f80: 2e39 2e20 5468 6520 6973 7375 6520 6469  .9. The issue di
+00000f90: 7361 7070 6561 7273 2066 6f72 2050 7974  sappears for Pyt
+00000fa0: 686f 6e20 332e 382e 0a0a 312e 2043 6c6f  hon 3.8...1. Clo
+00000fb0: 6e65 2074 6869 7320 7265 706f 7369 746f  ne this reposito
+00000fc0: 7279 2c20 616e 6420 656e 7465 7220 7468  ry, and enter th
+00000fd0: 6520 7265 706f 7369 746f 7279 2066 6f6c  e repository fol
+00000fe0: 6465 722e 0a32 2e20 4372 6561 7465 2061  der..2. Create a
+00000ff0: 2070 7974 686f 6e20 7669 7274 7561 6c20   python virtual 
+00001000: 656e 7669 726f 6e6d 656e 7420 616e 6420  environment and 
+00001010: 6163 7469 7661 7465 2069 7420 2874 6865  activate it (the
+00001020: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
+00001030: 6d65 6e74 206e 616d 6520 6d75 7374 2062  ment name must b
+00001040: 6520 272e 7665 6e76 2729 2e20 0a20 2020  e '.venv'). .   
+00001050: 2060 6060 0a20 2020 2070 7974 686f 6e20   ```.    python 
+00001060: 2d6d 2076 656e 7620 2e76 656e 760a 2020  -m venv .venv.  
+00001070: 2020 736f 7572 6365 202e 7665 6e76 2f62    source .venv/b
+00001080: 696e 2f61 6374 6976 6174 650a 2020 2020  in/activate.    
+00001090: 6060 600a 332e 2049 6e73 7461 6c6c 2064  ```.3. Install d
+000010a0: 6570 656e 6465 6e63 6965 7320 616e 6420  ependencies and 
+000010b0: 2a2a 457a 5461 6f2a 2a20 696e 2065 6469  **EzTao** in edi
+000010c0: 7461 626c 6520 6d6f 6465 2e0a 2020 2060  table mode..   `
+000010d0: 6060 0a20 2020 706f 6574 7279 2069 6e73  ``.   poetry ins
+000010e0: 7461 6c6c 0a20 2020 6060 600a 0a4e 6f77  tall.   ```..Now
+000010f0: 2079 6f75 2073 686f 756c 6420 6265 2072   you should be r
+00001100: 6561 6479 2074 6f20 7374 6172 7420 6164  eady to start ad
+00001110: 6469 6e67 206e 6577 2066 6561 7475 7265  ding new feature
+00001120: 732e 2042 6520 7375 7265 2074 6f20 6368  s. Be sure to ch
+00001130: 6563 6b6f 7574 2074 6865 206e 6f72 6d61  eckout the norma
+00001140: 6c20 7072 6163 7469 6365 2072 6567 6172  l practice regar
+00001150: 6469 6e67 2068 6f77 2074 6f20 7573 6520  ding how to use 
+00001160: 6070 6f65 7472 7960 206f 6e20 6974 7320  `poetry` on its 
+00001170: 7765 6273 6974 652e 2057 6865 6e20 796f  website. When yo
+00001180: 7520 6172 6520 7265 6164 7920 746f 2070  u are ready to p
+00001190: 7573 682c 2061 6c73 6f20 6d61 6b65 2073  ush, also make s
+000011a0: 7572 6520 7468 6520 706f 6574 7279 2e6c  ure the poetry.l
+000011b0: 6f63 6b20 6669 6c65 2069 7320 6368 6563  ock file is chec
+000011c0: 6b65 642d 696e 2069 6620 616e 7920 6465  ked-in if any de
+000011d0: 7065 6e64 656e 6379 2068 6173 2063 6861  pendency has cha
+000011e0: 6e67 6564 2e20 0a0a 2323 2043 6974 6174  nged. ..## Citat
+000011f0: 696f 6e0a 5765 2061 7265 2077 6f72 6b69  ion.We are worki
+00001200: 6e67 206f 6e20 6120 7061 7065 7220 746f  ng on a paper to
+00001210: 2064 6573 6372 6962 6520 7468 6520 6675   describe the fu
+00001220: 6c6c 2069 6d70 6c65 6d65 6e74 6174 696f  ll implementatio
+00001230: 6e20 6f66 202a 2a45 7a54 616f 2a2a 2e20  n of **EzTao**. 
+00001240: 496e 2074 6865 206d 6561 6e74 696d 652c  In the meantime,
+00001250: 2069 6620 796f 7520 6669 6e64 202a 2a45   if you find **E
+00001260: 7a54 616f 2a2a 2075 7365 6675 6c20 666f  zTao** useful fo
+00001270: 7220 796f 7572 2072 6573 6561 7263 682c  r your research,
+00001280: 2070 6c65 6173 6520 636f 6e73 6964 6572   please consider
+00001290: 2061 636b 6e6f 776c 6564 6769 6e67 202a   acknowledging *
+000012a0: 2a45 7a54 616f 2a2a 2075 7369 6e67 2074  *EzTao** using t
+000012b0: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 0a60  he following:..`
+000012c0: 6060 0a40 4d49 5343 7b59 7532 3032 322c  ``.@MISC{Yu2022,
+000012d0: 0a20 2020 2020 2020 6175 7468 6f72 203d  .       author =
+000012e0: 207b 7b59 757d 2c20 5765 6978 6961 6e67   {{Yu}, Weixiang
+000012f0: 2061 6e64 207b 5269 6368 6172 6473 7d2c   and {Richards},
+00001300: 2047 6f72 646f 6e20 542e 7d2c 0a20 2020   Gordon T.},.   
+00001310: 2020 2020 2074 6974 6c65 203d 2022 7b45       title = "{E
+00001320: 7a54 616f 3a20 4561 7369 6572 2043 4152  zTao: Easier CAR
+00001330: 4d41 204d 6f64 656c 696e 677d 222c 0a20  MA Modeling}",. 
+00001340: 2020 2020 6b65 7977 6f72 6473 203d 207b      keywords = {
+00001350: 536f 6674 7761 7265 7d2c 0a20 686f 7770  Software},. howp
+00001360: 7562 6c69 7368 6564 203d 207b 4173 7472  ublished = {Astr
+00001370: 6f70 6879 7369 6373 2053 6f75 7263 6520  ophysics Source 
+00001380: 436f 6465 204c 6962 7261 7279 2c20 7265  Code Library, re
+00001390: 636f 7264 2061 7363 6c3a 3232 3031 2e30  cord ascl:2201.0
+000013a0: 3031 7d2c 0a20 2020 2020 2020 2020 7965  01},.         ye
+000013b0: 6172 203d 2032 3032 322c 0a20 2020 2020  ar = 2022,.     
+000013c0: 2020 206d 6f6e 7468 203d 206a 616e 2c0a     month = jan,.
+000013d0: 2020 2020 2020 2020 2020 6569 6420 3d20            eid = 
+000013e0: 7b61 7363 6c3a 3232 3031 2e30 3031 7d2c  {ascl:2201.001},
+000013f0: 0a20 2020 2020 2020 2070 6167 6573 203d  .        pages =
+00001400: 207b 6173 636c 3a32 3230 312e 3030 317d   {ascl:2201.001}
+00001410: 2c0a 6172 6368 6976 6550 7265 6669 7820  ,.archivePrefix 
+00001420: 3d20 7b61 7363 6c7d 2c0a 2020 2020 2020  = {ascl},.      
+00001430: 2065 7072 696e 7420 3d20 7b32 3230 312e   eprint = {2201.
+00001440: 3030 317d 2c0a 2020 2020 2020 2061 6473  001},.       ads
+00001450: 7572 6c20 3d20 7b68 7474 7073 3a2f 2f75  url = {https://u
+00001460: 692e 6164 7361 6273 2e68 6172 7661 7264  i.adsabs.harvard
+00001470: 2e65 6475 2f61 6273 2f32 3032 3261 7363  .edu/abs/2022asc
+00001480: 6c2e 736f 6674 3031 3030 3159 7d2c 0a20  l.soft01001Y},. 
+00001490: 2020 2020 2061 6473 6e6f 7465 203d 207b       adsnote = {
+000014a0: 5072 6f76 6964 6564 2062 7920 7468 6520  Provided by the 
+000014b0: 5341 4f2f 4e41 5341 2041 7374 726f 7068  SAO/NASA Astroph
+000014c0: 7973 6963 7320 4461 7461 2053 7973 7465  ysics Data Syste
+000014d0: 6d7d 0a7d 0a60 6060 0a0a 0a              m}.}.```...
```

