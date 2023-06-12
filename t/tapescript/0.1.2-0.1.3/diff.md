# Comparing `tmp/tapescript-0.1.2.tar.gz` & `tmp/tapescript-0.1.3.tar.gz`

## Comparing `tapescript-0.1.2.tar` & `tapescript-0.1.3.tar`

### file list

```diff
@@ -1,977 +1,977 @@
--rw-r--r--   0        0        0    58563 2020-02-02 00:00:00.000000 tapescript-0.1.2/docs.md
--rw-r--r--   0        0        0    57325 2020-02-02 00:00:00.000000 tapescript-0.1.2/dox.md
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 tapescript-0.1.2/dox.py
--rw-r--r--   0        0        0    16878 2020-02-02 00:00:00.000000 tapescript-0.1.2/language_spec.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tapescript-0.1.2/requirements.txt
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 tapescript-0.1.2/script_examples.md
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/.gitignore
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/pyvenv.cfg
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/_tapescript.pth
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/LICENSE
--rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/METADATA
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/REQUESTED
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/WHEEL
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/autodox/__init__.py
--rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/autodox/functions.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/METADATA
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/WHEEL
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/licenses/license
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/__init__.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/_cffi_errors.h
--rw-r--r--   0        0        0    15185 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/_cffi_include.h
--rw-r--r--   0        0        0    18208 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/_embedding.h
--rw-r--r--   0        0        0    43029 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/api.py
--rw-r--r--   0        0        0    43575 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/backend_ctypes.py
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/cffi_opcode.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/commontypes.py
--rw-r--r--   0        0        0    45237 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/cparser.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/error.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/ffiplatform.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/lock.py
--rw-r--r--   0        0        0    22385 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/model.py
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/parse_c_type.h
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/pkgconfig.py
--rw-r--r--   0        0        0    66179 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/recompiler.py
--rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/setuptools_ext.py
--rw-r--r--   0        0        0    44396 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/vengine_cpy.py
--rw-r--r--   0        0        0    27359 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/vengine_gen.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi/verifier.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/METADATA
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/REQUESTED
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/WHEEL
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/top_level.txt
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/__init__.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/encoding.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/exceptions.py
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/hash.py
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/hashlib.py
--rw-r--r--   0        0        0    15215 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/public.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/py.typed
--rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/secret.py
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/signing.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/utils.py
--rw-r--r--   0        0        0    17448 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/__init__.py
--rw-r--r--   0        0        0    16156 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_aead.py
--rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_box.py
--rw-r--r--   0        0        0    14148 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_core.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_generichash.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_hash.py
--rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_kx.py
--rw-r--r--   0        0        0    19448 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_pwhash.py
--rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_scalarmult.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_secretbox.py
--rw-r--r--   0        0        0    11522 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_secretstream.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_shorthash.py
--rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_sign.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/randombytes.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/sodium_core.py
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/utils.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/__init__.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/_argon2.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/argon2i.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/argon2id.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/scrypt.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/py.typed
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18328 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28722 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    18817 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20435 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18442 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    27696 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27475 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    32782 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    18864 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0    84101 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109388 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    32064 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35601 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    71556 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53572 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99195 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35153 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39128 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/METADATA
--rw-r--r--   0        0        0    77162 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/top_level.txt
--rw-r--r--   0        0        0   108568 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   132569 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    18410 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/__init__.py
--rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/_ast_gen.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/_build_tables.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/_c_ast.cfg
--rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ast_transforms.py
--rw-r--r--   0        0        0    31445 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/c_ast.py
--rw-r--r--   0        0        0    17772 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/c_generator.py
--rw-r--r--   0        0        0    17167 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/c_lexer.py
--rw-r--r--   0        0        0    73680 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/c_parser.py
--rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/lextab.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/plyparser.py
--rw-r--r--   0        0        0   205652 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/yacctab.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/__init__.py
--rw-r--r--   0        0        0    33282 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/cpp.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/ctokens.py
--rw-r--r--   0        0        0    42918 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/lex.py
--rw-r--r--   0        0        0   137323 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/yacc.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/ygen.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/INSTALLER
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/LICENSE
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/METADATA
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/WHEEL
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/top_level.txt
--rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_entry_points.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_importlib.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_itertools.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_path.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_reqs.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    19539 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0   137216 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/cli-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    20799 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/discovery.py
--rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0   137728 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/gui-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/logging.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    47724 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    40020 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/py34compat.py
--rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14789 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    47369 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    17973 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    50186 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    13713 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    30235 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23602 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    18858 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    22051 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    31558 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    16568 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    30221 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0        0        0    30130 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    16623 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/build.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    14115 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    85662 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    31188 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0        0        0    26795 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/__init__.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0        0        0    16319 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/expand.py
--rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0        0        0    25198 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0        0        0   269900 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/METADATA
--rw-r--r--   0        0        0    37694 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/WHEEL
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/METADATA
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/direct_url.json
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/licenses/license
--rw-r--r--   0        0        0    24167 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/activate
--rwxr-xr-x   0        0        0     1021 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/activate.bat
--rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/autodox.exe
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   108428 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108428 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/pip3.10.exe
--rwxr-xr-x   0        0        0   108428 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/pip3.11.exe
--rwxr-xr-x   0        0        0   108428 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   268152 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/python.exe
--rwxr-xr-x   0        0        0   256384 2020-02-02 00:00:00.000000 tapescript-0.1.2/.venv/Scripts/pythonw.exe
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tapescript-0.1.2/tapescript/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 tapescript-0.1.2/tapescript/classes.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 tapescript-0.1.2/tapescript/errors.py
--rw-r--r--   0        0        0    43820 2020-02-02 00:00:00.000000 tapescript-0.1.2/tapescript/functions.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 tapescript-0.1.2/tapescript/interfaces.py
--rw-r--r--   0        0        0    34849 2020-02-02 00:00:00.000000 tapescript-0.1.2/tapescript/parsing.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 tapescript-0.1.2/tapescript/tools.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/context.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/test_classes.py
--rw-r--r--   0        0        0    78468 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/test_functions.py
--rw-r--r--   0        0        0    23975 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/test_parsing.py
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/test_tools.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/1.hex
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/1.src
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/2.hex
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/2.src
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/2_decompiled.src
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/3.hex
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/3.src
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/3_decompiled.src
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/4.hex
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/4.src
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/4_decompiled.src
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/5.hex
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/5.src
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/5_decompiled.src
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/6.hex
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/6.src
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/6_decompiled.src
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/branching_e2e.hex
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/branching_e2e.src
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/branching_e2e_decompiled.src
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_committed_script.hex
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_committed_script.src
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_committed_script_decompiled.src
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_locking_script.hex
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_locking_script.src
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_locking_script_decompiled.src
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_unlocking_script1.hex
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_unlocking_script1.src
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_unlocking_script1_decompiled.src
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_unlocking_script2.hex
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_unlocking_script2.src
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_unlocking_script2_decompiled.src
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_unlocking_script3.hex
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_unlocking_script3.src
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/cds_unlocking_script3_decompiled.src
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_committed_script.hex
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_committed_script.src
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_committed_script_decompiled.src
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_locking_script.hex
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_locking_script.src
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_locking_script_decompiled.src
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_unlocking_script1.hex
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_unlocking_script1.src
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_unlocking_script1_decompiled.src
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_unlocking_script2.hex
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_unlocking_script2.src
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/correspondent_unlocking_script2_decompiled.src
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_a.hex
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_a.src
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_a_decompiled.src
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_b.hex
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_b.src
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_ba.hex
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_ba.src
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_ba_decompiled.src
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_bb.hex
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_bb.src
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_committed_script_bb_decompiled.src
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_locking_script.hex
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_locking_script.src
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_unlocking_script_a.hex
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_unlocking_script_a.src
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_unlocking_script_a_decompiled.src
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_unlocking_script_ba.hex
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_unlocking_script_ba.src
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_unlocking_script_ba_decompiled.src
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_unlocking_script_bb.hex
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_unlocking_script_bb.src
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/merkleval_unlocking_script_bb_decompiled.src
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/omega_e2e.hex
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/omega_e2e.src
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/omega_e2e_decompiled.src
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2pk_locking_script.hex
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2pk_locking_script.src
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2pk_locking_script_decompiled.src
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2pk_unlocking_script1.hex
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2pk_unlocking_script1.src
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2pk_unlocking_script1_decompiled.src
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2pk_unlocking_script2.hex
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2pk_unlocking_script2.src
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2pk_unlocking_script2_decompiled.src
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2sh_committed_script.hex
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2sh_committed_script.src
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2sh_committed_script_decompiled.src
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2sh_locking_script.hex
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2sh_locking_script.src
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2sh_locking_script_decompiled.src
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2sh_unlocking_script.hex
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2sh_unlocking_script.src
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 tapescript-0.1.2/tests/vectors/p2sh_unlocking_script_decompiled.src
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tapescript-0.1.2/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tapescript-0.1.2/license
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 tapescript-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 tapescript-0.1.2/readme.md
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 tapescript-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    58563 2020-02-02 00:00:00.000000 tapescript-0.1.3/docs.md
+-rw-r--r--   0        0        0    57325 2020-02-02 00:00:00.000000 tapescript-0.1.3/dox.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 tapescript-0.1.3/dox.py
+-rw-r--r--   0        0        0    16878 2020-02-02 00:00:00.000000 tapescript-0.1.3/language_spec.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tapescript-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 tapescript-0.1.3/script_examples.md
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/.gitignore
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/_tapescript.pth
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/METADATA
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/autodox/__init__.py
+-rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/autodox/functions.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/METADATA
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/licenses/license
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/__init__.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/_cffi_errors.h
+-rw-r--r--   0        0        0    15185 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/_cffi_include.h
+-rw-r--r--   0        0        0    18208 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/_embedding.h
+-rw-r--r--   0        0        0    43029 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/api.py
+-rw-r--r--   0        0        0    43575 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/backend_ctypes.py
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/cffi_opcode.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/commontypes.py
+-rw-r--r--   0        0        0    45237 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/cparser.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/error.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/ffiplatform.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/lock.py
+-rw-r--r--   0        0        0    22385 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/model.py
+-rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/parse_c_type.h
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/pkgconfig.py
+-rw-r--r--   0        0        0    66179 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/recompiler.py
+-rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/setuptools_ext.py
+-rw-r--r--   0        0        0    44396 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/vengine_cpy.py
+-rw-r--r--   0        0        0    27359 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/vengine_gen.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi/verifier.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/__init__.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/encoding.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/exceptions.py
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/hash.py
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/hashlib.py
+-rw-r--r--   0        0        0    15215 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/public.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/py.typed
+-rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/secret.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/signing.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/utils.py
+-rw-r--r--   0        0        0    17448 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/__init__.py
+-rw-r--r--   0        0        0    16156 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_aead.py
+-rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_box.py
+-rw-r--r--   0        0        0    14148 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_core.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_generichash.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_hash.py
+-rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_kx.py
+-rw-r--r--   0        0        0    19448 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_pwhash.py
+-rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_scalarmult.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_secretbox.py
+-rw-r--r--   0        0        0    11522 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_secretstream.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_shorthash.py
+-rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_sign.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/randombytes.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/sodium_core.py
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/utils.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/__init__.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/_argon2.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/argon2i.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/argon2id.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/scrypt.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18328 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28722 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    18817 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20435 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18442 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    27696 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27475 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    32782 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    18864 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    84101 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/t32.exe
+-rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/w32.exe
+-rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109388 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    32064 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35601 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    71556 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53572 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99195 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35153 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39128 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0    77162 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0   108568 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   132569 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    18410 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/__init__.py
+-rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/_ast_gen.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/_build_tables.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/_c_ast.cfg
+-rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ast_transforms.py
+-rw-r--r--   0        0        0    31445 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/c_ast.py
+-rw-r--r--   0        0        0    17772 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/c_generator.py
+-rw-r--r--   0        0        0    17167 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/c_lexer.py
+-rw-r--r--   0        0        0    73680 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/c_parser.py
+-rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/lextab.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/plyparser.py
+-rw-r--r--   0        0        0   205652 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/yacctab.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/__init__.py
+-rw-r--r--   0        0        0    33282 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/cpp.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/ctokens.py
+-rw-r--r--   0        0        0    42918 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/lex.py
+-rw-r--r--   0        0        0   137323 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/yacc.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/ygen.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/LICENSE
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/METADATA
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/WHEEL
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/top_level.txt
+-rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_importlib.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_itertools.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_path.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_reqs.py
+-rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    19539 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/build_meta.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/cli-32.exe
+-rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/cli-64.exe
+-rwxr-xr-x   0        0        0   137216 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/cli-arm64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    20799 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/discovery.py
+-rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/glob.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/gui-32.exe
+-rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/gui-64.exe
+-rwxr-xr-x   0        0        0   137728 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/gui-arm64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/logging.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    47724 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    40020 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14789 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    47369 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    17973 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50186 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13713 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30235 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23602 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    18858 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    22051 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31558 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    16568 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    30221 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0        0        0    30130 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16623 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/build.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0    14115 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    85662 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    31188 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0        0        0    26795 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+-rw-r--r--   0        0        0    16319 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/expand.py
+-rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0        0        0    25198 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0        0        0   269900 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/METADATA
+-rw-r--r--   0        0        0    37694 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/direct_url.json
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/licenses/license
+-rw-r--r--   0        0        0    24167 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/activate
+-rwxr-xr-x   0        0        0     1021 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/activate.bat
+-rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/autodox.exe
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/deactivate.bat
+-rwxr-xr-x   0        0        0   108428 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/pip.exe
+-rwxr-xr-x   0        0        0   108428 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/pip3.10.exe
+-rwxr-xr-x   0        0        0   108428 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/pip3.11.exe
+-rwxr-xr-x   0        0        0   108428 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/pip3.exe
+-rwxr-xr-x   0        0        0   268152 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/python.exe
+-rwxr-xr-x   0        0        0   256384 2020-02-02 00:00:00.000000 tapescript-0.1.3/.venv/Scripts/pythonw.exe
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tapescript-0.1.3/tapescript/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 tapescript-0.1.3/tapescript/classes.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 tapescript-0.1.3/tapescript/errors.py
+-rw-r--r--   0        0        0    43820 2020-02-02 00:00:00.000000 tapescript-0.1.3/tapescript/functions.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 tapescript-0.1.3/tapescript/interfaces.py
+-rw-r--r--   0        0        0    34849 2020-02-02 00:00:00.000000 tapescript-0.1.3/tapescript/parsing.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 tapescript-0.1.3/tapescript/tools.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/context.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/test_classes.py
+-rw-r--r--   0        0        0    78468 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/test_functions.py
+-rw-r--r--   0        0        0    23975 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/test_parsing.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/test_tools.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/1.hex
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/1.src
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/2.hex
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/2.src
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/2_decompiled.src
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/3.hex
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/3.src
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/3_decompiled.src
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/4.hex
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/4.src
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/4_decompiled.src
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/5.hex
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/5.src
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/5_decompiled.src
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/6.hex
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/6.src
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/6_decompiled.src
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/branching_e2e.hex
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/branching_e2e.src
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/branching_e2e_decompiled.src
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_committed_script.hex
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_committed_script.src
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_committed_script_decompiled.src
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_locking_script.hex
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_locking_script.src
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_locking_script_decompiled.src
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_unlocking_script1.hex
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_unlocking_script1.src
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_unlocking_script1_decompiled.src
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_unlocking_script2.hex
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_unlocking_script2.src
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_unlocking_script2_decompiled.src
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_unlocking_script3.hex
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_unlocking_script3.src
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/cds_unlocking_script3_decompiled.src
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_committed_script.hex
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_committed_script.src
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_committed_script_decompiled.src
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_locking_script.hex
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_locking_script.src
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_locking_script_decompiled.src
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_unlocking_script1.hex
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_unlocking_script1.src
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_unlocking_script1_decompiled.src
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_unlocking_script2.hex
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_unlocking_script2.src
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/correspondent_unlocking_script2_decompiled.src
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_a.hex
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_a.src
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_a_decompiled.src
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_b.hex
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_b.src
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_ba.hex
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_ba.src
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_ba_decompiled.src
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_bb.hex
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_bb.src
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_committed_script_bb_decompiled.src
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_locking_script.hex
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_locking_script.src
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_unlocking_script_a.hex
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_unlocking_script_a.src
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_unlocking_script_a_decompiled.src
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_unlocking_script_ba.hex
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_unlocking_script_ba.src
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_unlocking_script_ba_decompiled.src
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_unlocking_script_bb.hex
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_unlocking_script_bb.src
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/merkleval_unlocking_script_bb_decompiled.src
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/omega_e2e.hex
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/omega_e2e.src
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/omega_e2e_decompiled.src
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2pk_locking_script.hex
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2pk_locking_script.src
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2pk_locking_script_decompiled.src
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2pk_unlocking_script1.hex
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2pk_unlocking_script1.src
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2pk_unlocking_script1_decompiled.src
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2pk_unlocking_script2.hex
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2pk_unlocking_script2.src
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2pk_unlocking_script2_decompiled.src
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2sh_committed_script.hex
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2sh_committed_script.src
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2sh_committed_script_decompiled.src
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2sh_locking_script.hex
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2sh_locking_script.src
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2sh_locking_script_decompiled.src
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2sh_unlocking_script.hex
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2sh_unlocking_script.src
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 tapescript-0.1.3/tests/vectors/p2sh_unlocking_script_decompiled.src
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tapescript-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tapescript-0.1.3/license
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 tapescript-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 tapescript-0.1.3/readme.md
+-rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 tapescript-0.1.3/PKG-INFO
```

### Comparing `tapescript-0.1.2/docs.md` & `tapescript-0.1.3/docs.md`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/dox.md` & `tapescript-0.1.3/dox.md`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/dox.py` & `tapescript-0.1.3/dox.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/language_spec.md` & `tapescript-0.1.3/language_spec.md`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/script_examples.md` & `tapescript-0.1.3/script_examples.md`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/LICENSE` & `tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/METADATA` & `tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/RECORD` & `tapescript-0.1.3/.venv/Lib/site-packages/PyNaCl-1.5.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/_distutils_hack/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/autodox/functions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/autodox/functions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/METADATA` & `tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/RECORD` & `tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/licenses/license` & `tapescript-0.1.3/.venv/Lib/site-packages/autodox-0.0.3.1.dist-info/licenses/license`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/_cffi_errors.h` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/_cffi_errors.h`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/_cffi_include.h` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/_cffi_include.h`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/_embedding.h` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/_embedding.h`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/api.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/api.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/backend_ctypes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/backend_ctypes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/cffi_opcode.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/cffi_opcode.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/commontypes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/commontypes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/cparser.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/cparser.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/error.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/error.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/ffiplatform.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/ffiplatform.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/lock.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/lock.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/model.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/model.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/parse_c_type.h` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/parse_c_type.h`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/pkgconfig.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/recompiler.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/recompiler.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/setuptools_ext.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/setuptools_ext.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/vengine_cpy.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/vengine_cpy.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/vengine_gen.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/vengine_gen.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi/verifier.py` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi/verifier.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/LICENSE` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/METADATA` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/cffi-1.15.1.dist-info/RECORD` & `tapescript-0.1.3/.venv/Lib/site-packages/cffi-1.15.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/encoding.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/encoding.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/exceptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/hash.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/hash.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/hashlib.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/hashlib.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/public.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/public.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/secret.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/secret.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/signing.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/signing.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_aead.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_aead.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_box.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_box.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_core.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_core.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_generichash.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_generichash.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_hash.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_hash.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_kx.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_kx.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_pwhash.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_pwhash.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_scalarmult.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_scalarmult.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_secretbox.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_secretbox.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_secretstream.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_secretstream.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_shorthash.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_shorthash.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/crypto_sign.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/crypto_sign.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/randombytes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/randombytes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/sodium_core.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/sodium_core.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/bindings/utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/bindings/utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/_argon2.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/_argon2.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/argon2i.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/argon2i.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/argon2id.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/argon2id.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/nacl/pwhash/scrypt.py` & `tapescript-0.1.3/.venv/Lib/site-packages/nacl/pwhash/scrypt.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/__main__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/__pip-runner__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/build_env.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cache.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/configuration.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/exceptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/pyproject.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/wheel_builder.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/base_command.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/command_context.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/main.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/parser.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/req_command.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/cli/spinners.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/cache.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/check.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/completion.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/configuration.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/debug.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/download.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/freeze.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/hash.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/help.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/index.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/inspect.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/install.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/list.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/search.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/show.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/commands/wheel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/base.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/installed.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/index/collector.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/index/package_finder.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/index/sources.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/locations/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/locations/base.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/_json.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/base.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/candidate.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/direct_url.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/format_control.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/index.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/installation_report.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/link.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/scheme.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/search_scope.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/target_python.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/models/wheel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/auth.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/cache.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/download.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/session.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/check.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/freeze.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/prepare.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/constructors.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/req_file.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/req_install.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/req_set.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/base.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/_log.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/encoding.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/glibc.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/hashes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/logging.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/misc.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/models.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/packaging.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/urls.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/utils/wheel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/git.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/six.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/certifi/core.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/database.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/index.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/t32.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/t64.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/version.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/w32.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/w64.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/distro/distro.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/codec.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/core.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/packaging/version.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/console.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/style.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/token.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/api.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/auth.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/certs.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/help.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/models.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/packages.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/structures.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/requests/utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/abc.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/align.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/bar.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/box.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/cells.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/color.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/columns.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/console.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/containers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/control.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/errors.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/json.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/layout.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/live.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/logging.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/markup.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/measure.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/padding.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/pager.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/palette.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/panel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/progress.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/repr.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/rule.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/scope.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/screen.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/segment.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/status.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/style.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/styled.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/table.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/text.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/theme.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/rich/tree.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt` & `tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt` & `tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/METADATA` & `tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pip-23.1.2.dist-info/RECORD` & `tapescript-0.1.3/.venv/Lib/site-packages/pip-23.1.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/zipp.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pkg_resources/extern/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/_ast_gen.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/_ast_gen.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/_build_tables.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/_build_tables.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/_c_ast.cfg` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/_c_ast.cfg`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ast_transforms.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ast_transforms.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/c_ast.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/c_ast.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/c_generator.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/c_generator.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/c_lexer.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/c_lexer.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/c_parser.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/c_parser.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/lextab.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/lextab.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/plyparser.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/plyparser.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/yacctab.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/yacctab.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/cpp.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/ctokens.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/lex.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/lex.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/yacc.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser/ply/ygen.py` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/LICENSE` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/METADATA` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/pycparser-2.21.dist-info/RECORD` & `tapescript-0.1.3/.venv/Lib/site-packages/pycparser-2.21.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_entry_points.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_imp.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_importlib.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_itertools.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_path.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/archive_util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/build_meta.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/cli-32.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/cli-64.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/cli-arm64.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/cli-arm64.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/cli.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/dep_util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/depends.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/discovery.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/dist.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/errors.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/extension.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/glob.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/gui-32.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/gui-64.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/gui-arm64.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/gui-arm64.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/gui.exe` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/installer.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/launch.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/logging.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/monkey.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/msvc.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/namespaces.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/package_index.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/sandbox.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/unicode_utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/wheel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/windows_support.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/_collections.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/archive_util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/ccompiler.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/cmd.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/config.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/core.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/dep_util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/dir_util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/dist.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/errors.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/extension.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/file_util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/filelist.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/log.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/py39compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/spawn.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/sysconfig.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/text_file.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/version.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/bdist.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_py.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/check.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/clean.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/config.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_data.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/register.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/sdist.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_distutils/command/upload.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/ordered_set.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/zipp.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/version.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/alias.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/bdist_egg.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/bdist_rpm.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/build.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/build_clib.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/build_ext.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/build_py.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/develop.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/dist_info.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/easy_install.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/editable_wheel.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/egg_info.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/install.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/install_egg_info.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/install_lib.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/install_scripts.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/launcher manifest.xml` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/py36compat.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/rotate.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/saveopts.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/sdist.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/setopt.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/test.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/command/upload_docs.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/expand.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/pyprojecttoml.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/setupcfg.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools/extern/__init__.py` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/LICENSE` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/METADATA` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/RECORD` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt` & `tapescript-0.1.3/.venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/METADATA` & `tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/RECORD` & `tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/licenses/license` & `tapescript-0.1.3/.venv/Lib/site-packages/tapescript-0.0.1.dist-info/licenses/license`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/Activate.ps1` & `tapescript-0.1.3/.venv/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/activate` & `tapescript-0.1.3/.venv/Scripts/activate`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/activate.bat` & `tapescript-0.1.3/.venv/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/autodox.exe` & `tapescript-0.1.3/.venv/Scripts/autodox.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/pip.exe` & `tapescript-0.1.3/.venv/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/pip3.10.exe` & `tapescript-0.1.3/.venv/Scripts/pip3.10.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/pip3.11.exe` & `tapescript-0.1.3/.venv/Scripts/pip3.11.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/pip3.exe` & `tapescript-0.1.3/.venv/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/python.exe` & `tapescript-0.1.3/.venv/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/.venv/Scripts/pythonw.exe` & `tapescript-0.1.3/.venv/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tapescript/classes.py` & `tapescript-0.1.3/tapescript/classes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tapescript/errors.py` & `tapescript-0.1.3/tapescript/errors.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tapescript/functions.py` & `tapescript-0.1.3/tapescript/functions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tapescript/interfaces.py` & `tapescript-0.1.3/tapescript/interfaces.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tapescript/parsing.py` & `tapescript-0.1.3/tapescript/parsing.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tapescript/tools.py` & `tapescript-0.1.3/tapescript/tools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/test_classes.py` & `tapescript-0.1.3/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/test_functions.py` & `tapescript-0.1.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/test_parsing.py` & `tapescript-0.1.3/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/test_tools.py` & `tapescript-0.1.3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_committed_script.hex` & `tapescript-0.1.3/tests/vectors/cds_committed_script.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_committed_script.src` & `tapescript-0.1.3/tests/vectors/cds_committed_script.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_committed_script_decompiled.src` & `tapescript-0.1.3/tests/vectors/cds_committed_script_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_unlocking_script1.hex` & `tapescript-0.1.3/tests/vectors/cds_unlocking_script1.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_unlocking_script1.src` & `tapescript-0.1.3/tests/vectors/cds_unlocking_script1.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_unlocking_script1_decompiled.src` & `tapescript-0.1.3/tests/vectors/cds_unlocking_script1_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_unlocking_script2.hex` & `tapescript-0.1.3/tests/vectors/cds_unlocking_script2.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_unlocking_script2.src` & `tapescript-0.1.3/tests/vectors/cds_unlocking_script2.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_unlocking_script2_decompiled.src` & `tapescript-0.1.3/tests/vectors/cds_unlocking_script2_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_unlocking_script3.hex` & `tapescript-0.1.3/tests/vectors/cds_unlocking_script3.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_unlocking_script3.src` & `tapescript-0.1.3/tests/vectors/cds_unlocking_script3.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/cds_unlocking_script3_decompiled.src` & `tapescript-0.1.3/tests/vectors/cds_unlocking_script3_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/correspondent_unlocking_script2.hex` & `tapescript-0.1.3/tests/vectors/correspondent_unlocking_script2.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/correspondent_unlocking_script2.src` & `tapescript-0.1.3/tests/vectors/correspondent_unlocking_script2.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/correspondent_unlocking_script2_decompiled.src` & `tapescript-0.1.3/tests/vectors/correspondent_unlocking_script2_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/omega_e2e.hex` & `tapescript-0.1.3/tests/vectors/omega_e2e.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/omega_e2e.src` & `tapescript-0.1.3/tests/vectors/omega_e2e.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/tests/vectors/omega_e2e_decompiled.src` & `tapescript-0.1.3/tests/vectors/omega_e2e_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/license` & `tapescript-0.1.3/license`

 * *Files identical despite different names*

### Comparing `tapescript-0.1.2/pyproject.toml` & `tapescript-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tapescript"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Scripting system for use in distributed systems"
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `tapescript-0.1.2/readme.md` & `tapescript-0.1.3/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 OP_TRUE
 
 # unlocking script that validates on both versions #
 OP_PUSH x0123
 OP_PUSH x0123
 OP_PUSH x0123
 
-# unlocking script that validates on only the new version #
+# unlocking script that fails validation on the new version #
 OP_PUSH x0123
 OP_PUSH x0123
 OP_PUSH x3210
 ```
 
 ### Testing
```

### Comparing `tapescript-0.1.2/PKG-INFO` & `tapescript-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapescript
-Version: 0.1.2
+Version: 0.1.3
 Summary: Scripting system for use in distributed systems
 Project-URL: Homepage, https://github.com/k98kurz/tapescript
 Project-URL: Bug Tracker, https://github.com/k98kurz/tapescript/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: ISC License (ISCL)
@@ -230,15 +230,15 @@
 OP_TRUE
 
 # unlocking script that validates on both versions #
 OP_PUSH x0123
 OP_PUSH x0123
 OP_PUSH x0123
 
-# unlocking script that validates on only the new version #
+# unlocking script that fails validation on the new version #
 OP_PUSH x0123
 OP_PUSH x0123
 OP_PUSH x3210
 ```
 
 ### Testing
```

