# Comparing `tmp/pytorchrl-3.2.13.tar.gz` & `tmp/pytorchrl-3.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorchrl-3.2.13.tar", last modified: Fri Jun  9 12:17:18 2023, max compression
+gzip compressed data, was "pytorchrl-3.2.14.tar", last modified: Mon Jun 12 15:25:09 2023, max compression
```

## Comparing `pytorchrl-3.2.13.tar` & `pytorchrl-3.2.14.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.309336 pytorchrl-3.2.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 12:17:04.000000 pytorchrl-3.2.13/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 12:17:04.000000 pytorchrl-3.2.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-09 12:17:18.309336 pytorchrl-3.2.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-09 12:17:04.000000 pytorchrl-3.2.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.273334 pytorchrl-3.2.13/pytorchrl/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.273334 pytorchrl-3.2.13/pytorchrl/agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.273334 pytorchrl-3.2.13/pytorchrl/agent/actors/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.273334 pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/squashed_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.277334 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/dictnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/ensemble_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/fixup_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.277334 pytorchrl-3.2.13/pytorchrl/agent/actors/memory_networks/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/memory_networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/memory_networks/gru_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/memory_networks/lstm_encoder_decoder_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/memory_networks/lstm_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/model_based_planner_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.277334 pytorchrl-3.2.13/pytorchrl/agent/actors/noise/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/noise/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/noise/nonoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/noise/ou.py
--rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/off_policy_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18095 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/on_policy_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.281334 pytorchrl-3.2.13/pytorchrl/agent/actors/reward_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/reward_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/reward_functions/gym_reward_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/reward_functions/pybullet_reward_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.281334 pytorchrl-3.2.13/pytorchrl/agent/actors/world_models/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/world_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/world_models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/actors/world_models/world_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.281334 pytorchrl-3.2.13/pytorchrl/agent/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.281334 pytorchrl-3.2.13/pytorchrl/agent/algorithms/model_based/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/model_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/model_based/mpc_cem.py
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/model_based/mpc_pddm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/model_based/mpc_rs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.281334 pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/ddpg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/ddqn.py
--rw-r--r--   0 runner    (1001) docker     (123)    32877 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/mpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24981 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/sac.py
--rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/td3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.281334 pytorchrl-3.2.13/pytorchrl/agent/algorithms/on_policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/on_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/on_policy/a2c.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/on_policy/ppo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/on_policy/rnd_ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.285335 pytorchrl-3.2.13/pytorchrl/agent/algorithms/policy_loss_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/policy_loss_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/policy_loss_addons/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/policy_loss_addons/kv_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/policy_loss_addons/return_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/policy_loss_addons/reward_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/algorithms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.285335 pytorchrl-3.2.13/pytorchrl/agent/env/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.285335 pytorchrl-3.2.13/pytorchrl/agent/env/base_envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/base_envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/base_envs/batched_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/base_envs/env_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.285335 pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/parallel_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/sequential_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/vec_env_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/vec_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/vector_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.289335 pytorchrl-3.2.13/pytorchrl/agent/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.289335 pytorchrl-3.2.13/pytorchrl/agent/storages/model_based/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/model_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/model_based/mb_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.289335 pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/ere_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/her_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/nstep_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/per_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/replay_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.289335 pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/gae_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/ppod2_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19127 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/ppod2rebel_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28310 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/ppod_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/vanilla_on_policy_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/vtrace_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.293335 pytorchrl-3.2.13/pytorchrl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.293335 pytorchrl-3.2.13/pytorchrl/envs/animal_olympics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/animal_olympics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/animal_olympics/animal_olympics_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/animal_olympics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/animal_olympics/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.293335 pytorchrl-3.2.13/pytorchrl/envs/atari/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/atari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/atari/atari_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/atari/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/atari/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.293335 pytorchrl-3.2.13/pytorchrl/envs/causal_world/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/causal_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/causal_world/causal_world_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.293335 pytorchrl-3.2.13/pytorchrl/envs/crafter/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/crafter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/crafter/crafter_env_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.293335 pytorchrl-3.2.13/pytorchrl/envs/dm_control/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/dm_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/dm_control/dmcontrol_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/dm_control/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.297335 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.297335 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/diversity_filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/diversity_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/diversity_filter/base_diversity_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/diversity_filter/diversity_filter_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/diversity_filter/no_filter_with_penalty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.297335 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/batched_rnn_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/generative_chemistry_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/rnn_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.297335 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/reinvent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/reinvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/reinvent/generative_chemistry_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/reinvent/rnn_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/reinvent/transformer_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.301336 pytorchrl-3.2.13/pytorchrl/envs/habitat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/habitat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/habitat/habitat_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/habitat/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/habitat/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.301336 pytorchrl-3.2.13/pytorchrl/envs/minigrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/minigrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.301336 pytorchrl-3.2.13/pytorchrl/envs/minigrid/custom_environments/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/minigrid/custom_environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/minigrid/custom_environments/deceiving_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/minigrid/custom_environments/multiple_deceiving_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/minigrid/minigrid_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/minigrid/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.301336 pytorchrl-3.2.13/pytorchrl/envs/mujoco/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/mujoco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/mujoco/mujoco_env_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.301336 pytorchrl-3.2.13/pytorchrl/envs/obstacle_tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/obstacle_tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/obstacle_tower/obstacle_tower_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/obstacle_tower/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/obstacle_tower/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.305336 pytorchrl-3.2.13/pytorchrl/envs/pybullet/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/pybullet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/pybullet/pybullet_env_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/envs/pybullet/sparse_reacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.305336 pytorchrl-3.2.13/pytorchrl/scheme/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.305336 pytorchrl-3.2.13/pytorchrl/scheme/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/base/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/base/worker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.305336 pytorchrl-3.2.13/pytorchrl/scheme/collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/collection/c_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/collection/c_worker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.305336 pytorchrl-3.2.13/pytorchrl/scheme/gradients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/gradients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21056 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/gradients/g_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/gradients/g_worker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.309336 pytorchrl-3.2.13/pytorchrl/scheme/updates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/updates/u_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/scheme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/pytorchrl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:17:18.273334 pytorchrl-3.2.13/pytorchrl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-09 12:17:18.000000 pytorchrl-3.2.13/pytorchrl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-09 12:17:18.000000 pytorchrl-3.2.13/pytorchrl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:17:18.000000 pytorchrl-3.2.13/pytorchrl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 12:17:18.000000 pytorchrl-3.2.13/pytorchrl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 12:17:18.000000 pytorchrl-3.2.13/pytorchrl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:17:18.309336 pytorchrl-3.2.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-09 12:17:05.000000 pytorchrl-3.2.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-12 15:24:56.000000 pytorchrl-3.2.14/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 15:24:56.000000 pytorchrl-3.2.14/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-12 15:24:56.000000 pytorchrl-3.2.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.254197 pytorchrl-3.2.14/pytorchrl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.254197 pytorchrl-3.2.14/pytorchrl/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.254197 pytorchrl-3.2.14/pytorchrl/agent/actors/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.254197 pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/squashed_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.254197 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/dictnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/ensemble_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/fixup_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/actors/memory_networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/memory_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/memory_networks/gru_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/memory_networks/lstm_encoder_decoder_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/memory_networks/lstm_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/model_based_planner_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/actors/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/noise/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/noise/nonoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/noise/ou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/off_policy_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18095 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/on_policy_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/actors/reward_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/reward_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/reward_functions/gym_reward_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/reward_functions/pybullet_reward_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/actors/world_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/world_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/world_models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/actors/world_models/world_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/algorithms/model_based/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/model_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/model_based/mpc_cem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/model_based/mpc_pddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/model_based/mpc_rs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/ddpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/ddqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32877 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/mpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24981 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/td3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/algorithms/on_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/on_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/on_policy/a2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/on_policy/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/on_policy/rnd_ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/algorithms/policy_loss_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/policy_loss_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/policy_loss_addons/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/policy_loss_addons/kv_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/policy_loss_addons/return_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/policy_loss_addons/reward_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/algorithms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/env/base_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/base_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/base_envs/batched_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/base_envs/env_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/parallel_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/sequential_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/vec_env_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/vec_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/vector_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.258197 pytorchrl-3.2.14/pytorchrl/agent/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/agent/storages/model_based/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/model_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/model_based/mb_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/ere_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/her_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/nstep_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/per_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/replay_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/gae_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/ppod2_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19127 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/ppod2rebel_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28310 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/ppod_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/vanilla_on_policy_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/vtrace_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/animal_olympics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/animal_olympics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/animal_olympics/animal_olympics_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/animal_olympics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/animal_olympics/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/atari/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/atari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/atari/atari_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/atari/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/atari/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/causal_world/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/causal_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/causal_world/causal_world_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/crafter/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/crafter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/crafter/crafter_env_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/dm_control/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/dm_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/dm_control/dmcontrol_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/dm_control/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/diversity_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/diversity_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/diversity_filter/base_diversity_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/diversity_filter/diversity_filter_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/diversity_filter/no_filter_with_penalty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/batched_rnn_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/generative_chemistry_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/rnn_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.262197 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/reinvent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/reinvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/reinvent/generative_chemistry_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/reinvent/rnn_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/reinvent/transformer_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/envs/habitat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/habitat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/habitat/habitat_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/habitat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/habitat/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/envs/minigrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/minigrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/envs/minigrid/custom_environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/minigrid/custom_environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/minigrid/custom_environments/deceiving_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/minigrid/custom_environments/multiple_deceiving_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/minigrid/minigrid_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/minigrid/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/envs/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/mujoco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/mujoco/mujoco_env_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/envs/obstacle_tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/obstacle_tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/obstacle_tower/obstacle_tower_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/obstacle_tower/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/obstacle_tower/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/envs/pybullet/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/pybullet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/pybullet/pybullet_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/envs/pybullet/sparse_reacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/scheme/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/base/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/base/worker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/scheme/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/collection/c_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/collection/c_worker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/scheme/gradients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/gradients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21056 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/gradients/g_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/gradients/g_worker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/pytorchrl/scheme/updates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/updates/u_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/scheme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/pytorchrl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:25:09.254197 pytorchrl-3.2.14/pytorchrl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 15:25:09.000000 pytorchrl-3.2.14/pytorchrl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-12 15:25:09.000000 pytorchrl-3.2.14/pytorchrl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:25:09.000000 pytorchrl-3.2.14/pytorchrl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 15:25:09.000000 pytorchrl-3.2.14/pytorchrl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 15:25:09.000000 pytorchrl-3.2.14/pytorchrl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:25:09.266197 pytorchrl-3.2.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-12 15:24:57.000000 pytorchrl-3.2.14/setup.py
```

### Comparing `pytorchrl-3.2.13/LICENCE` & `pytorchrl-3.2.14/LICENCE`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/PKG-INFO` & `pytorchrl-3.2.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorchrl
-Version: 3.2.13
+Version: 3.2.14
 Summary: Disributed RL implementations with ray and pytorch.
 Home-page: https://github.com/PyTorchRL/pytorchrl/
 Author: albertbou92
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytorchrl-3.2.13/README.md` & `pytorchrl-3.2.14/README.md`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/__init__.py` & `pytorchrl-3.2.14/pytorchrl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.2.11"
+__version__ = "3.2.14"
 
 from collections import namedtuple
 
 __all__ = [
     "ALGORITHM", "EPISODES", "SCHEME", "TIME", "INFO_KEYS",
     "COLLECTION", "GRADIENT", "UPDATE", "OP_KEYS",
     "VERSION", "WEIGHTS", "NUMSAMPLES",
```

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/base.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/base.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/__init__.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/categorical.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/categorical.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/deterministic.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/gaussian.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/gaussian.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/distributions/squashed_gaussian.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/distributions/squashed_gaussian.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/__init__.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/cnn.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/cnn.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/dictnet.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/dictnet.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/embedding.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/embedding.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/ensemble_layer.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/ensemble_layer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/fixup_cnn.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/fixup_cnn.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/gpt.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/gpt.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/feature_extractors/mlp.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/feature_extractors/mlp.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/memory_networks/__init__.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/memory_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/memory_networks/gru_net.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/memory_networks/gru_net.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/memory_networks/lstm_encoder_decoder_net.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/memory_networks/lstm_encoder_decoder_net.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/memory_networks/lstm_net.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/memory_networks/lstm_net.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/model_based_planner_actor.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/model_based_planner_actor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/noise/ou.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/noise/ou.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/off_policy_actor.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/off_policy_actor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/on_policy_actor.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/on_policy_actor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/reward_functions/__init__.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/reward_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/reward_functions/gym_reward_functions.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/reward_functions/gym_reward_functions.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/reward_functions/pybullet_reward_functions.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/reward_functions/pybullet_reward_functions.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/utils.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/world_models/utils.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/world_models/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/actors/world_models/world_model.py` & `pytorchrl-3.2.14/pytorchrl/agent/actors/world_models/world_model.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/__init__.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/base.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/model_based/mpc_cem.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/model_based/mpc_cem.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/model_based/mpc_pddm.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/model_based/mpc_pddm.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/model_based/mpc_rs.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/model_based/mpc_rs.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/ddpg.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/ddpg.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/ddqn.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/ddqn.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/mpo.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/mpo.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/sac.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/sac.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/off_policy/td3.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/off_policy/td3.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/on_policy/a2c.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/on_policy/a2c.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/on_policy/ppo.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/on_policy/ppo.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/on_policy/rnd_ppo.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/on_policy/rnd_ppo.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/policy_loss_addons/kv_similarity.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/policy_loss_addons/kv_similarity.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/policy_loss_addons/return_predictor.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/policy_loss_addons/return_predictor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/policy_loss_addons/reward_predictor.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/policy_loss_addons/reward_predictor.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/algorithms/utils.py` & `pytorchrl-3.2.14/pytorchrl/agent/algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/env/base_envs/batched_env.py` & `pytorchrl-3.2.14/pytorchrl/agent/env/base_envs/batched_env.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/env/base_envs/env_wrappers.py` & `pytorchrl-3.2.14/pytorchrl/agent/env/base_envs/env_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,21 @@
                     ob[k] = ob[k].transpose(self.op[0], self.op[1], self.op[2])
         else:
             if len(ob.shape) == 3:
                 ob = ob.transpose(self.op[0], self.op[1], self.op[2])
 
         return ob
 
+    def step(self, action):
+        obs, reward, done, info = self.env.step(action)
+        return self.observation(obs), reward, done, info
+
+    def reset(self):
+        return self.observation(self.env.reset())
+
 
 class PyTorchEnv(gym.Wrapper):
     """
     This wrapper turns obs, reward's and done's from numpy arrays to pytorch
     tensors and places them in the specified device, facilitating interaction
     between the environment and the actor critic function approximators (NNs).
 
@@ -132,15 +139,15 @@
 
     def __init__(self, env, filename, info_keywords=()):
         super(Monitor, self).__init__(env)
         self.tstart = time.time()
         if filename:
             self.results_writer = ResultsWriter(
                 filename,
-                header={"t_start": time.time(), 'env_id': env.spec and env.spec.id},
+                header={"t_start": time.time()},
                 extra_keys=info_keywords)
         else:
             self.results_writer = None
         self.info_keywords = info_keywords
         self.rewards = None
 
     def reset(self, **kwargs):
@@ -183,15 +190,15 @@
 
     def __init__(self, env, filename, info_keywords=()):
         super(BatchedMonitor, self).__init__(env)
         self.tstart = time.time()
         if filename:
             self.results_writer = ResultsWriter(
                 filename,
-                header={"t_start": time.time(), 'env_id': env.spec and env.spec.id},
+                header={"t_start": time.time()},
                 extra_keys=info_keywords)
         else:
             self.results_writer = None
         self.info_keywords = info_keywords
         self.rewards = None
         self.steps = None
```

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/parallel_vec_env.py` & `pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/parallel_vec_env.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/sequential_vec_env.py` & `pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/sequential_vec_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         obs_space = env.observation_space
         self.keys, shapes, dtypes = obs_space_info(obs_space)
         self.buf_obs = {k: np.zeros((self.num_envs,) + tuple(shapes[k]), dtype=dtypes[k]) for k in self.keys}
         self.buf_dones = np.zeros((self.num_envs,), dtype=bool)
         self.buf_rews = np.zeros((self.num_envs,), dtype=np.float32)
         self.buf_infos = [{} for _ in range(self.num_envs)]
         self.actions = None
-        self.spec = self.envs[0].spec
 
     def step_async(self, actions):
         listify = True
         try:
             if len(actions) == self.num_envs:
                 listify = False
         except TypeError:
```

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/util.py` & `pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/util.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/vec_env_base.py` & `pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/vec_env_base.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/vec_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/vec_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/env/vec_envs/vector_wrappers.py` & `pytorchrl-3.2.14/pytorchrl/agent/env/vec_envs/vector_wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/__init__.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/base.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/base.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/model_based/mb_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/model_based/mb_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/ere_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/ere_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/her_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/her_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/nstep_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/nstep_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/per_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/per_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/off_policy/replay_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/off_policy/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/gae_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/gae_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/ppod2_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/ppod2_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/ppod2rebel_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/ppod2rebel_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/ppod_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/ppod_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/vanilla_on_policy_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/vanilla_on_policy_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/agent/storages/on_policy/vtrace_buffer.py` & `pytorchrl-3.2.14/pytorchrl/agent/storages/on_policy/vtrace_buffer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/animal_olympics/animal_olympics_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/animal_olympics/animal_olympics_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/animal_olympics/utils.py` & `pytorchrl-3.2.14/pytorchrl/envs/animal_olympics/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/animal_olympics/wrappers.py` & `pytorchrl-3.2.14/pytorchrl/envs/animal_olympics/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/atari/atari_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/atari/atari_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/atari/wrappers.py` & `pytorchrl-3.2.14/pytorchrl/envs/atari/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/causal_world/causal_world_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/causal_world/causal_world_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/common.py` & `pytorchrl-3.2.14/pytorchrl/envs/common.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/crafter/crafter_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/crafter/crafter_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/dm_control/dmcontrol_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/dm_control/dmcontrol_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/dm_control/utils.py` & `pytorchrl-3.2.14/pytorchrl/envs/dm_control/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/diversity_filter/base_diversity_filter.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/diversity_filter/base_diversity_filter.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/diversity_filter/diversity_filter_memory.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/diversity_filter/diversity_filter_memory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/diversity_filter/no_filter_with_penalty.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/diversity_filter/no_filter_with_penalty.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/batched_rnn_environment.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/batched_rnn_environment.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/generative_chemistry_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/generative_chemistry_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/rnn_environment.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/rnn_environment.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/libinvent/utils.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/libinvent/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/reinvent/generative_chemistry_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/reinvent/generative_chemistry_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/reinvent/rnn_environment.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/reinvent/rnn_environment.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/reinvent/transformer_environment.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/reinvent/transformer_environment.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/utils.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/generative_chemistry/vocabulary.py` & `pytorchrl-3.2.14/pytorchrl/envs/generative_chemistry/vocabulary.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/habitat/habitat_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/habitat/habitat_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/habitat/utils.py` & `pytorchrl-3.2.14/pytorchrl/envs/habitat/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/habitat/wrappers.py` & `pytorchrl-3.2.14/pytorchrl/envs/habitat/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/minigrid/custom_environments/__init__.py` & `pytorchrl-3.2.14/pytorchrl/envs/minigrid/custom_environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/minigrid/custom_environments/deceiving_rewards.py` & `pytorchrl-3.2.14/pytorchrl/envs/minigrid/custom_environments/deceiving_rewards.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/minigrid/custom_environments/multiple_deceiving_rewards.py` & `pytorchrl-3.2.14/pytorchrl/envs/minigrid/custom_environments/multiple_deceiving_rewards.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/minigrid/minigrid_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/minigrid/minigrid_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/minigrid/wrappers.py` & `pytorchrl-3.2.14/pytorchrl/envs/minigrid/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/mujoco/mujoco_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/mujoco/mujoco_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/obstacle_tower/obstacle_tower_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/obstacle_tower/obstacle_tower_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/obstacle_tower/utils.py` & `pytorchrl-3.2.14/pytorchrl/envs/obstacle_tower/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/obstacle_tower/wrappers.py` & `pytorchrl-3.2.14/pytorchrl/envs/obstacle_tower/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/pybullet/pybullet_env_factory.py` & `pytorchrl-3.2.14/pytorchrl/envs/pybullet/pybullet_env_factory.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/envs/pybullet/sparse_reacher.py` & `pytorchrl-3.2.14/pytorchrl/envs/pybullet/sparse_reacher.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/learner.py` & `pytorchrl-3.2.14/pytorchrl/learner.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/scheme/base/worker.py` & `pytorchrl-3.2.14/pytorchrl/scheme/base/worker.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/scheme/base/worker_set.py` & `pytorchrl-3.2.14/pytorchrl/scheme/base/worker_set.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/scheme/collection/c_worker.py` & `pytorchrl-3.2.14/pytorchrl/scheme/collection/c_worker.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/scheme/collection/c_worker_set.py` & `pytorchrl-3.2.14/pytorchrl/scheme/collection/c_worker_set.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/scheme/gradients/g_worker.py` & `pytorchrl-3.2.14/pytorchrl/scheme/gradients/g_worker.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/scheme/gradients/g_worker_set.py` & `pytorchrl-3.2.14/pytorchrl/scheme/gradients/g_worker_set.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/scheme/scheme.py` & `pytorchrl-3.2.14/pytorchrl/scheme/scheme.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/scheme/updates/u_worker.py` & `pytorchrl-3.2.14/pytorchrl/scheme/updates/u_worker.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/scheme/utils.py` & `pytorchrl-3.2.14/pytorchrl/scheme/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/trainer.py` & `pytorchrl-3.2.14/pytorchrl/trainer.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl/utils.py` & `pytorchrl-3.2.14/pytorchrl/utils.py`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/pytorchrl.egg-info/PKG-INFO` & `pytorchrl-3.2.14/pytorchrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorchrl
-Version: 3.2.13
+Version: 3.2.14
 Summary: Disributed RL implementations with ray and pytorch.
 Home-page: https://github.com/PyTorchRL/pytorchrl/
 Author: albertbou92
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytorchrl-3.2.13/pytorchrl.egg-info/SOURCES.txt` & `pytorchrl-3.2.14/pytorchrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorchrl-3.2.13/setup.py` & `pytorchrl-3.2.14/setup.py`

 * *Files identical despite different names*

