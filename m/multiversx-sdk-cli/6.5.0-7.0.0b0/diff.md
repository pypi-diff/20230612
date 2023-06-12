# Comparing `tmp/multiversx_sdk_cli-6.5.0.tar.gz` & `tmp/multiversx_sdk_cli-7.0.0b0.tar.gz`

## Comparing `multiversx_sdk_cli-6.5.0.tar` & `multiversx_sdk_cli-7.0.0b0.tar`

### file list

```diff
@@ -1,104 +1,115 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/__init__.py
--rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/accounts.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_accounts.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_block.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_config.py
--rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_contracts.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_data.py
--rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_delegation.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_deps.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_dns.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_ledger.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_network.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_output.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_password.py
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_shared.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_testnet.py
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_transactions.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_validators.py
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_wallet.py
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/config.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/constants.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/contract_verification.py
--rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/contracts.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cosign_transaction.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/diskcache.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/dns.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/docker.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/downloader.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/errors.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/guards.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/interfaces.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/myprocess.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/simulation.py
--rw-r--r--   0        0        0    11018 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/transactions.py
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/utils.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/version.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/workstation.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/.vscode/settings.json
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/delegation/__init__.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/delegation/staking_provider.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/dependencies/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/dependencies/install.py
--rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/dependencies/modules.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/dependencies/resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/ledger/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/ledger/config.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/ledger/ledger_app_handler.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/ledger/ledger_functions.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/constants.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/core.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/eei_activation.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/eei_checks.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/eei_registry.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/interfaces.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/migrations.py
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/project_base.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/project_clang.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/project_cpp.py
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/project_rust.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/project_sol.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/shared.py
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/templates.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/templates_config.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/templates_repository.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/do_report.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/report_creator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/common.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/folder_report.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/project_report.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/wasm_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/features/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/features/features.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/features/report_option.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/features/size.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/format/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/format/change_type.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/format/format_options.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/__init__.py
--rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/config.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/core.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/genesis.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/genesis_json.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/genesis_smart_contracts_json.py
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/node_config_toml.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/nodes_setup_json.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/p2p_toml.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/seednode_p2pKey.pem
--rw-r--r--   0        0        0    10661 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/setup.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/wallets.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/validators/__init__.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/validators/core.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/validators/validators_file.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/LICENSE
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/README.md
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/pyproject.toml
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 multiversx_sdk_cli-6.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/__init__.py
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/accounts.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_accounts.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_block.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_config.py
+-rw-r--r--   0        0        0    19541 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_contracts.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_data.py
+-rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_delegation.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_deps.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_dns.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_ledger.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_localnet.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_network.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_output.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_password.py
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_shared.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_transactions.py
+-rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_validators.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_wallet.py
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/config.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/constants.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/contract_verification.py
+-rw-r--r--   0        0        0     9712 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/contracts.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cosign_transaction.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/diskcache.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dns.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/docker.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/downloader.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/errors.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/guards.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/interfaces.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/myprocess.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/simulation.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/transactions.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/utils.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ux.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/version.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/workstation.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/.vscode/settings.json
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/delegation/__init__.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/delegation/staking_provider.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/install.py
+-rw-r--r--   0        0        0    16479 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/modules.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/config.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/ledger_app_handler.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/ledger_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/__init__.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_default.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_general.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_networking.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_part.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_root.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_sharding.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/config_software.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/constants.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis_json.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/libraries.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/node.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/node_config_toml.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/nodes_setup_json.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/p2p_toml.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_build_software.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_clean.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_config.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_new.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_prerequisites.py
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/step_start.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/wallets.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/constants.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/core.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/interfaces.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/migrations.py
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_base.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_clang.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_cpp.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_rust.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_sol.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/shared.py
+-rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates_config.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates_repository.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/do_report.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/report_creator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/common.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/extracted_feature.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/folder_report.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/project_report.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/wasm_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/features.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/report_option.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/size.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/format/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/format/change_type.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/format/format_options.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/__init__.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/core.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/validators_file.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/LICENSE
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b0/PKG-INFO
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/accounts.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 import multiversx_sdk_cli.cli_config
 import multiversx_sdk_cli.cli_contracts
 import multiversx_sdk_cli.cli_data
 import multiversx_sdk_cli.cli_delegation
 import multiversx_sdk_cli.cli_deps
 import multiversx_sdk_cli.cli_dns
 import multiversx_sdk_cli.cli_ledger
+import multiversx_sdk_cli.cli_localnet
 import multiversx_sdk_cli.cli_network
-import multiversx_sdk_cli.cli_testnet
 import multiversx_sdk_cli.cli_transactions
 import multiversx_sdk_cli.cli_validators
 import multiversx_sdk_cli.cli_wallet
 import multiversx_sdk_cli.version
-from multiversx_sdk_cli import config, errors
+from multiversx_sdk_cli import config, errors, ux
 
 logger = logging.getLogger("cli")
 
 
 def main(cli_args: List[str] = sys.argv[1:]):
     try:
         _do_main(cli_args)
     except errors.KnownError as err:
         logger.critical(err.get_pretty())
+        ux.show_critical_error(err.get_pretty())
         return 1
     except KeyboardInterrupt:
         print("process killed by user.")
         return 1
     return 0
 
 
@@ -86,15 +87,15 @@
     commands.append(multiversx_sdk_cli.cli_accounts.setup_parser(subparsers))
     commands.append(multiversx_sdk_cli.cli_ledger.setup_parser(subparsers))
     commands.append(multiversx_sdk_cli.cli_wallet.setup_parser(args, subparsers))
     commands.append(multiversx_sdk_cli.cli_network.setup_parser(subparsers))
     commands.append(multiversx_sdk_cli.cli_deps.setup_parser(subparsers))
     commands.append(multiversx_sdk_cli.cli_config.setup_parser(subparsers))
     commands.append(multiversx_sdk_cli.cli_block.setup_parser(subparsers))
-    commands.append(multiversx_sdk_cli.cli_testnet.setup_parser(args, subparsers))
+    commands.append(multiversx_sdk_cli.cli_localnet.setup_parser(args, subparsers))
     commands.append(multiversx_sdk_cli.cli_data.setup_parser(subparsers))
     commands.append(multiversx_sdk_cli.cli_delegation.setup_parser(args, subparsers))
     commands.append(multiversx_sdk_cli.cli_dns.setup_parser(args, subparsers))
 
     parser.epilog = """
 ----------------------
 COMMAND GROUPS summary
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_accounts.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_accounts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 from typing import Any
 
+from multiversx_sdk_network_providers.proxy_network_provider import \
+    ProxyNetworkProvider
+
 from multiversx_sdk_cli import cli_shared, utils
 from multiversx_sdk_cli.accounts import Address
-from multiversx_sdk_network_providers.proxy_network_provider import ProxyNetworkProvider
 
 logger = logging.getLogger("cli.accounts")
 
 
 def setup_parser(subparsers: Any) -> Any:
     parser = cli_shared.add_group_subparser(subparsers, "account", "Get Account data (nonce, balance) from the Network")
     subparsers = parser.add_subparsers()
@@ -18,20 +20,14 @@
     mutex = sub.add_mutually_exclusive_group()
     mutex.add_argument("--balance", action="store_true", help="whether to only fetch the balance")
     mutex.add_argument("--nonce", action="store_true", help="whether to only fetch the nonce")
     mutex.add_argument("--username", action="store_true", help="whether to only fetch the username")
     cli_shared.add_omit_fields_arg(sub)
     sub.set_defaults(func=get_account)
 
-    sub = cli_shared.add_command_subparser(subparsers, "account", "get-transactions", "Query account transactions")
-    cli_shared.add_proxy_arg(sub)
-    cli_shared.add_outfile_arg(sub)
-    _add_address_arg(sub)
-    sub.set_defaults(func=get_account_transactions)
-
     parser.epilog = cli_shared.build_group_epilog(subparsers)
     return subparsers
 
 
 def _add_address_arg(sub: Any):
     sub.add_argument("--address", required=True, help="🖄 the address to query")
 
@@ -46,17 +42,7 @@
         print(account.balance)
     elif args.nonce:
         print(account.nonce)
     elif args.username:
         print(account.username)
     else:
         utils.dump_out_json(account.to_dictionary())
-
-
-def get_account_transactions(args: Any):
-    proxy_url = args.proxy
-    address = args.address
-    proxy = ProxyNetworkProvider(proxy_url)
-
-    response = proxy.get_account_transactions(Address(address))
-    transactions_as_dictionaries = [tx.to_dictionary() for tx in response]
-    utils.dump_out_json(transactions_as_dictionaries, args.outfile)
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_block.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_block.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_config.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_contracts.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from multiversx_sdk_cli.accounts import Account, Address, LedgerAccount
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
 from multiversx_sdk_cli.cli_password import load_password
 from multiversx_sdk_cli.contract_verification import \
     trigger_contract_verification
 from multiversx_sdk_cli.contracts import CodeMetadata, SmartContract
 from multiversx_sdk_cli.docker import is_docker_installed, run_docker
-from multiversx_sdk_cli.errors import DockerMissingError, NoWalletProvided
+from multiversx_sdk_cli.errors import DockerMissingError
 from multiversx_sdk_cli.projects import load_project
 from multiversx_sdk_cli.projects.core import get_project_paths_recursively
 from multiversx_sdk_cli.transactions import Transaction
 from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 
 logger = logging.getLogger("cli.contracts")
 
@@ -79,15 +79,14 @@
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
     _add_arguments_arg(sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     cli_shared.add_broadcast_args(sub)
-    cli_shared.add_guardian_wallet_args(args, sub)
 
     sub.set_defaults(func=deploy)
 
     sub = cli_shared.add_command_subparser(subparsers, "contract", "call",
                                            f"Interact with a Smart Contract (execute function).{output_description}")
     _add_contract_arg(sub)
     cli_shared.add_outfile_arg(sub)
@@ -97,15 +96,14 @@
     _add_function_arg(sub)
     _add_arguments_arg(sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     cli_shared.add_broadcast_args(sub, relay=True)
-    cli_shared.add_guardian_wallet_args(args, sub)
 
     sub.set_defaults(func=call)
 
     sub = cli_shared.add_command_subparser(subparsers, "contract", "upgrade",
                                            f"Upgrade a previously-deployed Smart Contract.{output_description}")
     _add_contract_arg(sub)
     cli_shared.add_outfile_arg(sub)
@@ -116,15 +114,14 @@
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
     _add_arguments_arg(sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     cli_shared.add_broadcast_args(sub)
-    cli_shared.add_guardian_wallet_args(args, sub)
 
     sub.set_defaults(func=upgrade)
 
     sub = cli_shared.add_command_subparser(subparsers, "contract", "query",
                                            "Query a Smart Contract (call a pure function)")
     _add_contract_arg(sub)
     cli_shared.add_proxy_arg(sub)
@@ -146,15 +143,14 @@
     _add_contract_arg(sub)
     sub.add_argument(
         "--verifier-url",
         required=True,
         help="the url of the service that validates the contract",
     )
     sub.add_argument("--docker-image", required=True, help="the docker image used for the build")
-    sub.add_argument("--contract-variant", required=False, default=None, help="in case of a multicontract, specify the contract variant you want to verify")
     cli_shared.add_wallet_args(args, sub)
     sub.set_defaults(func=verify)
 
     sub = cli_shared.add_command_subparser(subparsers, "contract", "reproducible-build",
                                            "Build a Smart Contract and get the same output as a previously built Smart Contract")
     _add_project_arg(sub)
     _add_build_options_args(sub)
@@ -186,19 +182,14 @@
     sub.add_argument("--wasm-symbols", action="store_true", default=False,
                      help="for rust projects, does not strip the symbols from the wasm output. Useful for analysing the bytecode. Creates larger wasm files. Avoid in production (default: %(default)s)")
     sub.add_argument("--wasm-name", type=str,
                      help="for rust projects, optionally specify the name of the wasm bytecode output file")
     sub.add_argument("--wasm-suffix", type=str,
                      help="for rust projects, optionally specify the suffix of the wasm bytecode output file")
 
-    sub.add_argument("--eei-checks", action="store_true", default=False, help="run EEI compatibility checks (default: %(default)s)")
-    # Flags are kept in order to avoid breaking changes, for the moment - we might completely remove them in the future.
-    sub.add_argument("--skip-eei-checks", action="store_true", default=True, help="deprecated flag")
-    sub.add_argument("--ignore-eei-checks", action="store_true", default=True, help="deprecated flag")
-
 
 def _add_recursive_arg(sub: Any):
     sub.add_argument("-r", "--recursive", dest="recursive", action="store_true", help="locate projects recursively")
 
 
 def _add_project_or_bytecode_arg(sub: Any):
     group = sub.add_mutually_exclusive_group(required=True)
@@ -273,20 +264,15 @@
         "debug": args.debug,
         "optimized": not args.no_optimization,
         "no-wasm-opt": args.no_wasm_opt,
         "verbose": args.verbose,
         "cargo-target-dir": args.cargo_target_dir,
         "wasm-symbols": args.wasm_symbols,
         "wasm-name": args.wasm_name,
-        "wasm-suffix": args.wasm_suffix,
-        "eei-checks": args.eei_checks,
-        # TODO: Remove this, in the future
-        "skip-eei-checks": args.skip_eei_checks,
-        # TODO: Remove this, in the future
-        "ignore-eei-checks": args.ignore_eei_checks
+        "wasm-suffix": args.wasm_suffix
     }
 
 
 def do_report(args: Any):
     build_options: Dict[str, Any] = _prepare_build_options(args)
     projects.do_report(args, build_options)
 
@@ -295,29 +281,31 @@
     project_paths = get_project_paths(args)
     for project in project_paths:
         projects.run_tests(project, args)
 
 
 def deploy(args: Any):
     logger.debug("deploy")
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
 
     arguments = args.arguments
     gas_price = args.gas_price
     gas_limit = args.gas_limit
     value = args.value
     chain = args.chain
     version = args.version
 
     contract = _prepare_contract(args)
     sender = _prepare_sender(args)
 
     tx = contract.deploy(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
-    tx = _sign_guarded_tx(args, tx)
+
+    if args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
 
     logger.info("Contract address: %s", contract.address)
     utils.log_explorer_contract_address(chain, contract.address)
 
     _send_or_simulate(tx, contract, args)
 
 
@@ -368,36 +356,17 @@
         sender = Account(key_file=args.keyfile, password=password)
     else:
         raise errors.NoWalletProvided()
 
     return sender
 
 
-def _sign_guarded_tx(args: Any, tx: Transaction) -> Transaction:
-    signature = tx.signature
-    tx.signature = ""
-
-    try:
-        guardian_account = cli_shared.prepare_guardian_account(args)
-    except NoWalletProvided:
-        guardian_account = None
-
-    if guardian_account:
-        tx.guardianSignature = guardian_account.sign_transaction(tx)
-    elif args.guardian:
-        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)  # type: ignore
-
-    tx.signature = signature
-
-    return tx
-
-
 def call(args: Any):
     logger.debug("call")
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
 
     contract_address = args.contract
     function = args.function
     arguments = args.arguments
     gas_price = args.gas_price
     gas_limit = args.gas_limit
@@ -405,15 +374,17 @@
     chain = args.chain
     version = args.version
 
     contract = SmartContract(contract_address)
     sender = _prepare_sender(args)
 
     tx = contract.execute(sender, function, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
-    tx = _sign_guarded_tx(args, tx)
+
+    if args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
 
     _send_or_simulate(tx, contract, args)
 
 
 def upgrade(args: Any):
     logger.debug("upgrade")
     cli_shared.check_broadcast_args(args)
@@ -426,16 +397,18 @@
     chain = args.chain
     version = args.version
 
     contract = _prepare_contract(args)
     contract.address = Address(contract_address)
     sender = _prepare_sender(args)
 
-    tx = contract.upgrade(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian, args.options)
-    tx = _sign_guarded_tx(args, tx)
+    tx = contract.upgrade(sender, arguments, gas_price, gas_limit, value, chain, version, args.guardian_address, args.options)
+
+    if args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
 
     _send_or_simulate(tx, contract, args)
 
 
 def query(args: Any):
     logger.debug("query")
 
@@ -458,18 +431,17 @@
     contract = Address(args.contract)
     verifier_url = args.verifier_url
 
     packaged_src = Path(args.packaged_src).expanduser().resolve()
 
     owner = _prepare_signer(args)
     docker_image = args.docker_image
-    contract_variant = args.contract_variant
 
     trigger_contract_verification(
-        packaged_src, owner, contract, verifier_url, docker_image, contract_variant
+        packaged_src, owner, contract, verifier_url, docker_image
     )
     logger.info("Contract verification request completed!")
 
 
 def do_reproducible_build(args: Any):
     project_path = args.project
     docker_image = args.docker_image
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_data.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_data.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_delegation.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_delegation.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,19 +130,18 @@
 
 def _add_common_arguments(args: List[str], sub: Any):
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_estimate_gas=True, with_guardian=True)
     cli_shared.add_broadcast_args(sub, relay=False)
     cli_shared.add_outfile_arg(sub, what="signed transaction, hash")
-    cli_shared.add_guardian_wallet_args(args, sub)
 
 
 def do_create_delegation_contract(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_create_new_staking_contract(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
@@ -158,114 +157,114 @@
         contract_address = transaction_events[0].address
         print(contract_address.bech32())
     else:
         raise errors.ProgrammingError("Tx has more than one event. Make sure it's a staking provider SC Deploy transaction.")
 
 
 def add_new_nodes(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_add_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def remove_nodes(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_remove_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def stake_nodes(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_stake_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unbond_nodes(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_unbond_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unstake_nodes(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_unstake_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def unjail_nodes(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_for_unjail_nodes(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def change_service_fee(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_change_service_fee(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def modify_delegation_cap(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_modify_delegation_cap(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def automatic_activation(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_automatic_activation(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def redelegate_cap(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_redelegate_cap(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
 
 
 def set_metadata(args: Any):
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     staking_provider.prepare_args_set_metadata(args)
     tx = do_prepare_transaction(args)
 
     cli_shared.send_or_simulate(tx, args)
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_deps.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_deps.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_dns.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
     sub = cli_shared.add_command_subparser(subparsers, "dns", "register", "Send a register transaction to the appropriate DNS contract from given user and with given name")
     cli_shared.add_outfile_arg(sub)
     cli_shared.add_broadcast_args(sub, relay=True)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_guardian=True)
-    cli_shared.add_guardian_wallet_args(args, sub)
     sub.add_argument("--name", help="the name to register")
     sub.set_defaults(func=register)
 
     sub = cli_shared.add_command_subparser(subparsers, "dns", "resolve", "Find the address for a name")
     _add_name_arg(sub)
     cli_shared.add_proxy_arg(sub)
     sub.set_defaults(func=dns_resolve)
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_ledger.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_ledger.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_network.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_network.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_output.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_output.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_shared.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_shared.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from multiversx_sdk_network_providers.proxy_network_provider import \
     ProxyNetworkProvider
 
 from multiversx_sdk_cli import config, errors, utils
 from multiversx_sdk_cli.accounts import Account
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
-from multiversx_sdk_cli.cli_password import load_password, load_guardian_password
+from multiversx_sdk_cli.cli_password import load_password
 from multiversx_sdk_cli.ledger.ledger_functions import do_get_ledger_address
 from multiversx_sdk_cli.simulation import Simulator
 from multiversx_sdk_cli.transactions import Transaction
 from multiversx_sdk_cli.constants import TRANSACTION_OPTIONS_TX_GUARDED
 
 
 def wider_help_formatter(prog: Text):
@@ -75,46 +75,32 @@
     if with_data:
         sub.add_argument("--data", default="", help="the payload, or 'memo' of the transaction (default: %(default)s)")
 
     sub.add_argument("--chain", default=config.get_chain_id(), help="the chain identifier (default: %(default)s)")
     sub.add_argument("--version", type=int, default=config.get_tx_version(), help="the transaction version (default: %(default)s)")
 
     if with_guardian:
-        add_guardian_args(sub)
+        sub.add_argument("--guardian", type=str, help="the address of the guradian")
+        sub.add_argument("--guardian-service-url", type=str, help="the url of the guardian service")
+        sub.add_argument("--guardian-2fa-code", type=str, help="the 2fa code for the guardian")
 
     sub.add_argument("--options", type=int, default=0, help="the transaction options (default: 0)")
 
 
-def add_guardian_args(sub: Any):
-    sub.add_argument("--guardian", type=str, help="the address of the guradian")
-    sub.add_argument("--guardian-service-url", type=str, help="the url of the guardian service")
-    sub.add_argument("--guardian-2fa-code", type=str, help="the 2fa code for the guardian")
-
-
 def add_wallet_args(args: List[str], sub: Any):
     sub.add_argument("--pem", required=check_if_sign_method_required(args, "--pem"), help="🔑 the PEM file, if keyfile not provided")
     sub.add_argument("--pem-index", default=0, help="🔑 the index in the PEM file (default: %(default)s)")
     sub.add_argument("--keyfile", required=check_if_sign_method_required(args, "--keyfile"), help="🔑 a JSON keyfile, if PEM not provided")
     sub.add_argument("--passfile", help="🔑 a file containing keyfile's password, if keyfile provided")
     sub.add_argument("--ledger", action="store_true", required=check_if_sign_method_required(args, "--ledger"), default=False, help="🔐 bool flag for signing transaction using ledger")
     sub.add_argument("--ledger-account-index", type=int, default=0, help="🔐 the index of the account when using Ledger")
     sub.add_argument("--ledger-address-index", type=int, default=0, help="🔐 the index of the address when using Ledger")
     sub.add_argument("--sender-username", required=False, help="🖄 the username of the sender")
 
 
-def add_guardian_wallet_args(args: List[str], sub: Any):
-    sub.add_argument("--guardian-pem", required=check_if_sign_method_required(args, "--guardian-pem"), help="🔑 the PEM file, if keyfile not provided")
-    sub.add_argument("--guardian-pem-index", default=0, help="🔑 the index in the PEM file (default: %(default)s)")
-    sub.add_argument("--guardian-keyfile", required=check_if_sign_method_required(args, "--guardian-keyfile"), help="🔑 a JSON keyfile, if PEM not provided")
-    sub.add_argument("--guardian-passfile", help="🔑 a file containing keyfile's password, if keyfile provided")
-    sub.add_argument("--guardian-ledger", action="store_true", required=check_if_sign_method_required(args, "--guardian-ledger"), default=False, help="🔐 bool flag for signing transaction using ledger")
-    sub.add_argument("--guardian-ledger-account-index", type=int, default=0, help="🔐 the index of the account when using Ledger")
-    sub.add_argument("--guardian-ledger-address-index", type=int, default=0, help="🔐 the index of the address when using Ledger")
-
-
 def add_proxy_arg(sub: Any):
     sub.add_argument("--proxy", default=config.get_proxy(), help="🔗 the URL of the proxy (default: %(default)s)")
 
 
 def add_outfile_arg(sub: Any, what: str = ""):
     what = f"({what})" if what else ""
     sub.add_argument("--outfile", type=FileType("w"), default=sys.stdout, help=f"where to save the output {what} (default: stdout)")
@@ -131,47 +117,27 @@
 
 def parse_omit_fields_arg(args: Any) -> List[str]:
     literal = args.omit_fields
     parsed = ast.literal_eval(literal)
     return cast(List[str], parsed)
 
 
-def prepare_account(args: Any):
-    if args.pem:
-        account = Account(pem_file=args.pem, pem_index=args.pem_index)
-    elif args.keyfile:
-        password = load_password(args)
-        account = Account(key_file=args.keyfile, password=password)
-    elif args.ledger:
-        address = do_get_ledger_address(account_index=args.ledger_account_index, address_index=args.ledger_address_index)
-        account = Account(address=address)
-    else:
-        raise errors.NoWalletProvided()
-
-    return account
-
-
-def prepare_guardian_account(args: Any):
-    if args.guardian_pem:
-        account = Account(pem_file=args.guardian_pem, pem_index=args.guardian_pem_index)
-    elif args.guardian_keyfile:
-        password = load_guardian_password(args)
-        account = Account(key_file=args.guardian_keyfile, password=password)
-    elif args.guardian_ledger:
-        address = do_get_ledger_address(account_index=args.guardian_ledger_account_index, address_index=args.guardian_ledger_address_index)
-        account = Account(address=address)
-    else:
-        raise errors.NoWalletProvided()
-
-    return account
-
-
 def prepare_nonce_in_args(args: Any):
     if args.recall_nonce:
-        account = prepare_account(args)
+        if args.pem:
+            account = Account(pem_file=args.pem, pem_index=args.pem_index)
+        elif args.keyfile:
+            password = load_password(args)
+            account = Account(key_file=args.keyfile, password=password)
+        elif args.ledger:
+            address = do_get_ledger_address(account_index=args.ledger_account_index, address_index=args.ledger_address_index)
+            account = Account(address=address)
+        else:
+            raise errors.NoWalletProvided()
+
         account.sync_nonce(ProxyNetworkProvider(args.proxy))
         args.nonce = account.nonce
 
 
 def add_broadcast_args(sub: Any, simulate: bool = True, relay: bool = False):
     sub.add_argument("--send", action="store_true", default=False, help="✓ whether to broadcast the transaction (default: %(default)s)")
 
@@ -184,40 +150,21 @@
 def check_broadcast_args(args: Any):
     if hasattr(args, "relay") and args.relay and args.send:
         raise errors.BadUsage("Cannot directly send a relayed transaction. Use 'mxpy tx new --relay' first, then 'mxpy tx send --data-file'")
     if args.send and args.simulate:
         raise errors.BadUsage("Cannot both 'simulate' and 'send' a transaction")
 
 
-def check_guardian_and_options_args(args: Any):
-    check_guardian_args(args)
-    if args.guardian:
-        check_options_for_guarded_tx(args.options)
-
-
 def check_guardian_args(args: Any):
-    if args.guardian:
-        if should_sign_with_cosigner_service(args) and should_sign_with_guardian_key(args):
-            raise errors.BadUsage("Guarded tx should be signed using either a cosigning service or a guardian key")
-
-        if not should_sign_with_cosigner_service(args) and not should_sign_with_guardian_key(args):
-            raise errors.BadUsage("Missing guardian signing arguments")
-
-
-def should_sign_with_cosigner_service(args: Any) -> bool:
-    return all([args.guardian_service_url, args.guardian_2fa_code])
-
-
-def should_sign_with_guardian_key(args: Any) -> bool:
-    return any([args.guardian_pem, args.guardian_keyfile, args.guardian_ledger])
-
+    if any([args.guardian, args.guardian_service_url, args.guardian_2fa_code]):
+        if not all([args.guardian, args.guardian_service_url, args.guardian_2fa_code]):
+            raise errors.BadUsage("All guardian arguments must be provided")
 
-def check_options_for_guarded_tx(options: int):
-    if not options & TRANSACTION_OPTIONS_TX_GUARDED == TRANSACTION_OPTIONS_TX_GUARDED:
-        raise errors.BadUsage("Invalid guarded transaction's options. The second least significant bit must be set.")
+        if not args.options & TRANSACTION_OPTIONS_TX_GUARDED == TRANSACTION_OPTIONS_TX_GUARDED:
+            raise errors.BadUsage("For guarded transactions the guarded flag must be set.")
 
 
 def send_or_simulate(tx: Transaction, args: Any, dump_output: bool = True) -> CLIOutputBuilder:
     proxy = ProxyNetworkProvider(args.proxy)
 
     is_set_wait_result = hasattr(args, "wait_result") and args.wait_result
     is_set_send = hasattr(args, "send") and args.send
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_transactions.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_transactions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from pathlib import Path
 from typing import Any, List
 
 from multiversx_sdk_cli import cli_shared, utils
 from multiversx_sdk_cli.cli_output import CLIOutputBuilder
 from multiversx_sdk_network_providers.proxy_network_provider import ProxyNetworkProvider
-from multiversx_sdk_cli.errors import NoWalletProvided
 from multiversx_sdk_cli.transactions import Transaction, do_prepare_transaction
-from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 
 
 def setup_parser(args: List[str], subparsers: Any) -> Any:
     parser = cli_shared.add_group_subparser(subparsers, "tx", "Create and broadcast Transactions")
     subparsers = parser.add_subparsers()
 
     sub = cli_shared.add_command_subparser(subparsers, "tx", "new", f"Create a new transaction.{CLIOutputBuilder.describe()}")
     _add_common_arguments(args, sub)
     cli_shared.add_outfile_arg(sub, what="signed transaction, hash")
     cli_shared.add_broadcast_args(sub, relay=True)
     cli_shared.add_proxy_arg(sub)
-    cli_shared.add_guardian_wallet_args(args, sub)
     sub.add_argument("--wait-result", action="store_true", default=False,
                      help="signal to wait for the transaction result - only valid if --send is set")
     sub.add_argument("--timeout", default=100, help="max num of seconds to wait for result"
                                                     " - only valid if --wait-result is set")
     sub.set_defaults(func=create_transaction)
 
     sub = cli_shared.add_command_subparser(subparsers, "tx", "send", f"Send a previously saved transaction.{CLIOutputBuilder.describe()}")
@@ -35,38 +32,28 @@
     sub.add_argument("--hash", required=True, help="the hash")
     sub.add_argument("--sender", required=False, help="the sender address")
     sub.add_argument("--with-results", action="store_true", help="will also return the results of transaction")
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_omit_fields_arg(sub)
     sub.set_defaults(func=get_transaction)
 
-    sub = cli_shared.add_command_subparser(subparsers, "tx", "sign", f"Sign a previously saved transaction.{CLIOutputBuilder.describe()}")
-    cli_shared.add_wallet_args(args, sub)
-    cli_shared.add_infile_arg(sub, what="a previously saved transaction")
-    cli_shared.add_outfile_arg(sub, what="the signed transaction")
-    cli_shared.add_broadcast_args(sub, relay=True)
-    cli_shared.add_proxy_arg(sub)
-    cli_shared.add_guardian_args(sub)
-    cli_shared.add_guardian_wallet_args(args, sub)
-    sub.set_defaults(func=sign_transaction)
-
     parser.epilog = cli_shared.build_group_epilog(subparsers)
     return subparsers
 
 
 def _add_common_arguments(args: List[str], sub: Any):
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_tx_args(args, sub, with_guardian=True)
     sub.add_argument("--data-file", type=str, default=None, help="a file containing transaction data")
 
 
 def create_transaction(args: Any):
     args = utils.as_object(args)
 
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
 
     if args.data_file:
         args.data = Path(args.data_file).read_text()
 
     tx = do_prepare_transaction(args)
@@ -94,39 +81,7 @@
     args = utils.as_object(args)
     omit_fields = cli_shared.parse_omit_fields_arg(args)
     proxy = ProxyNetworkProvider(args.proxy)
 
     transaction = proxy.get_transaction(args.hash)
     output = CLIOutputBuilder().set_transaction_on_network(transaction, omit_fields).build()
     utils.dump_out_json(output)
-
-
-def sign_transaction(args: Any):
-    args = utils.as_object(args)
-
-    cli_shared.check_guardian_args(args)
-    cli_shared.check_broadcast_args(args)
-
-    tx = Transaction.load_from_file(args.infile)
-    if args.guardian:
-        cli_shared.check_options_for_guarded_tx(tx.options)
-
-    # clear existing signatures, if any
-    tx.guardianSignature = ""
-    tx.signature = ""
-
-    account = cli_shared.prepare_account(args)
-    signature = account.sign_transaction(tx)
-
-    try:
-        guardian_account = cli_shared.prepare_guardian_account(args)
-    except NoWalletProvided:
-        guardian_account = None
-
-    if guardian_account:
-        tx.guardianSignature = guardian_account.sign_transaction(tx)
-    elif args.guardian:
-        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
-
-    tx.signature = signature
-
-    cli_shared.send_or_simulate(tx, args)
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_validators.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 
 def _add_common_arguments(args: List[str], sub: Any):
     cli_shared.add_proxy_arg(sub)
     cli_shared.add_wallet_args(args, sub)
     cli_shared.add_tx_args(args, sub, with_receiver=False, with_data=False, with_estimate_gas=True, with_guardian=True)
     cli_shared.add_broadcast_args(sub, relay=False)
     cli_shared.add_outfile_arg(sub, what="signed transaction, hash")
-    cli_shared.add_guardian_wallet_args(args, sub)
 
 
 def _add_nodes_arg(sub: Any):
     sub.add_argument("--nodes-public-keys", required=True, help="the public keys of the nodes as CSV (addrA,addrB)")
 
 
 def do_stake(args: Any):
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cli_wallet.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cli_wallet.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,40 +37,25 @@
 
     sub = cli_shared.add_command_subparser(
         subparsers,
         "wallet",
         "new",
         "Create a new wallet and print its mnemonic; optionally save as password-protected JSON (recommended) or PEM (not recommended)"
     )
-    sub.add_argument("--json", help="DEPRECATED, replaced by --format=keystore-mnemonic", action="store_true", default=False)
-    sub.add_argument("--pem", help="DEPRECATED, replaced by --format=pem", action="store_true", default=False)
-    sub.add_argument("--output-path", help="DEPRECATED, replaced by --outfile", type=str)
     sub.add_argument("--format", choices=WALLET_FORMATS, help="the format of the generated wallet file (default: %(default)s)", default=None)
     sub.add_argument("--outfile", help="the output path and base file name for the generated wallet files (default: %(default)s)", type=str)
     sub.add_argument("--address-hrp", help=f"the human-readable part of the address, when format is {WALLET_FORMAT_KEYSTORE_SECRET_KEY} or {WALLET_FORMAT_PEM} (default: %(default)s)", type=str, default="erd")
     sub.set_defaults(func=wallet_new)
 
     sub = cli_shared.add_command_subparser(
         subparsers,
         "wallet",
-        "derive",
-        "DEPRECATED COMMAND, replaced by 'wallet convert'"
-    )
-    sub.add_argument("pem", help="path of the output PEM file")
-    sub.add_argument("--mnemonic", action="store_true", help="whether to derive from an existing mnemonic")
-    sub.add_argument("--index", help="the address index", type=int, default=0)
-    sub.set_defaults(func=wallet_derive_deprecated)
-
-    sub = cli_shared.add_command_subparser(
-        subparsers,
-        "wallet",
         "convert",
         "Convert a wallet from one format to another"
     )
-
     sub.add_argument("--infile", help="path to the input file")
     sub.add_argument("--outfile", help="path to the output file")
     sub.add_argument("--in-format", required=True, choices=WALLET_FORMATS, help="the format of the input file")
     sub.add_argument("--out-format", required=True, choices=WALLET_FORMATS, help="the format of the output file")
     sub.add_argument("--address-index", help=f"the address index, if input format is {WALLET_FORMAT_RAW_MNEMONIC}, {WALLET_FORMAT_KEYSTORE_MNEMONIC} or {WALLET_FORMAT_PEM} (with multiple entries) and the output format is {WALLET_FORMAT_KEYSTORE_SECRET_KEY} or {WALLET_FORMAT_PEM}", type=int, default=0)
     sub.add_argument("--address-hrp", help=f"the human-readable part of the address, when the output format is {WALLET_FORMAT_KEYSTORE_SECRET_KEY} or {WALLET_FORMAT_PEM} (default: %(default)s)", type=str, default="erd")
     sub.set_defaults(func=convert_wallet)
@@ -112,25 +97,14 @@
 
 
 def wallet_new(args: Any):
     format = args.format
     outfile = args.outfile
     address_hrp = args.address_hrp
 
-    # Handle deprecated options
-    if args.json:
-        logger.warning("The --json option is deprecated, use --format=keystore-mnemonic instead.")
-        format = "keystore-mnemonic"
-    if args.pem:
-        logger.warning("The --pem option is deprecated, use --format=pem instead.")
-        format = "pem"
-    if args.output_path:
-        logger.warning("The --output-path option is deprecated, use --outfile instead.")
-        outfile = args.output_path
-
     mnemonic = Mnemonic.generate()
     print(f"Mnemonic: {mnemonic.get_text()}")
 
     if format is None:
         return
     if outfile is None:
         raise KnownError("The --outfile option is required when --format is specified.")
@@ -253,39 +227,14 @@
         address = pubkey.to_address(address_hrp)
         pem = UserPEM(address.bech32(), secret_key)
         return pem.to_text()
 
     raise KnownError(f"Cannot create wallet, unknown output format: <{out_format}>. Make sure to use one of following: {WALLET_FORMATS}.")
 
 
-def wallet_derive_deprecated(args: Any):
-    logger.warning("This command is deprecated. Use 'wallet convert' instead.")
-
-    pem_file_path = Path(args.pem)
-    ask_mnemonic = args.mnemonic
-    index = args.index
-
-    if ask_mnemonic:
-        mnemonic_str = input("Enter mnemonic:\n").rstrip().replace("\n", "")
-        mnemonic = Mnemonic(mnemonic_str)
-        secret_key = mnemonic.derive_key(index)
-        pubkey = secret_key.generate_public_key()
-    else:
-        mnemonic = Mnemonic.generate()
-
-    secret_key = mnemonic.derive_key(index)
-    pubkey = secret_key.generate_public_key()
-    address = Address(pubkey.hex())
-
-    pem_file = UserPEM(address.bech32(), secret_key)
-    pem_file.save(pem_file_path)
-
-    logger.info(f"Created PEM file [{pem_file_path}] for [{address.bech32()}]")
-
-
 def do_bech32(args: Any):
     encode = args.encode
     value = args.value
     address = Address(value)
 
     result = address.bech32() if encode else address.hex()
     print(result)
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/config.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -166,21 +166,14 @@
         "dependencies.vmtools.urlTemplate.windows": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
         "dependencies.llvm.tag": "v9-19feb",
         # ide.elrond.com will be removed, TBD if clang will still be downloaded
         "dependencies.llvm.urlTemplate.linux": "https://ide.elrond.com/vendor-llvm/{TAG}/linux-amd64.tar.gz?t=19feb",
         "dependencies.llvm.urlTemplate.osx": "https://ide.elrond.com/vendor-llvm/{TAG}/darwin-amd64.tar.gz?t=19feb",
         "dependencies.rust.resolution": "SDK",
         "dependencies.rust.tag": "nightly",
-        "dependencies.mx_chain_go.tag": "latest",
-        "dependencies.mx_chain_go.urlTemplate.linux": "https://github.com/multiversx/mx-chain-go/archive/{TAG}.tar.gz",
-        "dependencies.mx_chain_go.urlTemplate.osx": "https://github.com/multiversx/mx-chain-go/archive/{TAG}.tar.gz",
-        "dependencies.mx_chain_go.url": "https://github.com/multiversx/mx-chain-go/archive/{TAG}.tar.gz",
-        "dependencies.mx_chain_proxy_go.tag": "latest",
-        "dependencies.mx_chain_proxy_go.urlTemplate.linux": "https://github.com/multiversx/mx-chain-proxy-go/archive/{TAG}.tar.gz",
-        "dependencies.mx_chain_proxy_go.urlTemplate.osx": "https://github.com/multiversx/mx-chain-proxy-go/archive/{TAG}.tar.gz",
         "dependencies.golang.resolution": "SDK",
         "dependencies.golang.tag": "go1.18.4",
         "dependencies.golang.urlTemplate.linux": "https://golang.org/dl/{TAG}.linux-amd64.tar.gz",
         "dependencies.golang.urlTemplate.osx": "https://golang.org/dl/{TAG}.darwin-amd64.tar.gz",
         "dependencies.golang.urlTemplate.windows": "https://golang.org/dl/{TAG}.windows-amd64.zip",
         "dependencies.wasm-opt.tag": "latest",
         "dependencies.twiggy.tag": "latest",
@@ -189,15 +182,14 @@
         "dependencies.testwallets.urlTemplate.osx": "https://github.com/multiversx/mx-sdk-testwallets/archive/{TAG}.tar.gz",
         "dependencies.testwallets.urlTemplate.windows": "https://github.com/multiversx/mx-sdk-testwallets/archive/{TAG}.tar.gz",
         "dependencies.wasm-opt.resolution": "SDK",
         "dependencies.wasm-opt.tag": "version_112",
         "dependencies.wasm-opt.urlTemplate.linux": "https://github.com/WebAssembly/binaryen/releases/download/{TAG}/binaryen-{TAG}-x86_64-linux.tar.gz",
         "dependencies.wasm-opt.urlTemplate.osx": "https://github.com/WebAssembly/binaryen/releases/download/{TAG}/binaryen-{TAG}-x86_64-macos.tar.gz",
         "dependencies.wasm-opt.urlTemplate.windows": "https://github.com/WebAssembly/binaryen/releases/download/{TAG}/binaryen-{TAG}-x86_64-windows.tar.gz",
-        "testnet.validate_expected_keys": "false",
         "github_api_token": "",
     }
 
 
 def resolve_config_path() -> Path:
     if os.path.isfile(LOCAL_CONFIG_PATH):
         return LOCAL_CONFIG_PATH
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/contract_verification.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/contract_verification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hashlib
 import json
 import logging
 import time
 from pathlib import Path
-from typing import Any, Dict, Tuple, Optional
+from typing import Any, Dict, Tuple
 
 import requests
 
 from multiversx_sdk_cli.accounts import Account, Address
 from multiversx_sdk_cli.errors import KnownError
 from multiversx_sdk_cli.utils import dump_out_json, read_json_file
 
@@ -20,64 +20,59 @@
 class ContractVerificationRequest:
     def __init__(
         self,
         contract: Address,
         source_code: Dict[str, Any],
         signature: bytes,
         docker_image: str,
-        contract_variant: Optional[str]
     ) -> None:
         self.contract = contract
         self.source_code = source_code
         self.signature = signature
         self.docker_image = docker_image
-        self.contract_variant = contract_variant
 
     def to_dictionary(self) -> Dict[str, Any]:
         return {
             "signature": self.signature.hex(),
             "payload": {
                 "contract": self.contract.bech32(),
                 "dockerImage": self.docker_image,
-                "sourceCode": self.source_code,
-                "contractVariant": self.contract_variant
+                "sourceCode": self.source_code
             }
         }
 
 
 class ContractVerificationPayload:
-    def __init__(self, contract: Address, source_code: Dict[str, Any], docker_image: str, contract_variant: Optional[str]) -> None:
+    def __init__(self, contract: Address, source_code: Dict[str, Any], docker_image: str,) -> None:
         self.contract = contract
         self.source_code = source_code
         self.docker_image = docker_image
-        self.contract_variant = contract_variant
 
-    def serialize(self) -> str:
+    def serialize(self):
         payload = {
             "contract": self.contract.bech32(),
             "dockerImage": self.docker_image,
-            "sourceCode": self.source_code,
-            "contractVariant": self.contract_variant
+            "sourceCode": self.source_code
         }
 
         return json.dumps(payload, separators=(',', ':'))
 
 
 def trigger_contract_verification(
-        packaged_source: Path,
-        owner: Account,
-        contract: Address,
-        verifier_url: str,
-        docker_image: str,
-        contract_variant: Optional[str]):
+    packaged_source: Path,
+    owner: Account,
+    contract: Address,
+    verifier_url: str,
+    docker_image: str,
+):
     source_code = read_json_file(packaged_source)
 
-    payload = ContractVerificationPayload(contract, source_code, docker_image, contract_variant).serialize()
+    payload = ContractVerificationPayload(contract, source_code, docker_image).serialize()
     signature = _create_request_signature(owner, contract, payload.encode())
-    contract_verification = ContractVerificationRequest(contract, source_code, signature, docker_image, contract_variant)
+    contract_verification = ContractVerificationRequest(contract, source_code, signature, docker_image)
 
     request_dictionary = contract_verification.to_dictionary()
 
     url = f"{verifier_url}/verifier"
     status_code, message, data = _do_post(url, request_dictionary)
 
     if status_code == HTTP_REQUEST_TIMEOUT:
@@ -101,15 +96,15 @@
 
 
 def _create_request_signature(account: Account, contract_address: Address, request_payload: bytes) -> bytes:
     hashed_payload: str = hashlib.sha256(request_payload).hexdigest()
     raw_data_to_sign = f"{contract_address.bech32()}{hashed_payload}"
 
     signature_hex = account.sign_message(raw_data_to_sign.encode())
-    signature = bytes.fromhex(signature_hex)
+    signature: bytes = bytes.fromhex(signature_hex)
 
     return signature
 
 
 def query_status_with_task_id(url: str, task_id: str, interval: int = 10):
     logger.info(f"Please wait while we verify your contract. This may take a while.")
     old_status = ""
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/contracts.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/contracts.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class INetworkProvider(Protocol):
     def query_contract(self, query: Any) -> 'IContractQueryResponse':
         ...
 
 
 class QueryResult(Object):
-    def __init__(self, as_base64: str, as_hex: str, as_number: Optional[int]):
+    def __init__(self, as_base64: str, as_hex: str, as_number: int):
         self.base64 = as_base64
         self.hex = as_hex
         self.number = as_number
 
 
 class ContractQuery(IContractQuery):
     def __init__(self, address: Address, function: str, value: int, arguments: List[bytes], caller: Optional[Address] = None):
@@ -204,37 +204,23 @@
     def _interpret_return_data(self, data: str) -> Any:
         if not data:
             return data
 
         try:
             as_bytes = base64.b64decode(data)
             as_hex = as_bytes.hex()
-            as_number = _interpret_as_number_if_safely(as_hex)
+            as_number = int(as_hex, 16)
 
             result = QueryResult(data, as_hex, as_number)
             return result
         except Exception:
             logger.warn(f"Cannot interpret return data: {data}")
             return None
 
 
-def _interpret_as_number_if_safely(as_hex: str) -> Optional[int]:
-    """
-    Makes sure the string can be safely converted to an int (and then back to a string).
-
-    See:
-        - https://stackoverflow.com/questions/73693104/valueerror-exceeds-the-limit-4300-for-integer-string-conversion 
-        - https://github.com/python/cpython/issues/95778
-    """
-    try:
-        return int(str(int(as_hex or "0", 16)))
-    except:
-        return None
-
-
 def _prepare_argument(argument: Any):
     as_str = str(argument)
     as_hex = _to_hex(as_str)
     return as_hex
 
 
 def _to_hex(arg: str):
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/cosign_transaction.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/cosign_transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 from typing import Dict, Any, Protocol
 from multiversx_sdk_cli.errors import GuardianServiceError
 
 
 class ITransaction(Protocol):
-    guardianSignature: str
+    guardian_signature: str
 
     def to_dictionary(self) -> Dict[str, Any]:
         ...
 
 
 def cosign_transaction(transaction: ITransaction, service_url: str, guardian_code: str) -> ITransaction:
     payload = {
@@ -17,15 +17,15 @@
     }
 
     url = f"{service_url}/sign-transaction"
     response = requests.post(url, json=payload)
     check_for_guardian_error(response.json())
 
     tx_as_dict = response.json()["data"]["transaction"]
-    transaction.guardianSignature = tx_as_dict["guardianSignature"]
+    transaction.guardian_signature = tx_as_dict["guardianSignature"]
 
     return transaction
 
 
 def check_for_guardian_error(response: Dict[str, Any]):
     error = response["error"]
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/diskcache.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/diskcache.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/dns.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     contract = SmartContract(dns_address)
     contract.query(proxy, "validateName", [name_arg])
 
 
 def register(args: Any):
     args = utils.as_object(args)
 
-    cli_shared.check_guardian_and_options_args(args)
+    cli_shared.check_guardian_args(args)
     cli_shared.check_broadcast_args(args)
     cli_shared.prepare_nonce_in_args(args)
     args.receiver = dns_address_for_name(args.name).bech32()
     args.data = dns_register_data(args.name)
 
     tx = do_prepare_transaction(args)
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/docker.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/docker.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/downloader.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         chunk_number = 0
         progress = 0
         with open(filename, 'wb') as file:
             for chunk in response.iter_content(chunk_size=CHUNK_SIZE):
                 file.write(chunk)
                 progress = _report_download_progress(progress, chunk_number, total_size)
                 chunk_number += 1
+            file.flush()
         print('', file=sys.stderr)
         sys.stderr.flush()
     except requests.HTTPError as err:
         raise errors.DownloadError(
             f"Could not download [{url}] to [{filename}]") from err
 
     logger.info("Download done.")
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/errors.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,19 +166,14 @@
 
 
 class NoWalletProvided(KnownError):
     def __init__(self):
         super().__init__("No wallet provided.")
 
 
-class TestnetError(KnownError):
-    def __init__(self, message: str):
-        super().__init__(message)
-
-
 class LedgerError(KnownError):
     def __init__(self, message: str):
         super().__init__("Ledger error: " + message)
 
 
 class DockerMissingError(KnownError):
     def __init__(self):
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/guards.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/guards.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/interfaces.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/myprocess.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/myprocess.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/simulation.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/simulation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/transactions.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/transactions.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import logging
 import time
 from collections import OrderedDict
 from typing import Any, Dict, List, Protocol, Sequence, TextIO, Tuple
 
 from multiversx_sdk_cli import config, errors, utils
 from multiversx_sdk_cli.accounts import Account, Address, LedgerAccount
-from multiversx_sdk_cli.cli_password import load_password, load_guardian_password
-from multiversx_sdk_cli.errors import NoWalletProvided
+from multiversx_sdk_cli.cli_password import load_password
 from multiversx_sdk_cli.interfaces import ITransaction
 from multiversx_sdk_cli.cosign_transaction import cosign_transaction
-from multiversx_sdk_cli.ledger.ledger_functions import do_get_ledger_address
 
 logger = logging.getLogger("transactions")
 
 
 class ITransactionOnNetwork(Protocol):
     hash: str
     is_completed: bool
@@ -48,15 +46,15 @@
         self.gasLimit = 0
         self.data: str = ""
         self.chainID = ""
         self.version = 0
         self.options = 0
         self.signature = ""
         self.guardian = ""
-        self.guardianSignature = ""
+        self.guardian_signature = ""
 
     # The data field is base64-encoded. Here, we only support utf-8 "data" at this moment.
     def data_encoded(self) -> str:
         return self._field_encoded("data")
 
     # Useful when loading a tx from a file (when data is already encoded in base64)
     def data_decoded(self) -> str:
@@ -178,22 +176,22 @@
 
         if self.version:
             dictionary["version"] = int(self.version)
 
         if self.options:
             dictionary["options"] = int(self.options)
 
-        if self.guardian:
-            dictionary["guardian"] = self.guardian
-
         if self.signature:
             dictionary["signature"] = self.signature
 
-        if self.guardianSignature:
-            dictionary["guardianSignature"] = self.guardianSignature
+        if self.guardian:
+            dictionary["guardian"] = self.guardian
+
+        if self.guardian_signature:
+            dictionary["guardianSignature"] = self.guardian_signature
 
         return dictionary
 
     # Creates the payload for a "user" / "inner" transaction
     def to_dictionary_as_inner(self) -> Dict[str, Any]:
         dictionary = self.to_dictionary()
         dictionary["receiver"] = base64.b64encode(Address(self.receiver).pubkey()).decode()
@@ -277,46 +275,12 @@
     tx.data = args.data
     tx.chainID = args.chain
     tx.version = int(args.version)
     tx.options = int(args.options)
     tx.guardian = args.guardian
 
     tx.sign(account)
-    tx = sign_tx_by_guardian(args, tx)
 
-    return tx
-
-
-def sign_tx_by_guardian(args: Any, tx: Transaction) -> Transaction:
-    try:
-        guardian_account = get_guardian_account_from_args(args)
-    except NoWalletProvided:
-        guardian_account = None
-
-    # empty sender signature
-    sender_signature = tx.signature
-    tx.signature = ""
-
-    if guardian_account:
-        tx.guardianSignature = guardian_account.sign_transaction(tx)
-    elif args.guardian:
-        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)  # type: ignore
-
-    tx.signature = sender_signature
+    if args.guardian:
+        tx = cosign_transaction(tx, args.guardian_service_url, args.guardian_2fa_code)
 
     return tx
-
-
-# TODO: this is duplicated code; a proper refactoring will come later
-def get_guardian_account_from_args(args: Any):
-    if args.guardian_pem:
-        account = Account(pem_file=args.guardian_pem, pem_index=args.guardian_pem_index)
-    elif args.guardian_keyfile:
-        password = load_guardian_password(args)
-        account = Account(key_file=args.guardian_keyfile, password=password)
-    elif args.guardian_ledger:
-        address = do_get_ledger_address(account_index=args.guardian_ledger_account_index, address_index=args.guardian_ledger_address_index)
-        account = Account(address=address)
-    else:
-        raise errors.NoWalletProvided()
-
-    return account
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/utils.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,30 +103,30 @@
 
 
 def write_file(file_path: Path, text: str):
     with open(file_path, "w") as file:
         return file.write(text)
 
 
-def read_toml_file(filename):
+def read_toml_file(filename: Union[str, Path]):
     return toml.load(str(filename))
 
 
-def write_toml_file(filename, data):
+def write_toml_file(filename: Union[str, Path], data: Any):
     with open(str(filename), "w") as f:
         toml.dump(data, f)
 
 
 def read_json_file(filename: Union[str, Path]) -> Any:
     with open(filename) as f:
         return json.load(f)
 
 
-def write_json_file(filename: str, data: Any):
-    with open(filename, "w") as f:
+def write_json_file(filename: Union[str, Path], data: Any):
+    with open(str(filename), "w") as f:
         json.dump(data, f, indent=4)
 
 
 def dump_out_json(data: Any, outfile: Any = None):
     if not outfile:
         outfile = sys.stdout
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/version.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/version.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/delegation/__init__.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/delegation/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/delegation/staking_provider.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/delegation/staking_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/dependencies/install.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/install.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/dependencies/modules.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/dependencies/modules.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,18 @@
     def install(self, tag: str, overwrite: bool) -> None:
         # Fallback to default tag if not provided
         tag = tag or config.get_dependency_tag(self.key)
 
         if tag == 'latest':
             tag = self.get_latest_release()
 
-        logger.debug(f"install: key={self.key}, tag={tag}")
+        logger.info(f"install: key={self.key}, tag={tag}, overwrite={overwrite}")
 
         if self._should_skip(tag, overwrite):
-            logger.debug("Already exists. Skip install.")
+            logger.info("Already exists. Skip install.")
             return
 
         self._guard_cannot_install_on_host()
         self.uninstall(tag)
         self._do_install(tag)
 
         self._post_install(tag)
@@ -229,26 +229,31 @@
             return {
                 "PATH": os.environ.get("PATH", ""),
                 "GOPATH": os.environ.get("GOPATH", ""),
                 "GOCACHE": os.environ.get("GOCACHE", ""),
                 "GOROOT": os.environ.get("GOROOT", "")
             }
         if resolution == DependencyResolution.SDK:
+            current_path = os.environ.get("PATH", "")
+            current_path_parts = current_path.split(":")
+            current_path_parts_without_go = [part for part in current_path_parts if "/go/bin" not in part]
+            current_path_without_go = ":".join(current_path_parts_without_go)
+
             return {
                 # At this moment, cc (build-essential) is needed to compile go dependencies (e.g. Node, VM)
-                "PATH": f"{(directory / 'go' / 'bin')}:{os.environ['PATH']}",
-                "GOPATH": self.get_gopath(),
+                "PATH": f"{(directory / 'go' / 'bin')}:{current_path_without_go}",
+                "GOPATH": str(self.get_gopath()),
                 "GOCACHE": str(parent_directory / "GOCACHE"),
                 "GOROOT": str(directory / "go")
             }
 
         raise errors.BadDependencyResolution(self.key, resolution)
 
-    def get_gopath(self):
-        return path.join(self.get_parent_directory(), "GOPATH")
+    def get_gopath(self) -> Path:
+        return self.get_parent_directory() / "GOPATH"
 
     def get_latest_release(self) -> str:
         raise errors.UnsupportedConfigurationValue("Golang tag must always be explicit, not latest")
 
 
 class Rust(DependencyModule):
     def _do_install(self, tag: str) -> None:
@@ -264,25 +269,22 @@
             toolchain = "nightly"
 
         args = [str(installer_path), "--verbose", "--default-toolchain", toolchain, "--profile",
                 "minimal", "--target", "wasm32-unknown-unknown", "--no-modify-path", "-y"]
         myprocess.run_process(args, env=self.get_env_for_install())
 
     def _get_installer_url(self) -> str:
-        platform = workstation.get_platform()
-
-        if platform == "windows":
+        if workstation.is_windows():
             return "https://win.rustup.rs"
         return "https://sh.rustup.rs"
 
     def _get_installer_path(self) -> Path:
-        platform = workstation.get_platform()
         tools_folder = workstation.get_tools_folder()
 
-        if platform == "windows":
+        if workstation.is_windows():
             return tools_folder / "rustup-init.exe"
         return tools_folder / "rustup.sh"
 
     def uninstall(self, tag: str):
         directory = self.get_directory("")
         if os.path.isdir(directory):
             shutil.rmtree(directory)
@@ -338,24 +340,23 @@
             "PATH": str(directory / "bin"),
             "RUSTUP_HOME": str(directory),
             "CARGO_HOME": str(directory)
         }
 
     def get_env_for_install(self):
         directory = self.get_directory("")
-        platform = workstation.get_platform()
 
         env = {
             # For installation, wget (or curl) and cc (build-essential) are also required.
             "PATH": f"{path.join(directory, 'bin')}:{os.environ['PATH']}",
             "RUSTUP_HOME": str(directory),
             "CARGO_HOME": str(directory)
         }
 
-        if platform == "windows":
+        if workstation.is_windows():
             env["RUSTUP_USE_HYPER"] = "1"
 
         return env
 
     def get_latest_release(self) -> str:
         raise errors.UnsupportedConfigurationValue("Rust tag must either be explicit, empty or 'nightly'")
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/ledger/config.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/ledger/ledger_app_handler.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/ledger_app_handler.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/ledger/ledger_functions.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/ledger/ledger_functions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/__init__.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/core.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/migrations.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/migrations.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/project_base.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from abc import abstractmethod
 from os import path
 from pathlib import Path
 from typing import Any, Dict, List, Union, cast, final
 
 from multiversx_sdk_cli import dependencies, errors, myprocess, utils
 from multiversx_sdk_cli.dependencies.modules import StandaloneModule
-from multiversx_sdk_cli.projects import eei_checks
 from multiversx_sdk_cli.projects.constants import PROJECT_CONFIG_FILENAME
 from multiversx_sdk_cli.projects.interfaces import IProject
 from multiversx_sdk_cli.projects.migrations import migrate_project_config_file
 
 logger = logging.getLogger("Project")
 
 
@@ -79,16 +78,15 @@
 
     @abstractmethod
     def _do_after_build_custom(self) -> List[Path]:
         raise NotImplementedError()
 
     @final
     def _do_after_build_core(self):
-        # TODO: Remove this, in the future
-        eei_checks.check_compatibility(self)
+        pass
 
     def _copy_to_output(self, source: Path, destination: Union[str, None] = None) -> Path:
         output_folder = self.get_output_folder()
         utils.ensure_folder(output_folder)
         destination = path.join(output_folder, destination) if destination else output_folder
         output_wasm_file = shutil.copy(str(source), destination)
         return Path(output_wasm_file)
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/project_clang.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_clang.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/project_cpp.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_cpp.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/project_rust.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/project_rust.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/shared.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/shared.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/templates.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/templates_config.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/templates_repository.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/templates_repository.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/do_report.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/do_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/report_creator.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/report_creator.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/common.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/common.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/extracted_feature.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/folder_report.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/folder_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/project_report.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/project_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/report.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/data/wasm_report.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/data/wasm_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/features/report_option.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/report_option.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/projects/report/format/change_type.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/projects/report/format/change_type.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/genesis.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from multiversx_sdk_cli.accounts import Address
 from multiversx_sdk_cli.contracts import SmartContract
-from multiversx_sdk_cli.testnet import wallets
+from multiversx_sdk_cli.localnet import wallets
 
 
 def get_owner_of_genesis_contracts():
     users = wallets.get_users()
     return users["alice"]
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/genesis_json.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/genesis_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import Any, List
+from typing import Any, Dict, List
 
 from multiversx_sdk_cli.accounts import Account, Address
-from multiversx_sdk_cli.testnet import wallets
-from multiversx_sdk_cli.testnet.config import TestnetConfiguration
-from multiversx_sdk_cli.testnet.genesis import (get_delegation_address,
-                                   is_foundational_node, is_last_user)
+from multiversx_sdk_cli.localnet import wallets
+from multiversx_sdk_cli.localnet.config_root import ConfigRoot
+from multiversx_sdk_cli.localnet.genesis import (get_delegation_address,
+                                                 is_foundational_node,
+                                                 is_last_user)
 
 ENTIRE_SUPPLY = 20000000000000000000000000
-# For testnet, we delegate for 1 node
+# For localnet, we delegate for 1 node
 DELEGATED_VALUE = 2500000000000000000000
 
 
-def build(testnet_config: TestnetConfiguration) -> List[Any]:
-    num_validators = testnet_config.num_all_validators()
-    genesis_items = []
+def build(config: ConfigRoot) -> List[Any]:
+    num_validators = config.num_all_validators()
+    genesis_items: List[Dict[str, Any]] = []
     remaining_supply = ENTIRE_SUPPLY
     remaining_to_delegate = DELEGATED_VALUE
     delegation_address = get_delegation_address()
 
     for nickname, account in wallets.get_validator_wallets(num_validators).items():
         if is_foundational_node(nickname):
             continue
@@ -35,29 +36,29 @@
         genesis_items.append(entry)
         remaining_supply -= value
         remaining_to_delegate -= delegated_value
 
     return genesis_items
 
 
-def _build_validator_entry(nickname: str, account: Account, value: int):
+def _build_validator_entry(nickname: str, account: Account, value: int) -> Dict[str, Any]:
     return {
         "nickname": nickname,
         "address": account.address.bech32(),
         "supply": str(value),
         "balance": "0",
         "stakingvalue": str(value),
         "delegation": {
             "address": "",
             "value": "0"
         }
     }
 
 
-def _build_user_entry(nickname: str, account: Account, value: int, delegated_value: int, delegation_address: Address):
+def _build_user_entry(nickname: str, account: Account, value: int, delegated_value: int, delegation_address: Address) -> Dict[str, Any]:
     return {
         "nickname": nickname,
         "address": account.address.bech32(),
         "supply": str(value),
         "balance": str(value - delegated_value),
         "stakingvalue": "0",
         "delegation": {
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/nodes_setup_json.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/nodes_setup_json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-from typing import Any
+from typing import Any, Dict, List
 
 from multiversx_sdk_cli.accounts import Account
-from multiversx_sdk_cli.testnet import wallets
-from multiversx_sdk_cli.testnet.config import TestnetConfiguration
-from multiversx_sdk_cli.testnet.genesis import get_delegation_address, is_foundational_node
+from multiversx_sdk_cli.localnet import wallets
+from multiversx_sdk_cli.localnet.config_root import ConfigRoot
+from multiversx_sdk_cli.localnet.genesis import (get_delegation_address,
+                                                 is_foundational_node)
 
-CHAIN_ID = "local-testnet"
+CHAIN_ID = "localnet"
 
 
-def build(testnet_config: TestnetConfiguration) -> Any:
-    num_validators = testnet_config.num_all_validators()
-    initial_nodes = []
+def build(config: ConfigRoot) -> Any:
+    num_validators = config.num_all_validators()
+    initial_nodes: List[Dict[str, str]] = []
 
     for nickname, [pubkey, account] in wallets.get_validators(num_validators).items():
         entry = _build_initial_nodes_entry(nickname, pubkey, account)
         initial_nodes.append(entry)
 
     # Then, patch the list of initial nodes, so that higher indexes will become metachain nodes.
-    num_metachain_nodes = testnet_config.num_validators_in_metashard()
+    num_metachain_nodes = config.metashard.num_validators
     num_nodes = len(initial_nodes)
     initial_nodes = initial_nodes[num_nodes - num_metachain_nodes:] + initial_nodes[:num_nodes - num_metachain_nodes]
 
     return {
-        "startTime": testnet_config.genesis_time(),
-        "roundDuration": 6000,
-        "consensusGroupSize": testnet_config.shards["consensus_size"],
-        "minNodesPerShard": testnet_config.shards["consensus_size"],
-        "metaChainConsensusGroupSize": testnet_config.metashard["consensus_size"],
-        "metaChainMinNodes": testnet_config.metashard["validators"],
+        "startTime": config.genesis_time(),
+        "roundDuration": config.general.round_duration_milliseconds,
+        "consensusGroupSize": config.shards.consensus_size,
+        "minNodesPerShard": config.shards.consensus_size,
+        "metaChainConsensusGroupSize": config.metashard.consensus_size,
+        "metaChainMinNodes": config.metashard.num_validators,
         "hysteresis": 0,
         "adaptivity": False,
         "chainID": CHAIN_ID,
         "minTransactionVersion": 1,
         "initialNodes": initial_nodes
     }
 
 
-def _build_initial_nodes_entry(nickname: str, pubkey: str, account: Account) -> Any:
+def _build_initial_nodes_entry(nickname: str, pubkey: str, account: Account) -> Dict[str, str]:
     address = get_delegation_address().bech32() if is_foundational_node(nickname) else account.address.bech32()
 
     return {
         "nickname": nickname,
         "address": address,
         "pubkey": pubkey,
     }
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/testnet/wallets.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/localnet/wallets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import shutil
 from collections import OrderedDict
 from pathlib import Path
 from typing import Dict, Tuple
 
+from multiversx_sdk_wallet.validator_pem import ValidatorPEM
+
 from multiversx_sdk_cli import errors, utils
 from multiversx_sdk_cli.accounts import Account
-from multiversx_sdk_wallet.validator_pem import ValidatorPEM
 from multiversx_sdk_cli.workstation import get_tools_folder
 
 MAX_NUM_NODES = 12
 
 
 def copy_all_to(destination: str):
     shutil.copytree(_get_folder(), destination)
@@ -26,49 +27,49 @@
 
 def get_observer_key_file(observer_index: int):
     _guard_validator_index(observer_index)
     return _get_observers_folder().joinpath("observerKey{:02}.pem".format(observer_index))
 
 
 def get_validator_wallets(num_validators: int) -> Dict[str, Account]:
-    result = {}
+    result: Dict[str, Account] = {}
 
     for i in range(0, num_validators):
         pem_file = get_validator_wallet_file(i)
         nickname = "validator{:02}".format(i)
-        account = Account(pem_file=pem_file)
+        account = Account(pem_file=str(pem_file))
         result[nickname] = account
 
     return result
 
 
 def get_validators(num_validators: int) -> Dict[str, Tuple[str, Account]]:
-    result = {}
+    result: Dict[str, Tuple[str, Account]] = {}
 
     for i in range(0, num_validators):
         validator_pem_file = get_validator_key_file(i)
         pem_from_file = ValidatorPEM.from_file(validator_pem_file)
         pubkey = pem_from_file.label
 
         pem_file = get_validator_wallet_file(i)
         nickname = "validator{:02}".format(i)
-        account = Account(pem_file=pem_file)
+        account = Account(pem_file=str(pem_file))
         result[nickname] = (pubkey, account)
 
     return result
 
 
 def get_validator_wallet_file(validator_index: int):
     _guard_validator_index(validator_index)
     return _get_validators_folder().joinpath("wallet{:02}.pem".format(validator_index))
 
 
 def _guard_validator_index(validator_index: int):
     if validator_index >= MAX_NUM_NODES:
-        raise errors.TestnetError(f"Invalid validator index: {validator_index} >= {MAX_NUM_NODES}.")
+        raise errors.KnownError(f"Invalid validator index: {validator_index} >= {MAX_NUM_NODES}.")
 
 
 def _get_validators_folder():
     return _get_folder().joinpath("validators")
 
 
 def _get_observers_folder():
@@ -87,8 +88,8 @@
 
 
 def _get_users_folder():
     return _get_folder().joinpath("users")
 
 
 def _get_folder():
-    return get_tools_folder() / "testwallets" / "latest" 
+    return get_tools_folder() / "testwallets" / "latest"
```

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/validators/__init__.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/validators/core.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/multiversx_sdk_cli/validators/validators_file.py` & `multiversx_sdk_cli-7.0.0b0/multiversx_sdk_cli/validators/validators_file.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/LICENSE` & `multiversx_sdk_cli-7.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/README.md` & `multiversx_sdk_cli-7.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-6.5.0/pyproject.toml` & `multiversx_sdk_cli-7.0.0b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-cli"
-version = "6.5.0"
+version = "7.0.0b0"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "MultiversX Smart Contracts Tools"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -21,16 +21,17 @@
 dependencies = [
   "toml>=0.10.2",
   "requests",
   "prettytable",
   "ledgercomm[hid]",
   "semver",
   "requests-cache",
+  "rich==13.3.4",
   "multiversx-sdk-network-providers==0.6.*",
-  "multiversx-sdk-wallet==0.7.*",
+  "multiversx-sdk-wallet==0.6.*",
   "multiversx-sdk-core>=0.4.1"
 ]
 
 [tool.hatch.build]
 include = [
   "multiversx_sdk_cli/**"
 ]
```

### Comparing `multiversx_sdk_cli-6.5.0/PKG-INFO` & `multiversx_sdk_cli-7.0.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-cli
-Version: 6.5.0
+Version: 7.0.0b0
 Summary: MultiversX Smart Contracts Tools
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-cli
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: ledgercomm[hid]
 Requires-Dist: multiversx-sdk-core>=0.4.1
 Requires-Dist: multiversx-sdk-network-providers==0.6.*
-Requires-Dist: multiversx-sdk-wallet==0.7.*
+Requires-Dist: multiversx-sdk-wallet==0.6.*
 Requires-Dist: prettytable
 Requires-Dist: requests
 Requires-Dist: requests-cache
+Requires-Dist: rich==13.3.4
 Requires-Dist: semver
 Requires-Dist: toml>=0.10.2
 Description-Content-Type: text/markdown
 
 # Description
 Python Command Line Tools for interacting with Multivers<sup>X</sup>.
```

