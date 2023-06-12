# Comparing `tmp/aioarp-0.0.4.tar.gz` & `tmp/aioarp-0.0.5.tar.gz`

## Comparing `aioarp-0.0.4.tar` & `aioarp-0.0.5.tar`

### file list

```diff
@@ -1,215 +1,37 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aioarp-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aioarp-0.0.4/requirements.txt
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.4/unasync.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aioarp-0.0.4/.github/workflows/main.yml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 aioarp-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/120fd5a3e305da5b
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/12101680e8031881
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/16b1a595f0c0b695
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/17946c0e3734f56
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/18bd9323e775c06
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1911b721541a132
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1a43e2fa66cc521
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1bfc7af844c09624
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1c4766f25c290393
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1cf748db3edf4393
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1d813f87eae436dc
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/20360c87813708ee
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/20b471ae4ae2c716
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/20cf28b4a08829e
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/20e8c6fb6ec65fba
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/22273ee756d2aeab
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/22eb75e2705cd7cb
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/23b5bf7a560a3d85
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/258218bd1af61054
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/259f2d45c9b5e8f8
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/259f7be1f71aae17
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/27380b38303cddd4
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/277c58fd0e92dc6f
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/2894d2afe73e6dee
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/28bfffee8af0f637
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/29459fb899e6be63
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/29a3dfb41b2e153e
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/29ec5304bead68a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/2b17b1ab21ba1879
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/2b74d3f1efd79c7b
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/2f2908e30cbaaf6f
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/3546886ec7b89ca2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/3a9f29e79b12106b
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/3c82c38fdeb726f5
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/3cf42c96bb03e8e
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/40ec6c4657092d14
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/42d47131a22f033d
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/44618acc04af2a98
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/464ea8dcb036f50b
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/48dc01dafed313cb
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4bfeb322489be7b2
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4c18fbd43c6124d9
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4c7aefddb4afaa07
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4ce11f41c925600e
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4d80d8cbd7abb331
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4dcc3bf9688e8634
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4e4abc9127fe2106
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/522c23633820a258
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/5259c25c40a66c52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/53480da31b2357be
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/536385ed3a8bbf59
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/53922c565bc4cfdf
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/54ca2556c07eb0e4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/57ee6e97f4833ae1
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/5845e4d7f49b3f6b
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/590fd00a0401d086
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/5e5e4a02dc426617
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/608e0f7e2331dfd0
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6190d891377c8571
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6269535ee79a68b3
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6390cd3a2155b002
--rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/64f9f289e0610564
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6572fa7cae8df134
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/65bac7c6a4c4cb5e
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/65d6dc214750c212
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6857c9063a540073
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/68e278cd0a30d24c
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6aa5b22c44c81236
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6aee26157f3848b9
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6b926a7206e2e0f5
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6ba798af16bd34e5
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6dbcf7ab6c32f876
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6de1f164718890ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6ec79cb0a99a4ffa
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/70ee6f5e2e8b7d90
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/75d5cb975af2bc07
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/7753615b71d6a36e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/78dc31b63dbd1e69
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/79da2ffd4120460
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/7d0a3cccefcd7db3
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/7f23f9f7d375f4fd
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/80b8f04bc59d958c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/82b9ee56f8fed787
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8362e113a849836
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/837a3e06585749a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/841d7ee35702e48e
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/85532fbdb4ec8100
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/859b9d135acd891b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/85a7bda1ebac02be
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/869f865c9f14daf7
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/879246cf978566b8
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/89ad75a37b7215d3
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8af090de0021767
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8ba2e035b666505
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8caa6ea7d00a8ef9
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8e5085aaf38947dd
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8e9682f1b99c3026
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/93389fd7b221ce32
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/936f955f01285847
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/94a86b805b8c04e2
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/9600ec5b79137dcc
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/967dc6947ad8c113
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/990e2b74e6a14435
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/9db40d9bd33cc32a
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a0edd6b97fbe3e68
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a12cec0addd27620
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a22627f4ad982518
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a41b182cef331aa5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a42de4efa897ae1e
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a5253384caf62eef
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a62236fd623ff7ad
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a64cd85354e281c5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a7b52a5c13a67fed
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/aabe170d14233a1f
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/aac73f953da24b03
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/ac1d91a6ebb4bed9
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/ace8365de45531
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/aced40484cbf3132
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/adb7c2d2342ef983
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b1ec491bf059cec3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b27cd0e5108544e0
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b3202a665cec273b
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b74ab4e72907ed4b
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b752bc22791212b3
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b874aac73807837a
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bb3a8375be948e99
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bb98194f279aef4d
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bc9d2b60dadbf05e
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bd0ea26a717d1380
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bd3e6a97ee360bd7
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bdd7c44b4f88bf5b
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bffaaf1ee55da212
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c0cc1810bd812c85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c0d92e761aa72a56
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c12c935be2da0714
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c24cf3b955d01f58
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c2e7f8eb8bfe8525
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c370f17718b5228b
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c3b1cc9370bb49b5
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c54b124e74d7c29a
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c64725c588d56756
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c6c7c5bdc9a58d71
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c78c3248c370d9f2
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c7a507ee84d3e2ab
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c908c9d3ee0eb43c
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cc374f0497dbc539
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cc5595ab776e807c
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cd40078ccedf2012
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cd84fa1ee95c780c
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cdc31ad9b3ea9979
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/d08cf74ff5eeb16e
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/d3d46de068ceaf65
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/d4ed3103ad57bd80
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/d8259ee38b03fc0e
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/dc53fc214ceea0dd
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/de93c4dfa993ec19
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e11920c476dc4f59
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e12d636458d129da
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e25cfbd84c59869
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e2a8017124da7733
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e305b1c5b826225
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e512a2b647437caa
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e84bd53ae32ad4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e8f0ea35cc3b448a
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e9d1ab2b1a8c3cca
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/eb250aff0edc4ecb
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/eee42766c50b6490
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f0ff9ca6cba080b9
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f2ebd390a47aa1cd
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f3ac79af6cdde497
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f3d289f55f0ad6bd
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f45e36470415dca1
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f56e6b11a3d4a68b
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f58c3d661899d706
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f96d453d0b6b9c85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/fb10e8087c484390
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/fd508bd27e156044
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/ffe7d79671eca8f
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/__about__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/__init__.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_arp.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_async.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_client.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_exceptions.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_mock.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_sync.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/defaults.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/__init__.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/_async.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/_base.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/_mock.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/_sync.py
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.4/scripts/check
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.4/scripts/lint
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.4/scripts/test
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_async.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_client.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_proto.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_sync.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_utils.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aioarp-0.0.4/README.md
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 aioarp-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 aioarp-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 aioarp-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aioarp-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.5/unasync.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aioarp-0.0.5/.github/workflows/main.yml
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 aioarp-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/__about__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/__init__.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_arp.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_async.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_cli.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_client.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_exceptions.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_mock.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_sync.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_utils.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/defaults.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/__init__.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/_async.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/_base.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/_mock.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/_sync.py
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.5/scripts/check
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.5/scripts/lint
+-rwxr-xr-x   0        0        0       60 2020-02-02 00:00:00.000000 aioarp-0.0.5/scripts/publish
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.5/scripts/test
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_async.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_client.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_proto.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_sync.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_utils.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aioarp-0.0.5/README.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 aioarp-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 aioarp-0.0.5/PKG-INFO
```

### Comparing `aioarp-0.0.4/unasync.py` & `aioarp-0.0.5/unasync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/.github/workflows/main.yml` & `aioarp-0.0.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/.ruff_cache/content/120fd5a3e305da5b` & `aioarp-0.0.5/aioarp/_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,209 +1,136 @@
-00000000: 0100 0000 0000 0000 0e00 0000 0000 0000  ................
-00000010: 6169 6f61 7270 2e5f 636c 6965 6e74 0d00  aioarp._client..
-00000020: 0000 0000 0000 0900 0000 0000 0000 6970  ..............ip
-00000030: 6164 6472 6573 7300 0000 0010 0000 0006  address.........
-00000040: 0000 0000 0000 0073 6f63 6b65 7411 0000  .......socket...
-00000050: 001e 0000 0006 0000 0000 0000 0074 7970  .............typ
-00000060: 696e 671f 0000 002c 0000 0015 0000 0000  ing....,........
-00000070: 0000 0061 696f 6172 702e 5f61 7270 2e41  ...aioarp._arp.A
-00000080: 7270 5061 636b 6574 4600 0000 4f00 0000  rpPacketF...O...
-00000090: 1800 0000 0000 0000 6169 6f61 7270 2e5f  ........aioarp._
-000000a0: 6172 702e 4861 7264 7761 7265 5479 7065  arp.HardwareType
-000000b0: 5100 0000 5d00 0000 1400 0000 0000 0000  Q...]...........
-000000c0: 6169 6f61 7270 2e5f 6172 702e 5072 6f74  aioarp._arp.Prot
-000000d0: 6f63 6f6c 5f00 0000 6700 0000 1c00 0000  ocol_...g.......
-000000e0: 0000 0000 6169 6f61 7270 2e5f 6173 796e  ....aioarp._asyn
-000000f0: 632e 6173 796e 635f 7365 6e64 5f61 7270  c.async_send_arp
-00000100: 8200 0000 9000 0000 1a00 0000 0000 0000  ................
-00000110: 6169 6f61 7270 2e5f 7379 6e63 2e73 796e  aioarp._sync.syn
-00000120: 635f 7365 6e64 5f61 7270 aa00 0000 b700  c_send_arp......
-00000130: 0000 1400 0000 0000 0000 6169 6f61 7270  ..........aioarp
-00000140: 2e5f 7574 696c 732e 6765 745f 6970 d200  ._utils.get_ip..
-00000150: 0000 d800 0000 1500 0000 0000 0000 6169  ..............ai
-00000160: 6f61 7270 2e5f 7574 696c 732e 6765 745f  oarp._utils.get_
-00000170: 6d61 63da 0000 00e1 0000 0025 0000 0000  mac........%....
-00000180: 0000 0061 696f 6172 702e 6261 636b 656e  ...aioarp.backen
-00000190: 6473 2e5f 6261 7365 2e53 6f63 6b65 7449  ds._base.SocketI
-000001a0: 6e74 6572 6661 6365 0401 0000 1301 0000  nterface........
-000001b0: 2200 0000 0000 0000 6169 6f61 7270 2e62  ".......aioarp.b
-000001c0: 6163 6b65 6e64 732e 5f61 7379 6e63 2e41  ackends._async.A
-000001d0: 7379 6e63 5374 7265 616d 3701 0000 4201  syncStream7...B.
-000001e0: 0000 1c00 0000 0000 0000 6169 6f61 7270  ..........aioarp
-000001f0: 2e62 6163 6b65 6e64 732e 5f73 796e 632e  .backends._sync.
-00000200: 5374 7265 616d 6501 0000 6b01 0000 0300  Streame...k.....
-00000210: 0000 0000 0000 0c00 0000 0000 0000 556e  ..............Un
-00000220: 7573 6564 496d 706f 7274 1c00 0000 0000  usedImport......
-00000230: 0000 6073 6f63 6b65 7460 2069 6d70 6f72  ..`socket` impor
-00000240: 7465 6420 6275 7420 756e 7573 6564 011e  ted but unused..
-00000250: 0000 0000 0000 0052 656d 6f76 6520 756e  .......Remove un
-00000260: 7573 6564 2069 6d70 6f72 743a 2060 736f  used import: `so
-00000270: 636b 6574 6018 0000 001e 0000 0001 0100  cket`...........
-00000280: 0000 0000 0000 1100 0000 1f00 0000 0003  ................
-00000290: 0000 0000 0000 0000 0000 0018 0000 000c  ................
-000002a0: 0000 0000 0000 0055 6e75 7365 6449 6d70  .......UnusedImp
-000002b0: 6f72 7438 0000 0000 0000 0060 6169 6f61  ort8.......`aioa
-000002c0: 7270 2e62 6163 6b65 6e64 732e 5f61 7379  rp.backends._asy
-000002d0: 6e63 2e41 7379 6e63 5374 7265 616d 6020  nc.AsyncStream` 
-000002e0: 696d 706f 7274 6564 2062 7574 2075 6e75  imported but unu
-000002f0: 7365 6401 3a00 0000 0000 0000 5265 6d6f  sed.:.......Remo
-00000300: 7665 2075 6e75 7365 6420 696d 706f 7274  ve unused import
-00000310: 3a20 6061 696f 6172 702e 6261 636b 656e  : `aioarp.backen
-00000320: 6473 2e5f 6173 796e 632e 4173 796e 6353  ds._async.AsyncS
-00000330: 7472 6561 6d60 3701 0000 4201 0000 0101  tream`7...B.....
-00000340: 0000 0000 0000 0014 0100 0043 0100 0000  ...........C....
-00000350: 0300 0000 0000 0000 0000 0000 3701 0000  ............7...
-00000360: 0f00 0000 0000 0000 556e 736f 7274 6564  ........Unsorted
-00000370: 496d 706f 7274 7329 0000 0000 0000 0049  Imports).......I
-00000380: 6d70 6f72 7420 626c 6f63 6b20 6973 2075  mport block is u
-00000390: 6e2d 736f 7274 6564 206f 7220 756e 2d66  n-sorted or un-f
-000003a0: 6f72 6d61 7474 6564 0110 0000 0000 0000  ormatted........
-000003b0: 004f 7267 616e 697a 6520 696d 706f 7274  .Organize import
-000003c0: 7300 0000 006d 0100 0001 0100 0000 0000  s....m..........
-000003d0: 0000 0000 0000 6d01 0000 016d 0100 0000  ......m....m....
-000003e0: 0000 0069 6d70 6f72 7420 6970 6164 6472  ...import ipaddr
-000003f0: 6573 730a 696d 706f 7274 2073 6f63 6b65  ess.import socke
-00000400: 740a 696d 706f 7274 2074 7970 696e 670a  t.import typing.
-00000410: 0a66 726f 6d20 6169 6f61 7270 2e5f 6172  .from aioarp._ar
-00000420: 7020 696d 706f 7274 2041 7270 5061 636b  p import ArpPack
-00000430: 6574 2c20 4861 7264 7761 7265 5479 7065  et, HardwareType
-00000440: 2c20 5072 6f74 6f63 6f6c 0a66 726f 6d20  , Protocol.from 
-00000450: 6169 6f61 7270 2e5f 6173 796e 6320 696d  aioarp._async im
-00000460: 706f 7274 2061 7379 6e63 5f73 656e 645f  port async_send_
-00000470: 6172 700a 6672 6f6d 2061 696f 6172 702e  arp.from aioarp.
-00000480: 5f73 796e 6320 696d 706f 7274 2073 796e  _sync import syn
-00000490: 635f 7365 6e64 5f61 7270 0a66 726f 6d20  c_send_arp.from 
-000004a0: 6169 6f61 7270 2e5f 7574 696c 7320 696d  aioarp._utils im
-000004b0: 706f 7274 2067 6574 5f69 702c 2067 6574  port get_ip, get
-000004c0: 5f6d 6163 0a66 726f 6d20 6169 6f61 7270  _mac.from aioarp
-000004d0: 2e62 6163 6b65 6e64 732e 5f61 7379 6e63  .backends._async
-000004e0: 2069 6d70 6f72 7420 4173 796e 6353 7472   import AsyncStr
-000004f0: 6561 6d0a 6672 6f6d 2061 696f 6172 702e  eam.from aioarp.
-00000500: 6261 636b 656e 6473 2e5f 6261 7365 2069  backends._base i
-00000510: 6d70 6f72 7420 536f 636b 6574 496e 7465  mport SocketInte
-00000520: 7266 6163 650a 6672 6f6d 2061 696f 6172  rface.from aioar
-00000530: 702e 6261 636b 656e 6473 2e5f 7379 6e63  p.backends._sync
-00000540: 2069 6d70 6f72 7420 5374 7265 616d 0a0a   import Stream..
-00000550: 0300 0000 0000 0000 0000 0000 0000 0000  ................
-00000560: 0100 0000 0000 0000 2b00 0000 0000 0000  ........+.......
-00000570: 2f68 6f6d 652f 7465 7374 2f44 6573 6b74  /home/test/Deskt
-00000580: 6f70 2f61 696f 6172 702f 6169 6f61 7270  op/aioarp/aioarp
-00000590: 2f5f 636c 6965 6e74 2e70 796a 0700 0000  /_client.pyj....
-000005a0: 0000 0069 6d70 6f72 7420 6970 6164 6472  ...import ipaddr
-000005b0: 6573 730a 696d 706f 7274 2073 6f63 6b65  ess.import socke
-000005c0: 740a 696d 706f 7274 2074 7970 696e 670a  t.import typing.
-000005d0: 0a66 726f 6d20 6169 6f61 7270 2e5f 6172  .from aioarp._ar
-000005e0: 7020 696d 706f 7274 2041 7270 5061 636b  p import ArpPack
-000005f0: 6574 2c20 4861 7264 7761 7265 5479 7065  et, HardwareType
-00000600: 2c20 5072 6f74 6f63 6f6c 0a66 726f 6d20  , Protocol.from 
-00000610: 6169 6f61 7270 2e5f 6173 796e 6320 696d  aioarp._async im
-00000620: 706f 7274 2061 7379 6e63 5f73 656e 645f  port async_send_
-00000630: 6172 700a 6672 6f6d 2061 696f 6172 702e  arp.from aioarp.
-00000640: 5f73 796e 6320 696d 706f 7274 2073 796e  _sync import syn
-00000650: 635f 7365 6e64 5f61 7270 0a66 726f 6d20  c_send_arp.from 
-00000660: 6169 6f61 7270 2e5f 7574 696c 7320 696d  aioarp._utils im
-00000670: 706f 7274 2067 6574 5f69 702c 2067 6574  port get_ip, get
-00000680: 5f6d 6163 0a66 726f 6d20 6169 6f61 7270  _mac.from aioarp
-00000690: 2e62 6163 6b65 6e64 732e 5f62 6173 6520  .backends._base 
-000006a0: 696d 706f 7274 2053 6f63 6b65 7449 6e74  import SocketInt
-000006b0: 6572 6661 6365 0a66 726f 6d20 6169 6f61  erface.from aioa
-000006c0: 7270 2e62 6163 6b65 6e64 732e 5f61 7379  rp.backends._asy
-000006d0: 6e63 2069 6d70 6f72 7420 4173 796e 6353  nc import AsyncS
-000006e0: 7472 6561 6d0a 6672 6f6d 2061 696f 6172  tream.from aioar
-000006f0: 702e 6261 636b 656e 6473 2e5f 7379 6e63  p.backends._sync
-00000700: 2069 6d70 6f72 7420 5374 7265 616d 0a0a   import Stream..
-00000710: 5f5f 616c 6c5f 5f20 3d20 280a 2020 2020  __all__ = (.    
-00000720: 2762 7569 6c64 5f61 7270 5f70 6163 6b65  'build_arp_packe
-00000730: 7427 2c0a 2020 2020 2772 6571 7565 7374  t',.    'request
-00000740: 272c 0a20 2020 2027 6172 6571 7565 7374  ',.    'arequest
-00000750: 270a 290a 0a0a 6465 6620 6275 696c 645f  '.)...def build_
-00000760: 6172 705f 7061 636b 6574 280a 2020 2020  arp_packet(.    
-00000770: 2020 2020 696e 7465 7266 6163 653a 2073      interface: s
-00000780: 7472 2c0a 2020 2020 2020 2020 7461 7267  tr,.        targ
-00000790: 6574 5f69 703a 2073 7472 0a29 202d 3e20  et_ip: str.) -> 
-000007a0: 4172 7050 6163 6b65 743a 0a20 2020 2074  ArpPacket:.    t
-000007b0: 7279 3a0a 2020 2020 2020 2020 6970 6164  ry:.        ipad
-000007c0: 6472 6573 732e 4950 7634 4164 6472 6573  dress.IPv4Addres
-000007d0: 7328 7461 7267 6574 5f69 7029 0a20 2020  s(target_ip).   
-000007e0: 2065 7863 6570 7420 6970 6164 6472 6573   except ipaddres
-000007f0: 732e 4164 6472 6573 7356 616c 7565 4572  s.AddressValueEr
-00000800: 726f 723a 0a20 2020 2020 2020 2072 6169  ror:.        rai
-00000810: 7365 2045 7863 6570 7469 6f6e 2822 496e  se Exception("In
-00000820: 7661 6c69 6420 4950 7634 2041 6464 7265  valid IPv4 Addre
-00000830: 7373 2077 6173 2072 6563 6569 7665 6422  ss was received"
-00000840: 290a 0a20 2020 2068 6172 6477 6172 655f  )..    hardware_
-00000850: 7479 7065 203d 2048 6172 6477 6172 6554  type = HardwareT
-00000860: 7970 652e 6574 6865 726e 6574 0a20 2020  ype.ethernet.   
-00000870: 2070 726f 746f 636f 6c5f 7479 7065 203d   protocol_type =
-00000880: 2050 726f 746f 636f 6c2e 6970 0a0a 2020   Protocol.ip..  
-00000890: 2020 2320 544f 444f 3a20 6361 7463 6820    # TODO: catch 
-000008a0: 696e 7465 7266 6163 6520 6e6f 7420 666f  interface not fo
-000008b0: 756e 6420 6572 726f 720a 2020 2020 7365  und error.    se
-000008c0: 6e64 6572 5f6d 6163 203d 2067 6574 5f6d  nder_mac = get_m
-000008d0: 6163 2869 6e74 6572 6661 6365 290a 2020  ac(interface).  
-000008e0: 2020 7365 6e64 6572 5f69 7020 3d20 6765    sender_ip = ge
-000008f0: 745f 6970 2829 0a20 2020 2074 6172 6765  t_ip().    targe
-00000900: 745f 6d61 6320 3d20 2766 663a 6666 3a66  t_mac = 'ff:ff:f
-00000910: 663a 6666 3a66 663a 6666 270a 0a20 2020  f:ff:ff:ff'..   
-00000920: 2072 6571 7565 7374 5f70 6163 6b65 7420   request_packet 
-00000930: 3d20 4172 7050 6163 6b65 7428 0a20 2020  = ArpPacket(.   
-00000940: 2020 2020 2068 6172 6477 6172 655f 7479       hardware_ty
-00000950: 7065 2c0a 2020 2020 2020 2020 7072 6f74  pe,.        prot
-00000960: 6f63 6f6c 5f74 7970 652c 0a20 2020 2020  ocol_type,.     
-00000970: 2020 2073 656e 6465 725f 6d61 632c 0a20     sender_mac,. 
-00000980: 2020 2020 2020 2073 656e 6465 725f 6970         sender_ip
-00000990: 2c0a 2020 2020 2020 2020 7461 7267 6574  ,.        target
-000009a0: 5f6d 6163 2c0a 2020 2020 2020 2020 7461  _mac,.        ta
-000009b0: 7267 6574 5f69 702c 0a20 2020 2029 0a20  rget_ip,.    ). 
-000009c0: 2020 2072 6574 7572 6e20 7265 7175 6573     return reques
-000009d0: 745f 7061 636b 6574 0a0a 0a64 6566 2072  t_packet...def r
-000009e0: 6571 7565 7374 280a 2020 2020 2020 2020  equest(.        
-000009f0: 696e 7465 7266 6163 653a 2073 7472 2c0a  interface: str,.
-00000a00: 2020 2020 2020 2020 7461 7267 6574 5f69          target_i
-00000a10: 703a 2073 7472 2c0a 2020 2020 2020 2020  p: str,.        
-00000a20: 7469 6d65 6f75 743a 2074 7970 696e 672e  timeout: typing.
-00000a30: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
-00000a40: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00000a50: 736f 636b 3a20 7479 7069 6e67 2e4f 7074  sock: typing.Opt
-00000a60: 696f 6e61 6c5b 536f 636b 6574 496e 7465  ional[SocketInte
-00000a70: 7266 6163 655d 203d 204e 6f6e 650a 2920  rface] = None.) 
-00000a80: 2d3e 2041 7270 5061 636b 6574 3a0a 2020  -> ArpPacket:.  
-00000a90: 2020 7374 7265 616d 203d 2053 7472 6561    stream = Strea
-00000aa0: 6d28 696e 7465 7266 6163 653d 696e 7465  m(interface=inte
-00000ab0: 7266 6163 652c 0a20 2020 2020 2020 2020  rface,.         
-00000ac0: 2020 2020 2020 2020 2020 2073 6f63 6b3d             sock=
-00000ad0: 736f 636b 290a 2020 2020 7265 7175 6573  sock).    reques
-00000ae0: 745f 7061 636b 6574 203d 2062 7569 6c64  t_packet = build
-00000af0: 5f61 7270 5f70 6163 6b65 7428 696e 7465  _arp_packet(inte
-00000b00: 7266 6163 652c 2074 6172 6765 745f 6970  rface, target_ip
-00000b10: 290a 2020 2020 6172 705f 7265 7370 6f6e  ).    arp_respon
-00000b20: 7365 203d 2073 796e 635f 7365 6e64 5f61  se = sync_send_a
-00000b30: 7270 2872 6571 7565 7374 5f70 6163 6b65  rp(request_packe
-00000b40: 742c 2073 7472 6561 6d2c 2074 696d 656f  t, stream, timeo
-00000b50: 7574 290a 2020 2020 7265 7475 726e 2061  ut).    return a
-00000b60: 7270 5f72 6573 706f 6e73 650a 0a0a 6173  rp_response...as
-00000b70: 796e 6320 6465 6620 6172 6571 7565 7374  ync def arequest
-00000b80: 280a 2020 2020 2020 2020 696e 7465 7266  (.        interf
-00000b90: 6163 653a 2073 7472 2c0a 2020 2020 2020  ace: str,.      
-00000ba0: 2020 7461 7267 6574 5f69 703a 2073 7472    target_ip: str
-00000bb0: 2c0a 2020 2020 2020 2020 7469 6d65 6f75  ,.        timeou
-00000bc0: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
-00000bd0: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
-00000be0: 2c0a 2020 2020 2020 2020 736f 636b 3a20  ,.        sock: 
-00000bf0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00000c00: 536f 636b 6574 496e 7465 7266 6163 655d  SocketInterface]
-00000c10: 203d 204e 6f6e 650a 2920 2d3e 2041 7270   = None.) -> Arp
-00000c20: 5061 636b 6574 3a0a 2020 2020 7374 7265  Packet:.    stre
-00000c30: 616d 203d 2053 7472 6561 6d28 696e 7465  am = Stream(inte
-00000c40: 7266 6163 653d 696e 7465 7266 6163 652c  rface=interface,
-00000c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c60: 2020 2020 2073 6f63 6b3d 736f 636b 290a       sock=sock).
-00000c70: 2020 2020 7265 7175 6573 745f 7061 636b      request_pack
-00000c80: 6574 203d 2062 7569 6c64 5f61 7270 5f70  et = build_arp_p
-00000c90: 6163 6b65 7428 696e 7465 7266 6163 652c  acket(interface,
-00000ca0: 2074 6172 6765 745f 6970 290a 2020 2020   target_ip).    
-00000cb0: 6172 705f 7265 7370 6f6e 7365 203d 2061  arp_response = a
-00000cc0: 7761 6974 2061 7379 6e63 5f73 656e 645f  wait async_send_
-00000cd0: 6172 7028 7265 7175 6573 745f 7061 636b  arp(request_pack
-00000ce0: 6574 2c20 7374 7265 616d 2c20 7469 6d65  et, stream, time
-00000cf0: 6f75 7429 0a20 2020 2072 6574 7572 6e20  out).    return 
-00000d00: 6172 705f 7265 7370 6f6e 7365 0a         arp_response.
+00000000: 696d 706f 7274 2073 6f63 6b65 740a 696d  import socket.im
+00000010: 706f 7274 2074 7970 696e 670a 0a69 6d70  port typing..imp
+00000020: 6f72 7420 6169 6f61 7270 0a66 726f 6d20  ort aioarp.from 
+00000030: 6169 6f61 7270 2e5f 6172 7020 696d 706f  aioarp._arp impo
+00000040: 7274 2041 7270 5061 636b 6574 2c20 4861  rt ArpPacket, Ha
+00000050: 7264 7761 7265 5479 7065 2c20 5072 6f74  rdwareType, Prot
+00000060: 6f63 6f6c 0a66 726f 6d20 6169 6f61 7270  ocol.from aioarp
+00000070: 2e5f 6173 796e 6320 696d 706f 7274 2061  ._async import a
+00000080: 7379 6e63 5f73 656e 645f 6172 700a 6672  sync_send_arp.fr
+00000090: 6f6d 2061 696f 6172 702e 5f62 6163 6b65  om aioarp._backe
+000000a0: 6e64 732e 5f61 7379 6e63 2069 6d70 6f72  nds._async impor
+000000b0: 7420 4173 796e 6353 7472 6561 6d0a 6672  t AsyncStream.fr
+000000c0: 6f6d 2061 696f 6172 702e 5f62 6163 6b65  om aioarp._backe
+000000d0: 6e64 732e 5f62 6173 6520 696d 706f 7274  nds._base import
+000000e0: 2053 6f63 6b65 7449 6e74 6572 6661 6365   SocketInterface
+000000f0: 0a66 726f 6d20 6169 6f61 7270 2e5f 6261  .from aioarp._ba
+00000100: 636b 656e 6473 2e5f 7379 6e63 2069 6d70  ckends._sync imp
+00000110: 6f72 7420 5374 7265 616d 0a66 726f 6d20  ort Stream.from 
+00000120: 6169 6f61 7270 2e5f 7379 6e63 2069 6d70  aioarp._sync imp
+00000130: 6f72 7420 7379 6e63 5f73 656e 645f 6172  ort sync_send_ar
+00000140: 700a 6672 6f6d 2061 696f 6172 702e 5f75  p.from aioarp._u
+00000150: 7469 6c73 2069 6d70 6f72 7420 6765 745f  tils import get_
+00000160: 6970 2c20 6765 745f 6d61 632c 2069 735f  ip, get_mac, is_
+00000170: 7661 6c69 645f 6970 7634 0a0a 5f5f 616c  valid_ipv4..__al
+00000180: 6c5f 5f20 3d20 280a 2020 2020 2762 7569  l__ = (.    'bui
+00000190: 6c64 5f61 7270 5f70 6163 6b65 7427 2c0a  ld_arp_packet',.
+000001a0: 2020 2020 2772 6571 7565 7374 272c 0a20      'request',. 
+000001b0: 2020 2027 6172 6571 7565 7374 270a 290a     'arequest'.).
+000001c0: 0a0a 6465 6620 6275 696c 645f 6172 705f  ..def build_arp_
+000001d0: 7061 636b 6574 280a 2020 2020 2020 2020  packet(.        
+000001e0: 696e 7465 7266 6163 653a 2073 7472 2c0a  interface: str,.
+000001f0: 2020 2020 2020 2020 7461 7267 6574 5f69          target_i
+00000200: 703a 2073 7472 0a29 202d 3e20 4172 7050  p: str.) -> ArpP
+00000210: 6163 6b65 743a 0a20 2020 2069 6620 6e6f  acket:.    if no
+00000220: 7420 6973 5f76 616c 6964 5f69 7076 3428  t is_valid_ipv4(
+00000230: 7461 7267 6574 5f69 7029 3a0a 2020 2020  target_ip):.    
+00000240: 2020 2020 7261 6973 6520 6169 6f61 7270      raise aioarp
+00000250: 2e49 6e76 616c 6964 4970 4572 726f 7228  .InvalidIpError(
+00000260: 2249 6e76 616c 6964 2049 5076 3420 4164  "Invalid IPv4 Ad
+00000270: 6472 6573 7320 7761 7320 7265 6365 6976  dress was receiv
+00000280: 6564 2229 0a0a 2020 2020 6861 7264 7761  ed")..    hardwa
+00000290: 7265 5f74 7970 6520 3d20 4861 7264 7761  re_type = Hardwa
+000002a0: 7265 5479 7065 2e65 7468 6572 6e65 740a  reType.ethernet.
+000002b0: 2020 2020 7072 6f74 6f63 6f6c 5f74 7970      protocol_typ
+000002c0: 6520 3d20 5072 6f74 6f63 6f6c 2e69 700a  e = Protocol.ip.
+000002d0: 0a20 2020 2023 2054 4f44 4f3a 2063 6174  .    # TODO: cat
+000002e0: 6368 2069 6e74 6572 6661 6365 206e 6f74  ch interface not
+000002f0: 2066 6f75 6e64 2065 7272 6f72 0a20 2020   found error.   
+00000300: 2073 656e 6465 725f 6d61 6320 3d20 6765   sender_mac = ge
+00000310: 745f 6d61 6328 696e 7465 7266 6163 6529  t_mac(interface)
+00000320: 0a20 2020 2073 656e 6465 725f 6970 203d  .    sender_ip =
+00000330: 2067 6574 5f69 7028 290a 2020 2020 7461   get_ip().    ta
+00000340: 7267 6574 5f6d 6163 203d 2027 6666 3a66  rget_mac = 'ff:f
+00000350: 663a 6666 3a66 663a 6666 3a66 6627 0a0a  f:ff:ff:ff:ff'..
+00000360: 2020 2020 7265 7175 6573 745f 7061 636b      request_pack
+00000370: 6574 203d 2041 7270 5061 636b 6574 280a  et = ArpPacket(.
+00000380: 2020 2020 2020 2020 6861 7264 7761 7265          hardware
+00000390: 5f74 7970 652c 0a20 2020 2020 2020 2070  _type,.        p
+000003a0: 726f 746f 636f 6c5f 7479 7065 2c0a 2020  rotocol_type,.  
+000003b0: 2020 2020 2020 7365 6e64 6572 5f6d 6163        sender_mac
+000003c0: 2c0a 2020 2020 2020 2020 7365 6e64 6572  ,.        sender
+000003d0: 5f69 702c 0a20 2020 2020 2020 2074 6172  _ip,.        tar
+000003e0: 6765 745f 6d61 632c 0a20 2020 2020 2020  get_mac,.       
+000003f0: 2074 6172 6765 745f 6970 2c0a 2020 2020   target_ip,.    
+00000400: 290a 2020 2020 7265 7475 726e 2072 6571  ).    return req
+00000410: 7565 7374 5f70 6163 6b65 740a 0a0a 6465  uest_packet...de
+00000420: 6620 7265 7175 6573 7428 0a20 2020 2020  f request(.     
+00000430: 2020 2069 6e74 6572 6661 6365 3a20 7374     interface: st
+00000440: 722c 0a20 2020 2020 2020 2074 6172 6765  r,.        targe
+00000450: 745f 6970 3a20 7374 722c 0a20 2020 2020  t_ip: str,.     
+00000460: 2020 2074 696d 656f 7574 3a20 7479 7069     timeout: typi
+00000470: 6e67 2e4f 7074 696f 6e61 6c5b 666c 6f61  ng.Optional[floa
+00000480: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+00000490: 2020 2073 6f63 6b3a 2074 7970 696e 672e     sock: typing.
+000004a0: 4f70 7469 6f6e 616c 5b53 6f63 6b65 7449  Optional[SocketI
+000004b0: 6e74 6572 6661 6365 5d20 3d20 4e6f 6e65  nterface] = None
+000004c0: 0a29 202d 3e20 4172 7050 6163 6b65 743a  .) -> ArpPacket:
+000004d0: 0a20 2020 2069 6620 6e6f 7420 736f 636b  .    if not sock
+000004e0: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+000004f0: 636f 7665 720a 2020 2020 2020 2020 736f  cover.        so
+00000500: 636b 203d 2073 6f63 6b65 742e 736f 636b  ck = socket.sock
+00000510: 6574 2873 6f63 6b65 742e 5046 5f50 4143  et(socket.PF_PAC
+00000520: 4b45 542c 2073 6f63 6b65 742e 534f 434b  KET, socket.SOCK
+00000530: 5f52 4157 2c20 736f 636b 6574 2e6e 746f  _RAW, socket.nto
+00000540: 6873 2830 7830 3030 3329 290a 2020 2020  hs(0x0003)).    
+00000550: 7769 7468 2053 7472 6561 6d28 696e 7465  with Stream(inte
+00000560: 7266 6163 653d 696e 7465 7266 6163 652c  rface=interface,
+00000570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000580: 2020 2020 2073 6f63 6b3d 736f 636b 2920       sock=sock) 
+00000590: 6173 2073 7472 6561 6d3a 0a20 2020 2020  as stream:.     
+000005a0: 2020 2072 6571 7565 7374 5f70 6163 6b65     request_packe
+000005b0: 7420 3d20 6275 696c 645f 6172 705f 7061  t = build_arp_pa
+000005c0: 636b 6574 2869 6e74 6572 6661 6365 2c20  cket(interface, 
+000005d0: 7461 7267 6574 5f69 7029 0a20 2020 2020  target_ip).     
+000005e0: 2020 2061 7270 5f72 6573 706f 6e73 6520     arp_response 
+000005f0: 3d20 7379 6e63 5f73 656e 645f 6172 7028  = sync_send_arp(
+00000600: 7265 7175 6573 745f 7061 636b 6574 2c20  request_packet, 
+00000610: 7374 7265 616d 2c20 7469 6d65 6f75 7429  stream, timeout)
+00000620: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000630: 6172 705f 7265 7370 6f6e 7365 0a0a 0a61  arp_response...a
+00000640: 7379 6e63 2064 6566 2061 7265 7175 6573  sync def areques
+00000650: 7428 0a20 2020 2020 2020 2069 6e74 6572  t(.        inter
+00000660: 6661 6365 3a20 7374 722c 0a20 2020 2020  face: str,.     
+00000670: 2020 2074 6172 6765 745f 6970 3a20 7374     target_ip: st
+00000680: 722c 0a20 2020 2020 2020 2074 696d 656f  r,.        timeo
+00000690: 7574 3a20 7479 7069 6e67 2e4f 7074 696f  ut: typing.Optio
+000006a0: 6e61 6c5b 666c 6f61 745d 203d 204e 6f6e  nal[float] = Non
+000006b0: 652c 0a20 2020 2020 2020 2073 6f63 6b3a  e,.        sock:
+000006c0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+000006d0: 5b53 6f63 6b65 7449 6e74 6572 6661 6365  [SocketInterface
+000006e0: 5d20 3d20 4e6f 6e65 0a29 202d 3e20 4172  ] = None.) -> Ar
+000006f0: 7050 6163 6b65 743a 0a20 2020 2069 6620  pPacket:.    if 
+00000700: 6e6f 7420 736f 636b 3a20 2023 2070 7261  not sock:  # pra
+00000710: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+00000720: 2020 2020 2020 736f 636b 203d 2073 6f63        sock = soc
+00000730: 6b65 742e 736f 636b 6574 2873 6f63 6b65  ket.socket(socke
+00000740: 742e 5046 5f50 4143 4b45 542c 2073 6f63  t.PF_PACKET, soc
+00000750: 6b65 742e 534f 434b 5f52 4157 2c20 736f  ket.SOCK_RAW, so
+00000760: 636b 6574 2e6e 746f 6873 2830 7830 3030  cket.ntohs(0x000
+00000770: 3329 290a 2020 2020 7769 7468 2041 7379  3)).    with Asy
+00000780: 6e63 5374 7265 616d 2869 6e74 6572 6661  ncStream(interfa
+00000790: 6365 3d69 6e74 6572 6661 6365 2c0a 2020  ce=interface,.  
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 2020 736f 636b 3d73 6f63 6b29 2061 7320    sock=sock) as 
+000007c0: 7374 7265 616d 3a0a 2020 2020 2020 2020  stream:.        
+000007d0: 7265 7175 6573 745f 7061 636b 6574 203d  request_packet =
+000007e0: 2062 7569 6c64 5f61 7270 5f70 6163 6b65   build_arp_packe
+000007f0: 7428 696e 7465 7266 6163 652c 2074 6172  t(interface, tar
+00000800: 6765 745f 6970 290a 2020 2020 2020 2020  get_ip).        
+00000810: 6172 705f 7265 7370 6f6e 7365 203d 2061  arp_response = a
+00000820: 7761 6974 2061 7379 6e63 5f73 656e 645f  wait async_send_
+00000830: 6172 7028 7265 7175 6573 745f 7061 636b  arp(request_pack
+00000840: 6574 2c20 7374 7265 616d 2c20 7469 6d65  et, stream, time
+00000850: 6f75 7429 0a20 2020 2020 2020 2072 6574  out).        ret
+00000860: 7572 6e20 6172 705f 7265 7370 6f6e 7365  urn arp_response
+00000870: 0a                                       .
```

### Comparing `aioarp-0.0.4/.ruff_cache/content/16b1a595f0c0b695` & `aioarp-0.0.5/aioarp/_backends/_async.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,108 @@
-00000000: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-00000010: 0f00 0000 0000 0000 556e 736f 7274 6564  ........Unsorted
-00000020: 496d 706f 7274 7329 0000 0000 0000 0049  Imports).......I
-00000030: 6d70 6f72 7420 626c 6f63 6b20 6973 2075  mport block is u
-00000040: 6e2d 736f 7274 6564 206f 7220 756e 2d66  n-sorted or un-f
-00000050: 6f72 6d61 7474 6564 0110 0000 0000 0000  ormatted........
-00000060: 004f 7267 616e 697a 6520 696d 706f 7274  .Organize import
-00000070: 7300 0000 0045 0000 0001 0100 0000 0000  s....E..........
-00000080: 0000 0000 0000 4500 0000 0144 0000 0000  ......E....D....
-00000090: 0000 0069 6d70 6f72 7420 736f 636b 6574  ...import socket
-000000a0: 0a69 6d70 6f72 7420 7479 7069 6e67 0a0a  .import typing..
-000000b0: 6672 6f6d 2061 696f 6172 7020 696d 706f  from aioarp impo
-000000c0: 7274 205f 6578 6365 7074 696f 6e73 2061  rt _exceptions a
-000000d0: 7320 6578 630a 0a03 0000 0000 0000 0000  s exc...........
-000000e0: 0000 0000 0000 0001 0000 0000 0000 0032  ...............2
-000000f0: 0000 0000 0000 002f 686f 6d65 2f74 6573  ......./home/tes
-00000100: 742f 4465 736b 746f 702f 6169 6f61 7270  t/Desktop/aioarp
-00000110: 2f61 696f 6172 702f 6261 636b 656e 6473  /aioarp/backends
-00000120: 2f5f 7379 6e63 2e70 79bf 0300 0000 0000  /_sync.py.......
-00000130: 0069 6d70 6f72 7420 736f 636b 6574 0a69  .import socket.i
-00000140: 6d70 6f72 7420 7479 7069 6e67 0a0a 6672  mport typing..fr
-00000150: 6f6d 2061 696f 6172 7020 696d 706f 7274  om aioarp import
-00000160: 205f 6578 6365 7074 696f 6e73 2061 7320   _exceptions as 
-00000170: 6578 630a 0a0a 2320 544f 444f 3a20 6164  exc...# TODO: ad
-00000180: 6420 6572 726f 7220 6d61 700a 0a63 6c61  d error map..cla
-00000190: 7373 2053 7472 6561 6d3a 0a0a 2020 2020  ss Stream:..    
-000001a0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-000001b0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-000001c0: 2020 2020 696e 7465 7266 6163 653a 2073      interface: s
-000001d0: 7472 293a 0a20 2020 2020 2020 2073 6f63  tr):.        soc
-000001e0: 6b20 3d20 736f 636b 6574 2e73 6f63 6b65  k = socket.socke
-000001f0: 7428 736f 636b 6574 2e50 465f 5041 434b  t(socket.PF_PACK
-00000200: 4554 2c20 736f 636b 6574 2e53 4f43 4b5f  ET, socket.SOCK_
-00000210: 5241 572c 2073 6f63 6b65 742e 6e74 6f68  RAW, socket.ntoh
-00000220: 7328 3078 3030 3033 2929 0a20 2020 2020  s(0x0003)).     
-00000230: 2020 2073 6f63 6b2e 6269 6e64 2828 696e     sock.bind((in
-00000240: 7465 7266 6163 652c 2030 2929 0a20 2020  terface, 0)).   
-00000250: 2020 2020 2073 656c 662e 736f 636b 203d       self.sock =
-00000260: 2073 6f63 6b0a 0a20 2020 2064 6566 2072   sock..    def r
-00000270: 6563 6569 7665 5f66 7261 6d65 2873 656c  eceive_frame(sel
-00000280: 662c 2074 696d 656f 7574 3a20 666c 6f61  f, timeout: floa
-00000290: 7429 202d 3e20 6279 7465 733a 0a20 2020  t) -> bytes:.   
-000002a0: 2020 2020 2073 656c 662e 736f 636b 2e73       self.sock.s
-000002b0: 6574 7469 6d65 6f75 7428 7469 6d65 6f75  ettimeout(timeou
-000002c0: 7429 0a20 2020 2020 2020 2074 7279 3a0a  t).        try:.
-000002d0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-000002e0: 6520 3d20 7365 6c66 2e73 6f63 6b2e 7265  e = self.sock.re
-000002f0: 6376 2831 3132 3331 3233 290a 2020 2020  cv(1123123).    
-00000300: 2020 2020 6578 6365 7074 2073 6f63 6b65      except socke
-00000310: 742e 7469 6d65 6f75 743a 0a20 2020 2020  t.timeout:.     
-00000320: 2020 2020 2020 2072 6169 7365 2065 7863         raise exc
-00000330: 2e52 6561 6454 696d 656f 7574 4572 726f  .ReadTimeoutErro
-00000340: 7228 290a 2020 2020 2020 2020 7265 7475  r().        retu
-00000350: 726e 2066 7261 6d65 0a0a 2020 2020 6465  rn frame..    de
-00000360: 6620 7772 6974 655f 6672 616d 6528 7365  f write_frame(se
-00000370: 6c66 2c20 6672 616d 653a 2062 7974 6573  lf, frame: bytes
-00000380: 2c20 7469 6d65 6f75 743a 2066 6c6f 6174  , timeout: float
-00000390: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000003a0: 2020 2073 656c 662e 736f 636b 2e73 6574     self.sock.set
-000003b0: 7469 6d65 6f75 7428 7469 6d65 6f75 7429  timeout(timeout)
-000003c0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-000003d0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000003e0: 6f63 6b2e 7365 6e64 616c 6c28 6672 616d  ock.sendall(fram
-000003f0: 6529 0a20 2020 2020 2020 2065 7863 6570  e).        excep
-00000400: 7420 736f 636b 6574 2e74 696d 656f 7574  t socket.timeout
-00000410: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00000420: 6973 6520 6578 632e 5772 6974 6554 696d  ise exc.WriteTim
-00000430: 656f 7574 4572 726f 7228 290a 0a20 2020  eoutError()..   
-00000440: 2064 6566 205f 5f65 6e74 6572 5f5f 2873   def __enter__(s
-00000450: 656c 6629 202d 3e20 2753 7472 6561 6d27  elf) -> 'Stream'
-00000460: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00000470: 2073 656c 660a 0a20 2020 2064 6566 205f   self..    def _
-00000480: 5f65 7869 745f 5f28 7365 6c66 2c20 6578  _exit__(self, ex
-00000490: 635f 7479 7065 3a20 7479 7069 6e67 2e41  c_type: typing.A
-000004a0: 6e79 2c20 6578 635f 7661 6c3a 2074 7970  ny, exc_val: typ
-000004b0: 696e 672e 416e 792c 2065 7863 5f74 623a  ing.Any, exc_tb:
-000004c0: 2074 7970 696e 672e 416e 7929 202d 3e20   typing.Any) -> 
-000004d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
-000004e0: 6c66 2e73 6f63 6b2e 636c 6f73 6528 290a  lf.sock.close().
+00000000: 696d 706f 7274 2073 656c 6563 740a 696d  import select.im
+00000010: 706f 7274 2073 6f63 6b65 740a 696d 706f  port socket.impo
+00000020: 7274 2074 7970 696e 670a 0a69 6d70 6f72  rt typing..impor
+00000030: 7420 616e 7969 6f0a 0a66 726f 6d20 6169  t anyio..from ai
+00000040: 6f61 7270 2069 6d70 6f72 7420 5f65 7863  oarp import _exc
+00000050: 6570 7469 6f6e 7320 6173 2065 7863 0a0a  eptions as exc..
+00000060: 6672 6f6d 202e 5f62 6173 6520 696d 706f  from ._base impo
+00000070: 7274 2053 6f63 6b65 7449 6e74 6572 6661  rt SocketInterfa
+00000080: 6365 0a0a 5f5f 616c 6c5f 5f20 3d20 280a  ce..__all__ = (.
+00000090: 2020 2020 2741 7379 6e63 5374 7265 616d      'AsyncStream
+000000a0: 272c 0a29 0a0a 636c 6173 7320 4173 796e  ',.)..class Asyn
+000000b0: 6353 7472 6561 6d3a 0a0a 2020 2020 6465  cStream:..    de
+000000c0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+000000d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000000e0: 2020 696e 7465 7266 6163 653a 2073 7472    interface: str
+000000f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000100: 2020 2073 6f63 6b3a 2074 7970 696e 672e     sock: typing.
+00000110: 4f70 7469 6f6e 616c 5b53 6f63 6b65 7449  Optional[SocketI
+00000120: 6e74 6572 6661 6365 5d20 3d20 4e6f 6e65  nterface] = None
+00000130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000140: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00000150: 662e 736f 636b 3a20 536f 636b 6574 496e  f.sock: SocketIn
+00000160: 7465 7266 6163 650a 2020 2020 2020 2020  terface.        
+00000170: 6966 206e 6f74 2073 6f63 6b3a 2020 2320  if not sock:  # 
+00000180: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+00000190: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000001a0: 662e 736f 636b 203d 2073 6f63 6b65 742e  f.sock = socket.
+000001b0: 736f 636b 6574 2873 6f63 6b65 742e 5046  socket(socket.PF
+000001c0: 5f50 4143 4b45 542c 2073 6f63 6b65 742e  _PACKET, socket.
+000001d0: 534f 434b 5f52 4157 2c20 736f 636b 6574  SOCK_RAW, socket
+000001e0: 2e6e 746f 6873 2830 7830 3030 3329 290a  .ntohs(0x0003)).
+000001f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00000200: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00000210: 6f63 6b20 3d20 736f 636b 0a20 2020 2020  ock = sock.     
+00000220: 2020 2073 656c 662e 736f 636b 2e62 696e     self.sock.bin
+00000230: 6428 2869 6e74 6572 6661 6365 2c20 3029  d((interface, 0)
+00000240: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+00000250: 2072 6563 6569 7665 5f66 7261 6d65 2873   receive_frame(s
+00000260: 656c 662c 2074 696d 656f 7574 3a20 666c  elf, timeout: fl
+00000270: 6f61 7429 202d 3e20 6279 7465 733a 0a20  oat) -> bytes:. 
+00000280: 2020 2020 2020 2066 7261 6d65 3a20 7479         frame: ty
+00000290: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6279  ping.Optional[by
+000002a0: 7465 735d 0a20 2020 2020 2020 2077 6974  tes].        wit
+000002b0: 6820 616e 7969 6f2e 6d6f 7665 5f6f 6e5f  h anyio.move_on_
+000002c0: 6166 7465 7228 7469 6d65 6f75 7429 3a0a  after(timeout):.
+000002d0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
+000002e0: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
+000002f0: 2020 2020 2020 2020 722c 205f 2c20 5f20          r, _, _ 
+00000300: 3d20 7365 6c65 6374 2e73 656c 6563 7428  = select.select(
+00000310: 5b73 656c 662e 736f 636b 5d2c 205b 5d2c  [self.sock], [],
+00000320: 205b 5d2c 2030 2e30 3030 3031 290a 2020   [], 0.00001).  
+00000330: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00000340: 2072 3a0a 2020 2020 2020 2020 2020 2020   r:.            
+00000350: 2020 2020 2020 2020 6672 616d 6520 3d20          frame = 
+00000360: 7365 6c66 2e73 6f63 6b2e 7265 6376 2831  self.sock.recv(1
+00000370: 3132 3331 3233 290a 2020 2020 2020 2020  123123).        
+00000380: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00000390: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+000003a0: 2020 6177 6169 7420 616e 7969 6f2e 736c    await anyio.sl
+000003b0: 6565 7028 3029 2020 2320 7072 6167 6d61  eep(0)  # pragma
+000003c0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
+000003d0: 2020 2069 6620 6e6f 7420 6672 616d 653a     if not frame:
+000003e0: 2020 2023 2070 7261 676d 613a 206e 6f20     # pragma: no 
+000003f0: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+00000400: 2020 7261 6973 6520 6578 632e 5265 6164    raise exc.Read
+00000410: 5469 6d65 6f75 7445 7272 6f72 2829 0a20  TimeoutError(). 
+00000420: 2020 2020 2020 2072 6574 7572 6e20 6672         return fr
+00000430: 616d 650a 0a20 2020 2061 7379 6e63 2064  ame..    async d
+00000440: 6566 2077 7269 7465 5f66 7261 6d65 2873  ef write_frame(s
+00000450: 656c 662c 2066 7261 6d65 3a20 6279 7465  elf, frame: byte
+00000460: 732c 2074 696d 656f 7574 3a20 666c 6f61  s, timeout: floa
+00000470: 7429 202d 3e20 4e6f 6e65 3a0a 0a20 2020  t) -> None:..   
+00000480: 2020 2020 2077 6974 6820 616e 7969 6f2e       with anyio.
+00000490: 6d6f 7665 5f6f 6e5f 6166 7465 7228 7469  move_on_after(ti
+000004a0: 6d65 6f75 7429 3a0a 2020 2020 2020 2020  meout):.        
+000004b0: 2020 2020 7768 696c 6520 6672 616d 653a      while frame:
+000004c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004d0: 205f 2c20 772c 205f 203d 2073 656c 6563   _, w, _ = selec
+000004e0: 742e 7365 6c65 6374 285b 5d2c 205b 7365  t.select([], [se
+000004f0: 6c66 2e73 6f63 6b5d 2c20 5b5d 2c20 302e  lf.sock], [], 0.
+00000500: 3030 3030 3129 0a0a 2020 2020 2020 2020  00001)..        
+00000510: 2020 2020 2020 2020 6e73 656e 7420 3d20          nsent = 
+00000520: 7365 6c66 2e73 6f63 6b2e 7365 6e64 2866  self.sock.send(f
+00000530: 7261 6d65 290a 2020 2020 2020 2020 2020  rame).          
+00000540: 2020 2020 2020 6672 616d 6520 3d20 6672        frame = fr
+00000550: 616d 655b 6e73 656e 743a 5d0a 2020 2020  ame[nsent:].    
+00000560: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00000570: 7420 616e 7969 6f2e 736c 6565 7028 3029  t anyio.sleep(0)
+00000580: 0a20 2020 2020 2020 2069 6620 6672 616d  .        if fram
+00000590: 653a 2020 2320 7072 6167 6d61 3a20 6e6f  e:  # pragma: no
+000005a0: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
+000005b0: 2020 2072 6169 7365 2065 7863 2e57 7269     raise exc.Wri
+000005c0: 7465 5469 6d65 6f75 7445 7272 6f72 2829  teTimeoutError()
+000005d0: 0a0a 2020 2020 6465 6620 636c 6f73 6528  ..    def close(
+000005e0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+000005f0: 2020 2020 2020 2073 656c 662e 736f 636b         self.sock
+00000600: 2e63 6c6f 7365 2829 0a0a 2020 2020 6465  .close()..    de
+00000610: 6620 5f5f 656e 7465 725f 5f28 7365 6c66  f __enter__(self
+00000620: 2920 2d3e 2022 4173 796e 6353 7472 6561  ) -> "AsyncStrea
+00000630: 6d22 3a0a 2020 2020 2020 2020 7265 7475  m":.        retu
+00000640: 726e 2073 656c 660a 0a20 2020 2064 6566  rn self..    def
+00000650: 205f 5f65 7869 745f 5f28 7365 6c66 2c20   __exit__(self, 
+00000660: 6578 635f 7479 7065 3a20 7479 7069 6e67  exc_type: typing
+00000670: 2e41 6e79 2c20 6578 635f 7661 6c3a 2074  .Any, exc_val: t
+00000680: 7970 696e 672e 416e 792c 2065 7863 5f74  yping.Any, exc_t
+00000690: 623a 2074 7970 696e 672e 416e 7929 202d  b: typing.Any) -
+000006a0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000006b0: 7365 6c66 2e63 6c6f 7365 2829 0a         self.close().
```

### Comparing `aioarp-0.0.4/.ruff_cache/content/18bd9323e775c06` & `aioarp-0.0.5/aioarp/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,113 +1,107 @@
-00000000: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
-00000010: 6169 6f61 7270 2e5f 7574 696c 7304 0000  aioarp._utils...
-00000020: 0000 0000 0006 0000 0000 0000 0073 6f63  .............soc
-00000030: 6b65 7400 0000 000d 0000 0005 0000 0000  ket.............
-00000040: 0000 0066 636e 746c 0e00 0000 1a00 0000  ...fcntl........
-00000050: 0600 0000 0000 0000 7374 7275 6374 1b00  ........struct..
-00000060: 0000 2800 0000 0900 0000 0000 0000 6970  ..(...........ip
-00000070: 6164 6472 6573 7329 0000 0039 0000 0001  address)...9....
-00000080: 0000 0000 0000 000f 0000 0000 0000 0055  ...............U
-00000090: 6e73 6f72 7465 6449 6d70 6f72 7473 2900  nsortedImports).
-000000a0: 0000 0000 0000 496d 706f 7274 2062 6c6f  ......Import blo
-000000b0: 636b 2069 7320 756e 2d73 6f72 7465 6420  ck is un-sorted 
-000000c0: 6f72 2075 6e2d 666f 726d 6174 7465 6401  or un-formatted.
-000000d0: 1000 0000 0000 0000 4f72 6761 6e69 7a65  ........Organize
-000000e0: 2069 6d70 6f72 7473 0000 0000 3b00 0000   imports....;...
-000000f0: 0101 0000 0000 0000 0000 0000 003b 0000  .............;..
-00000100: 0001 3b00 0000 0000 0000 696d 706f 7274  ..;.......import
-00000110: 2066 636e 746c 0a69 6d70 6f72 7420 6970   fcntl.import ip
-00000120: 6164 6472 6573 730a 696d 706f 7274 2073  address.import s
-00000130: 6f63 6b65 740a 696d 706f 7274 2073 7472  ocket.import str
-00000140: 7563 740a 0a03 0000 0000 0000 0000 0000  uct.............
-00000150: 0000 0000 0001 0000 0000 0000 002a 0000  .............*..
-00000160: 0000 0000 002f 686f 6d65 2f74 6573 742f  ...../home/test/
-00000170: 4465 736b 746f 702f 6169 6f61 7270 2f61  Desktop/aioarp/a
-00000180: 696f 6172 702f 5f75 7469 6c73 2e70 7975  ioarp/_utils.pyu
-00000190: 0500 0000 0000 0069 6d70 6f72 7420 736f  .......import so
-000001a0: 636b 6574 0a69 6d70 6f72 7420 6663 6e74  cket.import fcnt
-000001b0: 6c0a 696d 706f 7274 2073 7472 7563 740a  l.import struct.
-000001c0: 696d 706f 7274 2069 7061 6464 7265 7373  import ipaddress
-000001d0: 0a0a 5f5f 616c 6c5f 5f20 3d20 280a 2020  ..__all__ = (.  
-000001e0: 2020 2769 735f 7661 6c69 645f 6970 7634    'is_valid_ipv4
-000001f0: 272c 0a20 2020 2027 6765 745f 6d61 6327  ',.    'get_mac'
-00000200: 2c0a 2020 2020 2767 6574 5f69 7027 2c0a  ,.    'get_ip',.
-00000210: 2020 2020 2765 6e66 6f72 6365 5f6d 6163      'enforce_mac
-00000220: 272c 0a20 2020 2027 656e 666f 7263 655f  ',.    'enforce_
-00000230: 6970 272c 0a20 2020 2027 7061 7273 655f  ip',.    'parse_
-00000240: 6d61 6327 2c0a 2020 2020 2770 6172 7365  mac',.    'parse
-00000250: 5f69 7027 0a29 0a0a 6465 6620 6973 5f76  _ip'.)..def is_v
-00000260: 616c 6964 5f69 7076 3428 6970 3a20 7374  alid_ipv4(ip: st
-00000270: 7229 202d 3e20 626f 6f6c 3a0a 2020 2020  r) -> bool:.    
-00000280: 7472 793a 0a20 2020 2020 2020 2069 7061  try:.        ipa
-00000290: 6464 7265 7373 2e49 5076 3441 6464 7265  ddress.IPv4Addre
-000002a0: 7373 2869 7029 0a20 2020 2020 2020 2072  ss(ip).        r
-000002b0: 6574 7572 6e20 5472 7565 0a20 2020 2065  eturn True.    e
-000002c0: 7863 6570 7420 6970 6164 6472 6573 732e  xcept ipaddress.
-000002d0: 4164 6472 6573 7356 616c 7565 4572 726f  AddressValueErro
-000002e0: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
-000002f0: 6e20 4661 6c73 650a 0a0a 6465 6620 6765  n False...def ge
-00000300: 745f 6d61 6328 696e 7465 7266 6163 6529  t_mac(interface)
-00000310: 202d 3e20 7374 723a 0a20 2020 2077 6974   -> str:.    wit
-00000320: 6820 736f 636b 6574 2e73 6f63 6b65 7428  h socket.socket(
-00000330: 736f 636b 6574 2e41 465f 494e 4554 2c20  socket.AF_INET, 
-00000340: 736f 636b 6574 2e53 4f43 4b5f 4447 5241  socket.SOCK_DGRA
-00000350: 4d29 2061 7320 733a 0a20 2020 2020 2020  M) as s:.       
-00000360: 2069 6e66 6f20 3d20 6663 6e74 6c2e 696f   info = fcntl.io
-00000370: 6374 6c28 732e 6669 6c65 6e6f 2829 2c20  ctl(s.fileno(), 
-00000380: 3078 3839 3237 2c20 7374 7275 6374 2e70  0x8927, struct.p
-00000390: 6163 6b28 2732 3536 7327 2c20 6279 7465  ack('256s', byte
-000003a0: 7328 696e 7465 7266 6163 652c 2027 7574  s(interface, 'ut
-000003b0: 662d 3827 295b 3a31 355d 2929 0a20 2020  f-8')[:15])).   
-000003c0: 2020 2020 2072 6574 7572 6e20 273a 272e       return ':'.
-000003d0: 6a6f 696e 2827 2530 3278 2720 2520 6220  join('%02x' % b 
-000003e0: 666f 7220 6220 696e 2069 6e66 6f5b 3138  for b in info[18
-000003f0: 3a32 345d 290a 0a0a 6465 6620 6765 745f  :24])...def get_
-00000400: 6970 2829 202d 3e20 7374 723a 0a20 2020  ip() -> str:.   
-00000410: 2077 6974 6820 736f 636b 6574 2e73 6f63   with socket.soc
-00000420: 6b65 7428 736f 636b 6574 2e41 465f 494e  ket(socket.AF_IN
-00000430: 4554 2c20 736f 636b 6574 2e53 4f43 4b5f  ET, socket.SOCK_
-00000440: 4447 5241 4d29 2061 7320 733a 0a20 2020  DGRAM) as s:.   
-00000450: 2020 2020 2073 2e63 6f6e 6e65 6374 2828       s.connect((
-00000460: 2231 2e31 2e31 2e31 222c 2038 3029 290a  "1.1.1.1", 80)).
-00000470: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000480: 2e67 6574 736f 636b 6e61 6d65 2829 5b30  .getsockname()[0
-00000490: 5d0a 0a0a 6465 6620 656e 666f 7263 655f  ]...def enforce_
-000004a0: 6d61 6328 6d61 633a 2073 7472 2920 2d3e  mac(mac: str) ->
-000004b0: 2062 7974 6573 3a0a 2020 2020 6d61 635f   bytes:.    mac_
-000004c0: 6279 7465 7320 3d20 5b5d 0a20 2020 2066  bytes = [].    f
-000004d0: 6f72 2062 2069 6e20 6d61 632e 7370 6c69  or b in mac.spli
-000004e0: 7428 273a 2729 3a0a 2020 2020 2020 2020  t(':'):.        
-000004f0: 6d61 635f 6279 7465 732e 6170 7065 6e64  mac_bytes.append
-00000500: 2869 6e74 2862 2c20 3136 2929 0a20 2020  (int(b, 16)).   
-00000510: 2072 6574 7572 6e20 6279 7465 7328 6d61   return bytes(ma
-00000520: 635f 6279 7465 7329 0a0a 0a64 6566 2065  c_bytes)...def e
-00000530: 6e66 6f72 6365 5f69 7028 6970 3a20 7374  nforce_ip(ip: st
-00000540: 7229 202d 3e20 6279 7465 733a 0a20 2020  r) -> bytes:.   
-00000550: 2069 705f 6279 7465 7320 3d20 5b5d 0a20   ip_bytes = []. 
-00000560: 2020 2066 6f72 2062 2069 6e20 6970 2e73     for b in ip.s
-00000570: 706c 6974 2827 2e27 293a 0a20 2020 2020  plit('.'):.     
-00000580: 2020 2069 705f 6279 7465 732e 6170 7065     ip_bytes.appe
-00000590: 6e64 2869 6e74 2862 2929 0a20 2020 2072  nd(int(b)).    r
-000005a0: 6574 7572 6e20 6279 7465 7328 6970 5f62  eturn bytes(ip_b
-000005b0: 7974 6573 290a 0a0a 6465 6620 7061 7273  ytes)...def pars
-000005c0: 655f 6d61 6328 6d61 633a 2062 7974 6573  e_mac(mac: bytes
-000005d0: 2920 2d3e 2073 7472 3a0a 2020 2020 6d61  ) -> str:.    ma
-000005e0: 635f 7061 7274 7320 3d20 5b5d 0a20 2020  c_parts = [].   
-000005f0: 2066 6f72 2062 2069 6e20 6d61 633a 0a20   for b in mac:. 
-00000600: 2020 2020 2020 2068 6578 203d 2066 277b         hex = f'{
-00000610: 623a 787d 270a 2020 2020 2020 2020 6966  b:x}'.        if
-00000620: 206c 656e 2868 6578 2920 3d3d 2031 3a0a   len(hex) == 1:.
-00000630: 2020 2020 2020 2020 2020 2020 6865 7820              hex 
-00000640: 3d20 2730 2720 2b20 6865 780a 2020 2020  = '0' + hex.    
-00000650: 2020 2020 6d61 635f 7061 7274 732e 6170      mac_parts.ap
-00000660: 7065 6e64 2868 6578 290a 2020 2020 7265  pend(hex).    re
-00000670: 7475 726e 2027 3a27 2e6a 6f69 6e28 6d61  turn ':'.join(ma
-00000680: 635f 7061 7274 7329 0a0a 0a64 6566 2070  c_parts)...def p
-00000690: 6172 7365 5f69 7028 6970 3a20 6279 7465  arse_ip(ip: byte
-000006a0: 7329 202d 3e20 7374 723a 0a20 2020 2069  s) -> str:.    i
-000006b0: 705f 7061 7274 7320 3d20 5b5d 0a20 2020  p_parts = [].   
-000006c0: 2066 6f72 2062 2069 6e20 6970 3a0a 2020   for b in ip:.  
-000006d0: 2020 2020 2020 6970 5f70 6172 7473 2e61        ip_parts.a
-000006e0: 7070 656e 6428 7374 7228 6229 290a 2020  ppend(str(b)).  
-000006f0: 2020 7265 7475 726e 2027 2e27 2e6a 6f69    return '.'.joi
-00000700: 6e28 6970 5f70 6172 7473 290a            n(ip_parts).
+00000000: 696d 706f 7274 2066 636e 746c 0a69 6d70  import fcntl.imp
+00000010: 6f72 7420 6970 6164 6472 6573 730a 696d  ort ipaddress.im
+00000020: 706f 7274 2073 6f63 6b65 740a 696d 706f  port socket.impo
+00000030: 7274 2073 7472 7563 740a 696d 706f 7274  rt struct.import
+00000040: 2074 7970 696e 670a 0a5f 5f61 6c6c 5f5f   typing..__all__
+00000050: 203d 2028 0a20 2020 2027 6973 5f76 616c   = (.    'is_val
+00000060: 6964 5f69 7076 3427 2c0a 2020 2020 2767  id_ipv4',.    'g
+00000070: 6574 5f6d 6163 272c 0a20 2020 2027 6765  et_mac',.    'ge
+00000080: 745f 6970 272c 0a20 2020 2027 656e 666f  t_ip',.    'enfo
+00000090: 7263 655f 6d61 6327 2c0a 2020 2020 2765  rce_mac',.    'e
+000000a0: 6e66 6f72 6365 5f69 7027 2c0a 2020 2020  nforce_ip',.    
+000000b0: 2770 6172 7365 5f6d 6163 272c 0a20 2020  'parse_mac',.   
+000000c0: 2027 7061 7273 655f 6970 270a 290a 0a4f   'parse_ip'.)..O
+000000d0: 5552 5f4d 4143 203d 204e 6f6e 650a 4f55  UR_MAC = None.OU
+000000e0: 525f 4950 203d 204e 6f6e 650a 0a0a 6465  R_IP = None...de
+000000f0: 6620 6973 5f76 616c 6964 5f69 7076 3428  f is_valid_ipv4(
+00000100: 6970 3a20 7374 7229 202d 3e20 626f 6f6c  ip: str) -> bool
+00000110: 3a0a 2020 2020 7472 793a 0a20 2020 2020  :.    try:.     
+00000120: 2020 2069 7061 6464 7265 7373 2e49 5076     ipaddress.IPv
+00000130: 3441 6464 7265 7373 2869 7029 0a20 2020  4Address(ip).   
+00000140: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00000150: 0a20 2020 2065 7863 6570 7420 6970 6164  .    except ipad
+00000160: 6472 6573 732e 4164 6472 6573 7356 616c  dress.AddressVal
+00000170: 7565 4572 726f 723a 0a20 2020 2020 2020  ueError:.       
+00000180: 2072 6574 7572 6e20 4661 6c73 650a 0a0a   return False...
+00000190: 6465 6620 6765 745f 6d61 6328 696e 7465  def get_mac(inte
+000001a0: 7266 6163 653a 2073 7472 2920 2d3e 2073  rface: str) -> s
+000001b0: 7472 3a20 2023 2070 7261 676d 613a 206e  tr:  # pragma: n
+000001c0: 6f20 636f 7665 720a 2020 2020 676c 6f62  o cover.    glob
+000001d0: 616c 204f 5552 5f4d 4143 0a20 2020 2069  al OUR_MAC.    i
+000001e0: 6620 4f55 525f 4d41 433a 0a20 2020 2020  f OUR_MAC:.     
+000001f0: 2020 2072 6574 7572 6e20 4f55 525f 4d41     return OUR_MA
+00000200: 430a 2020 2020 7769 7468 2073 6f63 6b65  C.    with socke
+00000210: 742e 736f 636b 6574 2873 6f63 6b65 742e  t.socket(socket.
+00000220: 4146 5f49 4e45 542c 2073 6f63 6b65 742e  AF_INET, socket.
+00000230: 534f 434b 5f44 4752 414d 2920 6173 2073  SOCK_DGRAM) as s
+00000240: 3a0a 2020 2020 2020 2020 696e 666f 203d  :.        info =
+00000250: 2066 636e 746c 2e69 6f63 746c 2873 2e66   fcntl.ioctl(s.f
+00000260: 696c 656e 6f28 292c 2030 7838 3932 372c  ileno(), 0x8927,
+00000270: 2073 7472 7563 742e 7061 636b 2827 3235   struct.pack('25
+00000280: 3673 272c 2062 7974 6573 2869 6e74 6572  6s', bytes(inter
+00000290: 6661 6365 2c20 2775 7466 2d38 2729 5b3a  face, 'utf-8')[:
+000002a0: 3135 5d29 290a 2020 2020 2020 2020 6d61  15])).        ma
+000002b0: 6320 3d20 273a 272e 6a6f 696e 2827 2530  c = ':'.join('%0
+000002c0: 3278 2720 2520 6220 666f 7220 6220 696e  2x' % b for b in
+000002d0: 2069 6e66 6f5b 3138 3a32 345d 290a 2020   info[18:24]).  
+000002e0: 2020 2020 2020 4f55 525f 4d41 4320 3d20        OUR_MAC = 
+000002f0: 6d61 630a 2020 2020 2020 2020 7265 7475  mac.        retu
+00000300: 726e 204f 5552 5f4d 4143 0a0a 0a64 6566  rn OUR_MAC...def
+00000310: 2067 6574 5f69 7028 2920 2d3e 2073 7472   get_ip() -> str
+00000320: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+00000330: 636f 7665 720a 2020 2020 676c 6f62 616c  cover.    global
+00000340: 204f 5552 5f49 500a 2020 2020 6966 204f   OUR_IP.    if O
+00000350: 5552 5f49 503a 0a20 2020 2020 2020 2072  UR_IP:.        r
+00000360: 6574 7572 6e20 4f55 525f 4950 0a20 2020  eturn OUR_IP.   
+00000370: 2077 6974 6820 736f 636b 6574 2e73 6f63   with socket.soc
+00000380: 6b65 7428 736f 636b 6574 2e41 465f 494e  ket(socket.AF_IN
+00000390: 4554 2c20 736f 636b 6574 2e53 4f43 4b5f  ET, socket.SOCK_
+000003a0: 4447 5241 4d29 2061 7320 733a 0a20 2020  DGRAM) as s:.   
+000003b0: 2020 2020 2073 2e63 6f6e 6e65 6374 2828       s.connect((
+000003c0: 2231 2e31 2e31 2e31 222c 2038 3029 290a  "1.1.1.1", 80)).
+000003d0: 2020 2020 2020 2020 6970 203d 2074 7970          ip = typ
+000003e0: 696e 672e 6361 7374 2873 7472 2c20 732e  ing.cast(str, s.
+000003f0: 6765 7473 6f63 6b6e 616d 6528 295b 305d  getsockname()[0]
+00000400: 290a 2020 2020 2020 2020 4f55 525f 4950  ).        OUR_IP
+00000410: 203d 2069 700a 2020 2020 2020 2020 7265   = ip.        re
+00000420: 7475 726e 204f 5552 5f49 500a 0a0a 6465  turn OUR_IP...de
+00000430: 6620 656e 666f 7263 655f 6d61 6328 6d61  f enforce_mac(ma
+00000440: 633a 2073 7472 2920 2d3e 2062 7974 6573  c: str) -> bytes
+00000450: 3a0a 2020 2020 6d61 635f 6279 7465 7320  :.    mac_bytes 
+00000460: 3d20 5b5d 0a20 2020 2066 6f72 2062 2069  = [].    for b i
+00000470: 6e20 6d61 632e 7370 6c69 7428 273a 2729  n mac.split(':')
+00000480: 3a0a 2020 2020 2020 2020 6d61 635f 6279  :.        mac_by
+00000490: 7465 732e 6170 7065 6e64 2869 6e74 2862  tes.append(int(b
+000004a0: 2c20 3136 2929 0a20 2020 2072 6574 7572  , 16)).    retur
+000004b0: 6e20 6279 7465 7328 6d61 635f 6279 7465  n bytes(mac_byte
+000004c0: 7329 0a0a 0a64 6566 2065 6e66 6f72 6365  s)...def enforce
+000004d0: 5f69 7028 6970 3a20 7374 7229 202d 3e20  _ip(ip: str) -> 
+000004e0: 6279 7465 733a 0a20 2020 2069 705f 6279  bytes:.    ip_by
+000004f0: 7465 7320 3d20 5b5d 0a20 2020 2066 6f72  tes = [].    for
+00000500: 2062 2069 6e20 6970 2e73 706c 6974 2827   b in ip.split('
+00000510: 2e27 293a 0a20 2020 2020 2020 2069 705f  .'):.        ip_
+00000520: 6279 7465 732e 6170 7065 6e64 2869 6e74  bytes.append(int
+00000530: 2862 2929 0a20 2020 2072 6574 7572 6e20  (b)).    return 
+00000540: 6279 7465 7328 6970 5f62 7974 6573 290a  bytes(ip_bytes).
+00000550: 0a0a 6465 6620 7061 7273 655f 6d61 6328  ..def parse_mac(
+00000560: 6d61 633a 2062 7974 6573 2920 2d3e 2073  mac: bytes) -> s
+00000570: 7472 3a0a 2020 2020 6d61 635f 7061 7274  tr:.    mac_part
+00000580: 7320 3d20 5b5d 0a20 2020 2066 6f72 2062  s = [].    for b
+00000590: 2069 6e20 6d61 633a 0a20 2020 2020 2020   in mac:.       
+000005a0: 2068 6578 203d 2066 277b 623a 787d 270a   hex = f'{b:x}'.
+000005b0: 2020 2020 2020 2020 6966 206c 656e 2868          if len(h
+000005c0: 6578 2920 3d3d 2031 3a0a 2020 2020 2020  ex) == 1:.      
+000005d0: 2020 2020 2020 6865 7820 3d20 2730 2720        hex = '0' 
+000005e0: 2b20 6865 780a 2020 2020 2020 2020 6d61  + hex.        ma
+000005f0: 635f 7061 7274 732e 6170 7065 6e64 2868  c_parts.append(h
+00000600: 6578 290a 2020 2020 7265 7475 726e 2027  ex).    return '
+00000610: 3a27 2e6a 6f69 6e28 6d61 635f 7061 7274  :'.join(mac_part
+00000620: 7329 0a0a 0a64 6566 2070 6172 7365 5f69  s)...def parse_i
+00000630: 7028 6970 3a20 6279 7465 7329 202d 3e20  p(ip: bytes) -> 
+00000640: 7374 723a 0a20 2020 2069 705f 7061 7274  str:.    ip_part
+00000650: 7320 3d20 5b5d 0a20 2020 2066 6f72 2062  s = [].    for b
+00000660: 2069 6e20 6970 3a0a 2020 2020 2020 2020   in ip:.        
+00000670: 6970 5f70 6172 7473 2e61 7070 656e 6428  ip_parts.append(
+00000680: 7374 7228 6229 290a 2020 2020 7265 7475  str(b)).    retu
+00000690: 726e 2027 2e27 2e6a 6f69 6e28 6970 5f70  rn '.'.join(ip_p
+000006a0: 6172 7473 290a                           arts).
```

### Comparing `aioarp-0.0.4/.ruff_cache/content/277c58fd0e92dc6f` & `aioarp-0.0.5/aioarp/_async.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,129 @@
-00000000: 0100 0000 0000 0000 0c00 0000 0000 0000  ................
-00000010: 6169 6f61 7270 2e5f 7379 6e63 0d00 0000  aioarp._sync....
-00000020: 0000 0000 0400 0000 0000 0000 7469 6d65  ............time
-00000030: 0000 0000 0b00 0000 0600 0000 0000 0000  ................
-00000040: 7479 7069 6e67 0c00 0000 1900 0000 1200  typing..........
-00000050: 0000 0000 0000 6169 6f61 7270 2e5f 6578  ......aioarp._ex
-00000060: 6365 7074 696f 6e73 2e00 0000 4000 0000  ceptions....@...
-00000070: 1b00 0000 0000 0000 6169 6f61 7270 2e5f  ........aioarp._
-00000080: 6172 702e 4152 505f 4845 4144 4552 5f53  arp.ARP_HEADER_S
-00000090: 495a 4559 0000 0068 0000 0020 0000 0000  IZEY...h... ....
-000000a0: 0000 0061 696f 6172 702e 5f61 7270 2e45  ...aioarp._arp.E
-000000b0: 5448 4552 4e45 545f 4845 4144 4552 5f53  THERNET_HEADER_S
-000000c0: 495a 456a 0000 007e 0000 0015 0000 0000  IZEj...~........
-000000d0: 0000 0061 696f 6172 702e 5f61 7270 2e41  ...aioarp._arp.A
-000000e0: 7270 5061 636b 6574 8000 0000 8900 0000  rpPacket........
-000000f0: 1500 0000 0000 0000 6169 6f61 7270 2e5f  ........aioarp._
-00000100: 6172 702e 4574 6850 6163 6b65 748b 0000  arp.EthPacket...
-00000110: 0094 0000 0014 0000 0000 0000 0061 696f  .............aio
-00000120: 6172 702e 5f61 7270 2e50 726f 746f 636f  arp._arp.Protoco
-00000130: 6c96 0000 009e 0000 001b 0000 0000 0000  l...............
-00000140: 0061 696f 6172 702e 5f75 7469 6c73 2e69  .aioarp._utils.i
-00000150: 735f 7661 6c69 645f 6970 7634 b900 0000  s_valid_ipv4....
-00000160: c600 0000 2400 0000 0000 0000 6169 6f61  ....$.......aioa
-00000170: 7270 2e64 6566 6175 6c74 732e 4445 4641  rp.defaults.DEFA
-00000180: 554c 545f 5245 4144 5f54 494d 454f 5554  ULT_READ_TIMEOUT
-00000190: e300 0000 f700 0000 2a00 0000 0000 0000  ........*.......
-000001a0: 6169 6f61 7270 2e64 6566 6175 6c74 732e  aioarp.defaults.
-000001b0: 4445 4641 554c 545f 5245 504c 595f 4d49  DEFAULT_REPLY_MI
-000001c0: 5353 494e 475f 5449 4d45 f900 0000 1301  SSING_TIME......
-000001d0: 0000 2500 0000 0000 0000 6169 6f61 7270  ..%.......aioarp
-000001e0: 2e64 6566 6175 6c74 732e 4445 4641 554c  .defaults.DEFAUL
-000001f0: 545f 5752 4954 455f 5449 4d45 4f55 5415  T_WRITE_TIMEOUT.
-00000200: 0100 002a 0100 001c 0000 0000 0000 0061  ...*...........a
-00000210: 696f 6172 702e 6261 636b 656e 6473 2e5f  ioarp.backends._
-00000220: 7379 6e63 2e53 7472 6561 6d47 0100 004d  sync.StreamG...M
-00000230: 0100 0001 0000 0000 0000 000f 0000 0000  ................
-00000240: 0000 0055 6e73 6f72 7465 6449 6d70 6f72  ...UnsortedImpor
-00000250: 7473 2900 0000 0000 0000 496d 706f 7274  ts).......Import
-00000260: 2062 6c6f 636b 2069 7320 756e 2d73 6f72   block is un-sor
-00000270: 7465 6420 6f72 2075 6e2d 666f 726d 6174  ted or un-format
-00000280: 7465 6401 1000 0000 0000 0000 4f72 6761  ted.........Orga
-00000290: 6e69 7a65 2069 6d70 6f72 7473 0000 0000  nize imports....
-000002a0: 4f01 0000 0101 0000 0000 0000 0000 0000  O...............
-000002b0: 004f 0100 0001 5001 0000 0000 0000 696d  .O....P.......im
-000002c0: 706f 7274 2074 696d 650a 696d 706f 7274  port time.import
-000002d0: 2074 7970 696e 670a 0a66 726f 6d20 6169   typing..from ai
-000002e0: 6f61 7270 2069 6d70 6f72 7420 5f65 7863  oarp import _exc
-000002f0: 6570 7469 6f6e 7320 6173 2065 7863 0a66  eptions as exc.f
-00000300: 726f 6d20 6169 6f61 7270 2e5f 6172 7020  rom aioarp._arp 
-00000310: 696d 706f 7274 2041 5250 5f48 4541 4445  import ARP_HEADE
-00000320: 525f 5349 5a45 2c20 4554 4845 524e 4554  R_SIZE, ETHERNET
-00000330: 5f48 4541 4445 525f 5349 5a45 2c20 4172  _HEADER_SIZE, Ar
-00000340: 7050 6163 6b65 742c 2045 7468 5061 636b  pPacket, EthPack
-00000350: 6574 2c20 5072 6f74 6f63 6f6c 0a66 726f  et, Protocol.fro
-00000360: 6d20 6169 6f61 7270 2e5f 7574 696c 7320  m aioarp._utils 
-00000370: 696d 706f 7274 2069 735f 7661 6c69 645f  import is_valid_
-00000380: 6970 7634 0a66 726f 6d20 6169 6f61 7270  ipv4.from aioarp
-00000390: 2e64 6566 6175 6c74 7320 696d 706f 7274  .defaults import
-000003a0: 2044 4546 4155 4c54 5f52 4541 445f 5449   DEFAULT_READ_TI
-000003b0: 4d45 4f55 542c 2044 4546 4155 4c54 5f52  MEOUT, DEFAULT_R
-000003c0: 4550 4c59 5f4d 4953 5349 4e47 5f54 494d  EPLY_MISSING_TIM
-000003d0: 452c 2044 4546 4155 4c54 5f57 5249 5445  E, DEFAULT_WRITE
-000003e0: 5f54 494d 454f 5554 0a0a 6672 6f6d 202e  _TIMEOUT..from .
-000003f0: 6261 636b 656e 6473 2e5f 7379 6e63 2069  backends._sync i
-00000400: 6d70 6f72 7420 5374 7265 616d 0a0a 0300  mport Stream....
-00000410: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000420: 0000 0000 0000 2900 0000 0000 0000 2f68  ......)......./h
-00000430: 6f6d 652f 7465 7374 2f44 6573 6b74 6f70  ome/test/Desktop
-00000440: 2f61 696f 6172 702f 6169 6f61 7270 2f5f  /aioarp/aioarp/_
-00000450: 7379 6e63 2e70 79a1 0700 0000 0000 0069  sync.py........i
-00000460: 6d70 6f72 7420 7469 6d65 0a69 6d70 6f72  mport time.impor
-00000470: 7420 7479 7069 6e67 0a0a 6672 6f6d 2061  t typing..from a
-00000480: 696f 6172 7020 696d 706f 7274 205f 6578  ioarp import _ex
-00000490: 6365 7074 696f 6e73 2061 7320 6578 630a  ceptions as exc.
-000004a0: 6672 6f6d 2061 696f 6172 702e 5f61 7270  from aioarp._arp
-000004b0: 2069 6d70 6f72 7420 4152 505f 4845 4144   import ARP_HEAD
-000004c0: 4552 5f53 495a 452c 2045 5448 4552 4e45  ER_SIZE, ETHERNE
-000004d0: 545f 4845 4144 4552 5f53 495a 452c 2041  T_HEADER_SIZE, A
-000004e0: 7270 5061 636b 6574 2c20 4574 6850 6163  rpPacket, EthPac
-000004f0: 6b65 742c 2050 726f 746f 636f 6c0a 6672  ket, Protocol.fr
-00000500: 6f6d 2061 696f 6172 702e 5f75 7469 6c73  om aioarp._utils
-00000510: 2069 6d70 6f72 7420 6973 5f76 616c 6964   import is_valid
-00000520: 5f69 7076 340a 6672 6f6d 2061 696f 6172  _ipv4.from aioar
-00000530: 702e 6465 6661 756c 7473 2069 6d70 6f72  p.defaults impor
-00000540: 7420 4445 4641 554c 545f 5245 4144 5f54  t DEFAULT_READ_T
-00000550: 494d 454f 5554 2c20 4445 4641 554c 545f  IMEOUT, DEFAULT_
-00000560: 5245 504c 595f 4d49 5353 494e 475f 5449  REPLY_MISSING_TI
-00000570: 4d45 2c20 4445 4641 554c 545f 5752 4954  ME, DEFAULT_WRIT
-00000580: 455f 5449 4d45 4f55 540a 6672 6f6d 202e  E_TIMEOUT.from .
-00000590: 6261 636b 656e 6473 2e5f 7379 6e63 2069  backends._sync i
-000005a0: 6d70 6f72 7420 5374 7265 616d 0a0a 5f5f  mport Stream..__
-000005b0: 616c 6c5f 5f20 3d20 280a 2020 2020 2773  all__ = (.    's
-000005c0: 796e 635f 7365 6e64 5f61 7270 272c 0a29  ync_send_arp',.)
-000005d0: 0a0a 0a64 6566 2072 6563 6569 7665 5f61  ...def receive_a
-000005e0: 7270 2873 6f63 6b3a 2053 7472 6561 6d2c  rp(sock: Stream,
-000005f0: 2074 696d 656f 7574 3a20 666c 6f61 7429   timeout: float)
-00000600: 202d 3e20 4172 7050 6163 6b65 743a 0a20   -> ArpPacket:. 
-00000610: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
-00000620: 7469 6d65 2e74 696d 6528 290a 2020 2020  time.time().    
-00000630: 7768 696c 6520 5472 7565 3a0a 0a20 2020  while True:..   
-00000640: 2020 2020 2023 2043 6865 636b 2069 6620       # Check if 
-00000650: 7469 6d65 6f75 7420 7761 7320 6578 7069  timeout was expi
-00000660: 7265 640a 2020 2020 2020 2020 6966 2074  red.        if t
-00000670: 696d 652e 7469 6d65 2829 202d 2073 7461  ime.time() - sta
-00000680: 7274 5f74 696d 6520 3e20 7469 6d65 6f75  rt_time > timeou
-00000690: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-000006a0: 6169 7365 2065 7863 2e4e 6f74 466f 756e  aise exc.NotFoun
-000006b0: 6445 7272 6f72 2829 0a0a 2020 2020 2020  dError()..      
-000006c0: 2020 2320 5472 7920 746f 2072 6561 6420    # Try to read 
-000006d0: 6672 616d 650a 2020 2020 2020 2020 7472  frame.        tr
-000006e0: 793a 0a20 2020 2020 2020 2020 2020 2066  y:.            f
-000006f0: 7261 6d65 203d 2073 6f63 6b2e 7265 6365  rame = sock.rece
-00000700: 6976 655f 6672 616d 6528 7469 6d65 6f75  ive_frame(timeou
-00000710: 743d 4445 4641 554c 545f 5245 4144 5f54  t=DEFAULT_READ_T
-00000720: 494d 454f 5554 290a 2020 2020 2020 2020  IMEOUT).        
-00000730: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00000740: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00000750: 2020 2072 6169 7365 2065 7863 2e4e 6f74     raise exc.Not
-00000760: 466f 756e 6445 7272 6f72 2829 2066 726f  FoundError() fro
-00000770: 6d20 650a 0a20 2020 2020 2020 2023 2045  m e..        # E
-00000780: 7874 7261 6374 2074 6865 2065 7468 6572  xtract the ether
-00000790: 6e65 7420 6865 6164 6572 0a20 2020 2020  net header.     
-000007a0: 2020 2065 7468 5f68 6561 6465 7220 3d20     eth_header = 
-000007b0: 6672 616d 655b 3a45 5448 4552 4e45 545f  frame[:ETHERNET_
-000007c0: 4845 4144 4552 5f53 495a 455d 0a0a 2020  HEADER_SIZE]..  
-000007d0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000007e0: 2020 2020 2020 2065 7468 5f70 6163 6b65         eth_packe
-000007f0: 7420 3d20 4574 6850 6163 6b65 742e 7061  t = EthPacket.pa
-00000800: 7273 6528 6574 685f 6865 6164 6572 290a  rse(eth_header).
-00000810: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-00000820: 7468 5f70 6163 6b65 742e 7072 6f74 6f20  th_packet.proto 
-00000830: 213d 2050 726f 746f 636f 6c2e 6172 703a  != Protocol.arp:
-00000840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000850: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
-00000860: 2020 2020 2020 2061 7270 5f72 6573 706f         arp_respo
-00000870: 6e73 6520 3d20 4172 7050 6163 6b65 742e  nse = ArpPacket.
-00000880: 7061 7273 6528 0a20 2020 2020 2020 2020  parse(.         
-00000890: 2020 2020 2020 2066 7261 6d65 5b45 5448         frame[ETH
-000008a0: 4552 4e45 545f 4845 4144 4552 5f53 495a  ERNET_HEADER_SIZ
-000008b0: 453a 2045 5448 4552 4e45 545f 4845 4144  E: ETHERNET_HEAD
-000008c0: 4552 5f53 495a 4520 2b20 4152 505f 4845  ER_SIZE + ARP_HE
-000008d0: 4144 4552 5f53 495a 455d 290a 2020 2020  ADER_SIZE]).    
-000008e0: 2020 2020 2020 2020 6966 2069 735f 7661          if is_va
-000008f0: 6c69 645f 6970 7634 2861 7270 5f72 6573  lid_ipv4(arp_res
-00000900: 706f 6e73 652e 7365 6e64 6572 5f69 7029  ponse.sender_ip)
-00000910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000920: 2020 7265 7475 726e 2061 7270 5f72 6573    return arp_res
-00000930: 706f 6e73 650a 2020 2020 2020 2020 6578  ponse.        ex
-00000940: 6365 7074 2042 6173 6545 7863 6570 7469  cept BaseExcepti
-00000950: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00000960: 2320 544f 444f 3a20 6361 7463 6820 636f  # TODO: catch co
-00000970: 6e63 7265 7465 2065 7272 6f72 730a 2020  ncrete errors.  
-00000980: 2020 2020 2020 2020 2020 2e2e 2e0a 0a0a            ......
-00000990: 6465 6620 7379 6e63 5f73 656e 645f 6172  def sync_send_ar
-000009a0: 7028 6172 705f 7061 636b 6574 3a20 4172  p(arp_packet: Ar
-000009b0: 7050 6163 6b65 742c 0a20 2020 2020 2020  pPacket,.       
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2020 7374 7265 616d 3a20 5374 7265 616d    stream: Stream
-000009e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000009f0: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
-00000a00: 7574 3a20 7479 7069 6e67 2e4f 7074 696f  ut: typing.Optio
-00000a10: 6e61 6c5b 666c 6f61 745d 203d 204e 6f6e  nal[float] = Non
-00000a20: 6529 202d 3e20 4172 7050 6163 6b65 743a  e) -> ArpPacket:
-00000a30: 0a20 2020 2065 7468 6572 6e65 745f 7061  .    ethernet_pa
-00000a40: 636b 6574 203d 2045 7468 5061 636b 6574  cket = EthPacket
-00000a50: 280a 2020 2020 2020 2020 7461 7267 6574  (.        target
-00000a60: 5f6d 6163 3d61 7270 5f70 6163 6b65 742e  _mac=arp_packet.
-00000a70: 7461 7267 6574 5f6d 6163 2c0a 2020 2020  target_mac,.    
-00000a80: 2020 2020 7365 6e64 6572 5f6d 6163 3d61      sender_mac=a
-00000a90: 7270 5f70 6163 6b65 742e 7365 6e64 6572  rp_packet.sender
-00000aa0: 5f6d 6163 2c0a 2020 2020 2020 2020 7072  _mac,.        pr
-00000ab0: 6f74 6f3d 5072 6f74 6f63 6f6c 2e61 7270  oto=Protocol.arp
-00000ac0: 0a20 2020 2029 0a0a 2020 2020 7472 793a  .    )..    try:
-00000ad0: 0a20 2020 2020 2020 2066 7261 6d65 5f74  .        frame_t
-00000ae0: 6f5f 7365 6e64 203d 2065 7468 6572 6e65  o_send = etherne
-00000af0: 745f 7061 636b 6574 2e62 7569 6c64 5f66  t_packet.build_f
-00000b00: 7261 6d65 2829 202b 2061 7270 5f70 6163  rame() + arp_pac
-00000b10: 6b65 742e 6275 696c 645f 6672 616d 6528  ket.build_frame(
-00000b20: 290a 2020 2020 2020 2020 7374 7265 616d  ).        stream
-00000b30: 2e77 7269 7465 5f66 7261 6d65 2866 7261  .write_frame(fra
-00000b40: 6d65 5f74 6f5f 7365 6e64 2c20 7469 6d65  me_to_send, time
-00000b50: 6f75 743d 4445 4641 554c 545f 5752 4954  out=DEFAULT_WRIT
-00000b60: 455f 5449 4d45 4f55 5429 0a20 2020 2065  E_TIMEOUT).    e
-00000b70: 7863 6570 7420 6578 632e 5772 6974 6554  xcept exc.WriteT
-00000b80: 696d 656f 7574 4572 726f 7220 6173 2065  imeoutError as e
-00000b90: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00000ba0: 6578 632e 4e6f 7446 6f75 6e64 4572 726f  exc.NotFoundErro
-00000bb0: 7220 6672 6f6d 2065 0a0a 2020 2020 7265  r from e..    re
-00000bc0: 7475 726e 2072 6563 6569 7665 5f61 7270  turn receive_arp
-00000bd0: 2873 7472 6561 6d2c 2074 696d 656f 7574  (stream, timeout
-00000be0: 206f 7220 4445 4641 554c 545f 5245 504c   or DEFAULT_REPL
-00000bf0: 595f 4d49 5353 494e 475f 5449 4d45 290a  Y_MISSING_TIME).
+00000000: 696d 706f 7274 2074 696d 650a 696d 706f  import time.impo
+00000010: 7274 2074 7970 696e 670a 0a66 726f 6d20  rt typing..from 
+00000020: 6169 6f61 7270 2069 6d70 6f72 7420 5f65  aioarp import _e
+00000030: 7863 6570 7469 6f6e 7320 6173 2065 7863  xceptions as exc
+00000040: 0a66 726f 6d20 6169 6f61 7270 2e5f 6172  .from aioarp._ar
+00000050: 7020 696d 706f 7274 2041 5250 5f48 4541  p import ARP_HEA
+00000060: 4445 525f 5349 5a45 2c20 4554 4845 524e  DER_SIZE, ETHERN
+00000070: 4554 5f48 4541 4445 525f 5349 5a45 2c20  ET_HEADER_SIZE, 
+00000080: 4172 7050 6163 6b65 742c 2045 7468 5061  ArpPacket, EthPa
+00000090: 636b 6574 2c20 5072 6f74 6f63 6f6c 0a66  cket, Protocol.f
+000000a0: 726f 6d20 6169 6f61 7270 2e5f 7574 696c  rom aioarp._util
+000000b0: 7320 696d 706f 7274 2069 735f 7661 6c69  s import is_vali
+000000c0: 645f 6970 7634 0a66 726f 6d20 6169 6f61  d_ipv4.from aioa
+000000d0: 7270 2e64 6566 6175 6c74 7320 696d 706f  rp.defaults impo
+000000e0: 7274 2044 4546 4155 4c54 5f52 4541 445f  rt DEFAULT_READ_
+000000f0: 5449 4d45 4f55 542c 2044 4546 4155 4c54  TIMEOUT, DEFAULT
+00000100: 5f52 4550 4c59 5f4d 4953 5349 4e47 5f54  _REPLY_MISSING_T
+00000110: 494d 452c 2044 4546 4155 4c54 5f57 5249  IME, DEFAULT_WRI
+00000120: 5445 5f54 494d 454f 5554 0a0a 6672 6f6d  TE_TIMEOUT..from
+00000130: 202e 5f62 6163 6b65 6e64 732e 5f61 7379   ._backends._asy
+00000140: 6e63 2069 6d70 6f72 7420 4173 796e 6353  nc import AsyncS
+00000150: 7472 6561 6d0a 0a5f 5f61 6c6c 5f5f 203d  tream..__all__ =
+00000160: 2028 0a20 2020 2027 6173 796e 635f 7365   (.    'async_se
+00000170: 6e64 5f61 7270 272c 0a29 0a0a 0a61 7379  nd_arp',.)...asy
+00000180: 6e63 2064 6566 2072 6563 6569 7665 5f61  nc def receive_a
+00000190: 7270 2873 6f63 6b3a 2041 7379 6e63 5374  rp(sock: AsyncSt
+000001a0: 7265 616d 2c20 7469 6d65 6f75 743a 2066  ream, timeout: f
+000001b0: 6c6f 6174 2920 2d3e 2041 7270 5061 636b  loat) -> ArpPack
+000001c0: 6574 3a0a 2020 2020 7374 6172 745f 7469  et:.    start_ti
+000001d0: 6d65 203d 2074 696d 652e 7469 6d65 2829  me = time.time()
+000001e0: 0a20 2020 2077 6869 6c65 2054 7275 653a  .    while True:
+000001f0: 0a0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
+00000200: 6b20 6966 2074 696d 656f 7574 2077 6173  k if timeout was
+00000210: 2065 7870 6972 6564 0a20 2020 2020 2020   expired.       
+00000220: 2069 6620 7469 6d65 2e74 696d 6528 2920   if time.time() 
+00000230: 2d20 7374 6172 745f 7469 6d65 203e 2074  - start_time > t
+00000240: 696d 656f 7574 3a0a 2020 2020 2020 2020  imeout:.        
+00000250: 2020 2020 7261 6973 6520 6578 632e 4e6f      raise exc.No
+00000260: 7446 6f75 6e64 4572 726f 7228 290a 0a20  tFoundError().. 
+00000270: 2020 2020 2020 2023 2054 7279 2074 6f20         # Try to 
+00000280: 7265 6164 2066 7261 6d65 0a20 2020 2020  read frame.     
+00000290: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000002a0: 2020 2020 6672 616d 6520 3d20 6177 6169      frame = awai
+000002b0: 7420 736f 636b 2e72 6563 6569 7665 5f66  t sock.receive_f
+000002c0: 7261 6d65 2874 696d 656f 7574 3d44 4546  rame(timeout=DEF
+000002d0: 4155 4c54 5f52 4541 445f 5449 4d45 4f55  AULT_READ_TIMEOU
+000002e0: 5429 0a20 2020 2020 2020 2065 7863 6570  T).        excep
+000002f0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00000300: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+00000310: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+00000320: 2020 7261 6973 6520 6578 632e 4e6f 7446    raise exc.NotF
+00000330: 6f75 6e64 4572 726f 7228 2920 6672 6f6d  oundError() from
+00000340: 2065 0a0a 2020 2020 2020 2020 2320 4578   e..        # Ex
+00000350: 7472 6163 7420 7468 6520 6574 6865 726e  tract the ethern
+00000360: 6574 2068 6561 6465 720a 2020 2020 2020  et header.      
+00000370: 2020 6574 685f 6865 6164 6572 203d 2066    eth_header = f
+00000380: 7261 6d65 5b3a 4554 4845 524e 4554 5f48  rame[:ETHERNET_H
+00000390: 4541 4445 525f 5349 5a45 5d0a 0a20 2020  EADER_SIZE]..   
+000003a0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000003b0: 2020 2020 2020 6574 685f 7061 636b 6574        eth_packet
+000003c0: 203d 2045 7468 5061 636b 6574 2e70 6172   = EthPacket.par
+000003d0: 7365 2865 7468 5f68 6561 6465 7229 0a20  se(eth_header). 
+000003e0: 2020 2020 2020 2020 2020 2069 6620 6574             if et
+000003f0: 685f 7061 636b 6574 2e70 726f 746f 2021  h_packet.proto !
+00000400: 3d20 5072 6f74 6f63 6f6c 2e61 7270 3a0a  = Protocol.arp:.
+00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000420: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
+00000430: 2020 2020 2020 6172 705f 7265 7370 6f6e        arp_respon
+00000440: 7365 203d 2041 7270 5061 636b 6574 2e70  se = ArpPacket.p
+00000450: 6172 7365 280a 2020 2020 2020 2020 2020  arse(.          
+00000460: 2020 2020 2020 6672 616d 655b 4554 4845        frame[ETHE
+00000470: 524e 4554 5f48 4541 4445 525f 5349 5a45  RNET_HEADER_SIZE
+00000480: 3a20 4554 4845 524e 4554 5f48 4541 4445  : ETHERNET_HEADE
+00000490: 525f 5349 5a45 202b 2041 5250 5f48 4541  R_SIZE + ARP_HEA
+000004a0: 4445 525f 5349 5a45 5d29 0a20 2020 2020  DER_SIZE]).     
+000004b0: 2020 2020 2020 2069 6620 6973 5f76 616c         if is_val
+000004c0: 6964 5f69 7076 3428 6172 705f 7265 7370  id_ipv4(arp_resp
+000004d0: 6f6e 7365 2e73 656e 6465 725f 6970 293a  onse.sender_ip):
+000004e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004f0: 2072 6574 7572 6e20 6172 705f 7265 7370   return arp_resp
+00000500: 6f6e 7365 0a20 2020 2020 2020 2065 7863  onse.        exc
+00000510: 6570 7420 4261 7365 4578 6365 7074 696f  ept BaseExceptio
+00000520: 6e3a 2020 2320 7072 6167 6d61 3a20 6e6f  n:  # pragma: no
+00000530: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
+00000540: 2020 2023 2054 4f44 4f3a 2063 6174 6368     # TODO: catch
+00000550: 2063 6f6e 6372 6574 6520 6572 726f 7273   concrete errors
+00000560: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00000570: 0a0a 0a61 7379 6e63 2064 6566 2061 7379  ...async def asy
+00000580: 6e63 5f73 656e 645f 6172 7028 6172 705f  nc_send_arp(arp_
+00000590: 7061 636b 6574 3a20 4172 7050 6163 6b65  packet: ArpPacke
+000005a0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+000005b0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+000005c0: 616d 3a20 4173 796e 6353 7472 6561 6d2c  am: AsyncStream,
+000005d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000005e0: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
+000005f0: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
+00000600: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
+00000610: 2920 2d3e 2041 7270 5061 636b 6574 3a0a  ) -> ArpPacket:.
+00000620: 2020 2020 6574 6865 726e 6574 5f70 6163      ethernet_pac
+00000630: 6b65 7420 3d20 4574 6850 6163 6b65 7428  ket = EthPacket(
+00000640: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
+00000650: 6d61 633d 6172 705f 7061 636b 6574 2e74  mac=arp_packet.t
+00000660: 6172 6765 745f 6d61 632c 0a20 2020 2020  arget_mac,.     
+00000670: 2020 2073 656e 6465 725f 6d61 633d 6172     sender_mac=ar
+00000680: 705f 7061 636b 6574 2e73 656e 6465 725f  p_packet.sender_
+00000690: 6d61 632c 0a20 2020 2020 2020 2070 726f  mac,.        pro
+000006a0: 746f 3d50 726f 746f 636f 6c2e 6172 700a  to=Protocol.arp.
+000006b0: 2020 2020 290a 0a20 2020 2074 7279 3a0a      )..    try:.
+000006c0: 2020 2020 2020 2020 6672 616d 655f 746f          frame_to
+000006d0: 5f73 656e 6420 3d20 6574 6865 726e 6574  _send = ethernet
+000006e0: 5f70 6163 6b65 742e 6275 696c 645f 6672  _packet.build_fr
+000006f0: 616d 6528 2920 2b20 6172 705f 7061 636b  ame() + arp_pack
+00000700: 6574 2e62 7569 6c64 5f66 7261 6d65 2829  et.build_frame()
+00000710: 0a20 2020 2020 2020 2061 7761 6974 2073  .        await s
+00000720: 7472 6561 6d2e 7772 6974 655f 6672 616d  tream.write_fram
+00000730: 6528 6672 616d 655f 746f 5f73 656e 642c  e(frame_to_send,
+00000740: 2074 696d 656f 7574 3d44 4546 4155 4c54   timeout=DEFAULT
+00000750: 5f57 5249 5445 5f54 494d 454f 5554 290a  _WRITE_TIMEOUT).
+00000760: 2020 2020 6578 6365 7074 2065 7863 2e57      except exc.W
+00000770: 7269 7465 5469 6d65 6f75 7445 7272 6f72  riteTimeoutError
+00000780: 2061 7320 653a 2020 2320 7072 6167 6d61   as e:  # pragma
+00000790: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
+000007a0: 2020 2072 6169 7365 2065 7863 2e4e 6f74     raise exc.Not
+000007b0: 466f 756e 6445 7272 6f72 2066 726f 6d20  FoundError from 
+000007c0: 650a 0a20 2020 2072 6574 7572 6e20 6177  e..    return aw
+000007d0: 6169 7420 7265 6365 6976 655f 6172 7028  ait receive_arp(
+000007e0: 7374 7265 616d 2c20 7469 6d65 6f75 7420  stream, timeout 
+000007f0: 6f72 2044 4546 4155 4c54 5f52 4550 4c59  or DEFAULT_REPLY
+00000800: 5f4d 4953 5349 4e47 5f54 494d 4529 0a    _MISSING_TIME).
```

### Comparing `aioarp-0.0.4/.ruff_cache/content/2b74d3f1efd79c7b` & `aioarp-0.0.5/aioarp/_backends/_sync.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,78 @@
-00000000: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-00000010: 0f00 0000 0000 0000 556e 736f 7274 6564  ........Unsorted
-00000020: 496d 706f 7274 7329 0000 0000 0000 0049  Imports).......I
-00000030: 6d70 6f72 7420 626c 6f63 6b20 6973 2075  mport block is u
-00000040: 6e2d 736f 7274 6564 206f 7220 756e 2d66  n-sorted or un-f
-00000050: 6f72 6d61 7474 6564 0110 0000 0000 0000  ormatted........
-00000060: 004f 7267 616e 697a 6520 696d 706f 7274  .Organize import
-00000070: 7300 0000 0045 0000 0001 0100 0000 0000  s....E..........
-00000080: 0000 0000 0000 4500 0000 0144 0000 0000  ......E....D....
-00000090: 0000 0069 6d70 6f72 7420 736f 636b 6574  ...import socket
-000000a0: 0a69 6d70 6f72 7420 7479 7069 6e67 0a0a  .import typing..
-000000b0: 6672 6f6d 2061 696f 6172 7020 696d 706f  from aioarp impo
-000000c0: 7274 205f 6578 6365 7074 696f 6e73 2061  rt _exceptions a
-000000d0: 7320 6578 630a 0a03 0000 0000 0000 0000  s exc...........
-000000e0: 0000 0000 0000 0001 0000 0000 0000 0032  ...............2
-000000f0: 0000 0000 0000 002f 686f 6d65 2f74 6573  ......./home/tes
-00000100: 742f 4465 736b 746f 702f 6169 6f61 7270  t/Desktop/aioarp
-00000110: 2f61 696f 6172 702f 6261 636b 656e 6473  /aioarp/backends
-00000120: 2f5f 7379 6e63 2e70 79bf 0300 0000 0000  /_sync.py.......
-00000130: 0069 6d70 6f72 7420 736f 636b 6574 0a69  .import socket.i
-00000140: 6d70 6f72 7420 7479 7069 6e67 0a0a 6672  mport typing..fr
-00000150: 6f6d 2061 696f 6172 7020 696d 706f 7274  om aioarp import
-00000160: 205f 6578 6365 7074 696f 6e73 2061 7320   _exceptions as 
-00000170: 6578 630a 0a0a 2320 544f 444f 3a20 6164  exc...# TODO: ad
-00000180: 6420 6572 726f 7220 6d61 700a 0a63 6c61  d error map..cla
-00000190: 7373 2053 6f63 6b65 743a 0a0a 2020 2020  ss Socket:..    
-000001a0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-000001b0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-000001c0: 2020 2020 696e 7465 7266 6163 653a 2073      interface: s
-000001d0: 7472 293a 0a20 2020 2020 2020 2073 6f63  tr):.        soc
-000001e0: 6b20 3d20 736f 636b 6574 2e73 6f63 6b65  k = socket.socke
-000001f0: 7428 736f 636b 6574 2e50 465f 5041 434b  t(socket.PF_PACK
-00000200: 4554 2c20 736f 636b 6574 2e53 4f43 4b5f  ET, socket.SOCK_
-00000210: 5241 572c 2073 6f63 6b65 742e 6e74 6f68  RAW, socket.ntoh
-00000220: 7328 3078 3030 3033 2929 0a20 2020 2020  s(0x0003)).     
-00000230: 2020 2073 6f63 6b2e 6269 6e64 2828 696e     sock.bind((in
-00000240: 7465 7266 6163 652c 2030 2929 0a20 2020  terface, 0)).   
-00000250: 2020 2020 2073 656c 662e 736f 636b 203d       self.sock =
-00000260: 2073 6f63 6b0a 0a20 2020 2064 6566 2072   sock..    def r
-00000270: 6563 6569 7665 5f66 7261 6d65 2873 656c  eceive_frame(sel
-00000280: 662c 2074 696d 656f 7574 3a20 666c 6f61  f, timeout: floa
-00000290: 7429 202d 3e20 6279 7465 733a 0a20 2020  t) -> bytes:.   
-000002a0: 2020 2020 2073 656c 662e 736f 636b 2e73       self.sock.s
-000002b0: 6574 7469 6d65 6f75 7428 7469 6d65 6f75  ettimeout(timeou
-000002c0: 7429 0a20 2020 2020 2020 2074 7279 3a0a  t).        try:.
-000002d0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-000002e0: 6520 3d20 7365 6c66 2e73 6f63 6b2e 7265  e = self.sock.re
-000002f0: 6376 2831 3132 3331 3233 290a 2020 2020  cv(1123123).    
-00000300: 2020 2020 6578 6365 7074 2073 6f63 6b65      except socke
-00000310: 742e 7469 6d65 6f75 743a 0a20 2020 2020  t.timeout:.     
-00000320: 2020 2020 2020 2072 6169 7365 2065 7863         raise exc
-00000330: 2e52 6561 6454 696d 656f 7574 4572 726f  .ReadTimeoutErro
-00000340: 7228 290a 2020 2020 2020 2020 7265 7475  r().        retu
-00000350: 726e 2066 7261 6d65 0a0a 2020 2020 6465  rn frame..    de
-00000360: 6620 7772 6974 655f 6672 616d 6528 7365  f write_frame(se
-00000370: 6c66 2c20 6672 616d 653a 2062 7974 6573  lf, frame: bytes
-00000380: 2c20 7469 6d65 6f75 743a 2066 6c6f 6174  , timeout: float
-00000390: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000003a0: 2020 2073 656c 662e 736f 636b 2e73 6574     self.sock.set
-000003b0: 7469 6d65 6f75 7428 7469 6d65 6f75 7429  timeout(timeout)
-000003c0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-000003d0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000003e0: 6f63 6b2e 7365 6e64 616c 6c28 6672 616d  ock.sendall(fram
-000003f0: 6529 0a20 2020 2020 2020 2065 7863 6570  e).        excep
-00000400: 7420 736f 636b 6574 2e74 696d 656f 7574  t socket.timeout
-00000410: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00000420: 6973 6520 6578 632e 5772 6974 6554 696d  ise exc.WriteTim
-00000430: 656f 7574 4572 726f 7228 290a 0a20 2020  eoutError()..   
-00000440: 2064 6566 205f 5f65 6e74 6572 5f5f 2873   def __enter__(s
-00000450: 656c 6629 202d 3e20 2753 6f63 6b65 7427  elf) -> 'Socket'
-00000460: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00000470: 2073 656c 660a 0a20 2020 2064 6566 205f   self..    def _
-00000480: 5f65 7869 745f 5f28 7365 6c66 2c20 6578  _exit__(self, ex
-00000490: 635f 7479 7065 3a20 7479 7069 6e67 2e41  c_type: typing.A
-000004a0: 6e79 2c20 6578 635f 7661 6c3a 2074 7970  ny, exc_val: typ
-000004b0: 696e 672e 416e 792c 2065 7863 5f74 623a  ing.Any, exc_tb:
-000004c0: 2074 7970 696e 672e 416e 7929 202d 3e20   typing.Any) -> 
-000004d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
-000004e0: 6c66 2e73 6f63 6b2e 636c 6f73 6528 290a  lf.sock.close().
+00000000: 696d 706f 7274 2073 6f63 6b65 740a 696d  import socket.im
+00000010: 706f 7274 2074 7970 696e 670a 0a66 726f  port typing..fro
+00000020: 6d20 6169 6f61 7270 2069 6d70 6f72 7420  m aioarp import 
+00000030: 5f65 7863 6570 7469 6f6e 7320 6173 2065  _exceptions as e
+00000040: 7863 0a66 726f 6d20 6169 6f61 7270 2e5f  xc.from aioarp._
+00000050: 6261 636b 656e 6473 2e5f 6261 7365 2069  backends._base i
+00000060: 6d70 6f72 7420 536f 636b 6574 496e 7465  mport SocketInte
+00000070: 7266 6163 650a 0a5f 5f61 6c6c 5f5f 203d  rface..__all__ =
+00000080: 2028 0a20 2020 2027 5374 7265 616d 272c   (.    'Stream',
+00000090: 0a29 0a63 6c61 7373 2053 7472 6561 6d3a  .).class Stream:
+000000a0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+000000b0: 5f5f 2873 656c 662c 0a20 2020 2020 2020  __(self,.       
+000000c0: 2020 2020 2020 2020 2020 696e 7465 7266            interf
+000000d0: 6163 653a 2073 7472 2c0a 2020 2020 2020  ace: str,.      
+000000e0: 2020 2020 2020 2020 2020 2073 6f63 6b3a             sock:
+000000f0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00000100: 5b53 6f63 6b65 7449 6e74 6572 6661 6365  [SocketInterface
+00000110: 5d20 3d20 4e6f 6e65 0a20 2020 2020 2020  ] = None.       
+00000120: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00000130: 2020 2020 2073 656c 662e 736f 636b 3a20       self.sock: 
+00000140: 536f 636b 6574 496e 7465 7266 6163 650a  SocketInterface.
+00000150: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00000160: 6f63 6b3a 2020 2320 7072 6167 6d61 3a20  ock:  # pragma: 
+00000170: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
+00000180: 2020 2020 2073 656c 662e 736f 636b 203d       self.sock =
+00000190: 2073 6f63 6b65 742e 736f 636b 6574 2873   socket.socket(s
+000001a0: 6f63 6b65 742e 5046 5f50 4143 4b45 542c  ocket.PF_PACKET,
+000001b0: 2073 6f63 6b65 742e 534f 434b 5f52 4157   socket.SOCK_RAW
+000001c0: 2c20 736f 636b 6574 2e6e 746f 6873 2830  , socket.ntohs(0
+000001d0: 7830 3030 3329 290a 2020 2020 2020 2020  x0003)).        
+000001e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000001f0: 2020 7365 6c66 2e73 6f63 6b20 3d20 736f    self.sock = so
+00000200: 636b 0a20 2020 2020 2020 2073 656c 662e  ck.        self.
+00000210: 736f 636b 2e62 696e 6428 2869 6e74 6572  sock.bind((inter
+00000220: 6661 6365 2c20 3029 290a 0a20 2020 2064  face, 0))..    d
+00000230: 6566 2072 6563 6569 7665 5f66 7261 6d65  ef receive_frame
+00000240: 2873 656c 662c 2074 696d 656f 7574 3a20  (self, timeout: 
+00000250: 666c 6f61 7429 202d 3e20 6279 7465 733a  float) -> bytes:
+00000260: 0a20 2020 2020 2020 2073 656c 662e 736f  .        self.so
+00000270: 636b 2e73 6574 7469 6d65 6f75 7428 7469  ck.settimeout(ti
+00000280: 6d65 6f75 7429 0a20 2020 2020 2020 2074  meout).        t
+00000290: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+000002a0: 6672 616d 6520 3d20 7365 6c66 2e73 6f63  frame = self.soc
+000002b0: 6b2e 7265 6376 2831 3132 3331 3233 290a  k.recv(1123123).
+000002c0: 2020 2020 2020 2020 6578 6365 7074 2073          except s
+000002d0: 6f63 6b65 742e 7469 6d65 6f75 743a 2020  ocket.timeout:  
+000002e0: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+000002f0: 6572 0a20 2020 2020 2020 2020 2020 2072  er.            r
+00000300: 6169 7365 2065 7863 2e52 6561 6454 696d  aise exc.ReadTim
+00000310: 656f 7574 4572 726f 7228 290a 2020 2020  eoutError().    
+00000320: 2020 2020 7265 7475 726e 2066 7261 6d65      return frame
+00000330: 0a0a 2020 2020 6465 6620 7772 6974 655f  ..    def write_
+00000340: 6672 616d 6528 7365 6c66 2c20 6672 616d  frame(self, fram
+00000350: 653a 2062 7974 6573 2c20 7469 6d65 6f75  e: bytes, timeou
+00000360: 743a 2066 6c6f 6174 2920 2d3e 204e 6f6e  t: float) -> Non
+00000370: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
+00000380: 736f 636b 2e73 6574 7469 6d65 6f75 7428  sock.settimeout(
+00000390: 7469 6d65 6f75 7429 0a20 2020 2020 2020  timeout).       
+000003a0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+000003b0: 2020 7365 6c66 2e73 6f63 6b2e 7365 6e64    self.sock.send
+000003c0: 616c 6c28 6672 616d 6529 0a20 2020 2020  all(frame).     
+000003d0: 2020 2065 7863 6570 7420 736f 636b 6574     except socket
+000003e0: 2e74 696d 656f 7574 3a20 2023 2070 7261  .timeout:  # pra
+000003f0: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+00000400: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00000410: 6578 632e 5772 6974 6554 696d 656f 7574  exc.WriteTimeout
+00000420: 4572 726f 7228 290a 0a20 2020 2064 6566  Error()..    def
+00000430: 205f 5f65 6e74 6572 5f5f 2873 656c 6629   __enter__(self)
+00000440: 202d 3e20 2753 7472 6561 6d27 3a0a 2020   -> 'Stream':.  
+00000450: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000460: 660a 0a20 2020 2064 6566 205f 5f65 7869  f..    def __exi
+00000470: 745f 5f28 7365 6c66 2c20 6578 635f 7479  t__(self, exc_ty
+00000480: 7065 3a20 7479 7069 6e67 2e41 6e79 2c20  pe: typing.Any, 
+00000490: 6578 635f 7661 6c3a 2074 7970 696e 672e  exc_val: typing.
+000004a0: 416e 792c 2065 7863 5f74 623a 2074 7970  Any, exc_tb: typ
+000004b0: 696e 672e 416e 7929 202d 3e20 4e6f 6e65  ing.Any) -> None
+000004c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e73  :.        self.s
+000004d0: 6f63 6b2e 636c 6f73 6528 290a            ock.close().
```

### Comparing `aioarp-0.0.4/.ruff_cache/content/64f9f289e0610564` & `aioarp-0.0.5/aioarp/_arp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,329 +1,297 @@
-00000000: 0100 0000 0000 0000 0b00 0000 0000 0000  ................
-00000010: 6169 6f61 7270 2e5f 6172 7007 0000 0000  aioarp._arp.....
-00000020: 0000 0006 0000 0000 0000 0073 7472 7563  ...........struc
-00000030: 7400 0000 000d 0000 0006 0000 0000 0000  t...............
-00000040: 0074 7970 696e 670e 0000 001b 0000 0009  .typing.........
-00000050: 0000 0000 0000 0065 6e75 6d2e 456e 756d  .......enum.Enum
-00000060: 2d00 0000 3100 0000 1700 0000 0000 0000  -...1...........
-00000070: 6169 6f61 7270 2e5f 7574 696c 732e 7061  aioarp._utils.pa
-00000080: 7273 655f 6d61 634d 0000 0056 0000 0019  rse_macM...V....
-00000090: 0000 0000 0000 0061 696f 6172 702e 5f75  .......aioarp._u
-000000a0: 7469 6c73 2e65 6e66 6f72 6365 5f6d 6163  tils.enforce_mac
-000000b0: 5800 0000 6300 0000 1600 0000 0000 0000  X...c...........
-000000c0: 6169 6f61 7270 2e5f 7574 696c 732e 7061  aioarp._utils.pa
-000000d0: 7273 655f 6970 6500 0000 6d00 0000 1800  rse_ipe...m.....
-000000e0: 0000 0000 0000 6169 6f61 7270 2e5f 7574  ......aioarp._ut
-000000f0: 696c 732e 656e 666f 7263 655f 6970 6f00  ils.enforce_ipo.
-00000100: 0000 7900 0000 0100 0000 0000 0000 0f00  ..y.............
-00000110: 0000 0000 0000 556e 736f 7274 6564 496d  ......UnsortedIm
-00000120: 706f 7274 7329 0000 0000 0000 0049 6d70  ports).......Imp
-00000130: 6f72 7420 626c 6f63 6b20 6973 2075 6e2d  ort block is un-
-00000140: 736f 7274 6564 206f 7220 756e 2d66 6f72  sorted or un-for
-00000150: 6d61 7474 6564 0110 0000 0000 0000 004f  matted.........O
-00000160: 7267 616e 697a 6520 696d 706f 7274 7300  rganize imports.
-00000170: 0000 007b 0000 0001 0100 0000 0000 0000  ...{............
-00000180: 0000 0000 7b00 0000 017b 0000 0000 0000  ....{....{......
-00000190: 0069 6d70 6f72 7420 7374 7275 6374 0a69  .import struct.i
-000001a0: 6d70 6f72 7420 7479 7069 6e67 0a66 726f  mport typing.fro
-000001b0: 6d20 656e 756d 2069 6d70 6f72 7420 456e  m enum import En
-000001c0: 756d 0a0a 6672 6f6d 2061 696f 6172 702e  um..from aioarp.
-000001d0: 5f75 7469 6c73 2069 6d70 6f72 7420 656e  _utils import en
-000001e0: 666f 7263 655f 6970 2c20 656e 666f 7263  force_ip, enforc
-000001f0: 655f 6d61 632c 2070 6172 7365 5f69 702c  e_mac, parse_ip,
-00000200: 2070 6172 7365 5f6d 6163 0a0a 0300 0000   parse_mac......
-00000210: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00000220: 0000 0000 2800 0000 0000 0000 2f68 6f6d  ....(......./hom
-00000230: 652f 7465 7374 2f44 6573 6b74 6f70 2f61  e/test/Desktop/a
-00000240: 696f 6172 702f 6169 6f61 7270 2f5f 6172  ioarp/aioarp/_ar
-00000250: 702e 7079 3312 0000 0000 0000 696d 706f  p.py3.......impo
-00000260: 7274 2073 7472 7563 740a 696d 706f 7274  rt struct.import
-00000270: 2074 7970 696e 670a 6672 6f6d 2065 6e75   typing.from enu
-00000280: 6d20 696d 706f 7274 2045 6e75 6d0a 0a66  m import Enum..f
-00000290: 726f 6d20 6169 6f61 7270 2e5f 7574 696c  rom aioarp._util
-000002a0: 7320 696d 706f 7274 2070 6172 7365 5f6d  s import parse_m
-000002b0: 6163 2c20 656e 666f 7263 655f 6d61 632c  ac, enforce_mac,
-000002c0: 2070 6172 7365 5f69 702c 2065 6e66 6f72   parse_ip, enfor
-000002d0: 6365 5f69 700a 0a45 5448 4552 4e45 545f  ce_ip..ETHERNET_
-000002e0: 4845 4144 4552 5f53 495a 4520 3d20 3134  HEADER_SIZE = 14
-000002f0: 0a41 5250 5f48 4541 4445 525f 5349 5a45  .ARP_HEADER_SIZE
-00000300: 203d 2032 380a 0a5f 5f61 6c6c 5f5f 203d   = 28..__all__ =
-00000310: 2028 0a20 2020 2027 4554 4845 524e 4554   (.    'ETHERNET
-00000320: 5f48 4541 4445 525f 5349 5a45 272c 0a20  _HEADER_SIZE',. 
-00000330: 2020 2027 4152 505f 4845 4144 4552 5f53     'ARP_HEADER_S
-00000340: 495a 4527 2c0a 2020 2020 2748 6172 6477  IZE',.    'Hardw
-00000350: 6172 6554 7970 6527 2c0a 2020 2020 2750  areType',.    'P
-00000360: 726f 746f 636f 6c27 2c0a 2020 2020 274f  rotocol',.    'O
-00000370: 7063 6f64 6527 2c0a 2020 2020 2745 7468  pcode',.    'Eth
-00000380: 5061 636b 6574 272c 0a20 2020 2027 4172  Packet',.    'Ar
-00000390: 7050 6163 6b65 7427 2c0a 2020 2020 2773  pPacket',.    's
-000003a0: 697a 655f 6f66 270a 290a 0a63 6c61 7373  ize_of'.)..class
-000003b0: 2048 6172 6477 6172 6554 7970 6528 456e   HardwareType(En
-000003c0: 756d 293a 0a20 2020 2065 7468 6572 6e65  um):.    etherne
-000003d0: 7420 3d20 310a 0a0a 636c 6173 7320 5072  t = 1...class Pr
-000003e0: 6f74 6f63 6f6c 2845 6e75 6d29 3a0a 2020  otocol(Enum):.  
-000003f0: 2020 6970 203d 2030 7830 3830 300a 2020    ip = 0x0800.  
-00000400: 2020 6172 7020 3d20 3078 3038 3036 0a0a    arp = 0x0806..
-00000410: 0a63 6c61 7373 204f 7063 6f64 6528 456e  .class Opcode(En
-00000420: 756d 293a 0a20 2020 2072 6571 7565 7374  um):.    request
-00000430: 203d 2031 0a20 2020 2072 6573 706f 6e73   = 1.    respons
-00000440: 6520 3d20 320a 0a0a 636c 6173 7320 4574  e = 2...class Et
-00000450: 6850 6163 6b65 743a 0a20 2020 2066 6f72  hPacket:.    for
-00000460: 6d61 7420 3d20 2221 3673 3673 4822 0a0a  mat = "!6s6sH"..
-00000470: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00000480: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00000490: 2020 2020 2020 2020 7461 7267 6574 5f6d          target_m
-000004a0: 6163 3a20 7374 722c 0a20 2020 2020 2020  ac: str,.       
-000004b0: 2020 2020 2020 2020 2020 7365 6e64 6572            sender
-000004c0: 5f6d 6163 3a20 7374 722c 0a20 2020 2020  _mac: str,.     
-000004d0: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-000004e0: 6f3a 2050 726f 746f 636f 6c29 3a0a 2020  o: Protocol):.  
-000004f0: 2020 2020 2020 7365 6c66 2e74 6172 6765        self.targe
-00000500: 745f 6d61 6320 3d20 7461 7267 6574 5f6d  t_mac = target_m
-00000510: 6163 0a20 2020 2020 2020 2073 656c 662e  ac.        self.
-00000520: 7365 6e64 6572 5f6d 6163 203d 2073 656e  sender_mac = sen
-00000530: 6465 725f 6d61 630a 2020 2020 2020 2020  der_mac.        
-00000540: 7365 6c66 2e70 726f 746f 203d 2070 726f  self.proto = pro
-00000550: 746f 0a0a 2020 2020 4063 6c61 7373 6d65  to..    @classme
-00000560: 7468 6f64 0a20 2020 2064 6566 2070 6172  thod.    def par
-00000570: 7365 2863 6c73 2c20 6672 616d 653a 2062  se(cls, frame: b
-00000580: 7974 6573 293a 0a20 2020 2020 2020 2074  ytes):.        t
-00000590: 6172 6765 745f 6d61 632c 2073 656e 6465  arget_mac, sende
-000005a0: 725f 6d61 632c 2070 726f 746f 203d 2073  r_mac, proto = s
-000005b0: 7472 7563 742e 756e 7061 636b 280a 2020  truct.unpack(.  
-000005c0: 2020 2020 2020 2020 2020 2721 3673 3673            '!6s6s
-000005d0: 4827 2c0a 2020 2020 2020 2020 2020 2020  H',.            
-000005e0: 6672 616d 650a 2020 2020 2020 2020 290a  frame.        ).
-000005f0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00000600: 6c73 280a 2020 2020 2020 2020 2020 2020  ls(.            
-00000610: 7461 7267 6574 5f6d 6163 3d70 6172 7365  target_mac=parse
-00000620: 5f6d 6163 2874 6172 6765 745f 6d61 6329  _mac(target_mac)
-00000630: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00000640: 6e64 6572 5f6d 6163 3d70 6172 7365 5f6d  nder_mac=parse_m
-00000650: 6163 2873 656e 6465 725f 6d61 6329 2c0a  ac(sender_mac),.
-00000660: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00000670: 6f3d 5072 6f74 6f63 6f6c 2870 726f 746f  o=Protocol(proto
-00000680: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-00000690: 2064 6566 2062 7569 6c64 5f66 7261 6d65   def build_frame
-000006a0: 2873 656c 6629 202d 3e20 6279 7465 733a  (self) -> bytes:
-000006b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000006c0: 7374 7275 6374 2e70 6163 6b28 0a20 2020  struct.pack(.   
-000006d0: 2020 2020 2020 2020 2073 656c 662e 666f           self.fo
-000006e0: 726d 6174 2c0a 2020 2020 2020 2020 2020  rmat,.          
-000006f0: 2020 656e 666f 7263 655f 6d61 6328 7365    enforce_mac(se
-00000700: 6c66 2e74 6172 6765 745f 6d61 6329 2c0a  lf.target_mac),.
-00000710: 2020 2020 2020 2020 2020 2020 656e 666f              enfo
-00000720: 7263 655f 6d61 6328 7365 6c66 2e73 656e  rce_mac(self.sen
-00000730: 6465 725f 6d61 6329 2c0a 2020 2020 2020  der_mac),.      
-00000740: 2020 2020 2020 7365 6c66 2e70 726f 746f        self.proto
-00000750: 2e76 616c 7565 0a20 2020 2020 2020 2029  .value.        )
-00000760: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
-00000770: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00000780: 2020 7265 7475 726e 2066 223c 4574 6850    return f"<EthP
-00000790: 6163 6b65 7420 7461 7267 6574 3d7b 7365  acket target={se
-000007a0: 6c66 2e74 6172 6765 745f 6d61 637d 2073  lf.target_mac} s
-000007b0: 6f75 7263 653d 7b73 656c 662e 7365 6e64  ource={self.send
-000007c0: 6572 5f6d 6163 7d20 7072 6f74 6f3d 7b73  er_mac} proto={s
-000007d0: 656c 662e 7072 6f74 6f2e 6e61 6d65 7d3e  elf.proto.name}>
-000007e0: 220a 0a0a 636c 6173 7320 4172 7050 6163  "...class ArpPac
-000007f0: 6b65 743a 0a0a 2020 2020 6465 6620 5f5f  ket:..    def __
-00000800: 696e 6974 5f5f 2873 656c 662c 0a20 2020  init__(self,.   
-00000810: 2020 2020 2020 2020 2020 2020 2020 6861                ha
-00000820: 7264 7761 7265 5f74 7970 653a 2048 6172  rdware_type: Har
-00000830: 6477 6172 6554 7970 652c 0a20 2020 2020  dwareType,.     
-00000840: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00000850: 6f63 6f6c 5f74 7970 653a 2050 726f 746f  ocol_type: Proto
-00000860: 636f 6c2c 0a20 2020 2020 2020 2020 2020  col,.           
-00000870: 2020 2020 2020 7365 6e64 6572 5f6d 6163        sender_mac
-00000880: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
-00000890: 2020 2020 2020 2020 7365 6e64 6572 5f69          sender_i
-000008a0: 703a 2073 7472 2c0a 2020 2020 2020 2020  p: str,.        
-000008b0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-000008c0: 6d61 633a 2073 7472 2c0a 2020 2020 2020  mac: str,.      
-000008d0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
-000008e0: 745f 6970 3a20 7374 722c 0a20 2020 2020  t_ip: str,.     
-000008f0: 2020 2020 2020 2020 2020 2020 6f70 636f              opco
-00000900: 6465 3a20 4f70 636f 6465 203d 204f 7063  de: Opcode = Opc
-00000910: 6f64 652e 7265 7175 6573 7429 3a0a 2020  ode.request):.  
-00000920: 2020 2020 2020 7365 6c66 2e68 6172 6477        self.hardw
-00000930: 6172 655f 7479 7065 203d 2068 6172 6477  are_type = hardw
-00000940: 6172 655f 7479 7065 0a20 2020 2020 2020  are_type.       
-00000950: 2073 656c 662e 7072 6f74 6f63 6f6c 5f74   self.protocol_t
-00000960: 7970 6520 3d20 7072 6f74 6f63 6f6c 5f74  ype = protocol_t
-00000970: 7970 650a 2020 2020 2020 2020 7365 6c66  ype.        self
-00000980: 2e6f 7063 6f64 6520 3d20 6f70 636f 6465  .opcode = opcode
-00000990: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-000009a0: 6e64 6572 5f6d 6163 203d 2073 656e 6465  nder_mac = sende
-000009b0: 725f 6d61 630a 2020 2020 2020 2020 7365  r_mac.        se
-000009c0: 6c66 2e73 656e 6465 725f 6970 203d 2073  lf.sender_ip = s
-000009d0: 656e 6465 725f 6970 0a20 2020 2020 2020  ender_ip.       
-000009e0: 2073 656c 662e 7461 7267 6574 5f6d 6163   self.target_mac
-000009f0: 203d 2074 6172 6765 745f 6d61 630a 2020   = target_mac.  
-00000a00: 2020 2020 2020 7365 6c66 2e74 6172 6765        self.targe
-00000a10: 745f 6970 203d 2074 6172 6765 745f 6970  t_ip = target_ip
-00000a20: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00000a30: 2020 2020 6465 6620 6861 7264 7761 7265      def hardware
-00000a40: 5f6c 656e 6774 6828 7365 6c66 2920 2d3e  _length(self) ->
-00000a50: 2069 6e74 3a0a 2020 2020 2020 2020 7265   int:.        re
-00000a60: 7475 726e 2073 697a 655f 6f66 2873 656c  turn size_of(sel
-00000a70: 662e 6861 7264 7761 7265 5f74 7970 6529  f.hardware_type)
-00000a80: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00000a90: 2020 2020 6465 6620 7072 6f74 6f63 6f6c      def protocol
-00000aa0: 5f6c 656e 6774 6828 7365 6c66 2920 2d3e  _length(self) ->
-00000ab0: 2069 6e74 3a0a 2020 2020 2020 2020 7265   int:.        re
-00000ac0: 7475 726e 2073 697a 655f 6f66 2873 656c  turn size_of(sel
-00000ad0: 662e 7072 6f74 6f63 6f6c 5f74 7970 6529  f.protocol_type)
-00000ae0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00000af0: 6f64 0a20 2020 2064 6566 2070 6172 7365  od.    def parse
-00000b00: 2863 6c73 2c20 6672 616d 653a 2062 7974  (cls, frame: byt
-00000b10: 6573 293a 0a20 2020 2020 2020 2068 6172  es):.        har
-00000b20: 6477 6172 655f 666f 726d 6174 203d 2027  dware_format = '
-00000b30: 3673 270a 2020 2020 2020 2020 7072 6f74  6s'.        prot
-00000b40: 6f63 6f6c 5f66 6f72 6d61 7420 3d20 2734  ocol_format = '4
-00000b50: 7327 0a20 2020 2020 2020 2070 6163 6b69  s'.        packi
-00000b60: 6e67 5f66 6f72 6d61 7420 3d20 2727 2e6a  ng_format = ''.j
-00000b70: 6f69 6e28 5b0a 2020 2020 2020 2020 2020  oin([.          
-00000b80: 2020 2221 220a 2020 2020 2020 2020 2020    "!".          
-00000b90: 2020 2248 222c 2020 2320 6861 7264 7761    "H",  # hardwa
-00000ba0: 7265 2074 7970 650a 2020 2020 2020 2020  re type.        
-00000bb0: 2020 2020 2248 222c 2020 2320 7072 6f74      "H",  # prot
-00000bc0: 6f63 6f6c 2074 7970 650a 2020 2020 2020  ocol type.      
-00000bd0: 2020 2020 2020 2742 272c 2020 2320 6861        'B',  # ha
-00000be0: 7264 7761 7265 5f6c 656e 6774 680a 2020  rdware_length.  
-00000bf0: 2020 2020 2020 2020 2020 2742 272c 2020            'B',  
-00000c00: 2320 7072 6f74 6f63 6f6c 5f6c 656e 6774  # protocol_lengt
-00000c10: 680a 2020 2020 2020 2020 2020 2020 2748  h.            'H
-00000c20: 272c 2020 2320 6f70 636f 6465 3a20 4f70  ',  # opcode: Op
-00000c30: 636f 6465 203d 204f 7063 6f64 652e 7265  code = Opcode.re
-00000c40: 7175 6573 740a 2020 2020 2020 2020 2020  quest.          
-00000c50: 2020 6861 7264 7761 7265 5f66 6f72 6d61    hardware_forma
-00000c60: 742c 2020 2320 7365 6e64 6572 5f6d 6163  t,  # sender_mac
-00000c70: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00000c80: 746f 636f 6c5f 666f 726d 6174 2c20 2023  tocol_format,  #
-00000c90: 2073 656e 6465 725f 6970 3a20 696e 740a   sender_ip: int.
-00000ca0: 2020 2020 2020 2020 2020 2020 6861 7264              hard
-00000cb0: 7761 7265 5f66 6f72 6d61 742c 2020 2320  ware_format,  # 
-00000cc0: 7461 7267 6574 5f6d 6170 3a20 696e 740a  target_map: int.
-00000cd0: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00000ce0: 6f63 6f6c 5f66 6f72 6d61 742c 2020 2320  ocol_format,  # 
-00000cf0: 7461 7267 6574 5f69 703a 2069 6e74 0a20  target_ip: int. 
-00000d00: 2020 2020 2020 205d 290a 0a20 2020 2020         ])..     
-00000d10: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-00000d20: 2068 6172 6477 6172 655f 7479 7065 2c0a   hardware_type,.
-00000d30: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00000d40: 6f63 6f6c 5f74 7970 652c 0a20 2020 2020  ocol_type,.     
-00000d50: 2020 2020 2020 2068 6172 6477 6172 655f         hardware_
-00000d60: 6c65 6e67 7468 2c0a 2020 2020 2020 2020  length,.        
-00000d70: 2020 2020 7072 6f74 6f63 6f6c 5f6c 656e      protocol_len
-00000d80: 6774 682c 0a20 2020 2020 2020 2020 2020  gth,.           
-00000d90: 206f 7063 6f64 652c 0a20 2020 2020 2020   opcode,.       
-00000da0: 2020 2020 2073 656e 6465 725f 6d61 632c       sender_mac,
-00000db0: 0a20 2020 2020 2020 2020 2020 2073 656e  .            sen
-00000dc0: 6465 725f 6970 2c0a 2020 2020 2020 2020  der_ip,.        
-00000dd0: 2020 2020 7461 7267 6574 5f6d 6163 2c0a      target_mac,.
-00000de0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00000df0: 6574 5f69 700a 2020 2020 2020 2020 2920  et_ip.        ) 
-00000e00: 3d20 7374 7275 6374 2e75 6e70 6163 6b28  = struct.unpack(
-00000e10: 0a20 2020 2020 2020 2020 2020 2070 6163  .            pac
-00000e20: 6b69 6e67 5f66 6f72 6d61 742c 0a20 2020  king_format,.   
-00000e30: 2020 2020 2020 2020 2066 7261 6d65 0a20           frame. 
-00000e40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00000e50: 2072 6574 7572 6e20 636c 7328 0a20 2020   return cls(.   
-00000e60: 2020 2020 2020 2020 2068 6172 6477 6172           hardwar
-00000e70: 655f 7479 7065 3d68 6172 6477 6172 655f  e_type=hardware_
-00000e80: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
-00000e90: 2020 7072 6f74 6f63 6f6c 5f74 7970 653d    protocol_type=
-00000ea0: 7072 6f74 6f63 6f6c 5f74 7970 652c 0a20  protocol_type,. 
-00000eb0: 2020 2020 2020 2020 2020 206f 7063 6f64             opcod
-00000ec0: 653d 4f70 636f 6465 286f 7063 6f64 6529  e=Opcode(opcode)
-00000ed0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00000ee0: 6e64 6572 5f6d 6163 3d70 6172 7365 5f6d  nder_mac=parse_m
-00000ef0: 6163 2873 656e 6465 725f 6d61 6329 2c0a  ac(sender_mac),.
-00000f00: 2020 2020 2020 2020 2020 2020 7365 6e64              send
-00000f10: 6572 5f69 703d 7061 7273 655f 6970 2873  er_ip=parse_ip(s
-00000f20: 656e 6465 725f 6970 292c 0a20 2020 2020  ender_ip),.     
-00000f30: 2020 2020 2020 2074 6172 6765 745f 6d61         target_ma
-00000f40: 633d 7061 7273 655f 6d61 6328 7461 7267  c=parse_mac(targ
-00000f50: 6574 5f6d 6163 292c 0a20 2020 2020 2020  et_mac),.       
-00000f60: 2020 2020 2074 6172 6765 745f 6970 3d70       target_ip=p
-00000f70: 6172 7365 5f69 7028 7461 7267 6574 5f69  arse_ip(target_i
-00000f80: 7029 0a20 2020 2020 2020 2029 0a0a 2020  p).        )..  
-00000f90: 2020 6465 6620 6275 696c 645f 6672 616d    def build_fram
-00000fa0: 6528 7365 6c66 2920 2d3e 2062 7974 6573  e(self) -> bytes
-00000fb0: 3a0a 2020 2020 2020 2020 6861 7264 7761  :.        hardwa
-00000fc0: 7265 5f66 6f72 6d61 7420 3d20 7374 7228  re_format = str(
-00000fd0: 7365 6c66 2e68 6172 6477 6172 655f 6c65  self.hardware_le
-00000fe0: 6e67 7468 2920 2b20 2773 270a 2020 2020  ngth) + 's'.    
-00000ff0: 2020 2020 7072 6f74 6f63 6f6c 5f66 6f72      protocol_for
-00001000: 6d61 7420 3d20 7374 7228 7365 6c66 2e70  mat = str(self.p
-00001010: 726f 746f 636f 6c5f 6c65 6e67 7468 2920  rotocol_length) 
-00001020: 2b20 2773 270a 2020 2020 2020 2020 7061  + 's'.        pa
-00001030: 636b 696e 675f 666f 726d 6174 203d 2027  cking_format = '
-00001040: 272e 6a6f 696e 285b 0a20 2020 2020 2020  '.join([.       
-00001050: 2020 2020 2022 2122 0a20 2020 2020 2020       "!".       
-00001060: 2020 2020 2022 4822 2c20 2023 2068 6172       "H",  # har
-00001070: 6477 6172 6520 7479 7065 0a20 2020 2020  dware type.     
-00001080: 2020 2020 2020 2022 4822 2c20 2023 2070         "H",  # p
-00001090: 726f 746f 636f 6c20 7479 7065 0a20 2020  rotocol type.   
-000010a0: 2020 2020 2020 2020 2027 4227 2c20 2023           'B',  #
-000010b0: 2068 6172 6477 6172 655f 6c65 6e67 7468   hardware_length
-000010c0: 0a20 2020 2020 2020 2020 2020 2027 4227  .            'B'
-000010d0: 2c20 2023 2070 726f 746f 636f 6c5f 6c65  ,  # protocol_le
-000010e0: 6e67 7468 0a20 2020 2020 2020 2020 2020  ngth.           
-000010f0: 2027 4827 2c20 2023 206f 7063 6f64 653a   'H',  # opcode:
-00001100: 204f 7063 6f64 6520 3d20 4f70 636f 6465   Opcode = Opcode
-00001110: 2e72 6571 7565 7374 0a20 2020 2020 2020  .request.       
-00001120: 2020 2020 2068 6172 6477 6172 655f 666f       hardware_fo
-00001130: 726d 6174 2c20 2023 2073 656e 6465 725f  rmat,  # sender_
-00001140: 6d61 630a 2020 2020 2020 2020 2020 2020  mac.            
-00001150: 7072 6f74 6f63 6f6c 5f66 6f72 6d61 742c  protocol_format,
-00001160: 2020 2320 7365 6e64 6572 5f69 703a 2069    # sender_ip: i
-00001170: 6e74 0a20 2020 2020 2020 2020 2020 2068  nt.            h
-00001180: 6172 6477 6172 655f 666f 726d 6174 2c20  ardware_format, 
-00001190: 2023 2074 6172 6765 745f 6d61 703a 2069   # target_map: i
-000011a0: 6e74 0a20 2020 2020 2020 2020 2020 2070  nt.            p
-000011b0: 726f 746f 636f 6c5f 666f 726d 6174 2c20  rotocol_format, 
-000011c0: 2023 2074 6172 6765 745f 6970 3a20 696e   # target_ip: in
-000011d0: 740a 2020 2020 2020 2020 5d29 0a0a 2020  t.        ])..  
-000011e0: 2020 2020 2020 7265 7475 726e 2073 7472        return str
-000011f0: 7563 742e 7061 636b 280a 2020 2020 2020  uct.pack(.      
-00001200: 2020 2020 2020 7061 636b 696e 675f 666f        packing_fo
-00001210: 726d 6174 2c0a 2020 2020 2020 2020 2020  rmat,.          
-00001220: 2020 7365 6c66 2e68 6172 6477 6172 655f    self.hardware_
-00001230: 7479 7065 2e76 616c 7565 2c0a 2020 2020  type.value,.    
-00001240: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00001250: 746f 636f 6c5f 7479 7065 2e76 616c 7565  tocol_type.value
-00001260: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00001270: 6c66 2e68 6172 6477 6172 655f 6c65 6e67  lf.hardware_leng
-00001280: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-00001290: 7365 6c66 2e70 726f 746f 636f 6c5f 6c65  self.protocol_le
-000012a0: 6e67 7468 2c0a 2020 2020 2020 2020 2020  ngth,.          
-000012b0: 2020 7365 6c66 2e6f 7063 6f64 652e 7661    self.opcode.va
-000012c0: 6c75 652c 0a20 2020 2020 2020 2020 2020  lue,.           
-000012d0: 2065 6e66 6f72 6365 5f6d 6163 2873 656c   enforce_mac(sel
-000012e0: 662e 7365 6e64 6572 5f6d 6163 292c 0a20  f.sender_mac),. 
-000012f0: 2020 2020 2020 2020 2020 2065 6e66 6f72             enfor
-00001300: 6365 5f69 7028 7365 6c66 2e73 656e 6465  ce_ip(self.sende
-00001310: 725f 6970 292c 0a20 2020 2020 2020 2020  r_ip),.         
-00001320: 2020 2065 6e66 6f72 6365 5f6d 6163 2873     enforce_mac(s
-00001330: 656c 662e 7461 7267 6574 5f6d 6163 292c  elf.target_mac),
-00001340: 0a20 2020 2020 2020 2020 2020 2065 6e66  .            enf
-00001350: 6f72 6365 5f69 7028 7365 6c66 2e74 6172  orce_ip(self.tar
-00001360: 6765 745f 6970 292c 0a20 2020 2020 2020  get_ip),.       
-00001370: 2029 0a0a 2020 2020 6465 6620 5f5f 7265   )..    def __re
-00001380: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-00001390: 2020 2020 7265 7475 726e 2066 223c 4172      return f"<Ar
-000013a0: 7050 6163 6b65 7420 7461 7267 6574 5f69  pPacket target_i
-000013b0: 703d 7b73 656c 662e 7461 7267 6574 5f69  p={self.target_i
-000013c0: 707d 3e22 0a0a 0a64 6566 2073 697a 655f  p}>"...def size_
-000013d0: 6f66 2874 7970 653a 2074 7970 696e 672e  of(type: typing.
-000013e0: 556e 696f 6e5b 4861 7264 7761 7265 5479  Union[HardwareTy
-000013f0: 7065 2c20 5072 6f74 6f63 6f6c 5d29 202d  pe, Protocol]) -
-00001400: 3e20 696e 743a 0a20 2020 2069 6620 7479  > int:.    if ty
-00001410: 7065 2069 7320 5072 6f74 6f63 6f6c 2e69  pe is Protocol.i
-00001420: 703a 0a20 2020 2020 2020 2072 6574 7572  p:.        retur
-00001430: 6e20 340a 2020 2020 656c 6966 2074 7970  n 4.    elif typ
-00001440: 6520 6973 2048 6172 6477 6172 6554 7970  e is HardwareTyp
-00001450: 652e 6574 6865 726e 6574 3a0a 2020 2020  e.ethernet:.    
-00001460: 2020 2020 7265 7475 726e 2036 0a20 2020      return 6.   
-00001470: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-00001480: 6169 7365 2045 7863 6570 7469 6f6e 0a    aise Exception.
+00000000: 696d 706f 7274 2073 7472 7563 740a 696d  import struct.im
+00000010: 706f 7274 2074 7970 696e 670a 6672 6f6d  port typing.from
+00000020: 2065 6e75 6d20 696d 706f 7274 2045 6e75   enum import Enu
+00000030: 6d0a 0a66 726f 6d20 6169 6f61 7270 2e5f  m..from aioarp._
+00000040: 7574 696c 7320 696d 706f 7274 2065 6e66  utils import enf
+00000050: 6f72 6365 5f69 702c 2065 6e66 6f72 6365  orce_ip, enforce
+00000060: 5f6d 6163 2c20 7061 7273 655f 6970 2c20  _mac, parse_ip, 
+00000070: 7061 7273 655f 6d61 630a 0a45 5448 4552  parse_mac..ETHER
+00000080: 4e45 545f 4845 4144 4552 5f53 495a 4520  NET_HEADER_SIZE 
+00000090: 3d20 3134 0a41 5250 5f48 4541 4445 525f  = 14.ARP_HEADER_
+000000a0: 5349 5a45 203d 2032 380a 0a5f 5f61 6c6c  SIZE = 28..__all
+000000b0: 5f5f 203d 2028 0a20 2020 2027 4554 4845  __ = (.    'ETHE
+000000c0: 524e 4554 5f48 4541 4445 525f 5349 5a45  RNET_HEADER_SIZE
+000000d0: 272c 0a20 2020 2027 4152 505f 4845 4144  ',.    'ARP_HEAD
+000000e0: 4552 5f53 495a 4527 2c0a 2020 2020 2748  ER_SIZE',.    'H
+000000f0: 6172 6477 6172 6554 7970 6527 2c0a 2020  ardwareType',.  
+00000100: 2020 2750 726f 746f 636f 6c27 2c0a 2020    'Protocol',.  
+00000110: 2020 274f 7063 6f64 6527 2c0a 2020 2020    'Opcode',.    
+00000120: 2745 7468 5061 636b 6574 272c 0a20 2020  'EthPacket',.   
+00000130: 2027 4172 7050 6163 6b65 7427 2c0a 2020   'ArpPacket',.  
+00000140: 2020 2773 697a 655f 6f66 270a 290a 0a63    'size_of'.)..c
+00000150: 6c61 7373 2048 6172 6477 6172 6554 7970  lass HardwareTyp
+00000160: 6528 456e 756d 293a 0a20 2020 2065 7468  e(Enum):.    eth
+00000170: 6572 6e65 7420 3d20 310a 0a0a 636c 6173  ernet = 1...clas
+00000180: 7320 5072 6f74 6f63 6f6c 2845 6e75 6d29  s Protocol(Enum)
+00000190: 3a0a 2020 2020 6970 203d 2030 7830 3830  :.    ip = 0x080
+000001a0: 300a 2020 2020 6172 7020 3d20 3078 3038  0.    arp = 0x08
+000001b0: 3036 0a0a 0a63 6c61 7373 204f 7063 6f64  06...class Opcod
+000001c0: 6528 456e 756d 293a 0a20 2020 2072 6571  e(Enum):.    req
+000001d0: 7565 7374 203d 2031 0a20 2020 2072 6573  uest = 1.    res
+000001e0: 706f 6e73 6520 3d20 320a 0a0a 636c 6173  ponse = 2...clas
+000001f0: 7320 4574 6850 6163 6b65 743a 0a20 2020  s EthPacket:.   
+00000200: 2066 6f72 6d61 7420 3d20 2221 3673 3673   format = "!6s6s
+00000210: 4822 0a0a 2020 2020 6465 6620 5f5f 696e  H"..    def __in
+00000220: 6974 5f5f 2873 656c 662c 0a20 2020 2020  it__(self,.     
+00000230: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00000240: 6574 5f6d 6163 3a20 7374 722c 0a20 2020  et_mac: str,.   
+00000250: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00000260: 6e64 6572 5f6d 6163 3a20 7374 722c 0a20  nder_mac: str,. 
+00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000280: 7072 6f74 6f3a 2050 726f 746f 636f 6c29  proto: Protocol)
+00000290: 3a0a 2020 2020 2020 2020 7365 6c66 2e74  :.        self.t
+000002a0: 6172 6765 745f 6d61 6320 3d20 7461 7267  arget_mac = targ
+000002b0: 6574 5f6d 6163 0a20 2020 2020 2020 2073  et_mac.        s
+000002c0: 656c 662e 7365 6e64 6572 5f6d 6163 203d  elf.sender_mac =
+000002d0: 2073 656e 6465 725f 6d61 630a 2020 2020   sender_mac.    
+000002e0: 2020 2020 7365 6c66 2e70 726f 746f 203d      self.proto =
+000002f0: 2070 726f 746f 0a0a 2020 2020 4063 6c61   proto..    @cla
+00000300: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00000310: 2070 6172 7365 2863 6c73 2c20 6672 616d   parse(cls, fram
+00000320: 653a 2062 7974 6573 2920 2d3e 2022 4574  e: bytes) -> "Et
+00000330: 6850 6163 6b65 7422 3a0a 2020 2020 2020  hPacket":.      
+00000340: 2020 7461 7267 6574 5f6d 6163 2c20 7365    target_mac, se
+00000350: 6e64 6572 5f6d 6163 2c20 7072 6f74 6f20  nder_mac, proto 
+00000360: 3d20 7374 7275 6374 2e75 6e70 6163 6b28  = struct.unpack(
+00000370: 0a20 2020 2020 2020 2020 2020 2027 2136  .            '!6
+00000380: 7336 7348 272c 0a20 2020 2020 2020 2020  s6sH',.         
+00000390: 2020 2066 7261 6d65 0a20 2020 2020 2020     frame.       
+000003a0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+000003b0: 6e20 636c 7328 0a20 2020 2020 2020 2020  n cls(.         
+000003c0: 2020 2074 6172 6765 745f 6d61 633d 7061     target_mac=pa
+000003d0: 7273 655f 6d61 6328 7461 7267 6574 5f6d  rse_mac(target_m
+000003e0: 6163 292c 0a20 2020 2020 2020 2020 2020  ac),.           
+000003f0: 2073 656e 6465 725f 6d61 633d 7061 7273   sender_mac=pars
+00000400: 655f 6d61 6328 7365 6e64 6572 5f6d 6163  e_mac(sender_mac
+00000410: 292c 0a20 2020 2020 2020 2020 2020 2070  ),.            p
+00000420: 726f 746f 3d50 726f 746f 636f 6c28 7072  roto=Protocol(pr
+00000430: 6f74 6f29 0a20 2020 2020 2020 2029 0a0a  oto).        )..
+00000440: 2020 2020 6465 6620 6275 696c 645f 6672      def build_fr
+00000450: 616d 6528 7365 6c66 2920 2d3e 2062 7974  ame(self) -> byt
+00000460: 6573 3a0a 2020 2020 2020 2020 7265 7475  es:.        retu
+00000470: 726e 2073 7472 7563 742e 7061 636b 280a  rn struct.pack(.
+00000480: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000490: 2e66 6f72 6d61 742c 0a20 2020 2020 2020  .format,.       
+000004a0: 2020 2020 2065 6e66 6f72 6365 5f6d 6163       enforce_mac
+000004b0: 2873 656c 662e 7461 7267 6574 5f6d 6163  (self.target_mac
+000004c0: 292c 0a20 2020 2020 2020 2020 2020 2065  ),.            e
+000004d0: 6e66 6f72 6365 5f6d 6163 2873 656c 662e  nforce_mac(self.
+000004e0: 7365 6e64 6572 5f6d 6163 292c 0a20 2020  sender_mac),.   
+000004f0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00000500: 6f74 6f2e 7661 6c75 650a 2020 2020 2020  oto.value.      
+00000510: 2020 290a 0a20 2020 2064 6566 205f 5f72    )..    def __r
+00000520: 6570 725f 5f28 7365 6c66 2920 2d3e 2073  epr__(self) -> s
+00000530: 7472 3a0a 2020 2020 2020 2020 7265 7475  tr:.        retu
+00000540: 726e 2066 223c 4574 6850 6163 6b65 7420  rn f"<EthPacket 
+00000550: 7461 7267 6574 3d7b 7365 6c66 2e74 6172  target={self.tar
+00000560: 6765 745f 6d61 637d 2073 6f75 7263 653d  get_mac} source=
+00000570: 7b73 656c 662e 7365 6e64 6572 5f6d 6163  {self.sender_mac
+00000580: 7d20 7072 6f74 6f3d 7b73 656c 662e 7072  } proto={self.pr
+00000590: 6f74 6f2e 6e61 6d65 7d3e 220a 0a0a 636c  oto.name}>"...cl
+000005a0: 6173 7320 4172 7050 6163 6b65 743a 0a0a  ass ArpPacket:..
+000005b0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000005c0: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+000005d0: 2020 2020 2020 2020 6861 7264 7761 7265          hardware
+000005e0: 5f74 7970 653a 2048 6172 6477 6172 6554  _type: HardwareT
+000005f0: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+00000600: 2020 2020 2020 7072 6f74 6f63 6f6c 5f74        protocol_t
+00000610: 7970 653a 2050 726f 746f 636f 6c2c 0a20  ype: Protocol,. 
+00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000630: 7365 6e64 6572 5f6d 6163 3a20 7374 722c  sender_mac: str,
+00000640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000650: 2020 7365 6e64 6572 5f69 703a 2073 7472    sender_ip: str
+00000660: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000670: 2020 2074 6172 6765 745f 6d61 633a 2073     target_mac: s
+00000680: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00000690: 2020 2020 2074 6172 6765 745f 6970 3a20       target_ip: 
+000006a0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+000006b0: 2020 2020 2020 6f70 636f 6465 3a20 4f70        opcode: Op
+000006c0: 636f 6465 203d 204f 7063 6f64 652e 7265  code = Opcode.re
+000006d0: 7175 6573 7429 3a0a 2020 2020 2020 2020  quest):.        
+000006e0: 7365 6c66 2e68 6172 6477 6172 655f 7479  self.hardware_ty
+000006f0: 7065 203d 2068 6172 6477 6172 655f 7479  pe = hardware_ty
+00000700: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
+00000710: 7072 6f74 6f63 6f6c 5f74 7970 6520 3d20  protocol_type = 
+00000720: 7072 6f74 6f63 6f6c 5f74 7970 650a 2020  protocol_type.  
+00000730: 2020 2020 2020 7365 6c66 2e6f 7063 6f64        self.opcod
+00000740: 6520 3d20 6f70 636f 6465 0a20 2020 2020  e = opcode.     
+00000750: 2020 2073 656c 662e 7365 6e64 6572 5f6d     self.sender_m
+00000760: 6163 203d 2073 656e 6465 725f 6d61 630a  ac = sender_mac.
+00000770: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+00000780: 6465 725f 6970 203d 2073 656e 6465 725f  der_ip = sender_
+00000790: 6970 0a20 2020 2020 2020 2073 656c 662e  ip.        self.
+000007a0: 7461 7267 6574 5f6d 6163 203d 2074 6172  target_mac = tar
+000007b0: 6765 745f 6d61 630a 2020 2020 2020 2020  get_mac.        
+000007c0: 7365 6c66 2e74 6172 6765 745f 6970 203d  self.target_ip =
+000007d0: 2074 6172 6765 745f 6970 0a0a 2020 2020   target_ip..    
+000007e0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+000007f0: 6620 6861 7264 7761 7265 5f6c 656e 6774  f hardware_lengt
+00000800: 6828 7365 6c66 2920 2d3e 2069 6e74 3a0a  h(self) -> int:.
+00000810: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000820: 697a 655f 6f66 2873 656c 662e 6861 7264  ize_of(self.hard
+00000830: 7761 7265 5f74 7970 6529 0a0a 2020 2020  ware_type)..    
+00000840: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00000850: 6620 7072 6f74 6f63 6f6c 5f6c 656e 6774  f protocol_lengt
+00000860: 6828 7365 6c66 2920 2d3e 2069 6e74 3a0a  h(self) -> int:.
+00000870: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000880: 697a 655f 6f66 2873 656c 662e 7072 6f74  ize_of(self.prot
+00000890: 6f63 6f6c 5f74 7970 6529 0a0a 2020 2020  ocol_type)..    
+000008a0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+000008b0: 2064 6566 2070 6172 7365 2863 6c73 2c20   def parse(cls, 
+000008c0: 6672 616d 653a 2062 7974 6573 2920 2d3e  frame: bytes) ->
+000008d0: 2022 4172 7050 6163 6b65 7422 3a0a 2020   "ArpPacket":.  
+000008e0: 2020 2020 2020 6861 7264 7761 7265 5f66        hardware_f
+000008f0: 6f72 6d61 7420 3d20 2736 7327 0a20 2020  ormat = '6s'.   
+00000900: 2020 2020 2070 726f 746f 636f 6c5f 666f       protocol_fo
+00000910: 726d 6174 203d 2027 3473 270a 2020 2020  rmat = '4s'.    
+00000920: 2020 2020 7061 636b 696e 675f 666f 726d      packing_form
+00000930: 6174 203d 2027 272e 6a6f 696e 285b 0a20  at = ''.join([. 
+00000940: 2020 2020 2020 2020 2020 2022 2122 0a20             "!". 
+00000950: 2020 2020 2020 2020 2020 2022 4822 2c20             "H", 
+00000960: 2023 2068 6172 6477 6172 6520 7479 7065   # hardware type
+00000970: 0a20 2020 2020 2020 2020 2020 2022 4822  .            "H"
+00000980: 2c20 2023 2070 726f 746f 636f 6c20 7479  ,  # protocol ty
+00000990: 7065 0a20 2020 2020 2020 2020 2020 2027  pe.            '
+000009a0: 4227 2c20 2023 2068 6172 6477 6172 655f  B',  # hardware_
+000009b0: 6c65 6e67 7468 0a20 2020 2020 2020 2020  length.         
+000009c0: 2020 2027 4227 2c20 2023 2070 726f 746f     'B',  # proto
+000009d0: 636f 6c5f 6c65 6e67 7468 0a20 2020 2020  col_length.     
+000009e0: 2020 2020 2020 2027 4827 2c20 2023 206f         'H',  # o
+000009f0: 7063 6f64 653a 204f 7063 6f64 6520 3d20  pcode: Opcode = 
+00000a00: 4f70 636f 6465 2e72 6571 7565 7374 0a20  Opcode.request. 
+00000a10: 2020 2020 2020 2020 2020 2068 6172 6477             hardw
+00000a20: 6172 655f 666f 726d 6174 2c20 2023 2073  are_format,  # s
+00000a30: 656e 6465 725f 6d61 630a 2020 2020 2020  ender_mac.      
+00000a40: 2020 2020 2020 7072 6f74 6f63 6f6c 5f66        protocol_f
+00000a50: 6f72 6d61 742c 2020 2320 7365 6e64 6572  ormat,  # sender
+00000a60: 5f69 703a 2069 6e74 0a20 2020 2020 2020  _ip: int.       
+00000a70: 2020 2020 2068 6172 6477 6172 655f 666f       hardware_fo
+00000a80: 726d 6174 2c20 2023 2074 6172 6765 745f  rmat,  # target_
+00000a90: 6d61 703a 2069 6e74 0a20 2020 2020 2020  map: int.       
+00000aa0: 2020 2020 2070 726f 746f 636f 6c5f 666f       protocol_fo
+00000ab0: 726d 6174 2c20 2023 2074 6172 6765 745f  rmat,  # target_
+00000ac0: 6970 3a20 696e 740a 2020 2020 2020 2020  ip: int.        
+00000ad0: 5d29 0a0a 2020 2020 2020 2020 280a 2020  ])..        (.  
+00000ae0: 2020 2020 2020 2020 2020 6861 7264 7761            hardwa
+00000af0: 7265 5f74 7970 652c 0a20 2020 2020 2020  re_type,.       
+00000b00: 2020 2020 2070 726f 746f 636f 6c5f 7479       protocol_ty
+00000b10: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+00000b20: 6861 7264 7761 7265 5f6c 656e 6774 682c  hardware_length,
+00000b30: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00000b40: 746f 636f 6c5f 6c65 6e67 7468 2c0a 2020  tocol_length,.  
+00000b50: 2020 2020 2020 2020 2020 6f70 636f 6465            opcode
+00000b60: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+00000b70: 6e64 6572 5f6d 6163 2c0a 2020 2020 2020  nder_mac,.      
+00000b80: 2020 2020 2020 7365 6e64 6572 5f69 702c        sender_ip,
+00000b90: 0a20 2020 2020 2020 2020 2020 2074 6172  .            tar
+00000ba0: 6765 745f 6d61 632c 0a20 2020 2020 2020  get_mac,.       
+00000bb0: 2020 2020 2074 6172 6765 745f 6970 0a20       target_ip. 
+00000bc0: 2020 2020 2020 2029 203d 2073 7472 7563         ) = struc
+00000bd0: 742e 756e 7061 636b 280a 2020 2020 2020  t.unpack(.      
+00000be0: 2020 2020 2020 7061 636b 696e 675f 666f        packing_fo
+00000bf0: 726d 6174 2c0a 2020 2020 2020 2020 2020  rmat,.          
+00000c00: 2020 6672 616d 650a 2020 2020 2020 2020    frame.        
+00000c10: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00000c20: 2063 6c73 280a 2020 2020 2020 2020 2020   cls(.          
+00000c30: 2020 6861 7264 7761 7265 5f74 7970 653d    hardware_type=
+00000c40: 4861 7264 7761 7265 5479 7065 2868 6172  HardwareType(har
+00000c50: 6477 6172 655f 7479 7065 292c 0a20 2020  dware_type),.   
+00000c60: 2020 2020 2020 2020 2070 726f 746f 636f           protoco
+00000c70: 6c5f 7479 7065 3d50 726f 746f 636f 6c28  l_type=Protocol(
+00000c80: 7072 6f74 6f63 6f6c 5f74 7970 6529 2c0a  protocol_type),.
+00000c90: 2020 2020 2020 2020 2020 2020 6f70 636f              opco
+00000ca0: 6465 3d4f 7063 6f64 6528 6f70 636f 6465  de=Opcode(opcode
+00000cb0: 292c 0a20 2020 2020 2020 2020 2020 2073  ),.            s
+00000cc0: 656e 6465 725f 6d61 633d 7061 7273 655f  ender_mac=parse_
+00000cd0: 6d61 6328 7365 6e64 6572 5f6d 6163 292c  mac(sender_mac),
+00000ce0: 0a20 2020 2020 2020 2020 2020 2073 656e  .            sen
+00000cf0: 6465 725f 6970 3d70 6172 7365 5f69 7028  der_ip=parse_ip(
+00000d00: 7365 6e64 6572 5f69 7029 2c0a 2020 2020  sender_ip),.    
+00000d10: 2020 2020 2020 2020 7461 7267 6574 5f6d          target_m
+00000d20: 6163 3d70 6172 7365 5f6d 6163 2874 6172  ac=parse_mac(tar
+00000d30: 6765 745f 6d61 6329 2c0a 2020 2020 2020  get_mac),.      
+00000d40: 2020 2020 2020 7461 7267 6574 5f69 703d        target_ip=
+00000d50: 7061 7273 655f 6970 2874 6172 6765 745f  parse_ip(target_
+00000d60: 6970 290a 2020 2020 2020 2020 290a 0a20  ip).        ).. 
+00000d70: 2020 2064 6566 2062 7569 6c64 5f66 7261     def build_fra
+00000d80: 6d65 2873 656c 6629 202d 3e20 6279 7465  me(self) -> byte
+00000d90: 733a 0a20 2020 2020 2020 2068 6172 6477  s:.        hardw
+00000da0: 6172 655f 666f 726d 6174 203d 2073 7472  are_format = str
+00000db0: 2873 656c 662e 6861 7264 7761 7265 5f6c  (self.hardware_l
+00000dc0: 656e 6774 6829 202b 2027 7327 0a20 2020  ength) + 's'.   
+00000dd0: 2020 2020 2070 726f 746f 636f 6c5f 666f       protocol_fo
+00000de0: 726d 6174 203d 2073 7472 2873 656c 662e  rmat = str(self.
+00000df0: 7072 6f74 6f63 6f6c 5f6c 656e 6774 6829  protocol_length)
+00000e00: 202b 2027 7327 0a20 2020 2020 2020 2070   + 's'.        p
+00000e10: 6163 6b69 6e67 5f66 6f72 6d61 7420 3d20  acking_format = 
+00000e20: 2727 2e6a 6f69 6e28 5b0a 2020 2020 2020  ''.join([.      
+00000e30: 2020 2020 2020 2221 220a 2020 2020 2020        "!".      
+00000e40: 2020 2020 2020 2248 222c 2020 2320 6861        "H",  # ha
+00000e50: 7264 7761 7265 2074 7970 650a 2020 2020  rdware type.    
+00000e60: 2020 2020 2020 2020 2248 222c 2020 2320          "H",  # 
+00000e70: 7072 6f74 6f63 6f6c 2074 7970 650a 2020  protocol type.  
+00000e80: 2020 2020 2020 2020 2020 2742 272c 2020            'B',  
+00000e90: 2320 6861 7264 7761 7265 5f6c 656e 6774  # hardware_lengt
+00000ea0: 680a 2020 2020 2020 2020 2020 2020 2742  h.            'B
+00000eb0: 272c 2020 2320 7072 6f74 6f63 6f6c 5f6c  ',  # protocol_l
+00000ec0: 656e 6774 680a 2020 2020 2020 2020 2020  ength.          
+00000ed0: 2020 2748 272c 2020 2320 6f70 636f 6465    'H',  # opcode
+00000ee0: 3a20 4f70 636f 6465 203d 204f 7063 6f64  : Opcode = Opcod
+00000ef0: 652e 7265 7175 6573 740a 2020 2020 2020  e.request.      
+00000f00: 2020 2020 2020 6861 7264 7761 7265 5f66        hardware_f
+00000f10: 6f72 6d61 742c 2020 2320 7365 6e64 6572  ormat,  # sender
+00000f20: 5f6d 6163 0a20 2020 2020 2020 2020 2020  _mac.           
+00000f30: 2070 726f 746f 636f 6c5f 666f 726d 6174   protocol_format
+00000f40: 2c20 2023 2073 656e 6465 725f 6970 3a20  ,  # sender_ip: 
+00000f50: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+00000f60: 6861 7264 7761 7265 5f66 6f72 6d61 742c  hardware_format,
+00000f70: 2020 2320 7461 7267 6574 5f6d 6170 3a20    # target_map: 
+00000f80: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+00000f90: 7072 6f74 6f63 6f6c 5f66 6f72 6d61 742c  protocol_format,
+00000fa0: 2020 2320 7461 7267 6574 5f69 703a 2069    # target_ip: i
+00000fb0: 6e74 0a20 2020 2020 2020 205d 290a 0a20  nt.        ]).. 
+00000fc0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+00000fd0: 7275 6374 2e70 6163 6b28 0a20 2020 2020  ruct.pack(.     
+00000fe0: 2020 2020 2020 2070 6163 6b69 6e67 5f66         packing_f
+00000ff0: 6f72 6d61 742c 0a20 2020 2020 2020 2020  ormat,.         
+00001000: 2020 2073 656c 662e 6861 7264 7761 7265     self.hardware
+00001010: 5f74 7970 652e 7661 6c75 652c 0a20 2020  _type.value,.   
+00001020: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00001030: 6f74 6f63 6f6c 5f74 7970 652e 7661 6c75  otocol_type.valu
+00001040: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
+00001050: 656c 662e 6861 7264 7761 7265 5f6c 656e  elf.hardware_len
+00001060: 6774 682c 0a20 2020 2020 2020 2020 2020  gth,.           
+00001070: 2073 656c 662e 7072 6f74 6f63 6f6c 5f6c   self.protocol_l
+00001080: 656e 6774 682c 0a20 2020 2020 2020 2020  ength,.         
+00001090: 2020 2073 656c 662e 6f70 636f 6465 2e76     self.opcode.v
+000010a0: 616c 7565 2c0a 2020 2020 2020 2020 2020  alue,.          
+000010b0: 2020 656e 666f 7263 655f 6d61 6328 7365    enforce_mac(se
+000010c0: 6c66 2e73 656e 6465 725f 6d61 6329 2c0a  lf.sender_mac),.
+000010d0: 2020 2020 2020 2020 2020 2020 656e 666f              enfo
+000010e0: 7263 655f 6970 2873 656c 662e 7365 6e64  rce_ip(self.send
+000010f0: 6572 5f69 7029 2c0a 2020 2020 2020 2020  er_ip),.        
+00001100: 2020 2020 656e 666f 7263 655f 6d61 6328      enforce_mac(
+00001110: 7365 6c66 2e74 6172 6765 745f 6d61 6329  self.target_mac)
+00001120: 2c0a 2020 2020 2020 2020 2020 2020 656e  ,.            en
+00001130: 666f 7263 655f 6970 2873 656c 662e 7461  force_ip(self.ta
+00001140: 7267 6574 5f69 7029 2c0a 2020 2020 2020  rget_ip),.      
+00001150: 2020 290a 0a20 2020 2064 6566 205f 5f72    )..    def __r
+00001160: 6570 725f 5f28 7365 6c66 2920 2d3e 2073  epr__(self) -> s
+00001170: 7472 3a0a 2020 2020 2020 2020 7265 7475  tr:.        retu
+00001180: 726e 2066 223c 4172 7050 6163 6b65 7420  rn f"<ArpPacket 
+00001190: 7461 7267 6574 5f69 703d 7b73 656c 662e  target_ip={self.
+000011a0: 7461 7267 6574 5f69 707d 3e22 0a0a 0a64  target_ip}>"...d
+000011b0: 6566 2073 697a 655f 6f66 2874 7970 653a  ef size_of(type:
+000011c0: 2074 7970 696e 672e 556e 696f 6e5b 4861   typing.Union[Ha
+000011d0: 7264 7761 7265 5479 7065 2c20 5072 6f74  rdwareType, Prot
+000011e0: 6f63 6f6c 5d29 202d 3e20 696e 743a 0a20  ocol]) -> int:. 
+000011f0: 2020 2069 6620 7479 7065 2069 7320 5072     if type is Pr
+00001200: 6f74 6f63 6f6c 2e69 703a 0a20 2020 2020  otocol.ip:.     
+00001210: 2020 2072 6574 7572 6e20 340a 2020 2020     return 4.    
+00001220: 656c 6966 2074 7970 6520 6973 2048 6172  elif type is Har
+00001230: 6477 6172 6554 7970 652e 6574 6865 726e  dwareType.ethern
+00001240: 6574 3a0a 2020 2020 2020 2020 7265 7475  et:.        retu
+00001250: 726e 2036 0a20 2020 2065 6c73 653a 0a20  rn 6.    else:. 
+00001260: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00001270: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00001280: 2829 0a                                  ().
```

### Comparing `aioarp-0.0.4/.ruff_cache/content/b74ab4e72907ed4b` & `aioarp-0.0.5/aioarp/_sync.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,193 +1,125 @@
-00000000: 0100 0000 0000 0000 0c00 0000 0000 0000  ................
-00000010: 6169 6f61 7270 2e5f 7379 6e63 0d00 0000  aioarp._sync....
-00000020: 0000 0000 0400 0000 0000 0000 7469 6d65  ............time
-00000030: 0000 0000 0b00 0000 0600 0000 0000 0000  ................
-00000040: 7479 7069 6e67 0c00 0000 1900 0000 1200  typing..........
-00000050: 0000 0000 0000 6169 6f61 7270 2e5f 6578  ......aioarp._ex
-00000060: 6365 7074 696f 6e73 2e00 0000 4000 0000  ceptions....@...
-00000070: 1b00 0000 0000 0000 6169 6f61 7270 2e5f  ........aioarp._
-00000080: 6172 702e 4152 505f 4845 4144 4552 5f53  arp.ARP_HEADER_S
-00000090: 495a 4559 0000 0068 0000 0020 0000 0000  IZEY...h... ....
-000000a0: 0000 0061 696f 6172 702e 5f61 7270 2e45  ...aioarp._arp.E
-000000b0: 5448 4552 4e45 545f 4845 4144 4552 5f53  THERNET_HEADER_S
-000000c0: 495a 456a 0000 007e 0000 0015 0000 0000  IZEj...~........
-000000d0: 0000 0061 696f 6172 702e 5f61 7270 2e41  ...aioarp._arp.A
-000000e0: 7270 5061 636b 6574 8000 0000 8900 0000  rpPacket........
-000000f0: 1500 0000 0000 0000 6169 6f61 7270 2e5f  ........aioarp._
-00000100: 6172 702e 4574 6850 6163 6b65 748b 0000  arp.EthPacket...
-00000110: 0094 0000 0014 0000 0000 0000 0061 696f  .............aio
-00000120: 6172 702e 5f61 7270 2e50 726f 746f 636f  arp._arp.Protoco
-00000130: 6c96 0000 009e 0000 001b 0000 0000 0000  l...............
-00000140: 0061 696f 6172 702e 5f75 7469 6c73 2e69  .aioarp._utils.i
-00000150: 735f 7661 6c69 645f 6970 7634 b900 0000  s_valid_ipv4....
-00000160: c600 0000 2400 0000 0000 0000 6169 6f61  ....$.......aioa
-00000170: 7270 2e64 6566 6175 6c74 732e 4445 4641  rp.defaults.DEFA
-00000180: 554c 545f 5245 4144 5f54 494d 454f 5554  ULT_READ_TIMEOUT
-00000190: e300 0000 f700 0000 2a00 0000 0000 0000  ........*.......
-000001a0: 6169 6f61 7270 2e64 6566 6175 6c74 732e  aioarp.defaults.
-000001b0: 4445 4641 554c 545f 5245 504c 595f 4d49  DEFAULT_REPLY_MI
-000001c0: 5353 494e 475f 5449 4d45 f900 0000 1301  SSING_TIME......
-000001d0: 0000 2500 0000 0000 0000 6169 6f61 7270  ..%.......aioarp
-000001e0: 2e64 6566 6175 6c74 732e 4445 4641 554c  .defaults.DEFAUL
-000001f0: 545f 5752 4954 455f 5449 4d45 4f55 5415  T_WRITE_TIMEOUT.
-00000200: 0100 002a 0100 000d 0000 0000 0000 0061  ...*...........a
-00000210: 696f 6172 702e 5374 7265 616d 3f01 0000  ioarp.Stream?...
-00000220: 4501 0000 0100 0000 0000 0000 0f00 0000  E...............
-00000230: 0000 0000 556e 736f 7274 6564 496d 706f  ....UnsortedImpo
-00000240: 7274 7329 0000 0000 0000 0049 6d70 6f72  rts).......Impor
-00000250: 7420 626c 6f63 6b20 6973 2075 6e2d 736f  t block is un-so
-00000260: 7274 6564 206f 7220 756e 2d66 6f72 6d61  rted or un-forma
-00000270: 7474 6564 0110 0000 0000 0000 004f 7267  tted.........Org
-00000280: 616e 697a 6520 696d 706f 7274 7300 0000  anize imports...
-00000290: 0047 0100 0001 0100 0000 0000 0000 0000  .G..............
-000002a0: 0000 4701 0000 0134 0100 0000 0000 0069  ..G....4.......i
-000002b0: 6d70 6f72 7420 7469 6d65 0a69 6d70 6f72  mport time.impor
-000002c0: 7420 7479 7069 6e67 0a0a 6672 6f6d 2061  t typing..from a
-000002d0: 696f 6172 7020 696d 706f 7274 2053 7472  ioarp import Str
-000002e0: 6561 6d2c 205f 6578 6365 7074 696f 6e73  eam, _exceptions
-000002f0: 2061 7320 6578 630a 6672 6f6d 2061 696f   as exc.from aio
-00000300: 6172 702e 5f61 7270 2069 6d70 6f72 7420  arp._arp import 
-00000310: 4152 505f 4845 4144 4552 5f53 495a 452c  ARP_HEADER_SIZE,
-00000320: 2045 5448 4552 4e45 545f 4845 4144 4552   ETHERNET_HEADER
-00000330: 5f53 495a 452c 2041 7270 5061 636b 6574  _SIZE, ArpPacket
-00000340: 2c20 4574 6850 6163 6b65 742c 2050 726f  , EthPacket, Pro
-00000350: 746f 636f 6c0a 6672 6f6d 2061 696f 6172  tocol.from aioar
-00000360: 702e 5f75 7469 6c73 2069 6d70 6f72 7420  p._utils import 
-00000370: 6973 5f76 616c 6964 5f69 7076 340a 6672  is_valid_ipv4.fr
-00000380: 6f6d 2061 696f 6172 702e 6465 6661 756c  om aioarp.defaul
-00000390: 7473 2069 6d70 6f72 7420 4445 4641 554c  ts import DEFAUL
-000003a0: 545f 5245 4144 5f54 494d 454f 5554 2c20  T_READ_TIMEOUT, 
-000003b0: 4445 4641 554c 545f 5245 504c 595f 4d49  DEFAULT_REPLY_MI
-000003c0: 5353 494e 475f 5449 4d45 2c20 4445 4641  SSING_TIME, DEFA
-000003d0: 554c 545f 5752 4954 455f 5449 4d45 4f55  ULT_WRITE_TIMEOU
-000003e0: 540a 0a03 0000 0000 0000 0000 0000 0000  T...............
-000003f0: 0000 0001 0000 0000 0000 0029 0000 0000  ...........)....
-00000400: 0000 002f 686f 6d65 2f74 6573 742f 4465  .../home/test/De
-00000410: 736b 746f 702f 6169 6f61 7270 2f61 696f  sktop/aioarp/aio
-00000420: 6172 702f 5f73 796e 632e 7079 d507 0000  arp/_sync.py....
-00000430: 0000 0000 696d 706f 7274 2074 696d 650a  ....import time.
-00000440: 696d 706f 7274 2074 7970 696e 670a 0a66  import typing..f
-00000450: 726f 6d20 6169 6f61 7270 2069 6d70 6f72  rom aioarp impor
-00000460: 7420 5f65 7863 6570 7469 6f6e 7320 6173  t _exceptions as
-00000470: 2065 7863 0a66 726f 6d20 6169 6f61 7270   exc.from aioarp
-00000480: 2e5f 6172 7020 696d 706f 7274 2041 5250  ._arp import ARP
-00000490: 5f48 4541 4445 525f 5349 5a45 2c20 4554  _HEADER_SIZE, ET
-000004a0: 4845 524e 4554 5f48 4541 4445 525f 5349  HERNET_HEADER_SI
-000004b0: 5a45 2c20 4172 7050 6163 6b65 742c 2045  ZE, ArpPacket, E
-000004c0: 7468 5061 636b 6574 2c20 5072 6f74 6f63  thPacket, Protoc
-000004d0: 6f6c 0a66 726f 6d20 6169 6f61 7270 2e5f  ol.from aioarp._
-000004e0: 7574 696c 7320 696d 706f 7274 2069 735f  utils import is_
-000004f0: 7661 6c69 645f 6970 7634 0a66 726f 6d20  valid_ipv4.from 
-00000500: 6169 6f61 7270 2e64 6566 6175 6c74 7320  aioarp.defaults 
-00000510: 696d 706f 7274 2044 4546 4155 4c54 5f52  import DEFAULT_R
-00000520: 4541 445f 5449 4d45 4f55 542c 2044 4546  EAD_TIMEOUT, DEF
-00000530: 4155 4c54 5f52 4550 4c59 5f4d 4953 5349  AULT_REPLY_MISSI
-00000540: 4e47 5f54 494d 452c 2044 4546 4155 4c54  NG_TIME, DEFAULT
-00000550: 5f57 5249 5445 5f54 494d 454f 5554 0a0a  _WRITE_TIMEOUT..
-00000560: 6672 6f6d 2061 696f 6172 7020 696d 706f  from aioarp impo
-00000570: 7274 2053 7472 6561 6d0a 0a5f 5f61 6c6c  rt Stream..__all
-00000580: 5f5f 203d 2028 0a20 2020 2027 7379 6e63  __ = (.    'sync
-00000590: 5f73 656e 645f 6172 7027 2c0a 290a 0a0a  _send_arp',.)...
-000005a0: 6465 6620 7265 6365 6976 655f 6172 7028  def receive_arp(
-000005b0: 736f 636b 3a20 5374 7265 616d 2c20 7469  sock: Stream, ti
-000005c0: 6d65 6f75 743a 2066 6c6f 6174 2920 2d3e  meout: float) ->
-000005d0: 2041 7270 5061 636b 6574 3a0a 2020 2020   ArpPacket:.    
-000005e0: 7374 6172 745f 7469 6d65 203d 2074 696d  start_time = tim
-000005f0: 652e 7469 6d65 2829 0a20 2020 2077 6869  e.time().    whi
-00000600: 6c65 2054 7275 653a 0a0a 2020 2020 2020  le True:..      
-00000610: 2020 2320 4368 6563 6b20 6966 2074 696d    # Check if tim
-00000620: 656f 7574 2077 6173 2065 7870 6972 6564  eout was expired
-00000630: 0a20 2020 2020 2020 2069 6620 7469 6d65  .        if time
-00000640: 2e74 696d 6528 2920 2d20 7374 6172 745f  .time() - start_
-00000650: 7469 6d65 203e 2074 696d 656f 7574 3a0a  time > timeout:.
-00000660: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00000670: 6520 6578 632e 4e6f 7446 6f75 6e64 4572  e exc.NotFoundEr
-00000680: 726f 7228 290a 0a20 2020 2020 2020 2023  ror()..        #
-00000690: 2054 7279 2074 6f20 7265 6164 2066 7261   Try to read fra
-000006a0: 6d65 0a20 2020 2020 2020 2074 7279 3a0a  me.        try:.
-000006b0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-000006c0: 6520 3d20 736f 636b 2e72 6563 6569 7665  e = sock.receive
-000006d0: 5f66 7261 6d65 2874 696d 656f 7574 3d44  _frame(timeout=D
-000006e0: 4546 4155 4c54 5f52 4541 445f 5449 4d45  EFAULT_READ_TIME
-000006f0: 4f55 5429 0a20 2020 2020 2020 2065 7863  OUT).        exc
-00000700: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00000710: 2065 3a20 2023 2070 7261 676d 613a 206e   e:  # pragma: n
-00000720: 6f20 636f 7665 720a 2020 2020 2020 2020  o cover.        
-00000730: 2020 2020 7261 6973 6520 6578 632e 4e6f      raise exc.No
-00000740: 7446 6f75 6e64 4572 726f 7228 2920 6672  tFoundError() fr
-00000750: 6f6d 2065 0a0a 2020 2020 2020 2020 2320  om e..        # 
-00000760: 4578 7472 6163 7420 7468 6520 6574 6865  Extract the ethe
-00000770: 726e 6574 2068 6561 6465 720a 2020 2020  rnet header.    
-00000780: 2020 2020 6574 685f 6865 6164 6572 203d      eth_header =
-00000790: 2066 7261 6d65 5b3a 4554 4845 524e 4554   frame[:ETHERNET
-000007a0: 5f48 4541 4445 525f 5349 5a45 5d0a 0a20  _HEADER_SIZE].. 
-000007b0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-000007c0: 2020 2020 2020 2020 6574 685f 7061 636b          eth_pack
-000007d0: 6574 203d 2045 7468 5061 636b 6574 2e70  et = EthPacket.p
-000007e0: 6172 7365 2865 7468 5f68 6561 6465 7229  arse(eth_header)
-000007f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000800: 6574 685f 7061 636b 6574 2e70 726f 746f  eth_packet.proto
-00000810: 2021 3d20 5072 6f74 6f63 6f6c 2e61 7270   != Protocol.arp
-00000820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000830: 2020 636f 6e74 696e 7565 0a0a 2020 2020    continue..    
-00000840: 2020 2020 2020 2020 6172 705f 7265 7370          arp_resp
-00000850: 6f6e 7365 203d 2041 7270 5061 636b 6574  onse = ArpPacket
-00000860: 2e70 6172 7365 280a 2020 2020 2020 2020  .parse(.        
-00000870: 2020 2020 2020 2020 6672 616d 655b 4554          frame[ET
-00000880: 4845 524e 4554 5f48 4541 4445 525f 5349  HERNET_HEADER_SI
-00000890: 5a45 3a20 4554 4845 524e 4554 5f48 4541  ZE: ETHERNET_HEA
-000008a0: 4445 525f 5349 5a45 202b 2041 5250 5f48  DER_SIZE + ARP_H
-000008b0: 4541 4445 525f 5349 5a45 5d29 0a20 2020  EADER_SIZE]).   
-000008c0: 2020 2020 2020 2020 2069 6620 6973 5f76           if is_v
-000008d0: 616c 6964 5f69 7076 3428 6172 705f 7265  alid_ipv4(arp_re
-000008e0: 7370 6f6e 7365 2e73 656e 6465 725f 6970  sponse.sender_ip
-000008f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00000900: 2020 2072 6574 7572 6e20 6172 705f 7265     return arp_re
-00000910: 7370 6f6e 7365 0a20 2020 2020 2020 2065  sponse.        e
-00000920: 7863 6570 7420 4261 7365 4578 6365 7074  xcept BaseExcept
-00000930: 696f 6e3a 2020 2320 7072 6167 6d61 3a20  ion:  # pragma: 
-00000940: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
-00000950: 2020 2020 2023 2054 4f44 4f3a 2063 6174       # TODO: cat
-00000960: 6368 2063 6f6e 6372 6574 6520 6572 726f  ch concrete erro
-00000970: 7273 0a20 2020 2020 2020 2020 2020 202e  rs.            .
-00000980: 2e2e 0a0a 0a64 6566 2073 796e 635f 7365  .....def sync_se
-00000990: 6e64 5f61 7270 2861 7270 5f70 6163 6b65  nd_arp(arp_packe
-000009a0: 743a 2041 7270 5061 636b 6574 2c0a 2020  t: ArpPacket,.  
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 2020 2020 2073 7472 6561 6d3a 2053         stream: S
-000009d0: 7472 6561 6d2c 0a20 2020 2020 2020 2020  tream,.         
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 7469 6d65 6f75 743a 2074 7970 696e 672e  timeout: typing.
-00000a00: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
-00000a10: 3d20 4e6f 6e65 2920 2d3e 2041 7270 5061  = None) -> ArpPa
-00000a20: 636b 6574 3a0a 2020 2020 6574 6865 726e  cket:.    ethern
-00000a30: 6574 5f70 6163 6b65 7420 3d20 4574 6850  et_packet = EthP
-00000a40: 6163 6b65 7428 0a20 2020 2020 2020 2074  acket(.        t
-00000a50: 6172 6765 745f 6d61 633d 6172 705f 7061  arget_mac=arp_pa
-00000a60: 636b 6574 2e74 6172 6765 745f 6d61 632c  cket.target_mac,
-00000a70: 0a20 2020 2020 2020 2073 656e 6465 725f  .        sender_
-00000a80: 6d61 633d 6172 705f 7061 636b 6574 2e73  mac=arp_packet.s
-00000a90: 656e 6465 725f 6d61 632c 0a20 2020 2020  ender_mac,.     
-00000aa0: 2020 2070 726f 746f 3d50 726f 746f 636f     proto=Protoco
-00000ab0: 6c2e 6172 700a 2020 2020 290a 0a20 2020  l.arp.    )..   
-00000ac0: 2074 7279 3a0a 2020 2020 2020 2020 6672   try:.        fr
-00000ad0: 616d 655f 746f 5f73 656e 6420 3d20 6574  ame_to_send = et
-00000ae0: 6865 726e 6574 5f70 6163 6b65 742e 6275  hernet_packet.bu
-00000af0: 696c 645f 6672 616d 6528 2920 2b20 6172  ild_frame() + ar
-00000b00: 705f 7061 636b 6574 2e62 7569 6c64 5f66  p_packet.build_f
-00000b10: 7261 6d65 2829 0a20 2020 2020 2020 2073  rame().        s
-00000b20: 7472 6561 6d2e 7772 6974 655f 6672 616d  tream.write_fram
-00000b30: 6528 6672 616d 655f 746f 5f73 656e 642c  e(frame_to_send,
-00000b40: 2074 696d 656f 7574 3d44 4546 4155 4c54   timeout=DEFAULT
-00000b50: 5f57 5249 5445 5f54 494d 454f 5554 290a  _WRITE_TIMEOUT).
-00000b60: 2020 2020 6578 6365 7074 2065 7863 2e57      except exc.W
-00000b70: 7269 7465 5469 6d65 6f75 7445 7272 6f72  riteTimeoutError
-00000b80: 2061 7320 653a 2020 2320 7072 6167 6d61   as e:  # pragma
-00000b90: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
-00000ba0: 2020 2072 6169 7365 2065 7863 2e4e 6f74     raise exc.Not
-00000bb0: 466f 756e 6445 7272 6f72 2066 726f 6d20  FoundError from 
-00000bc0: 650a 0a20 2020 2072 6574 7572 6e20 7265  e..    return re
-00000bd0: 6365 6976 655f 6172 7028 7374 7265 616d  ceive_arp(stream
-00000be0: 2c20 7469 6d65 6f75 7420 6f72 2044 4546  , timeout or DEF
-00000bf0: 4155 4c54 5f52 4550 4c59 5f4d 4953 5349  AULT_REPLY_MISSI
-00000c00: 4e47 5f54 494d 4529 0a                   NG_TIME).
+00000000: 696d 706f 7274 2074 696d 650a 696d 706f  import time.impo
+00000010: 7274 2074 7970 696e 670a 0a66 726f 6d20  rt typing..from 
+00000020: 6169 6f61 7270 2069 6d70 6f72 7420 5374  aioarp import St
+00000030: 7265 616d 2c20 5f65 7863 6570 7469 6f6e  ream, _exception
+00000040: 7320 6173 2065 7863 0a66 726f 6d20 6169  s as exc.from ai
+00000050: 6f61 7270 2e5f 6172 7020 696d 706f 7274  oarp._arp import
+00000060: 2041 5250 5f48 4541 4445 525f 5349 5a45   ARP_HEADER_SIZE
+00000070: 2c20 4554 4845 524e 4554 5f48 4541 4445  , ETHERNET_HEADE
+00000080: 525f 5349 5a45 2c20 4172 7050 6163 6b65  R_SIZE, ArpPacke
+00000090: 742c 2045 7468 5061 636b 6574 2c20 5072  t, EthPacket, Pr
+000000a0: 6f74 6f63 6f6c 0a66 726f 6d20 6169 6f61  otocol.from aioa
+000000b0: 7270 2e5f 7574 696c 7320 696d 706f 7274  rp._utils import
+000000c0: 2069 735f 7661 6c69 645f 6970 7634 0a66   is_valid_ipv4.f
+000000d0: 726f 6d20 6169 6f61 7270 2e64 6566 6175  rom aioarp.defau
+000000e0: 6c74 7320 696d 706f 7274 2044 4546 4155  lts import DEFAU
+000000f0: 4c54 5f52 4541 445f 5449 4d45 4f55 542c  LT_READ_TIMEOUT,
+00000100: 2044 4546 4155 4c54 5f52 4550 4c59 5f4d   DEFAULT_REPLY_M
+00000110: 4953 5349 4e47 5f54 494d 452c 2044 4546  ISSING_TIME, DEF
+00000120: 4155 4c54 5f57 5249 5445 5f54 494d 454f  AULT_WRITE_TIMEO
+00000130: 5554 0a0a 5f5f 616c 6c5f 5f20 3d20 280a  UT..__all__ = (.
+00000140: 2020 2020 2773 796e 635f 7365 6e64 5f61      'sync_send_a
+00000150: 7270 272c 0a29 0a0a 0a64 6566 2072 6563  rp',.)...def rec
+00000160: 6569 7665 5f61 7270 2873 6f63 6b3a 2053  eive_arp(sock: S
+00000170: 7472 6561 6d2c 2074 696d 656f 7574 3a20  tream, timeout: 
+00000180: 666c 6f61 7429 202d 3e20 4172 7050 6163  float) -> ArpPac
+00000190: 6b65 743a 0a20 2020 2073 7461 7274 5f74  ket:.    start_t
+000001a0: 696d 6520 3d20 7469 6d65 2e74 696d 6528  ime = time.time(
+000001b0: 290a 2020 2020 7768 696c 6520 5472 7565  ).    while True
+000001c0: 3a0a 0a20 2020 2020 2020 2023 2043 6865  :..        # Che
+000001d0: 636b 2069 6620 7469 6d65 6f75 7420 7761  ck if timeout wa
+000001e0: 7320 6578 7069 7265 640a 2020 2020 2020  s expired.      
+000001f0: 2020 6966 2074 696d 652e 7469 6d65 2829    if time.time()
+00000200: 202d 2073 7461 7274 5f74 696d 6520 3e20   - start_time > 
+00000210: 7469 6d65 6f75 743a 0a20 2020 2020 2020  timeout:.       
+00000220: 2020 2020 2072 6169 7365 2065 7863 2e4e       raise exc.N
+00000230: 6f74 466f 756e 6445 7272 6f72 2829 0a0a  otFoundError()..
+00000240: 2020 2020 2020 2020 2320 5472 7920 746f          # Try to
+00000250: 2072 6561 6420 6672 616d 650a 2020 2020   read frame.    
+00000260: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00000270: 2020 2020 2066 7261 6d65 203d 2073 6f63       frame = soc
+00000280: 6b2e 7265 6365 6976 655f 6672 616d 6528  k.receive_frame(
+00000290: 7469 6d65 6f75 743d 4445 4641 554c 545f  timeout=DEFAULT_
+000002a0: 5245 4144 5f54 494d 454f 5554 290a 2020  READ_TIMEOUT).  
+000002b0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+000002c0: 6570 7469 6f6e 2061 7320 653a 2020 2320  eption as e:  # 
+000002d0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+000002e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000002f0: 7365 2065 7863 2e4e 6f74 466f 756e 6445  se exc.NotFoundE
+00000300: 7272 6f72 2829 2066 726f 6d20 650a 0a20  rror() from e.. 
+00000310: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
+00000320: 2074 6865 2065 7468 6572 6e65 7420 6865   the ethernet he
+00000330: 6164 6572 0a20 2020 2020 2020 2065 7468  ader.        eth
+00000340: 5f68 6561 6465 7220 3d20 6672 616d 655b  _header = frame[
+00000350: 3a45 5448 4552 4e45 545f 4845 4144 4552  :ETHERNET_HEADER
+00000360: 5f53 495a 455d 0a0a 2020 2020 2020 2020  _SIZE]..        
+00000370: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00000380: 2065 7468 5f70 6163 6b65 7420 3d20 4574   eth_packet = Et
+00000390: 6850 6163 6b65 742e 7061 7273 6528 6574  hPacket.parse(et
+000003a0: 685f 6865 6164 6572 290a 2020 2020 2020  h_header).      
+000003b0: 2020 2020 2020 6966 2065 7468 5f70 6163        if eth_pac
+000003c0: 6b65 742e 7072 6f74 6f20 213d 2050 726f  ket.proto != Pro
+000003d0: 746f 636f 6c2e 6172 703a 0a20 2020 2020  tocol.arp:.     
+000003e0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+000003f0: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
+00000400: 2061 7270 5f72 6573 706f 6e73 6520 3d20   arp_response = 
+00000410: 4172 7050 6163 6b65 742e 7061 7273 6528  ArpPacket.parse(
+00000420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000430: 2066 7261 6d65 5b45 5448 4552 4e45 545f   frame[ETHERNET_
+00000440: 4845 4144 4552 5f53 495a 453a 2045 5448  HEADER_SIZE: ETH
+00000450: 4552 4e45 545f 4845 4144 4552 5f53 495a  ERNET_HEADER_SIZ
+00000460: 4520 2b20 4152 505f 4845 4144 4552 5f53  E + ARP_HEADER_S
+00000470: 495a 455d 290a 2020 2020 2020 2020 2020  IZE]).          
+00000480: 2020 6966 2069 735f 7661 6c69 645f 6970    if is_valid_ip
+00000490: 7634 2861 7270 5f72 6573 706f 6e73 652e  v4(arp_response.
+000004a0: 7365 6e64 6572 5f69 7029 3a0a 2020 2020  sender_ip):.    
+000004b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000004c0: 726e 2061 7270 5f72 6573 706f 6e73 650a  rn arp_response.
+000004d0: 2020 2020 2020 2020 6578 6365 7074 2042          except B
+000004e0: 6173 6545 7863 6570 7469 6f6e 3a20 2023  aseException:  #
+000004f0: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+00000500: 720a 2020 2020 2020 2020 2020 2020 2320  r.            # 
+00000510: 544f 444f 3a20 6361 7463 6820 636f 6e63  TODO: catch conc
+00000520: 7265 7465 2065 7272 6f72 730a 2020 2020  rete errors.    
+00000530: 2020 2020 2020 2020 2e2e 2e0a 0a0a 6465          ......de
+00000540: 6620 7379 6e63 5f73 656e 645f 6172 7028  f sync_send_arp(
+00000550: 6172 705f 7061 636b 6574 3a20 4172 7050  arp_packet: ArpP
+00000560: 6163 6b65 742c 0a20 2020 2020 2020 2020  acket,.         
+00000570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000580: 7374 7265 616d 3a20 5374 7265 616d 2c0a  stream: Stream,.
+00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005a0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+000005b0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000005c0: 6c5b 666c 6f61 745d 203d 204e 6f6e 6529  l[float] = None)
+000005d0: 202d 3e20 4172 7050 6163 6b65 743a 0a20   -> ArpPacket:. 
+000005e0: 2020 2065 7468 6572 6e65 745f 7061 636b     ethernet_pack
+000005f0: 6574 203d 2045 7468 5061 636b 6574 280a  et = EthPacket(.
+00000600: 2020 2020 2020 2020 7461 7267 6574 5f6d          target_m
+00000610: 6163 3d61 7270 5f70 6163 6b65 742e 7461  ac=arp_packet.ta
+00000620: 7267 6574 5f6d 6163 2c0a 2020 2020 2020  rget_mac,.      
+00000630: 2020 7365 6e64 6572 5f6d 6163 3d61 7270    sender_mac=arp
+00000640: 5f70 6163 6b65 742e 7365 6e64 6572 5f6d  _packet.sender_m
+00000650: 6163 2c0a 2020 2020 2020 2020 7072 6f74  ac,.        prot
+00000660: 6f3d 5072 6f74 6f63 6f6c 2e61 7270 0a20  o=Protocol.arp. 
+00000670: 2020 2029 0a0a 2020 2020 7472 793a 0a20     )..    try:. 
+00000680: 2020 2020 2020 2066 7261 6d65 5f74 6f5f         frame_to_
+00000690: 7365 6e64 203d 2065 7468 6572 6e65 745f  send = ethernet_
+000006a0: 7061 636b 6574 2e62 7569 6c64 5f66 7261  packet.build_fra
+000006b0: 6d65 2829 202b 2061 7270 5f70 6163 6b65  me() + arp_packe
+000006c0: 742e 6275 696c 645f 6672 616d 6528 290a  t.build_frame().
+000006d0: 2020 2020 2020 2020 7374 7265 616d 2e77          stream.w
+000006e0: 7269 7465 5f66 7261 6d65 2866 7261 6d65  rite_frame(frame
+000006f0: 5f74 6f5f 7365 6e64 2c20 7469 6d65 6f75  _to_send, timeou
+00000700: 743d 4445 4641 554c 545f 5752 4954 455f  t=DEFAULT_WRITE_
+00000710: 5449 4d45 4f55 5429 0a20 2020 2065 7863  TIMEOUT).    exc
+00000720: 6570 7420 6578 632e 5772 6974 6554 696d  ept exc.WriteTim
+00000730: 656f 7574 4572 726f 7220 6173 2065 3a20  eoutError as e: 
+00000740: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+00000750: 7665 720a 2020 2020 2020 2020 7261 6973  ver.        rais
+00000760: 6520 6578 632e 4e6f 7446 6f75 6e64 4572  e exc.NotFoundEr
+00000770: 726f 7220 6672 6f6d 2065 0a0a 2020 2020  ror from e..    
+00000780: 7265 7475 726e 2072 6563 6569 7665 5f61  return receive_a
+00000790: 7270 2873 7472 6561 6d2c 2074 696d 656f  rp(stream, timeo
+000007a0: 7574 206f 7220 4445 4641 554c 545f 5245  ut or DEFAULT_RE
+000007b0: 504c 595f 4d49 5353 494e 475f 5449 4d45  PLY_MISSING_TIME
+000007c0: 290a                                     ).
```

### Comparing `aioarp-0.0.4/aioarp/_backends/_mock.py` & `aioarp-0.0.5/aioarp/_backends/_mock.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/tests/test_async.py` & `aioarp-0.0.5/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/tests/test_client.py` & `aioarp-0.0.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/tests/test_proto.py` & `aioarp-0.0.5/tests/test_proto.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/tests/test_sync.py` & `aioarp-0.0.5/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/.gitignore` & `aioarp-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/LICENSE.txt` & `aioarp-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/README.md` & `aioarp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.4/pyproject.toml` & `aioarp-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,23 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "anyio==3.6.2",
   "typing_extensions==4.6.3"
 ]
 
+[project.optional-dependencies]
+
+cli = [
+  "typer==0.9.0"
+]
+
+[project.scripts]
+aioarp = "aioarp._cli:app"
+
 [project.urls]
 Documentation = "https://github.com/karosis88/aioarp#readme"
 Issues = "https://github.com/karosis88/aioarp/issues"
 Source = "https://github.com/karosis88/aioarp"
 
 [tool.hatch.version]
 path = "aioarp/__about__.py"
@@ -44,15 +53,15 @@
 
 [tool.ruff.isort]
 combine-as-imports = true
 
 [tool.mypy]
 ignore_missing_imports = true
 strict = true
-exclude = ["unasync.py", "_mock.py"]
+exclude = ["unasync.py", "_mock.py", "aioarp/_cli.py"]
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 disallow_untyped_defs = false
 check_untyped_defs = true
 
 [tool.coverage.report]
```

### Comparing `aioarp-0.0.4/PKG-INFO` & `aioarp-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioarp
-Version: 0.0.4
+Version: 0.0.5
 Summary: Aioarp is a ARP protocol implementation that provides synchronous and asynchronous interfaces and gives you complete control over how ARP packets are sent.
 Project-URL: Documentation, https://github.com/karosis88/aioarp#readme
 Project-URL: Issues, https://github.com/karosis88/aioarp/issues
 Project-URL: Source, https://github.com/karosis88/aioarp
 Author-email: Karen Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: anyio==3.6.2
 Requires-Dist: typing-extensions==4.6.3
+Provides-Extra: cli
+Requires-Dist: typer==0.9.0; extra == 'cli'
 Description-Content-Type: text/markdown
 
 # aioarp
 
 [![PyPI - Version](https://img.shields.io/pypi/v/aioarp.svg)](https://pypi.org/project/aioarp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aioarp.svg)](https://pypi.org/project/aioarp)
 [![coverage](https://img.shields.io/codecov/c/github/karosis88/aioarp/master)](https://app.codecov.io/gh/karosis88/aioarp)
```

